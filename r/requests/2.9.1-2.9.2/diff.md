# Comparing `tmp/requests-2.9.1.tar.gz` & `tmp/requests-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests-2.9.1.tar", last modified: Mon Dec 21 14:54:58 2015, max compression
+gzip compressed data, was "dist/requests-2.9.2.tar", last modified: Fri Apr 29 21:57:09 2016, max compression
```

## Comparing `requests-2.9.1.tar` & `requests-2.9.2.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/
--rw-r--r--   0 cory       (501) staff       (20)    32942 2015-12-21 14:52:43.000000 requests-2.9.1/HISTORY.rst
--rw-r--r--   0 cory       (501) staff       (20)      581 2015-12-18 13:37:38.000000 requests-2.9.1/LICENSE
--rw-r--r--   0 cory       (501) staff       (20)      100 2015-05-26 19:52:24.000000 requests-2.9.1/MANIFEST.in
--rw-r--r--   0 cory       (501) staff       (20)     2292 2015-12-18 13:37:38.000000 requests-2.9.1/NOTICE
--rw-r--r--   0 cory       (501) staff       (20)    46161 2015-12-21 14:54:58.000000 requests-2.9.1/PKG-INFO
--rw-r--r--   0 cory       (501) staff       (20)     2748 2015-12-18 13:37:38.000000 requests-2.9.1/README.rst
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/
--rw-r--r--   0 cory       (501) staff       (20)     2007 2015-12-21 14:53:09.000000 requests-2.9.1/requests/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)    17495 2015-12-18 13:37:38.000000 requests-2.9.1/requests/adapters.py
--rw-r--r--   0 cory       (501) staff       (20)     5419 2015-12-18 13:37:38.000000 requests-2.9.1/requests/api.py
--rw-r--r--   0 cory       (501) staff       (20)     7550 2015-12-18 13:37:38.000000 requests-2.9.1/requests/auth.py
--rw-r--r--   0 cory       (501) staff       (20)   344712 2015-12-18 13:37:38.000000 requests-2.9.1/requests/cacert.pem
--rw-r--r--   0 cory       (501) staff       (20)      613 2015-12-18 13:37:38.000000 requests-2.9.1/requests/certs.py
--rw-r--r--   0 cory       (501) staff       (20)     1469 2015-12-18 13:37:38.000000 requests-2.9.1/requests/compat.py
--rw-r--r--   0 cory       (501) staff       (20)    17387 2015-12-18 13:37:38.000000 requests-2.9.1/requests/cookies.py
--rw-r--r--   0 cory       (501) staff       (20)     2776 2015-12-18 13:37:38.000000 requests-2.9.1/requests/exceptions.py
--rw-r--r--   0 cory       (501) staff       (20)      767 2015-12-18 13:37:38.000000 requests-2.9.1/requests/hooks.py
--rw-r--r--   0 cory       (501) staff       (20)    29277 2015-12-18 13:37:38.000000 requests-2.9.1/requests/models.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/
--rw-r--r--   0 cory       (501) staff       (20)     1384 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/__init__.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/chardet/
--rw-r--r--   0 cory       (501) staff       (20)     1295 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)    82594 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/big5freq.py
--rw-r--r--   0 cory       (501) staff       (20)     1684 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/big5prober.py
--rwxr-xr-x   0 cory       (501) staff       (20)     2504 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/chardetect.py
--rw-r--r--   0 cory       (501) staff       (20)     9226 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/chardistribution.py
--rw-r--r--   0 cory       (501) staff       (20)     3791 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/charsetgroupprober.py
--rw-r--r--   0 cory       (501) staff       (20)     1902 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/charsetprober.py
--rw-r--r--   0 cory       (501) staff       (20)     2318 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/codingstatemachine.py
--rw-r--r--   0 cory       (501) staff       (20)     1157 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/compat.py
--rw-r--r--   0 cory       (501) staff       (20)     1335 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/constants.py
--rw-r--r--   0 cory       (501) staff       (20)     1782 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/cp949prober.py
--rw-r--r--   0 cory       (501) staff       (20)     3187 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/escprober.py
--rw-r--r--   0 cory       (501) staff       (20)     7839 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/escsm.py
--rw-r--r--   0 cory       (501) staff       (20)     3678 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/eucjpprober.py
--rw-r--r--   0 cory       (501) staff       (20)    45978 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/euckrfreq.py
--rw-r--r--   0 cory       (501) staff       (20)     1675 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/euckrprober.py
--rw-r--r--   0 cory       (501) staff       (20)    34872 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/euctwfreq.py
--rw-r--r--   0 cory       (501) staff       (20)     1676 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/euctwprober.py
--rw-r--r--   0 cory       (501) staff       (20)    36011 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/gb2312freq.py
--rw-r--r--   0 cory       (501) staff       (20)     1681 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/gb2312prober.py
--rw-r--r--   0 cory       (501) staff       (20)    13359 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/hebrewprober.py
--rw-r--r--   0 cory       (501) staff       (20)    47315 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/jisfreq.py
--rw-r--r--   0 cory       (501) staff       (20)    19348 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/jpcntx.py
--rw-r--r--   0 cory       (501) staff       (20)    12784 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/langbulgarianmodel.py
--rw-r--r--   0 cory       (501) staff       (20)    17725 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/langcyrillicmodel.py
--rw-r--r--   0 cory       (501) staff       (20)    12628 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/langgreekmodel.py
--rw-r--r--   0 cory       (501) staff       (20)    11318 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/langhebrewmodel.py
--rw-r--r--   0 cory       (501) staff       (20)    12536 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/langhungarianmodel.py
--rw-r--r--   0 cory       (501) staff       (20)    11275 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/langthaimodel.py
--rw-r--r--   0 cory       (501) staff       (20)     5232 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/latin1prober.py
--rw-r--r--   0 cory       (501) staff       (20)     3268 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/mbcharsetprober.py
--rw-r--r--   0 cory       (501) staff       (20)     1967 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/mbcsgroupprober.py
--rw-r--r--   0 cory       (501) staff       (20)    19590 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/mbcssm.py
--rw-r--r--   0 cory       (501) staff       (20)     4793 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/sbcharsetprober.py
--rw-r--r--   0 cory       (501) staff       (20)     3291 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/sbcsgroupprober.py
--rw-r--r--   0 cory       (501) staff       (20)     3764 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/sjisprober.py
--rw-r--r--   0 cory       (501) staff       (20)     6840 2015-12-18 13:37:38.000000 requests-2.9.1/requests/packages/chardet/universaldetector.py
--rw-r--r--   0 cory       (501) staff       (20)     2652 2015-05-26 19:52:24.000000 requests-2.9.1/requests/packages/chardet/utf8prober.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/urllib3/
--rw-r--r--   0 cory       (501) staff       (20)     2648 2015-12-21 14:52:43.000000 requests-2.9.1/requests/packages/urllib3/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)    10542 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/_collections.py
--rw-r--r--   0 cory       (501) staff       (20)    10286 2015-12-21 14:52:43.000000 requests-2.9.1/requests/packages/urllib3/connection.py
--rw-r--r--   0 cory       (501) staff       (20)    31221 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/connectionpool.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/urllib3/contrib/
--rw-r--r--   0 cory       (501) staff       (20)        0 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)     7531 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 cory       (501) staff       (20)     4546 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 cory       (501) staff       (20)    10094 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 cory       (501) staff       (20)     5440 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/exceptions.py
--rw-r--r--   0 cory       (501) staff       (20)     5872 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/fields.py
--rw-r--r--   0 cory       (501) staff       (20)     2320 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/filepost.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/urllib3/packages/
--rw-r--r--   0 cory       (501) staff       (20)      109 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/packages/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)     8935 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/packages/ordered_dict.py
--rw-r--r--   0 cory       (501) staff       (20)    11628 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/packages/six.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 cory       (501) staff       (20)      460 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)     3778 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 cory       (501) staff       (20)     9470 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/poolmanager.py
--rw-r--r--   0 cory       (501) staff       (20)     5988 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/request.py
--rw-r--r--   0 cory       (501) staff       (20)    18103 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/response.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests/packages/urllib3/util/
--rw-r--r--   0 cory       (501) staff       (20)      854 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/__init__.py
--rw-r--r--   0 cory       (501) staff       (20)     3380 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/connection.py
--rw-r--r--   0 cory       (501) staff       (20)     2128 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/request.py
--rw-r--r--   0 cory       (501) staff       (20)     2167 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/response.py
--rw-r--r--   0 cory       (501) staff       (20)     9981 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/retry.py
--rw-r--r--   0 cory       (501) staff       (20)    11401 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/ssl_.py
--rw-r--r--   0 cory       (501) staff       (20)     9596 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/timeout.py
--rw-r--r--   0 cory       (501) staff       (20)     5879 2015-12-19 08:40:26.000000 requests-2.9.1/requests/packages/urllib3/util/url.py
--rw-r--r--   0 cory       (501) staff       (20)    24544 2015-12-18 13:37:38.000000 requests-2.9.1/requests/sessions.py
--rw-r--r--   0 cory       (501) staff       (20)     3280 2015-12-18 13:37:38.000000 requests-2.9.1/requests/status_codes.py
--rw-r--r--   0 cory       (501) staff       (20)     2977 2015-12-18 13:37:38.000000 requests-2.9.1/requests/structures.py
--rw-r--r--   0 cory       (501) staff       (20)    21845 2015-12-21 14:52:43.000000 requests-2.9.1/requests/utils.py
-drwxr-xr-x   0 cory       (501) staff       (20)        0 2015-12-21 14:54:58.000000 requests-2.9.1/requests.egg-info/
--rw-r--r--   0 cory       (501) staff       (20)        1 2015-12-21 14:54:57.000000 requests-2.9.1/requests.egg-info/dependency_links.txt
--rw-r--r--   0 cory       (501) staff       (20)        1 2015-10-06 14:47:29.000000 requests-2.9.1/requests.egg-info/not-zip-safe
--rw-r--r--   0 cory       (501) staff       (20)    46161 2015-12-21 14:54:57.000000 requests-2.9.1/requests.egg-info/PKG-INFO
--rw-r--r--   0 cory       (501) staff       (20)       51 2015-12-21 14:54:57.000000 requests-2.9.1/requests.egg-info/requires.txt
--rw-r--r--   0 cory       (501) staff       (20)     3401 2015-12-21 14:54:58.000000 requests-2.9.1/requests.egg-info/SOURCES.txt
--rw-r--r--   0 cory       (501) staff       (20)        9 2015-12-21 14:54:57.000000 requests-2.9.1/requests.egg-info/top_level.txt
--rw-r--r--   0 cory       (501) staff       (20)       86 2015-12-18 13:37:38.000000 requests-2.9.1/requirements.txt
--rw-r--r--   0 cory       (501) staff       (20)       82 2015-12-21 14:54:58.000000 requests-2.9.1/setup.cfg
--rwxr-xr-x   0 cory       (501) staff       (20)     2080 2015-12-18 13:37:38.000000 requests-2.9.1/setup.py
--rwxr-xr-x   0 cory       (501) staff       (20)    60734 2015-12-18 13:37:38.000000 requests-2.9.1/test_requests.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    33355 2016-04-29 21:51:36.000000 requests-2.9.2/HISTORY.rst
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      581 2016-02-02 07:35:16.000000 requests-2.9.2/LICENSE
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      100 2015-09-18 21:53:51.000000 requests-2.9.2/MANIFEST.in
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2292 2016-02-19 01:40:29.000000 requests-2.9.2/NOTICE
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    47535 2016-04-29 21:57:09.000000 requests-2.9.2/PKG-INFO
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3310 2016-02-19 01:41:04.000000 requests-2.9.2/README.rst
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2035 2016-04-29 21:56:32.000000 requests-2.9.2/requests/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    17698 2016-04-29 21:48:41.000000 requests-2.9.2/requests/adapters.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     5795 2016-04-29 21:48:41.000000 requests-2.9.2/requests/api.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     8075 2016-04-29 21:48:41.000000 requests-2.9.2/requests/auth.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)   344712 2016-02-02 05:11:59.000000 requests-2.9.2/requests/cacert.pem
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      613 2015-09-18 21:53:51.000000 requests-2.9.2/requests/certs.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1469 2015-09-18 21:53:51.000000 requests-2.9.2/requests/compat.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    17564 2016-04-29 21:48:41.000000 requests-2.9.2/requests/cookies.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2776 2016-02-18 09:48:03.000000 requests-2.9.2/requests/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      767 2016-02-02 05:11:59.000000 requests-2.9.2/requests/hooks.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    29530 2016-04-29 21:48:41.000000 requests-2.9.2/requests/models.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1384 2016-02-03 08:33:44.000000 requests-2.9.2/requests/packages/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/chardet/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1295 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    82594 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/big5freq.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1684 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/big5prober.py
+-rwxr-xr-x   0 kennethreitz   (501) staff       (20)     2504 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/chardetect.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     9226 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/chardistribution.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3791 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/charsetgroupprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1902 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/charsetprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2318 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/codingstatemachine.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1157 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/compat.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1335 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/constants.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1782 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/cp949prober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3187 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/escprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     7839 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/escsm.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3678 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/eucjpprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    45978 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/euckrfreq.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1675 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/euckrprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    34872 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/euctwfreq.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1676 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/euctwprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    36011 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/gb2312freq.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1681 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/gb2312prober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    13359 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/hebrewprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    47315 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/jisfreq.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    19348 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/jpcntx.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    12784 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/langbulgarianmodel.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    17725 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/langcyrillicmodel.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    12628 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/langgreekmodel.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    11318 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/langhebrewmodel.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    12536 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/langhungarianmodel.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    11275 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/langthaimodel.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     5232 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/latin1prober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3268 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/mbcharsetprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     1967 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/mbcsgroupprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    19590 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/mbcssm.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     4793 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/sbcharsetprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3291 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/sbcsgroupprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3764 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/sjisprober.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     6840 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/universaldetector.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2652 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/chardet/utf8prober.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/urllib3/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2648 2016-02-03 08:26:50.000000 requests-2.9.2/requests/packages/urllib3/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    10542 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/_collections.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    10286 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/connection.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    31220 2016-04-29 21:48:41.000000 requests-2.9.2/requests/packages/urllib3/connectionpool.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/urllib3/contrib/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)        0 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     7530 2016-04-29 21:48:41.000000 requests-2.9.2/requests/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     4546 2016-02-03 08:26:50.000000 requests-2.9.2/requests/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    10094 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     5440 2016-02-03 08:26:50.000000 requests-2.9.2/requests/packages/urllib3/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     5872 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/fields.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2320 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/filepost.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/urllib3/packages/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      109 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/packages/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     8935 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/urllib3/packages/ordered_dict.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    11628 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/urllib3/packages/six.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      460 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3778 2015-09-18 21:53:51.000000 requests-2.9.2/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     9470 2016-02-03 08:26:50.000000 requests-2.9.2/requests/packages/urllib3/poolmanager.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     5988 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/request.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    18103 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/response.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests/packages/urllib3/util/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      854 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/util/__init__.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3380 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/util/connection.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2128 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/util/request.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     2167 2016-02-03 08:26:50.000000 requests-2.9.2/requests/packages/urllib3/util/response.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     9981 2016-02-03 08:26:50.000000 requests-2.9.2/requests/packages/urllib3/util/retry.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    11399 2016-04-29 21:48:41.000000 requests-2.9.2/requests/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     9596 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/util/timeout.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     5879 2016-02-02 05:11:59.000000 requests-2.9.2/requests/packages/urllib3/util/url.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    24897 2016-04-29 21:48:41.000000 requests-2.9.2/requests/sessions.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3315 2016-04-29 21:48:41.000000 requests-2.9.2/requests/status_codes.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3017 2016-04-29 21:48:41.000000 requests-2.9.2/requests/structures.py
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    22228 2016-04-29 21:48:41.000000 requests-2.9.2/requests/utils.py
+drwxr-xr-x   0 kennethreitz   (501) staff       (20)        0 2016-04-29 21:57:09.000000 requests-2.9.2/requests.egg-info/
+-rw-r--r--   0 kennethreitz   (501) staff       (20)        1 2016-04-29 21:57:09.000000 requests-2.9.2/requests.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethreitz   (501) staff       (20)        1 2016-04-29 21:55:27.000000 requests-2.9.2/requests.egg-info/not-zip-safe
+-rw-r--r--   0 kennethreitz   (501) staff       (20)    47535 2016-04-29 21:57:09.000000 requests-2.9.2/requests.egg-info/PKG-INFO
+-rw-r--r--   0 kennethreitz   (501) staff       (20)       51 2016-04-29 21:57:09.000000 requests-2.9.2/requests.egg-info/requires.txt
+-rw-r--r--   0 kennethreitz   (501) staff       (20)     3374 2016-04-29 21:57:09.000000 requests-2.9.2/requests.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethreitz   (501) staff       (20)        9 2016-04-29 21:57:09.000000 requests-2.9.2/requests.egg-info/top_level.txt
+-rw-r--r--   0 kennethreitz   (501) staff       (20)      373 2016-04-29 21:48:41.000000 requests-2.9.2/requirements.txt
+-rw-r--r--   0 kennethreitz   (501) staff       (20)       59 2016-04-29 21:57:09.000000 requests-2.9.2/setup.cfg
+-rwxr-xr-x   0 kennethreitz   (501) staff       (20)     2860 2016-02-19 01:40:29.000000 requests-2.9.2/setup.py
```

### Comparing `requests-2.9.1/HISTORY.rst` & `requests-2.9.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 .. :changelog:
 
 Release History
 ---------------
 
