# Comparing `tmp/pythonSCHED-1.8.2.tar.gz` & `tmp/pythonSCHED-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythonSCHED-1.8.2.tar", last modified: Wed May 27 14:19:45 2020, max compression
+gzip compressed data, was "dist/pythonSCHED-1.9.0.tar", last modified: Tue Jun  9 14:19:50 2020, max compression
```

## Comparing `pythonSCHED-1.8.2.tar` & `pythonSCHED-1.9.0.tar`

### file list

```diff
@@ -1,784 +1,784 @@
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/
--rw-r--r--   0 eldering  (3587) jive      (3500)     3879 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/PKG-INFO
--rw-r--r--   0 eldering  (3587) jive      (3500)    12022 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/README
--rw-r--r--   0 eldering  (3587) jive      (3500)     2663 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/README.md
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/catalogs/
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/catalogs/Master_ATNF/
--rw-r--r--   0 eldering  (3587) jive      (3500)    25164 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_ATNF/freq_ATNF.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    60924 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_ATNF/locations.dat_from_ATNF
--rw-r--r--   0 eldering  (3587) jive      (3500)    13624 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_ATNF/locations_ATNF.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     7504 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_ATNF/stations_ATNF.dat
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/catalogs/Master_JIVE/
--rw-r--r--   0 eldering  (3587) jive      (3500)    70582 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_JIVE/freq_EVN.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     1325 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_JIVE/locations_KVN.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     5529 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_JIVE/messages_VEX.txt
--rw-r--r--   0 eldering  (3587) jive      (3500)    29069 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_JIVE/stations_EVN.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     1508 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_JIVE/stations_KVN.dat
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/
--rw-r--r--   0 eldering  (3587) jive      (3500)     5916 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/DSN_rationalization.txt
--rw-r--r--   0 eldering  (3587) jive      (3500)      388 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/README
--rw-r--r--   0 eldering  (3587) jive      (3500)    37343 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq.3mm.krichbaum.2005nov15
--rw-r--r--   0 eldering  (3587) jive      (3500)     3182 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_APT.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    14306 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_Arecibo.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     6812 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_DSN.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    16940 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_GB.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    24148 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_EB.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    19673 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_GB.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)   152919 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_VLBA.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     4771 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_top.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    69617 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_VLA.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)   143882 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_VLBA.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     2627 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_geodesy.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     2699 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_mm.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     4584 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_top.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     3470 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/gbt4mmfreqs.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    64136 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2005f
--rw-r--r--   0 eldering  (3587) jive      (3500)    70164 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2008a
--rw-r--r--   0 eldering  (3587) jive      (3500)    64622 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2009a
--rw-r--r--   0 eldering  (3587) jive      (3500)    57589 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2010a
--rw-r--r--   0 eldering  (3587) jive      (3500)    61195 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.gsfc2011a
--rw-r--r--   0 eldering  (3587) jive      (3500)    63396 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.gsfc_2014a
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.gsfc -> locations_gsfc2016aplus.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    27530 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.gsfc.2015feb.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     1038 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.top
--rw-r--r--   0 eldering  (3587) jive      (3500)     5752 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_DSN.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    20381 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_VLA.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    10659 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_extras.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    20962 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_gsfc2016aplus.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    31042 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/messages_NRAO.txt
--rw-r--r--   0 eldering  (3587) jive      (3500)     5834 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/peak.cmd
--rw-r--r--   0 eldering  (3587) jive      (3500)   143360 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/sched-lba.tar
--rw-r--r--   0 eldering  (3587) jive      (3500)      621 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations.tmp.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     4431 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_APT.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     8530 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_DSN.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    13032 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_RDBE_US.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     7431 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_RDBE_top.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    13739 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_US.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     3596 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_geodesy.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     3761 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_mm.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     6451 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_top.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     4024 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Master_NRAO/tapasi.email
--rw-r--r--   0 eldering  (3587) jive      (3500)      609 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/README.sources
--rwxr-xr-x   0 eldering  (3587) jive      (3500)     3792 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/Update
--rw-r--r--   0 eldering  (3587) jive      (3500)   360581 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/freq.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)   302921 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/freq_RDBE.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)     1382 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/linefreqs.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    73927 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/locations.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    36585 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/messages.txt
--rw-r--r--   0 eldering  (3587) jive      (3500)     5854 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/peak.cmd
--rw-r--r--   0 eldering  (3587) jive      (3500)     5860 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/peak_RDBE_DDC.cmd
--rw-r--r--   0 eldering  (3587) jive      (3500)     5858 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/peak_RDBE_PFB.cmd
--rw-r--r--   0 eldering  (3587) jive      (3500)    36116 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/pointing_source_fluxes
--rw-r--r--   0 eldering  (3587) jive      (3500)  2676070 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/rfc_2015a_cat.key
--rw-r--r--   0 eldering  (3587) jive      (3500)  4460285 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/rfc_2018a_cat.key
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.gsfc -> sources.gsfc2016
--rw-r--r--   0 eldering  (3587) jive      (3500)   858292 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.gsfc.2015feb
--rw-r--r--   0 eldering  (3587) jive      (3500)  1092041 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.gsfc2016
--rw-r--r--   0 eldering  (3587) jive      (3500)    32986 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.pointing
--rw-r--r--   0 eldering  (3587) jive      (3500)    24667 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.pttest
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.rfc -> rfc_2018a_cat.key
--rw-r--r--   0 eldering  (3587) jive      (3500)  1963165 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/sources.vlba.2012jul
--rw-r--r--   0 eldering  (3587) jive      (3500)    78775 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/stations.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    79048 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/stations_RDBE.dat
--rw-r--r--   0 eldering  (3587) jive      (3500)    28311 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/catalogs/stations_VLA.dat
--rwxr-xr-x   0 eldering  (3587) jive      (3500)    10676 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setup.py
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/setups/
--rw-r--r--   0 eldering  (3587) jive      (3500)     5028 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/DIR
--rw-r--r--   0 eldering  (3587) jive      (3500)    56029 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/Master_setups
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/setups/TEST/
--rw-r--r--   0 eldering  (3587) jive      (3500)     1930 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/Test128.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     1012 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/Test256.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     1413 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/Test64a.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     1269 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/Test64b.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     2021 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/TestM3.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     1400 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/TestSpec.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     1770 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/TestUL.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     2544 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/dum-y1.key
--rw-r--r--   0 eldering  (3587) jive      (3500)     2545 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/dum-yp.key
--rw-r--r--   0 eldering  (3587) jive      (3500)      231 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/TEST/test128.skd
--rw-r--r--   0 eldering  (3587) jive      (3500)     5116 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/frequencies.list
--rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba12mm-1p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba13cm-1p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      231 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba13cm-2p-1IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      147 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba13cm-2p-1IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      300 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba13cm-2p-2IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      309 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba13cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      406 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba13cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba18cm-1p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      324 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba18cm-2p-1IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      181 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba18cm-2p-1IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      312 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba18cm-2p-2IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      410 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba18cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      548 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba18cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      122 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba1cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      227 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba1cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba21cm-1p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      199 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba21cm-2p-1IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      101 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba21cm-2p-1IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      222 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba21cm-2p-2IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      133 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba21cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      223 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba21cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      118 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-1p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      254 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-1p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      465 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-2p-1IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      144 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-2p-1IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      770 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-2p-2IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      216 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba3cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      121 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba5cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      211 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba5cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      118 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba6cm-1p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      100 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba6cm-2p-1IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      187 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba6cm-2p-2IF-64MHz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      120 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba6cm-2p-2IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      211 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba6cm-2p-4IF.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      107 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/lba_sx.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      854 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/mer3b18cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      963 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/mer3cpol18cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      452 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt13cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      415 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt18cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      419 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt1cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      499 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt1cm2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      469 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt24ghz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      453 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt2cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      419 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt3mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      452 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt4cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      465 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt4cmsx.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      472 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt6cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      483 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt6cmw.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      669 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt7ghz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      419 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt7mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      412 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/pt90cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      451 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd13cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      414 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd18cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      418 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd1cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      498 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd1cm2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      468 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd24ghz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      452 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd2cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      418 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd3mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      451 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd4cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      464 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd4cmsx.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      471 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd6cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      650 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd7ghz.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      418 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd7mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      411 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptd90cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptdl1cm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      415 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptdl3mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptdl7mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      449 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/ptr7mm.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1980 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_15256_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     3136 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_1548_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1575 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_18cm_HSA_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1780 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_22220_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     2155 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_2284_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1938 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_4120_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1521 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_43120_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1721 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_4980_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1857 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_6588_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1816 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_6cm_wide_lcp.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1518 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_7680_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1799 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_8416_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1675 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/rdbe_pfb_86252_dual.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-128-4-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      463 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-256-8-2-R-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-256-8-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      790 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-512-16-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      791 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      566 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-512-8-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      509 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v13cm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-128-4-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      463 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-256-8-2-L-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-256-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      790 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-512-16-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      791 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      508 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-512-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      509 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v18cm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      410 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-128-4-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      411 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      454 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-256-8-2-L-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      454 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-256-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      455 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      455 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      738 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-512-16-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      739 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      456 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-512-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      457 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v1cm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      955 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-128-4-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      956 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      999 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-256-8-2-L-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      999 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-256-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1000 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1000 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1283 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-512-16-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1284 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1001 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-512-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1002 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v2cm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      416 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-128-4-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      460 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-256-8-2-R-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      460 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-256-8-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      461 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      461 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      744 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-512-16-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      745 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-512-8-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      463 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v4cm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      751 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v50cm-32-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1017 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-128-4-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1018 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1061 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-256-8-2-L-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1061 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-256-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1062 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1062 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1345 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-512-16-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1346 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1102 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-512-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1064 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v6cm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      523 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-128-4-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      524 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      567 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-256-8-2-L-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      567 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-256-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      568 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      568 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      524 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-32-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      851 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-512-16-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      852 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      569 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-512-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      570 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v7mm-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      423 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v9050cm-128-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      370 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v9050cm-64-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      652 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v90cm-32-8-2-L.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      625 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/v90cm-32-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      856 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vOH.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1162 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vgeo-128-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1106 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vgeo-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)     1243 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vgeo-512-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      407 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vla_c_pointing.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      407 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vla_x_pointing.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      668 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vmeth.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      488 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-128-4-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      514 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-128-4-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      586 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-256-8-2-R-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      586 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-256-8-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      612 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-256-8-2-UL.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      612 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-256-8-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      964 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-512-16-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      990 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-512-16-2.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      588 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-512-8-2-R.set
--rw-r--r--   0 eldering  (3587) jive      (3500)      614 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/setups/vsx-512-8-2.set
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Cit/
--rw-r--r--   0 eldering  (3587) jive      (3500)      818 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/geoid.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6102 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/geoxyz.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1503 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/julda.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      827 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/len1.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3195 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/pangle.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     9622 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/rdcat.inc
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/
--rw-r--r--   0 eldering  (3587) jive      (3500)      837 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/error.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      117 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/exit.c
--rw-r--r--   0 eldering  (3587) jive      (3500)      638 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/gerror.c
--rw-r--r--   0 eldering  (3587) jive      (3500)      793 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/idate.c
--rw-r--r--   0 eldering  (3587) jive      (3500)      300 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/isatty.c
--rw-r--r--   0 eldering  (3587) jive      (3500)     4490 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_linux/vlbope.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/
--rw-r--r--   0 eldering  (3587) jive      (3500)     2127 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/envir.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1427 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/krdlin.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      642 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/prognm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      588 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/putout.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1444 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/schdefs.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      846 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/symsub.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      267 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/tsttty.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      127 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/sys_unix/vmshlp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1968 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/tdatecw.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6176 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/tform.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      677 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Cit/upcase.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Jpl/
--rw-r--r--   0 eldering  (3587) jive      (3500)     1000 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/const.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2351 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/findt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1601 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/fsizer2.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3137 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/interp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3318 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/jplep2.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12471 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/jplpo2.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      313 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/jplver.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4888 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/pleph.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4398 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/pvobs.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      870 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/split.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7811 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/state.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      348 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Jpl/transp.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Plot/
--rw-r--r--   0 eldering  (3587) jive      (3500)      807 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/beam.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     9016 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/plbeam.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14316 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/plfft.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6704 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/plot.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     2267 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/pltran.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      599 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/plver.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2111 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/plweig.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1407 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/proj.inc
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/sched.inc -> ../Sched/sched.inc
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/schset.inc -> ../Sched/schset.inc
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plot/srlist.inc -> ../Sched/srlist.inc
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Plotstub/
--rw-r--r--   0 eldering  (3587) jive      (3500)      519 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Plotstub/pgqinf.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Sat/
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sat/sched.inc -> ../Sched/sched.inc
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Satstub/
--rw-r--r--   0 eldering  (3587) jive      (3500)      573 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Satstub/satep.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      606 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Satstub/sattle.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Sched/
--rw-r--r--   0 eldering  (3587) jive      (3500)     6519 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/accsrc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5062 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/addgeo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    24480 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/addpeak.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2128 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/antpos.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4633 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/autodown.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2015 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/azelxyew.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1856 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/azelxyns.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3511 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/badlo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7693 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcalt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      936 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbccdas.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2444 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcdbbc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2683 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcgeo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1616 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbckvsr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2177 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbclba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4298 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcm4.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1602 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcrdbe.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1505 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcvlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2399 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcvs2.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1401 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/bbcwidar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chars.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      795 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkcdas.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2114 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkcode.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2330 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkcor.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    11746 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkdbbc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14633 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkdbfq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2221 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkdisk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2297 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkfirm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2750 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkgdar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2113 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkif.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14388 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkrdbe.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    21669 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkrdfq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6060 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chksc1.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    17340 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkscn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    11446 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3992 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chksfil.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1838 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkspd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4750 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkvdar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2394 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkvdifx.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12597 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkvla.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    19651 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkvlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      743 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/chkwidar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1270 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/cordef.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14947 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/corlst.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5648 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/corsoc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1260 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/crdwrt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3676 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/defaults.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1610 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/defset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1639 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/delscr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      445 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/dequal.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2881 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/diskpos.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    18140 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/dopcrd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14329 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/dopfq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      732 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/dwcase.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      846 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/errlog.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2781 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/errset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13376 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fcompare.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4506 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fileopen.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7461 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/flags.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1230 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/flagwrt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1396 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/flush.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4757 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fmatch.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2215 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fmtmkiii.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13896 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fmtmkiv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6960 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fmtpick.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1858 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fmts2.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13274 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fmtvlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1662 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/frchar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    24538 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fsfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3527 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fsmatch.f
--rwxr-xr-x   0 eldering  (3587) jive      (3500)     9504 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fspread.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1064 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/fsvlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10944 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/geochk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14368 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/geomake.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12386 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/geoqual.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13516 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/getcrdn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7514 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/getfset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2931 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/getpairs.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      827 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/getsun.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2781 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/glstday.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    11049 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/gmkscn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3543 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/gnset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2555 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/haavai.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     9898 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/halim.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6862 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/harmwarn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2062 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/headpos.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3598 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/horchk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1772 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/ifdbbc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      394 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/inarray.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3146 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/jplgot.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5467 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/listfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    15672 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/lsqfit.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2276 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/lst2ut.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4533 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/lstfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10572 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/makeptg.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4296 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/makescn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    47843 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/makeseg.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      912 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/maxbas.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1865 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/mtaltaz.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4039 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/mtequat.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1684 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/mtxyew.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1724 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/mtxyns.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4653 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/omscor.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2489 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/omsfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4375 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/omsout.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6321 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/omsset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1674 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/omssrc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2694 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/omssta.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    15681 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optcells.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14213 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optcsar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6686 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optcspt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3749 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optcsub.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    25004 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/opthas.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4091 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/opthiel.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2300 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optnone.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8230 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optsch.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7100 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optskd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    18021 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/opttim.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3912 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/optupt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13706 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/pcalfq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4608 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/phint.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2844 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/pkfinish.f
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/plot.inc -> ../Plot/plot.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     2757 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/pn3db.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    18999 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/protect.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10123 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/prtfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10841 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/prtsch.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2638 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/prtscn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6647 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/prtset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1658 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/ptpat.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1920 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/ptvlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1456 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/ran5.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10504 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/rdbelevt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6706 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/rdbemtch.f
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/rdcat.inc -> ../Cit/rdcat.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     4004 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/recctl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4109 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/reconfig.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13723 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/resync.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10946 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/rotvlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8436 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sameset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4010 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/satgot.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8338 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sattim.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6943 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sbhours.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5665 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sbpair.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1470 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/scanid.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4715 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sch24.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1053 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schday.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    39024 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sched.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     3883 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schfreq.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     3992 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schgeo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    26873 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schopt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1229 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schpeak.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     6483 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schpre.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12471 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schset.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)    10025 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schsum.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13987 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/schtim.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6919 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/scndup.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2724 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/scngeo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2538 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/scnrange.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      760 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/scramble.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3466 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sdopincr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10294 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setband.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4235 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setbbc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12151 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setchan.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5097 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setcop.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4736 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setdefs.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6151 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setexpnd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    17321 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setfcat.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1647 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setfirm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2269 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setfmt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13417 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setform.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8547 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      946 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sethw1.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2677 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setnorec.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2689 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setrec.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4764 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setstdef.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10621 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/settps.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    16607 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/settrk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    17401 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/setusyn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8555 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sfinfo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2728 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/shortn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2343 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sidtim.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12651 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/slew.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2418 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/socdef.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2386 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srcflg.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2657 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srcloc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7733 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srclst.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    15906 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srcwrt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5992 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srfinish.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3119 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srinsert.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3029 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srlist.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1273 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srlist.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)      983 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/srlpre.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3203 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stafiles.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3869 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stafrd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5763 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stageo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8594 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stalst.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3220 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stano.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1552 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stauv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4343 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stmsg.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     9381 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/stsum.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5545 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sumdat.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3177 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sumdesc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2732 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sumope.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    10687 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sumscn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1010 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sunpos.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1240 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/sunwarn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7778 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/suvopt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1725 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/tavlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1079 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/timej.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3688 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/tpmfix.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6132 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/tpsum.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3853 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/tptpns.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2411 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/twohdset.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12296 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/uvopt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12659 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/uvqual.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7158 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/v2dout.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3417 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/versched.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4561 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vexout.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    11196 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlascns.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8405 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlba.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5471 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbabws.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3252 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbachar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1155 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbadk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1503 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbaend.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4209 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbaini.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3553 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbaint.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2693 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbareal.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4264 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbast.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1018 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbastop.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    23570 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vlbasu.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      238 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vsopwrt.f
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/vxlink.inc -> ../Vex/vxlink.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     1587 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/wlog.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    17679 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/wrap.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6614 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/wrapzone.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      999 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/wrtcov.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5138 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/wrtfreq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3019 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sched/wrtmsg.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Sla/
--rw-r--r--   0 eldering  (3587) jive      (3500)     2949 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/amp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3951 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/ampqk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2613 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/calyd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2642 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/cldj.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3461 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/clyd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1621 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/cs2c.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6074 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dat.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1821 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dcc2s.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1649 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dcs2c.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5250 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/deuler.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1731 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dimxv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2189 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/djcl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1846 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dmxm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1772 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dmxv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1394 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dranrm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1690 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dsep.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2142 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dsepv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3052 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1309 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dvdv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1802 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dvn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1505 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/dvxv.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3499 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/earth.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2824 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/ecor.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1370 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/epb2d.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1337 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/epj.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2286 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/eqeqx.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    16115 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/evp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6225 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/fk45z.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8671 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/fk524.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3012 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/fk54z.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2687 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/gmst.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3511 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/map.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4174 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/mappa.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5005 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/mapqk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4047 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/mapqkz.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2391 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/nut.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    38617 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/nutc.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2972 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/pm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2437 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/prebn.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3189 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/prec.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3003 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/preces.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4266 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/precl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1843 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/prenut.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2971 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/rvlsrk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1281 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Sla/vdv.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/Vex/
--rw-r--r--   0 eldering  (3587) jive      (3500)    19125 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/chk4dar.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3736 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/chkjive.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2974 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/chkv4dar.f
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/sched.inc -> ../Sched/sched.inc
-lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/schset.inc -> ../Sched/schset.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)      591 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfan.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1792 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfbb.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3585 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfda.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2142 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcffq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2705 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfhp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3534 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfif.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3611 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfph.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3033 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfpo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1695 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfrl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      611 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcfsi.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2498 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcftr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1398 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxcovr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2509 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxdefs.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2653 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxfqvx.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      680 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxgtst.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6779 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxlink.inc
--rw-r--r--   0 eldering  (3587) jive      (3500)     3468 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxmode.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      659 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnhds.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      760 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnman.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1444 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmbb.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1983 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmda.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3162 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmfq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1494 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmhp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3530 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmif.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2081 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmph.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1688 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmpo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      540 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmpr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1214 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmrl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      785 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmsi.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3135 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmtr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1971 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxnmxx.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2669 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxrl16.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1891 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxrl8.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2753 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxs2df.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1774 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxs2md.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12278 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxs2vl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    27918 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxsch.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    13411 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxschk.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    14058 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxscns.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    12877 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxsort.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2194 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxstky.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2320 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxstli.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2752 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxstnm.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     9313 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxsudt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2895 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtels.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    11606 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxton2.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     6649 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtone.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4869 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtrafq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2791 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtraif.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     9407 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtramd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1660 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtran.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2726 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxtraph.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2797 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxunql.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4633 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxvbrx.f
--rw-r--r--   0 eldering  (3587) jive      (3500)      508 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxvers.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5359 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwran.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1711 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrbb.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7348 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrda.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     8712 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrex.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4095 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrfq.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1205 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrgl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1411 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrhp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4465 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrif.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    20486 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrmd.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1755 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrph.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2811 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrpo.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     3249 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrpr.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     4615 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrrl.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     5885 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrsi.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     1554 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrst.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2684 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrsu.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     7684 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrt.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    18330 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/Vex/vxwrtr.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/pysched/
--rw-r--r--   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/__init__.py
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/pysched/catalog/
--rw-r--r--   0 eldering  (3587) jive      (3500)      517 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/__init__.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     5374 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2545 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/frequency_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      550 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/line_rest_frequency_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1732 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/peak_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1129 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/phase_center_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      632 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/satellite_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     6490 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/scan_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     9651 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/setup_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1828 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/setup_file_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2718 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/source_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      783 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/source_plot_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     8006 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/catalog/station_catalog.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     3989 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/dbbc_patching.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    17698 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/key.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      373 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/openwrap.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    56388 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/plot.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    11060 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/plot_toolbar.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      165 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/ran5wrap.f
-drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-05-27 14:19:45.000000 pythonSCHED-1.8.2/src/pysched/sched/
--rw-r--r--   0 eldering  (3587) jive      (3500)     2216 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/__init__.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2021 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/addgeo_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    14992 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/addpeak_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2811 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/bbcalt_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      975 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/bbcdbbc_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      878 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/bbcemerlin_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      363 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/checkemerlin_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     4686 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/chkdbbc_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     6792 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/chkset_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2301 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/defaults_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      266 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/defset_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     5558 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/geochk_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     8283 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/geomake_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     5843 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/getcor_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     3364 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/getcov_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     3605 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/getfreq_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1151 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/getset_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2789 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/getsta_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2322 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/gettim_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1496 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/gintent_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     4180 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/gmkscn_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      291 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/ifdbbc3_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      868 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/ifdbbc_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2450 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/infdb_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      843 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/input_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1563 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/invla_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1771 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/makescn_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    27278 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/makeseg_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     8225 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/optcells_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    18933 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/opthas_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2154 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/opthiel_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      827 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/optnone_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     3244 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/optskd_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2691 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/optupt_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      279 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/parameter.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1015 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/pcread_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     5179 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/rdpeak_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     9522 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/rdset_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1378 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/rfreq_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2190 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/satini_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      628 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/schdefs_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2873 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/schfiles_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    30609 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/schin_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     7345 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/schopt_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1241 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/schrep_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     3170 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/scndup_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2181 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/setbbc_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2583 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/setdefs_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2362 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/setexpnd_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     9790 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/srread_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2109 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/stmsg_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    14038 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/stread_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1267 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/sttant_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     1247 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/times_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      400 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/toggle_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     2870 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/sched/vexout_module.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      422 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/tformwrp.f
--rw-r--r--   0 eldering  (3587) jive      (3500)     2075 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/update_catalogs.py
--rw-r--r--   0 eldering  (3587) jive      (3500)     6057 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/util.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      714 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/version.py
--rw-r--r--   0 eldering  (3587) jive      (3500)      203 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/verwrap.f
--rw-r--r--   0 eldering  (3587) jive      (3500)    59639 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/vex.py
--rw-r--r--   0 eldering  (3587) jive      (3500)    10629 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/pysched/vex_scans.py
--rwxr-xr-x   0 eldering  (3587) jive      (3500)     7232 2020-05-27 14:19:32.000000 pythonSCHED-1.8.2/src/sched.py
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6867 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/PKG-INFO
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12022 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/README
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5179 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/README.md
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/catalogs/
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/catalogs/Master_ATNF/
+-rw-r--r--   0 eldering  (3587) jive      (3500)    25164 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_ATNF/freq_ATNF.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    60924 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_ATNF/locations.dat_from_ATNF
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13624 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_ATNF/locations_ATNF.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7504 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_ATNF/stations_ATNF.dat
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/catalogs/Master_JIVE/
+-rw-r--r--   0 eldering  (3587) jive      (3500)    70582 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_JIVE/freq_EVN.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1325 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_JIVE/locations_KVN.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5529 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_JIVE/messages_VEX.txt
+-rw-r--r--   0 eldering  (3587) jive      (3500)    29069 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_JIVE/stations_EVN.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1508 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_JIVE/stations_KVN.dat
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5916 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/DSN_rationalization.txt
+-rw-r--r--   0 eldering  (3587) jive      (3500)      388 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/README
+-rw-r--r--   0 eldering  (3587) jive      (3500)    37343 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq.3mm.krichbaum.2005nov15
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3182 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_APT.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14306 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_Arecibo.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6812 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_DSN.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    16940 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_GB.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    24148 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_EB.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    19673 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_GB.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)   152919 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_VLBA.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4771 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_top.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    69617 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_VLA.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)   143882 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_VLBA.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2627 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_geodesy.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2699 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_mm.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4584 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_top.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3470 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/gbt4mmfreqs.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    64136 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2005f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    70164 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2008a
+-rw-r--r--   0 eldering  (3587) jive      (3500)    64622 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2009a
+-rw-r--r--   0 eldering  (3587) jive      (3500)    57589 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2010a
+-rw-r--r--   0 eldering  (3587) jive      (3500)    61195 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.gsfc2011a
+-rw-r--r--   0 eldering  (3587) jive      (3500)    63396 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.gsfc_2014a
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.gsfc -> locations_gsfc2016aplus.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    27530 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.gsfc.2015feb.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1038 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.top
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5752 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_DSN.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    20381 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_VLA.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10659 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_extras.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    20962 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_gsfc2016aplus.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    31042 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/messages_NRAO.txt
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5834 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/peak.cmd
+-rw-r--r--   0 eldering  (3587) jive      (3500)   143360 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/sched-lba.tar
+-rw-r--r--   0 eldering  (3587) jive      (3500)      621 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations.tmp.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4431 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_APT.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8530 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_DSN.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13032 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_RDBE_US.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7431 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_RDBE_top.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13739 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_US.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3596 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_geodesy.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3761 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_mm.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6451 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_top.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4024 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Master_NRAO/tapasi.email
+-rw-r--r--   0 eldering  (3587) jive      (3500)      609 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/README.sources
+-rwxr-xr-x   0 eldering  (3587) jive      (3500)     3792 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/Update
+-rw-r--r--   0 eldering  (3587) jive      (3500)   360581 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/freq.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)   302921 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/freq_RDBE.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1382 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/linefreqs.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    73927 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/locations.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    36585 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/messages.txt
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5854 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/peak.cmd
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5860 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/peak_RDBE_DDC.cmd
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5858 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/peak_RDBE_PFB.cmd
+-rw-r--r--   0 eldering  (3587) jive      (3500)    36116 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/pointing_source_fluxes
+-rw-r--r--   0 eldering  (3587) jive      (3500)  2676070 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/rfc_2015a_cat.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)  4460285 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/rfc_2018a_cat.key
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.gsfc -> sources.gsfc2016
+-rw-r--r--   0 eldering  (3587) jive      (3500)   858292 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.gsfc.2015feb
+-rw-r--r--   0 eldering  (3587) jive      (3500)  1092041 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.gsfc2016
+-rw-r--r--   0 eldering  (3587) jive      (3500)    32986 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.pointing
+-rw-r--r--   0 eldering  (3587) jive      (3500)    24667 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.pttest
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.rfc -> rfc_2018a_cat.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)  1963165 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/sources.vlba.2012jul
+-rw-r--r--   0 eldering  (3587) jive      (3500)    78775 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/stations.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    79048 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/stations_RDBE.dat
+-rw-r--r--   0 eldering  (3587) jive      (3500)    28311 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/catalogs/stations_VLA.dat
+-rwxr-xr-x   0 eldering  (3587) jive      (3500)    10676 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setup.py
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/setups/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5028 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/DIR
+-rw-r--r--   0 eldering  (3587) jive      (3500)    56029 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/Master_setups
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/setups/TEST/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1930 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/Test128.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1012 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/Test256.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1413 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/Test64a.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1269 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/Test64b.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2021 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/TestM3.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1400 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/TestSpec.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1770 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/TestUL.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2544 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/dum-y1.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2545 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/dum-yp.key
+-rw-r--r--   0 eldering  (3587) jive      (3500)      231 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/TEST/test128.skd
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5116 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/frequencies.list
+-rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba12mm-1p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba13cm-1p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      231 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba13cm-2p-1IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      147 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba13cm-2p-1IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      300 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba13cm-2p-2IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      309 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba13cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      406 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba13cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba18cm-1p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      324 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba18cm-2p-1IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      181 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba18cm-2p-1IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      312 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba18cm-2p-2IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      410 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba18cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      548 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba18cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      122 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba1cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      227 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba1cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      119 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba21cm-1p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      199 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba21cm-2p-1IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      101 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba21cm-2p-1IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      222 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba21cm-2p-2IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      133 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba21cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      223 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba21cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      118 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-1p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      254 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-1p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      465 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-2p-1IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      144 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-2p-1IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      770 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-2p-2IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      216 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba3cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      121 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba5cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      211 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba5cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      118 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba6cm-1p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      100 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba6cm-2p-1IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      187 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba6cm-2p-2IF-64MHz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      120 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba6cm-2p-2IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      211 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba6cm-2p-4IF.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      107 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/lba_sx.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      854 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/mer3b18cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      963 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/mer3cpol18cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      452 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt13cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      415 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt18cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      419 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt1cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      499 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt1cm2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      469 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt24ghz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      453 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt2cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      419 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt3mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      452 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt4cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      465 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt4cmsx.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      472 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt6cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      483 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt6cmw.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      669 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt7ghz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      419 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt7mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      412 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/pt90cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      451 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd13cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      414 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd18cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      418 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd1cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      498 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd1cm2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      468 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd24ghz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      452 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd2cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      418 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd3mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      451 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd4cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      464 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd4cmsx.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      471 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd6cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      650 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd7ghz.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      418 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd7mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      411 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptd90cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptdl1cm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      415 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptdl3mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptdl7mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      449 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/ptr7mm.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1980 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_15256_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3136 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_1548_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1575 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_18cm_HSA_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1780 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_22220_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2155 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_2284_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1938 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_4120_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1521 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_43120_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1721 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_4980_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1857 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_6588_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1816 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_6cm_wide_lcp.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1518 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_7680_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1799 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_8416_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1675 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/rdbe_pfb_86252_dual.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-128-4-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      463 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-256-8-2-R-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-256-8-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      790 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-512-16-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      791 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      566 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-512-8-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      509 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v13cm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-128-4-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      463 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-256-8-2-L-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      506 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-256-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      507 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      790 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-512-16-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      791 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      508 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-512-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      509 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v18cm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      410 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-128-4-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      411 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      454 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-256-8-2-L-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      454 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-256-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      455 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      455 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      738 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-512-16-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      739 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      456 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-512-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      457 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v1cm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      955 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-128-4-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      956 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      999 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-256-8-2-L-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      999 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-256-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1000 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1000 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1283 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-512-16-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1284 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1001 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-512-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1002 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v2cm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      416 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-128-4-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      417 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      460 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-256-8-2-R-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      460 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-256-8-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      461 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      461 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      744 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-512-16-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      745 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-512-8-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      463 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v4cm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      751 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v50cm-32-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1017 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-128-4-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1018 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1061 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-256-8-2-L-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1061 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-256-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1062 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1062 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1345 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-512-16-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1346 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1102 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-512-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1064 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v6cm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      523 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-128-4-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      524 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      567 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-256-8-2-L-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      567 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-256-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      568 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      568 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      524 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-32-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      851 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-512-16-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      852 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      569 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-512-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      570 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v7mm-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      423 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v9050cm-128-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      370 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v9050cm-64-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      652 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v90cm-32-8-2-L.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      625 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/v90cm-32-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      856 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vOH.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1162 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vgeo-128-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1106 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vgeo-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1243 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vgeo-512-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      407 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vla_c_pointing.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      407 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vla_x_pointing.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      668 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vmeth.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      488 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-128-4-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      514 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-128-4-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      586 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-256-8-2-R-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      586 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-256-8-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      612 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-256-8-2-UL.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      612 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-256-8-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      964 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-512-16-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      990 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-512-16-2.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      588 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-512-8-2-R.set
+-rw-r--r--   0 eldering  (3587) jive      (3500)      614 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/setups/vsx-512-8-2.set
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Cit/
+-rw-r--r--   0 eldering  (3587) jive      (3500)      818 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/geoid.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6102 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/geoxyz.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1503 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/julda.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      827 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/len1.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3195 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/pangle.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9622 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/rdcat.inc
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/
+-rw-r--r--   0 eldering  (3587) jive      (3500)      837 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/error.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      117 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/exit.c
+-rw-r--r--   0 eldering  (3587) jive      (3500)      638 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/gerror.c
+-rw-r--r--   0 eldering  (3587) jive      (3500)      793 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/idate.c
+-rw-r--r--   0 eldering  (3587) jive      (3500)      300 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/isatty.c
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4490 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_linux/vlbope.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2127 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/envir.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1427 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/krdlin.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      642 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/prognm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      588 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/putout.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1444 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/schdefs.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      846 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/symsub.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      267 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/tsttty.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      127 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/sys_unix/vmshlp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1968 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/tdatecw.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6176 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/tform.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      677 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Cit/upcase.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Jpl/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1000 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/const.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2351 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/findt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1601 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/fsizer2.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3137 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/interp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3318 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/jplep2.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12471 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/jplpo2.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      313 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/jplver.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4888 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/pleph.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4398 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/pvobs.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      870 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/split.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7811 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/state.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      348 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Jpl/transp.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Plot/
+-rw-r--r--   0 eldering  (3587) jive      (3500)      807 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/beam.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9016 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/plbeam.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14316 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/plfft.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6704 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/plot.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2267 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/pltran.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      599 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/plver.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2111 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/plweig.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1407 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/proj.inc
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/sched.inc -> ../Sched/sched.inc
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/schset.inc -> ../Sched/schset.inc
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plot/srlist.inc -> ../Sched/srlist.inc
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Plotstub/
+-rw-r--r--   0 eldering  (3587) jive      (3500)      519 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Plotstub/pgqinf.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Sat/
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sat/sched.inc -> ../Sched/sched.inc
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Satstub/
+-rw-r--r--   0 eldering  (3587) jive      (3500)      573 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Satstub/satep.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      606 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Satstub/sattle.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Sched/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6519 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/accsrc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5062 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/addgeo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    24480 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/addpeak.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2128 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/antpos.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4633 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/autodown.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2015 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/azelxyew.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1856 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/azelxyns.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3511 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/badlo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7693 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcalt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      936 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbccdas.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2444 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcdbbc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2683 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcgeo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1616 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbckvsr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2177 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbclba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4298 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcm4.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1602 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcrdbe.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1505 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcvlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2399 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcvs2.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1401 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/bbcwidar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      462 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chars.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      795 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkcdas.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2114 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkcode.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2330 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkcor.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    11746 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkdbbc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14633 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkdbfq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2221 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkdisk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2297 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkfirm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2750 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkgdar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2113 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkif.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14388 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkrdbe.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    21669 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkrdfq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6060 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chksc1.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    17340 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkscn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    11446 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3992 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chksfil.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1838 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkspd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4750 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkvdar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2394 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkvdifx.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12597 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkvla.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    19651 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkvlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      743 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/chkwidar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1270 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/cordef.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14947 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/corlst.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5648 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/corsoc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1260 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/crdwrt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3676 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/defaults.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1610 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/defset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1639 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/delscr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      445 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/dequal.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2881 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/diskpos.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    18140 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/dopcrd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14329 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/dopfq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      732 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/dwcase.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      846 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/errlog.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2781 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/errset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13376 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fcompare.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4506 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fileopen.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7461 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/flags.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1230 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/flagwrt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1396 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/flush.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4757 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fmatch.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2215 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fmtmkiii.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13896 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fmtmkiv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6960 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fmtpick.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1858 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fmts2.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13274 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fmtvlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1662 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/frchar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    24538 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fsfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3527 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fsmatch.f
+-rwxr-xr-x   0 eldering  (3587) jive      (3500)     9504 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fspread.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1064 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/fsvlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10944 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/geochk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14368 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/geomake.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12386 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/geoqual.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13516 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/getcrdn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7514 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/getfset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2931 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/getpairs.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      827 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/getsun.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2781 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/glstday.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    11049 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/gmkscn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3543 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/gnset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2555 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/haavai.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9898 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/halim.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6862 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/harmwarn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2062 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/headpos.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3598 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/horchk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1772 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/ifdbbc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      394 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/inarray.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3146 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/jplgot.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5467 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/listfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    15672 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/lsqfit.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2276 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/lst2ut.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4533 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/lstfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10572 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/makeptg.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4296 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/makescn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    47843 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/makeseg.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      912 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/maxbas.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1865 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/mtaltaz.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4039 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/mtequat.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1684 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/mtxyew.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1724 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/mtxyns.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4653 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/omscor.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2489 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/omsfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4375 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/omsout.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6321 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/omsset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1674 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/omssrc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2694 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/omssta.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    15681 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optcells.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14213 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optcsar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6686 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optcspt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3749 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optcsub.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    25004 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/opthas.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4091 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/opthiel.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2300 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optnone.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8230 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optsch.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7100 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optskd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    18021 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/opttim.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3912 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/optupt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13706 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/pcalfq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4608 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/phint.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2844 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/pkfinish.f
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/plot.inc -> ../Plot/plot.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2757 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/pn3db.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    18999 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/protect.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10123 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/prtfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10841 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/prtsch.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2638 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/prtscn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6647 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/prtset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1658 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/ptpat.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1920 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/ptvlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1456 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/ran5.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10504 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/rdbelevt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6706 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/rdbemtch.f
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/rdcat.inc -> ../Cit/rdcat.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4004 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/recctl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4109 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/reconfig.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13723 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/resync.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10946 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/rotvlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8436 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sameset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4010 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/satgot.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8338 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sattim.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6943 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sbhours.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5665 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sbpair.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1470 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/scanid.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4715 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sch24.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1053 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schday.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    39024 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sched.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3883 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schfreq.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3992 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schgeo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    26873 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schopt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1229 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schpeak.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6483 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schpre.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12471 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schset.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10025 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schsum.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13987 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/schtim.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6919 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/scndup.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2724 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/scngeo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2538 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/scnrange.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      760 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/scramble.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3466 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sdopincr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10294 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setband.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4235 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setbbc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12151 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setchan.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5097 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setcop.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4736 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setdefs.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6151 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setexpnd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    17321 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setfcat.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1647 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setfirm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2269 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setfmt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13417 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setform.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8547 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      946 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sethw1.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2677 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setnorec.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2689 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setrec.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4764 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setstdef.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10621 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/settps.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    16607 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/settrk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    17401 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/setusyn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8555 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sfinfo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2728 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/shortn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2343 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sidtim.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12651 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/slew.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2418 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/socdef.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2386 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srcflg.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2657 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srcloc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7733 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srclst.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    15906 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srcwrt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5992 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srfinish.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3119 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srinsert.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3029 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srlist.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1273 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srlist.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)      983 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/srlpre.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3203 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stafiles.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3869 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stafrd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5763 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stageo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8594 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stalst.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3220 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stano.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1552 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stauv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4343 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stmsg.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9381 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/stsum.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5545 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sumdat.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3177 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sumdesc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2732 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sumope.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10687 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sumscn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1010 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sunpos.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1240 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/sunwarn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7778 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/suvopt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1725 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/tavlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1079 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/timej.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3688 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/tpmfix.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6132 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/tpsum.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3853 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/tptpns.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2411 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/twohdset.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12296 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/uvopt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12659 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/uvqual.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7158 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/v2dout.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3417 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/versched.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4561 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vexout.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    11196 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlascns.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8405 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlba.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5471 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbabws.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3252 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbachar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1155 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbadk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1503 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbaend.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4209 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbaini.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3553 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbaint.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2693 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbareal.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4264 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbast.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1018 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbastop.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    23570 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vlbasu.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      238 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vsopwrt.f
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/vxlink.inc -> ../Vex/vxlink.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1587 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/wlog.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    17679 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/wrap.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6614 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/wrapzone.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      999 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/wrtcov.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5138 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/wrtfreq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3019 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sched/wrtmsg.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Sla/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2949 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/amp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3951 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/ampqk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2613 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/calyd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2642 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/cldj.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3461 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/clyd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1621 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/cs2c.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6074 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dat.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1821 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dcc2s.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1649 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dcs2c.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5250 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/deuler.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1731 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dimxv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2189 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/djcl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1846 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dmxm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1772 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dmxv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1394 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dranrm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1690 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dsep.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2142 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dsepv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3052 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1309 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dvdv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1802 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dvn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1505 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/dvxv.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3499 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/earth.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2824 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/ecor.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1370 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/epb2d.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1337 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/epj.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2286 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/eqeqx.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    16115 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/evp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6225 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/fk45z.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8671 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/fk524.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3012 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/fk54z.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2687 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/gmst.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3511 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/map.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4174 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/mappa.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5005 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/mapqk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4047 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/mapqkz.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2391 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/nut.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    38617 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/nutc.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2972 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/pm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2437 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/prebn.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3189 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/prec.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3003 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/preces.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4266 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/precl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1843 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/prenut.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2971 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/rvlsrk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1281 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Sla/vdv.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/Vex/
+-rw-r--r--   0 eldering  (3587) jive      (3500)    19125 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/chk4dar.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3736 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/chkjive.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2974 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/chkv4dar.f
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/sched.inc -> ../Sched/sched.inc
+lrwxrwxrwx   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/schset.inc -> ../Sched/schset.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)      591 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfan.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1792 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfbb.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3585 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfda.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2142 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcffq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2705 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfhp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3534 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfif.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3611 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfph.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3033 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfpo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1695 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfrl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      611 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcfsi.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2498 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcftr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1398 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxcovr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2509 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxdefs.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2653 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxfqvx.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      680 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxgtst.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6779 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxlink.inc
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3468 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxmode.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      659 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnhds.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      760 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnman.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1444 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmbb.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1983 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmda.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3162 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmfq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1494 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmhp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3530 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmif.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2081 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmph.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1688 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmpo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      540 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmpr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1214 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmrl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      785 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmsi.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3135 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmtr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1971 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxnmxx.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2669 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxrl16.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1891 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxrl8.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2753 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxs2df.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1774 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxs2md.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12278 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxs2vl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    27918 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxsch.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    13411 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxschk.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14058 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxscns.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    12877 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxsort.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2194 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxstky.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2320 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxstli.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2752 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxstnm.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9313 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxsudt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2895 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtels.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    11606 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxton2.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6649 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtone.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4869 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtrafq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2791 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtraif.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9407 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtramd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1660 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtran.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2726 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxtraph.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2797 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxunql.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4633 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxvbrx.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)      508 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxvers.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5359 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwran.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1711 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrbb.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7348 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrda.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8712 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrex.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4095 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrfq.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1205 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrgl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1411 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrhp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4465 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrif.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    20486 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrmd.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1755 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrph.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2811 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrpo.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3249 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrpr.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4615 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrrl.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5885 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrsi.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1554 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrst.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2684 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrsu.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7684 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrt.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    18330 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/Vex/vxwrtr.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/pysched/
+-rw-r--r--   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/__init__.py
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/pysched/catalog/
+-rw-r--r--   0 eldering  (3587) jive      (3500)      517 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/__init__.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5374 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2545 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/frequency_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      550 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/line_rest_frequency_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1732 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/peak_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1129 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/phase_center_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      632 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/satellite_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6490 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/scan_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9651 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/setup_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1828 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/setup_file_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2718 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/source_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      783 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/source_plot_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8006 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/catalog/station_catalog.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3989 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/dbbc_patching.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    17698 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/key.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      373 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/openwrap.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    56388 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/plot.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    11060 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/plot_toolbar.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      165 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/ran5wrap.f
+drwxr-xr-x   0 eldering  (3587) jive      (3500)        0 2020-06-09 14:19:50.000000 pythonSCHED-1.9.0/src/pysched/sched/
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2216 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/__init__.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2021 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/addgeo_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14992 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/addpeak_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2811 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/bbcalt_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      975 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/bbcdbbc_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      878 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/bbcemerlin_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      363 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/checkemerlin_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4686 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/chkdbbc_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6792 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/chkset_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2301 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/defaults_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      266 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/defset_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5558 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/geochk_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8283 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/geomake_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5843 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/getcor_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3364 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/getcov_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3605 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/getfreq_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1151 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/getset_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2789 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/getsta_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2322 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/gettim_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1496 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/gintent_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     4180 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/gmkscn_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      291 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/ifdbbc3_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      868 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/ifdbbc_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2450 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/infdb_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      843 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/input_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1563 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/invla_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1771 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/makescn_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    27278 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/makeseg_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     8225 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/optcells_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    18933 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/opthas_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2154 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/opthiel_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      827 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/optnone_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3244 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/optskd_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2691 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/optupt_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      279 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/parameter.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1015 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/pcread_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     5179 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/rdpeak_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9522 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/rdset_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1378 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/rfreq_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2190 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/satini_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      628 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/schdefs_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2873 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/schfiles_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    30609 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/schin_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     7345 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/schopt_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1241 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/schrep_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     3170 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/scndup_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2181 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/setbbc_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2583 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/setdefs_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2362 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/setexpnd_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     9790 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/srread_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2109 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/stmsg_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    14038 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/stread_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1267 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/sttant_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     1247 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/times_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      400 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/toggle_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2870 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/sched/vexout_module.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      422 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/tformwrp.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)     2075 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/update_catalogs.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)     6057 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/util.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      714 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/version.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)      203 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/verwrap.f
+-rw-r--r--   0 eldering  (3587) jive      (3500)    59639 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/vex.py
+-rw-r--r--   0 eldering  (3587) jive      (3500)    10629 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/pysched/vex_scans.py
+-rwxr-xr-x   0 eldering  (3587) jive      (3500)     7232 2020-06-09 14:19:22.000000 pythonSCHED-1.9.0/src/sched.py
```

### Comparing `pythonSCHED-1.8.2/README` & `pythonSCHED-1.9.0/README`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_ATNF/freq_ATNF.dat` & `pythonSCHED-1.9.0/catalogs/Master_ATNF/freq_ATNF.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_ATNF/locations.dat_from_ATNF` & `pythonSCHED-1.9.0/catalogs/Master_ATNF/locations.dat_from_ATNF`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_ATNF/locations_ATNF.dat` & `pythonSCHED-1.9.0/catalogs/Master_ATNF/locations_ATNF.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_ATNF/stations_ATNF.dat` & `pythonSCHED-1.9.0/catalogs/Master_ATNF/stations_ATNF.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_JIVE/freq_EVN.dat` & `pythonSCHED-1.9.0/catalogs/Master_JIVE/freq_EVN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_JIVE/locations_KVN.dat` & `pythonSCHED-1.9.0/catalogs/Master_JIVE/locations_KVN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_JIVE/messages_VEX.txt` & `pythonSCHED-1.9.0/catalogs/Master_JIVE/messages_VEX.txt`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_JIVE/stations_EVN.dat` & `pythonSCHED-1.9.0/catalogs/Master_JIVE/stations_EVN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_JIVE/stations_KVN.dat` & `pythonSCHED-1.9.0/catalogs/Master_JIVE/stations_KVN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/DSN_rationalization.txt` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/DSN_rationalization.txt`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq.3mm.krichbaum.2005nov15` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq.3mm.krichbaum.2005nov15`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_APT.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_APT.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_Arecibo.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_Arecibo.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_DSN.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_DSN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_GB.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_GB.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_EB.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_EB.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_GB.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_GB.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_VLBA.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_VLBA.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_RDBE_top.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_RDBE_top.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_VLA.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_VLA.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_VLBA.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_VLBA.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_geodesy.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_geodesy.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_mm.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_mm.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/freq_top.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/freq_top.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/gbt4mmfreqs.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/gbt4mmfreqs.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2005f` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2005f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2008a` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2008a`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2009a` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2009a`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.2010a` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.2010a`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.gsfc2011a` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.gsfc2011a`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.dat.gsfc_2014a` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.dat.gsfc_2014a`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.gsfc.2015feb.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.gsfc.2015feb.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations.top` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations.top`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_DSN.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_DSN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_VLA.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_VLA.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_extras.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_extras.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/locations_gsfc2016aplus.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/locations_gsfc2016aplus.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/messages_NRAO.txt` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/messages_NRAO.txt`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/peak.cmd` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/peak.cmd`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/sched-lba.tar` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/sched-lba.tar`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations.tmp.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations.tmp.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_APT.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_APT.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_DSN.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_DSN.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_RDBE_US.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_RDBE_US.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_RDBE_top.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_RDBE_top.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_US.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_US.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_geodesy.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_geodesy.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_mm.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_mm.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/stations_top.dat` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/stations_top.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Master_NRAO/tapasi.email` & `pythonSCHED-1.9.0/catalogs/Master_NRAO/tapasi.email`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/README.sources` & `pythonSCHED-1.9.0/catalogs/README.sources`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/Update` & `pythonSCHED-1.9.0/catalogs/Update`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/freq.dat` & `pythonSCHED-1.9.0/catalogs/freq.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/freq_RDBE.dat` & `pythonSCHED-1.9.0/catalogs/freq_RDBE.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/linefreqs.dat` & `pythonSCHED-1.9.0/catalogs/linefreqs.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/locations.dat` & `pythonSCHED-1.9.0/catalogs/locations.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/messages.txt` & `pythonSCHED-1.9.0/catalogs/messages.txt`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/peak.cmd` & `pythonSCHED-1.9.0/catalogs/peak.cmd`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/peak_RDBE_DDC.cmd` & `pythonSCHED-1.9.0/catalogs/peak_RDBE_DDC.cmd`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/peak_RDBE_PFB.cmd` & `pythonSCHED-1.9.0/catalogs/peak_RDBE_PFB.cmd`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/pointing_source_fluxes` & `pythonSCHED-1.9.0/catalogs/pointing_source_fluxes`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/rfc_2015a_cat.key` & `pythonSCHED-1.9.0/catalogs/rfc_2015a_cat.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/rfc_2018a_cat.key` & `pythonSCHED-1.9.0/catalogs/rfc_2018a_cat.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/sources.gsfc.2015feb` & `pythonSCHED-1.9.0/catalogs/sources.gsfc.2015feb`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/sources.gsfc2016` & `pythonSCHED-1.9.0/catalogs/sources.gsfc2016`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/sources.pointing` & `pythonSCHED-1.9.0/catalogs/sources.pointing`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/sources.pttest` & `pythonSCHED-1.9.0/catalogs/sources.pttest`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/sources.vlba.2012jul` & `pythonSCHED-1.9.0/catalogs/sources.vlba.2012jul`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/stations.dat` & `pythonSCHED-1.9.0/catalogs/stations.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/stations_RDBE.dat` & `pythonSCHED-1.9.0/catalogs/stations_RDBE.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/catalogs/stations_VLA.dat` & `pythonSCHED-1.9.0/catalogs/stations_VLA.dat`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setup.py` & `pythonSCHED-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,15 @@
 extension = Extension(
     name="schedlib",
     sources=["src/" + s for s in sources + includes],
     f2py_options=["only:"] + functions + [":"])
 setup(
     cmdclass={"sdist": sdist},
     name="pythonSCHED",
-    version="1.8.2",
+    version="1.9.0",
     author="Bob Eldering",
     author_email="eldering@jive.eu",
     description="Python extension of NRAO's VLBI scheduling program SCHED "
     "(see http://www.aoc.nrao.edu/~cwalker/sched/)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jive-vlbi/sched",
```

