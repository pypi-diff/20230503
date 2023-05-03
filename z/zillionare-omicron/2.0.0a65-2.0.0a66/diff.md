# Comparing `tmp/zillionare-omicron-2.0.0a65.tar.gz` & `tmp/zillionare_omicron-2.0.0a66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare-omicron-2.0.0a65.tar", max compression
+gzip compressed data, was "zillionare_omicron-2.0.0a66.tar", max compression
```

## Comparing `zillionare-omicron-2.0.0a65.tar` & `zillionare_omicron-2.0.0a66.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0      112 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/AUTHORS.md
--rw-r--r--   0        0        0     1561 2022-09-19 02:47:00.722663 zillionare-omicron-2.0.0a65/HISTORY.md
--rw-r--r--   0        0        0     1068 2022-05-19 11:28:00.022177 zillionare-omicron-2.0.0a65/LICENSE
--rw-r--r--   0        0        0     1880 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/README.md
--rw-r--r--   0        0        0   503846 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a65/docs/_static/Omicron_Windows10.docx
--rw-r--r--   0        0        0     5620 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/_static/jetbrains-variant-3.svg
--rw-r--r--   0        0        0       84 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/dal/flux.md
--rw-r--r--   0        0        0      110 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/dal/influxclient.md
--rw-r--r--   0        0        0      189 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/dal/serialize.md
--rw-r--r--   0        0        0     5772 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a65/docs/api/metrics.md
--rw-r--r--   0        0        0      203 2022-11-08 08:08:31.311437 zillionare-omicron-2.0.0a65/docs/api/omicron.md
--rw-r--r--   0        0        0       73 2022-09-19 02:47:00.726663 zillionare-omicron-2.0.0a65/docs/api/plotting.md
--rw-r--r--   0        0        0       68 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a65/docs/api/security.md
--rw-r--r--   0        0        0       65 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/stock.md
--rw-r--r--   0        0        0       58 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/talib.md
--rw-r--r--   0        0        0       57 2022-05-19 11:30:57.754131 zillionare-omicron-2.0.0a65/docs/api/timeframe.md
--rw-r--r--   0        0        0       66 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/api/triggers.md
--rw-r--r--   0        0        0      907 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/css/extra.css
--rw-r--r--   0        0        0     1778 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a65/docs/developer.md
--rw-r--r--   0        0        0       43 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/history.md
--rw-r--r--   0        0        0       42 2022-05-19 11:28:00.026177 zillionare-omicron-2.0.0a65/docs/index.md
--rw-r--r--   0        0        0     1820 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a65/docs/installation.md
--rw-r--r--   0        0        0     9823 2022-09-07 09:45:22.189476 zillionare-omicron-2.0.0a65/docs/usage.md
--rw-r--r--   0        0        0      920 2022-09-25 07:32:43.784350 zillionare-omicron-2.0.0a65/omicron/__init__.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a65/omicron/config/__init__.py
--rw-r--r--   0        0        0    56389 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a65/omicron/config/calendar.json
--rw-r--r--   0        0        0      441 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a65/omicron/config/defaults.yaml
--rw-r--r--   0        0        0      378 2022-10-02 07:50:29.380175 zillionare-omicron-2.0.0a65/omicron/config/dev.yaml
--rw-r--r--   0        0        0     1334 2022-09-07 09:45:22.201476 zillionare-omicron-2.0.0a65/omicron/config/schema.py
--rw-r--r--   0        0        0      816 2022-05-19 11:28:00.030177 zillionare-omicron-2.0.0a65/omicron/config/sql/v0.6.sql
--rw-r--r--   0        0        0     2785 2022-05-19 11:30:57.758131 zillionare-omicron-2.0.0a65/omicron/config/sql/v1.0.sql
--rw-r--r--   0        0        0       46 2022-05-19 11:28:00.030177 zillionare-omicron-2.0.0a65/omicron/core/__init__.py
--rw-r--r--   0        0        0      140 2022-08-04 07:38:19.097441 zillionare-omicron-2.0.0a65/omicron/core/constants.py
--rw-r--r--   0        0        0     1095 2022-09-07 09:45:22.201476 zillionare-omicron-2.0.0a65/omicron/core/errors.py
--rw-r--r--   0        0        0       46 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/core/events.py
--rw-r--r--   0        0        0     6517 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/core/triggers.py
--rw-r--r--   0        0        0       71 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/dal/__init__.py
--rw-r--r--   0        0        0     3215 2022-12-08 01:58:13.329503 zillionare-omicron-2.0.0a65/omicron/dal/cache.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/dal/influx/__init__.py
--rw-r--r--   0        0        0      370 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/dal/influx/errors.py
--rw-r--r--   0        0        0      996 2022-05-19 11:30:57.762131 zillionare-omicron-2.0.0a65/omicron/dal/influx/escape.py
--rw-r--r--   0        0        0    19097 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/dal/influx/flux.py
--rw-r--r--   0        0        0    16805 2022-09-24 09:12:02.824758 zillionare-omicron-2.0.0a65/omicron/dal/influx/influxclient.py
--rw-r--r--   0        0        0    27708 2022-09-07 09:45:22.205476 zillionare-omicron-2.0.0a65/omicron/dal/influx/serialize.py
--rw-r--r--   0        0        0       78 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a65/omicron/extensions/__init__.py
--rw-r--r--   0        0        0      656 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a65/omicron/extensions/decimals.py
--rw-r--r--   0        0        0    15929 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/extensions/np.py
--rw-r--r--   0        0        0      492 2022-10-14 08:08:29.548960 zillionare-omicron-2.0.0a65/omicron/models/__init__.py
--rw-r--r--   0        0        0     7867 2022-12-14 05:13:08.492827 zillionare-omicron-2.0.0a65/omicron/models/board.py
--rw-r--r--   0        0        0    26127 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/models/security.py
--rw-r--r--   0        0        0    53741 2022-12-16 02:06:19.061417 zillionare-omicron-2.0.0a65/omicron/models/stock.py
--rw-r--r--   0        0        0    41959 2022-09-26 02:36:43.062543 zillionare-omicron-2.0.0a65/omicron/models/timeframe.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.766131 zillionare-omicron-2.0.0a65/omicron/notify/__init__.py
--rw-r--r--   0        0        0     5472 2022-09-19 02:47:00.730664 zillionare-omicron-2.0.0a65/omicron/notify/dingtalk.py
--rw-r--r--   0        0        0     6006 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/notify/mail.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.770131 zillionare-omicron-2.0.0a65/omicron/notify/tts.py
--rw-r--r--   0        0        0        0 2022-09-19 02:47:00.734664 zillionare-omicron-2.0.0a65/omicron/plotting/__init__.py
--rw-r--r--   0        0        0    14071 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/plotting/candlestick.py
--rw-r--r--   0        0        0      114 2022-09-19 02:47:00.734664 zillionare-omicron-2.0.0a65/omicron/talib/__init__.py
--rw-r--r--   0        0        0     9958 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/talib/core.py
--rw-r--r--   0        0        0    23141 2022-12-04 08:55:43.447990 zillionare-omicron-2.0.0a65/omicron/talib/morph.py
--rwxr-xr-x   0        0        0     3297 2022-12-16 02:17:43.823747 zillionare-omicron-2.0.0a65/pyproject.toml
--rw-r--r--   0        0        0     5556 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a65/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.782132 zillionare-omicron-2.0.0a65/tests/core/__init__.py
--rw-r--r--   0        0        0      297 2022-09-07 09:45:22.237476 zillionare-omicron-2.0.0a65/tests/core/test_errors.py
--rw-r--r--   0        0        0     3615 2022-05-19 11:30:57.782132 zillionare-omicron-2.0.0a65/tests/core/test_triggers.py
--rw-r--r--   0        0        0     1024 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/core/test_types.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/dal/__init__.py
--rw-r--r--   0        0        0      622 2022-06-25 11:03:39.472127 zillionare-omicron-2.0.0a65/tests/dal/influx/__init__.py
--rw-r--r--   0        0        0     1177 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/dal/influx/test_escape.py
--rw-r--r--   0        0        0     8531 2022-06-25 11:03:39.472127 zillionare-omicron-2.0.0a65/tests/dal/influx/test_flux.py
--rw-r--r--   0        0        0    14284 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a65/tests/dal/influx/test_influxclient.py
--rw-r--r--   0        0        0    15710 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a65/tests/dal/influx/test_serialize.py
--rw-r--r--   0        0        0     1253 2022-09-07 09:45:22.245477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.15m.csv
--rw-r--r--   0        0        0      118 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1M.csv
--rw-r--r--   0        0        0      188 2022-09-07 09:45:22.253477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1d.csv
--rw-r--r--   0        0        0    22206 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1m.csv
--rw-r--r--   0        0        0      115 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1w.csv
--rw-r--r--   0        0        0      654 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.30m.csv
--rw-r--r--   0        0        0     3633 2022-09-07 09:45:22.257477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.5m.csv
--rw-r--r--   0        0        0      352 2022-09-07 09:45:22.257477 zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.60m.csv
--rw-r--r--   0        0        0     8089 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1d.csv
--rw-r--r--   0        0        0    22419 2022-05-19 11:30:57.786132 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1m.csv
--rw-r--r--   0        0        0     7166 2022-09-07 09:45:22.269477 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1w.csv
--rw-r--r--   0        0        0     8096 2022-09-07 09:45:22.281477 zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.30m.csv
--rw-r--r--   0        0        0     7585 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1d.csv
--rw-r--r--   0        0        0    20344 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1m.csv
--rw-r--r--   0        0        0     6443 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1w.csv
--rw-r--r--   0        0        0     7688 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.30m.csv
--rw-r--r--   0        0        0     1145 2022-09-07 09:45:22.289477 zillionare-omicron-2.0.0a65/tests/data/README.md
--rw-r--r--   0        0        0     2191 2022-05-19 11:30:57.790132 zillionare-omicron-2.0.0a65/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2022-05-19 11:30:57.794132 zillionare-omicron-2.0.0a65/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      713 2022-05-19 11:30:57.794132 zillionare-omicron-2.0.0a65/tests/data/limits.csv
--rw-r--r--   0        0        0   164066 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/data/stock_bars_flux_query.txt
--rw-r--r--   0        0        0     6315 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/data/test.jpg
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/extensions/__init__.py
--rw-r--r--   0        0        0      594 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/extensions/test_decimals.py
--rw-r--r--   0        0        0     9864 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a65/tests/extensions/test_np.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.798132 zillionare-omicron-2.0.0a65/tests/models/__init__.py
--rw-r--r--   0        0        0     6802 2022-12-14 09:53:29.108769 zillionare-omicron-2.0.0a65/tests/models/test_board.py
--rw-r--r--   0        0        0    11161 2022-12-04 08:55:43.451990 zillionare-omicron-2.0.0a65/tests/models/test_security.py
--rw-r--r--   0        0        0    68822 2022-11-08 08:08:31.311437 zillionare-omicron-2.0.0a65/tests/models/test_stock.py
--rw-r--r--   0        0        0    36351 2022-09-23 11:09:33.778515 zillionare-omicron-2.0.0a65/tests/models/test_timeframe.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.802132 zillionare-omicron-2.0.0a65/tests/notify/__init__.py
--rw-r--r--   0        0        0      823 2022-09-07 09:45:22.293477 zillionare-omicron-2.0.0a65/tests/notify/test_dingtalk.py
--rw-r--r--   0        0        0     2686 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a65/tests/notify/test_mail.py
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a65/tests/performance/influx/__init__.py
--rw-r--r--   0        0        0     3317 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a65/tests/performance/influx/end2end.py
--rw-r--r--   0        0        0     4197 2022-06-25 11:03:39.476127 zillionare-omicron-2.0.0a65/tests/performance/influx/serialize.py
--rw-r--r--   0        0        0      294 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a65/tests/performance/readme.md
--rw-r--r--   0        0        0      406 2022-05-19 11:28:00.038178 zillionare-omicron-2.0.0a65/tests/pyrightconfig.json
--rw-r--r--   0        0        0        0 2022-05-19 11:30:57.806132 zillionare-omicron-2.0.0a65/tests/talib/__init__.py
--rw-r--r--   0        0        0     2917 2022-09-19 02:47:00.742664 zillionare-omicron-2.0.0a65/tests/talib/test_core.py
--rw-r--r--   0        0        0    37991 2022-12-12 12:04:52.265182 zillionare-omicron-2.0.0a65/tests/talib/test_morph.py
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 zillionare-omicron-2.0.0a65/setup.py
--rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 zillionare-omicron-2.0.0a65/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a66/AUTHORS.md
+-rw-r--r--   0        0        0     1561 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a66/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a66/LICENSE
+-rw-r--r--   0        0        0     1880 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a66/README.md
+-rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/_static/Omicron_Windows10.docx
+-rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a66/docs/_static/jetbrains-variant-3.svg
+-rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/dal/flux.md
+-rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/dal/influxclient.md
+-rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/dal/serialize.md
+-rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/metrics.md
+-rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/omicron.md
+-rw-r--r--   0        0        0       73 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/plotting.md
+-rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/security.md
+-rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/stock.md
+-rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/talib.md
+-rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/timeframe.md
+-rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/api/triggers.md
+-rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/css/extra.css
+-rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/developer.md
+-rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/history.md
+-rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/index.md
+-rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/installation.md
+-rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/usage.md
+-rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/omicron/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/omicron/config/__init__.py
+-rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/calendar.json
+-rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/defaults.yaml
+-rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/dev.yaml
+-rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/schema.py
+-rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a66/omicron/config/sql/v0.6.sql
+-rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/sql/v1.0.sql
+-rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a66/omicron/core/__init__.py
+-rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/constants.py
+-rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/errors.py
+-rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/events.py
+-rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/triggers.py
+-rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/__init__.py
+-rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/cache.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/influx/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/influx/errors.py
+-rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/influx/escape.py
+-rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/dal/influx/flux.py
+-rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/dal/influx/influxclient.py
+-rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/dal/influx/serialize.py
+-rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/extensions/__init__.py
+-rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/extensions/decimals.py
+-rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a66/omicron/extensions/np.py
+-rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/models/__init__.py
+-rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/models/board.py
+-rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/models/security.py
+-rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/models/stock.py
+-rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/models/timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/__init__.py
+-rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/dingtalk.py
+-rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/tts.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/plotting/__init__.py
+-rw-r--r--   0        0        0    14220 2023-05-03 09:06:32.908144 zillionare_omicron-2.0.0a66/omicron/plotting/candlestick.py
+-rw-r--r--   0        0        0     8636 2023-05-03 08:59:53.293039 zillionare_omicron-2.0.0a66/omicron/plotting/metrics.py
+-rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/talib/__init__.py
+-rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a66/omicron/talib/core.py
+-rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a66/omicron/talib/morph.py
+-rwxr-xr-x   0        0        0     3312 2023-05-03 10:52:55.254047 zillionare_omicron-2.0.0a66/pyproject.toml
+-rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/core/__init__.py
+-rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/core/test_errors.py
+-rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/core/test_triggers.py
+-rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/core/test_types.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/__init__.py
+-rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/__init__.py
+-rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_escape.py
+-rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_flux.py
+-rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_influxclient.py
+-rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_serialize.py
+-rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.15m.csv
+-rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1M.csv
+-rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1d.csv
+-rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1m.csv
+-rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1w.csv
+-rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.30m.csv
+-rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.5m.csv
+-rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.60m.csv
+-rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1d.csv
+-rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1m.csv
+-rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1w.csv
+-rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.30m.csv
+-rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1d.csv
+-rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1m.csv
+-rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1w.csv
+-rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.30m.csv
+-rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/README.md
+-rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a66/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/data/limits.csv
+-rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/data/stock_bars_flux_query.txt
+-rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/data/test.jpg
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/extensions/__init__.py
+-rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/extensions/test_decimals.py
+-rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/extensions/test_np.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/models/__init__.py
+-rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/models/test_board.py
+-rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/models/test_security.py
+-rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/models/test_stock.py
+-rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/models/test_timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/notify/__init__.py
+-rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/notify/test_dingtalk.py
+-rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/notify/test_mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/influx/__init__.py
+-rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/influx/end2end.py
+-rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/influx/serialize.py
+-rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/readme.md
+-rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a66/tests/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/talib/__init__.py
+-rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/talib/test_core.py
+-rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/talib/test_morph.py
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a66/PKG-INFO
```

### Comparing `zillionare-omicron-2.0.0a65/HISTORY.md` & `zillionare_omicron-2.0.0a66/HISTORY.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/LICENSE` & `zillionare_omicron-2.0.0a66/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/README.md` & `zillionare_omicron-2.0.0a66/README.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/_static/Omicron_Windows10.docx` & `zillionare_omicron-2.0.0a66/docs/_static/Omicron_Windows10.docx`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/_static/jetbrains-variant-3.svg` & `zillionare_omicron-2.0.0a66/docs/_static/jetbrains-variant-3.svg`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/api/metrics.md` & `zillionare_omicron-2.0.0a66/docs/api/metrics.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/css/extra.css` & `zillionare_omicron-2.0.0a66/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/developer.md` & `zillionare_omicron-2.0.0a66/docs/developer.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/installation.md` & `zillionare_omicron-2.0.0a66/docs/installation.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/docs/usage.md` & `zillionare_omicron-2.0.0a66/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/__init__.py` & `zillionare_omicron-2.0.0a66/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/config/calendar.json` & `zillionare_omicron-2.0.0a66/omicron/config/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/config/schema.py` & `zillionare_omicron-2.0.0a66/omicron/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/config/sql/v0.6.sql` & `zillionare_omicron-2.0.0a66/omicron/config/sql/v0.6.sql`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/config/sql/v1.0.sql` & `zillionare_omicron-2.0.0a66/omicron/config/sql/v1.0.sql`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/core/errors.py` & `zillionare_omicron-2.0.0a66/omicron/core/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/core/triggers.py` & `zillionare_omicron-2.0.0a66/omicron/core/triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/dal/cache.py` & `zillionare_omicron-2.0.0a66/omicron/dal/cache.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/dal/influx/escape.py` & `zillionare_omicron-2.0.0a66/omicron/dal/influx/escape.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/dal/influx/flux.py` & `zillionare_omicron-2.0.0a66/omicron/dal/influx/flux.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/dal/influx/influxclient.py` & `zillionare_omicron-2.0.0a66/omicron/dal/influx/influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/dal/influx/serialize.py` & `zillionare_omicron-2.0.0a66/omicron/dal/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/extensions/decimals.py` & `zillionare_omicron-2.0.0a66/omicron/extensions/decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/extensions/np.py` & `zillionare_omicron-2.0.0a66/omicron/extensions/np.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/models/board.py` & `zillionare_omicron-2.0.0a66/omicron/models/board.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/models/security.py` & `zillionare_omicron-2.0.0a66/omicron/models/security.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/models/stock.py` & `zillionare_omicron-2.0.0a66/omicron/models/stock.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/models/timeframe.py` & `zillionare_omicron-2.0.0a66/omicron/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/notify/dingtalk.py` & `zillionare_omicron-2.0.0a66/omicron/notify/dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/notify/mail.py` & `zillionare_omicron-2.0.0a66/omicron/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/plotting/candlestick.py` & `zillionare_omicron-2.0.0a66/omicron/plotting/candlestick.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,17 @@
         """
         boxes = plateaus(self.bars["close"], min_size)
         self.add_main_trace("bbox", boxes=boxes)
 
     def mark_backtest_result(self, result: dict):
         """标记买卖点和回测数据
 