+2.9.2 (04-29-2016)
+++++++++++++++++++
+
+**Improvements**
+
+- Change built-in CaseInsensitiveDict (used for headers) to use OrderedDict
+  as its underlying datastore.
+
+**Bugfixes**
+
+- Don't use redirect_cache if allow_redirects=False
+- When passed objects that throw exceptions from ``tell()``, send them via
+  chunked transfer encoding instead of failing.
+- Raise a ProxyError for proxy related connection issues.
+
 2.9.1 (2015-12-21)
 ++++++++++++++++++
 
 **Bugfixes**
 
 - Resolve regression introduced in 2.9.0 that made it impossible to send binary
   strings as bodies in Python 3.
```

### Comparing `requests-2.9.1/LICENSE` & `requests-2.9.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2015 Kenneth Reitz
+Copyright 2016 Kenneth Reitz
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `requests-2.9.1/NOTICE` & `requests-2.9.2/NOTICE`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/PKG-INFO` & `requests-2.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,92 +1,103 @@
 Metadata-Version: 1.1
 Name: requests
-Version: 2.9.1
+Version: 2.9.2
 Summary: Python HTTP for Humans.
 Home-page: http://python-requests.org
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: Apache 2.0
 Description: Requests: HTTP for Humans
         =========================
         
         .. image:: https://img.shields.io/pypi/v/requests.svg
             :target: https://pypi.python.org/pypi/requests
         
         .. image:: https://img.shields.io/pypi/dm/requests.svg
                 :target: https://pypi.python.org/pypi/requests
         
