# Comparing `tmp/pkilint-0.8.0.tar.gz` & `tmp/pkilint-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkilint-0.8.0.tar", last modified: Tue May  2 20:13:40 2023, max compression
+gzip compressed data, was "pkilint-0.8.1.tar", last modified: Wed May  3 13:12:28 2023, max compression
```

## Comparing `pkilint-0.8.0.tar` & `pkilint-0.8.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.937238 pkilint-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-02 20:13:33.000000 pkilint-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-02 20:13:40.937238 pkilint-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-05-02 20:13:33.000000 pkilint-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 20:13:33.000000 pkilint-0.8.0/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.925237 pkilint-0.8.0/pkilint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.925237 pkilint-0.8.0/pkilint/adobe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/adobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/adobe/adobe_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.925237 pkilint-0.8.0/pkilint/adobe/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/adobe/asn1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/convert_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/lint_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/lint_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/lint_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/lint_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/lint_pkix_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/cabf/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/cabf_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/cabf_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/cabf_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/cabf_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/cabf_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/cabf/servercert/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/cabf/servercert/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/asn1/ev_guidelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/servercert_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/servercert_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/servercert_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/servercert/servercert_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/cabf/smime/
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/smime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/smime/smime_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/smime/smime_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/smime/smime_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/cabf/smime/smime_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/etsi/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/etsi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/etsi/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/etsi/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/etsi/asn1/en_319_412_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/etsi/asn1/ts_119_495.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.929237 pkilint-0.8.0/pkilint/iso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/iso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/iso/lei.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/itu/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/itu/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/itu/x520_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/msft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/msft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/msft/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/msft/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/msft/msft_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/pkix/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/pkix/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/certificate/certificate_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/certificate/certificate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/certificate/certificate_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/certificate/certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/certificate/certificate_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/pkix/crl/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/crl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/crl/crl_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/crl/crl_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/crl/crl_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.933237 pkilint-0.8.0/pkilint/pkix/ocsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/ocsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/ocsp/ocsp_basic_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/ocsp/ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/ocsp/ocsp_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/pkix/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-02 20:13:33.000000 pkilint-0.8.0/pkilint/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.925237 pkilint-0.8.0/pkilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:13:40.000000 pkilint-0.8.0/pkilint.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-02 20:13:40.937238 pkilint-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 20:13:33.000000 pkilint-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.937238 pkilint-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.937238 pkilint-0.8.0/tests/integration_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/integration_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/integration_certificate/test_cabf_smime_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:40.937238 pkilint-0.8.0/tests/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/itu/test_bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/itu/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-02 20:13:33.000000 pkilint-0.8.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 13:12:10.000000 pkilint-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-03 13:12:28.503013 pkilint-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-03 13:12:10.000000 pkilint-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 13:12:10.000000 pkilint-0.8.1/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/adobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/adobe/adobe_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint/adobe/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/adobe/asn1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/convert_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_pkix_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/servercert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/servercert/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/asn1/ev_guidelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/smime/
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/etsi/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/etsi/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/asn1/en_319_412_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/asn1/ts_119_495.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/iso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/iso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/iso/lei.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/x520_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/msft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/msft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/msft/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/msft/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/msft/msft_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/pkix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/pkilint/pkix/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/pkilint/pkix/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/crl_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/crl_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/crl_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/pkilint/pkix/ocsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_basic_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-03 13:12:28.503013 pkilint-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 13:12:10.000000 pkilint-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/tests/integration_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/integration_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/integration_certificate/test_cabf_smime_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/tests/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/itu/test_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/itu/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/util.py
```

### Comparing `pkilint-0.8.0/LICENSE` & `pkilint-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/PKG-INFO` & `pkilint-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.0
+Version: 0.8.1
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pkilint
 
 
-[![PyPI](https://img.shields.io/pypi/v/pkilint.svg?maxAge=2592000)](https://pypi.org/project/pkilint)
-[![Python Versions](https://img.shields.io/pypi/pyversions/pkilint.svg)](https://pypi.org/project/pkilint/)
+[![PyPI](https://img.shields.io/pypi/v/pkilint)](https://pypi.org/project/pkilint)
+[![Python Versions](https://img.shields.io/pypi/pyversions/pkilint)](https://pypi.org/project/pkilint/)
 [![Build status](https://github.com/digicert/pkilint/actions/workflows/build_and_publish.yml/badge.svg)](https://github.com/digicert/pkilint/actions/workflows/build_and_publish.yml)
 [![GitHub license](https://img.shields.io/pypi/l/pkilint)](https://raw.githubusercontent.com/digicert/pkilint/main/LICENSE)
 
 pkilint is a linting framework for documents that are encoded using ASN.1. pkilint is designed to
 be a highly extensible toolbox to quickly create linters for a variety of ASN.1 structure/"document" types to check for compliance with
 various standards and policies.
```

### Comparing `pkilint-0.8.0/README.md` & `pkilint-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pkilint
 
 
-[![PyPI](https://img.shields.io/pypi/v/pkilint.svg?maxAge=2592000)](https://pypi.org/project/pkilint)
-[![Python Versions](https://img.shields.io/pypi/pyversions/pkilint.svg)](https://pypi.org/project/pkilint/)
+[![PyPI](https://img.shields.io/pypi/v/pkilint)](https://pypi.org/project/pkilint)
+[![Python Versions](https://img.shields.io/pypi/pyversions/pkilint)](https://pypi.org/project/pkilint/)
 [![Build status](https://github.com/digicert/pkilint/actions/workflows/build_and_publish.yml/badge.svg)](https://github.com/digicert/pkilint/actions/workflows/build_and_publish.yml)
 [![GitHub license](https://img.shields.io/pypi/l/pkilint)](https://raw.githubusercontent.com/digicert/pkilint/main/LICENSE)
 
 pkilint is a linting framework for documents that are encoded using ASN.1. pkilint is designed to
 be a highly extensible toolbox to quickly create linters for a variety of ASN.1 structure/"document" types to check for compliance with
 various standards and policies.
```

### Comparing `pkilint-0.8.0/pkilint/adobe/adobe_validator.py` & `pkilint-0.8.1/pkilint/adobe/adobe_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/adobe/asn1/__init__.py` & `pkilint-0.8.1/pkilint/adobe/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/convert_cert.py` & `pkilint-0.8.1/pkilint/bin/convert_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/lint_cabf_serverauth_cert.py` & `pkilint-0.8.1/pkilint/bin/lint_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/lint_cabf_smime_cert.py` & `pkilint-0.8.1/pkilint/bin/lint_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/lint_crl.py` & `pkilint-0.8.1/pkilint/bin/lint_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/lint_ocsp_response.py` & `pkilint-0.8.1/pkilint/bin/lint_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/lint_pkix_cert.py` & `pkilint-0.8.1/pkilint/bin/lint_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/bin/lint_pkix_signer_signee_cert_chain.py` & `pkilint-0.8.1/pkilint/bin/lint_pkix_signer_signee_cert_chain.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/__init__.py` & `pkilint-0.8.1/pkilint/cabf/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/cabf_constants.py` & `pkilint-0.8.1/pkilint/cabf/cabf_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/cabf_crl.py` & `pkilint-0.8.1/pkilint/cabf/cabf_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/cabf_extension.py` & `pkilint-0.8.1/pkilint/cabf/cabf_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/cabf_key.py` & `pkilint-0.8.1/pkilint/cabf/cabf_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/cabf_name.py` & `pkilint-0.8.1/pkilint/cabf/cabf_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/servercert/__init__.py` & `pkilint-0.8.1/pkilint/cabf/servercert/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/servercert/asn1/ev_guidelines.py` & `pkilint-0.8.1/pkilint/cabf/servercert/asn1/ev_guidelines.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/servercert/servercert_extension.py` & `pkilint-0.8.1/pkilint/cabf/servercert/servercert_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/servercert/servercert_key.py` & `pkilint-0.8.1/pkilint/cabf/servercert/servercert_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/servercert/servercert_name.py` & `pkilint-0.8.1/pkilint/cabf/servercert/servercert_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/smime/__init__.py` & `pkilint-0.8.1/pkilint/cabf/smime/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/smime/smime_constants.py` & `pkilint-0.8.1/pkilint/cabf/smime/smime_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/smime/smime_extension.py` & `pkilint-0.8.1/pkilint/cabf/smime/smime_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/smime/smime_key.py` & `pkilint-0.8.1/pkilint/cabf/smime/smime_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/cabf/smime/smime_name.py` & `pkilint-0.8.1/pkilint/cabf/smime/smime_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/document.py` & `pkilint-0.8.1/pkilint/document.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/etsi/__init__.py` & `pkilint-0.8.1/pkilint/etsi/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/etsi/asn1/en_319_412_5.py` & `pkilint-0.8.1/pkilint/etsi/asn1/en_319_412_5.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/etsi/asn1/ts_119_495.py` & `pkilint-0.8.1/pkilint/etsi/asn1/ts_119_495.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/iso/lei.py` & `pkilint-0.8.1/pkilint/iso/lei.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/itu/bitstring.py` & `pkilint-0.8.1/pkilint/itu/bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/itu/string.py` & `pkilint-0.8.1/pkilint/itu/string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/itu/x520_name.py` & `pkilint-0.8.1/pkilint/itu/x520_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/loader.py` & `pkilint-0.8.1/pkilint/loader.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/msft/msft_name.py` & `pkilint-0.8.1/pkilint/msft/msft_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/__init__.py` & `pkilint-0.8.1/pkilint/pkix/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/algorithm.py` & `pkilint-0.8.1/pkilint/pkix/algorithm.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/certificate/__init__.py` & `pkilint-0.8.1/pkilint/pkix/certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/certificate/certificate_extension.py` & `pkilint-0.8.1/pkilint/pkix/certificate/certificate_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/certificate/certificate_key.py` & `pkilint-0.8.1/pkilint/pkix/certificate/certificate_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/certificate/certificate_name.py` & `pkilint-0.8.1/pkilint/pkix/certificate/certificate_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/certificate/certificate_validator.py` & `pkilint-0.8.1/pkilint/pkix/certificate/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/certificate/certificate_validity.py` & `pkilint-0.8.1/pkilint/pkix/certificate/certificate_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/crl/__init__.py` & `pkilint-0.8.1/pkilint/pkix/crl/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/crl/crl_extension.py` & `pkilint-0.8.1/pkilint/pkix/crl/crl_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/crl/crl_validator.py` & `pkilint-0.8.1/pkilint/pkix/crl/crl_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/crl/crl_validity.py` & `pkilint-0.8.1/pkilint/pkix/crl/crl_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/extension.py` & `pkilint-0.8.1/pkilint/pkix/extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/general_name.py` & `pkilint-0.8.1/pkilint/pkix/general_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/name.py` & `pkilint-0.8.1/pkilint/pkix/name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/ocsp/__init__.py` & `pkilint-0.8.1/pkilint/pkix/ocsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/ocsp/ocsp_basic_response.py` & `pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_basic_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/ocsp/ocsp_response.py` & `pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/ocsp/ocsp_validity.py` & `pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/pkix/time.py` & `pkilint-0.8.1/pkilint/pkix/time.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/report.py` & `pkilint-0.8.1/pkilint/report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/util.py` & `pkilint-0.8.1/pkilint/util.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint/validation.py` & `pkilint-0.8.1/pkilint/validation.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/pkilint.egg-info/PKG-INFO` & `pkilint-0.8.1/pkilint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.0
+Version: 0.8.1
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pkilint
 
 
-[![PyPI](https://img.shields.io/pypi/v/pkilint.svg?maxAge=2592000)](https://pypi.org/project/pkilint)
-[![Python Versions](https://img.shields.io/pypi/pyversions/pkilint.svg)](https://pypi.org/project/pkilint/)
+[![PyPI](https://img.shields.io/pypi/v/pkilint)](https://pypi.org/project/pkilint)
+[![Python Versions](https://img.shields.io/pypi/pyversions/pkilint)](https://pypi.org/project/pkilint/)
 [![Build status](https://github.com/digicert/pkilint/actions/workflows/build_and_publish.yml/badge.svg)](https://github.com/digicert/pkilint/actions/workflows/build_and_publish.yml)
 [![GitHub license](https://img.shields.io/pypi/l/pkilint)](https://raw.githubusercontent.com/digicert/pkilint/main/LICENSE)
 
 pkilint is a linting framework for documents that are encoded using ASN.1. pkilint is designed to
 be a highly extensible toolbox to quickly create linters for a variety of ASN.1 structure/"document" types to check for compliance with
 various standards and policies.
```

### Comparing `pkilint-0.8.0/pkilint.egg-info/SOURCES.txt` & `pkilint-0.8.1/pkilint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/setup.cfg` & `pkilint-0.8.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 author_email = corey.bonnell@digicert.com
 url = https://github.com/digicert/pkilint
 description = A framework for verifying PKI structures
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 platform = any
-python_requires = '>=3.9'
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Programming Language :: Python
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = True
 packages = find:
+python_requires = >=3.9
 install_requires = 
 	pyasn1
 	pyasn1-alt-modules
 	pyyaml
 	cryptography
 	iso3166
 	validators
```

### Comparing `pkilint-0.8.0/tests/integration_certificate/__init__.py` & `pkilint-0.8.1/tests/integration_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/tests/integration_certificate/test_cabf_smime_cert.py` & `pkilint-0.8.1/tests/integration_certificate/test_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/tests/itu/test_bitstring.py` & `pkilint-0.8.1/tests/itu/test_bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/tests/itu/test_string.py` & `pkilint-0.8.1/tests/itu/test_string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.0/tests/util.py` & `pkilint-0.8.1/tests/util.py`

 * *Files identical despite different names*

