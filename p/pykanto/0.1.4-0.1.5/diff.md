# Comparing `tmp/pykanto-0.1.4.tar.gz` & `tmp/pykanto-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykanto-0.1.4.tar", last modified: Tue Mar 14 22:15:49 2023, max compression
+gzip compressed data, was "pykanto-0.1.5.tar", last modified: Wed May  3 00:39:53 2023, max compression
```

## Comparing `pykanto-0.1.4.tar` & `pykanto-0.1.5.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rwxr-xr-x   0        0        0     1084 2023-03-14 22:15:35.585716 pykanto-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     4677 2023-03-14 22:15:35.585716 pykanto-0.1.4/README.md
--rwxr-xr-x   0        0        0        0 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/__init__.py
--rw-r--r--   0        0        0       89 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/__init__.py
--rw-r--r--   0        0        0     7980 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/data.py
--rw-r--r--   0        0        0    19349 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/main.py
--rw-r--r--   0        0        0     1331 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/static/lasso.png
--rw-r--r--   0        0        0     5780 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/static/pykanto-logo.svg
--rw-r--r--   0        0        0     2565 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/templates/index.html
--rw-r--r--   0        0        0     6889 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/templates/styles.css
--rw-r--r--   0        0        0      536 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/app/theme.yaml
--rw-r--r--   0        0        0    94446 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/data/raw/AM/20210502_040000.WAV
--rw-r--r--   0        0        0      957 2023-03-14 22:15:35.797717 pykanto-0.1.4/pykanto/data/raw/AM/20210502_040000.xml
--rwxr-xr-x   0        0        0  1464876 2023-03-14 22:15:35.809717 pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.wav
--rwxr-xr-x   0        0        0      609 2023-03-14 22:15:35.809717 pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.xml
--rwxr-xr-x   0        0        0  1345900 2023-03-14 22:15:35.821717 pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.wav
--rwxr-xr-x   0        0        0      611 2023-03-14 22:15:35.821717 pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.xml
--rwxr-xr-x   0        0        0  1235284 2023-03-14 22:15:35.829717 pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC46092.wav
--rwxr-xr-x   0        0        0     1054 2023-03-14 22:15:35.829717 pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC46092.xml
--rwxr-xr-x   0        0        0  2713688 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC663885.wav
--rwxr-xr-x   0        0        0      967 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC663885.xml
--rwxr-xr-x   0        0        0      869 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-11.JSON
--rwxr-xr-x   0        0        0      870 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-15.JSON
--rwxr-xr-x   0        0        0      869 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-21.JSON
--rwxr-xr-x   0        0        0      869 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-23.JSON
--rwxr-xr-x   0        0        0      867 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-3.JSON
--rwxr-xr-x   0        0        0      869 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-6.JSON
--rwxr-xr-x   0        0        0      867 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-9.JSON
--rwxr-xr-x   0        0        0      873 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-21.JSON
--rwxr-xr-x   0        0        0      874 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-23.JSON
--rwxr-xr-x   0        0        0      874 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-24.JSON
--rwxr-xr-x   0        0        0      870 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_05-20.JSON
--rwxr-xr-x   0        0        0      872 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-77.JSON
--rwxr-xr-x   0        0        0      868 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-78.JSON
--rwxr-xr-x   0        0        0      872 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-79.JSON
--rwxr-xr-x   0        0        0      869 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-80.JSON
--rwxr-xr-x   0        0        0      870 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-81.JSON
--rwxr-xr-x   0        0        0      872 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-86.JSON
--rwxr-xr-x   0        0        0      872 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-88.JSON
--rwxr-xr-x   0        0        0      870 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-91.JSON
--rwxr-xr-x   0        0        0      871 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-92.JSON
--rwxr-xr-x   0        0        0   109412 2023-03-14 22:15:35.849717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-11.wav
--rwxr-xr-x   0        0        0   114704 2023-03-14 22:15:35.853717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-15.wav
--rwxr-xr-x   0        0        0   114116 2023-03-14 22:15:35.853717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-21.wav
--rwxr-xr-x   0        0        0   118820 2023-03-14 22:15:35.853717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-23.wav
--rwxr-xr-x   0        0        0    95300 2023-03-14 22:15:35.853717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-3.wav
--rwxr-xr-x   0        0        0   119408 2023-03-14 22:15:35.853717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-6.wav
--rwxr-xr-x   0        0        0   147044 2023-03-14 22:15:35.857717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-9.wav
--rwxr-xr-x   0        0        0   131992 2023-03-14 22:15:35.857717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-21.wav
--rwxr-xr-x   0        0        0   155982 2023-03-14 22:15:35.857717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-23.wav
--rwxr-xr-x   0        0        0   127758 2023-03-14 22:15:35.861717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-24.wav
--rwxr-xr-x   0        0        0    92360 2023-03-14 22:15:35.861717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_05-20.wav
--rwxr-xr-x   0        0        0    97652 2023-03-14 22:15:35.861717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-77.wav
--rwxr-xr-x   0        0        0   183500 2023-03-14 22:15:35.861717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-78.wav
--rwxr-xr-x   0        0        0   222308 2023-03-14 22:15:35.865718 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-79.wav
--rwxr-xr-x   0        0        0   131756 2023-03-14 22:15:35.865718 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-80.wav
--rwxr-xr-x   0        0        0   119996 2023-03-14 22:15:35.865718 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-81.wav
--rwxr-xr-x   0        0        0   142340 2023-03-14 22:15:35.865718 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-86.wav
--rwxr-xr-x   0        0        0   142340 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-88.wav
--rwxr-xr-x   0        0        0   127052 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-91.wav
--rwxr-xr-x   0        0        0    72956 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-92.wav
--rwxr-xr-x   0        0        0    43241 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_0.gzip
--rwxr-xr-x   0        0        0    42128 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_1.gzip
--rwxr-xr-x   0        0        0    44120 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_2.gzip
--rwxr-xr-x   0        0        0    41684 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_3.gzip
--rwxr-xr-x   0        0        0    41167 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_4.gzip
--rwxr-xr-x   0        0        0    40197 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_5.gzip
--rwxr-xr-x   0        0        0    40034 2023-03-14 22:15:35.869717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_0.gzip
--rwxr-xr-x   0        0        0    38139 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_1.gzip
--rwxr-xr-x   0        0        0    42169 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_2.gzip
--rwxr-xr-x   0        0        0    43081 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_3.gzip
--rwxr-xr-x   0        0        0    36610 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_4.gzip
--rw-r--r--   0        0        0      578 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_0.JSON
--rw-r--r--   0        0        0      580 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_1.JSON
--rw-r--r--   0        0        0      582 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_2.JSON
--rw-r--r--   0        0        0      580 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_3.JSON
--rw-r--r--   0        0        0      580 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_4.JSON
--rw-r--r--   0        0        0      580 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_5.JSON
--rw-r--r--   0        0        0      468 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_0.JSON
--rw-r--r--   0        0        0      585 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_1.JSON
--rw-r--r--   0        0        0      584 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_2.JSON
--rw-r--r--   0        0        0      585 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_3.JSON
--rw-r--r--   0        0        0      583 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_4.JSON
--rw-r--r--   0        0        0    35189 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/dataset.py
--rw-r--r--   0        0        0     4925 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/parameters.py
--rw-r--r--   0        0        0    16544 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/plot.py
--rwxr-xr-x   0        0        0       84 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/signal/__init__.py
--rw-r--r--   0        0        0     6340 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/signal/analysis.py
--rw-r--r--   0        0        0     9724 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/signal/cluster.py
--rwxr-xr-x   0        0        0     7266 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/signal/filter.py
--rwxr-xr-x   0        0        0    26755 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/signal/segment.py
--rw-r--r--   0        0        0    15761 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/signal/spectrogram.py
--rwxr-xr-x   0        0        0       59 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/__init__.py
--rw-r--r--   0        0        0     6257 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/compute.py
--rw-r--r--   0        0        0     6050 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/custom.py
--rw-r--r--   0        0        0    12023 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/io.py
--rwxr-xr-x   0        0        0    16024 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/paths.py
--rw-r--r--   0        0        0        7 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/slurm/.gitignore
--rw-r--r--   0        0        0     1070 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/slurm/LICENSE
--rwxr-xr-x   0        0        0       50 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/slurm/__init__.py
--rw-r--r--   0        0        0     5544 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/slurm/launch.py
--rw-r--r--   0        0        0     2422 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/slurm/sbatch_template.sh
--rw-r--r--   0        0        0      792 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/slurm/tester.py
--rw-r--r--   0        0        0     4760 2023-03-14 22:15:35.873717 pykanto-0.1.4/pykanto/utils/types.py
--rw-r--r--   0        0        0     1593 2023-03-14 22:15:35.873717 pykanto-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6444 1970-01-01 00:00:00.000000 pykanto-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1084 2023-05-03 00:39:40.591061 pykanto-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     4677 2023-05-03 00:39:40.591061 pykanto-0.1.5/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/__init__.py
+-rw-r--r--   0        0        0     7980 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/data.py
+-rw-r--r--   0        0        0    19087 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/main.py
+-rw-r--r--   0        0        0     1331 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/static/lasso.png
+-rw-r--r--   0        0        0     5780 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/static/pykanto-logo.svg
+-rw-r--r--   0        0        0     2565 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/templates/index.html
+-rw-r--r--   0        0        0     6889 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/templates/styles.css
+-rw-r--r--   0        0        0      536 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/app/theme.yaml
+-rw-r--r--   0        0        0    94446 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/data/raw/AM/20210502_040000.WAV
+-rw-r--r--   0        0        0      957 2023-05-03 00:39:40.779063 pykanto-0.1.5/pykanto/data/raw/AM/20210502_040000.xml
+-rwxr-xr-x   0        0        0  1464876 2023-05-03 00:39:40.791063 pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.wav
+-rwxr-xr-x   0        0        0      609 2023-05-03 00:39:40.791063 pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.xml
+-rwxr-xr-x   0        0        0  1345900 2023-05-03 00:39:40.799063 pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.wav
+-rwxr-xr-x   0        0        0      611 2023-05-03 00:39:40.799063 pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.xml
+-rwxr-xr-x   0        0        0  1235284 2023-05-03 00:39:40.807063 pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC46092.wav
+-rwxr-xr-x   0        0        0     1054 2023-05-03 00:39:40.807063 pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC46092.xml
+-rwxr-xr-x   0        0        0  2713688 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC663885.wav
+-rwxr-xr-x   0        0        0      967 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC663885.xml
+-rwxr-xr-x   0        0        0      869 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-11.JSON
+-rwxr-xr-x   0        0        0      870 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-15.JSON
+-rwxr-xr-x   0        0        0      869 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-21.JSON
+-rwxr-xr-x   0        0        0      869 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-23.JSON
+-rwxr-xr-x   0        0        0      867 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-3.JSON
+-rwxr-xr-x   0        0        0      869 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-6.JSON
+-rwxr-xr-x   0        0        0      867 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-9.JSON
+-rwxr-xr-x   0        0        0      873 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-21.JSON
+-rwxr-xr-x   0        0        0      874 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-23.JSON
+-rwxr-xr-x   0        0        0      874 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-24.JSON
+-rwxr-xr-x   0        0        0      870 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_05-20.JSON
+-rwxr-xr-x   0        0        0      872 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-77.JSON
+-rwxr-xr-x   0        0        0      868 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-78.JSON
+-rwxr-xr-x   0        0        0      872 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-79.JSON
+-rwxr-xr-x   0        0        0      869 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-80.JSON
+-rwxr-xr-x   0        0        0      870 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-81.JSON
+-rwxr-xr-x   0        0        0      872 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-86.JSON
+-rwxr-xr-x   0        0        0      872 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-88.JSON
+-rwxr-xr-x   0        0        0      870 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-91.JSON
+-rwxr-xr-x   0        0        0      871 2023-05-03 00:39:40.823063 pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-92.JSON
+-rwxr-xr-x   0        0        0   109412 2023-05-03 00:39:40.827063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-11.wav
+-rwxr-xr-x   0        0        0   114704 2023-05-03 00:39:40.827063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-15.wav
+-rwxr-xr-x   0        0        0   114116 2023-05-03 00:39:40.827063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-21.wav
+-rwxr-xr-x   0        0        0   118820 2023-05-03 00:39:40.827063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-23.wav
+-rwxr-xr-x   0        0        0    95300 2023-05-03 00:39:40.827063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-3.wav
+-rwxr-xr-x   0        0        0   119408 2023-05-03 00:39:40.831063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-6.wav
+-rwxr-xr-x   0        0        0   147044 2023-05-03 00:39:40.831063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-9.wav
+-rwxr-xr-x   0        0        0   131992 2023-05-03 00:39:40.831063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-21.wav
+-rwxr-xr-x   0        0        0   155982 2023-05-03 00:39:40.831063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-23.wav
+-rwxr-xr-x   0        0        0   127758 2023-05-03 00:39:40.831063 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-24.wav
+-rwxr-xr-x   0        0        0    92360 2023-05-03 00:39:40.835064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_05-20.wav
+-rwxr-xr-x   0        0        0    97652 2023-05-03 00:39:40.835064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-77.wav
+-rwxr-xr-x   0        0        0   183500 2023-05-03 00:39:40.835064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-78.wav
+-rwxr-xr-x   0        0        0   222308 2023-05-03 00:39:40.835064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-79.wav
+-rwxr-xr-x   0        0        0   131756 2023-05-03 00:39:40.839064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-80.wav
+-rwxr-xr-x   0        0        0   119996 2023-05-03 00:39:40.839064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-81.wav
+-rwxr-xr-x   0        0        0   142340 2023-05-03 00:39:40.839064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-86.wav
+-rwxr-xr-x   0        0        0   142340 2023-05-03 00:39:40.839064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-88.wav
+-rwxr-xr-x   0        0        0   127052 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-91.wav
+-rwxr-xr-x   0        0        0    72956 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-92.wav
+-rwxr-xr-x   0        0        0    43241 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_0.gzip
+-rwxr-xr-x   0        0        0    42128 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_1.gzip
+-rwxr-xr-x   0        0        0    44120 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_2.gzip
+-rwxr-xr-x   0        0        0    41684 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_3.gzip
+-rwxr-xr-x   0        0        0    41167 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_4.gzip
+-rwxr-xr-x   0        0        0    40197 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_5.gzip
+-rwxr-xr-x   0        0        0    40034 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_0.gzip
+-rwxr-xr-x   0        0        0    38139 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_1.gzip
+-rwxr-xr-x   0        0        0    42169 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_2.gzip
+-rwxr-xr-x   0        0        0    43081 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_3.gzip
+-rwxr-xr-x   0        0        0    36610 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_4.gzip
+-rw-r--r--   0        0        0      578 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_0.JSON
+-rw-r--r--   0        0        0      580 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_1.JSON
+-rw-r--r--   0        0        0      582 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_2.JSON
+-rw-r--r--   0        0        0      580 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_3.JSON
+-rw-r--r--   0        0        0      580 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_4.JSON
+-rw-r--r--   0        0        0      580 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_5.JSON
+-rw-r--r--   0        0        0      468 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_0.JSON
+-rw-r--r--   0        0        0      585 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_1.JSON
+-rw-r--r--   0        0        0      584 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_2.JSON
+-rw-r--r--   0        0        0      585 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_3.JSON
+-rw-r--r--   0        0        0      583 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_4.JSON
+-rw-r--r--   0        0        0    35189 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/dataset.py
+-rw-r--r--   0        0        0     4925 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/parameters.py
+-rw-r--r--   0        0        0    16544 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/plot.py
+-rwxr-xr-x   0        0        0       84 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/signal/__init__.py
+-rw-r--r--   0        0        0     6340 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/signal/analysis.py
+-rw-r--r--   0        0        0     9724 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/signal/cluster.py
+-rwxr-xr-x   0        0        0     7266 2023-05-03 00:39:40.843064 pykanto-0.1.5/pykanto/signal/filter.py
+-rwxr-xr-x   0        0        0    26776 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/signal/segment.py
+-rw-r--r--   0        0        0    15761 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/signal/spectrogram.py
+-rwxr-xr-x   0        0        0       59 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/__init__.py
+-rw-r--r--   0        0        0     6257 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/compute.py
+-rw-r--r--   0        0        0     6050 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/custom.py
+-rw-r--r--   0        0        0    12023 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/io.py
+-rwxr-xr-x   0        0        0    16024 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/paths.py
+-rw-r--r--   0        0        0        7 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/slurm/.gitignore
+-rw-r--r--   0        0        0     1070 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/slurm/LICENSE
+-rwxr-xr-x   0        0        0       50 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/slurm/__init__.py
+-rw-r--r--   0        0        0     5544 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/slurm/launch.py
+-rw-r--r--   0        0        0     2422 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/slurm/sbatch_template.sh
+-rw-r--r--   0        0        0      792 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/slurm/tester.py
+-rw-r--r--   0        0        0     4760 2023-05-03 00:39:40.847064 pykanto-0.1.5/pykanto/utils/types.py
+-rw-r--r--   0        0        0     1593 2023-05-03 00:39:40.847064 pykanto-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6444 1970-01-01 00:00:00.000000 pykanto-0.1.5/PKG-INFO
```

### Comparing `pykanto-0.1.4/LICENSE` & `pykanto-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/README.md` & `pykanto-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <a href="https://nilomr.github.io/pykanto">
     <img src="https://raw.githubusercontent.com/nilomr/pykanto/2c1613a928c4f98ce982176e52ddadc23e043834/docs/custom/pykanto-logo-grey-04.svg?token=AOQJBIQLQ4VKUF4V7NFYLKTD3TWVG" alt="pykanto logo" title="pykanto" height="80" style="padding-bottom:1em !important;" />
 </a>
 
 <br>
 <br>
 