+        Requests is the only *Non-GMO* HTTP library for Python, safe for human
+        consumption.
         
+        **Warning:** Recreational use of other HTTP libraries may result in dangerous side-effects,
+        including: security vulnerabilities, verbose code, reinventing the wheel,
+        constantly reading documentation, depression, headaches, or even death.
         
-        
-        Requests is an Apache2 Licensed HTTP library, written in Python, for human
-        beings.
-        
-        Most existing Python modules for sending HTTP requests are extremely
-        verbose and cumbersome. Python's builtin urllib2 module provides most of
-        the HTTP capabilities you should need, but the api is thoroughly broken.
-        It requires an enormous amount of work (even method overrides) to
-        perform the simplest of tasks.
-        
-        Things shouldn't be this way. Not in Python.
+        Behold, the power of Requests:
         
         .. code-block:: python
         
-            >>> r = requests.get('https://api.github.com', auth=('user', 'pass'))
+            >>> r = requests.get('https://api.github.com/user', auth=('user', 'pass'))
             >>> r.status_code
-            204
+            200
             >>> r.headers['content-type']
-            'application/json'
+            'application/json; charset=utf8'
+            >>> r.encoding
+            'utf-8'
             >>> r.text
-            ...
-        
-        See `the same code, without Requests <https://gist.github.com/973705>`_.
-        
-        Requests allow you to send HTTP/1.1 requests. You can add headers, form data,
-        multipart files, and parameters with simple Python dictionaries, and access the
-        response data in the same way. It's powered by httplib and `urllib3
-        <https://github.com/shazow/urllib3>`_, but it does all the hard work and crazy
-        hacks for you.
+            u'{"type":"User"...'
+            >>> r.json()
+            {u'disk_usage': 368627, u'private_gists': 484, ...}
+        
+        See `the similar code, sans Requests <https://gist.github.com/973705>`_.
+        
+        Requests allows you to send *organic, grass-fed* HTTP/1.1 requests, without the
+        need for manual labor. There's no need to manually add query strings to your
+        URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling
+        are 100% automatic, powered by `urllib3 <https://github.com/shazow/urllib3>`_,
+        which is embedded within Requests.
+        
+        Besides, all the cool kids are doing it. Requests is one of the most
+        downloaded Python packages of all time, pulling in over 7,000,000 downloads
+        every month. You don't want to be left out!
         
+        Feature Support
+        ---------------
         
-        Features
-        --------
+        Requests is ready for today's web.
         
         - International Domains and URLs
         - Keep-Alive & Connection Pooling
         - Sessions with Cookie Persistence
         - Browser-style SSL Verification
         - Basic/Digest Authentication
         - Elegant Key/Value Cookies
         - Automatic Decompression
+        - Automatic Content Decoding
         - Unicode Response Bodies
         - Multipart File Uploads
+        - HTTP(S) Proxy Support
         - Connection Timeouts
+        - Streaming Downloads
+        - ``.netrc`` Support
+        - Chunked Requests
         - Thread-safety
-        - HTTP(S) proxy support
         
+        Requests supports Python 2.6 — 3.5, and runs great on PyPy.
         
         Installation
         ------------
         
         To install Requests, simply:
         
         .. code-block:: bash
         
             $ pip install requests
+            ✨🍰✨
         
+        Satisfaction, guaranteed.
         
         Documentation
         -------------
         
-        Documentation is available at http://docs.python-requests.org/.
+        Fantastic documentation is available at http://docs.python-requests.org/, for a limited time only.
         
         
-        Contribute
-        ----------
+        How to Contribute
+        -----------------
         
         #. Check for open issues or open a fresh issue to start a discussion around a feature idea or a bug. There is a `Contributor Friendly`_ tag for issues that should be ideal for people who are not very familiar with the codebase yet.
         #. Fork `the repository`_ on GitHub to start making your changes to the **master** branch (or branch off of it).
         #. Write a test which shows that the bug was fixed or that the feature works as expected.
         #. Send a pull request and bug the maintainer until it gets merged and published. :) Make sure to add yourself to AUTHORS_.
         
         .. _`the repository`: http://github.com/kennethreitz/requests
@@ -95,14 +106,29 @@
         
         
         .. :changelog:
         
         Release History
         ---------------
         
+        2.9.2 (04-29-2016)
+        ++++++++++++++++++
+        
+        **Improvements**
+        
+        - Change built-in CaseInsensitiveDict (used for headers) to use OrderedDict
+          as its underlying datastore.
+        
+        **Bugfixes**
+        
+        - Don't use redirect_cache if allow_redirects=False
+        - When passed objects that throw exceptions from ``tell()``, send them via
+          chunked transfer encoding instead of failing.
+        - Raise a ProxyError for proxy related connection issues.
+        
         2.9.1 (2015-12-21)
         ++++++++++++++++++
         
         **Bugfixes**
         
         - Resolve regression introduced in 2.9.0 that made it impossible to send binary
           strings as bodies in Python 3.
