# Comparing `tmp/h5pyd-0.9.1.tar.gz` & `tmp/h5pyd-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5pyd-0.9.1.tar", last modified: Thu Dec 16 17:01:02 2021, max compression
+gzip compressed data, was "h5pyd-0.9.2.tar", last modified: Thu Dec 16 19:07:40 2021, max compression
```

## Comparing `h5pyd-0.9.1.tar` & `h5pyd-0.9.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.702206 h5pyd-0.9.1/
--rw-r--r--   0 john       (501) staff       (20)      813 2021-12-15 01:10:39.000000 h5pyd-0.9.1/.gitignore
--rw-r--r--   0 john       (501) staff       (20)     3315 2021-10-31 18:08:16.000000 h5pyd-0.9.1/.travis.yml
--rwxr-xr-x   0 john       (501) staff       (20)     1779 2021-10-31 18:08:16.000000 h5pyd-0.9.1/COPYING
--rwxr-xr-x   0 john       (501) staff       (20)      467 2021-10-31 18:08:16.000000 h5pyd-0.9.1/Dockerfile
--rw-r--r--   0 john       (501) staff       (20)     3776 2021-12-16 17:01:02.701863 h5pyd-0.9.1/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     2889 2021-10-31 18:08:16.000000 h5pyd-0.9.1/README.rst
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.651600 h5pyd-0.9.1/docs/
--rw-r--r--   0 john       (501) staff       (20)     6755 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/Makefile
--rw-r--r--   0 john       (501) staff       (20)     9040 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/build.rst
--rw-r--r--   0 john       (501) staff       (20)     5906 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/conf.py
--rw-r--r--   0 john       (501) staff       (20)     2942 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/config.rst
--rw-r--r--   0 john       (501) staff       (20)    16441 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/contributing.rst
--rw-r--r--   0 john       (501) staff       (20)    10190 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/faq.rst
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.656741 h5pyd-0.9.1/docs/high/
--rw-r--r--   0 john       (501) staff       (20)     3972 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/high/attr.rst
--rw-r--r--   0 john       (501) staff       (20)    24127 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/high/dataset.rst
--rw-r--r--   0 john       (501) staff       (20)     3729 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/high/dims.rst
--rw-r--r--   0 john       (501) staff       (20)    18276 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/high/file.rst
--rw-r--r--   0 john       (501) staff       (20)    18251 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/high/group.rst
--rw-r--r--   0 john       (501) staff       (20)     1363 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/high/lowlevel.rst
--rw-r--r--   0 john       (501) staff       (20)     1375 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/index.rst
--rw-r--r--   0 john       (501) staff       (20)    11708 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/licenses.rst
--rw-r--r--   0 john       (501) staff       (20)     5131 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/mpi.rst
--rw-r--r--   0 john       (501) staff       (20)     5733 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/quick.rst
--rw-r--r--   0 john       (501) staff       (20)     3985 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/refs.rst
--rw-r--r--   0 john       (501) staff       (20)     1201 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/release_guide.rst
--rw-r--r--   0 john       (501) staff       (20)       47 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/requirements-docs.txt
--rw-r--r--   0 john       (501) staff       (20)     7866 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/special.rst
--rw-r--r--   0 john       (501) staff       (20)     5962 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/strings.rst
--rw-r--r--   0 john       (501) staff       (20)     6987 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/swmr.rst
--rw-r--r--   0 john       (501) staff       (20)     5811 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/vds.rst
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.657900 h5pyd-0.9.1/docs/whatsnew/
--rw-r--r--   0 john       (501) staff       (20)      140 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/whatsnew/0.9.0.rst
--rw-r--r--   0 john       (501) staff       (20)      180 2021-12-15 01:10:39.000000 h5pyd-0.9.1/docs/whatsnew/index.rst
--rw-r--r--   0 john       (501) staff       (20)      277 2021-10-31 18:08:16.000000 h5pyd-0.9.1/environment.yml
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.660165 h5pyd-0.9.1/examples/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.660632 h5pyd-0.9.1/examples/notebooks/
--rw-r--r--   0 john       (501) staff       (20)     2753 2021-10-31 18:08:16.000000 h5pyd-0.9.1/examples/notebooks/tasmax.ipynb
--rwxr-xr-x   0 john       (501) staff       (20)     2415 2021-10-31 18:08:16.000000 h5pyd-0.9.1/examples/read_example.py
--rw-r--r--   0 john       (501) staff       (20)     2138 2021-10-31 18:08:16.000000 h5pyd-0.9.1/examples/readdatacube.py
--rw-r--r--   0 john       (501) staff       (20)     2478 2021-10-31 18:08:16.000000 h5pyd-0.9.1/examples/writedatacube.py
--rw-r--r--   0 john       (501) staff       (20)     1856 2021-10-31 18:08:16.000000 h5pyd-0.9.1/examples/writedatacube_compress.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.662570 h5pyd-0.9.1/h5pyd/
--rw-r--r--   0 john       (501) staff       (20)     2496 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/__init__.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.673377 h5pyd-0.9.1/h5pyd/_apps/
--rw-r--r--   0 john       (501) staff       (20)      909 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     5152 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/chunkiter.py
--rwxr-xr-x   0 john       (501) staff       (20)     3237 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/config.py
--rwxr-xr-x   0 john       (501) staff       (20)    11385 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsacl.py
--rw-r--r--   0 john       (501) staff       (20)     4234 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsconfigure.py
--rwxr-xr-x   0 john       (501) staff       (20)    10594 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hscopy.py
--rw-r--r--   0 john       (501) staff       (20)     4718 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsdel.py
--rwxr-xr-x   0 john       (501) staff       (20)    18706 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsdiff.py
--rwxr-xr-x   0 john       (501) staff       (20)     7236 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsget.py
--rw-r--r--   0 john       (501) staff       (20)    10738 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsinfo.py
--rwxr-xr-x   0 john       (501) staff       (20)    13123 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsload.py
--rw-r--r--   0 john       (501) staff       (20)    17067 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsls.py
--rwxr-xr-x   0 john       (501) staff       (20)     9621 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hsmv.py
--rw-r--r--   0 john       (501) staff       (20)     6741 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/hstouch.py
--rwxr-xr-x   0 john       (501) staff       (20)    28187 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_apps/utillib.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.683361 h5pyd-0.9.1/h5pyd/_hl/
--rw-r--r--   0 john       (501) staff       (20)      910 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/__init__.py
--rw-r--r--   0 john       (501) staff       (20)    14079 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/attrs.py
--rw-r--r--   0 john       (501) staff       (20)    36369 2021-12-15 01:10:39.000000 h5pyd-0.9.1/h5pyd/_hl/base.py
--rwxr-xr-x   0 john       (501) staff       (20)     3574 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/config.py
--rw-r--r--   0 john       (501) staff       (20)    55312 2021-12-16 16:26:21.000000 h5pyd-0.9.1/h5pyd/_hl/dataset.py
--rw-r--r--   0 john       (501) staff       (20)     1863 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/datatype.py
--rw-r--r--   0 john       (501) staff       (20)    15280 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/dims.py
--rw-r--r--   0 john       (501) staff       (20)    21131 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/files.py
--rw-r--r--   0 john       (501) staff       (20)    11354 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/filters.py
--rw-r--r--   0 john       (501) staff       (20)    13452 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/folders.py
--rw-r--r--   0 john       (501) staff       (20)    43803 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/group.py
--rw-r--r--   0 john       (501) staff       (20)    27453 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/h5type.py
--rwxr-xr-x   0 john       (501) staff       (20)    13125 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/h5type_test.py
--rw-r--r--   0 john       (501) staff       (20)     9935 2021-12-01 17:13:06.000000 h5pyd-0.9.1/h5pyd/_hl/hsdsapp.py
--rw-r--r--   0 john       (501) staff       (20)    27584 2021-12-01 18:45:09.000000 h5pyd-0.9.1/h5pyd/_hl/httpconn.py
--rw-r--r--   0 john       (501) staff       (20)     5935 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/objectid.py
--rw-r--r--   0 john       (501) staff       (20)    14797 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/openid.py
--rw-r--r--   0 john       (501) staff       (20)     2861 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/requests_lambda.py
--rw-r--r--   0 john       (501) staff       (20)    25040 2021-12-15 01:10:39.000000 h5pyd-0.9.1/h5pyd/_hl/selections.py
--rw-r--r--   0 john       (501) staff       (20)     2272 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/_hl/serverinfo.py
--rw-r--r--   0 john       (501) staff       (20)    14893 2021-11-12 01:42:05.000000 h5pyd-0.9.1/h5pyd/_hl/table.py
--rwxr-xr-x   0 john       (501) staff       (20)     3260 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/config.py
--rw-r--r--   0 john       (501) staff       (20)     3078 2021-10-31 18:08:16.000000 h5pyd-0.9.1/h5pyd/h5ds.py
--rw-r--r--   0 john       (501) staff       (20)     1659 2021-12-16 16:59:21.000000 h5pyd-0.9.1/h5pyd/version.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.664818 h5pyd-0.9.1/h5pyd.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     3776 2021-12-16 17:01:02.000000 h5pyd-0.9.1/h5pyd.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     2530 2021-12-16 17:01:02.000000 h5pyd-0.9.1/h5pyd.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2021-12-16 17:01:02.000000 h5pyd-0.9.1/h5pyd.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)      441 2021-12-16 17:01:02.000000 h5pyd-0.9.1/h5pyd.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2021-11-01 02:16:53.000000 h5pyd-0.9.1/h5pyd.egg-info/not-zip-safe
--rw-r--r--   0 john       (501) staff       (20)      152 2021-12-16 17:01:02.000000 h5pyd-0.9.1/h5pyd.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        6 2021-12-16 17:01:02.000000 h5pyd-0.9.1/h5pyd.egg-info/top_level.txt
--rwxr-xr-x   0 john       (501) staff       (20)      244 2021-10-31 18:08:16.000000 h5pyd-0.9.1/run_docker.sh
--rw-r--r--   0 john       (501) staff       (20)       38 2021-12-16 17:01:02.702309 h5pyd-0.9.1/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     1967 2021-12-16 16:58:31.000000 h5pyd-0.9.1/setup.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.635185 h5pyd-0.9.1/test/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.688010 h5pyd-0.9.1/test/apps/
--rw-r--r--   0 john       (501) staff       (20)     7944 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/common.py
--rwxr-xr-x   0 john       (501) staff       (20)     1612 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/config.py
--rw-r--r--   0 john       (501) staff       (20)     1415 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/is_hsds.py
--rw-r--r--   0 john       (501) staff       (20)     2323 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/load_files.py
--rw-r--r--   0 john       (501) staff       (20)     2613 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/test_diamond_inspect.py
--rw-r--r--   0 john       (501) staff       (20)     1302 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/test_hsinfo.py
--rw-r--r--   0 john       (501) staff       (20)     1967 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/test_shuffle_inspect.py
--rw-r--r--   0 john       (501) staff       (20)     3761 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/apps/test_tall_inspect.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 17:01:02.701181 h5pyd-0.9.1/test/hl/
--rw-r--r--   0 john       (501) staff       (20)     8171 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/common.py
--rwxr-xr-x   0 john       (501) staff       (20)     1526 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/config.py
--rw-r--r--   0 john       (501) staff       (20)     4605 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_attribute.py
--rw-r--r--   0 john       (501) staff       (20)     1787 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_committedtype.py
--rw-r--r--   0 john       (501) staff       (20)     3134 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_complex_numbers.py
--rw-r--r--   0 john       (501) staff       (20)     1953 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_compound.py
--rw-r--r--   0 john       (501) staff       (20)    20378 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_create.py
--rw-r--r--   0 john       (501) staff       (20)     2411 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_extend.py
--rw-r--r--   0 john       (501) staff       (20)     1804 2021-12-15 01:10:39.000000 h5pyd-0.9.1/test/hl/test_dataset_fancyselect.py
--rw-r--r--   0 john       (501) staff       (20)    19630 2021-12-15 01:10:39.000000 h5pyd-0.9.1/test/hl/test_dataset_getitem.py
--rw-r--r--   0 john       (501) staff       (20)     5891 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_objref.py
--rw-r--r--   0 john       (501) staff       (20)     4412 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_pointselect.py
--rw-r--r--   0 john       (501) staff       (20)     4021 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_scalar.py
--rw-r--r--   0 john       (501) staff       (20)     2249 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dataset_setitem.py
--rw-r--r--   0 john       (501) staff       (20)     7164 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_dimscale.py
--rw-r--r--   0 john       (501) staff       (20)    13988 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_file.py
--rw-r--r--   0 john       (501) staff       (20)     8675 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_folder.py
--rw-r--r--   0 john       (501) staff       (20)    11114 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_group.py
--rw-r--r--   0 john       (501) staff       (20)     6197 2021-11-12 01:36:19.000000 h5pyd-0.9.1/test/hl/test_table.py
--rw-r--r--   0 john       (501) staff       (20)     3906 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_visit.py
--rw-r--r--   0 john       (501) staff       (20)    15841 2021-10-31 18:08:16.000000 h5pyd-0.9.1/test/hl/test_vlentype.py
--rwxr-xr-x   0 john       (501) staff       (20)     2757 2021-10-31 18:08:16.000000 h5pyd-0.9.1/testall.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.241819 h5pyd-0.9.2/
+-rw-r--r--   0 john       (501) staff       (20)      813 2021-12-15 01:10:39.000000 h5pyd-0.9.2/.gitignore
+-rw-r--r--   0 john       (501) staff       (20)     3315 2021-10-31 18:08:16.000000 h5pyd-0.9.2/.travis.yml
+-rwxr-xr-x   0 john       (501) staff       (20)     1779 2021-10-31 18:08:16.000000 h5pyd-0.9.2/COPYING
+-rwxr-xr-x   0 john       (501) staff       (20)      467 2021-10-31 18:08:16.000000 h5pyd-0.9.2/Dockerfile
+-rw-r--r--   0 john       (501) staff       (20)     3776 2021-12-16 19:07:40.241522 h5pyd-0.9.2/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     2889 2021-10-31 18:08:16.000000 h5pyd-0.9.2/README.rst
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.212808 h5pyd-0.9.2/docs/
+-rw-r--r--   0 john       (501) staff       (20)     6755 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/Makefile
+-rw-r--r--   0 john       (501) staff       (20)     9040 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/build.rst
+-rw-r--r--   0 john       (501) staff       (20)     5906 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/conf.py
+-rw-r--r--   0 john       (501) staff       (20)     2942 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/config.rst
+-rw-r--r--   0 john       (501) staff       (20)    16441 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/contributing.rst
+-rw-r--r--   0 john       (501) staff       (20)    10190 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/faq.rst
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.214918 h5pyd-0.9.2/docs/high/
+-rw-r--r--   0 john       (501) staff       (20)     3972 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/high/attr.rst
+-rw-r--r--   0 john       (501) staff       (20)    24127 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/high/dataset.rst
+-rw-r--r--   0 john       (501) staff       (20)     3729 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/high/dims.rst
+-rw-r--r--   0 john       (501) staff       (20)    18276 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/high/file.rst
+-rw-r--r--   0 john       (501) staff       (20)    18251 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/high/group.rst
+-rw-r--r--   0 john       (501) staff       (20)     1363 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/high/lowlevel.rst
+-rw-r--r--   0 john       (501) staff       (20)     1375 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/index.rst
+-rw-r--r--   0 john       (501) staff       (20)    11708 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/licenses.rst
+-rw-r--r--   0 john       (501) staff       (20)     5131 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/mpi.rst
+-rw-r--r--   0 john       (501) staff       (20)     5733 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/quick.rst
+-rw-r--r--   0 john       (501) staff       (20)     3985 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/refs.rst
+-rw-r--r--   0 john       (501) staff       (20)     1201 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/release_guide.rst
+-rw-r--r--   0 john       (501) staff       (20)       47 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/requirements-docs.txt
+-rw-r--r--   0 john       (501) staff       (20)     7866 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/special.rst
+-rw-r--r--   0 john       (501) staff       (20)     5962 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/strings.rst
+-rw-r--r--   0 john       (501) staff       (20)     6987 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/swmr.rst
+-rw-r--r--   0 john       (501) staff       (20)     5811 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/vds.rst
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.215677 h5pyd-0.9.2/docs/whatsnew/
+-rw-r--r--   0 john       (501) staff       (20)      140 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/whatsnew/0.9.0.rst
+-rw-r--r--   0 john       (501) staff       (20)      180 2021-12-15 01:10:39.000000 h5pyd-0.9.2/docs/whatsnew/index.rst
+-rw-r--r--   0 john       (501) staff       (20)      277 2021-10-31 18:08:16.000000 h5pyd-0.9.2/environment.yml
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.217269 h5pyd-0.9.2/examples/
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.217646 h5pyd-0.9.2/examples/notebooks/
+-rw-r--r--   0 john       (501) staff       (20)     2753 2021-10-31 18:08:16.000000 h5pyd-0.9.2/examples/notebooks/tasmax.ipynb
+-rwxr-xr-x   0 john       (501) staff       (20)     2415 2021-10-31 18:08:16.000000 h5pyd-0.9.2/examples/read_example.py
+-rw-r--r--   0 john       (501) staff       (20)     2138 2021-10-31 18:08:16.000000 h5pyd-0.9.2/examples/readdatacube.py
+-rw-r--r--   0 john       (501) staff       (20)     2478 2021-10-31 18:08:16.000000 h5pyd-0.9.2/examples/writedatacube.py
+-rw-r--r--   0 john       (501) staff       (20)     1856 2021-10-31 18:08:16.000000 h5pyd-0.9.2/examples/writedatacube_compress.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.218715 h5pyd-0.9.2/h5pyd/
+-rw-r--r--   0 john       (501) staff       (20)     2496 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.225613 h5pyd-0.9.2/h5pyd/_apps/
+-rw-r--r--   0 john       (501) staff       (20)      909 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     5152 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/chunkiter.py
+-rwxr-xr-x   0 john       (501) staff       (20)     3237 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/config.py
+-rwxr-xr-x   0 john       (501) staff       (20)    11385 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsacl.py
+-rw-r--r--   0 john       (501) staff       (20)     4234 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsconfigure.py
+-rwxr-xr-x   0 john       (501) staff       (20)    10594 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hscopy.py
+-rw-r--r--   0 john       (501) staff       (20)     4718 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsdel.py
+-rwxr-xr-x   0 john       (501) staff       (20)    18706 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsdiff.py
+-rwxr-xr-x   0 john       (501) staff       (20)     7236 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsget.py
+-rw-r--r--   0 john       (501) staff       (20)    10738 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsinfo.py
+-rwxr-xr-x   0 john       (501) staff       (20)    13123 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsload.py
+-rw-r--r--   0 john       (501) staff       (20)    17067 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsls.py
+-rwxr-xr-x   0 john       (501) staff       (20)     9621 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hsmv.py
+-rw-r--r--   0 john       (501) staff       (20)     6741 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/hstouch.py
+-rwxr-xr-x   0 john       (501) staff       (20)    28187 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_apps/utillib.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.232153 h5pyd-0.9.2/h5pyd/_hl/
+-rw-r--r--   0 john       (501) staff       (20)      910 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)    14079 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/attrs.py
+-rw-r--r--   0 john       (501) staff       (20)    36369 2021-12-15 01:10:39.000000 h5pyd-0.9.2/h5pyd/_hl/base.py
+-rwxr-xr-x   0 john       (501) staff       (20)     3574 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/config.py
+-rw-r--r--   0 john       (501) staff       (20)    58287 2021-12-16 19:02:15.000000 h5pyd-0.9.2/h5pyd/_hl/dataset.py
+-rw-r--r--   0 john       (501) staff       (20)     1863 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/datatype.py
+-rw-r--r--   0 john       (501) staff       (20)    15280 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/dims.py
+-rw-r--r--   0 john       (501) staff       (20)    21131 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/files.py
+-rw-r--r--   0 john       (501) staff       (20)    11354 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/filters.py
+-rw-r--r--   0 john       (501) staff       (20)    13452 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/folders.py
+-rw-r--r--   0 john       (501) staff       (20)    43803 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/group.py
+-rw-r--r--   0 john       (501) staff       (20)    27453 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/h5type.py
+-rwxr-xr-x   0 john       (501) staff       (20)    13125 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/h5type_test.py
+-rw-r--r--   0 john       (501) staff       (20)     9935 2021-12-01 17:13:06.000000 h5pyd-0.9.2/h5pyd/_hl/hsdsapp.py
+-rw-r--r--   0 john       (501) staff       (20)    27584 2021-12-01 18:45:09.000000 h5pyd-0.9.2/h5pyd/_hl/httpconn.py
+-rw-r--r--   0 john       (501) staff       (20)     5935 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/objectid.py
+-rw-r--r--   0 john       (501) staff       (20)    14797 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/openid.py
+-rw-r--r--   0 john       (501) staff       (20)     2861 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/requests_lambda.py
+-rw-r--r--   0 john       (501) staff       (20)    25040 2021-12-15 01:10:39.000000 h5pyd-0.9.2/h5pyd/_hl/selections.py
+-rw-r--r--   0 john       (501) staff       (20)     2272 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/_hl/serverinfo.py
+-rw-r--r--   0 john       (501) staff       (20)    14893 2021-11-12 01:42:05.000000 h5pyd-0.9.2/h5pyd/_hl/table.py
+-rwxr-xr-x   0 john       (501) staff       (20)     3260 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/config.py
+-rw-r--r--   0 john       (501) staff       (20)     3078 2021-10-31 18:08:16.000000 h5pyd-0.9.2/h5pyd/h5ds.py
+-rw-r--r--   0 john       (501) staff       (20)     1659 2021-12-16 19:07:14.000000 h5pyd-0.9.2/h5pyd/version.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.220803 h5pyd-0.9.2/h5pyd.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     3776 2021-12-16 19:07:39.000000 h5pyd-0.9.2/h5pyd.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     2530 2021-12-16 19:07:40.000000 h5pyd-0.9.2/h5pyd.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2021-12-16 19:07:39.000000 h5pyd-0.9.2/h5pyd.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)      441 2021-12-16 19:07:39.000000 h5pyd-0.9.2/h5pyd.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2021-11-01 02:16:53.000000 h5pyd-0.9.2/h5pyd.egg-info/not-zip-safe
+-rw-r--r--   0 john       (501) staff       (20)      152 2021-12-16 19:07:39.000000 h5pyd-0.9.2/h5pyd.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        6 2021-12-16 19:07:39.000000 h5pyd-0.9.2/h5pyd.egg-info/top_level.txt
+-rwxr-xr-x   0 john       (501) staff       (20)      244 2021-10-31 18:08:16.000000 h5pyd-0.9.2/run_docker.sh
+-rw-r--r--   0 john       (501) staff       (20)       38 2021-12-16 19:07:40.241907 h5pyd-0.9.2/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     1967 2021-12-16 19:06:57.000000 h5pyd-0.9.2/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.205729 h5pyd-0.9.2/test/
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.234275 h5pyd-0.9.2/test/apps/
+-rw-r--r--   0 john       (501) staff       (20)     7944 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/common.py
+-rwxr-xr-x   0 john       (501) staff       (20)     1612 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/config.py
+-rw-r--r--   0 john       (501) staff       (20)     1415 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/is_hsds.py
+-rw-r--r--   0 john       (501) staff       (20)     2323 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/load_files.py
+-rw-r--r--   0 john       (501) staff       (20)     2613 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/test_diamond_inspect.py
+-rw-r--r--   0 john       (501) staff       (20)     1302 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/test_hsinfo.py
+-rw-r--r--   0 john       (501) staff       (20)     1967 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/test_shuffle_inspect.py
+-rw-r--r--   0 john       (501) staff       (20)     3761 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/apps/test_tall_inspect.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2021-12-16 19:07:40.241096 h5pyd-0.9.2/test/hl/
+-rw-r--r--   0 john       (501) staff       (20)     8171 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/common.py
+-rwxr-xr-x   0 john       (501) staff       (20)     1526 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/config.py
+-rw-r--r--   0 john       (501) staff       (20)     4605 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_attribute.py
+-rw-r--r--   0 john       (501) staff       (20)     1787 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_committedtype.py
+-rw-r--r--   0 john       (501) staff       (20)     3134 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_complex_numbers.py
+-rw-r--r--   0 john       (501) staff       (20)     1953 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_compound.py
+-rw-r--r--   0 john       (501) staff       (20)    20378 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_create.py
+-rw-r--r--   0 john       (501) staff       (20)     2411 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_extend.py
+-rw-r--r--   0 john       (501) staff       (20)     1804 2021-12-15 01:10:39.000000 h5pyd-0.9.2/test/hl/test_dataset_fancyselect.py
+-rw-r--r--   0 john       (501) staff       (20)    19630 2021-12-16 18:59:32.000000 h5pyd-0.9.2/test/hl/test_dataset_getitem.py
+-rw-r--r--   0 john       (501) staff       (20)     5891 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_objref.py
+-rw-r--r--   0 john       (501) staff       (20)     4412 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_pointselect.py
+-rw-r--r--   0 john       (501) staff       (20)     4021 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_scalar.py
+-rw-r--r--   0 john       (501) staff       (20)     2249 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dataset_setitem.py
+-rw-r--r--   0 john       (501) staff       (20)     7164 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_dimscale.py
+-rw-r--r--   0 john       (501) staff       (20)    13988 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_file.py
+-rw-r--r--   0 john       (501) staff       (20)     8675 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_folder.py
+-rw-r--r--   0 john       (501) staff       (20)    11114 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_group.py
+-rw-r--r--   0 john       (501) staff       (20)     6197 2021-11-12 01:36:19.000000 h5pyd-0.9.2/test/hl/test_table.py
+-rw-r--r--   0 john       (501) staff       (20)     3906 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_visit.py
+-rw-r--r--   0 john       (501) staff       (20)    15841 2021-10-31 18:08:16.000000 h5pyd-0.9.2/test/hl/test_vlentype.py
+-rwxr-xr-x   0 john       (501) staff       (20)     2757 2021-10-31 18:08:16.000000 h5pyd-0.9.2/testall.py
```

### Comparing `h5pyd-0.9.1/.gitignore` & `h5pyd-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/.travis.yml` & `h5pyd-0.9.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/COPYING` & `h5pyd-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/PKG-INFO` & `h5pyd-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: h5pyd
-Version: 0.9.1
+Version: 0.9.2
 Summary: h5py compatible client lib for HDF REST API
 Home-page: http://github.com/HDFGroup/h5pyd
 Author: John Readey
 Author-email: jreadey@hdfgrouup.org
 License: BSD
 Description: h5pyd
         =====