### Comparing `pythonSCHED-1.8.2/setups/DIR` & `pythonSCHED-1.9.0/setups/DIR`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/Master_setups` & `pythonSCHED-1.9.0/setups/Master_setups`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/Test128.key` & `pythonSCHED-1.9.0/setups/TEST/Test128.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/Test256.key` & `pythonSCHED-1.9.0/setups/TEST/Test256.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/Test64a.key` & `pythonSCHED-1.9.0/setups/TEST/Test64a.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/Test64b.key` & `pythonSCHED-1.9.0/setups/TEST/Test64b.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/TestM3.key` & `pythonSCHED-1.9.0/setups/TEST/TestM3.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/TestSpec.key` & `pythonSCHED-1.9.0/setups/TEST/TestSpec.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/TestUL.key` & `pythonSCHED-1.9.0/setups/TEST/TestUL.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/dum-y1.key` & `pythonSCHED-1.9.0/setups/TEST/dum-y1.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/TEST/dum-yp.key` & `pythonSCHED-1.9.0/setups/TEST/dum-yp.key`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/frequencies.list` & `pythonSCHED-1.9.0/setups/frequencies.list`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/lba18cm-2p-4IF.set` & `pythonSCHED-1.9.0/setups/lba18cm-2p-4IF.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/lba3cm-2p-2IF-64MHz.set` & `pythonSCHED-1.9.0/setups/lba3cm-2p-2IF-64MHz.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/mer3b18cm.set` & `pythonSCHED-1.9.0/setups/mer3b18cm.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/mer3cpol18cm.set` & `pythonSCHED-1.9.0/setups/mer3cpol18cm.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/pt7ghz.set` & `pythonSCHED-1.9.0/setups/pt7ghz.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/ptd7ghz.set` & `pythonSCHED-1.9.0/setups/ptd7ghz.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_15256_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_15256_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_1548_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_1548_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_18cm_HSA_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_18cm_HSA_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_22220_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_22220_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_2284_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_2284_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_4120_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_4120_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_43120_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_43120_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_4980_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_4980_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_6588_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_6588_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_6cm_wide_lcp.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_6cm_wide_lcp.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_7680_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_7680_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_8416_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_8416_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/rdbe_pfb_86252_dual.set` & `pythonSCHED-1.9.0/setups/rdbe_pfb_86252_dual.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v13cm-512-16-2-R.set` & `pythonSCHED-1.9.0/setups/v13cm-512-16-2-R.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v13cm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v13cm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v13cm-512-8-2-R.set` & `pythonSCHED-1.9.0/setups/v13cm-512-8-2-R.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v18cm-512-16-2-L.set` & `pythonSCHED-1.9.0/setups/v18cm-512-16-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v18cm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v18cm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v1cm-512-16-2-L.set` & `pythonSCHED-1.9.0/setups/v1cm-512-16-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v1cm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v1cm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-128-4-2-L.set` & `pythonSCHED-1.9.0/setups/v2cm-128-4-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-128-4-2.set` & `pythonSCHED-1.9.0/setups/v2cm-128-4-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-256-8-2-L-UL.set` & `pythonSCHED-1.9.0/setups/v2cm-256-8-2-L-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-256-8-2-L.set` & `pythonSCHED-1.9.0/setups/v2cm-256-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-256-8-2-UL.set` & `pythonSCHED-1.9.0/setups/v2cm-256-8-2-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-256-8-2.set` & `pythonSCHED-1.9.0/setups/v2cm-256-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-512-16-2-L.set` & `pythonSCHED-1.9.0/setups/v2cm-512-16-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v2cm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-512-8-2-L.set` & `pythonSCHED-1.9.0/setups/v2cm-512-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v2cm-512-8-2.set` & `pythonSCHED-1.9.0/setups/v2cm-512-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v4cm-512-16-2-R.set` & `pythonSCHED-1.9.0/setups/v4cm-512-16-2-R.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v4cm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v4cm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v50cm-32-8-2.set` & `pythonSCHED-1.9.0/setups/v50cm-32-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-128-4-2-L.set` & `pythonSCHED-1.9.0/setups/v6cm-128-4-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-128-4-2.set` & `pythonSCHED-1.9.0/setups/v6cm-128-4-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-256-8-2-L-UL.set` & `pythonSCHED-1.9.0/setups/v6cm-256-8-2-L-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-256-8-2-L.set` & `pythonSCHED-1.9.0/setups/v6cm-256-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-256-8-2-UL.set` & `pythonSCHED-1.9.0/setups/v6cm-256-8-2-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-256-8-2.set` & `pythonSCHED-1.9.0/setups/v6cm-256-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-512-16-2-L.set` & `pythonSCHED-1.9.0/setups/v6cm-512-16-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v6cm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-512-8-2-L.set` & `pythonSCHED-1.9.0/setups/v6cm-512-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v6cm-512-8-2.set` & `pythonSCHED-1.9.0/setups/v6cm-512-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-128-4-2-L.set` & `pythonSCHED-1.9.0/setups/v7mm-128-4-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-128-4-2.set` & `pythonSCHED-1.9.0/setups/v7mm-128-4-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-256-8-2-L-UL.set` & `pythonSCHED-1.9.0/setups/v7mm-256-8-2-L-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-256-8-2-L.set` & `pythonSCHED-1.9.0/setups/v7mm-256-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-256-8-2-UL.set` & `pythonSCHED-1.9.0/setups/v7mm-256-8-2-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-256-8-2.set` & `pythonSCHED-1.9.0/setups/v7mm-256-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-32-4-2.set` & `pythonSCHED-1.9.0/setups/v7mm-32-4-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-512-16-2-L.set` & `pythonSCHED-1.9.0/setups/v7mm-512-16-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-512-16-2.set` & `pythonSCHED-1.9.0/setups/v7mm-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-512-8-2-L.set` & `pythonSCHED-1.9.0/setups/v7mm-512-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v7mm-512-8-2.set` & `pythonSCHED-1.9.0/setups/v7mm-512-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v90cm-32-8-2-L.set` & `pythonSCHED-1.9.0/setups/v90cm-32-8-2-L.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/v90cm-32-8-2.set` & `pythonSCHED-1.9.0/setups/v90cm-32-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vOH.set` & `pythonSCHED-1.9.0/setups/vOH.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vgeo-128-8-2.set` & `pythonSCHED-1.9.0/setups/vgeo-128-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vgeo-256-8-2.set` & `pythonSCHED-1.9.0/setups/vgeo-256-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vgeo-512-8-2.set` & `pythonSCHED-1.9.0/setups/vgeo-512-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vmeth.set` & `pythonSCHED-1.9.0/setups/vmeth.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-128-4-2.set` & `pythonSCHED-1.9.0/setups/vsx-128-4-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-256-8-2-R-UL.set` & `pythonSCHED-1.9.0/setups/vsx-256-8-2-R-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-256-8-2-R.set` & `pythonSCHED-1.9.0/setups/vsx-256-8-2-R.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-256-8-2-UL.set` & `pythonSCHED-1.9.0/setups/vsx-256-8-2-UL.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-256-8-2.set` & `pythonSCHED-1.9.0/setups/vsx-256-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-512-16-2-R.set` & `pythonSCHED-1.9.0/setups/vsx-512-16-2-R.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-512-16-2.set` & `pythonSCHED-1.9.0/setups/vsx-512-16-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-512-8-2-R.set` & `pythonSCHED-1.9.0/setups/vsx-512-8-2-R.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/setups/vsx-512-8-2.set` & `pythonSCHED-1.9.0/setups/vsx-512-8-2.set`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/geoid.f` & `pythonSCHED-1.9.0/src/Cit/geoid.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/geoxyz.f` & `pythonSCHED-1.9.0/src/Cit/geoxyz.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/julda.f` & `pythonSCHED-1.9.0/src/Cit/julda.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/len1.f` & `pythonSCHED-1.9.0/src/Cit/len1.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/pangle.f` & `pythonSCHED-1.9.0/src/Cit/pangle.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/rdcat.inc` & `pythonSCHED-1.9.0/src/Cit/rdcat.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_linux/error.f` & `pythonSCHED-1.9.0/src/Cit/sys_linux/error.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_linux/gerror.c` & `pythonSCHED-1.9.0/src/Cit/sys_linux/gerror.c`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_linux/idate.c` & `pythonSCHED-1.9.0/src/Cit/sys_linux/idate.c`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_linux/vlbope.f` & `pythonSCHED-1.9.0/src/Cit/sys_linux/vlbope.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_unix/envir.f` & `pythonSCHED-1.9.0/src/Cit/sys_unix/envir.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_unix/krdlin.f` & `pythonSCHED-1.9.0/src/Cit/sys_unix/krdlin.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_unix/prognm.f` & `pythonSCHED-1.9.0/src/Cit/sys_unix/prognm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_unix/putout.f` & `pythonSCHED-1.9.0/src/Cit/sys_unix/putout.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_unix/schdefs.f` & `pythonSCHED-1.9.0/src/Cit/sys_unix/schdefs.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/sys_unix/symsub.f` & `pythonSCHED-1.9.0/src/Cit/sys_unix/symsub.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/tdatecw.f` & `pythonSCHED-1.9.0/src/Cit/tdatecw.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/tform.f` & `pythonSCHED-1.9.0/src/Cit/tform.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Cit/upcase.f` & `pythonSCHED-1.9.0/src/Cit/upcase.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/const.f` & `pythonSCHED-1.9.0/src/Jpl/const.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/findt.f` & `pythonSCHED-1.9.0/src/Jpl/findt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/fsizer2.f` & `pythonSCHED-1.9.0/src/Jpl/fsizer2.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/interp.f` & `pythonSCHED-1.9.0/src/Jpl/interp.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/jplep2.f` & `pythonSCHED-1.9.0/src/Jpl/jplep2.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/jplpo2.f` & `pythonSCHED-1.9.0/src/Jpl/jplpo2.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/pleph.f` & `pythonSCHED-1.9.0/src/Jpl/pleph.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/pvobs.f` & `pythonSCHED-1.9.0/src/Jpl/pvobs.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/split.f` & `pythonSCHED-1.9.0/src/Jpl/split.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Jpl/state.f` & `pythonSCHED-1.9.0/src/Jpl/state.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/beam.inc` & `pythonSCHED-1.9.0/src/Plot/beam.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/plbeam.f` & `pythonSCHED-1.9.0/src/Plot/plbeam.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/plfft.f` & `pythonSCHED-1.9.0/src/Plot/plfft.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/plot.inc` & `pythonSCHED-1.9.0/src/Plot/plot.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/pltran.f` & `pythonSCHED-1.9.0/src/Plot/pltran.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/plver.f` & `pythonSCHED-1.9.0/src/Plot/plver.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/plweig.f` & `pythonSCHED-1.9.0/src/Plot/plweig.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plot/proj.inc` & `pythonSCHED-1.9.0/src/Plot/proj.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Plotstub/pgqinf.f` & `pythonSCHED-1.9.0/src/Plotstub/pgqinf.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Satstub/satep.f` & `pythonSCHED-1.9.0/src/Satstub/satep.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Satstub/sattle.f` & `pythonSCHED-1.9.0/src/Satstub/sattle.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/accsrc.f` & `pythonSCHED-1.9.0/src/Sched/accsrc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/addgeo.f` & `pythonSCHED-1.9.0/src/Sched/addgeo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/addpeak.f` & `pythonSCHED-1.9.0/src/Sched/addpeak.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/antpos.f` & `pythonSCHED-1.9.0/src/Sched/antpos.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/autodown.f` & `pythonSCHED-1.9.0/src/Sched/autodown.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/azelxyew.f` & `pythonSCHED-1.9.0/src/Sched/azelxyew.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/azelxyns.f` & `pythonSCHED-1.9.0/src/Sched/azelxyns.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/badlo.f` & `pythonSCHED-1.9.0/src/Sched/badlo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcalt.f` & `pythonSCHED-1.9.0/src/Sched/bbcalt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbccdas.f` & `pythonSCHED-1.9.0/src/Sched/bbccdas.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcdbbc.f` & `pythonSCHED-1.9.0/src/Sched/bbcdbbc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcgeo.f` & `pythonSCHED-1.9.0/src/Sched/bbcgeo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbckvsr.f` & `pythonSCHED-1.9.0/src/Sched/bbckvsr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbclba.f` & `pythonSCHED-1.9.0/src/Sched/bbclba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcm4.f` & `pythonSCHED-1.9.0/src/Sched/bbcm4.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcrdbe.f` & `pythonSCHED-1.9.0/src/Sched/bbcrdbe.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcvlba.f` & `pythonSCHED-1.9.0/src/Sched/bbcvlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcvs2.f` & `pythonSCHED-1.9.0/src/Sched/bbcvs2.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/bbcwidar.f` & `pythonSCHED-1.9.0/src/Sched/bbcwidar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkcdas.f` & `pythonSCHED-1.9.0/src/Sched/chkcdas.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkcode.f` & `pythonSCHED-1.9.0/src/Sched/chkcode.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkcor.f` & `pythonSCHED-1.9.0/src/Sched/chkcor.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkdbbc.f` & `pythonSCHED-1.9.0/src/Sched/chkdbbc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkdbfq.f` & `pythonSCHED-1.9.0/src/Sched/chkdbfq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkdisk.f` & `pythonSCHED-1.9.0/src/Sched/chkdisk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkfirm.f` & `pythonSCHED-1.9.0/src/Sched/chkfirm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkgdar.f` & `pythonSCHED-1.9.0/src/Sched/chkgdar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkif.f` & `pythonSCHED-1.9.0/src/Sched/chkif.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkrdbe.f` & `pythonSCHED-1.9.0/src/Sched/chkrdbe.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkrdfq.f` & `pythonSCHED-1.9.0/src/Sched/chkrdfq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chksc1.f` & `pythonSCHED-1.9.0/src/Sched/chksc1.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkscn.f` & `pythonSCHED-1.9.0/src/Sched/chkscn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkset.f` & `pythonSCHED-1.9.0/src/Sched/chkset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chksfil.f` & `pythonSCHED-1.9.0/src/Sched/chksfil.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkspd.f` & `pythonSCHED-1.9.0/src/Sched/chkspd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkvdar.f` & `pythonSCHED-1.9.0/src/Sched/chkvdar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkvdifx.f` & `pythonSCHED-1.9.0/src/Sched/chkvdifx.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkvla.f` & `pythonSCHED-1.9.0/src/Sched/chkvla.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkvlba.f` & `pythonSCHED-1.9.0/src/Sched/chkvlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/chkwidar.f` & `pythonSCHED-1.9.0/src/Sched/chkwidar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/cordef.f` & `pythonSCHED-1.9.0/src/Sched/cordef.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/corlst.f` & `pythonSCHED-1.9.0/src/Sched/corlst.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/corsoc.f` & `pythonSCHED-1.9.0/src/Sched/corsoc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/crdwrt.f` & `pythonSCHED-1.9.0/src/Sched/crdwrt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/defaults.f` & `pythonSCHED-1.9.0/src/Sched/defaults.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/defset.f` & `pythonSCHED-1.9.0/src/Sched/defset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/delscr.f` & `pythonSCHED-1.9.0/src/Sched/delscr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/diskpos.f` & `pythonSCHED-1.9.0/src/Sched/diskpos.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/dopcrd.f` & `pythonSCHED-1.9.0/src/Sched/dopcrd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/dopfq.f` & `pythonSCHED-1.9.0/src/Sched/dopfq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/dwcase.f` & `pythonSCHED-1.9.0/src/Sched/dwcase.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/errlog.f` & `pythonSCHED-1.9.0/src/Sched/errlog.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/errset.f` & `pythonSCHED-1.9.0/src/Sched/errset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fcompare.f` & `pythonSCHED-1.9.0/src/Sched/fcompare.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fileopen.f` & `pythonSCHED-1.9.0/src/Sched/fileopen.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/flags.f` & `pythonSCHED-1.9.0/src/Sched/flags.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/flagwrt.f` & `pythonSCHED-1.9.0/src/Sched/flagwrt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/flush.f` & `pythonSCHED-1.9.0/src/Sched/flush.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fmatch.f` & `pythonSCHED-1.9.0/src/Sched/fmatch.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fmtmkiii.f` & `pythonSCHED-1.9.0/src/Sched/fmtmkiii.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fmtmkiv.f` & `pythonSCHED-1.9.0/src/Sched/fmtmkiv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fmtpick.f` & `pythonSCHED-1.9.0/src/Sched/fmtpick.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fmts2.f` & `pythonSCHED-1.9.0/src/Sched/fmts2.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fmtvlba.f` & `pythonSCHED-1.9.0/src/Sched/fmtvlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/frchar.f` & `pythonSCHED-1.9.0/src/Sched/frchar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fsfreq.f` & `pythonSCHED-1.9.0/src/Sched/fsfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fsmatch.f` & `pythonSCHED-1.9.0/src/Sched/fsmatch.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fspread.f` & `pythonSCHED-1.9.0/src/Sched/fspread.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/fsvlba.f` & `pythonSCHED-1.9.0/src/Sched/fsvlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/geochk.f` & `pythonSCHED-1.9.0/src/Sched/geochk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/geomake.f` & `pythonSCHED-1.9.0/src/Sched/geomake.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/geoqual.f` & `pythonSCHED-1.9.0/src/Sched/geoqual.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/getcrdn.f` & `pythonSCHED-1.9.0/src/Sched/getcrdn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/getfset.f` & `pythonSCHED-1.9.0/src/Sched/getfset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/getpairs.f` & `pythonSCHED-1.9.0/src/Sched/getpairs.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/getsun.f` & `pythonSCHED-1.9.0/src/Sched/getsun.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/glstday.f` & `pythonSCHED-1.9.0/src/Sched/glstday.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/gmkscn.f` & `pythonSCHED-1.9.0/src/Sched/gmkscn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/gnset.f` & `pythonSCHED-1.9.0/src/Sched/gnset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/haavai.f` & `pythonSCHED-1.9.0/src/Sched/haavai.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/halim.f` & `pythonSCHED-1.9.0/src/Sched/halim.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/harmwarn.f` & `pythonSCHED-1.9.0/src/Sched/harmwarn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/headpos.f` & `pythonSCHED-1.9.0/src/Sched/headpos.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/horchk.f` & `pythonSCHED-1.9.0/src/Sched/horchk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/ifdbbc.f` & `pythonSCHED-1.9.0/src/Sched/ifdbbc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/jplgot.f` & `pythonSCHED-1.9.0/src/Sched/jplgot.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/listfreq.f` & `pythonSCHED-1.9.0/src/Sched/listfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/lsqfit.f` & `pythonSCHED-1.9.0/src/Sched/lsqfit.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/lst2ut.f` & `pythonSCHED-1.9.0/src/Sched/lst2ut.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/lstfreq.f` & `pythonSCHED-1.9.0/src/Sched/lstfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/makeptg.f` & `pythonSCHED-1.9.0/src/Sched/makeptg.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/makescn.f` & `pythonSCHED-1.9.0/src/Sched/makescn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/makeseg.f` & `pythonSCHED-1.9.0/src/Sched/makeseg.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/maxbas.f` & `pythonSCHED-1.9.0/src/Sched/maxbas.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/mtaltaz.f` & `pythonSCHED-1.9.0/src/Sched/mtaltaz.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/mtequat.f` & `pythonSCHED-1.9.0/src/Sched/mtequat.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/mtxyew.f` & `pythonSCHED-1.9.0/src/Sched/mtxyew.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/mtxyns.f` & `pythonSCHED-1.9.0/src/Sched/mtxyns.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/omscor.f` & `pythonSCHED-1.9.0/src/Sched/omscor.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/omsfreq.f` & `pythonSCHED-1.9.0/src/Sched/omsfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/omsout.f` & `pythonSCHED-1.9.0/src/Sched/omsout.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/omsset.f` & `pythonSCHED-1.9.0/src/Sched/omsset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/omssrc.f` & `pythonSCHED-1.9.0/src/Sched/omssrc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/omssta.f` & `pythonSCHED-1.9.0/src/Sched/omssta.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optcells.f` & `pythonSCHED-1.9.0/src/Sched/optcells.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optcsar.f` & `pythonSCHED-1.9.0/src/Sched/optcsar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optcspt.f` & `pythonSCHED-1.9.0/src/Sched/optcspt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optcsub.f` & `pythonSCHED-1.9.0/src/Sched/optcsub.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/opthas.f` & `pythonSCHED-1.9.0/src/Sched/opthas.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/opthiel.f` & `pythonSCHED-1.9.0/src/Sched/opthiel.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optnone.f` & `pythonSCHED-1.9.0/src/Sched/optnone.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optsch.f` & `pythonSCHED-1.9.0/src/Sched/optsch.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optskd.f` & `pythonSCHED-1.9.0/src/Sched/optskd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/opttim.f` & `pythonSCHED-1.9.0/src/Sched/opttim.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/optupt.f` & `pythonSCHED-1.9.0/src/Sched/optupt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/pcalfq.f` & `pythonSCHED-1.9.0/src/Sched/pcalfq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/phint.f` & `pythonSCHED-1.9.0/src/Sched/phint.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/pkfinish.f` & `pythonSCHED-1.9.0/src/Sched/pkfinish.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/pn3db.f` & `pythonSCHED-1.9.0/src/Sched/pn3db.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/protect.f` & `pythonSCHED-1.9.0/src/Sched/protect.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/prtfreq.f` & `pythonSCHED-1.9.0/src/Sched/prtfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/prtsch.f` & `pythonSCHED-1.9.0/src/Sched/prtsch.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/prtscn.f` & `pythonSCHED-1.9.0/src/Sched/prtscn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/prtset.f` & `pythonSCHED-1.9.0/src/Sched/prtset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/ptpat.f` & `pythonSCHED-1.9.0/src/Sched/ptpat.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/ptvlba.f` & `pythonSCHED-1.9.0/src/Sched/ptvlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/ran5.f` & `pythonSCHED-1.9.0/src/Sched/ran5.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/rdbelevt.f` & `pythonSCHED-1.9.0/src/Sched/rdbelevt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/rdbemtch.f` & `pythonSCHED-1.9.0/src/Sched/rdbemtch.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/recctl.f` & `pythonSCHED-1.9.0/src/Sched/recctl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/reconfig.f` & `pythonSCHED-1.9.0/src/Sched/reconfig.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/resync.f` & `pythonSCHED-1.9.0/src/Sched/resync.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/rotvlba.f` & `pythonSCHED-1.9.0/src/Sched/rotvlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sameset.f` & `pythonSCHED-1.9.0/src/Sched/sameset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/satgot.f` & `pythonSCHED-1.9.0/src/Sched/satgot.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sattim.f` & `pythonSCHED-1.9.0/src/Sched/sattim.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sbhours.f` & `pythonSCHED-1.9.0/src/Sched/sbhours.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sbpair.f` & `pythonSCHED-1.9.0/src/Sched/sbpair.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/scanid.f` & `pythonSCHED-1.9.0/src/Sched/scanid.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sch24.f` & `pythonSCHED-1.9.0/src/Sched/sch24.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schday.f` & `pythonSCHED-1.9.0/src/Sched/schday.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sched.inc` & `pythonSCHED-1.9.0/src/Sched/sched.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schfreq.inc` & `pythonSCHED-1.9.0/src/Sched/schfreq.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schgeo.f` & `pythonSCHED-1.9.0/src/Sched/schgeo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schopt.f` & `pythonSCHED-1.9.0/src/Sched/schopt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schpeak.inc` & `pythonSCHED-1.9.0/src/Sched/schpeak.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schpre.f` & `pythonSCHED-1.9.0/src/Sched/schpre.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schset.inc` & `pythonSCHED-1.9.0/src/Sched/schset.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schsum.f` & `pythonSCHED-1.9.0/src/Sched/schsum.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/schtim.f` & `pythonSCHED-1.9.0/src/Sched/schtim.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/scndup.f` & `pythonSCHED-1.9.0/src/Sched/scndup.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/scngeo.f` & `pythonSCHED-1.9.0/src/Sched/scngeo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/scnrange.f` & `pythonSCHED-1.9.0/src/Sched/scnrange.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/scramble.f` & `pythonSCHED-1.9.0/src/Sched/scramble.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sdopincr.f` & `pythonSCHED-1.9.0/src/Sched/sdopincr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setband.f` & `pythonSCHED-1.9.0/src/Sched/setband.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setbbc.f` & `pythonSCHED-1.9.0/src/Sched/setbbc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setchan.f` & `pythonSCHED-1.9.0/src/Sched/setchan.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setcop.f` & `pythonSCHED-1.9.0/src/Sched/setcop.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setdefs.f` & `pythonSCHED-1.9.0/src/Sched/setdefs.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setexpnd.f` & `pythonSCHED-1.9.0/src/Sched/setexpnd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setfcat.f` & `pythonSCHED-1.9.0/src/Sched/setfcat.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setfirm.f` & `pythonSCHED-1.9.0/src/Sched/setfirm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setfmt.f` & `pythonSCHED-1.9.0/src/Sched/setfmt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setform.f` & `pythonSCHED-1.9.0/src/Sched/setform.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setfreq.f` & `pythonSCHED-1.9.0/src/Sched/setfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sethw1.f` & `pythonSCHED-1.9.0/src/Sched/sethw1.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setnorec.f` & `pythonSCHED-1.9.0/src/Sched/setnorec.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setrec.f` & `pythonSCHED-1.9.0/src/Sched/setrec.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setstdef.f` & `pythonSCHED-1.9.0/src/Sched/setstdef.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/settps.f` & `pythonSCHED-1.9.0/src/Sched/settps.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/settrk.f` & `pythonSCHED-1.9.0/src/Sched/settrk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/setusyn.f` & `pythonSCHED-1.9.0/src/Sched/setusyn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sfinfo.f` & `pythonSCHED-1.9.0/src/Sched/sfinfo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/shortn.f` & `pythonSCHED-1.9.0/src/Sched/shortn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sidtim.f` & `pythonSCHED-1.9.0/src/Sched/sidtim.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/slew.f` & `pythonSCHED-1.9.0/src/Sched/slew.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/socdef.f` & `pythonSCHED-1.9.0/src/Sched/socdef.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srcflg.f` & `pythonSCHED-1.9.0/src/Sched/srcflg.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srcloc.f` & `pythonSCHED-1.9.0/src/Sched/srcloc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srclst.f` & `pythonSCHED-1.9.0/src/Sched/srclst.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srcwrt.f` & `pythonSCHED-1.9.0/src/Sched/srcwrt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srfinish.f` & `pythonSCHED-1.9.0/src/Sched/srfinish.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srinsert.f` & `pythonSCHED-1.9.0/src/Sched/srinsert.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srlist.f` & `pythonSCHED-1.9.0/src/Sched/srlist.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srlist.inc` & `pythonSCHED-1.9.0/src/Sched/srlist.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/srlpre.f` & `pythonSCHED-1.9.0/src/Sched/srlpre.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stafiles.f` & `pythonSCHED-1.9.0/src/Sched/stafiles.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stafrd.f` & `pythonSCHED-1.9.0/src/Sched/stafrd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stageo.f` & `pythonSCHED-1.9.0/src/Sched/stageo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stalst.f` & `pythonSCHED-1.9.0/src/Sched/stalst.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stano.f` & `pythonSCHED-1.9.0/src/Sched/stano.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stauv.f` & `pythonSCHED-1.9.0/src/Sched/stauv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stmsg.f` & `pythonSCHED-1.9.0/src/Sched/stmsg.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/stsum.f` & `pythonSCHED-1.9.0/src/Sched/stsum.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sumdat.f` & `pythonSCHED-1.9.0/src/Sched/sumdat.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sumdesc.f` & `pythonSCHED-1.9.0/src/Sched/sumdesc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sumope.f` & `pythonSCHED-1.9.0/src/Sched/sumope.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sumscn.f` & `pythonSCHED-1.9.0/src/Sched/sumscn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sunpos.f` & `pythonSCHED-1.9.0/src/Sched/sunpos.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/sunwarn.f` & `pythonSCHED-1.9.0/src/Sched/sunwarn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/suvopt.f` & `pythonSCHED-1.9.0/src/Sched/suvopt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/tavlba.f` & `pythonSCHED-1.9.0/src/Sched/tavlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/timej.f` & `pythonSCHED-1.9.0/src/Sched/timej.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/tpmfix.f` & `pythonSCHED-1.9.0/src/Sched/tpmfix.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/tpsum.f` & `pythonSCHED-1.9.0/src/Sched/tpsum.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/tptpns.f` & `pythonSCHED-1.9.0/src/Sched/tptpns.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/twohdset.f` & `pythonSCHED-1.9.0/src/Sched/twohdset.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/uvopt.f` & `pythonSCHED-1.9.0/src/Sched/uvopt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/uvqual.f` & `pythonSCHED-1.9.0/src/Sched/uvqual.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/v2dout.f` & `pythonSCHED-1.9.0/src/Sched/v2dout.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/versched.f` & `pythonSCHED-1.9.0/src/Sched/versched.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vexout.f` & `pythonSCHED-1.9.0/src/Sched/vexout.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlascns.f` & `pythonSCHED-1.9.0/src/Sched/vlascns.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlba.f` & `pythonSCHED-1.9.0/src/Sched/vlba.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbabws.f` & `pythonSCHED-1.9.0/src/Sched/vlbabws.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbachar.f` & `pythonSCHED-1.9.0/src/Sched/vlbachar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbadk.f` & `pythonSCHED-1.9.0/src/Sched/vlbadk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbaend.f` & `pythonSCHED-1.9.0/src/Sched/vlbaend.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbaini.f` & `pythonSCHED-1.9.0/src/Sched/vlbaini.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbaint.f` & `pythonSCHED-1.9.0/src/Sched/vlbaint.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbareal.f` & `pythonSCHED-1.9.0/src/Sched/vlbareal.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbast.f` & `pythonSCHED-1.9.0/src/Sched/vlbast.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbastop.f` & `pythonSCHED-1.9.0/src/Sched/vlbastop.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/vlbasu.f` & `pythonSCHED-1.9.0/src/Sched/vlbasu.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/wlog.f` & `pythonSCHED-1.9.0/src/Sched/wlog.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/wrap.f` & `pythonSCHED-1.9.0/src/Sched/wrap.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/wrapzone.f` & `pythonSCHED-1.9.0/src/Sched/wrapzone.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/wrtcov.f` & `pythonSCHED-1.9.0/src/Sched/wrtcov.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/wrtfreq.f` & `pythonSCHED-1.9.0/src/Sched/wrtfreq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sched/wrtmsg.f` & `pythonSCHED-1.9.0/src/Sched/wrtmsg.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/amp.f` & `pythonSCHED-1.9.0/src/Sla/amp.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/ampqk.f` & `pythonSCHED-1.9.0/src/Sla/ampqk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/calyd.f` & `pythonSCHED-1.9.0/src/Sla/calyd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/cldj.f` & `pythonSCHED-1.9.0/src/Sla/cldj.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/clyd.f` & `pythonSCHED-1.9.0/src/Sla/clyd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/cs2c.f` & `pythonSCHED-1.9.0/src/Sla/cs2c.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dat.f` & `pythonSCHED-1.9.0/src/Sla/dat.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dcc2s.f` & `pythonSCHED-1.9.0/src/Sla/dcc2s.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dcs2c.f` & `pythonSCHED-1.9.0/src/Sla/dcs2c.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/deuler.f` & `pythonSCHED-1.9.0/src/Sla/deuler.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dimxv.f` & `pythonSCHED-1.9.0/src/Sla/dimxv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/djcl.f` & `pythonSCHED-1.9.0/src/Sla/djcl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dmxm.f` & `pythonSCHED-1.9.0/src/Sla/dmxm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dmxv.f` & `pythonSCHED-1.9.0/src/Sla/dmxv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dranrm.f` & `pythonSCHED-1.9.0/src/Sla/dranrm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dsep.f` & `pythonSCHED-1.9.0/src/Sla/dsep.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dsepv.f` & `pythonSCHED-1.9.0/src/Sla/dsepv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dt.f` & `pythonSCHED-1.9.0/src/Sla/dt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dvdv.f` & `pythonSCHED-1.9.0/src/Sla/dvdv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dvn.f` & `pythonSCHED-1.9.0/src/Sla/dvn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/dvxv.f` & `pythonSCHED-1.9.0/src/Sla/dvxv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/earth.f` & `pythonSCHED-1.9.0/src/Sla/earth.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/ecor.f` & `pythonSCHED-1.9.0/src/Sla/ecor.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/epb2d.f` & `pythonSCHED-1.9.0/src/Sla/epb2d.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/epj.f` & `pythonSCHED-1.9.0/src/Sla/epj.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/eqeqx.f` & `pythonSCHED-1.9.0/src/Sla/eqeqx.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/evp.f` & `pythonSCHED-1.9.0/src/Sla/evp.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/fk45z.f` & `pythonSCHED-1.9.0/src/Sla/fk45z.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/fk524.f` & `pythonSCHED-1.9.0/src/Sla/fk524.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/fk54z.f` & `pythonSCHED-1.9.0/src/Sla/fk54z.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/gmst.f` & `pythonSCHED-1.9.0/src/Sla/gmst.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/map.f` & `pythonSCHED-1.9.0/src/Sla/map.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/mappa.f` & `pythonSCHED-1.9.0/src/Sla/mappa.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/mapqk.f` & `pythonSCHED-1.9.0/src/Sla/mapqk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/mapqkz.f` & `pythonSCHED-1.9.0/src/Sla/mapqkz.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/nut.f` & `pythonSCHED-1.9.0/src/Sla/nut.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/nutc.f` & `pythonSCHED-1.9.0/src/Sla/nutc.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/pm.f` & `pythonSCHED-1.9.0/src/Sla/pm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/prebn.f` & `pythonSCHED-1.9.0/src/Sla/prebn.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/prec.f` & `pythonSCHED-1.9.0/src/Sla/prec.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/preces.f` & `pythonSCHED-1.9.0/src/Sla/preces.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/precl.f` & `pythonSCHED-1.9.0/src/Sla/precl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/prenut.f` & `pythonSCHED-1.9.0/src/Sla/prenut.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/rvlsrk.f` & `pythonSCHED-1.9.0/src/Sla/rvlsrk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Sla/vdv.f` & `pythonSCHED-1.9.0/src/Sla/vdv.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/chk4dar.f` & `pythonSCHED-1.9.0/src/Vex/chk4dar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/chkjive.f` & `pythonSCHED-1.9.0/src/Vex/chkjive.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/chkv4dar.f` & `pythonSCHED-1.9.0/src/Vex/chkv4dar.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfan.f` & `pythonSCHED-1.9.0/src/Vex/vxcfan.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfbb.f` & `pythonSCHED-1.9.0/src/Vex/vxcfbb.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfda.f` & `pythonSCHED-1.9.0/src/Vex/vxcfda.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcffq.f` & `pythonSCHED-1.9.0/src/Vex/vxcffq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfhp.f` & `pythonSCHED-1.9.0/src/Vex/vxcfhp.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfif.f` & `pythonSCHED-1.9.0/src/Vex/vxcfif.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfph.f` & `pythonSCHED-1.9.0/src/Vex/vxcfph.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfpo.f` & `pythonSCHED-1.9.0/src/Vex/vxcfpo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfrl.f` & `pythonSCHED-1.9.0/src/Vex/vxcfrl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcfsi.f` & `pythonSCHED-1.9.0/src/Vex/vxcfsi.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcftr.f` & `pythonSCHED-1.9.0/src/Vex/vxcftr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxcovr.f` & `pythonSCHED-1.9.0/src/Vex/vxcovr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxdefs.f` & `pythonSCHED-1.9.0/src/Vex/vxdefs.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxfqvx.f` & `pythonSCHED-1.9.0/src/Vex/vxfqvx.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxgtst.f` & `pythonSCHED-1.9.0/src/Vex/vxgtst.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxlink.inc` & `pythonSCHED-1.9.0/src/Vex/vxlink.inc`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxmode.f` & `pythonSCHED-1.9.0/src/Vex/vxmode.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnhds.f` & `pythonSCHED-1.9.0/src/Vex/vxnhds.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnman.f` & `pythonSCHED-1.9.0/src/Vex/vxnman.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmbb.f` & `pythonSCHED-1.9.0/src/Vex/vxnmbb.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmda.f` & `pythonSCHED-1.9.0/src/Vex/vxnmda.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmfq.f` & `pythonSCHED-1.9.0/src/Vex/vxnmfq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmhp.f` & `pythonSCHED-1.9.0/src/Vex/vxnmhp.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmif.f` & `pythonSCHED-1.9.0/src/Vex/vxnmif.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmph.f` & `pythonSCHED-1.9.0/src/Vex/vxnmph.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmpo.f` & `pythonSCHED-1.9.0/src/Vex/vxnmpo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmpr.f` & `pythonSCHED-1.9.0/src/Vex/vxnmpr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmrl.f` & `pythonSCHED-1.9.0/src/Vex/vxnmrl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmsi.f` & `pythonSCHED-1.9.0/src/Vex/vxnmsi.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmtr.f` & `pythonSCHED-1.9.0/src/Vex/vxnmtr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxnmxx.f` & `pythonSCHED-1.9.0/src/Vex/vxnmxx.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxrl16.f` & `pythonSCHED-1.9.0/src/Vex/vxrl16.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxrl8.f` & `pythonSCHED-1.9.0/src/Vex/vxrl8.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxs2df.f` & `pythonSCHED-1.9.0/src/Vex/vxs2df.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxs2md.f` & `pythonSCHED-1.9.0/src/Vex/vxs2md.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxs2vl.f` & `pythonSCHED-1.9.0/src/Vex/vxs2vl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxsch.f` & `pythonSCHED-1.9.0/src/Vex/vxsch.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxschk.f` & `pythonSCHED-1.9.0/src/Vex/vxschk.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxscns.f` & `pythonSCHED-1.9.0/src/Vex/vxscns.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxsort.f` & `pythonSCHED-1.9.0/src/Vex/vxsort.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxstky.f` & `pythonSCHED-1.9.0/src/Vex/vxstky.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxstli.f` & `pythonSCHED-1.9.0/src/Vex/vxstli.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxstnm.f` & `pythonSCHED-1.9.0/src/Vex/vxstnm.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxsudt.f` & `pythonSCHED-1.9.0/src/Vex/vxsudt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtels.f` & `pythonSCHED-1.9.0/src/Vex/vxtels.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxton2.f` & `pythonSCHED-1.9.0/src/Vex/vxton2.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtone.f` & `pythonSCHED-1.9.0/src/Vex/vxtone.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtrafq.f` & `pythonSCHED-1.9.0/src/Vex/vxtrafq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtraif.f` & `pythonSCHED-1.9.0/src/Vex/vxtraif.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtramd.f` & `pythonSCHED-1.9.0/src/Vex/vxtramd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtran.f` & `pythonSCHED-1.9.0/src/Vex/vxtran.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxtraph.f` & `pythonSCHED-1.9.0/src/Vex/vxtraph.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxunql.f` & `pythonSCHED-1.9.0/src/Vex/vxunql.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxvbrx.f` & `pythonSCHED-1.9.0/src/Vex/vxvbrx.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwran.f` & `pythonSCHED-1.9.0/src/Vex/vxwran.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrbb.f` & `pythonSCHED-1.9.0/src/Vex/vxwrbb.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrda.f` & `pythonSCHED-1.9.0/src/Vex/vxwrda.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrex.f` & `pythonSCHED-1.9.0/src/Vex/vxwrex.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrfq.f` & `pythonSCHED-1.9.0/src/Vex/vxwrfq.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrgl.f` & `pythonSCHED-1.9.0/src/Vex/vxwrgl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrhp.f` & `pythonSCHED-1.9.0/src/Vex/vxwrhp.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrif.f` & `pythonSCHED-1.9.0/src/Vex/vxwrif.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrmd.f` & `pythonSCHED-1.9.0/src/Vex/vxwrmd.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrph.f` & `pythonSCHED-1.9.0/src/Vex/vxwrph.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrpo.f` & `pythonSCHED-1.9.0/src/Vex/vxwrpo.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrpr.f` & `pythonSCHED-1.9.0/src/Vex/vxwrpr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrrl.f` & `pythonSCHED-1.9.0/src/Vex/vxwrrl.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrsi.f` & `pythonSCHED-1.9.0/src/Vex/vxwrsi.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrst.f` & `pythonSCHED-1.9.0/src/Vex/vxwrst.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrsu.f` & `pythonSCHED-1.9.0/src/Vex/vxwrsu.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrt.f` & `pythonSCHED-1.9.0/src/Vex/vxwrt.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/Vex/vxwrtr.f` & `pythonSCHED-1.9.0/src/Vex/vxwrtr.f`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/__init__.py` & `pythonSCHED-1.9.0/src/pysched/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/frequency_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/frequency_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/line_rest_frequency_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/line_rest_frequency_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/peak_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/peak_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/phase_center_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/phase_center_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/satellite_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/satellite_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/scan_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/scan_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/setup_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/setup_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/setup_file_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/setup_file_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/source_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/source_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/source_plot_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/source_plot_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/catalog/station_catalog.py` & `pythonSCHED-1.9.0/src/pysched/catalog/station_catalog.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/dbbc_patching.py` & `pythonSCHED-1.9.0/src/pysched/dbbc_patching.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/key.py` & `pythonSCHED-1.9.0/src/pysched/key.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/plot.py` & `pythonSCHED-1.9.0/src/pysched/plot.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/plot_toolbar.py` & `pythonSCHED-1.9.0/src/pysched/plot_toolbar.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/__init__.py` & `pythonSCHED-1.9.0/src/pysched/sched/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/addgeo_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/addgeo_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/addpeak_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/addpeak_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/bbcalt_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/bbcalt_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/bbcdbbc_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/bbcdbbc_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/bbcemerlin_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/bbcemerlin_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/chkdbbc_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/chkdbbc_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/chkset_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/chkset_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/defaults_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/defaults_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/geochk_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/geochk_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/geomake_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/geomake_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/getcor_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/getcor_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/getcov_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/getcov_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/getfreq_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/getfreq_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/getset_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/getset_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/getsta_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/getsta_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/gettim_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/gettim_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/gintent_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/gintent_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/gmkscn_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/gmkscn_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/ifdbbc_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/ifdbbc_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/infdb_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/infdb_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/input_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/input_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/invla_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/invla_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/makescn_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/makescn_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/makeseg_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/makeseg_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/optcells_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/optcells_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/opthas_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/opthas_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/opthiel_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/opthiel_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/optnone_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/optnone_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/optskd_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/optskd_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/optupt_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/optupt_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/pcread_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/pcread_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/rdpeak_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/rdpeak_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/rdset_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/rdset_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/rfreq_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/rfreq_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/satini_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/satini_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/schdefs_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/schdefs_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/schfiles_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/schfiles_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/schin_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/schin_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/schopt_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/schopt_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/schrep_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/schrep_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/scndup_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/scndup_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/setbbc_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/setbbc_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/setdefs_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/setdefs_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/setexpnd_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/setexpnd_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/srread_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/srread_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/stmsg_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/stmsg_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/stread_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/stread_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/sttant_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/sttant_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/times_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/times_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/sched/vexout_module.py` & `pythonSCHED-1.9.0/src/pysched/sched/vexout_module.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/update_catalogs.py` & `pythonSCHED-1.9.0/src/pysched/update_catalogs.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/util.py` & `pythonSCHED-1.9.0/src/pysched/util.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/version.py` & `pythonSCHED-1.9.0/src/pysched/version.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/vex.py` & `pythonSCHED-1.9.0/src/pysched/vex.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/pysched/vex_scans.py` & `pythonSCHED-1.9.0/src/pysched/vex_scans.py`

 * *Files identical despite different names*

### Comparing `pythonSCHED-1.8.2/src/sched.py` & `pythonSCHED-1.9.0/src/sched.py`

 * *Files identical despite different names*