@@ -1227,12 +1253,15 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `requests-2.9.1/README.rst` & `requests-2.9.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -3,82 +3,93 @@
 
 .. image:: https://img.shields.io/pypi/v/requests.svg
     :target: https://pypi.python.org/pypi/requests
 
 .. image:: https://img.shields.io/pypi/dm/requests.svg
         :target: https://pypi.python.org/pypi/requests
 
+Requests is the only *Non-GMO* HTTP library for Python, safe for human
+consumption.
 
+**Warning:** Recreational use of other HTTP libraries may result in dangerous side-effects,
+including: security vulnerabilities, verbose code, reinventing the wheel,
+constantly reading documentation, depression, headaches, or even death.
 
-
-Requests is an Apache2 Licensed HTTP library, written in Python, for human
-beings.
-
-Most existing Python modules for sending HTTP requests are extremely
-verbose and cumbersome. Python's builtin urllib2 module provides most of
-the HTTP capabilities you should need, but the api is thoroughly broken.
-It requires an enormous amount of work (even method overrides) to
-perform the simplest of tasks.
-
-Things shouldn't be this way. Not in Python.
+Behold, the power of Requests:
 
 .. code-block:: python
 
-    >>> r = requests.get('https://api.github.com', auth=('user', 'pass'))
+    >>> r = requests.get('https://api.github.com/user', auth=('user', 'pass'))
     >>> r.status_code
-    204
+    200
     >>> r.headers['content-type']
-    'application/json'
+    'application/json; charset=utf8'
+    >>> r.encoding
+    'utf-8'
     >>> r.text
-    ...
-
-See `the same code, without Requests <https://gist.github.com/973705>`_.
-
-Requests allow you to send HTTP/1.1 requests. You can add headers, form data,
-multipart files, and parameters with simple Python dictionaries, and access the
-response data in the same way. It's powered by httplib and `urllib3
-<https://github.com/shazow/urllib3>`_, but it does all the hard work and crazy
-hacks for you.
+    u'{"type":"User"...'
+    >>> r.json()
+    {u'disk_usage': 368627, u'private_gists': 484, ...}
+
+See `the similar code, sans Requests <https://gist.github.com/973705>`_.
+
+Requests allows you to send *organic, grass-fed* HTTP/1.1 requests, without the
+need for manual labor. There's no need to manually add query strings to your
+URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling
+are 100% automatic, powered by `urllib3 <https://github.com/shazow/urllib3>`_,
+which is embedded within Requests.
+
+Besides, all the cool kids are doing it. Requests is one of the most
+downloaded Python packages of all time, pulling in over 7,000,000 downloads
+every month. You don't want to be left out!
 
+Feature Support
+---------------
 
-Features
---------
+Requests is ready for today's web.
 
 - International Domains and URLs
 - Keep-Alive & Connection Pooling
 - Sessions with Cookie Persistence
 - Browser-style SSL Verification
 - Basic/Digest Authentication
 - Elegant Key/Value Cookies
 - Automatic Decompression
+- Automatic Content Decoding
 - Unicode Response Bodies
 - Multipart File Uploads
+- HTTP(S) Proxy Support
 - Connection Timeouts
+- Streaming Downloads
+- ``.netrc`` Support
+- Chunked Requests
 - Thread-safety
-- HTTP(S) proxy support
 
+Requests supports Python 2.6 — 3.5, and runs great on PyPy.
 
 Installation
 ------------
 
 To install Requests, simply:
 
 .. code-block:: bash
 
     $ pip install requests
+    ✨🍰✨
 
+Satisfaction, guaranteed.
 
 Documentation
 -------------
 
-Documentation is available at http://docs.python-requests.org/.
+Fantastic documentation is available at http://docs.python-requests.org/, for a limited time only.
 
 
-Contribute
-----------
+How to Contribute
+-----------------
 
 #. Check for open issues or open a fresh issue to start a discussion around a feature idea or a bug. There is a `Contributor Friendly`_ tag for issues that should be ideal for people who are not very familiar with the codebase yet.
 #. Fork `the repository`_ on GitHub to start making your changes to the **master** branch (or branch off of it).
 #. Write a test which shows that the bug was fixed or that the feature works as expected.
 #. Send a pull request and bug the maintainer until it gets merged and published. :) Make sure to add yourself to AUTHORS_.
 
 .. _`the repository`: http://github.com/kennethreitz/requests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `requests-2.9.1/requests/__init__.py` & `requests-2.9.2/requests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 
 :copyright: (c) 2015 by Kenneth Reitz.
 :license: Apache 2.0, see LICENSE for more details.
 
 """
 
 __title__ = 'requests'
-__version__ = '2.9.1'
-__build__ = 0x020901
+__version__ = '2.9.2'
+__build__ = 0x020902
 __author__ = 'Kenneth Reitz'
 __license__ = 'Apache 2.0'
-__copyright__ = 'Copyright 2015 Kenneth Reitz'
+__copyright__ = 'Copyright 2016 Kenneth Reitz'
 
 # Attempt to enable urllib3's SNI support, if possible
 try:
     from .packages.urllib3.contrib import pyopenssl
     pyopenssl.inject_into_urllib3()
 except ImportError:
     pass
@@ -59,15 +59,15 @@
 from .models import Request, Response, PreparedRequest
 from .api import request, get, head, post, patch, put, delete, options
 from .sessions import session, Session
 from .status_codes import codes
 from .exceptions import (
     RequestException, Timeout, URLRequired,
     TooManyRedirects, HTTPError, ConnectionError,
-    FileModeWarning,
+    FileModeWarning, ConnectTimeout, ReadTimeout
 )
 
 # Set default logging handler to avoid "No handler found" warnings.
 import logging
 try:  # Python 2.7+
     from logging import NullHandler
 except ImportError:
```

### Comparing `requests-2.9.1/requests/adapters.py` & `requests-2.9.2/requests/adapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     Provides a general-case interface for Requests sessions to contact HTTP and
     HTTPS urls by implementing the Transport Adapter interface. This class will
     usually be created by the :class:`Session <Session>` class under the
     covers.
 
     :param pool_connections: The number of urllib3 connection pools to cache.
     :param pool_maxsize: The maximum number of connections to save in the pool.
-    :param int max_retries: The maximum number of retries each connection
+    :param max_retries: The maximum number of retries each connection
         should attempt. Note, this applies only to failed DNS lookups, socket
         connections and connection timeouts, never to requests where data has
         made it to the server. By default, Requests does not retry failed
         connections. If you need granular control over the conditions under
         which we retry a request, import urllib3's ``Retry`` class and pass
         that instead.
     :param pool_block: Whether the connection pool should block for connections.
@@ -260,18 +260,20 @@
             conn = self.poolmanager.connection_from_url(url)
 
         return conn
 
     def close(self):
         """Disposes of any internal state.
 
-        Currently, this just closes the PoolManager, which closes pooled
-        connections.
+        Currently, this closes the PoolManager and any active ProxyManager,
+        which closes any pooled connections.
         """
         self.poolmanager.clear()
+        for proxy in self.proxy_manager.values():
+            proxy.clear()
 
     def request_url(self, request, proxies):
         """Obtain the url to use when making the final request.
 
         If the message is being sent through a HTTP proxy, the full URL has to
         be used. Otherwise, we should only use the path portion of the URL.
 
@@ -430,14 +432,17 @@
                 # TODO: Remove this in 3.0.0: see #2811
                 if not isinstance(e.reason, NewConnectionError):
                     raise ConnectTimeout(e, request=request)
 
             if isinstance(e.reason, ResponseError):
                 raise RetryError(e, request=request)
 
+            if isinstance(e.reason, _ProxyError):
+                raise ProxyError(e, request=request)
+
             raise ConnectionError(e, request=request)
 
         except ClosedPoolError as e:
             raise ConnectionError(e, request=request)
 
         except _ProxyError as e:
             raise ProxyError(e)