```

### Comparing `h5pyd-0.9.1/README.rst` & `h5pyd-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/Makefile` & `h5pyd-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/build.rst` & `h5pyd-0.9.2/docs/build.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/conf.py` & `h5pyd-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/config.rst` & `h5pyd-0.9.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/contributing.rst` & `h5pyd-0.9.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/faq.rst` & `h5pyd-0.9.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/high/attr.rst` & `h5pyd-0.9.2/docs/high/attr.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/high/dataset.rst` & `h5pyd-0.9.2/docs/high/dataset.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/high/dims.rst` & `h5pyd-0.9.2/docs/high/dims.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/high/file.rst` & `h5pyd-0.9.2/docs/high/file.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/high/group.rst` & `h5pyd-0.9.2/docs/high/group.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/high/lowlevel.rst` & `h5pyd-0.9.2/docs/high/lowlevel.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/index.rst` & `h5pyd-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/licenses.rst` & `h5pyd-0.9.2/docs/licenses.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/mpi.rst` & `h5pyd-0.9.2/docs/mpi.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/quick.rst` & `h5pyd-0.9.2/docs/quick.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/refs.rst` & `h5pyd-0.9.2/docs/refs.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/release_guide.rst` & `h5pyd-0.9.2/docs/release_guide.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/special.rst` & `h5pyd-0.9.2/docs/special.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/strings.rst` & `h5pyd-0.9.2/docs/strings.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/swmr.rst` & `h5pyd-0.9.2/docs/swmr.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/docs/vds.rst` & `h5pyd-0.9.2/docs/vds.rst`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/examples/notebooks/tasmax.ipynb` & `h5pyd-0.9.2/examples/notebooks/tasmax.ipynb`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/examples/read_example.py` & `h5pyd-0.9.2/examples/read_example.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/examples/readdatacube.py` & `h5pyd-0.9.2/examples/readdatacube.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/examples/writedatacube.py` & `h5pyd-0.9.2/examples/writedatacube.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/examples/writedatacube_compress.py` & `h5pyd-0.9.2/examples/writedatacube_compress.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/__init__.py` & `h5pyd-0.9.2/h5pyd/__init__.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/__init__.py` & `h5pyd-0.9.2/h5pyd/_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/chunkiter.py` & `h5pyd-0.9.2/h5pyd/_apps/chunkiter.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/config.py` & `h5pyd-0.9.2/h5pyd/_apps/config.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsacl.py` & `h5pyd-0.9.2/h5pyd/_apps/hsacl.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsconfigure.py` & `h5pyd-0.9.2/h5pyd/_apps/hsconfigure.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hscopy.py` & `h5pyd-0.9.2/h5pyd/_apps/hscopy.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsdel.py` & `h5pyd-0.9.2/h5pyd/_apps/hsdel.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsdiff.py` & `h5pyd-0.9.2/h5pyd/_apps/hsdiff.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsget.py` & `h5pyd-0.9.2/h5pyd/_apps/hsget.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsinfo.py` & `h5pyd-0.9.2/h5pyd/_apps/hsinfo.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsload.py` & `h5pyd-0.9.2/h5pyd/_apps/hsload.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsls.py` & `h5pyd-0.9.2/h5pyd/_apps/hsls.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hsmv.py` & `h5pyd-0.9.2/h5pyd/_apps/hsmv.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/hstouch.py` & `h5pyd-0.9.2/h5pyd/_apps/hstouch.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_apps/utillib.py` & `h5pyd-0.9.2/h5pyd/_apps/utillib.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/__init__.py` & `h5pyd-0.9.2/h5pyd/_hl/__init__.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/attrs.py` & `h5pyd-0.9.2/h5pyd/_hl/attrs.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/base.py` & `h5pyd-0.9.2/h5pyd/_hl/base.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/config.py` & `h5pyd-0.9.2/h5pyd/_hl/config.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/dataset.py` & `h5pyd-0.9.2/h5pyd/_hl/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,14 +211,93 @@
     def __enter__(self):
         self._dset._local.astype = self._dtype
 
     def __exit__(self, *args):
         self._dset._local.astype = None
 
 
