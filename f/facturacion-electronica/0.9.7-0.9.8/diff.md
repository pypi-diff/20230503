# Comparing `tmp/facturacion_electronica-0.9.7.tar.gz` & `tmp/facturacion_electronica-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/facturacion_electronica-0.9.7.tar", last modified: Tue Jan 21 20:29:41 2020, max compression
+gzip compressed data, was "dist/facturacion_electronica-0.9.8.tar", last modified: Wed Jan 22 00:49:45 2020, max compression
```

## Comparing `facturacion_electronica-0.9.7.tar` & `facturacion_electronica-0.9.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1680 2019-05-11 23:31:45.000000 facturacion_electronica-0.9.7/README.md
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1161 2020-01-21 20:29:33.000000 facturacion_electronica-0.9.7/setup.py
-drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica.egg-info/
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)      102 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica.egg-info/requires.txt
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2241 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica.egg-info/SOURCES.txt
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)       24 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica.egg-info/top_level.txt
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)      640 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica.egg-info/PKG-INFO
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)        1 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica.egg-info/dependency_links.txt
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)      640 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/PKG-INFO
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)       38 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/setup.cfg
-drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica/
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    12723 2019-12-12 21:09:26.000000 facturacion_electronica-0.9.7/facturacion_electronica/consumo_folios.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)       33 2018-10-04 00:56:37.000000 facturacion_electronica-0.9.7/facturacion_electronica/__init__.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4937 2020-01-20 18:18:26.000000 facturacion_electronica-0.9.7/facturacion_electronica/clase_util.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    13061 2019-12-28 06:04:15.000000 facturacion_electronica-0.9.7/facturacion_electronica/conexion.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    11215 2019-10-13 07:05:48.000000 facturacion_electronica-0.9.7/facturacion_electronica/firma.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)      483 2018-09-16 06:57:02.000000 facturacion_electronica-0.9.7/facturacion_electronica/documento_respuesta.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    13277 2019-12-19 00:14:50.000000 facturacion_electronica-0.9.7/facturacion_electronica/respuesta.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    11597 2020-01-20 17:17:58.000000 facturacion_electronica-0.9.7/facturacion_electronica/dte.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1656 2019-09-09 01:37:48.000000 facturacion_electronica-0.9.7/facturacion_electronica/documento_referencias.py
--rw-rw-r--   0 dansanti  (1000) dansanti  (1000)     7325 2020-01-20 23:56:04.000000 facturacion_electronica-0.9.7/facturacion_electronica/documento_exportacion.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    22360 2019-12-19 00:17:34.000000 facturacion_electronica-0.9.7/facturacion_electronica/envio.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     8834 2020-01-20 03:42:45.000000 facturacion_electronica-0.9.7/facturacion_electronica/documento_linea.py
-drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-21 20:29:41.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    72177 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroCV_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    25891 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroGuia_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     9034 2018-07-04 19:59:38.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/Cesion_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    72739 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroCVS_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     3776 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/EnvioRecibos_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    52658 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/EnvioBOLETA_v11.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     7135 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/xmldsignature_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)   231196 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/DTE_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    17918 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/RespuestaEnvioDTE_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4202 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/Recibos_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2619 2018-07-04 19:20:35.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/DTECedido_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     3962 2018-07-04 19:59:35.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/AEC_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    33065 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroBOLETA_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    28914 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/SiiTypes_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4738 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/EnvioDTE_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     9509 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LceSiiTypes_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2438 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LceCoCertif_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     5671 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/LceCal_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4180 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/RespSII_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     9982 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.7/facturacion_electronica/xsd/ConsumoFolio_v10.xsd
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2592 2020-01-17 16:41:39.000000 facturacion_electronica-0.9.7/facturacion_electronica/receptor.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1494 2019-11-26 02:10:31.000000 facturacion_electronica-0.9.7/facturacion_electronica/impuestos.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1806 2020-01-21 19:37:02.000000 facturacion_electronica-0.9.7/facturacion_electronica/linea_impuesto.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4173 2020-01-03 00:35:18.000000 facturacion_electronica-0.9.7/facturacion_electronica/emisor.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1419 2019-10-13 07:03:05.000000 facturacion_electronica-0.9.7/facturacion_electronica/caf.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     7891 2019-12-04 10:07:19.000000 facturacion_electronica-0.9.7/facturacion_electronica/cesion.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2760 2019-02-15 10:28:41.000000 facturacion_electronica-0.9.7/facturacion_electronica/libro_boletas.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2728 2019-12-27 05:19:25.000000 facturacion_electronica-0.9.7/facturacion_electronica/global_descuento_recargo.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     3463 2019-04-28 00:42:08.000000 facturacion_electronica-0.9.7/facturacion_electronica/signature_cert.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1122 2019-11-28 14:57:13.000000 facturacion_electronica-0.9.7/facturacion_electronica/cesionario.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    41598 2020-01-21 01:14:51.000000 facturacion_electronica-0.9.7/facturacion_electronica/documento.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)      291 2019-11-28 13:16:07.000000 facturacion_electronica-0.9.7/facturacion_electronica/cesion_imagen.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1021 2019-11-28 15:20:46.000000 facturacion_electronica-0.9.7/facturacion_electronica/cedente.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    14192 2020-01-21 20:29:24.000000 facturacion_electronica-0.9.7/facturacion_electronica/facturacion_electronica.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)    28427 2020-01-15 20:55:49.000000 facturacion_electronica-0.9.7/facturacion_electronica/libro.py
--rw-r--r--   0 dansanti  (1000) dansanti  (1000)       38 2018-09-15 02:44:46.000000 facturacion_electronica-0.9.7/MANIFEST.in
+drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1680 2019-05-11 23:31:45.000000 facturacion_electronica-0.9.8/README.md
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1161 2020-01-22 00:48:22.000000 facturacion_electronica-0.9.8/setup.py
+drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica.egg-info/
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)      102 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica.egg-info/requires.txt
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2241 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica.egg-info/SOURCES.txt
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)       24 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica.egg-info/top_level.txt
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)      640 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica.egg-info/PKG-INFO
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)        1 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica.egg-info/dependency_links.txt
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)      640 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/PKG-INFO
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)       38 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/setup.cfg
+drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica/
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    12723 2019-12-12 21:09:26.000000 facturacion_electronica-0.9.8/facturacion_electronica/consumo_folios.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)       33 2018-10-04 00:56:37.000000 facturacion_electronica-0.9.8/facturacion_electronica/__init__.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4937 2020-01-20 18:18:26.000000 facturacion_electronica-0.9.8/facturacion_electronica/clase_util.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    13061 2019-12-28 06:04:15.000000 facturacion_electronica-0.9.8/facturacion_electronica/conexion.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    11215 2019-10-13 07:05:48.000000 facturacion_electronica-0.9.8/facturacion_electronica/firma.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)      483 2018-09-16 06:57:02.000000 facturacion_electronica-0.9.8/facturacion_electronica/documento_respuesta.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    13277 2019-12-19 00:14:50.000000 facturacion_electronica-0.9.8/facturacion_electronica/respuesta.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    11597 2020-01-20 17:17:58.000000 facturacion_electronica-0.9.8/facturacion_electronica/dte.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1656 2019-09-09 01:37:48.000000 facturacion_electronica-0.9.8/facturacion_electronica/documento_referencias.py
+-rw-rw-r--   0 dansanti  (1000) dansanti  (1000)     7325 2020-01-20 23:56:04.000000 facturacion_electronica-0.9.8/facturacion_electronica/documento_exportacion.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    22360 2019-12-19 00:17:34.000000 facturacion_electronica-0.9.8/facturacion_electronica/envio.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     8834 2020-01-20 03:42:45.000000 facturacion_electronica-0.9.8/facturacion_electronica/documento_linea.py
+drwxr-xr-x   0 dansanti  (1000) dansanti  (1000)        0 2020-01-22 00:49:45.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    72177 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroCV_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    25891 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroGuia_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     9034 2018-07-04 19:59:38.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/Cesion_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    72739 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroCVS_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     3776 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/EnvioRecibos_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    52658 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/EnvioBOLETA_v11.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     7135 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/xmldsignature_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)   231196 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/DTE_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    17918 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/RespuestaEnvioDTE_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4202 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/Recibos_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2619 2018-07-04 19:20:35.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/DTECedido_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     3962 2018-07-04 19:59:35.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/AEC_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    33065 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroBOLETA_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    28914 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/SiiTypes_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4738 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/EnvioDTE_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     9509 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LceSiiTypes_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2438 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LceCoCertif_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     5671 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/LceCal_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4180 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/RespSII_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     9982 2018-09-15 02:44:47.000000 facturacion_electronica-0.9.8/facturacion_electronica/xsd/ConsumoFolio_v10.xsd
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2592 2020-01-17 16:41:39.000000 facturacion_electronica-0.9.8/facturacion_electronica/receptor.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1494 2019-11-26 02:10:31.000000 facturacion_electronica-0.9.8/facturacion_electronica/impuestos.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1806 2020-01-21 19:37:02.000000 facturacion_electronica-0.9.8/facturacion_electronica/linea_impuesto.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     4173 2020-01-03 00:35:18.000000 facturacion_electronica-0.9.8/facturacion_electronica/emisor.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1419 2019-10-13 07:03:05.000000 facturacion_electronica-0.9.8/facturacion_electronica/caf.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     7891 2019-12-04 10:07:19.000000 facturacion_electronica-0.9.8/facturacion_electronica/cesion.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2760 2019-02-15 10:28:41.000000 facturacion_electronica-0.9.8/facturacion_electronica/libro_boletas.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     2728 2019-12-27 05:19:25.000000 facturacion_electronica-0.9.8/facturacion_electronica/global_descuento_recargo.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     3463 2019-04-28 00:42:08.000000 facturacion_electronica-0.9.8/facturacion_electronica/signature_cert.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1122 2019-11-28 14:57:13.000000 facturacion_electronica-0.9.8/facturacion_electronica/cesionario.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    41659 2020-01-22 00:46:44.000000 facturacion_electronica-0.9.8/facturacion_electronica/documento.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)      291 2019-11-28 13:16:07.000000 facturacion_electronica-0.9.8/facturacion_electronica/cesion_imagen.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)     1021 2019-11-28 15:20:46.000000 facturacion_electronica-0.9.8/facturacion_electronica/cedente.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    14192 2020-01-21 20:29:24.000000 facturacion_electronica-0.9.8/facturacion_electronica/facturacion_electronica.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)    28427 2020-01-15 20:55:49.000000 facturacion_electronica-0.9.8/facturacion_electronica/libro.py
+-rw-r--r--   0 dansanti  (1000) dansanti  (1000)       38 2018-09-15 02:44:46.000000 facturacion_electronica-0.9.8/MANIFEST.in
```

### Comparing `facturacion_electronica-0.9.7/README.md` & `facturacion_electronica-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/setup.py` & `facturacion_electronica-0.9.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
         name='facturacion_electronica',