```

### Comparing `requests-2.9.1/requests/api.py` & `requests-2.9.2/requests/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     :param method: method for the new :class:`Request` object.
     :param url: URL for the new :class:`Request` object.
     :param params: (optional) Dictionary or bytes to be sent in the query string for the :class:`Request`.
     :param data: (optional) Dictionary, bytes, or file-like object to send in the body of the :class:`Request`.
     :param json: (optional) json data to send in the body of the :class:`Request`.
     :param headers: (optional) Dictionary of HTTP Headers to send with the :class:`Request`.
     :param cookies: (optional) Dict or CookieJar object to send with the :class:`Request`.
-    :param files: (optional) Dictionary of ``'name': file-like-objects`` (or ``{'name': ('filename', fileobj)}``) for multipart encoding upload.
+    :param files: (optional) Dictionary of ``'name': file-like-objects`` (or ``{'name': file-tuple}``) for multipart encoding upload.
+        ``file-tuple`` can be a 2-tuple ``('filename', fileobj)``, 3-tuple ``('filename', fileobj, 'content_type')``
+        or a 4-tuple ``('filename', fileobj, 'content_type', custom_headers)``, where ``'content-type'`` is a string
+        defining the content type of the given file and ``custom_headers`` a dict-like object containing additional headers
+        to add for the file.
     :param auth: (optional) Auth tuple to enable Basic/Digest/Custom HTTP Auth.
     :param timeout: (optional) How long to wait for the server to send data
         before giving up, as a float, or a :ref:`(connect timeout, read
         timeout) <timeouts>` tuple.
     :type timeout: float or tuple
     :param allow_redirects: (optional) Boolean. Set to True if POST/PUT/DELETE redirect following is allowed.
     :type allow_redirects: bool
```

### Comparing `requests-2.9.1/requests/auth.py` & `requests-2.9.2/requests/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,23 @@
 
 class HTTPBasicAuth(AuthBase):
     """Attaches HTTP Basic Authentication to the given Request object."""
     def __init__(self, username, password):
         self.username = username
         self.password = password
 
+    def __eq__(self, other):
+        return all([
+            self.username == getattr(other, 'username', None),
+            self.password == getattr(other, 'password', None)
+        ])
+
+    def __ne__(self, other):
+        return not self == other
+
     def __call__(self, r):
         r.headers['Authorization'] = _basic_auth_str(self.username, self.password)
         return r
 
 
 class HTTPProxyAuth(HTTPBasicAuth):
     """Attaches HTTP Proxy Authentication to a given Request object."""
@@ -80,14 +89,15 @@
     def build_digest_header(self, method, url):
 
         realm = self._thread_local.chal['realm']
         nonce = self._thread_local.chal['nonce']
         qop = self._thread_local.chal.get('qop')
         algorithm = self._thread_local.chal.get('algorithm')
         opaque = self._thread_local.chal.get('opaque')
+        hash_utf8 = None
 
         if algorithm is None:
             _algorithm = 'MD5'
         else:
             _algorithm = algorithm.upper()
         # lambdas assume digest modules are imported at the top level
         if _algorithm == 'MD5' or _algorithm == 'MD5-SESS':
@@ -217,7 +227,16 @@
             # None.
             self._thread_local.pos = None
         r.register_hook('response', self.handle_401)
         r.register_hook('response', self.handle_redirect)
         self._thread_local.num_401_calls = 1
 
         return r
+
+    def __eq__(self, other):
+        return all([
+            self.username == getattr(other, 'username', None),
+            self.password == getattr(other, 'password', None)
+        ])
+
+    def __ne__(self, other):
+        return not self == other
```

### Comparing `requests-2.9.1/requests/cacert.pem` & `requests-2.9.2/requests/cacert.pem`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/certs.py` & `requests-2.9.2/requests/certs.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/compat.py` & `requests-2.9.2/requests/compat.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/cookies.py` & `requests-2.9.2/requests/cookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,20 @@
         dictionary = {}
         for cookie in iter(self):
             if (domain is None or cookie.domain == domain) and (path is None
                                                 or cookie.path == path):
                 dictionary[cookie.name] = cookie.value
         return dictionary
 
+    def __contains__(self, name):
+        try:
+            return super(RequestsCookieJar, self).__contains__(name)
+        except CookieConflictError:
+            return True
+
     def __getitem__(self, name):
         """Dict-like __getitem__() for compatibility with client code. Throws
         exception if there are more than one cookie with name. In that case,
         use the more explicit get() method instead.
 
         .. warning:: operation is O(n), not O(1)."""
```

### Comparing `requests-2.9.1/requests/exceptions.py` & `requests-2.9.2/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/hooks.py` & `requests-2.9.2/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/models.py` & `requests-2.9.2/requests/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,18 @@
             return data
 
     @staticmethod
     def _encode_files(files, data):
         """Build the body for a multipart/form-data request.
 
         Will successfully encode files when passed as a dict or a list of
-        2-tuples. Order is retained if data is a list of 2-tuples but arbitrary
+        tuples. Order is retained if data is a list of tuples but arbitrary
         if parameters are supplied as a dict.
+        The tuples may be 2-tuples (filename, fileobj), 3-tuples (filename, fileobj, contentype)
+        or 4-tuples (filename, fileobj, contentype, custom_headers).
 
         """
         if (not files):
             raise ValueError("Files must be provided.")
         elif isinstance(data, basestring):
             raise ValueError("Data must not be a string.")
 
@@ -459,17 +461,19 @@
             if content_type and ('content-type' not in self.headers):
                 self.headers['Content-Type'] = content_type
 
         self.body = body
 
     def prepare_content_length(self, body):
         if hasattr(body, 'seek') and hasattr(body, 'tell'):
+            curr_pos = body.tell()
             body.seek(0, 2)
-            self.headers['Content-Length'] = builtin_str(body.tell())
-            body.seek(0, 0)
+            end_pos = body.tell()
+            self.headers['Content-Length'] = builtin_str(max(0, end_pos - curr_pos))
+            body.seek(curr_pos, 0)
         elif body is not None:
             l = super_len(body)
             if l:
                 self.headers['Content-Length'] = builtin_str(l)
         elif (self.method not in ('GET', 'HEAD')) and (self.headers.get('Content-Length') is None):
             self.headers['Content-Length'] = '0'