+class ChunkIterator(object):
+    """
+    Class to iterate through list of chunks of a given dataset
+    """
+    def __init__(self, dset, source_sel=None):
+        self._shape = dset.shape
+        rank = len(dset.shape)
+
+        if not dset.chunks:
+            # can only use with chunked datasets
+            # (currently all datasets are chunked, but check for future compat)
+            raise TypeError("Chunked dataset required")
+
+        if isinstance(dset.chunks, dict):
+            self._layout = dset.chunks["dims"]
+        else:
+            self._layout = dset.chunks
+
+        if source_sel is None:
+            # select over entire dataset
+            slices = []
+            for dim in range(rank):
+                slices.append(slice(0, self._shape[dim]))
+            self._sel = tuple(slices)
+        else:
+            if isinstance(source_sel, slice):
+                self._sel = (source_sel,)
+            else:
+                self._sel = source_sel
+        if len(self._sel) != rank:
+            raise ValueError("Invalid selection - selection region must have same rank as dataset")
+        self._chunk_index = []
+        for dim in range(rank):
+            s = self._sel[dim]
+            if s.start < 0 or s.stop > self._shape[dim] or s.stop <= s.start:
+                raise ValueError("Invalid selection - selection region must be within dataset space")
+            index = s.start // self._layout[dim]
+            self._chunk_index.append(index)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        rank = len(self._shape)
+        slices = []
+        if rank == 0 or self._chunk_index[0] * self._layout[0] >= self._sel[0].stop:
+            # ran past the last chunk, end iteration
+            raise StopIteration()
+
+        for dim in range(rank):
+            s = self._sel[dim]
+            start = self._chunk_index[dim] * self._layout[dim]
+            stop = (self._chunk_index[dim] + 1) * self._layout[dim]
+            # adjust the start if this is an edge chunk
+            if start < s.start:
+                start = s.start
+            if stop > s.stop:
+                stop = s.stop  # trim to end of the selection
+            s = slice(start, stop, 1)
+            slices.append(s)
+
+        # bump up the last index and carry forward if we run outside the selection
+        dim = rank - 1
+        while dim >= 0:
+            s = self._sel[dim]
+            self._chunk_index[dim] += 1
+
+            chunk_end = self._chunk_index[dim] * self._layout[dim]
+            if chunk_end < s.stop:
+                # we still have room to extend along this dimensions
+                return tuple(slices)
+
+            if dim > 0:
+                # reset to the start and continue iterating with higher dimension
+                self._chunk_index[dim] = 0
+            dim -= 1
+        return tuple(slices)
+
+
 class Dataset(HLObject):
 
     """
         Represents an HDF5 dataset
     """
 
     def astype(self, dtype):
