# Comparing `tmp/qsimcirq-0.9.2.tar.gz` & `tmp/qsimcirq-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qsimcirq-0.9.2.tar", last modified: Thu Apr 22 19:54:02 2021, max compression
+gzip compressed data, was "dist/qsimcirq-0.9.5.tar", last modified: Tue May 25 14:47:37 2021, max compression
```

## Comparing `qsimcirq-0.9.2.tar` & `qsimcirq-0.9.5.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/
-drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/pybind_interface/
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      435 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/pybind_interface/Makefile
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    31251 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/pybind_interface/pybind_main.cpp
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    12585 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/pybind_interface/pybind_main.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      598 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/pybind_interface/Dockerfile
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     5568 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/README.md
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2872 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/setup.py
-drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/qsimcirq.egg-info/
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)        1 2021-04-22 19:54:01.000000 qsimcirq-0.9.2/qsimcirq.egg-info/dependency_links.txt
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1256 2021-04-22 19:54:01.000000 qsimcirq-0.9.2/qsimcirq.egg-info/SOURCES.txt
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       23 2021-04-22 19:54:01.000000 qsimcirq-0.9.2/qsimcirq.egg-info/top_level.txt
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       59 2021-04-22 19:54:01.000000 qsimcirq-0.9.2/qsimcirq.egg-info/requires.txt
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)        1 2021-04-22 19:54:01.000000 qsimcirq-0.9.2/qsimcirq.egg-info/not-zip-safe
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6922 2021-04-22 19:54:01.000000 qsimcirq-0.9.2/qsimcirq.egg-info/PKG-INFO
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      461 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/CMakeLists.txt
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       38 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/setup.cfg
-drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/lib/
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2429 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/util.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1227 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/umux.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3632 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/parfor.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   137184 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitary_calculator_sse.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   181634 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/simulator_sse.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     4004 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/statespace.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    32390 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/fuser_mqubit.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     8932 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/statespace_basic.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3178 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitaryspace_basic.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3177 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/vectorspace.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     8763 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/BUILD
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1088 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/io.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    57330 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/gates_cirq.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     4400 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/expect.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    13886 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/qtrajectory.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    25807 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitary_calculator_basic.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   226274 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/simulator_avx.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6960 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/matrix.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1765 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitaryspace.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    13650 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/statespace_sse.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    17842 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/gates_qsim.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1080 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/simmux.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     7219 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/run_qsim.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   169133 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitary_calculator_avx.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    14001 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/circuit_qsim_parser.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    14640 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/statespace_avx.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3496 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitaryspace_sse.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     4429 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/fuser.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      846 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/formux.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3570 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/circuit_noisy.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2023 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/seqfor.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1783 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/io_file.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    11374 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/channels_cirq.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      986 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/circuit.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    36429 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/simulator_basic.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    18808 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/hybrid.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2983 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/bitstring.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1886 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/channel.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     9354 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/gate_appl.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3514 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/unitaryspace_avx.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3891 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/run_qsimh.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2257 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/bits.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    13847 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/fuser_basic.h
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6228 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/lib/gate.h
-drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/qsimcirq/
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2763 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/qsimcirq/qsimh_simulator.py
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       91 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/qsimcirq/__init__.py
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       59 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/qsimcirq/py.typed
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    14736 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/qsimcirq/qsim_circuit.py
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    19715 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/qsimcirq/qsim_simulator.py
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6922 2021-04-22 19:54:02.000000 qsimcirq-0.9.2/PKG-INFO
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      149 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/requirements.txt
--rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       82 2021-04-22 19:52:17.000000 qsimcirq-0.9.2/MANIFEST.in
+drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/
+drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/pybind_interface/
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      598 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/pybind_interface/Dockerfile
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    12585 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/pybind_interface/pybind_main.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    31251 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/pybind_interface/pybind_main.cpp
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      435 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/pybind_interface/Makefile
+drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq/
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2913 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/qsimcirq/qsimh_simulator.py
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       91 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/qsimcirq/__init__.py
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    21328 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/qsimcirq/qsim_simulator.py
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       59 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/qsimcirq/py.typed
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    16302 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/qsimcirq/qsim_circuit.py
+drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       23 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/top_level.txt
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       85 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/requires.txt
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1361 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/SOURCES.txt
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)        1 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/not-zip-safe
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6922 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/PKG-INFO
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)        1 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/qsimcirq.egg-info/dependency_links.txt
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      461 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/CMakeLists.txt
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3134 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/setup.py
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      175 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/requirements.txt
+drwxrwsr-x   0 kbuilder  (1000) kokoro    (1003)        0 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/lib/
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2429 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/util.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   137179 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitary_calculator_sse.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    11374 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/channels_cirq.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2983 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/bitstring.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3560 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitaryspace_avx512.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    14001 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/circuit_qsim_parser.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3177 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/vectorspace.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      986 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/circuit.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1088 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/io.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   259761 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/simulator_avx512.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     9354 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/gate_appl.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    36429 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/simulator_basic.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2023 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/seqfor.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   191199 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitary_calculator_avx512.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3891 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/run_qsimh.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   181634 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/simulator_sse.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6960 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/matrix.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     8932 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/statespace_basic.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     4004 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/statespace.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3632 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/parfor.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     2257 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/bits.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     4400 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/expect.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1765 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitaryspace.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)      846 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/formux.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    18808 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/hybrid.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3496 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitaryspace_sse.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    14640 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/statespace_avx.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    17842 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/gates_qsim.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    13886 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/qtrajectory.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1422 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/umux.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    13650 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/statespace_sse.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3570 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/circuit_noisy.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   169123 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitary_calculator_avx.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    14486 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/statespace_avx512.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1224 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/simmux.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)   226274 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/simulator_avx.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     7219 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/run_qsim.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    13847 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/fuser_basic.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3178 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitaryspace_basic.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     9660 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/BUILD
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1783 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/io_file.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    25807 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitary_calculator_basic.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    32390 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/fuser_mqubit.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     4429 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/fuser.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     1886 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/channel.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)    57330 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/gates_cirq.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     3514 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/unitaryspace_avx.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6233 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/lib/gate.h
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       82 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/MANIFEST.in
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     6922 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/PKG-INFO
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)       38 2021-05-25 14:47:37.000000 qsimcirq-0.9.5/setup.cfg
+-rw-rw-r--   0 kbuilder  (1000) kokoro    (1003)     5568 2021-05-25 14:45:52.000000 qsimcirq-0.9.5/README.md
```

### Comparing `qsimcirq-0.9.2/pybind_interface/pybind_main.cpp` & `qsimcirq-0.9.5/pybind_interface/pybind_main.cpp`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/pybind_interface/pybind_main.h` & `qsimcirq-0.9.5/pybind_interface/pybind_main.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/pybind_interface/Dockerfile` & `qsimcirq-0.9.5/pybind_interface/Dockerfile`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/README.md` & `qsimcirq-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/setup.py` & `qsimcirq-0.9.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,90 +6,93 @@
 
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 from distutils.version import LooseVersion
 
 
 class CMakeExtension(Extension):
-
-  def __init__(self, name, sourcedir=''):
-    Extension.__init__(self, name, sources=[])
-    self.sourcedir = os.path.abspath(sourcedir)
+    def __init__(self, name, sourcedir=""):
+        Extension.__init__(self, name, sources=[])
+        self.sourcedir = os.path.abspath(sourcedir)
 
 
 class CMakeBuild(build_ext):
