# Comparing `tmp/zillionare-omicron-2.0.0a64.tar.gz` & `tmp/zillionare-omicron-2.0.0a65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare-omicron-2.0.0a64.tar", max compression
+gzip compressed data, was "zillionare-omicron-2.0.0a65.tar", max compression
```

## Comparing `zillionare-omicron-2.0.0a64.tar` & `zillionare-omicron-2.0.0a65.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0      112 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/AUTHORS.md
--rw-r--r--   0        0        0     1561 2022-09-19 02:47:00.722663 zillionare-omicron-2.0.0a64/HISTORY.md
--rw-r--r--   0        0        0     1068 2022-05-19 11:28:00.022177 zillionare-omicron-2.0.0a64/LICENSE
--rw-r--r--   0        0        0     1880 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/README.md
--rw-r--r--   0        0        0   503846 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a64/docs/_static/Omicron_Windows10.docx
--rw-r--r--   0        0        0     5620 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a64/docs/_static/jetbrains-variant-3.svg
--rw-r--r--   0        0        0       84 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/docs/api/dal/flux.md
--rw-r--r--   0        0        0      110 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/docs/api/dal/influxclient.md
--rw-r--r--   0        0        0      189 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/docs/api/dal/serialize.md
--rw-r--r--   0        0        0     5772 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a64/docs/api/metrics.md
--rw-r--r--   0        0        0      203 2022-11-08 08:08:31.311437 zillionare-omicron-2.0.0a64/docs/api/omicron.md
--rw-r--r--   0        0        0       73 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a64/docs/api/plotting.md
--rw-r--r--   0        0        0       68 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a64/docs/api/security.md
--rw-r--r--   0        0        0       65 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/docs/api/stock.md
--rw-r--r--   0        0        0       58 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/docs/api/talib.md
--rw-r--r--   0        0        0       57 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a64/docs/api/timeframe.md
--rw-r--r--   0        0        0       66 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a64/docs/api/triggers.md
--rw-r--r--   0        0        0      907 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a64/docs/css/extra.css
--rw-r--r--   0        0        0     1778 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a64/docs/developer.md
--rw-r--r--   0        0        0       43 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a64/docs/history.md
--rw-r--r--   0        0        0       42 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a64/docs/index.md
--rw-r--r--   0        0        0     1820 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a64/docs/installation.md
--rw-r--r--   0        0        0     9823 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a64/docs/usage.md
--rw-r--r--   0        0        0      920 2022-09-25 07:32:43.784350 zillionare-omicron-2.0.0a64/omicron/__init__.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a64/omicron/config/__init__.py
--rw-r--r--   0        0        0    56389 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a64/omicron/config/calendar.json
--rw-r--r--   0        0        0      441 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a64/omicron/config/defaults.yaml
--rw-r--r--   0        0        0      378 2022-10-02 07:50:29.380175 zillionare-omicron-2.0.0a64/omicron/config/dev.yaml
--rw-r--r--   0        0        0     1334 2022-09-07 09:45:22.201476 zillionare-omicron-2.0.0a64/omicron/config/schema.py
--rw-r--r--   0        0        0      816 2022-05-19 11:28:00.030177 zillionare-omicron-2.0.0a64/omicron/config/sql/v0.6.sql
--rw-r--r--   0        0        0     2785 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a64/omicron/config/sql/v1.0.sql
--rw-r--r--   0        0        0       46 2022-05-19 11:28:00.030177 zillionare-omicron-2.0.0a64/omicron/core/__init__.py
--rw-r--r--   0        0        0      140 2022-08-04 07:38:19.097441 zillionare-omicron-2.0.0a64/omicron/core/constants.py
--rw-r--r--   0        0        0     1095 2022-09-07 09:45:22.201476 zillionare-omicron-2.0.0a64/omicron/core/errors.py
--rw-r--r--   0        0        0       46 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a64/omicron/core/events.py
--rw-r--r--   0        0        0     6517 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a64/omicron/core/triggers.py
--rw-r--r--   0        0        0       71 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a64/omicron/dal/__init__.py
--rw-r--r--   0        0        0     3215 2022-12-08 01:58:13.329503 zillionare-omicron-2.0.0a64/omicron/dal/cache.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a64/omicron/dal/influx/__init__.py
--rw-r--r--   0        0        0      370 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a64/omicron/dal/influx/errors.py
--rw-r--r--   0        0        0      996 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a64/omicron/dal/influx/escape.py
--rw-r--r--   0        0        0    19097 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a64/omicron/dal/influx/flux.py
--rw-r--r--   0        0        0    16805 2022-09-24 09:12:02.824758 zillionare-omicron-2.0.0a64/omicron/dal/influx/influxclient.py
--rw-r--r--   0        0        0    27708 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a64/omicron/dal/influx/serialize.py
--rw-r--r--   0        0        0       78 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a64/omicron/extensions/__init__.py
--rw-r--r--   0        0        0      656 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a64/omicron/extensions/decimals.py
--rw-r--r--   0        0        0    15929 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/omicron/extensions/np.py
--rw-r--r--   0        0        0      492 2022-10-14 08:08:29.548960 zillionare-omicron-2.0.0a64/omicron/models/__init__.py
--rw-r--r--   0        0        0     7867 2022-12-14 05:13:08.492827 zillionare-omicron-2.0.0a64/omicron/models/board.py
--rw-r--r--   0        0        0    26127 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/omicron/models/security.py
--rw-r--r--   0        0        0    53664 2022-12-14 05:46:42.382228 zillionare-omicron-2.0.0a64/omicron/models/stock.py
--rw-r--r--   0        0        0    41959 2022-09-26 02:36:43.062543 zillionare-omicron-2.0.0a64/omicron/models/timeframe.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a64/omicron/notify/__init__.py
--rw-r--r--   0        0        0     5472 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a64/omicron/notify/dingtalk.py
--rw-r--r--   0        0        0     6006 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/omicron/notify/mail.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.770131 zillionare-omicron-2.0.0a64/omicron/notify/tts.py
--rw-r--r--   0        0        0        0 2022-09-19 02:47:00.734664 zillionare-omicron-2.0.0a64/omicron/plotting/__init__.py
--rw-r--r--   0        0        0    14071 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/omicron/plotting/candlestick.py
--rw-r--r--   0        0        0      114 2022-09-19 02:47:00.734664 zillionare-omicron-2.0.0a64/omicron/talib/__init__.py
--rw-r--r--   0        0        0     9958 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/omicron/talib/core.py
--rw-r--r--   0        0        0    23141 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a64/omicron/talib/morph.py
--rwxr-xr-x   0        0        0     3297 2022-12-14 09:52:15.663297 zillionare-omicron-2.0.0a64/pyproject.toml
--rw-r--r--   0        0        0     5556 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a64/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.782132 zillionare-omicron-2.0.0a64/tests/core/__init__.py
--rw-r--r--   0        0        0      297 2022-09-07 09:45:22.237476 zillionare-omicron-2.0.0a64/tests/core/test_errors.py
--rw-r--r--   0        0        0     3615 2022-05-19 11:30:57.782132 zillionare-omicron-2.0.0a64/tests/core/test_triggers.py
--rw-r--r--   0        0        0     1024 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/core/test_types.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/dal/__init__.py
--rw-r--r--   0        0        0      622 2022-06-25 11:03:39.472127 zillionare-omicron-2.0.0a64/tests/dal/influx/__init__.py
--rw-r--r--   0        0        0     1177 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/dal/influx/test_escape.py
--rw-r--r--   0        0        0     8531 2022-06-25 11:03:39.472127 zillionare-omicron-2.0.0a64/tests/dal/influx/test_flux.py
--rw-r--r--   0        0        0    14284 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a64/tests/dal/influx/test_influxclient.py
--rw-r--r--   0        0        0    15710 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a64/tests/dal/influx/test_serialize.py
--rw-r--r--   0        0        0     1253 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.15m.csv
--rw-r--r--   0        0        0      118 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.1M.csv
--rw-r--r--   0        0        0      188 2022-09-07 09:45:22.253477 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.1d.csv
--rw-r--r--   0        0        0    22206 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.1m.csv
--rw-r--r--   0        0        0      115 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.1w.csv
--rw-r--r--   0        0        0      654 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.30m.csv
--rw-r--r--   0        0        0     3633 2022-09-07 09:45:22.257477 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.5m.csv
--rw-r--r--   0        0        0      352 2022-09-07 09:45:22.257477 zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.60m.csv
--rw-r--r--   0        0        0     8089 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.1d.csv
--rw-r--r--   0        0        0    22419 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.1m.csv
--rw-r--r--   0        0        0     7166 2022-09-07 09:45:22.269477 zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.1w.csv
--rw-r--r--   0        0        0     8096 2022-09-07 09:45:22.281477 zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.30m.csv
--rw-r--r--   0        0        0     7585 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.1d.csv
--rw-r--r--   0        0        0    20344 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.1m.csv
--rw-r--r--   0        0        0     6443 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.1w.csv
--rw-r--r--   0        0        0     7688 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.30m.csv
--rw-r--r--   0        0        0     1145 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a64/tests/data/README.md
--rw-r--r--   0        0        0     2191 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a64/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2022-05-19 11:30:57.794132 zillionare-omicron-2.0.0a64/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      713 2022-05-19 11:30:57.794132 zillionare-omicron-2.0.0a64/tests/data/limits.csv
--rw-r--r--   0        0        0   164066 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a64/tests/data/stock_bars_flux_query.txt
--rw-r--r--   0        0        0     6315 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a64/tests/data/test.jpg
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a64/tests/extensions/__init__.py
--rw-r--r--   0        0        0      594 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a64/tests/extensions/test_decimals.py
--rw-r--r--   0        0        0     9864 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a64/tests/extensions/test_np.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a64/tests/models/__init__.py
--rw-r--r--   0        0        0     6802 2022-12-14 09:53:29.108769 zillionare-omicron-2.0.0a64/tests/models/test_board.py
--rw-r--r--   0        0        0    11161 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a64/tests/models/test_security.py
--rw-r--r--   0        0        0    68822 2022-11-08 08:08:31.311437 zillionare-omicron-2.0.0a64/tests/models/test_stock.py
--rw-r--r--   0        0        0    36351 2022-09-23 11:09:33.778515 zillionare-omicron-2.0.0a64/tests/models/test_timeframe.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.802132 zillionare-omicron-2.0.0a64/tests/notify/__init__.py
--rw-r--r--   0        0        0      823 2022-09-07 09:45:22.293477 zillionare-omicron-2.0.0a64/tests/notify/test_dingtalk.py
--rw-r--r--   0        0        0     2686 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a64/tests/notify/test_mail.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a64/tests/performance/influx/__init__.py
--rw-r--r--   0        0        0     3317 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a64/tests/performance/influx/end2end.py
--rw-r--r--   0        0        0     4197 2022-06-25 11:03:39.476127 zillionare-omicron-2.0.0a64/tests/performance/influx/serialize.py
--rw-r--r--   0        0        0      294 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a64/tests/performance/readme.md
--rw-r--r--   0        0        0      406 2022-05-19 11:28:00.038178 zillionare-omicron-2.0.0a64/tests/pyrightconfig.json
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a64/tests/talib/__init__.py
--rw-r--r--   0        0        0     2917 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a64/tests/talib/test_core.py
--rw-r--r--   0        0        0    37991 2022-12-12 12:04:52.265182 zillionare-omicron-2.0.0a64/tests/talib/test_morph.py
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 zillionare-omicron-2.0.0a64/setup.py
--rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 zillionare-omicron-2.0.0a64/PKG-INFO
+-rw-r--r--   0        0        0      112 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/AUTHORS.md
+-rw-r--r--   0        0        0     1561 2022-09-19 02:47:00.722663 zillionare-omicron-2.0.0a65/HISTORY.md
+-rw-r--r--   0        0        0     1068 2022-05-19 11:28:00.022177 zillionare-omicron-2.0.0a65/LICENSE
+-rw-r--r--   0        0        0     1880 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/README.md
+-rw-r--r--   0        0        0   503846 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a65/docs/_static/Omicron_Windows10.docx
+-rw-r--r--   0        0        0     5620 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/_static/jetbrains-variant-3.svg
+-rw-r--r--   0        0        0       84 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/dal/flux.md
+-rw-r--r--   0        0        0      110 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/dal/influxclient.md
+-rw-r--r--   0        0        0      189 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/dal/serialize.md
+-rw-r--r--   0        0        0     5772 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a65/docs/api/metrics.md
+-rw-r--r--   0        0        0      203 2022-11-08 08:08:31.311437 zillionare-omicron-2.0.0a65/docs/api/omicron.md
+-rw-r--r--   0        0        0       73 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a65/docs/api/plotting.md
+-rw-r--r--   0        0        0       68 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a65/docs/api/security.md
+-rw-r--r--   0        0        0       65 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/stock.md
+-rw-r--r--   0        0        0       58 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/talib.md
+-rw-r--r--   0        0        0       57 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/timeframe.md
+-rw-r--r--   0        0        0       66 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/api/triggers.md
+-rw-r--r--   0        0        0      907 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/css/extra.css
+-rw-r--r--   0        0        0     1778 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a65/docs/developer.md
+-rw-r--r--   0        0        0       43 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/history.md
+-rw-r--r--   0        0        0       42 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/index.md
+-rw-r--r--   0        0        0     1820 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a65/docs/installation.md
+-rw-r--r--   0        0        0     9823 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a65/docs/usage.md
+-rw-r--r--   0        0        0      920 2022-09-25 07:32:43.784350 zillionare-omicron-2.0.0a65/omicron/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a65/omicron/config/__init__.py
+-rw-r--r--   0        0        0    56389 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a65/omicron/config/calendar.json
+-rw-r--r--   0        0        0      441 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a65/omicron/config/defaults.yaml
+-rw-r--r--   0        0        0      378 2022-10-02 07:50:29.380175 zillionare-omicron-2.0.0a65/omicron/config/dev.yaml
+-rw-r--r--   0        0        0     1334 2022-09-07 09:45:22.201476 zillionare-omicron-2.0.0a65/omicron/config/schema.py
+-rw-r--r--   0        0        0      816 2022-05-19 11:28:00.030177 zillionare-omicron-2.0.0a65/omicron/config/sql/v0.6.sql
+-rw-r--r--   0        0        0     2785 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a65/omicron/config/sql/v1.0.sql
+-rw-r--r--   0        0        0       46 2022-05-19 11:28:00.030177 zillionare-omicron-2.0.0a65/omicron/core/__init__.py
+-rw-r--r--   0        0        0      140 2022-08-04 07:38:19.097441 zillionare-omicron-2.0.0a65/omicron/core/constants.py
+-rw-r--r--   0        0        0     1095 2022-09-07 09:45:22.201476 zillionare-omicron-2.0.0a65/omicron/core/errors.py
+-rw-r--r--   0        0        0       46 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/core/events.py
+-rw-r--r--   0        0        0     6517 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/core/triggers.py
+-rw-r--r--   0        0        0       71 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/dal/__init__.py
+-rw-r--r--   0        0        0     3215 2022-12-08 01:58:13.329503 zillionare-omicron-2.0.0a65/omicron/dal/cache.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/dal/influx/__init__.py
+-rw-r--r--   0        0        0      370 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/dal/influx/errors.py
+-rw-r--r--   0        0        0      996 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/dal/influx/escape.py
+-rw-r--r--   0        0        0    19097 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/dal/influx/flux.py
+-rw-r--r--   0        0        0    16805 2022-09-24 09:12:02.824758 zillionare-omicron-2.0.0a65/omicron/dal/influx/influxclient.py
+-rw-r--r--   0        0        0    27708 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/dal/influx/serialize.py
+-rw-r--r--   0        0        0       78 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a65/omicron/extensions/__init__.py
+-rw-r--r--   0        0        0      656 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a65/omicron/extensions/decimals.py
+-rw-r--r--   0        0        0    15929 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/extensions/np.py
+-rw-r--r--   0        0        0      492 2022-10-14 08:08:29.548960 zillionare-omicron-2.0.0a65/omicron/models/__init__.py
+-rw-r--r--   0        0        0     7867 2022-12-14 05:13:08.492827 zillionare-omicron-2.0.0a65/omicron/models/board.py
+-rw-r--r--   0        0        0    26127 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/models/security.py
+-rw-r--r--   0        0        0    53741 2022-12-16 02:06:19.061417 zillionare-omicron-2.0.0a65/omicron/models/stock.py
+-rw-r--r--   0        0        0    41959 2022-09-26 02:36:43.062543 zillionare-omicron-2.0.0a65/omicron/models/timeframe.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a65/omicron/notify/__init__.py
+-rw-r--r--   0        0        0     5472 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a65/omicron/notify/dingtalk.py
+-rw-r--r--   0        0        0     6006 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/notify/mail.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.770131 zillionare-omicron-2.0.0a65/omicron/notify/tts.py
+-rw-r--r--   0        0        0        0 2022-09-19 02:47:00.734664 zillionare-omicron-2.0.0a65/omicron/plotting/__init__.py
+-rw-r--r--   0        0        0    14071 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/plotting/candlestick.py
+-rw-r--r--   0        0        0      114 2022-09-19 02:47:00.734664 zillionare-omicron-2.0.0a65/omicron/talib/__init__.py
+-rw-r--r--   0        0        0     9958 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/talib/core.py
+-rw-r--r--   0        0        0    23141 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/talib/morph.py
+-rwxr-xr-x   0        0        0     3297 2022-12-16 02:17:43.823747 zillionare-omicron-2.0.0a65/pyproject.toml
+-rw-r--r--   0        0        0     5556 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a65/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.782132 zillionare-omicron-2.0.0a65/tests/core/__init__.py
+-rw-r--r--   0        0        0      297 2022-09-07 09:45:22.237476 zillionare-omicron-2.0.0a65/tests/core/test_errors.py
+-rw-r--r--   0        0        0     3615 2022-05-19 11:30:57.782132 zillionare-omicron-2.0.0a65/tests/core/test_triggers.py
+-rw-r--r--   0        0        0     1024 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/core/test_types.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/dal/__init__.py
+-rw-r--r--   0        0        0      622 2022-06-25 11:03:39.472127 zillionare-omicron-2.0.0a65/tests/dal/influx/__init__.py
+-rw-r--r--   0        0        0     1177 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/dal/influx/test_escape.py
+-rw-r--r--   0        0        0     8531 2022-06-25 11:03:39.472127 zillionare-omicron-2.0.0a65/tests/dal/influx/test_flux.py
+-rw-r--r--   0        0        0    14284 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a65/tests/dal/influx/test_influxclient.py
+-rw-r--r--   0        0        0    15710 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a65/tests/dal/influx/test_serialize.py
+-rw-r--r--   0        0        0     1253 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.15m.csv
+-rw-r--r--   0        0        0      118 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1M.csv
+-rw-r--r--   0        0        0      188 2022-09-07 09:45:22.253477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1d.csv
+-rw-r--r--   0        0        0    22206 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1m.csv
+-rw-r--r--   0        0        0      115 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1w.csv
+-rw-r--r--   0        0        0      654 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.30m.csv
+-rw-r--r--   0        0        0     3633 2022-09-07 09:45:22.257477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.5m.csv
+-rw-r--r--   0        0        0      352 2022-09-07 09:45:22.257477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.60m.csv
+-rw-r--r--   0        0        0     8089 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1d.csv
+-rw-r--r--   0        0        0    22419 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1m.csv
+-rw-r--r--   0        0        0     7166 2022-09-07 09:45:22.269477 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1w.csv
+-rw-r--r--   0        0        0     8096 2022-09-07 09:45:22.281477 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.30m.csv
+-rw-r--r--   0        0        0     7585 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1d.csv
+-rw-r--r--   0        0        0    20344 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1m.csv
+-rw-r--r--   0        0        0     6443 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1w.csv
+-rw-r--r--   0        0        0     7688 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.30m.csv
+-rw-r--r--   0        0        0     1145 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a65/tests/data/README.md
+-rw-r--r--   0        0        0     2191 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a65/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2022-05-19 11:30:57.794132 zillionare-omicron-2.0.0a65/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      713 2022-05-19 11:30:57.794132 zillionare-omicron-2.0.0a65/tests/data/limits.csv
+-rw-r--r--   0        0        0   164066 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/data/stock_bars_flux_query.txt
+-rw-r--r--   0        0        0     6315 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/data/test.jpg
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/extensions/__init__.py
+-rw-r--r--   0        0        0      594 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/extensions/test_decimals.py
+-rw-r--r--   0        0        0     9864 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a65/tests/extensions/test_np.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/models/__init__.py
+-rw-r--r--   0        0        0     6802 2022-12-14 09:53:29.108769 zillionare-omicron-2.0.0a65/tests/models/test_board.py
+-rw-r--r--   0        0        0    11161 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a65/tests/models/test_security.py
+-rw-r--r--   0        0        0    68822 2022-11-08 08:08:31.311437 zillionare-omicron-2.0.0a65/tests/models/test_stock.py
+-rw-r--r--   0        0        0    36351 2022-09-23 11:09:33.778515 zillionare-omicron-2.0.0a65/tests/models/test_timeframe.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.802132 zillionare-omicron-2.0.0a65/tests/notify/__init__.py
+-rw-r--r--   0        0        0      823 2022-09-07 09:45:22.293477 zillionare-omicron-2.0.0a65/tests/notify/test_dingtalk.py
+-rw-r--r--   0        0        0     2686 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a65/tests/notify/test_mail.py
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a65/tests/performance/influx/__init__.py
+-rw-r--r--   0        0        0     3317 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a65/tests/performance/influx/end2end.py
+-rw-r--r--   0        0        0     4197 2022-06-25 11:03:39.476127 zillionare-omicron-2.0.0a65/tests/performance/influx/serialize.py
+-rw-r--r--   0        0        0      294 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a65/tests/performance/readme.md
+-rw-r--r--   0        0        0      406 2022-05-19 11:28:00.038178 zillionare-omicron-2.0.0a65/tests/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a65/tests/talib/__init__.py
+-rw-r--r--   0        0        0     2917 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a65/tests/talib/test_core.py
+-rw-r--r--   0        0        0    37991 2022-12-12 12:04:52.265182 zillionare-omicron-2.0.0a65/tests/talib/test_morph.py
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 zillionare-omicron-2.0.0a65/setup.py
+-rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 zillionare-omicron-2.0.0a65/PKG-INFO
```

### Comparing `zillionare-omicron-2.0.0a64/HISTORY.md` & `zillionare-omicron-2.0.0a65/HISTORY.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/LICENSE` & `zillionare-omicron-2.0.0a65/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/README.md` & `zillionare-omicron-2.0.0a65/README.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/_static/Omicron_Windows10.docx` & `zillionare-omicron-2.0.0a65/docs/_static/Omicron_Windows10.docx`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/_static/jetbrains-variant-3.svg` & `zillionare-omicron-2.0.0a65/docs/_static/jetbrains-variant-3.svg`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/api/metrics.md` & `zillionare-omicron-2.0.0a65/docs/api/metrics.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/css/extra.css` & `zillionare-omicron-2.0.0a65/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/developer.md` & `zillionare-omicron-2.0.0a65/docs/developer.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/installation.md` & `zillionare-omicron-2.0.0a65/docs/installation.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/docs/usage.md` & `zillionare-omicron-2.0.0a65/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/__init__.py` & `zillionare-omicron-2.0.0a65/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/config/calendar.json` & `zillionare-omicron-2.0.0a65/omicron/config/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/config/schema.py` & `zillionare-omicron-2.0.0a65/omicron/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/config/sql/v0.6.sql` & `zillionare-omicron-2.0.0a65/omicron/config/sql/v0.6.sql`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/config/sql/v1.0.sql` & `zillionare-omicron-2.0.0a65/omicron/config/sql/v1.0.sql`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/core/errors.py` & `zillionare-omicron-2.0.0a65/omicron/core/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/core/triggers.py` & `zillionare-omicron-2.0.0a65/omicron/core/triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/dal/cache.py` & `zillionare-omicron-2.0.0a65/omicron/dal/cache.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/dal/influx/escape.py` & `zillionare-omicron-2.0.0a65/omicron/dal/influx/escape.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/dal/influx/flux.py` & `zillionare-omicron-2.0.0a65/omicron/dal/influx/flux.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/dal/influx/influxclient.py` & `zillionare-omicron-2.0.0a65/omicron/dal/influx/influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/dal/influx/serialize.py` & `zillionare-omicron-2.0.0a65/omicron/dal/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/extensions/decimals.py` & `zillionare-omicron-2.0.0a65/omicron/extensions/decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/extensions/np.py` & `zillionare-omicron-2.0.0a65/omicron/extensions/np.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/models/board.py` & `zillionare-omicron-2.0.0a65/omicron/models/board.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/models/security.py` & `zillionare-omicron-2.0.0a65/omicron/models/security.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/models/stock.py` & `zillionare-omicron-2.0.0a65/omicron/models/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,39 +360,41 @@
             frame_type : 行情数据的帧类型
             start : 起始时间
             end : 结束时间,如果为None，则表明取到当前时间。
             fq : 是否对行情数据执行前复权操作
             unclosed : 是否包含未收盘的数据
         """
         now = datetime.datetime.now()
+
         if frame_type in tf.day_level_frames:
             end = end or now.date()
             if unclosed and tf.day_shift(end, 0) == now.date():
                 part2 = await cls._get_cached_bars_n(code, 1, frame_type)
             else:
                 part2 = np.array([], dtype=bars_dtype)
 
             # get rest from persisted
             part1 = await cls._get_persisted_bars_in_range(code, frame_type, start, end)
             bars = np.concatenate((part1, part2))
         else:
             end = end or now
             closed_end = tf.floor(end, frame_type)
-            ff = tf.first_min_frame(now, frame_type)
-            if end < ff or tf.day_shift(end, 0) < now.date():
+            ff_min1 = tf.first_min_frame(now, FrameType.MIN1)
+            if tf.day_shift(end, 0) < now.date() or end < ff_min1:
                 part1 = await cls._get_persisted_bars_in_range(
                     code, frame_type, start, end
                 )
                 part2 = np.array([], dtype=bars_dtype)
-            elif start >= ff:  # all in cache
+            elif start >= ff_min1:  # all in cache
                 part1 = np.array([], dtype=bars_dtype)
                 n = tf.count_frames(start, closed_end, frame_type) + 1
                 part2 = await cls._get_cached_bars_n(code, n, frame_type, end)
                 part2 = part2[part2["frame"] >= start]
             else:  # in both cache and persisted
+                ff = tf.first_min_frame(now, frame_type)
                 part1 = await cls._get_persisted_bars_in_range(
                     code, frame_type, start, ff
                 )
                 n = tf.count_frames(ff, closed_end, frame_type) + 1
                 part2 = await cls._get_cached_bars_n(code, n, frame_type, end)
 
             if not unclosed:
```

### Comparing `zillionare-omicron-2.0.0a64/omicron/models/timeframe.py` & `zillionare-omicron-2.0.0a65/omicron/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/notify/dingtalk.py` & `zillionare-omicron-2.0.0a65/omicron/notify/dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/notify/mail.py` & `zillionare-omicron-2.0.0a65/omicron/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/plotting/candlestick.py` & `zillionare-omicron-2.0.0a65/omicron/plotting/candlestick.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/talib/core.py` & `zillionare-omicron-2.0.0a65/omicron/talib/core.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/omicron/talib/morph.py` & `zillionare-omicron-2.0.0a65/omicron/talib/morph.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/pyproject.toml` & `zillionare-omicron-2.0.0a65/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.poetry.dev-dependencies]
 [tool.poetry]
 name = "zillionare-omicron"
 packages = [
     {include = "omicron"}
 ]
-version = "2.0.0a64"
+version = "2.0.0a65"
 description = "Core Library for Zillionare"
 authors = ["jieyu <code@jieyu.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zillionare-omicron.readthedocs.io"
 repository = "https://github.com/zillionare/omicron"
 documentation = "https://zillionare-omicron.readthedocs.io"
```

### Comparing `zillionare-omicron-2.0.0a64/tests/__init__.py` & `zillionare-omicron-2.0.0a65/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/core/test_triggers.py` & `zillionare-omicron-2.0.0a65/tests/core/test_triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/core/test_types.py` & `zillionare-omicron-2.0.0a65/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/dal/influx/__init__.py` & `zillionare-omicron-2.0.0a65/tests/dal/influx/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/dal/influx/test_escape.py` & `zillionare-omicron-2.0.0a65/tests/dal/influx/test_escape.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/dal/influx/test_flux.py` & `zillionare-omicron-2.0.0a65/tests/dal/influx/test_flux.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/dal/influx/test_influxclient.py` & `zillionare-omicron-2.0.0a65/tests/dal/influx/test_influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/dal/influx/test_serialize.py` & `zillionare-omicron-2.0.0a65/tests/dal/influx/test_serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.15m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.15m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.1m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.30m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000001.XSHE.5m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.5m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.1d.csv` & `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.1m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.1w.csv` & `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000002.XSHE.30m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.1d.csv` & `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.1m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.1w.csv` & `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/000004.XSHE.30m.csv` & `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/README.md` & `zillionare-omicron-2.0.0a65/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/bars_1d.pkl` & `zillionare-omicron-2.0.0a65/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/bars_1m.pkl` & `zillionare-omicron-2.0.0a65/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/limits.csv` & `zillionare-omicron-2.0.0a65/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/stock_bars_flux_query.txt` & `zillionare-omicron-2.0.0a65/tests/data/stock_bars_flux_query.txt`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/data/test.jpg` & `zillionare-omicron-2.0.0a65/tests/data/test.jpg`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/extensions/test_decimals.py` & `zillionare-omicron-2.0.0a65/tests/extensions/test_decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/extensions/test_np.py` & `zillionare-omicron-2.0.0a65/tests/extensions/test_np.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/models/test_board.py` & `zillionare-omicron-2.0.0a65/tests/models/test_board.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/models/test_security.py` & `zillionare-omicron-2.0.0a65/tests/models/test_security.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/models/test_stock.py` & `zillionare-omicron-2.0.0a65/tests/models/test_stock.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/models/test_timeframe.py` & `zillionare-omicron-2.0.0a65/tests/models/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/notify/test_dingtalk.py` & `zillionare-omicron-2.0.0a65/tests/notify/test_dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/notify/test_mail.py` & `zillionare-omicron-2.0.0a65/tests/notify/test_mail.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/performance/influx/end2end.py` & `zillionare-omicron-2.0.0a65/tests/performance/influx/end2end.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/performance/influx/serialize.py` & `zillionare-omicron-2.0.0a65/tests/performance/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/talib/test_core.py` & `zillionare-omicron-2.0.0a65/tests/talib/test_core.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/tests/talib/test_morph.py` & `zillionare-omicron-2.0.0a65/tests/talib/test_morph.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a64/setup.py` & `zillionare-omicron-2.0.0a65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
           'pytest>=7.0.1,<8.0.0',
           'pytest-cov>=3.0.0,<4.0.0',
           'psutil>=5.7.3,<6.0.0',
           'freezegun>=1.2.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'zillionare-omicron',
-    'version': '2.0.0a64',
+    'version': '2.0.0a65',
     'description': 'Core Library for Zillionare',
     'long_description': '\n![](http://images.jieyu.ai/images/hot/zillionbanner.jpg)\n\n<h1 align="center">Omicron - Core Library for Zillionare</h1>\n\n\n[![Version](http://img.shields.io/pypi/v/zillionare-omicron?color=brightgreen)](https://pypi.python.org/pypi/zillionare-omicron)\n[![CI Status](https://github.com/zillionare/omicron/actions/workflows/release.yml/badge.svg)](https://github.com/zillionare/omicron)\n[![Code Coverage](https://img.shields.io/codecov/c/github/zillionare/omicron)](https://app.codecov.io/gh/zillionare/omicron)\n<<<<<<< HEAD\n=======\n[![ReadtheDos](https://readthedocs.org/projects/omicron/badge/?version=latest)](https://omicron.readthedocs.io/en/latest/?badge=latest)\n>>>>>>> master\n[![Downloads](https://pepy.tech/badge/zillionare-omicron)](https://pepy.tech/project/zillionare-omicron)\n[![License](https://img.shields.io/badge/License-MIT.svg)](https://opensource.org/licenses/MIT)\n[![Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# Contents\n\n## 简介\n\nOmicron是Zillionare的核心公共模块，向其它模块提供行情数据、交易日历、证券列表、时间操作及Trigger等功能。\n\nOmicron是大富翁量化框架的一部分。您必须至少安装并运行[Omega](https://zillionare.github.io/omega)，然后才能利用omicron来访问上述数据。\n\n[使用文档](https://zillionare.github.io/omicron)\n\n## Credits\n\n<<<<<<< HEAD\nZillionare-Omicron采用[Python Project Wizard](https://zillionare.github.io/python-project-wizard)构建。\n=======\n* [Cookiecutter](https://github.com/audreyr/cookiecutter)\n* [Cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-pypackage)\n* ![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.svg) [Pycharm开源项目支持计划](https://www.jetbrains.com/?from=zillionare-omega)\n>>>>>>> master\n',
     'author': 'jieyu',
     'author_email': 'code@jieyu.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://zillionare-omicron.readthedocs.io',
```

### Comparing `zillionare-omicron-2.0.0a64/PKG-INFO` & `zillionare-omicron-2.0.0a65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-omicron
-Version: 2.0.0a64
+Version: 2.0.0a65
 Summary: Core Library for Zillionare
 Home-page: https://zillionare-omicron.readthedocs.io
 License: MIT
 Keywords: AI,quant,trade,stock
 Author: jieyu
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
```