```

### Comparing `requests-2.9.1/requests/packages/__init__.py` & `requests-2.9.2/requests/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/__init__.py` & `requests-2.9.2/requests/packages/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/big5freq.py` & `requests-2.9.2/requests/packages/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/big5prober.py` & `requests-2.9.2/requests/packages/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/chardetect.py` & `requests-2.9.2/requests/packages/chardet/chardetect.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/chardistribution.py` & `requests-2.9.2/requests/packages/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/charsetgroupprober.py` & `requests-2.9.2/requests/packages/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/charsetprober.py` & `requests-2.9.2/requests/packages/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/codingstatemachine.py` & `requests-2.9.2/requests/packages/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/compat.py` & `requests-2.9.2/requests/packages/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/constants.py` & `requests-2.9.2/requests/packages/chardet/constants.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/cp949prober.py` & `requests-2.9.2/requests/packages/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/escprober.py` & `requests-2.9.2/requests/packages/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/escsm.py` & `requests-2.9.2/requests/packages/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/eucjpprober.py` & `requests-2.9.2/requests/packages/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/euckrfreq.py` & `requests-2.9.2/requests/packages/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/euckrprober.py` & `requests-2.9.2/requests/packages/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/euctwfreq.py` & `requests-2.9.2/requests/packages/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/euctwprober.py` & `requests-2.9.2/requests/packages/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/gb2312freq.py` & `requests-2.9.2/requests/packages/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/gb2312prober.py` & `requests-2.9.2/requests/packages/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/hebrewprober.py` & `requests-2.9.2/requests/packages/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/jisfreq.py` & `requests-2.9.2/requests/packages/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/jpcntx.py` & `requests-2.9.2/requests/packages/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/langbulgarianmodel.py` & `requests-2.9.2/requests/packages/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/langcyrillicmodel.py` & `requests-2.9.2/requests/packages/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/langgreekmodel.py` & `requests-2.9.2/requests/packages/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/langhebrewmodel.py` & `requests-2.9.2/requests/packages/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/langhungarianmodel.py` & `requests-2.9.2/requests/packages/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/langthaimodel.py` & `requests-2.9.2/requests/packages/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/latin1prober.py` & `requests-2.9.2/requests/packages/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/mbcharsetprober.py` & `requests-2.9.2/requests/packages/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/mbcsgroupprober.py` & `requests-2.9.2/requests/packages/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/mbcssm.py` & `requests-2.9.2/requests/packages/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/sbcharsetprober.py` & `requests-2.9.2/requests/packages/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/sbcsgroupprober.py` & `requests-2.9.2/requests/packages/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/sjisprober.py` & `requests-2.9.2/requests/packages/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/universaldetector.py` & `requests-2.9.2/requests/packages/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/chardet/utf8prober.py` & `requests-2.9.2/requests/packages/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/__init__.py` & `requests-2.9.2/requests/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/_collections.py` & `requests-2.9.2/requests/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/connection.py` & `requests-2.9.2/requests/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/connectionpool.py` & `requests-2.9.2/requests/packages/urllib3/connectionpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,15 +783,15 @@
         if not getattr(conn, 'sock', None):  # AppEngine might not have  `.sock`
             conn.connect()
 
         if not conn.is_verified:
             warnings.warn((
                 'Unverified HTTPS request is being made. '
                 'Adding certificate verification is strongly advised. See: '
-                'https://urllib3.readthedocs.org/en/latest/security.html'),
+                'https://urllib3.readthedocs.io/en/latest/security.html'),
                 InsecureRequestWarning)
 
 
 def connection_from_url(url, **kw):
     """
     Given a url, return an :class:`.ConnectionPool` instance of its host.
```

### Comparing `requests-2.9.1/requests/packages/urllib3/contrib/appengine.py` & `requests-2.9.2/requests/packages/urllib3/contrib/appengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 "Use normal urllib3.PoolManager instead of AppEngineManager"
                 "on Managed VMs, as using URLFetch is not necessary in "
                 "this environment.")
 
         warnings.warn(
             "urllib3 is using URLFetch on Google App Engine sandbox instead "
             "of sockets. To use sockets directly instead of URLFetch see "
-            "https://urllib3.readthedocs.org/en/latest/contrib.html.",
+            "https://urllib3.readthedocs.io/en/latest/contrib.html.",
             AppEnginePlatformWarning)
 
         RequestMethods.__init__(self, headers)
         self.validate_certificate = validate_certificate
 
         self.retries = retries or Retry.DEFAULT
```

### Comparing `requests-2.9.1/requests/packages/urllib3/contrib/ntlmpool.py` & `requests-2.9.2/requests/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/contrib/pyopenssl.py` & `requests-2.9.2/requests/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/exceptions.py` & `requests-2.9.2/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/fields.py` & `requests-2.9.2/requests/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/filepost.py` & `requests-2.9.2/requests/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/packages/ordered_dict.py` & `requests-2.9.2/requests/packages/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/packages/six.py` & `requests-2.9.2/requests/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py` & `requests-2.9.2/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/poolmanager.py` & `requests-2.9.2/requests/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/request.py` & `requests-2.9.2/requests/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/response.py` & `requests-2.9.2/requests/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/__init__.py` & `requests-2.9.2/requests/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/connection.py` & `requests-2.9.2/requests/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/request.py` & `requests-2.9.2/requests/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/response.py` & `requests-2.9.2/requests/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/retry.py` & `requests-2.9.2/requests/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/ssl_.py` & `requests-2.9.2/requests/packages/urllib3/util/ssl_.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             self.ciphers = cipher_suite
 
         def wrap_socket(self, socket, server_hostname=None):
             warnings.warn(
                 'A true SSLContext object is not available. This prevents '
                 'urllib3 from configuring SSL appropriately and may cause '
                 'certain SSL connections to fail. For more information, see '
-                'https://urllib3.readthedocs.org/en/latest/security.html'
+                'https://urllib3.readthedocs.io/en/latest/security.html'
                 '#insecureplatformwarning.',
                 InsecurePlatformWarning
             )
             kwargs = {
                 'keyfile': self.keyfile,
                 'certfile': self.certfile,
                 'ca_certs': self.ca_certs,
@@ -306,12 +306,12 @@
 
     warnings.warn(
         'An HTTPS request has been made, but the SNI (Subject Name '
         'Indication) extension to TLS is not available on this platform. '
         'This may cause the server to present an incorrect TLS '
         'certificate, which can cause validation failures. For more '
         'information, see '
-        'https://urllib3.readthedocs.org/en/latest/security.html'
+        'https://urllib3.readthedocs.io/en/latest/security.html'
         '#snimissingwarning.',
         SNIMissingWarning
     )
     return context.wrap_socket(sock)
```

### Comparing `requests-2.9.1/requests/packages/urllib3/util/timeout.py` & `requests-2.9.2/requests/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/packages/urllib3/util/url.py` & `requests-2.9.2/requests/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `requests-2.9.1/requests/sessions.py` & `requests-2.9.2/requests/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,21 +106,20 @@
 
             try:
                 resp.content  # Consume socket so it can be released
             except (ChunkedEncodingError, ContentDecodingError, RuntimeError):
                 resp.raw.read(decode_content=False)
 
             if i >= self.max_redirects:
-                raise TooManyRedirects('Exceeded %s redirects.' % self.max_redirects)
+                raise TooManyRedirects('Exceeded %s redirects.' % self.max_redirects, response=resp)
 
             # Release the connection back into the pool.
             resp.close()
 
             url = resp.headers['location']
-            method = req.method
 
             # Handle redirection without scheme (see: RFC 1808 Section 4)
             if url.startswith('//'):
                 parsed_rurl = urlparse(resp.url)
                 url = '%s:%s' % (parsed_rurl.scheme, url)
 
             # The scheme should be lower case...
@@ -136,30 +135,15 @@
                 url = requote_uri(url)
 
             prepared_request.url = to_native_string(url)
             # Cache the url, unless it redirects to itself.
             if resp.is_permanent_redirect and req.url != prepared_request.url:
                 self.redirect_cache[req.url] = prepared_request.url
 
-            # http://tools.ietf.org/html/rfc7231#section-6.4.4
-            if (resp.status_code == codes.see_other and
-                    method != 'HEAD'):
-                method = 'GET'
-
-            # Do what the browsers do, despite standards...
-            # First, turn 302s into GETs.
-            if resp.status_code == codes.found and method != 'HEAD':
-                method = 'GET'
-
-            # Second, if a POST is responded to with a 301, turn it into a GET.
-            # This bizarre behaviour is explained in Issue 1704.
-            if resp.status_code == codes.moved and method == 'POST':
-                method = 'GET'
-
-            prepared_request.method = method
+            self.rebuild_method(prepared_request, resp)
 
             # https://github.com/kennethreitz/requests/issues/1084
             if resp.status_code not in (codes.temporary_redirect, codes.permanent_redirect):
                 if 'Content-Length' in prepared_request.headers:
                     del prepared_request.headers['Content-Length']
 
                 prepared_request.body = None
@@ -258,14 +242,36 @@
             username, password = None, None
 
         if username and password:
             headers['Proxy-Authorization'] = _basic_auth_str(username, password)
 
         return new_proxies
 
+    def rebuild_method(self, prepared_request, response):
+        """When being redirected we may want to change the method of the request
+        based on certain specs or browser behavior.
+        """
+        method = prepared_request.method
+
+        # http://tools.ietf.org/html/rfc7231#section-6.4.4
+        if response.status_code == codes.see_other and method != 'HEAD':
+            method = 'GET'
+
+        # Do what the browsers do, despite standards...
+        # First, turn 302s into GETs.
+        if response.status_code == codes.found and method != 'HEAD':
+            method = 'GET'
+
+        # Second, if a POST is responded to with a 301, turn it into a GET.
+        # This bizarre behaviour is explained in Issue 1704.
+        if response.status_code == codes.moved and method == 'POST':
+            method = 'GET'
+
+        prepared_request.method = method
+
 
 class Session(SessionRedirectMixin):
     """A Requests session.
 
     Provides cookie persistence, connection-pooling, and configuration.
 
     Basic Usage::