+        TODO:
+            此方法可能未与backtest返回值同步。此外，在portofolio回测中，不可能在k线图中使用此方法。
+
         Args:
             points : 买卖点的坐标。
         """
         trades = result.get("trades")
         assets = result.get("assets")
 
         x, y, labels = [], [], []
```

### Comparing `zillionare-omicron-2.0.0a65/omicron/talib/core.py` & `zillionare_omicron-2.0.0a66/omicron/talib/core.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/omicron/talib/morph.py` & `zillionare_omicron-2.0.0a66/omicron/talib/morph.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/pyproject.toml` & `zillionare_omicron-2.0.0a66/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [[tool.poetry.source]]
 name = "ali"
 url = "https://mirrors.aliyun.com/pypi/simple/"
-secondary = true
+default = true
+secondary=false
 
 
 [tool.poetry.dev-dependencies]
 [tool.poetry]
 name = "zillionare-omicron"
 packages = [
     {include = "omicron"}
 ]
-version = "2.0.0a65"
+version = "2.0.0.a66"
 description = "Core Library for Zillionare"
 authors = ["jieyu <code@jieyu.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zillionare-omicron.readthedocs.io"
 repository = "https://github.com/zillionare/omicron"
 documentation = "https://zillionare-omicron.readthedocs.io"
```

### Comparing `zillionare-omicron-2.0.0a65/tests/__init__.py` & `zillionare_omicron-2.0.0a66/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/core/test_triggers.py` & `zillionare_omicron-2.0.0a66/tests/core/test_triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/core/test_types.py` & `zillionare_omicron-2.0.0a66/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/dal/influx/__init__.py` & `zillionare_omicron-2.0.0a66/tests/dal/influx/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/dal/influx/test_escape.py` & `zillionare_omicron-2.0.0a66/tests/dal/influx/test_escape.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/dal/influx/test_flux.py` & `zillionare_omicron-2.0.0a66/tests/dal/influx/test_flux.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/dal/influx/test_influxclient.py` & `zillionare_omicron-2.0.0a66/tests/dal/influx/test_influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/dal/influx/test_serialize.py` & `zillionare_omicron-2.0.0a66/tests/dal/influx/test_serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.15m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.15m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.1m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.30m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000001.XSHE.5m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.5m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1d.csv` & `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.1w.csv` & `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000002.XSHE.30m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1d.csv` & `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.1w.csv` & `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/000004.XSHE.30m.csv` & `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/README.md` & `zillionare_omicron-2.0.0a66/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/bars_1d.pkl` & `zillionare_omicron-2.0.0a66/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/bars_1m.pkl` & `zillionare_omicron-2.0.0a66/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/limits.csv` & `zillionare_omicron-2.0.0a66/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/stock_bars_flux_query.txt` & `zillionare_omicron-2.0.0a66/tests/data/stock_bars_flux_query.txt`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/data/test.jpg` & `zillionare_omicron-2.0.0a66/tests/data/test.jpg`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/extensions/test_decimals.py` & `zillionare_omicron-2.0.0a66/tests/extensions/test_decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/extensions/test_np.py` & `zillionare_omicron-2.0.0a66/tests/extensions/test_np.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/models/test_board.py` & `zillionare_omicron-2.0.0a66/tests/models/test_board.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/models/test_security.py` & `zillionare_omicron-2.0.0a66/tests/models/test_security.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/models/test_stock.py` & `zillionare_omicron-2.0.0a66/tests/models/test_stock.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/models/test_timeframe.py` & `zillionare_omicron-2.0.0a66/tests/models/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/notify/test_dingtalk.py` & `zillionare_omicron-2.0.0a66/tests/notify/test_dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/notify/test_mail.py` & `zillionare_omicron-2.0.0a66/tests/notify/test_mail.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/performance/influx/end2end.py` & `zillionare_omicron-2.0.0a66/tests/performance/influx/end2end.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/performance/influx/serialize.py` & `zillionare_omicron-2.0.0a66/tests/performance/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/talib/test_core.py` & `zillionare_omicron-2.0.0a66/tests/talib/test_core.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/tests/talib/test_morph.py` & `zillionare_omicron-2.0.0a66/tests/talib/test_morph.py`

 * *Files identical despite different names*

### Comparing `zillionare-omicron-2.0.0a65/PKG-INFO` & `zillionare_omicron-2.0.0a66/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-omicron
-Version: 2.0.0a65
+Version: 2.0.0a66
 Summary: Core Library for Zillionare
 Home-page: https://zillionare-omicron.readthedocs.io
 License: MIT
 Keywords: AI,quant,trade,stock
 Author: jieyu
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
@@ -15,53 +15,53 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: Bottleneck (>=1.3.4,<2.0.0)
-Requires-Dist: TA-Lib (>=0.4.25,<0.5.0); sys_platform == "linux"
+Requires-Dist: TA-Lib (>=0.4.25,<0.5.0) ; sys_platform == "linux"
 Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
 Requires-Dist: aioredis (>=2.0.1,<3.0.0)
 Requires-Dist: aiosmtplib (>=1.1.6,<2.0.0)
 Requires-Dist: arrow (>=1.2,<2.0)
-Requires-Dist: black (>=22.3.0,<23.0.0); extra == "test"
+Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "test"
 Requires-Dist: cfg4py (>=0.9)
 Requires-Dist: ciso8601 (>=2.2.0,<3.0.0)
 Requires-Dist: ckwrap (>=0.1.10,<0.2.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: empyrical-reloaded (>=0.5.8,<0.6.0)
-Requires-Dist: flake8 (==4.0.1); extra == "test"
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0); extra == "test"
-Requires-Dist: freezegun (>=1.2.1,<2.0.0); extra == "test"
+Requires-Dist: flake8 (==4.0.1) ; extra == "test"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
+Requires-Dist: freezegun (>=1.2.1,<2.0.0) ; extra == "test"
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: isort (==5.10.1); extra == "test"
-Requires-Dist: livereload (>=2.6.3,<3.0.0); extra == "doc"
-Requires-Dist: mike (>=1.1.2,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs (>=1.3.0,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs-autorefs (>=0.3.1,<0.4.0); extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0); extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0); extra == "doc"
+Requires-Dist: isort (==5.10.1) ; extra == "test"
+Requires-Dist: livereload (>=2.6.3,<3.0.0) ; extra == "doc"
+Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs (>=1.3.0,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-autorefs (>=0.3.1,<0.4.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
-Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0); extra == "doc"
+Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra == "doc"
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
-Requires-Dist: pip (>=22.0.3,<23.0.0); extra == "dev"
+Requires-Dist: pip (>=22.0.3,<23.0.0) ; extra == "dev"
 Requires-Dist: plotly (>=5.10.0,<6.0.0)
-Requires-Dist: pre-commit (>=2.17.0,<3.0.0); extra == "dev"
-Requires-Dist: psutil (>=5.7.3,<6.0.0); extra == "test"
+Requires-Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev"
+Requires-Dist: psutil (>=5.7.3,<6.0.0) ; extra == "test"
 Requires-Dist: pyreadline (>=2.1,<3.0)
-Requires-Dist: pytest (>=7.0.1,<8.0.0); extra == "test"
-Requires-Dist: pytest-cov (>=3.0.0,<4.0.0); extra == "test"
+Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: sh (==1.14.1)
-Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "dev"
-Requires-Dist: tox (>=3.24.5,<4.0.0); extra == "dev"
-Requires-Dist: twine (>=3.8.0,<4.0.0); extra == "dev"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
+Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev"
+Requires-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev"
 Requires-Dist: zigzag (>=0.3,<0.4)
 Requires-Dist: zillionare-core-types (>=0.5.2,<0.6.0)
 Project-URL: Documentation, https://zillionare-omicron.readthedocs.io
 Project-URL: Repository, https://github.com/zillionare/omicron
 Description-Content-Type: text/markdown
```