-        version='0.9.7',
+        version='0.9.8',
         packages=find_packages(),
         package_data={'facturacion_electronica': ['xsd/*.xsd']},
         install_requires=[
             'lxml',
             'cryptography',
             'pyOpenSSL',
             'certifi',
```

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica.egg-info/SOURCES.txt` & `facturacion_electronica-0.9.8/facturacion_electronica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/PKG-INFO` & `facturacion_electronica-0.9.8/facturacion_electronica.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: facturacion_electronica
-Version: 0.9.7
+Name: facturacion-electronica
+Version: 0.9.8
 Summary: UNKNOWN
 Home-page: https://gitlab.com/dansanti/facturacion_electronica
 Author: Daniel Santibáñez Polanco
 Author-email: dansanti@gmail.com
 License: GPLV3+
 Description: Módulo de Facturación Electrónica Chilena
 Platform: UNKNOWN
```

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/consumo_folios.py` & `facturacion_electronica-0.9.8/facturacion_electronica/consumo_folios.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/clase_util.py` & `facturacion_electronica-0.9.8/facturacion_electronica/clase_util.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/conexion.py` & `facturacion_electronica-0.9.8/facturacion_electronica/conexion.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/firma.py` & `facturacion_electronica-0.9.8/facturacion_electronica/firma.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/respuesta.py` & `facturacion_electronica-0.9.8/facturacion_electronica/respuesta.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/dte.py` & `facturacion_electronica-0.9.8/facturacion_electronica/dte.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/documento_referencias.py` & `facturacion_electronica-0.9.8/facturacion_electronica/documento_referencias.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/documento_exportacion.py` & `facturacion_electronica-0.9.8/facturacion_electronica/documento_exportacion.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/envio.py` & `facturacion_electronica-0.9.8/facturacion_electronica/envio.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/documento_linea.py` & `facturacion_electronica-0.9.8/facturacion_electronica/documento_linea.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroCV_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroCV_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroGuia_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroGuia_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/Cesion_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/Cesion_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroCVS_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroCVS_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/EnvioRecibos_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/EnvioRecibos_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/EnvioBOLETA_v11.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/EnvioBOLETA_v11.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/xmldsignature_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/xmldsignature_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/DTE_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/DTE_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/RespuestaEnvioDTE_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/RespuestaEnvioDTE_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/Recibos_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/Recibos_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/DTECedido_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/DTECedido_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/AEC_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/AEC_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LibroBOLETA_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LibroBOLETA_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/SiiTypes_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/SiiTypes_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/EnvioDTE_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/EnvioDTE_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LceSiiTypes_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LceSiiTypes_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LceCoCertif_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LceCoCertif_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/LceCal_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/LceCal_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/RespSII_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/RespSII_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/xsd/ConsumoFolio_v10.xsd` & `facturacion_electronica-0.9.8/facturacion_electronica/xsd/ConsumoFolio_v10.xsd`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/receptor.py` & `facturacion_electronica-0.9.8/facturacion_electronica/receptor.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/impuestos.py` & `facturacion_electronica-0.9.8/facturacion_electronica/impuestos.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/linea_impuesto.py` & `facturacion_electronica-0.9.8/facturacion_electronica/linea_impuesto.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/emisor.py` & `facturacion_electronica-0.9.8/facturacion_electronica/emisor.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/caf.py` & `facturacion_electronica-0.9.8/facturacion_electronica/caf.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/cesion.py` & `facturacion_electronica-0.9.8/facturacion_electronica/cesion.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/libro_boletas.py` & `facturacion_electronica-0.9.8/facturacion_electronica/libro_boletas.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/global_descuento_recargo.py` & `facturacion_electronica-0.9.8/facturacion_electronica/global_descuento_recargo.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/signature_cert.py` & `facturacion_electronica-0.9.8/facturacion_electronica/signature_cert.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/cesionario.py` & `facturacion_electronica-0.9.8/facturacion_electronica/cesionario.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/documento.py` & `facturacion_electronica-0.9.8/facturacion_electronica/documento.py`

 * *Files 0% similar despite different names*

```diff
@@ -959,14 +959,16 @@
             return False
         return self._patente
 
     @property
     def OtraMoneda(self):
         if not self.TpoCambio:
             return False
+        if self.FmaPagExp == 21:
+            return ''
         Totales = {}
         Totales['TpoMoneda'] = self.TpoMonedaOtr
         Totales['TpoCambio'] = self.TpoCambio
         if self.MntNetoOtrMnda:
             Totales['MntNetoOtrMnda'] = self.MntNetoOtrMnda
         if self.MntExeOtrMnda:
             Totales['MntExeOtrMnda'] = self.MntExeOtrMnda
@@ -1268,15 +1270,15 @@
                 Transporte['Chofer']['RUTChofer'] = self.RUTChofer
                 Transporte['Chofer']['NombreChofer'] = self.NombreChofer[:30]
         if self.IndTraslado:
             Transporte['DirDest'] = self.DirDest
             Transporte['CmnaDest'] = self.CmnaDest
             Transporte['CiudadDest'] = self.CiudadDest
         if self.Aduana or self.es_exportacion:
-            Transporte['Aduana'] = self.Aduana
+            Transporte['Aduana'] = self.Aduana or ''
         return Transporte
 
     @Transporte.setter
     def Transporte(self, vals):
         util.set_from_keys(self, vals)
 
     def es_boleta(self, include_reference=True):
```

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/cedente.py` & `facturacion_electronica-0.9.8/facturacion_electronica/cedente.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/facturacion_electronica.py` & `facturacion_electronica-0.9.8/facturacion_electronica/facturacion_electronica.py`

 * *Files identical despite different names*

### Comparing `facturacion_electronica-0.9.7/facturacion_electronica/libro.py` & `facturacion_electronica-0.9.8/facturacion_electronica/libro.py`

 * *Files identical despite different names*