-
-  def run(self):
-    try:
-      out = subprocess.check_output(['cmake', '--version'])
-    except OSError:
-      raise RuntimeError(
-          'CMake must be installed to build the following extensions: ' +
-          ', '.join(e.name for e in self.extensions))
-
-    if platform.system() == 'Windows':
-      cmake_version = LooseVersion(
-          re.search(r'version\s*([\d.]+)', out.decode()).group(1))
-      if cmake_version < '3.1.0':
-        raise RuntimeError('CMake >= 3.1.0 is required on Windows')
-
-    for ext in self.extensions:
-      self.build_extension(ext)
-
-  def build_extension(self, ext):
-    extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
-    cmake_args = [
-        '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + extdir,
-        '-DPYTHON_EXECUTABLE=' + sys.executable
-    ]
-
-    cfg = 'Debug' if self.debug else 'Release'
-    build_args = ['--config', cfg]
-
-    if platform.system() == 'Windows':
-      cmake_args += [
-          '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}'.format(cfg.upper(), extdir)
-      ]
-      if sys.maxsize > 2**32:
-        cmake_args += ['-A', 'x64']
-      build_args += ['--', '/m']
-    else:
-      cmake_args += ['-DCMAKE_BUILD_TYPE=' + cfg]
-      build_args += ['--', '-j2']
-
-    env = os.environ.copy()
-    env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(
-        env.get('CXXFLAGS', ''), self.distribution.get_version())
-    if not os.path.exists(self.build_temp):
-      os.makedirs(self.build_temp)
-    subprocess.check_call(
-        ['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
-    subprocess.check_call(
-        ['cmake', '--build', '.'] + build_args, cwd=self.build_temp)
+    def run(self):
+        try:
+            out = subprocess.check_output(["cmake", "--version"])
+        except OSError:
+            raise RuntimeError(
+                "CMake must be installed to build the following extensions: "
+                + ", ".join(e.name for e in self.extensions)
+            )
+
+        if platform.system() == "Windows":
+            cmake_version = LooseVersion(
+                re.search(r"version\s*([\d.]+)", out.decode()).group(1)
+            )
+            if cmake_version < "3.1.0":
+                raise RuntimeError("CMake >= 3.1.0 is required on Windows")
+
+        for ext in self.extensions:
+            self.build_extension(ext)
+
+    def build_extension(self, ext):
+        extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
+        cmake_args = [
+            "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + extdir,
+            "-DPYTHON_EXECUTABLE=" + sys.executable,
+        ]
+
+        cfg = "Debug" if self.debug else "Release"
+        build_args = ["--config", cfg]
+
+        if platform.system() == "Windows":
+            cmake_args += [
+                "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}".format(cfg.upper(), extdir)
+            ]
+            if sys.maxsize > 2 ** 32:
+                cmake_args += ["-A", "x64"]
+            build_args += ["--", "/m"]
+        else:
+            cmake_args += ["-DCMAKE_BUILD_TYPE=" + cfg]
+            build_args += ["--", "-j2"]
+
+        env = os.environ.copy()
+        env["CXXFLAGS"] = '{} -DVERSION_INFO=\\"{}\\"'.format(
+            env.get("CXXFLAGS", ""), self.distribution.get_version()
+        )
+        if not os.path.exists(self.build_temp):
+            os.makedirs(self.build_temp)
+        subprocess.check_call(
+            ["cmake", ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env
+        )
+        subprocess.check_call(
+            ["cmake", "--build", "."] + build_args, cwd=self.build_temp
+        )
 
 
-requirements = open('requirements.txt').readlines()
+requirements = open("requirements.txt").readlines()
 
-description = ('Schrödinger and Schrödinger-Feynman simulators for quantum circuits.')
+description = "Schrödinger and Schrödinger-Feynman simulators for quantum circuits."
 
 # README file as long_description.
-long_description = open('README.md', encoding='utf-8').read()
+long_description = open("README.md", encoding="utf-8").read()
 
-__version__ = '0.9.2'
+__version__ = "0.9.5"
 
 setup(
-    name='qsimcirq',
+    name="qsimcirq",
     version=__version__,
-    author='Vamsi Krishna Devabathini',
-    author_email='devabathini92@gmail.com',
-    python_requires='>=3.3.0',
+    author="Vamsi Krishna Devabathini",
+    author_email="devabathini92@gmail.com",
+    python_requires=">=3.3.0",
     install_requires=requirements,
-    license='Apache 2',
+    license="Apache 2",
     description=description,
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    ext_modules=[CMakeExtension('qsimcirq/qsim')],
+    long_description_content_type="text/markdown",
+    ext_modules=[CMakeExtension("qsimcirq/qsim")],
     cmdclass=dict(build_ext=CMakeBuild),
     zip_safe=False,
-    packages=['qsimcirq'],
-    package_data={'qsimcirq': ['py.typed']},
+    packages=["qsimcirq"],
+    package_data={"qsimcirq": ["py.typed"]},
 )
```

### Comparing `qsimcirq-0.9.2/qsimcirq.egg-info/SOURCES.txt` & `qsimcirq-0.9.5/qsimcirq.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,30 @@
 lib/parfor.h
 lib/qtrajectory.h
 lib/run_qsim.h
 lib/run_qsimh.h
 lib/seqfor.h
 lib/simmux.h
 lib/simulator_avx.h
+lib/simulator_avx512.h
 lib/simulator_basic.h
 lib/simulator_sse.h
 lib/statespace.h
 lib/statespace_avx.h
+lib/statespace_avx512.h
 lib/statespace_basic.h
 lib/statespace_sse.h
 lib/umux.h
 lib/unitary_calculator_avx.h
+lib/unitary_calculator_avx512.h
 lib/unitary_calculator_basic.h
 lib/unitary_calculator_sse.h
 lib/unitaryspace.h
 lib/unitaryspace_avx.h
+lib/unitaryspace_avx512.h
 lib/unitaryspace_basic.h
 lib/unitaryspace_sse.h
 lib/util.h
 lib/vectorspace.h
 pybind_interface/Dockerfile
 pybind_interface/Makefile
 pybind_interface/pybind_main.cpp
```

### Comparing `qsimcirq-0.9.2/qsimcirq.egg-info/PKG-INFO` & `qsimcirq-0.9.5/qsimcirq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsimcirq
-Version: 0.9.2
+Version: 0.9.5
 Summary: Schrödinger and Schrödinger-Feynman simulators for quantum circuits.
 Home-page: UNKNOWN
 Author: Vamsi Krishna Devabathini
 Author-email: devabathini92@gmail.com
 License: Apache 2
 Description: # qsim and qsimh
```

### Comparing `qsimcirq-0.9.2/lib/util.h` & `qsimcirq-0.9.5/lib/util.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/umux.h` & `qsimcirq-0.9.5/lib/umux.h`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,23 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef UMUX_H_
 #define UMUX_H_
 
-#ifdef __AVX2__
+#ifdef __AVX512F__
+# include "unitary_calculator_avx512.h"
+  namespace qsim {
+  namespace unitary {
+    template <typename For>
+    using UnitaryCalculator = UnitaryCalculatorAVX512<For>;
+  }
+  }
+#elif __AVX2__
 # include "unitary_calculator_avx.h"
   namespace qsim {
   namespace unitary {
     template <typename For>
     using UnitaryCalculator = UnitaryCalculatorAVX<For>;
   }
   }
```

### Comparing `qsimcirq-0.9.2/lib/parfor.h` & `qsimcirq-0.9.5/lib/parfor.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitary_calculator_sse.h` & `qsimcirq-0.9.5/lib/unitary_calculator_sse.h`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     for_.Run(size * size2, f, matrix, ms, xss, size, raw_size, rstate);
   }
 
   void ApplyGate1L(const std::vector<unsigned>& qs,
                    const fp_type* matrix, Unitary& state) const {
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(3);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned m = 0; m < 2; ++m) {
@@ -479,15 +479,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -566,15 +566,15 @@
     for_.Run(size * size2, f, w, ms, xss, qs[0], size, raw_size, rstate);
   }
 
   void ApplyGate2LL(const std::vector<unsigned>& qs,
                     const fp_type* matrix, Unitary& state) const {
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -754,15 +754,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -859,15 +859,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -1050,15 +1050,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 8; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -1160,15 +1160,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -1351,15 +1351,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(11);
+    auto s = UnitarySpace::Create(6);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 16; ++i) {
       for (unsigned m = 0; m < 32; ++m) {
@@ -1461,15 +1461,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(10);
+    auto s = UnitarySpace::Create(5);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 8; ++i) {
       for (unsigned m = 0; m < 32; ++m) {
@@ -1654,15 +1654,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(13);
+    auto s = UnitarySpace::Create(7);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 32; ++i) {
       for (unsigned m = 0; m < 64; ++m) {
@@ -1764,15 +1764,15 @@
         }
       }
       xss[i] = a;
     }
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(12);
+    auto s = UnitarySpace::Create(6);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 16; ++i) {
       for (unsigned m = 0; m < 64; ++m) {
@@ -1989,15 +1989,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 2; ++m) {
@@ -2091,15 +2091,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(3);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned m = 0; m < 2; ++m) {
@@ -2205,15 +2205,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(3);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned m = 0; m < 2; ++m) {
@@ -2438,15 +2438,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -2558,15 +2558,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -2691,15 +2691,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -2799,15 +2799,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -2914,15 +2914,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -3148,15 +3148,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 8; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -3272,15 +3272,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -3409,15 +3409,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -3535,15 +3535,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -3669,15 +3669,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -3904,15 +3904,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(10);
+    auto s = UnitarySpace::Create(5);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 16; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -4028,15 +4028,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 8; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -4165,15 +4165,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 8; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -4295,15 +4295,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -4433,15 +4433,15 @@
       }
     }
 
     emaskh = ~emaskh ^ 3;
 
     unsigned p[4];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m128* w = (__m128*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
```

### Comparing `qsimcirq-0.9.2/lib/simulator_sse.h` & `qsimcirq-0.9.5/lib/simulator_sse.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/statespace.h` & `qsimcirq-0.9.5/lib/statespace.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/fuser_mqubit.h` & `qsimcirq-0.9.5/lib/fuser_mqubit.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/statespace_basic.h` & `qsimcirq-0.9.5/lib/statespace_basic.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitaryspace_basic.h` & `qsimcirq-0.9.5/lib/unitaryspace_basic.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/vectorspace.h` & `qsimcirq-0.9.5/lib/vectorspace.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/BUILD` & `qsimcirq-0.9.5/lib/BUILD`

 * *Files 12% similar despite different names*

```diff
@@ -29,26 +29,30 @@
         "parfor.h",
         "qtrajectory.h",
         "run_qsim.h",
         "run_qsimh.h",
         "seqfor.h",
         "simmux.h",
         "simulator_avx.h",
+        "simulator_avx512.h",
         "simulator_basic.h",
         "simulator_sse.h",
         "statespace_avx.h",
+        "statespace_avx512.h",
         "statespace_basic.h",
         "statespace_sse.h",
         "statespace.h",
         "umux.h",
         "unitaryspace.h",
         "unitaryspace_avx.h",
+        "unitaryspace_avx512.h",
         "unitaryspace_basic.h",
         "unitaryspace_sse.h",
         "unitary_calculator_avx.h",
+        "unitary_calculator_avx512.h",
         "unitary_calculator_basic.h",
         "unitary_calculator_sse.h",
         "util.h",
         "vectorspace.h",
     ],
 )
 
@@ -71,18 +75,20 @@
         "io_file.h",
         "matrix.h",
         "parfor.h",
         "run_qsim.h",
         "seqfor.h",
         "simmux.h",
         "simulator_avx.h",
+        "simulator_avx512.h",
         "simulator_basic.h",
         "simulator_sse.h",
         "statespace.h",
         "statespace_avx.h",
+        "statespace_avx512.h",
         "statespace_basic.h",
         "statespace_sse.h",
         "umux.h",
         "unitaryspace.h",
         "unitaryspace_avx.h",
         "unitaryspace_basic.h",
         "unitaryspace_sse.h",
@@ -114,18 +120,20 @@
         "io_file.h",
         "matrix.h",
         "parfor.h",
         "run_qsimh.h",
         "seqfor.h",
         "simmux.h",
         "simulator_avx.h",
+        "simulator_avx512.h",
         "simulator_basic.h",
         "simulator_sse.h",
         "statespace.h",
         "statespace_avx.h",
+        "statespace_avx512.h",
         "statespace_basic.h",
         "statespace_sse.h",
         "util.h",
         "vectorspace.h",
     ],
 )
 
@@ -327,14 +335,23 @@
     deps = [
         ":statespace",
         ":util",
     ],
 )
 
 cc_library(
+    name = "statespace_avx512",
+    hdrs = ["statespace_avx512.h"],
+    deps = [
+        ":statespace",
+        ":util",
+    ],
+)
+
+cc_library(
     name = "statespace_basic",
     hdrs = ["statespace_basic.h"],
     deps = [
         ":statespace",
         ":util",
     ],
 )
@@ -356,14 +373,23 @@
     deps = [
         ":bits",
         ":statespace_avx",
     ],
 )
 
 cc_library(
+    name = "simulator_avx512",
+    hdrs = ["simulator_avx512.h"],
+    deps = [
+        ":bits",
+        ":statespace_avx512",
+    ],
+)
+
+cc_library(
     name = "simulator_basic",
     hdrs = ["simulator_basic.h"],
     deps = [
         ":bits",
         ":statespace_basic",
     ],
 )