@@ -433,15 +439,16 @@
             hostname to the URL of the proxy.
         :param stream: (optional) whether to immediately download the response
             content. Defaults to ``False``.
         :param verify: (optional) whether the SSL cert will be verified.
             A CA_BUNDLE path can also be provided. Defaults to ``True``.
         :param cert: (optional) if String, path to ssl client cert file (.pem).
             If Tuple, ('cert', 'key') pair.
-        """
+        :rtype: requests.Response
+	"""
         # Create the Request.
         req = Request(
             method = method.upper(),
             url = url,
             headers = headers,
             files = files,
             data = data or {},
@@ -546,30 +553,32 @@
         kwargs.setdefault('stream', self.stream)
         kwargs.setdefault('verify', self.verify)
         kwargs.setdefault('cert', self.cert)
         kwargs.setdefault('proxies', self.proxies)
 
         # It's possible that users might accidentally send a Request object.
         # Guard against that specific failure case.
-        if not isinstance(request, PreparedRequest):
+        if isinstance(request, Request):
             raise ValueError('You can only send PreparedRequests.')
 
-        checked_urls = set()
-        while request.url in self.redirect_cache:
-            checked_urls.add(request.url)
-            new_url = self.redirect_cache.get(request.url)
-            if new_url in checked_urls:
-                break
-            request.url = new_url
-
         # Set up variables needed for resolve_redirects and dispatching of hooks
         allow_redirects = kwargs.pop('allow_redirects', True)
         stream = kwargs.get('stream')
         hooks = request.hooks
 
+        # Resolve URL in redirect cache, if available.
+        if allow_redirects:
+            checked_urls = set()
+            while request.url in self.redirect_cache:
+                checked_urls.add(request.url)
+                new_url = self.redirect_cache.get(request.url)
+                if new_url in checked_urls:
+                    break
+                request.url = new_url
+
         # Get the appropriate adapter to use
         adapter = self.get_adapter(url=request.url)
 
         # Start time (approximately) of the request
         start = datetime.utcnow()
 
         # Send the request
```

### Comparing `requests-2.9.1/requests/status_codes.py` & `requests-2.9.2/requests/status_codes.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     412: ('precondition_failed', 'precondition'),
     413: ('request_entity_too_large',),
     414: ('request_uri_too_large',),
     415: ('unsupported_media_type', 'unsupported_media', 'media_type'),
     416: ('requested_range_not_satisfiable', 'requested_range', 'range_not_satisfiable'),
     417: ('expectation_failed',),
     418: ('im_a_teapot', 'teapot', 'i_am_a_teapot'),
+    421: ('misdirected_request',),
     422: ('unprocessable_entity', 'unprocessable'),
     423: ('locked',),
     424: ('failed_dependency', 'dependency'),
     425: ('unordered_collection', 'unordered'),
     426: ('upgrade_required', 'upgrade'),
     428: ('precondition_required', 'precondition'),
     429: ('too_many_requests', 'too_many'),
```

### Comparing `requests-2.9.1/requests/structures.py` & `requests-2.9.2/requests/structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 Data structures that power Requests.
 
 """
 
 import collections
 
+from .compat import OrderedDict
+
 
 class CaseInsensitiveDict(collections.MutableMapping):
     """
     A case-insensitive ``dict``-like object.
 
     Implements all methods and operations of
     ``collections.MutableMapping`` as well as dict's ``copy``. Also
@@ -36,15 +38,15 @@
 
     If the constructor, ``.update``, or equality comparison
     operations are given keys that have equal ``.lower()``s, the
     behavior is undefined.
 
     """
     def __init__(self, data=None, **kwargs):
-        self._store = dict()
+        self._store = OrderedDict()
         if data is None:
             data = {}
         self.update(data, **kwargs)
 
     def __setitem__(self, key, value):
         # Use the lowercased key for lookups, but store the actual
         # key alongside the value.
```

### Comparing `requests-2.9.1/requests/utils.py` & `requests-2.9.2/requests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 """
 
 import cgi
 import codecs
 import collections
 import io
 import os
-import platform
 import re
-import sys
 import socket
 import struct
 import warnings
 
 from . import __version__
 from . import certs
 from .compat import parse_http_list as _parse_list_header
@@ -79,15 +77,22 @@
                     "flag in the mode). This may lead to an incorrect "
                     "content-length. In Requests 3.0, support will be removed "
                     "for files in text mode."),
                     FileModeWarning
                 )
 
     if hasattr(o, 'tell'):
-        current_position = o.tell()
+        try:
+            current_position = o.tell()
+        except (OSError, IOError):
+            # This can happen in some weird situations, such as when the file
+            # is actually a special file descriptor like stdin. In this
+            # instance, we don't know what the length is, so set it to zero and
+            # let requests chunk it instead.
+            current_position = total_length
 
     return max(0, total_length - current_position)
 
 
 def get_netrc_auth(url, raise_errors=False):
     """Returns the Requests tuple auth for a given url from netrc."""
 
@@ -553,34 +558,40 @@
         bypass = False
 
     if bypass:
         return True
 
     return False
 
+
 def get_environ_proxies(url):
     """Return a dict of environment proxies."""
     if should_bypass_proxies(url):
         return {}
     else:
         return getproxies()
 
+
 def select_proxy(url, proxies):
     """Select a proxy for the url, if applicable.
 
     :param url: The url being for the request
     :param proxies: A dictionary of schemes or schemes and hosts to proxy URLs
     """
     proxies = proxies or {}
     urlparts = urlparse(url)
-    proxy = proxies.get(urlparts.scheme+'://'+urlparts.hostname)
+    if urlparts.hostname is None:
+        proxy = None
+    else:
+        proxy = proxies.get(urlparts.scheme+'://'+urlparts.hostname)
     if proxy is None:
         proxy = proxies.get(urlparts.scheme)
     return proxy
 