@@ -433,14 +512,19 @@
         return arr[()]
 
     def _is_empty(self):
         """ check if this is a null-space datset """
         return self._shape is None
 
     @property
+    def _is_empty(self):
+        """ check if this is a null-space datset """
+        return self._shape is None
+
+    @property
     def num_chunks(self):
         """ return number of allocated chunks"""
         self._getVerboseInfo()
         return self._num_chunks
 
     @property
     def allocated_size(self):
```

### Comparing `h5pyd-0.9.1/h5pyd/_hl/datatype.py` & `h5pyd-0.9.2/h5pyd/_hl/datatype.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/dims.py` & `h5pyd-0.9.2/h5pyd/_hl/dims.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/files.py` & `h5pyd-0.9.2/h5pyd/_hl/files.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/filters.py` & `h5pyd-0.9.2/h5pyd/_hl/filters.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/folders.py` & `h5pyd-0.9.2/h5pyd/_hl/folders.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/group.py` & `h5pyd-0.9.2/h5pyd/_hl/group.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/h5type.py` & `h5pyd-0.9.2/h5pyd/_hl/h5type.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/h5type_test.py` & `h5pyd-0.9.2/h5pyd/_hl/h5type_test.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/hsdsapp.py` & `h5pyd-0.9.2/h5pyd/_hl/hsdsapp.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/httpconn.py` & `h5pyd-0.9.2/h5pyd/_hl/httpconn.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/objectid.py` & `h5pyd-0.9.2/h5pyd/_hl/objectid.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/openid.py` & `h5pyd-0.9.2/h5pyd/_hl/openid.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/requests_lambda.py` & `h5pyd-0.9.2/h5pyd/_hl/requests_lambda.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/selections.py` & `h5pyd-0.9.2/h5pyd/_hl/selections.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/serverinfo.py` & `h5pyd-0.9.2/h5pyd/_hl/serverinfo.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/_hl/table.py` & `h5pyd-0.9.2/h5pyd/_hl/table.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/config.py` & `h5pyd-0.9.2/h5pyd/config.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/h5ds.py` & `h5pyd-0.9.2/h5pyd/h5ds.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/h5pyd/version.py` & `h5pyd-0.9.2/h5pyd/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 from __future__ import absolute_import
 
 from distutils.version import StrictVersion as _sv
 import sys
 import numpy
 