-![version](https://img.shields.io/badge/package_version-0.1.4-orange)
+![version](https://img.shields.io/badge/package_version-0.1.5-orange)
 ![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)
 ![license](https://img.shields.io/github/license/mashape/apistatus.svg)
 ![Open Source Love](https://img.shields.io/badge/open%20source-♡-lightgrey)
 ![Python 3.8](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue.svg)
 
 **pykanto** is a python library to manage and analyse bird vocalisations
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
 
                                 [pykanto_logo]
 
- ![version](https://img.shields.io/badge/package_version-0.1.4-orange) ![PyPI
+ ![version](https://img.shields.io/badge/package_version-0.1.5-orange) ![PyPI
 status](https://img.shields.io/pypi/status/ansicolortags.svg) ![license](https:
   //img.shields.io/github/license/mashape/apistatus.svg) ![Open Source Love]
 (https://img.shields.io/badge/open%20source-â¡-lightgrey) ![Python 3.8](https:
 //img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue.svg) **pykanto** is
    a python library to manage and analyse bird vocalisations [Installation]
 (#installation) â¢ [Getting started](#getting-started) â¢ [Acknowledgements]
                            (#acknowledgements) # ã¤
```

### Comparing `pykanto-0.1.4/pykanto/app/data.py` & `pykanto-0.1.5/pykanto/app/data.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/app/main.py` & `pykanto-0.1.5/pykanto/app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from bokeh.models.widgets import Button, Dropdown
 from bokeh.palettes import Set3_12
 from bokeh.plotting import curdoc, figure
 from bokeh.themes import Theme
 from bokeh.transform import factor_cmap
 
 from pykanto.app.data import load_app_data
+from pykanto.utils.io import load_dataset
 from pykanto.utils.paths import ProjDirs
 
 # ──── FUNCTIONS ───────────────────────────────────────────────────────────────
 
 
 def get_markers(marker_types: List[str], mapping: np.ndarray) -> List[str]:
     """
@@ -52,14 +53,16 @@
     Args:
         marker_types (List[str]): List of marker types.
         mapping (np.ndarray): List of labels.
 
     Returns:
         List[str]: List of markers.
     """
+    if "-1" not in labs:
+        labs.insert(0, "-1")
     marker_dict = {
         lab: marker for marker, lab in zip(cycle(marker_types), labs)
     }
     markers = [marker_dict.get(e, "") for e in mapping]
     return markers
 
 
@@ -100,17 +103,19 @@
         "circle",
         "triangle",
         "hex",
     ]
     source.data["markers"] = get_markers(
         marker_types, source.data[grouping_labels]
     )
-
     # Build colour palette for the scatterplot
-    palette.insert(0, "#d92400")  # Add red for -1
+    # Add red for -1
+    if "-1" not in labs:
+        labs.insert(0, "-1")
+    palette.insert(0, "#d92400")
     palette = tuple(palette)
     colours = factor_cmap(
         field_name=grouping_labels, palette=palette, factors=labs
     )
 
     return palette, marker_types, colours
 
@@ -210,46 +215,35 @@
     ystart, yend = ymin - yextra, ymax + yextra
     return (xstart, xend), (ystart, yend)
 
 
 if "sphinx" in sys.modules:
     pass
 else:
-
     # ──── SETTINGS ────────────────────────────────────────────────────────────────
 
     debug = False
 
     if debug:
         warnings.warn(
             "Debug is set to true. The app will not work "
             "unless served directly"
         )
-        # YEAR = "2021"
-        # DATASET_ID = f"WYTHAM_GRETIS_2021_TEST"
-        # PROJECT = Path(
-        #     git.Repo('.', search_parent_directories=True).working_tree_dir)
-        # # Build the project structure if it isn't already:
-        # DIRS = ProjDirs(PROJECT, mkdir=True)
-        # dataset_loc = DIRS.DATA / "datasets" / DATASET_ID / f"{DATASET_ID}.db"
-        # max_n_labs = 12
-        # palette = list(Set3_12)
-        # song_level = True
+        song_level = False
+        DATASET_ID = "GREAT_TIT"
+        DATA_PATH = Path(pkg_resources.resource_filename("pykanto", "data"))
+        PROJECT = Path(DATA_PATH).parent
+        RAW_DATA = DATA_PATH / "segmented" / "great_tit"
+        DIRS = ProjDirs(PROJECT, RAW_DATA, DATASET_ID, mkdir=True)
         max_n_labs = 12
         palette = list(Set3_12)
-        song_level = False
-        PROJECT_ROOT = Path("/home/nilomr/projects/storm-petrel-song")
-        DATASET = "STORM_PETREL_2021"
-        RAW_DATA = PROJECT_ROOT / "data" / "raw" / DATASET
-        DIRS = ProjDirs(PROJECT_ROOT, RAW_DATA)
-        DATASET_ID = "STORM_PETREL_SONGS"
         dataset_loc = DIRS.DATA / "datasets" / DATASET_ID / f"{DATASET_ID}.db"
+        dataset = load_dataset(dataset_loc, DIRS)
 
     else:
-
         # Get dataset location from command line args
         dataset_loc = Path(sys.argv[1])
         # Maximum possible n of vocalisation types
         max_n_labs = int(float(sys.argv[2]))
         # Whether to use single units or their average per vocalisation
         song_level = parse_boolean(sys.argv[3])
         # Colour palette to use
@@ -295,15 +289,16 @@
         )
 
     source = load_app_data(dataset, labtype, remaining_indvs[0])
 
     # Generate labels, markers and colours
 
     # Build labels
-    labs = [str(lab) for lab in np.unique(source.data["auto_class"])]
+    labs = [str(lab) for lab in range(0, max_n_labs)]
+
     palette, marker_types, colours = prepare_legend(source, palette, labs)
 
     lightgrey = "#9e9e9e"
     background_grey = "#2F2F2F"
 
     # Tools in app
     TOOLS = "pan, wheel_zoom, box_select, lasso_select, crosshair, tap, undo, redo, reset"
@@ -319,15 +314,15 @@
         max_width=930,
         min_width=650,
         toolbar_location="above",
         x_axis_location=None,
         y_axis_location=None,
         output_backend="webgl",
     )
-    splot.title.text = f"{remaining_indvs[0].title()}: vocal repertoire"
+    splot.title.text = f"{remaining_indvs[0]}: vocal repertoire"
     splot.select(BoxSelectTool).select_every_mousemove = False
     splot.select(LassoSelectTool).select_every_mousemove = False
 
     r = splot.scatter(
         source=source,
         x="umap_x",
         y="umap_y",
@@ -503,15 +498,14 @@
 
     # Add right legend panel
     class_examples_div = Div(text=legend_html)
 
     # Interactive labelling and updating
 
     def next_plot(event):
-
         # Add previous individual to list of already checked
         indv = source.data["ID"][0]
 
         dataset.files.loc[
             (dataset.files[checktype] == False) & (dataset.files["ID"] == indv),
             checktype,
         ] = True
```

### Comparing `pykanto-0.1.4/pykanto/app/static/lasso.png` & `pykanto-0.1.5/pykanto/app/static/lasso.png`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/app/static/pykanto-logo.svg` & `pykanto-0.1.5/pykanto/app/static/pykanto-logo.svg`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/app/templates/index.html` & `pykanto-0.1.5/pykanto/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/app/templates/styles.css` & `pykanto-0.1.5/pykanto/app/templates/styles.css`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/app/theme.yaml` & `pykanto-0.1.5/pykanto/app/theme.yaml`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/AM/20210502_040000.WAV` & `pykanto-0.1.5/pykanto/data/raw/AM/20210502_040000.WAV`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/AM/20210502_040000.xml` & `pykanto-0.1.5/pykanto/data/raw/AM/20210502_040000.xml`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.wav` & `pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.xml` & `pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/348.xml`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.wav` & `pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.xml` & `pykanto-0.1.5/pykanto/data/raw/BENGALESE_FINCH/bird_3/363.xml`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC46092.wav` & `pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC46092.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC46092.xml` & `pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC46092.xml`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC663885.wav` & `pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC663885.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/raw/STORM-PETREL/XC663885.xml` & `pykanto-0.1.5/pykanto/data/raw/STORM-PETREL/XC663885.xml`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-11.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-11.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-15.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-15.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-21.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-21.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-23.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-23.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-3.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-3.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-6.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-6.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-9.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0415_05-9.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-21.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-21.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-23.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-23.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-24.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_04-24.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_05-20.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-B32-0416_05-20.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-77.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-77.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-78.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-78.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-79.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-79.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-80.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-80.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-81.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-81.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-86.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-86.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-88.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-88.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-91.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-91.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-92.JSON` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/JSON/2021-SW83-0418_04-92.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-11.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-11.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-15.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-15.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-21.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-21.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-23.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-23.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-3.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-3.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-6.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-6.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-9.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0415_05-9.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-21.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-21.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-23.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-23.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-24.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_04-24.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_05-20.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-B32-0416_05-20.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-77.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-77.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-78.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-78.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-79.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-79.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-80.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-80.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-81.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-81.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-86.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-86.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-88.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-88.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-91.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-91.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-92.wav` & `pykanto-0.1.5/pykanto/data/segmented/great_tit/WAV/2021-SW83-0418_04-92.wav`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_0.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_0.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_1.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_1.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_2.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_2.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_3.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_3.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_4.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_4.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_5.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC46092_5.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_0.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_0.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_1.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_1.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_2.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_2.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_3.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_3.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_4.gzip` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/GZIP/SegSyllsOutput_STORM-PETREL_XC663885_4.gzip`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_0.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_0.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_1.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_1.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_2.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_2.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_3.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_3.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_4.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_4.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_5.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC46092_5.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_1.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_1.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_2.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_2.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_3.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_3.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_4.JSON` & `pykanto-0.1.5/pykanto/data/segmented/storm-petrel/JSON/STORM-PETREL_XC663885_4.JSON`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/dataset.py` & `pykanto-0.1.5/pykanto/dataset.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/parameters.py` & `pykanto-0.1.5/pykanto/parameters.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/plot.py` & `pykanto-0.1.5/pykanto/plot.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/signal/analysis.py` & `pykanto-0.1.5/pykanto/signal/analysis.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/signal/cluster.py` & `pykanto-0.1.5/pykanto/signal/cluster.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/signal/filter.py` & `pykanto-0.1.5/pykanto/signal/filter.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/signal/segment.py` & `pykanto-0.1.5/pykanto/signal/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,14 @@
         **kwargs: Keyword arguments passed to
             :func:`~pykanto.signal.segment.segment_is_valid`.
     """
 
     n_segments = len(metadata.start_times)
 
     for i in range(n_segments):
-
         # Get segment frames
         wavfile.seek(metadata.start_times[i])
         audio_section: np.ndarray = wavfile.read(metadata.durations[i])
 
         # Collapse to mono if not already the case
         if len(audio_section.shape) == 2:
             audio_section: np.ndarray = librosa.to_mono(
@@ -355,15 +354,15 @@
                 orig_sr=sr,
                 target_sr=resample,
                 res_type="kaiser_fast",
             )
             sr = resample
 
         # Both to disk under name:
-        name: str = f"{metadata.ID}_{metadata.source_wav.stem}_{i}"
+        name: str = f"{metadata.ID}_{metadata.source_wav.stem}_{metadata.start_times[i]}"
 
         # Save .wav
         wav_out = wav_outdir / f"{name}.wav"
         sf.write(wav_out.as_posix(), audio_section, sr)
 
         # Save metadata .JSON
         segment_metadata = SegmentMetadata(
```

### Comparing `pykanto-0.1.4/pykanto/signal/spectrogram.py` & `pykanto-0.1.5/pykanto/signal/spectrogram.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/compute.py` & `pykanto-0.1.5/pykanto/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/custom.py` & `pykanto-0.1.5/pykanto/utils/custom.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/io.py` & `pykanto-0.1.5/pykanto/utils/io.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/paths.py` & `pykanto-0.1.5/pykanto/utils/paths.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/slurm/LICENSE` & `pykanto-0.1.5/pykanto/utils/slurm/LICENSE`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/slurm/launch.py` & `pykanto-0.1.5/pykanto/utils/slurm/launch.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/slurm/sbatch_template.sh` & `pykanto-0.1.5/pykanto/utils/slurm/sbatch_template.sh`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/slurm/tester.py` & `pykanto-0.1.5/pykanto/utils/slurm/tester.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pykanto/utils/types.py` & `pykanto-0.1.5/pykanto/utils/types.py`

 * *Files identical despite different names*

### Comparing `pykanto-0.1.4/pyproject.toml` & `pykanto-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pykanto"
 description = "A library for managing and analysing animal vocalisation data."
-version = "0.1.4"
+version = "0.1.5"
 authors = [{ name = "Nilo M. Recalde", email = "nilomerinorecalde@gmail.com" }]
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
```

### Comparing `pykanto-0.1.4/PKG-INFO` & `pykanto-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykanto
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for managing and analysing animal vocalisation data.
 Author-email: "Nilo M. Recalde" <nilomerinorecalde@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -54,15 +54,15 @@
 <a href="https://nilomr.github.io/pykanto">
     <img src="https://raw.githubusercontent.com/nilomr/pykanto/2c1613a928c4f98ce982176e52ddadc23e043834/docs/custom/pykanto-logo-grey-04.svg?token=AOQJBIQLQ4VKUF4V7NFYLKTD3TWVG" alt="pykanto logo" title="pykanto" height="80" style="padding-bottom:1em !important;" />
 </a>
 
 <br>
 <br>
 
-![version](https://img.shields.io/badge/package_version-0.1.4-orange)
+![version](https://img.shields.io/badge/package_version-0.1.5-orange)
 ![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)
 ![license](https://img.shields.io/github/license/mashape/apistatus.svg)
 ![Open Source Love](https://img.shields.io/badge/open%20source-♡-lightgrey)
 ![Python 3.8](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue.svg)
 
 **pykanto** is a python library to manage and analyse bird vocalisations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pykanto Version: 0.1.4 Summary: A library for
+Metadata-Version: 2.1 Name: pykanto Version: 0.1.5 Summary: A library for
 managing and analysing animal vocalisation data. Author-email: "Nilo M.
 Recalde"
 gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: pandas >= 1 Requires-Dist: numpy >=
@@ -21,15 +21,15 @@
 nb == 0.17 ; extra == "doc" Requires-Dist: myst-parser == 0.18 ; extra == "doc"
 Requires-Dist: pytest >=7 ; extra == "test" Project-URL: Documentation, https:/
 /nilomr.github.io/pykanto Project-URL: Source, https://github.com/nilomr/
 pykanto Provides-Extra: dev Provides-Extra: doc Provides-Extra: test
 
                                 [pykanto_logo]
 
- ![version](https://img.shields.io/badge/package_version-0.1.4-orange) ![PyPI
+ ![version](https://img.shields.io/badge/package_version-0.1.5-orange) ![PyPI
 status](https://img.shields.io/pypi/status/ansicolortags.svg) ![license](https:
   //img.shields.io/github/license/mashape/apistatus.svg) ![Open Source Love]
 (https://img.shields.io/badge/open%20source-â¡-lightgrey) ![Python 3.8](https:
 //img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue.svg) **pykanto** is
    a python library to manage and analyse bird vocalisations [Installation]
 (#installation) â¢ [Getting started](#getting-started) â¢ [Acknowledgements]
                            (#acknowledgements) # ã¤
```