+
 def default_user_agent(name="python-requests"):
     """Return a string representing the default user agent."""
     return '%s/%s' % (name, __version__)
 
 
 def default_headers():
     return CaseInsensitiveDict({
@@ -596,29 +607,27 @@
 
     i.e. Link: <http:/.../front.jpeg>; rel=front; type="image/jpeg",<http://.../back.jpeg>; rel=back;type="image/jpeg"
 
     """
 
     links = []
 
-    replace_chars = " '\""
+    replace_chars = ' \'"'
 
-    for val in re.split(", *<", value):
+    for val in re.split(', *<', value):
         try:
-            url, params = val.split(";", 1)
+            url, params = val.split(';', 1)
         except ValueError:
             url, params = val, ''
 
-        link = {}
-
-        link["url"] = url.strip("<> '\"")
+        link = {'url': url.strip('<> \'"')}
 
-        for param in params.split(";"):
+        for param in params.split(';'):
             try:
-                key, value = param.split("=")
+                key, value = param.split('=')
             except ValueError:
                 break
 
             link[key.strip(replace_chars)] = value.strip(replace_chars)
 
         links.append(link)
 
@@ -657,16 +666,16 @@
         if sample[1:] == _null3:
             return 'utf-32-le'
         # Did not detect a valid UTF-32 ascii-range character
     return None
 
 
 def prepend_scheme_if_needed(url, new_scheme):
-    '''Given a URL that may or may not have a scheme, prepend the given scheme.
-    Does not replace a present scheme with the one provided as an argument.'''
+    """Given a URL that may or may not have a scheme, prepend the given scheme.
+    Does not replace a present scheme with the one provided as an argument."""
     scheme, netloc, path, params, query, fragment = urlparse(url, new_scheme)
 
     # urlparse is a finicky beast, and sometimes decides that there isn't a
     # netloc present. Assume that it's being over-cautious, and switch netloc
     # and path if urlparse decided there was no netloc.
     if not netloc:
         netloc, path = path, netloc
@@ -689,16 +698,14 @@
 
 def to_native_string(string, encoding='ascii'):
     """
     Given a string object, regardless of type, returns a representation of that
     string in the native string type, encoding and decoding where necessary.
     This assumes ASCII unless told otherwise.
     """
-    out = None
-
     if isinstance(string, builtin_str):
         out = string
     else:
         if is_py2:
             out = string.encode(encoding)
         else:
             out = string.decode(encoding)
```

### Comparing `requests-2.9.1/requests.egg-info/PKG-INFO` & `requests-2.9.2/requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,92 +1,103 @@
 Metadata-Version: 1.1
 Name: requests
-Version: 2.9.1
+Version: 2.9.2
 Summary: Python HTTP for Humans.
 Home-page: http://python-requests.org
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: Apache 2.0
 Description: Requests: HTTP for Humans
         =========================
         
         .. image:: https://img.shields.io/pypi/v/requests.svg
             :target: https://pypi.python.org/pypi/requests
         
         .. image:: https://img.shields.io/pypi/dm/requests.svg
                 :target: https://pypi.python.org/pypi/requests
         
+        Requests is the only *Non-GMO* HTTP library for Python, safe for human
+        consumption.
         
+        **Warning:** Recreational use of other HTTP libraries may result in dangerous side-effects,
+        including: security vulnerabilities, verbose code, reinventing the wheel,
+        constantly reading documentation, depression, headaches, or even death.
         
-        
-        Requests is an Apache2 Licensed HTTP library, written in Python, for human
-        beings.
-        
-        Most existing Python modules for sending HTTP requests are extremely
-        verbose and cumbersome. Python's builtin urllib2 module provides most of
-        the HTTP capabilities you should need, but the api is thoroughly broken.
-        It requires an enormous amount of work (even method overrides) to
-        perform the simplest of tasks.
-        
-        Things shouldn't be this way. Not in Python.
+        Behold, the power of Requests:
         
         .. code-block:: python
         
-            >>> r = requests.get('https://api.github.com', auth=('user', 'pass'))
+            >>> r = requests.get('https://api.github.com/user', auth=('user', 'pass'))
             >>> r.status_code
-            204
+            200
             >>> r.headers['content-type']
-            'application/json'
+            'application/json; charset=utf8'
+            >>> r.encoding
+            'utf-8'
             >>> r.text
-            ...
-        
-        See `the same code, without Requests <https://gist.github.com/973705>`_.
-        
-        Requests allow you to send HTTP/1.1 requests. You can add headers, form data,
-        multipart files, and parameters with simple Python dictionaries, and access the
-        response data in the same way. It's powered by httplib and `urllib3
-        <https://github.com/shazow/urllib3>`_, but it does all the hard work and crazy
-        hacks for you.
+            u'{"type":"User"...'
+            >>> r.json()
+            {u'disk_usage': 368627, u'private_gists': 484, ...}
+        
+        See `the similar code, sans Requests <https://gist.github.com/973705>`_.
+        
+        Requests allows you to send *organic, grass-fed* HTTP/1.1 requests, without the
+        need for manual labor. There's no need to manually add query strings to your
+        URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling
+        are 100% automatic, powered by `urllib3 <https://github.com/shazow/urllib3>`_,
+        which is embedded within Requests.
+        
+        Besides, all the cool kids are doing it. Requests is one of the most
+        downloaded Python packages of all time, pulling in over 7,000,000 downloads
+        every month. You don't want to be left out!
         
+        Feature Support
+        ---------------
         
-        Features
-        --------
+        Requests is ready for today's web.
         
         - International Domains and URLs
         - Keep-Alive & Connection Pooling
         - Sessions with Cookie Persistence
         - Browser-style SSL Verification
         - Basic/Digest Authentication
         - Elegant Key/Value Cookies
         - Automatic Decompression
+        - Automatic Content Decoding
         - Unicode Response Bodies
         - Multipart File Uploads
+        - HTTP(S) Proxy Support
         - Connection Timeouts
+        - Streaming Downloads
+        - ``.netrc`` Support
+        - Chunked Requests
         - Thread-safety
-        - HTTP(S) proxy support
         
+        Requests supports Python 2.6 — 3.5, and runs great on PyPy.
         
         Installation
         ------------
         
         To install Requests, simply:
         
         .. code-block:: bash
         
             $ pip install requests
+            ✨🍰✨
         
+        Satisfaction, guaranteed.
         
         Documentation
         -------------
         
-        Documentation is available at http://docs.python-requests.org/.
+        Fantastic documentation is available at http://docs.python-requests.org/, for a limited time only.
         
         
-        Contribute
-        ----------
+        How to Contribute
+        -----------------
         
         #. Check for open issues or open a fresh issue to start a discussion around a feature idea or a bug. There is a `Contributor Friendly`_ tag for issues that should be ideal for people who are not very familiar with the codebase yet.
         #. Fork `the repository`_ on GitHub to start making your changes to the **master** branch (or branch off of it).
         #. Write a test which shows that the bug was fixed or that the feature works as expected.
         #. Send a pull request and bug the maintainer until it gets merged and published. :) Make sure to add yourself to AUTHORS_.
         
         .. _`the repository`: http://github.com/kennethreitz/requests
@@ -95,14 +106,29 @@
         
         
         .. :changelog:
         
         Release History
         ---------------
         
+        2.9.2 (04-29-2016)
+        ++++++++++++++++++
+        
+        **Improvements**
+        
+        - Change built-in CaseInsensitiveDict (used for headers) to use OrderedDict
+          as its underlying datastore.
+        
+        **Bugfixes**
+        
+        - Don't use redirect_cache if allow_redirects=False
+        - When passed objects that throw exceptions from ``tell()``, send them via
+          chunked transfer encoding instead of failing.
+        - Raise a ProxyError for proxy related connection issues.
+        
         2.9.1 (2015-12-21)
         ++++++++++++++++++
         
         **Bugfixes**
         
         - Resolve regression introduced in 2.9.0 that made it impossible to send binary
           strings as bodies in Python 3.
@@ -1227,12 +1253,15 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `requests-2.9.1/requests.egg-info/SOURCES.txt` & `requests-2.9.2/requests.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 NOTICE
 README.rst
 requirements.txt
-setup.cfg
 setup.py
-test_requests.py
 requests/__init__.py
 requests/adapters.py
 requests/api.py
 requests/auth.py
 requests/cacert.pem
 requests/certs.py
 requests/compat.py
```

### Comparing `requests-2.9.1/setup.py` & `requests-2.9.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,36 @@
 
 import os
 import re
 import sys
 
 from codecs import open
 
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
+from setuptools import setup
+from setuptools.command.test import test as TestCommand
+
+
+class PyTest(TestCommand):
+    user_options = [('pytest-args=', 'a', "Arguments to pass into py.test")]
+
+    def initialize_options(self):
+        TestCommand.initialize_options(self)
+        self.pytest_args = []
+
+    def finalize_options(self):
+        TestCommand.finalize_options(self)
+        self.test_args = []
+        self.test_suite = True
+
+    def run_tests(self):
+        import pytest
+
+        errno = pytest.main(self.pytest_args)
+        sys.exit(errno)
+
 
 if sys.argv[-1] == 'publish':
     os.system('python setup.py sdist upload')
     sys.exit()
 
 packages = [
     'requests',
@@ -23,16 +41,16 @@
     'requests.packages.urllib3.packages',
     'requests.packages.urllib3.contrib',
     'requests.packages.urllib3.util',
     'requests.packages.urllib3.packages.ssl_match_hostname',
 ]
 
 requires = []
+test_requirements = ['pytest>=2.8.0', 'pytest-httpbin==0.0.7', 'pytest-cov']
 
-version = ''
 with open('requests/__init__.py', 'r') as fd:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
 if not version:
     raise RuntimeError('Cannot find version information')
 
@@ -58,17 +76,22 @@
     zip_safe=False,
     classifiers=(
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
+        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
     ),
+    cmdclass={'test': PyTest},
+    tests_require=test_requirements,
     extras_require={
         'security': ['pyOpenSSL>=0.13', 'ndg-httpsclient', 'pyasn1'],
     },
 )
```