-version = "0.9.1"
+version = "0.9.2"
 
 hdf5_version = "REST"
 
 _exp = _sv(version)
 
 version_tuple = (
     _exp.version +
     (
         (''.join(str(x) for x in _exp.prerelease),)
         if _exp.prerelease is not None else ('',)
     )
 )
 
-api_version_tuple = (0, 9, 1)
-api_version = "0.9.1"
+api_version_tuple = (0, 9, 2)
+api_version = "0.9.2"
 
 __doc__ = """\
 This is h5pyd **%s**
 
 """ % (version)
 
 info = """\
```

### Comparing `h5pyd-0.9.1/h5pyd.egg-info/PKG-INFO` & `h5pyd-0.9.2/h5pyd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: h5pyd
-Version: 0.9.1
+Version: 0.9.2
 Summary: h5py compatible client lib for HDF REST API
 Home-page: http://github.com/HDFGroup/h5pyd
 Author: John Readey
 Author-email: jreadey@hdfgrouup.org
 License: BSD
 Description: h5pyd
         =====
```

### Comparing `h5pyd-0.9.1/h5pyd.egg-info/SOURCES.txt` & `h5pyd-0.9.2/h5pyd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/setup.py` & `h5pyd-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='h5pyd',
-      version='0.9.1',
+      version='0.9.2',
       description='h5py compatible client lib for HDF REST API',
       long_description=long_description,
       url='http://github.com/HDFGroup/h5pyd',
       author='John Readey',
       author_email='jreadey@hdfgrouup.org',
       license='BSD',
       packages=['h5pyd', 'h5pyd._hl', 'h5pyd._apps'],
```

### Comparing `h5pyd-0.9.1/test/apps/common.py` & `h5pyd-0.9.2/test/apps/common.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/config.py` & `h5pyd-0.9.2/test/apps/config.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/is_hsds.py` & `h5pyd-0.9.2/test/apps/is_hsds.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/load_files.py` & `h5pyd-0.9.2/test/apps/load_files.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/test_diamond_inspect.py` & `h5pyd-0.9.2/test/apps/test_diamond_inspect.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/test_hsinfo.py` & `h5pyd-0.9.2/test/apps/test_hsinfo.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/test_shuffle_inspect.py` & `h5pyd-0.9.2/test/apps/test_shuffle_inspect.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/apps/test_tall_inspect.py` & `h5pyd-0.9.2/test/apps/test_tall_inspect.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/common.py` & `h5pyd-0.9.2/test/hl/common.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/config.py` & `h5pyd-0.9.2/test/hl/config.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_attribute.py` & `h5pyd-0.9.2/test/hl/test_attribute.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_committedtype.py` & `h5pyd-0.9.2/test/hl/test_committedtype.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_complex_numbers.py` & `h5pyd-0.9.2/test/hl/test_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_compound.py` & `h5pyd-0.9.2/test/hl/test_dataset_compound.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_create.py` & `h5pyd-0.9.2/test/hl/test_dataset_create.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_extend.py` & `h5pyd-0.9.2/test/hl/test_dataset_extend.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_fancyselect.py` & `h5pyd-0.9.2/test/hl/test_dataset_fancyselect.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_getitem.py` & `h5pyd-0.9.2/test/hl/test_dataset_getitem.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_objref.py` & `h5pyd-0.9.2/test/hl/test_dataset_objref.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_pointselect.py` & `h5pyd-0.9.2/test/hl/test_dataset_pointselect.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_scalar.py` & `h5pyd-0.9.2/test/hl/test_dataset_scalar.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dataset_setitem.py` & `h5pyd-0.9.2/test/hl/test_dataset_setitem.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_dimscale.py` & `h5pyd-0.9.2/test/hl/test_dimscale.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_file.py` & `h5pyd-0.9.2/test/hl/test_file.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_folder.py` & `h5pyd-0.9.2/test/hl/test_folder.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_group.py` & `h5pyd-0.9.2/test/hl/test_group.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_table.py` & `h5pyd-0.9.2/test/hl/test_table.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_visit.py` & `h5pyd-0.9.2/test/hl/test_visit.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/test/hl/test_vlentype.py` & `h5pyd-0.9.2/test/hl/test_vlentype.py`

 * *Files identical despite different names*

### Comparing `h5pyd-0.9.1/testall.py` & `h5pyd-0.9.2/testall.py`

 * *Files identical despite different names*