@@ -379,14 +405,15 @@
 
 # All three state-vector simulators with multiplexer
 cc_library(
     name = "simulator",
     hdrs = ["simmux.h"],
     deps = [
         ":simulator_avx",
+        ":simulator_avx512",
         ":simulator_basic",
         ":simulator_sse",
     ],
 )
 
 # Hybrid simulator
 cc_library(
@@ -447,14 +474,20 @@
 cc_library(
     name = "unitaryspace_avx",
     hdrs = ["unitaryspace_avx.h"],
     deps = [":unitaryspace"],
 )
 
 cc_library(
+    name = "unitaryspace_avx512",
+    hdrs = ["unitaryspace_avx512.h"],
+    deps = [":unitaryspace"],
+)
+
+cc_library(
     name = "unitaryspace_basic",
     hdrs = ["unitaryspace_basic.h"],
     deps = [":unitaryspace"],
 )
 
 cc_library(
     name = "unitaryspace_sse",
@@ -470,14 +503,23 @@
     deps = [
         ":bits",
         ":unitaryspace_avx"
     ],
 )
 
 cc_library(
+    name = "unitary_calculator_avx512",
+    hdrs = ["unitary_calculator_avx512.h"],
+    deps = [
+        ":bits",
+        ":unitaryspace_avx512"
+    ],
+)
+
+cc_library(
     name = "unitary_calculator_basic",
     hdrs = ["unitary_calculator_basic.h"],
     deps = [
         ":bits",
         ":unitaryspace_basic"
     ],
 )
@@ -494,11 +536,12 @@
 ### Unitary mux header ###
 
 cc_library(
     name = "umux",
     hdrs = ["umux.h"],
     deps = [
         ":unitary_calculator_avx",
+        ":unitary_calculator_avx512",
         ":unitary_calculator_basic",
         ":unitary_calculator_sse",
     ],
 )
```

### Comparing `qsimcirq-0.9.2/lib/io.h` & `qsimcirq-0.9.5/lib/io.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/gates_cirq.h` & `qsimcirq-0.9.5/lib/gates_cirq.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/expect.h` & `qsimcirq-0.9.5/lib/expect.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/qtrajectory.h` & `qsimcirq-0.9.5/lib/qtrajectory.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitary_calculator_basic.h` & `qsimcirq-0.9.5/lib/unitary_calculator_basic.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/simulator_avx.h` & `qsimcirq-0.9.5/lib/simulator_avx.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/matrix.h` & `qsimcirq-0.9.5/lib/matrix.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitaryspace.h` & `qsimcirq-0.9.5/lib/unitaryspace.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/statespace_sse.h` & `qsimcirq-0.9.5/lib/statespace_sse.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/gates_qsim.h` & `qsimcirq-0.9.5/lib/gates_qsim.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/simmux.h` & `qsimcirq-0.9.5/lib/simmux.h`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef SIMMUX_H_
 #define SIMMUX_H_
 
-#ifdef __AVX2__
+#ifdef __AVX512F__
+# include "simulator_avx512.h"
+  namespace qsim {
+    template <typename For>
+    using Simulator = SimulatorAVX512<For>;
+  }
+#elif __AVX2__
 # include "simulator_avx.h"
   namespace qsim {
     template <typename For>
     using Simulator = SimulatorAVX<For>;
   }
 #elif __SSE4_1__
 # include "simulator_sse.h"
```

### Comparing `qsimcirq-0.9.2/lib/run_qsim.h` & `qsimcirq-0.9.5/lib/run_qsim.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitary_calculator_avx.h` & `qsimcirq-0.9.5/lib/unitary_calculator_avx.h`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
   }
 
   void ApplyGate1L(const std::vector<unsigned>& qs,
                    const fp_type* matrix, Unitary& state) const {
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -509,15 +509,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -605,15 +605,15 @@
   }
 
   void ApplyGate2LL(const std::vector<unsigned>& qs,
                     const fp_type* matrix, Unitary& state) const {
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -801,15 +801,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -915,15 +915,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1011,15 +1011,15 @@
   }
 
   void ApplyGate3LLL(const std::vector<unsigned>& qs,
                      const fp_type* matrix, Unitary& state) const {
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1207,15 +1207,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(10);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1326,15 +1326,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1440,15 +1440,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1639,15 +1639,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(12);
+    auto s = UnitarySpace::Create(6);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1758,15 +1758,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(11);
+    auto s = UnitarySpace::Create(6);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -1877,15 +1877,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(10);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -2077,15 +2077,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(14);
+    auto s = UnitarySpace::Create(7);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -2196,15 +2196,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(13);
+    auto s = UnitarySpace::Create(7);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -2315,15 +2315,15 @@
       }
       xss[i] = a;
     }
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(12);
+    auto s = UnitarySpace::Create(6);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -2547,15 +2547,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 2; ++i) {
       for (unsigned m = 0; m < 2; ++m) {
@@ -2650,15 +2650,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -2773,15 +2773,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(4);
+    auto s = UnitarySpace::Create(2);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -3014,15 +3014,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 4; ++i) {
       for (unsigned m = 0; m < 4; ++m) {
@@ -3135,15 +3135,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -3277,15 +3277,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -3394,15 +3394,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -3517,15 +3517,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(5);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -3758,15 +3758,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 8; ++i) {
       for (unsigned m = 0; m < 8; ++m) {
@@ -3883,15 +3883,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -4029,15 +4029,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -4164,15 +4164,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -4306,15 +4306,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(7);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -4423,15 +4423,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -4546,15 +4546,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(6);
+    auto s = UnitarySpace::Create(3);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -4787,15 +4787,15 @@
       emaskh |= uint64_t{1} << q;
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
 
-    auto s = UnitarySpace::Create(11);
+    auto s = UnitarySpace::Create(6);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 16; ++i) {
       for (unsigned m = 0; m < 16; ++m) {
@@ -4912,15 +4912,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(10);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -5058,15 +5058,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[1];
 
-    auto s = UnitarySpace::Create(10);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]);
 
     for (unsigned i = 0; i < 1; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -5197,15 +5197,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -5343,15 +5343,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[3];
 
-    auto s = UnitarySpace::Create(9);
+    auto s = UnitarySpace::Create(5);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]);
 
     for (unsigned i = 0; i < 3; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -5478,15 +5478,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
@@ -5620,15 +5620,15 @@
     }
 
     emaskh = ~emaskh ^ 7;
 
     unsigned p[8];
     __m256i idx[7];
 
-    auto s = UnitarySpace::Create(8);
+    auto s = UnitarySpace::Create(4);
     __m256* w = (__m256*) s.get();
     fp_type* wf = (fp_type*) w;
 
     unsigned qmask = (1 << qs[0]) | (1 << qs[1]) | (1 << qs[2]);
 
     for (unsigned i = 0; i < 7; ++i) {
       for (unsigned j = 0; j < 8; ++j) {
```

### Comparing `qsimcirq-0.9.2/lib/circuit_qsim_parser.h` & `qsimcirq-0.9.5/lib/circuit_qsim_parser.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/statespace_avx.h` & `qsimcirq-0.9.5/lib/statespace_avx.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitaryspace_sse.h` & `qsimcirq-0.9.5/lib/unitaryspace_sse.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/fuser.h` & `qsimcirq-0.9.5/lib/fuser.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/formux.h` & `qsimcirq-0.9.5/lib/formux.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/circuit_noisy.h` & `qsimcirq-0.9.5/lib/circuit_noisy.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/seqfor.h` & `qsimcirq-0.9.5/lib/seqfor.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/io_file.h` & `qsimcirq-0.9.5/lib/io_file.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/channels_cirq.h` & `qsimcirq-0.9.5/lib/channels_cirq.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/circuit.h` & `qsimcirq-0.9.5/lib/circuit.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/simulator_basic.h` & `qsimcirq-0.9.5/lib/simulator_basic.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/hybrid.h` & `qsimcirq-0.9.5/lib/hybrid.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/bitstring.h` & `qsimcirq-0.9.5/lib/bitstring.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/channel.h` & `qsimcirq-0.9.5/lib/channel.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/gate_appl.h` & `qsimcirq-0.9.5/lib/gate_appl.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/unitaryspace_avx.h` & `qsimcirq-0.9.5/lib/unitaryspace_avx.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/run_qsimh.h` & `qsimcirq-0.9.5/lib/run_qsimh.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/bits.h` & `qsimcirq-0.9.5/lib/bits.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/fuser_basic.h` & `qsimcirq-0.9.5/lib/fuser_basic.h`

 * *Files identical despite different names*

### Comparing `qsimcirq-0.9.2/lib/gate.h` & `qsimcirq-0.9.5/lib/gate.h`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
           typename M = Matrix<typename Gate::fp_type>>
 inline Gate CreateGate(unsigned time, Qubits&& qubits, M&& matrix = {},
                        std::vector<typename Gate::fp_type>&& params = {}) {
   Gate gate = {GateDef::kind, time, std::forward<Qubits>(qubits), {}, 0,
                std::move(params), std::forward<M>(matrix), false, false};
 
   if (GateDef::kind != gate::kMeasurement) {
-    switch (qubits.size()) {
+    switch (gate.qubits.size()) {
     case 1:
       break;
     case 2:
       if (gate.qubits[0] > gate.qubits[1]) {
         gate.swapped = true;
         std::swap(gate.qubits[0], gate.qubits[1]);
         if (!GateDef::symmetric) {
```

### Comparing `qsimcirq-0.9.2/qsimcirq/qsimh_simulator.py` & `qsimcirq-0.9.5/qsimcirq/qsimh_simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,65 +10,65 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Union, Sequence
 
-from cirq import study, ops, protocols, circuits, value,  SimulatesAmplitudes
+from cirq import study, ops, protocols, circuits, value, SimulatesAmplitudes
 
 from qsimcirq import qsim
 import qsimcirq.qsim_circuit as qsimc
 
 
 class QSimhSimulator(SimulatesAmplitudes):
+    def __init__(self, qsimh_options: dict = {}):
+        """Creates a new QSimhSimulator using the given options.
 
-  def __init__(self, qsimh_options: dict = {}):
-    """Creates a new QSimhSimulator using the given options.
-    
-    Args:
-        qsim_options: A map of circuit options for the simulator. These will be
-            applied to all circuits run using this simulator. Accepted keys and
-            their behavior are as follows:
-                - 'k': Comma-separated list of ints. Indices of "part 1" qubits.
-                - 'p': int (>= 0). Number of "prefix" gates.
-                - 'r': int (>= 0). Number of "root" gates.
-                - 't': int (> 0). Number of threads to run on. Default: 1.
-                - 'v': int (>= 0). Log verbosity. Default: 0.
-                - 'w': int (>= 0). Prefix value.
-            See qsim/docs/usage.md for more details on these options.
-    """
-    self.qsimh_options = {'t': 1, 'f': 2, 'v': 0}
-    self.qsimh_options.update(qsimh_options)
-
-  def compute_amplitudes_sweep(
-      self,
-      program: circuits.Circuit,
-      bitstrings: Sequence[int],
-      params: study.Sweepable,
-      qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
-  ) -> Sequence[Sequence[complex]]:
-
-    if not isinstance(program, qsimc.QSimCircuit):
-      program = qsimc.QSimCircuit(program, device=program.device)
-
-    n_qubits = len(program.all_qubits())
-    # qsim numbers qubits in reverse order from cirq
-    bitstrings = [format(bitstring, 'b').zfill(n_qubits)[::-1]
-                  for bitstring in bitstrings]
-
-    options = {'i': '\n'.join(bitstrings)}
-    options.update(self.qsimh_options)
-    param_resolvers = study.to_resolvers(params)
-
-    trials_results = []
-    for prs in param_resolvers:
-
-      solved_circuit = protocols.resolve_parameters(program, prs)
-
-      options['c'] = solved_circuit.translate_cirq_to_qsim(qubit_order)
-
-      options.update(self.qsimh_options)
-      amplitudes = qsim.qsimh_simulate(options)
-      trials_results.append(amplitudes)
+        Args:
+            qsim_options: A map of circuit options for the simulator. These will be
+                applied to all circuits run using this simulator. Accepted keys and
+                their behavior are as follows:
+                    - 'k': Comma-separated list of ints. Indices of "part 1" qubits.
+                    - 'p': int (>= 0). Number of "prefix" gates.
+                    - 'r': int (>= 0). Number of "root" gates.
+                    - 't': int (> 0). Number of threads to run on. Default: 1.
+                    - 'v': int (>= 0). Log verbosity. Default: 0.
+                    - 'w': int (>= 0). Prefix value.
+                See qsim/docs/usage.md for more details on these options.
+        """
+        self.qsimh_options = {"t": 1, "f": 2, "v": 0}
+        self.qsimh_options.update(qsimh_options)
+
+    def compute_amplitudes_sweep(
+        self,
+        program: circuits.Circuit,
+        bitstrings: Sequence[int],
+        params: study.Sweepable,
+        qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
+    ) -> Sequence[Sequence[complex]]:
+
+        if not isinstance(program, qsimc.QSimCircuit):
+            program = qsimc.QSimCircuit(program, device=program.device)
+
+        n_qubits = len(program.all_qubits())
+        # qsim numbers qubits in reverse order from cirq
+        bitstrings = [
+            format(bitstring, "b").zfill(n_qubits)[::-1] for bitstring in bitstrings
+        ]
+
+        options = {"i": "\n".join(bitstrings)}
+        options.update(self.qsimh_options)
+        param_resolvers = study.to_resolvers(params)
+
+        trials_results = []
+        for prs in param_resolvers:
+
+            solved_circuit = protocols.resolve_parameters(program, prs)
+
+            options["c"] = solved_circuit.translate_cirq_to_qsim(qubit_order)
+
+            options.update(self.qsimh_options)
+            amplitudes = qsim.qsimh_simulate(options)
+            trials_results.append(amplitudes)
 
-    return trials_results
+        return trials_results
```

### Comparing `qsimcirq-0.9.2/qsimcirq/qsim_circuit.py` & `qsimcirq-0.9.5/qsimcirq/qsim_circuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,404 +18,405 @@
 import cirq
 from qsimcirq import qsim
 from typing import Dict, Union
 
 
 # List of parameter names that appear in valid Cirq protos.
 GATE_PARAMS = [
-  'exponent', 'phase_exponent', 'global_shift',
-  'x_exponent', 'z_exponent', 'axis_phase_exponent',
-  'phi', 'theta'
+    "exponent",
+    "phase_exponent",
+    "global_shift",
+    "x_exponent",
+    "z_exponent",
+    "axis_phase_exponent",
+    "phi",
+    "theta",
 ]
 
 
 def _cirq_gate_kind(gate: cirq.ops.Gate):
-  if isinstance(gate, cirq.ops.ControlledGate):
-    return _cirq_gate_kind(gate.sub_gate)
-  if isinstance(gate, cirq.ops.identity.IdentityGate):
-    if gate.num_qubits() == 1:
-      return qsim.kI1
-    if gate.num_qubits() == 2:
-      return qsim.kI2
-    if gate.num_qubits() <= 6:
-      return qsim.kI
-    raise NotImplementedError(
-      f'Received identity on {gate.num_qubits()} qubits; '
-      + 'only up to 6-qubit gates are supported.')
-  if isinstance(gate, cirq.ops.XPowGate):
-    # cirq.rx also uses this path.
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kX
-    return qsim.kXPowGate
-  if isinstance(gate, cirq.ops.YPowGate):
-    # cirq.ry also uses this path.
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kY
-    return qsim.kYPowGate
-  if isinstance(gate, cirq.ops.ZPowGate):
-    # cirq.rz also uses this path.
-    if gate.global_shift == 0:
-      if gate.exponent == 1:
-        return qsim.kZ
-      if gate.exponent == 0.5:
-        return qsim.kS
-      if gate.exponent == 0.25:
-        return qsim.kT
-    return qsim.kZPowGate
-  if isinstance(gate, cirq.ops.HPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kH
-    return qsim.kHPowGate
-  if isinstance(gate, cirq.ops.CZPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kCZ
-    return qsim.kCZPowGate
-  if isinstance(gate, cirq.ops.CXPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kCX
-    return qsim.kCXPowGate
-  if isinstance(gate, cirq.ops.PhasedXPowGate):
-    return qsim.kPhasedXPowGate
-  if isinstance(gate, cirq.ops.PhasedXZGate):
-    return qsim.kPhasedXZGate
-  if isinstance(gate, cirq.ops.XXPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kXX
-    return qsim.kXXPowGate
-  if isinstance(gate, cirq.ops.YYPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kYY
-    return qsim.kYYPowGate
-  if isinstance(gate, cirq.ops.ZZPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kZZ
-    return qsim.kZZPowGate
-  if isinstance(gate, cirq.ops.SwapPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kSWAP
-    return qsim.kSwapPowGate
-  if isinstance(gate, cirq.ops.ISwapPowGate):
-    # cirq.riswap also uses this path.
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kISWAP
-    return qsim.kISwapPowGate
-  if isinstance(gate, cirq.ops.PhasedISwapPowGate):
-    # cirq.givens also uses this path.
-    return qsim.kPhasedISwapPowGate
-  if isinstance(gate, cirq.ops.FSimGate):
-    return qsim.kFSimGate
-  if isinstance(gate, cirq.ops.TwoQubitDiagonalGate):
-    return qsim.kTwoQubitDiagonalGate
-  if isinstance(gate, cirq.ops.ThreeQubitDiagonalGate):
-    return qsim.kThreeQubitDiagonalGate
-  if isinstance(gate, cirq.ops.CCZPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kCCZ
-    return qsim.kCCZPowGate
-  if isinstance(gate, cirq.ops.CCXPowGate):
-    if gate.exponent == 1 and gate.global_shift == 0:
-      return qsim.kCCX
-    return qsim.kCCXPowGate
-  if isinstance(gate, cirq.ops.CSwapGate):
-    return qsim.kCSwapGate
-  if isinstance(gate, cirq.ops.MatrixGate):
-    if gate.num_qubits() <= 6:
-      return qsim.kMatrixGate
-    raise NotImplementedError(
-      f'Received matrix on {gate.num_qubits()} qubits; '
-      + 'only up to 6-qubit gates are supported.')
-  if isinstance(gate, cirq.ops.MeasurementGate):
-    # needed to inherit SimulatesSamples in sims
-    return qsim.kMeasurement
-  # Unrecognized gates will be decomposed.
-  return None
+    if isinstance(gate, cirq.ops.ControlledGate):
+        return _cirq_gate_kind(gate.sub_gate)
+    if isinstance(gate, cirq.ops.identity.IdentityGate):
+        # Identity gates will decompose to no-ops.
+        pass
+    if isinstance(gate, cirq.ops.XPowGate):
+        # cirq.rx also uses this path.
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kX
+        return qsim.kXPowGate
+    if isinstance(gate, cirq.ops.YPowGate):
+        # cirq.ry also uses this path.
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kY
+        return qsim.kYPowGate
+    if isinstance(gate, cirq.ops.ZPowGate):
+        # cirq.rz also uses this path.
+        if gate.global_shift == 0:
+            if gate.exponent == 1:
+                return qsim.kZ
+            if gate.exponent == 0.5:
+                return qsim.kS
+            if gate.exponent == 0.25:
+                return qsim.kT
+        return qsim.kZPowGate
+    if isinstance(gate, cirq.ops.HPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kH
+        return qsim.kHPowGate
+    if isinstance(gate, cirq.ops.CZPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kCZ
+        return qsim.kCZPowGate
+    if isinstance(gate, cirq.ops.CXPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kCX
+        return qsim.kCXPowGate
+    if isinstance(gate, cirq.ops.PhasedXPowGate):
+        return qsim.kPhasedXPowGate
+    if isinstance(gate, cirq.ops.PhasedXZGate):
+        return qsim.kPhasedXZGate
+    if isinstance(gate, cirq.ops.XXPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kXX
+        return qsim.kXXPowGate
+    if isinstance(gate, cirq.ops.YYPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kYY
+        return qsim.kYYPowGate
+    if isinstance(gate, cirq.ops.ZZPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kZZ
+        return qsim.kZZPowGate
+    if isinstance(gate, cirq.ops.SwapPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kSWAP
+        return qsim.kSwapPowGate
+    if isinstance(gate, cirq.ops.ISwapPowGate):
+        # cirq.riswap also uses this path.
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kISWAP
+        return qsim.kISwapPowGate
+    if isinstance(gate, cirq.ops.PhasedISwapPowGate):
+        # cirq.givens also uses this path.
+        return qsim.kPhasedISwapPowGate
+    if isinstance(gate, cirq.ops.FSimGate):
+        return qsim.kFSimGate
+    if isinstance(gate, cirq.ops.TwoQubitDiagonalGate):
+        return qsim.kTwoQubitDiagonalGate
+    if isinstance(gate, cirq.ops.ThreeQubitDiagonalGate):
+        return qsim.kThreeQubitDiagonalGate
+    if isinstance(gate, cirq.ops.CCZPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kCCZ
+        return qsim.kCCZPowGate
+    if isinstance(gate, cirq.ops.CCXPowGate):
+        if gate.exponent == 1 and gate.global_shift == 0:
+            return qsim.kCCX
+        return qsim.kCCXPowGate
+    if isinstance(gate, cirq.ops.CSwapGate):
+        return qsim.kCSwapGate
+    if isinstance(gate, cirq.ops.MatrixGate):
+        if gate.num_qubits() <= 6:
+            return qsim.kMatrixGate
+        raise NotImplementedError(
+            f"Received matrix on {gate.num_qubits()} qubits; "
+            + "only up to 6-qubit gates are supported."
+        )
+    if isinstance(gate, cirq.ops.MeasurementGate):
+        # needed to inherit SimulatesSamples in sims
+        return qsim.kMeasurement
+    # Unrecognized gates will be decomposed.
+    return None
 
 
 def _control_details(gate: cirq.ops.ControlledGate, qubits):
-  control_qubits = []
-  control_values = []
-  # TODO: support qudit control
-  for i, cvs in enumerate(gate.control_values):
-    if 0 in cvs and 1 in cvs:
-      # This qubit does not affect control.
-      continue
-    elif 0 not in cvs and 1 not in cvs:
-      # This gate will never trigger.
-      warnings.warn(f'Gate has no valid control value: {gate}', RuntimeWarning)
-      return (None, None)
-    # Either 0 or 1 is in cvs, but not both.
-    control_qubits.append(qubits[i])
-    if 0 in cvs:
-      control_values.append(0)
-    elif 1 in cvs:
-      control_values.append(1)
+    control_qubits = []
+    control_values = []
+    # TODO: support qudit control
+    for i, cvs in enumerate(gate.control_values):
+        if 0 in cvs and 1 in cvs:
+            # This qubit does not affect control.
+            continue
+        elif 0 not in cvs and 1 not in cvs:
+            # This gate will never trigger.
+            warnings.warn(f"Gate has no valid control value: {gate}", RuntimeWarning)
+            return (None, None)
+        # Either 0 or 1 is in cvs, but not both.
+        control_qubits.append(qubits[i])
+        if 0 in cvs:
+            control_values.append(0)
+        elif 1 in cvs:
+            control_values.append(1)
 
-  return (control_qubits, control_values)
+    return (control_qubits, control_values)
 
 
 def add_op_to_opstring(
     qsim_op: cirq.GateOperation,
     qubit_to_index_dict: Dict[cirq.Qid, int],
     opstring: qsim.OpString,
 ):
-  """Adds an operation to an opstring (observable).
+    """Adds an operation to an opstring (observable).
 
-  Raises:
-    ValueError if qsim_op is not a single-qubit Pauli (I, X, Y, or Z).
-  """
-  qsim_gate = qsim_op.gate
-  gate_kind = _cirq_gate_kind(qsim_gate)
-  if gate_kind not in {qsim.kX, qsim.kY, qsim.kZ, qsim.kI1}:
-    raise ValueError(f'OpString should only have Paulis; got {gate_kind}')
-  if len(qsim_op.qubits) != 1:
-    raise ValueError(
-      f'OpString ops should have 1 qubit; got {len(qsim_op.qubits)}')
-
-  is_controlled = isinstance(qsim_gate, cirq.ops.ControlledGate)
-  if is_controlled:
-    raise ValueError(f'OpString ops should not be controlled.')
+    Raises:
+      ValueError if qsim_op is not a single-qubit Pauli (I, X, Y, or Z).
+    """
+    qsim_gate = qsim_op.gate
+    gate_kind = _cirq_gate_kind(qsim_gate)
+    if gate_kind not in {qsim.kX, qsim.kY, qsim.kZ, qsim.kI1}:
+        raise ValueError(f"OpString should only have Paulis; got {gate_kind}")
+    if len(qsim_op.qubits) != 1:
+        raise ValueError(f"OpString ops should have 1 qubit; got {len(qsim_op.qubits)}")
+
+    is_controlled = isinstance(qsim_gate, cirq.ops.ControlledGate)
+    if is_controlled:
+        raise ValueError(f"OpString ops should not be controlled.")
 
-  qubits = [qubit_to_index_dict[q] for q in qsim_op.qubits]
-  qsim.add_gate_to_opstring(gate_kind, qubits, opstring)
+    qubits = [qubit_to_index_dict[q] for q in qsim_op.qubits]
+    qsim.add_gate_to_opstring(gate_kind, qubits, opstring)
 
 
 def add_op_to_circuit(
     qsim_op: cirq.GateOperation,
     time: int,
     qubit_to_index_dict: Dict[cirq.Qid, int],
-    circuit: Union[qsim.Circuit, qsim.NoisyCircuit]
+    circuit: Union[qsim.Circuit, qsim.NoisyCircuit],
 ):
-  """Adds an operation to a noisy or noiseless circuit."""
-  qsim_gate = qsim_op.gate
-  gate_kind = _cirq_gate_kind(qsim_gate)
-  qubits = [qubit_to_index_dict[q] for q in qsim_op.qubits]
-
-  qsim_qubits = qubits
-  is_controlled = isinstance(qsim_gate, cirq.ops.ControlledGate)
-  if is_controlled:
-    control_qubits, control_values = _control_details(qsim_gate, qubits)
-    if control_qubits is None:
-      # This gate has no valid control, and will be omitted.
-      return
-
-    if qsim_gate.num_qubits() > 4:
-      raise NotImplementedError(
-      f'Received control gate on {gate.num_qubits()} target qubits; '
-      + 'only up to 4-qubit gates are supported.')
-
-    qsim_qubits = qubits[qsim_gate.num_controls():]
-    qsim_gate = qsim_gate.sub_gate
-
-  if (gate_kind == qsim.kTwoQubitDiagonalGate or
-      gate_kind == qsim.kThreeQubitDiagonalGate):
-    if isinstance(circuit, qsim.Circuit):
-      qsim.add_diagonal_gate(
-        time, qsim_qubits, qsim_gate._diag_angles_radians, circuit)
-    else:
-      qsim.add_diagonal_gate_channel(
-        time, qsim_qubits, qsim_gate._diag_angles_radians, circuit)
-  elif gate_kind == qsim.kMatrixGate:
-    m = [
-      val for i in list(cirq.unitary(qsim_gate).flat)
-      for val in [i.real, i.imag]
-    ]
-    if isinstance(circuit, qsim.Circuit):
-      qsim.add_matrix_gate(time, qsim_qubits, m, circuit)
-    else:
-      qsim.add_matrix_gate_channel(time, qsim_qubits, m, circuit)
-  else:
-    params = {}
-    for p, val in vars(qsim_gate).items():
-      key = p.strip('_')
-      if key not in GATE_PARAMS:
-        continue
-      if isinstance(val, (int, float, np.integer, np.floating)):
-        params[key] = val
-      else:
-        raise ValueError('Parameters must be numeric.')
-    if isinstance(circuit, qsim.Circuit):
-      qsim.add_gate(gate_kind, time, qsim_qubits, params, circuit)
+    """Adds an operation to a noisy or noiseless circuit."""
+    qsim_gate = qsim_op.gate
+    gate_kind = _cirq_gate_kind(qsim_gate)
+    qubits = [qubit_to_index_dict[q] for q in qsim_op.qubits]
+
+    qsim_qubits = qubits
+    is_controlled = isinstance(qsim_gate, cirq.ops.ControlledGate)
+    if is_controlled:
+        control_qubits, control_values = _control_details(qsim_gate, qubits)
+        if control_qubits is None:
+            # This gate has no valid control, and will be omitted.
+            return
+
+        num_targets = qsim_gate.num_qubits() - qsim_gate.num_controls()
+        if num_targets > 4:
+            raise NotImplementedError(
+                f"Received control gate on {num_targets} target qubits; "
+                + "only up to 4-qubit gates are supported."
+            )
+
+        qsim_qubits = qubits[qsim_gate.num_controls() :]
+        qsim_gate = qsim_gate.sub_gate
+
+    if (
+        gate_kind == qsim.kTwoQubitDiagonalGate
+        or gate_kind == qsim.kThreeQubitDiagonalGate
+    ):
+        if isinstance(circuit, qsim.Circuit):
+            qsim.add_diagonal_gate(
+                time, qsim_qubits, qsim_gate._diag_angles_radians, circuit
+            )
+        else:
+            qsim.add_diagonal_gate_channel(
+                time, qsim_qubits, qsim_gate._diag_angles_radians, circuit
+            )
+    elif gate_kind == qsim.kMatrixGate:
+        m = [
+            val for i in list(cirq.unitary(qsim_gate).flat) for val in [i.real, i.imag]
+        ]
+        if isinstance(circuit, qsim.Circuit):
+            qsim.add_matrix_gate(time, qsim_qubits, m, circuit)
+        else:
+            qsim.add_matrix_gate_channel(time, qsim_qubits, m, circuit)
     else:
-      qsim.add_gate_channel(gate_kind, time, qsim_qubits, params, circuit)
+        params = {}
+        for p, val in vars(qsim_gate).items():
+            key = p.strip("_")
+            if key not in GATE_PARAMS:
+                continue
+            if isinstance(val, (int, float, np.integer, np.floating)):
+                params[key] = val
+            else:
+                raise ValueError("Parameters must be numeric.")
+        if isinstance(circuit, qsim.Circuit):
+            qsim.add_gate(gate_kind, time, qsim_qubits, params, circuit)
+        else:
+            qsim.add_gate_channel(gate_kind, time, qsim_qubits, params, circuit)
 
-  if is_controlled:
-    if isinstance(circuit, qsim.Circuit):
-      qsim.control_last_gate(control_qubits, control_values, circuit)
-    else:
-      qsim.control_last_gate_channel(control_qubits, control_values, circuit)
+    if is_controlled:
+        if isinstance(circuit, qsim.Circuit):
+            qsim.control_last_gate(control_qubits, control_values, circuit)
+        else:
+            qsim.control_last_gate_channel(control_qubits, control_values, circuit)
 
 
 class QSimCircuit(cirq.Circuit):
+    def __init__(
+        self,
+        cirq_circuit: cirq.Circuit,
+        device: cirq.devices = cirq.devices.UNCONSTRAINED_DEVICE,
+        allow_decomposition: bool = False,
+    ):
+
+        if allow_decomposition:
+            super().__init__([], device=device)
+            for moment in cirq_circuit:
+                for op in moment:
+                    # This should call decompose on the gates
+                    self.append(op)
+        else:
+            super().__init__(cirq_circuit, device=device)
 
-  def __init__(self,
-               cirq_circuit: cirq.Circuit,
-               device: cirq.devices = cirq.devices.UNCONSTRAINED_DEVICE,
-               allow_decomposition: bool = False):
-
-    if allow_decomposition:
-      super().__init__([], device=device)
-      for moment in cirq_circuit:
-        for op in moment:
-          # This should call decompose on the gates
-          self.append(op)
-    else:
-      super().__init__(cirq_circuit, device=device)
-
-  def __eq__(self, other):
-    if not isinstance(other, QSimCircuit):
-      return False
-    # equality is tested, for the moment, for cirq.Circuit
-    return super().__eq__(other)
-
-  def _resolve_parameters_(
-      self,
-      param_resolver: cirq.study.ParamResolver,
-      recursive: bool = True
-  ):
-    return QSimCircuit(
-      cirq.resolve_parameters(super(), param_resolver, recursive),
-      device=self.device,
-    )
-
-  def translate_cirq_to_qsim(
-      self,
-      qubit_order: cirq.ops.QubitOrderOrList = cirq.ops.QubitOrder.DEFAULT
-  ) -> qsim.Circuit:
-    """
+    def __eq__(self, other):
+        if not isinstance(other, QSimCircuit):
+            return False
+        # equality is tested, for the moment, for cirq.Circuit
+        return super().__eq__(other)
+
+    def _resolve_parameters_(
+        self, param_resolver: cirq.study.ParamResolver, recursive: bool = True
+    ):
+        return QSimCircuit(
+            cirq.resolve_parameters(super(), param_resolver, recursive),
+            device=self.device,
+        )
+
+    def translate_cirq_to_qsim(
+        self, qubit_order: cirq.ops.QubitOrderOrList = cirq.ops.QubitOrder.DEFAULT
+    ) -> qsim.Circuit:
+        """
         Translates this Cirq circuit to the qsim representation.
         :qubit_order: Ordering of qubits
         :return: a C++ qsim Circuit object
         """
 
-    qsim_circuit = qsim.Circuit()
-    qubits = self.all_qubits()
-    qsim_circuit.num_qubits = len(qubits)
-    ordered_qubits = cirq.ops.QubitOrder.as_qubit_order(qubit_order).order_for(
-      qubits)
-
-    # qsim numbers qubits in reverse order from cirq
-    ordered_qubits = list(reversed(ordered_qubits))
-
-    def has_qsim_kind(op: cirq.ops.GateOperation):
-      return _cirq_gate_kind(op.gate) != None
-
-    def to_matrix(op: cirq.ops.GateOperation):
-      mat = cirq.protocols.unitary(op.gate, None)
-      if mat is None:
-          return NotImplemented
-
-      return cirq.ops.MatrixGate(mat).on(*op.qubits)
-
-    qubit_to_index_dict = {q: i for i, q in enumerate(ordered_qubits)}
-    time_offset = 0
-    for moment in self:
-      ops_by_gate = [
-        cirq.decompose(op, fallback_decomposer=to_matrix, keep=has_qsim_kind)
-        for op in moment
-      ]
-      moment_length = max(len(gate_ops) for gate_ops in ops_by_gate)
-
-      # Gates must be added in time order.
-      for gi in range(moment_length):
-        for gate_ops in ops_by_gate:
-          if gi >= len(gate_ops):
-            continue
-          qsim_op = gate_ops[gi]
-          time = time_offset + gi
-          gate_kind = _cirq_gate_kind(qsim_op.gate)
-          add_op_to_circuit(qsim_op, time, qubit_to_index_dict, qsim_circuit)
-      time_offset += moment_length
-
-    return qsim_circuit
-
-
-  def translate_cirq_to_qtrajectory(
-      self,
-      qubit_order: cirq.ops.QubitOrderOrList = cirq.ops.QubitOrder.DEFAULT
-  ) -> qsim.NoisyCircuit:
-    """
+        qsim_circuit = qsim.Circuit()
+        ordered_qubits = cirq.ops.QubitOrder.as_qubit_order(qubit_order).order_for(
+            self.all_qubits()
+        )
+        qsim_circuit.num_qubits = len(ordered_qubits)
+
+        # qsim numbers qubits in reverse order from cirq
+        ordered_qubits = list(reversed(ordered_qubits))
+
+        def has_qsim_kind(op: cirq.ops.GateOperation):
+            return _cirq_gate_kind(op.gate) != None
+
+        def to_matrix(op: cirq.ops.GateOperation):
+            mat = cirq.protocols.unitary(op.gate, None)
+            if mat is None:
+                return NotImplemented
+
+            return cirq.ops.MatrixGate(mat).on(*op.qubits)
+
+        qubit_to_index_dict = {q: i for i, q in enumerate(ordered_qubits)}
+        time_offset = 0
+        for moment in self:
+            ops_by_gate = [
+                cirq.decompose(op, fallback_decomposer=to_matrix, keep=has_qsim_kind)
+                for op in moment
+            ]
+            moment_length = max((len(gate_ops) for gate_ops in ops_by_gate), default=0)
+
+            # Gates must be added in time order.
+            for gi in range(moment_length):
+                for gate_ops in ops_by_gate:
+                    if gi >= len(gate_ops):
+                        continue
+                    qsim_op = gate_ops[gi]
+                    time = time_offset + gi
+                    gate_kind = _cirq_gate_kind(qsim_op.gate)
+                    add_op_to_circuit(qsim_op, time, qubit_to_index_dict, qsim_circuit)
+            time_offset += moment_length
+
+        return qsim_circuit
+
+    def translate_cirq_to_qtrajectory(
+        self, qubit_order: cirq.ops.QubitOrderOrList = cirq.ops.QubitOrder.DEFAULT
+    ) -> qsim.NoisyCircuit:
+        """
         Translates this noisy Cirq circuit to the qsim representation.
         :qubit_order: Ordering of qubits
         :return: a C++ qsim NoisyCircuit object
         """
-    qsim_ncircuit = qsim.NoisyCircuit()
-    ordered_qubits = cirq.ops.QubitOrder.as_qubit_order(qubit_order).order_for(
-        self.all_qubits())
-
-    # qsim numbers qubits in reverse order from cirq
-    ordered_qubits = list(reversed(ordered_qubits))
-
-    qsim_ncircuit.num_qubits = len(ordered_qubits)
-
-    def has_qsim_kind(op: cirq.ops.GateOperation):
-      return _cirq_gate_kind(op.gate) != None
-
-    def to_matrix(op: cirq.ops.GateOperation):
-      mat = cirq.unitary(op.gate, None)
-      if mat is None:
-          return NotImplemented
-
-      return cirq.ops.MatrixGate(mat).on(*op.qubits)
-
-    qubit_to_index_dict = {q: i for i, q in enumerate(ordered_qubits)}
-    time_offset = 0
-    for moment in self:
-      moment_length = 0
-      ops_by_gate = []
-      ops_by_mix = []
-      ops_by_channel = []
-      # Capture ops of each type in the appropriate list.
-      for qsim_op in moment:
-        if cirq.has_unitary(qsim_op) or cirq.is_measurement(qsim_op):
-          oplist = cirq.decompose(
-            qsim_op, fallback_decomposer=to_matrix, keep=has_qsim_kind)
-          ops_by_gate.append(oplist)
-          moment_length = max(moment_length, len(oplist))
-          pass
-        elif cirq.has_mixture(qsim_op):
-          ops_by_mix.append(qsim_op)
-          moment_length = max(moment_length, 1)
-          pass
-        elif cirq.has_channel(qsim_op):
-          ops_by_channel.append(qsim_op)
-          moment_length = max(moment_length, 1)
-          pass
-        else:
-          raise ValueError(f'Encountered unparseable op: {qsim_op}')
-
-      # Gates must be added in time order.
-      for gi in range(moment_length):
-        # Handle gate output.
-        for gate_ops in ops_by_gate:
-          if gi >= len(gate_ops):
-            continue
-          qsim_op = gate_ops[gi]
-          time = time_offset + gi
-          gate_kind = _cirq_gate_kind(qsim_op.gate)
-          add_op_to_circuit(qsim_op, time, qubit_to_index_dict, qsim_ncircuit)
-        # Handle mixture output.
-        for mixture in ops_by_mix:
-          mixdata = []
-          for prob, mat in cirq.mixture(mixture):
-            square_mat = np.reshape(mat, (int(np.sqrt(mat.size)), -1))
-            unitary = cirq.is_unitary(square_mat)
-            # Package matrix into a qsim-friendly format.
-            mat = np.reshape(mat, (-1,)).astype(np.complex64, copy=False)
-            mixdata.append((prob, mat.view(np.float32), unitary))
-          qubits = [qubit_to_index_dict[q] for q in mixture.qubits]
-          qsim.add_channel(time_offset, qubits, mixdata, qsim_ncircuit)
-        # Handle channel output.
-        for channel in ops_by_channel:
-          chdata = []
-          for i, mat in enumerate(cirq.channel(channel)):
-            square_mat = np.reshape(mat, (int(np.sqrt(mat.size)), -1))
-            unitary = cirq.is_unitary(square_mat)
-            singular_vals = np.linalg.svd(square_mat)[1]
-            lower_bound_prob = min(singular_vals) ** 2
-            # Package matrix into a qsim-friendly format.
-            mat = np.reshape(mat, (-1,)).astype(np.complex64, copy=False)
-            chdata.append((lower_bound_prob, mat.view(np.float32), unitary))
-          qubits = [qubit_to_index_dict[q] for q in channel.qubits]
-          qsim.add_channel(time_offset, qubits, chdata, qsim_ncircuit)
-      time_offset += moment_length
+        qsim_ncircuit = qsim.NoisyCircuit()
+        ordered_qubits = cirq.ops.QubitOrder.as_qubit_order(qubit_order).order_for(
+            self.all_qubits()
+        )
+
+        # qsim numbers qubits in reverse order from cirq
+        ordered_qubits = list(reversed(ordered_qubits))
+
+        qsim_ncircuit.num_qubits = len(ordered_qubits)
+
+        def has_qsim_kind(op: cirq.ops.GateOperation):
+            return _cirq_gate_kind(op.gate) != None
+
+        def to_matrix(op: cirq.ops.GateOperation):
+            mat = cirq.unitary(op.gate, None)
+            if mat is None:
+                return NotImplemented
+
+            return cirq.ops.MatrixGate(mat).on(*op.qubits)
+
+        qubit_to_index_dict = {q: i for i, q in enumerate(ordered_qubits)}
+        time_offset = 0
+        for moment in self:
+            moment_length = 0
+            ops_by_gate = []
+            ops_by_mix = []
+            ops_by_channel = []
+            # Capture ops of each type in the appropriate list.
+            for qsim_op in moment:
+                if cirq.has_unitary(qsim_op) or cirq.is_measurement(qsim_op):
+                    oplist = cirq.decompose(
+                        qsim_op, fallback_decomposer=to_matrix, keep=has_qsim_kind
+                    )
+                    ops_by_gate.append(oplist)
+                    moment_length = max(moment_length, len(oplist))
+                    pass
+                elif cirq.has_mixture(qsim_op):
+                    ops_by_mix.append(qsim_op)
+                    moment_length = max(moment_length, 1)
+                    pass
+                elif cirq.has_channel(qsim_op):
+                    ops_by_channel.append(qsim_op)
+                    moment_length = max(moment_length, 1)
+                    pass
+                else:
+                    raise ValueError(f"Encountered unparseable op: {qsim_op}")
+
+            # Gates must be added in time order.
+            for gi in range(moment_length):
+                # Handle gate output.
+                for gate_ops in ops_by_gate:
+                    if gi >= len(gate_ops):
+                        continue
+                    qsim_op = gate_ops[gi]
+                    time = time_offset + gi
+                    gate_kind = _cirq_gate_kind(qsim_op.gate)
+                    add_op_to_circuit(qsim_op, time, qubit_to_index_dict, qsim_ncircuit)
+                # Handle mixture output.
+                for mixture in ops_by_mix:
+                    mixdata = []
+                    for prob, mat in cirq.mixture(mixture):
+                        square_mat = np.reshape(mat, (int(np.sqrt(mat.size)), -1))
+                        unitary = cirq.is_unitary(square_mat)
+                        # Package matrix into a qsim-friendly format.
+                        mat = np.reshape(mat, (-1,)).astype(np.complex64, copy=False)
+                        mixdata.append((prob, mat.view(np.float32), unitary))
+                    qubits = [qubit_to_index_dict[q] for q in mixture.qubits]
+                    qsim.add_channel(time_offset, qubits, mixdata, qsim_ncircuit)
+                # Handle channel output.
+                for channel in ops_by_channel:
+                    chdata = []
+                    for i, mat in enumerate(cirq.channel(channel)):
+                        square_mat = np.reshape(mat, (int(np.sqrt(mat.size)), -1))
+                        unitary = cirq.is_unitary(square_mat)
+                        singular_vals = np.linalg.svd(square_mat)[1]
+                        lower_bound_prob = min(singular_vals) ** 2
+                        # Package matrix into a qsim-friendly format.
+                        mat = np.reshape(mat, (-1,)).astype(np.complex64, copy=False)
+                        chdata.append((lower_bound_prob, mat.view(np.float32), unitary))
+                    qubits = [qubit_to_index_dict[q] for q in channel.qubits]
+                    qsim.add_channel(time_offset, qubits, chdata, qsim_ncircuit)
+            time_offset += moment_length
 
-    return qsim_ncircuit
+        return qsim_ncircuit
```

### Comparing `qsimcirq-0.9.2/qsimcirq/qsim_simulator.py` & `qsimcirq-0.9.5/qsimcirq/qsim_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,493 +11,506 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from cirq import (
-  circuits,
-  linalg,
-  ops,
-  protocols,
-  sim,
-  study,
-  value,
-  SimulatesAmplitudes,
-  SimulatesFinalState,
-  SimulatesSamples,
+    circuits,
+    linalg,
+    ops,
+    protocols,
+    sim,
+    study,
+    value,
+    SimulatesAmplitudes,
+    SimulatesFinalState,
+    SimulatesSamples,
 )
 
+# TODO: import from cirq directly when fix is released
+from cirq.sim.simulator import SimulatesExpectationValues
+
 import numpy as np
 
 from qsimcirq import qsim
 import qsimcirq.qsim_circuit as qsimc
 
 
 class QSimSimulatorState(sim.StateVectorSimulatorState):
-
-    def __init__(self,
-                 qsim_data: np.ndarray,
-                 qubit_map: Dict[ops.Qid, int]):
-      state_vector = qsim_data.view(np.complex64)
-      super().__init__(state_vector=state_vector, qubit_map=qubit_map)
+    def __init__(self, qsim_data: np.ndarray, qubit_map: Dict[ops.Qid, int]):
+        state_vector = qsim_data.view(np.complex64)
+        super().__init__(state_vector=state_vector, qubit_map=qubit_map)
 
 
 class QSimSimulatorTrialResult(sim.StateVectorTrialResult):
-
-    def __init__(self,
-                 params: study.ParamResolver,
-                 measurements: Dict[str, np.ndarray],
-                 final_simulator_state: QSimSimulatorState):
-      super().__init__(params=params,
-                       measurements=measurements,
-                       final_simulator_state=final_simulator_state)
+    def __init__(
+        self,
+        params: study.ParamResolver,
+        measurements: Dict[str, np.ndarray],
+        final_simulator_state: QSimSimulatorState,
+    ):
+        super().__init__(
+            params=params,
+            measurements=measurements,
+            final_simulator_state=final_simulator_state,
+        )
 
 
 # This should probably live in Cirq...
 # TODO: update to support CircuitOperations.
 def _needs_trajectories(circuit: circuits.Circuit) -> bool:
-  """Checks if the circuit requires trajectory simulation."""
-  for op in circuit.all_operations():
-    test_op = (
-      op if not protocols.is_parameterized(op)
-      else protocols.resolve_parameters(
-          op, {param: 1 for param in protocols.parameter_names(op)}
+    """Checks if the circuit requires trajectory simulation."""
+    for op in circuit.all_operations():
+        test_op = (
+            op
+            if not protocols.is_parameterized(op)
+            else protocols.resolve_parameters(
+                op, {param: 1 for param in protocols.parameter_names(op)}
+            )
         )
-    )
-    if not (protocols.has_unitary(test_op) or protocols.is_measurement(test_op)):
-      return True
-  return False
-
-
-class QSimSimulator(SimulatesSamples, SimulatesAmplitudes, SimulatesFinalState):
-
-  def __init__(self, qsim_options: dict = {},
-               seed: value.RANDOM_STATE_OR_SEED_LIKE = None):
-    """Creates a new QSimSimulator using the given options and seed.
-
-    Args:
-        qsim_options: A map of circuit options for the simulator. These will be
-            applied to all circuits run using this simulator. Accepted keys and
-            their behavior are as follows:
-                - 'f': int (> 0). Maximum size of fused gates. Default: 2.
-                - 'r': int (> 0). Noisy repetitions (see below). Default: 1.
-                - 't': int (> 0). Number of threads to run on. Default: 1.
-                - 'v': int (>= 0). Log verbosity. Default: 0.
-            See qsim/docs/usage.md for more details on these options.
-            "Noisy repetitions" specifies how many repetitions to aggregate
-            over when calculating expectation values for a noisy circuit.
-            Note that this does not apply to other simulation types.
-        seed: A random state or seed object, as defined in cirq.value.
-
-    Raises:
-        ValueError if internal keys 'c', 'i' or 's' are included in 'qsim_options'.
-    """
-    if any(k in qsim_options for k in ('c', 'i', 's')):
-      raise ValueError(
-          'Keys {"c", "i", "s"} are reserved for internal use and cannot be '
-          'used in QSimCircuit instantiation.'
-      )
-    self._prng = value.parse_random_state(seed)
-    self.qsim_options = {'t': 1, 'f': 2, 'v': 0, 'r': 1}
-    self.qsim_options.update(qsim_options)
-
-  def get_seed(self):
-    # Limit seed size to 32-bit integer for C++ conversion.
-    return self._prng.randint(2 ** 31 - 1)
+        if not (protocols.has_unitary(test_op) or protocols.is_measurement(test_op)):
+            return True
+    return False
+
+
+class QSimSimulator(
+    SimulatesSamples,
+    SimulatesAmplitudes,
+    SimulatesFinalState,
+    SimulatesExpectationValues,
+):
+    def __init__(
+        self, qsim_options: dict = {}, seed: value.RANDOM_STATE_OR_SEED_LIKE = None
+    ):
+        """Creates a new QSimSimulator using the given options and seed.
+
+        Args:
+            qsim_options: A map of circuit options for the simulator. These will be
+                applied to all circuits run using this simulator. Accepted keys and
+                their behavior are as follows:
+                    - 'f': int (> 0). Maximum size of fused gates. Default: 2.
+                    - 'r': int (> 0). Noisy repetitions (see below). Default: 1.
+                    - 't': int (> 0). Number of threads to run on. Default: 1.
+                    - 'v': int (>= 0). Log verbosity. Default: 0.
+                See qsim/docs/usage.md for more details on these options.
+                "Noisy repetitions" specifies how many repetitions to aggregate
+                over when calculating expectation values for a noisy circuit.
+                Note that this does not apply to other simulation types.
+            seed: A random state or seed object, as defined in cirq.value.
+
+        Raises:
+            ValueError if internal keys 'c', 'i' or 's' are included in 'qsim_options'.
+        """
+        if any(k in qsim_options for k in ("c", "i", "s")):
+            raise ValueError(
+                'Keys {"c", "i", "s"} are reserved for internal use and cannot be '
+                "used in QSimCircuit instantiation."
+            )
+        self._prng = value.parse_random_state(seed)
+        self.qsim_options = {"t": 1, "f": 2, "v": 0, "r": 1}
+        self.qsim_options.update(qsim_options)
+
+    def get_seed(self):
+        # Limit seed size to 32-bit integer for C++ conversion.
+        return self._prng.randint(2 ** 31 - 1)
 
-  def _run(
+    def _run(
         self,
         circuit: circuits.Circuit,
         param_resolver: study.ParamResolver,
-        repetitions: int
-  ) -> Dict[str, np.ndarray]:
-    """Run a simulation, mimicking quantum hardware.
-
-    Args:
-        program: The circuit to simulate.
-        param_resolver: Parameters to run with the program.
-        repetitions: Number of times to repeat the run.
-
-    Returns:
-        A dictionary from measurement gate key to measurement
-        results.
-    """
-    param_resolver = param_resolver or study.ParamResolver({})
-    solved_circuit = protocols.resolve_parameters(circuit, param_resolver)
-
-    return self._sample_measure_results(solved_circuit, repetitions)
-
-  def _sample_measure_results(
-    self,
-    program: circuits.Circuit,
-    repetitions: int = 1,
-  ) -> Dict[str, np.ndarray]:
-    """Samples from measurement gates in the circuit.
-
-    Note that this will execute the circuit 'repetitions' times.
-
-    Args:
-        program: The circuit to sample from.
-        repetitions: The number of samples to take.
-
-    Returns:
-        A dictionary from measurement gate key to measurement
-        results. Measurement results are stored in a 2-dimensional
-        numpy array, the first dimension corresponding to the repetition
-        and the second to the actual boolean measurement results (ordered
-        by the qubits being measured.)
-
-    Raises:
-        ValueError: If there are multiple MeasurementGates with the same key,
-            or if repetitions is negative.
-    """
-    if not isinstance(program, qsimc.QSimCircuit):
-      program = qsimc.QSimCircuit(program, device=program.device)
-
-    # Compute indices of measured qubits
-    ordered_qubits = ops.QubitOrder.DEFAULT.order_for(program.all_qubits())
-    num_qubits = len(ordered_qubits)
-
-    qubit_map = {
-      qubit: index for index, qubit in enumerate(ordered_qubits)
-    }
-
-    # Computes
-    # - the list of qubits to be measured
-    # - the start (inclusive) and end (exclusive) indices of each measurement
-    # - a mapping from measurement key to measurement gate
-    measurement_ops = [
-      op for _, op, _ in program.findall_operations_with_gate_type(ops.MeasurementGate)
-    ]
-    measured_qubits = []  # type: List[ops.Qid]
-    bounds = {}  # type: Dict[str, Tuple]
-    meas_ops = {}  # type: Dict[str, cirq.GateOperation]
-    current_index = 0
-    for op in measurement_ops:
-      gate = op.gate
-      key = protocols.measurement_key(gate)
-      meas_ops[key] = op
-      if key in bounds:
-        raise ValueError("Duplicate MeasurementGate with key {}".format(key))
-      bounds[key] = (current_index, current_index + len(op.qubits))
-      measured_qubits.extend(op.qubits)
-      current_index += len(op.qubits)
-
-    # Set qsim options
-    options = {}
-    options.update(self.qsim_options)
-
-    results = {}
-    for key, bound in bounds.items():
-      results[key] = np.ndarray(shape=(repetitions, bound[1]-bound[0]),
-                                dtype=int)
-
-
-    noisy = _needs_trajectories(program)
-    if noisy:
-      translator_fn_name = 'translate_cirq_to_qtrajectory'
-      sampler_fn = qsim.qtrajectory_sample
-    else:
-      translator_fn_name = 'translate_cirq_to_qsim'
-      sampler_fn = qsim.qsim_sample
-
-    if not noisy and program.are_all_measurements_terminal() and repetitions > 1:
-      print('Provided circuit has no intermediate measurements. ' +
-            'Sampling repeatedly from final state vector.')
-      # Measurements must be replaced with identity gates to sample properly.
-      # Simply removing them may omit qubits from the circuit.
-      for i in range(len(program.moments)):
-        program.moments[i] = ops.Moment(
-          op if not isinstance(op.gate, ops.MeasurementGate)
-          else [ops.IdentityGate(1).on(q) for q in op.qubits]
-          for op in program.moments[i]
-        )
-      options['c'] = program.translate_cirq_to_qsim(ops.QubitOrder.DEFAULT)
-      options['s'] = self.get_seed()
-      final_state = qsim.qsim_simulate_fullstate(options, 0)
-      full_results = sim.sample_state_vector(
-        final_state.view(np.complex64), range(num_qubits),
-        repetitions=repetitions, seed=self._prng)
-
-      for i in range(repetitions):
-        for key, op in meas_ops.items():
-          meas_indices = [qubit_map[qubit] for qubit in op.qubits]
-          for j, q in enumerate(meas_indices):
-            results[key][i][j] = full_results[i][q]
-    else:
-      translator_fn = getattr(program, translator_fn_name)
-      options['c'] = translator_fn(ops.QubitOrder.DEFAULT)
-      for i in range(repetitions):
-        options['s'] = self.get_seed()
-        measurements = sampler_fn(options)
+        repetitions: int,
+    ) -> Dict[str, np.ndarray]:
+        """Run a simulation, mimicking quantum hardware.
+
+        Args:
+            program: The circuit to simulate.
+            param_resolver: Parameters to run with the program.
+            repetitions: Number of times to repeat the run.
+
+        Returns:
+            A dictionary from measurement gate key to measurement
+            results.
+        """
+        param_resolver = param_resolver or study.ParamResolver({})
+        solved_circuit = protocols.resolve_parameters(circuit, param_resolver)
+
+        return self._sample_measure_results(solved_circuit, repetitions)
+
+    def _sample_measure_results(
+        self,
+        program: circuits.Circuit,
+        repetitions: int = 1,
+    ) -> Dict[str, np.ndarray]:
+        """Samples from measurement gates in the circuit.
+
+        Note that this will execute the circuit 'repetitions' times.
+
+        Args:
+            program: The circuit to sample from.
+            repetitions: The number of samples to take.
+
+        Returns:
+            A dictionary from measurement gate key to measurement
+            results. Measurement results are stored in a 2-dimensional
+            numpy array, the first dimension corresponding to the repetition
+            and the second to the actual boolean measurement results (ordered
+            by the qubits being measured.)
+
+        Raises:
+            ValueError: If there are multiple MeasurementGates with the same key,
+                or if repetitions is negative.
+        """
+        if not isinstance(program, qsimc.QSimCircuit):
+            program = qsimc.QSimCircuit(program, device=program.device)
+
+        # Compute indices of measured qubits
+        ordered_qubits = ops.QubitOrder.DEFAULT.order_for(program.all_qubits())
+        num_qubits = len(ordered_qubits)
+
+        qubit_map = {qubit: index for index, qubit in enumerate(ordered_qubits)}
+
+        # Computes
+        # - the list of qubits to be measured
+        # - the start (inclusive) and end (exclusive) indices of each measurement
+        # - a mapping from measurement key to measurement gate
+        measurement_ops = [
+            op
+            for _, op, _ in program.findall_operations_with_gate_type(
+                ops.MeasurementGate
+            )
+        ]
+        measured_qubits = []  # type: List[ops.Qid]
+        bounds = {}  # type: Dict[str, Tuple]
+        meas_ops = {}  # type: Dict[str, cirq.GateOperation]
+        current_index = 0
+        for op in measurement_ops:
+            gate = op.gate
+            key = protocols.measurement_key(gate)
+            meas_ops[key] = op
+            if key in bounds:
+                raise ValueError(f"Duplicate MeasurementGate with key {key}")
+            bounds[key] = (current_index, current_index + len(op.qubits))
+            measured_qubits.extend(op.qubits)
+            current_index += len(op.qubits)
+
+        # Set qsim options
+        options = {}
+        options.update(self.qsim_options)
+
+        results = {}
         for key, bound in bounds.items():
-          for j in range(bound[1]-bound[0]):
-            results[key][i][j] = int(measurements[bound[0]+j])
+            results[key] = np.ndarray(
+                shape=(repetitions, bound[1] - bound[0]), dtype=int
+            )
+
+        noisy = _needs_trajectories(program)
+        if noisy:
+            translator_fn_name = "translate_cirq_to_qtrajectory"
+            sampler_fn = qsim.qtrajectory_sample
+        else:
+            translator_fn_name = "translate_cirq_to_qsim"
+            sampler_fn = qsim.qsim_sample
+
+        if not noisy and program.are_all_measurements_terminal() and repetitions > 1:
+            print(
+                "Provided circuit has no intermediate measurements. "
+                + "Sampling repeatedly from final state vector."
+            )
+            # Measurements must be replaced with identity gates to sample properly.
+            # Simply removing them may omit qubits from the circuit.
+            for i in range(len(program.moments)):
+                program.moments[i] = ops.Moment(
+                    op
+                    if not isinstance(op.gate, ops.MeasurementGate)
+                    else [ops.IdentityGate(1).on(q) for q in op.qubits]
+                    for op in program.moments[i]
+                )
+            options["c"] = program.translate_cirq_to_qsim(ops.QubitOrder.DEFAULT)
+            options["s"] = self.get_seed()
+            final_state = qsim.qsim_simulate_fullstate(options, 0)
+            full_results = sim.sample_state_vector(
+                final_state.view(np.complex64),
+                range(num_qubits),
+                repetitions=repetitions,
+                seed=self._prng,
+            )
+
+            for i in range(repetitions):
+                for key, op in meas_ops.items():
+                    meas_indices = [qubit_map[qubit] for qubit in op.qubits]
+                    for j, q in enumerate(meas_indices):
+                        results[key][i][j] = full_results[i][q]
+        else:
+            translator_fn = getattr(program, translator_fn_name)
+            options["c"] = translator_fn(ops.QubitOrder.DEFAULT)
+            for i in range(repetitions):
+                options["s"] = self.get_seed()
+                measurements = sampler_fn(options)
+                for key, bound in bounds.items():
+                    for j in range(bound[1] - bound[0]):
+                        results[key][i][j] = int(measurements[bound[0] + j])
 
-    return results
+        return results
 
+    def compute_amplitudes_sweep(
+        self,
+        program: circuits.Circuit,
+        bitstrings: Sequence[int],
+        params: study.Sweepable,
+        qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
+    ) -> Sequence[Sequence[complex]]:
+        """Computes the desired amplitudes using qsim.
+
+        The initial state is assumed to be the all zeros state.
+
+        Args:
+            program: The circuit to simulate.
+            bitstrings: The bitstrings whose amplitudes are desired, input as an
+              string array where each string is formed from measured qubit values
+              according to `qubit_order` from most to least significant qubit,
+              i.e. in big-endian ordering.
+            param_resolver: Parameters to run with the program.
+            qubit_order: Determines the canonical ordering of the qubits. This is
+              often used in specifying the initial state, i.e. the ordering of the
+              computational basis states.
+
+        Returns:
+            List of amplitudes.
+        """
+        if not isinstance(program, qsimc.QSimCircuit):
+            program = qsimc.QSimCircuit(program, device=program.device)
+
+        # qsim numbers qubits in reverse order from cirq
+        cirq_order = ops.QubitOrder.as_qubit_order(qubit_order).order_for(
+            program.all_qubits()
+        )
+        num_qubits = len(cirq_order)
+        bitstrings = [
+            format(bitstring, "b").zfill(num_qubits)[::-1] for bitstring in bitstrings
+        ]
+
+        options = {"i": "\n".join(bitstrings)}
+        options.update(self.qsim_options)
+
+        param_resolvers = study.to_resolvers(params)
+
+        trials_results = []
+        if _needs_trajectories(program):
+            translator_fn_name = "translate_cirq_to_qtrajectory"
+            simulator_fn = qsim.qtrajectory_simulate
+        else:
+            translator_fn_name = "translate_cirq_to_qsim"
+            simulator_fn = qsim.qsim_simulate
+
+        for prs in param_resolvers:
+            solved_circuit = protocols.resolve_parameters(program, prs)
+            translator_fn = getattr(solved_circuit, translator_fn_name)
+            options["c"] = translator_fn(cirq_order)
+            options["s"] = self.get_seed()
+            amplitudes = simulator_fn(options)
+            trials_results.append(amplitudes)
+
+        return trials_results
+
+    def simulate_sweep(
+        self,
+        program: circuits.Circuit,
+        params: study.Sweepable,
+        qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
+        initial_state: Optional[Union[int, np.ndarray]] = None,
+    ) -> List["SimulationTrialResult"]:
+        """Simulates the supplied Circuit.
+
+        This method returns a result which allows access to the entire
+        wave function. In contrast to simulate, this allows for sweeping
+        over different parameter values.
+
+        Args:
+            program: The circuit to simulate.
+            params: Parameters to run with the program.
+            qubit_order: Determines the canonical ordering of the qubits. This is
+              often used in specifying the initial state, i.e. the ordering of the
+              computational basis states.
+            initial_state: The initial state for the simulation. This can either
+              be an integer representing a pure state (e.g. 11010) or a numpy
+              array containing the full state vector. If none is provided, this
+              is assumed to be the all-zeros state.
+
+        Returns:
+            List of SimulationTrialResults for this run, one for each
+            possible parameter resolver.
+
+        Raises:
+            TypeError: if an invalid initial_state is provided.
+        """
+        if initial_state is None:
+            initial_state = 0
+        if not isinstance(initial_state, (int, np.ndarray)):
+            raise TypeError("initial_state must be an int or state vector.")
+        if not isinstance(program, qsimc.QSimCircuit):
+            program = qsimc.QSimCircuit(program, device=program.device)
+
+        options = {}
+        options.update(self.qsim_options)
+
+        param_resolvers = study.to_resolvers(params)
+        # qsim numbers qubits in reverse order from cirq
+        cirq_order = ops.QubitOrder.as_qubit_order(qubit_order).order_for(
+            program.all_qubits()
+        )
+        qsim_order = list(reversed(cirq_order))
+        num_qubits = len(qsim_order)
+        if isinstance(initial_state, np.ndarray):
+            if initial_state.dtype != np.complex64:
+                raise TypeError(f"initial_state vector must have dtype np.complex64.")
+            input_vector = initial_state.view(np.float32)
+            if len(input_vector) != 2 ** num_qubits * 2:
+                raise ValueError(
+                    f"initial_state vector size must match number of qubits."
+                    f"Expected: {2**num_qubits * 2} Received: {len(input_vector)}"
+                )
+
+        trials_results = []
+        if _needs_trajectories(program):
+            translator_fn_name = "translate_cirq_to_qtrajectory"
+            fullstate_simulator_fn = qsim.qtrajectory_simulate_fullstate
+        else:
+            translator_fn_name = "translate_cirq_to_qsim"
+            fullstate_simulator_fn = qsim.qsim_simulate_fullstate
+
+        for prs in param_resolvers:
+            solved_circuit = protocols.resolve_parameters(program, prs)
+            translator_fn = getattr(solved_circuit, translator_fn_name)
+            options["c"] = translator_fn(cirq_order)
+            options["s"] = self.get_seed()
+            qubit_map = {qubit: index for index, qubit in enumerate(qsim_order)}
+
+            if isinstance(initial_state, int):
+                qsim_state = fullstate_simulator_fn(options, initial_state)
+            elif isinstance(initial_state, np.ndarray):
+                qsim_state = fullstate_simulator_fn(options, input_vector)
+            assert qsim_state.dtype == np.float32
+            assert qsim_state.ndim == 1
+            final_state = QSimSimulatorState(qsim_state, qubit_map)
+            # create result for this parameter
+            # TODO: We need to support measurements.
+            result = QSimSimulatorTrialResult(
+                params=prs, measurements={}, final_simulator_state=final_state
+            )
+            trials_results.append(result)
+
+        return trials_results
 
-  def compute_amplitudes_sweep(
-      self,
-      program: circuits.Circuit,
-      bitstrings: Sequence[int],
-      params: study.Sweepable,
-      qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
-  ) -> Sequence[Sequence[complex]]:
-    """Computes the desired amplitudes using qsim.
-
-      The initial state is assumed to be the all zeros state.
-
-      Args:
-          program: The circuit to simulate.
-          bitstrings: The bitstrings whose amplitudes are desired, input as an
-            string array where each string is formed from measured qubit values
-            according to `qubit_order` from most to least significant qubit,
-            i.e. in big-endian ordering.
-          param_resolver: Parameters to run with the program.
-          qubit_order: Determines the canonical ordering of the qubits. This is
-            often used in specifying the initial state, i.e. the ordering of the
-            computational basis states.
-
-      Returns:
-          List of amplitudes.
-      """
-    if not isinstance(program, qsimc.QSimCircuit):
-      program = qsimc.QSimCircuit(program, device=program.device)
-
-    num_qubits = len(program.all_qubits())
-    # qsim numbers qubits in reverse order from cirq
-    cirq_order = ops.QubitOrder.as_qubit_order(qubit_order).order_for(
-      program.all_qubits())
-    bitstrings = [format(bitstring, 'b').zfill(num_qubits)[::-1]
-                  for bitstring in bitstrings]
-
-    options = {'i': '\n'.join(bitstrings)}
-    options.update(self.qsim_options)
-
-    param_resolvers = study.to_resolvers(params)
-
-    trials_results = []
-    if _needs_trajectories(program):
-      translator_fn_name = 'translate_cirq_to_qtrajectory'
-      simulator_fn = qsim.qtrajectory_simulate
-    else:
-      translator_fn_name = 'translate_cirq_to_qsim'
-      simulator_fn = qsim.qsim_simulate
-
-    for prs in param_resolvers:
-      solved_circuit = protocols.resolve_parameters(program, prs)
-      translator_fn = getattr(solved_circuit, translator_fn_name)
-      options['c'] = translator_fn(cirq_order)
-      options['s'] = self.get_seed()
-      amplitudes = simulator_fn(options)
-      trials_results.append(amplitudes)
-
-    return trials_results
-
-  def simulate_sweep(
-      self,
-      program: circuits.Circuit,
-      params: study.Sweepable,
-      qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
-      initial_state: Optional[Union[int, np.ndarray]] = None,
-  ) -> List['SimulationTrialResult']:
-    """Simulates the supplied Circuit.
-
-      This method returns a result which allows access to the entire
-      wave function. In contrast to simulate, this allows for sweeping
-      over different parameter values.
-
-      Args:
-          program: The circuit to simulate.
-          params: Parameters to run with the program.
-          qubit_order: Determines the canonical ordering of the qubits. This is
-            often used in specifying the initial state, i.e. the ordering of the
-            computational basis states.
-          initial_state: The initial state for the simulation. This can either
-            be an integer representing a pure state (e.g. 11010) or a numpy
-            array containing the full state vector. If none is provided, this
-            is assumed to be the all-zeros state.
-
-      Returns:
-          List of SimulationTrialResults for this run, one for each
-          possible parameter resolver.
-
-      Raises:
-          TypeError: if an invalid initial_state is provided.
-      """
-    if initial_state is None:
-      initial_state = 0
-    if not isinstance(initial_state, (int, np.ndarray)):
-      raise TypeError('initial_state must be an int or state vector.')
-    if not isinstance(program, qsimc.QSimCircuit):
-      program = qsimc.QSimCircuit(program, device=program.device)
-
-    options = {}
-    options.update(self.qsim_options)
-
-    param_resolvers = study.to_resolvers(params)
-    qubits = program.all_qubits()
-    num_qubits = len(qubits)
-    # qsim numbers qubits in reverse order from cirq
-    cirq_order = ops.QubitOrder.as_qubit_order(qubit_order).order_for(
-      qubits)
-    qsim_order = list(reversed(cirq_order))
-    if isinstance(initial_state, np.ndarray):
-      if initial_state.dtype != np.complex64:
-        raise TypeError(f'initial_state vector must have dtype np.complex64.')
-      input_vector = initial_state.view(np.float32)
-      if len(input_vector) != 2**num_qubits * 2:
-        raise ValueError(f'initial_state vector size must match number of qubits.'
-          f'Expected: {2**num_qubits * 2} Received: {len(input_vector)}')
-
-    trials_results = []
-    if _needs_trajectories(program):
-      translator_fn_name = 'translate_cirq_to_qtrajectory'
-      fullstate_simulator_fn = qsim.qtrajectory_simulate_fullstate
-    else:
-      translator_fn_name = 'translate_cirq_to_qsim'
-      fullstate_simulator_fn = qsim.qsim_simulate_fullstate
-
-    for prs in param_resolvers:
-      solved_circuit = protocols.resolve_parameters(program, prs)
-      translator_fn = getattr(solved_circuit, translator_fn_name)
-      options['c'] = translator_fn(cirq_order)
-      options['s'] = self.get_seed()
-      qubit_map = {
-        qubit: index for index, qubit in enumerate(qsim_order)
-      }
-
-      if isinstance(initial_state, int):
-        qsim_state = fullstate_simulator_fn(options, initial_state)
-      elif isinstance(initial_state, np.ndarray):
-        qsim_state = fullstate_simulator_fn(options, input_vector)
-      assert qsim_state.dtype == np.float32
-      assert qsim_state.ndim == 1
-      final_state = QSimSimulatorState(qsim_state, qubit_map)
-      # create result for this parameter
-      # TODO: We need to support measurements.
-      result = QSimSimulatorTrialResult(params=prs,
-                                        measurements={},
-                                        final_simulator_state=final_state)
-      trials_results.append(result)
-
-    return trials_results
-
-  def simulate_expectation_values_sweep(
-    self,
-    program: 'cirq.Circuit',
-    observables: Union['cirq.PauliSumLike', List['cirq.PauliSumLike']],
-    params: 'study.Sweepable',
-    qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
-    initial_state: Any = None,
-    permit_terminal_measurements: bool = False,
-  ) -> List[List[float]]:
-    """Simulates the supplied circuit and calculates exact expectation
-    values for the given observables on its final state.
-
-    This method has no perfect analogy in hardware. Instead compare with
-    Sampler.sample_expectation_values, which calculates estimated
-    expectation values by sampling multiple times.
-
-    Args:
-        program: The circuit to simulate.
-        observables: An observable or list of observables.
-        param_resolver: Parameters to run with the program.
-        qubit_order: Determines the canonical ordering of the qubits. This
-            is often used in specifying the initial state, i.e. the
-            ordering of the computational basis states.
-        initial_state: The initial state for the simulation. The form of
-            this state depends on the simulation implementation. See
-            documentation of the implementing class for details.
-        permit_terminal_measurements: If the provided circuit ends with
-            measurement(s), this method will generate an error unless this
-            is set to True. This is meant to prevent measurements from
-            ruining expectation value calculations.
-
-    Returns:
-        A list of expectation values, with the value at index `n`
-        corresponding to `observables[n]` from the input.
-
-    Raises:
-        ValueError if 'program' has terminal measurement(s) and
-        'permit_terminal_measurements' is False. (Note: We cannot test this
-        until Cirq's `are_any_measurements_terminal` is released.)
-    """
-    # TODO: replace with commented check when Cirq v0.10 is released.
-    if not permit_terminal_measurements:
-      raise ValueError(
-        'Automatic terminal measurement checking is not supported in qsim. '
-        'Please check that your circuit has no terminal measurements, then '
-        'set permit_terminal_measurements=True to bypass this error.'
-      )
-    # if not permit_terminal_measurements and program.are_any_measurements_terminal():
-    #   raise ValueError(
-    #     'Provided circuit has terminal measurements, which may '
-    #     'skew expectation values. If this is intentional, set '
-    #     'permit_terminal_measurements=True.'
-    #   )
-    if not isinstance(observables, List):
-      observables = [observables]
-    psumlist = [ops.PauliSum.wrap(pslike) for pslike in observables]
-
-    cirq_order = ops.QubitOrder.as_qubit_order(qubit_order).order_for(
-      program.all_qubits())
-    qsim_order = list(reversed(cirq_order))
-    num_qubits = len(qsim_order)
-    qubit_map = {qubit: index for index, qubit in enumerate(qsim_order)}
-
-    opsums_and_qubit_counts = []
-    for psum in psumlist:
-      opsum = []
-      opsum_qubits = set()
-      for pstr in psum:
-        opstring = qsim.OpString()
-        opstring.weight = pstr.coefficient
-        for q, pauli in pstr.items():
-          op = pauli.on(q)
-          opsum_qubits.add(q)
-          qsimc.add_op_to_opstring(op, qubit_map, opstring)
-        opsum.append(opstring)
-      opsums_and_qubit_counts.append((opsum, len(opsum_qubits)))
-
-    if initial_state is None:
-      initial_state = 0
-    if not isinstance(initial_state, (int, np.ndarray)):
-      raise TypeError('initial_state must be an int or state vector.')
-    if not isinstance(program, qsimc.QSimCircuit):
-      program = qsimc.QSimCircuit(program, device=program.device)
-
-    options = {}
-    options.update(self.qsim_options)
-
-    param_resolvers = study.to_resolvers(params)
-    if isinstance(initial_state, np.ndarray):
-      if initial_state.dtype != np.complex64:
-        raise TypeError(f'initial_state vector must have dtype np.complex64.')
-      input_vector = initial_state.view(np.float32)
-      if len(input_vector) != 2**num_qubits * 2:
-        raise ValueError(f'initial_state vector size must match number of qubits.'
-          f'Expected: {2**num_qubits * 2} Received: {len(input_vector)}')
-
-    results = []
-    if _needs_trajectories(program):
-      translator_fn_name = 'translate_cirq_to_qtrajectory'
-      ev_simulator_fn = qsim.qtrajectory_simulate_expectation_values
-    else:
-      translator_fn_name = 'translate_cirq_to_qsim'
-      ev_simulator_fn = qsim.qsim_simulate_expectation_values
-
-    for prs in param_resolvers:
-      solved_circuit = protocols.resolve_parameters(program, prs)
-      translator_fn = getattr(solved_circuit, translator_fn_name)
-      options['c'] = translator_fn(cirq_order)
-      options['s'] = self.get_seed()
-
-      if isinstance(initial_state, int):
-        evs = ev_simulator_fn(options, opsums_and_qubit_counts, initial_state)
-      elif isinstance(initial_state, np.ndarray):
-        evs = ev_simulator_fn(options, opsums_and_qubit_counts, input_vector)
-      results.append(evs)
+    def simulate_expectation_values_sweep(
+        self,
+        program: "cirq.Circuit",
+        observables: Union["cirq.PauliSumLike", List["cirq.PauliSumLike"]],
+        params: "study.Sweepable",
+        qubit_order: ops.QubitOrderOrList = ops.QubitOrder.DEFAULT,
+        initial_state: Any = None,
+        permit_terminal_measurements: bool = False,
+    ) -> List[List[float]]:
+        """Simulates the supplied circuit and calculates exact expectation
+        values for the given observables on its final state.
+
+        This method has no perfect analogy in hardware. Instead compare with
+        Sampler.sample_expectation_values, which calculates estimated
+        expectation values by sampling multiple times.
+
+        Args:
+            program: The circuit to simulate.
+            observables: An observable or list of observables.
+            param_resolver: Parameters to run with the program.
+            qubit_order: Determines the canonical ordering of the qubits. This
+                is often used in specifying the initial state, i.e. the
+                ordering of the computational basis states.
+            initial_state: The initial state for the simulation. The form of
+                this state depends on the simulation implementation. See
+                documentation of the implementing class for details.
+            permit_terminal_measurements: If the provided circuit ends with
+                measurement(s), this method will generate an error unless this
+                is set to True. This is meant to prevent measurements from
+                ruining expectation value calculations.
+
+        Returns:
+            A list of expectation values, with the value at index `n`
+            corresponding to `observables[n]` from the input.
+
+        Raises:
+            ValueError if 'program' has terminal measurement(s) and
+            'permit_terminal_measurements' is False. (Note: We cannot test this
+            until Cirq's `are_any_measurements_terminal` is released.)
+        """
+        if not permit_terminal_measurements and program.are_any_measurements_terminal():
+            raise ValueError(
+                "Provided circuit has terminal measurements, which may "
+                "skew expectation values. If this is intentional, set "
+                "permit_terminal_measurements=True."
+            )
+        if not isinstance(observables, List):
+            observables = [observables]
+        psumlist = [ops.PauliSum.wrap(pslike) for pslike in observables]
+
+        cirq_order = ops.QubitOrder.as_qubit_order(qubit_order).order_for(
+            program.all_qubits()
+        )
+        qsim_order = list(reversed(cirq_order))
+        num_qubits = len(qsim_order)
+        qubit_map = {qubit: index for index, qubit in enumerate(qsim_order)}
+
+        opsums_and_qubit_counts = []
+        for psum in psumlist:
+            opsum = []
+            opsum_qubits = set()
+            for pstr in psum:
+                opstring = qsim.OpString()
+                opstring.weight = pstr.coefficient
+                for q, pauli in pstr.items():
+                    op = pauli.on(q)
+                    opsum_qubits.add(q)
+                    qsimc.add_op_to_opstring(op, qubit_map, opstring)
+                opsum.append(opstring)
+            opsums_and_qubit_counts.append((opsum, len(opsum_qubits)))
+
+        if initial_state is None:
+            initial_state = 0
+        if not isinstance(initial_state, (int, np.ndarray)):
+            raise TypeError("initial_state must be an int or state vector.")
+        if not isinstance(program, qsimc.QSimCircuit):
+            program = qsimc.QSimCircuit(program, device=program.device)
+
+        options = {}
+        options.update(self.qsim_options)
+
+        param_resolvers = study.to_resolvers(params)
+        if isinstance(initial_state, np.ndarray):
+            if initial_state.dtype != np.complex64:
+                raise TypeError(f"initial_state vector must have dtype np.complex64.")
+            input_vector = initial_state.view(np.float32)
+            if len(input_vector) != 2 ** num_qubits * 2:
+                raise ValueError(
+                    f"initial_state vector size must match number of qubits."
+                    f"Expected: {2**num_qubits * 2} Received: {len(input_vector)}"
+                )
+
+        results = []
+        if _needs_trajectories(program):
+            translator_fn_name = "translate_cirq_to_qtrajectory"
+            ev_simulator_fn = qsim.qtrajectory_simulate_expectation_values
+        else:
+            translator_fn_name = "translate_cirq_to_qsim"
+            ev_simulator_fn = qsim.qsim_simulate_expectation_values
+
+        for prs in param_resolvers:
+            solved_circuit = protocols.resolve_parameters(program, prs)
+            translator_fn = getattr(solved_circuit, translator_fn_name)
+            options["c"] = translator_fn(cirq_order)
+            options["s"] = self.get_seed()
+
+            if isinstance(initial_state, int):
+                evs = ev_simulator_fn(options, opsums_and_qubit_counts, initial_state)
+            elif isinstance(initial_state, np.ndarray):
+                evs = ev_simulator_fn(options, opsums_and_qubit_counts, input_vector)
+            results.append(evs)
 
-    return results
+        return results
```

### Comparing `qsimcirq-0.9.2/PKG-INFO` & `qsimcirq-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsimcirq
-Version: 0.9.2
+Version: 0.9.5
 Summary: Schrödinger and Schrödinger-Feynman simulators for quantum circuits.
 Home-page: UNKNOWN
 Author: Vamsi Krishna Devabathini
 Author-email: devabathini92@gmail.com
 License: Apache 2
 Description: # qsim and qsimh
```

