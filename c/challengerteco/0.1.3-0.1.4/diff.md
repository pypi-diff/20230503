# Comparing `tmp/challengerteco-0.1.3.tar.gz` & `tmp/challengerteco-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengerteco-0.1.3.tar", max compression
+gzip compressed data, was "challengerteco-0.1.4.tar", max compression
```

## Comparing `challengerteco-0.1.3.tar` & `challengerteco-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.3/README.md
--rw-r--r--   0        0        0    81982 2023-04-18 13:26:24.964418 challengerteco-0.1.3/challengerteco/Challenger.py
--rw-r--r--   0        0        0       37 2023-04-19 10:31:49.657535 challengerteco-0.1.3/challengerteco/__init__.py
--rw-r--r--   0        0        0      315 2023-04-19 10:31:59.204062 challengerteco-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.4/README.md
+-rw-r--r--   0        0        0    83000 2023-05-03 21:14:29.986893 challengerteco-0.1.4/challengerteco/Challenger.py
+-rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.4/challengerteco/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-03 21:17:34.959641 challengerteco-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.4/PKG-INFO
```

### Comparing `challengerteco-0.1.3/challengerteco/Challenger.py` & `challengerteco-0.1.4/challengerteco/Challenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             return self.spark.read.format("bigquery").option("query", query).load()
         else:
             return spark.sql(query)
 
 
 
 
-class Challenger():
+class Challengercito():
     def __init__(self,
                  BALANCEAR_TARGET:bool,
                  ELIMINAR_CORRELACIONES:bool,
                  CASTEAR_BIGINT:bool,
                  REDONDEAR_DECIMALES:bool,
                  CON_SCALER:bool,
                  TIENE_TESTING:bool,
@@ -140,14 +140,19 @@
                  bucket,
                  PATH:str='',
                  modelo_text:str='',
                  ambiente:str="sdb_datamining",
                  plataforma="OP",
                  gcp_project=None,
                  gcs_path=None,
+                 formato='parquet', #Fix
+                 PATH_MODELO=None, #Fix
+                 TMP_PATH=None, #Fix
+                 qm=None, #Fix
+                 
                  ) -> None:
 
 
         self.BALANCEAR_TARGET=BALANCEAR_TARGET
         self.ELIMINAR_CORRELACIONES=ELIMINAR_CORRELACIONES
         self.CASTEAR_BIGINT=CASTEAR_BIGINT
         self.REDONDEAR_DECIMALES=REDONDEAR_DECIMALES
@@ -194,15 +199,15 @@
         self.Tabla_Performance_Modelos = Tabla_Performance_Modelos
         self.spark=spark
         self.bq=bq
         self.bucket=bucket
 
         self.modelo_text=modelo_text
         self.ambiente=ambiente
-        self.formato='parquet'
+        self.formato=formato
         ## Paths
         # Path HDFS
         self.PATH_MODELO = os.path.join("/adv/modelos/", modelo)
         self.PATH=os.path.join(self.PATH_MODELO, "challenger")
         # Path Local
         self.TMP_PATH=os.path.join("/tmp/adv/DM/datastore/DS_sandbox", modelo)
         self.plataforma=plataforma
@@ -218,14 +223,17 @@
 
                 bq=self.bq,
 
                 spark=self.spark,
                 bucket=self.bucket,
 
                 formatofile_spark=self.formato)
+                
+                
+
 
     def BorrarTablasTemporales(self ):
 
         try:
             query=f"DROP TABLE IF EXISTS   " + self.qm.getNombreTabla(f"tmp_challenger_{self.modelo}_0")
             self.qm.execute_query(query)
             print("INFORMACION DE SEGUIMIENTO: DROP TABLA _0")
@@ -708,21 +716,18 @@
             self.qm.to_table(model_cvresults, "overwrite",  self.qm.getNombreTabla('tmp_challenger_' + self.modelo + '_metricas').replace('`', ''))
             print('Grabo Metricas -- overwrite')
 
 
         ### Save model
         # Seleccionamos el mejor modelo y lo guardamos para compararlo con el otros modelos para luego elegir el modelo ganador
         if self.GRABAR_BINARIOS:
-            print("intentando grabar")
-            print(type(cvModel3))
             if self.plataforma=="GCP":
                 cvModel3.write().overwrite().save(BINARIO+".bin")
                 print(os.popen(f"hdfs dfs -get -f {BINARIO}.bin ./"))
                 print(f"gsutil cp -r ./{BINARIO}.bin {self.gcs_path}")
-
                 print(os.popen(f"gsutil cp -r ./{BINARIO}.bin {self.gcs_path}/"))
             elif self.plataforma=="OP":
                 try:
                     # Crear carpeta HDFS
                     os.popen(f'hadoop fs -mkdir -p {self.PATH}')
                     # Guarda binario
                     assert BINARIO
@@ -1871,7 +1876,30 @@
             json_data=json.load(reader)
         return cls(**json_data)
 
     def json_dump(self):
         import json
         return json.dumps(self.__dict__)
 
+    def json_dump_nospark(self):
+            import json
+            import copy
+            todump=copy.copy(self)
+            todump.spark=None
+            todump.bq=None
+            todump.qm=None
+            return json.dumps(todump.__dict__)
+    
+    def reset_query_manager(self):
+        """Reconstruye el objeto Query_manager, deberia usarse en caso de que la clase sea instanciada via JSON
+        No tengo la mas palida idea de porque se lleva el nombre de la clase como parte del nombre del metodo... Pero asi y todo funciona"""
+        self.qm=query_manager(plataforma=self.plataforma,
+
+                gcp_project=self.gcp_project, ambiente=self.ambiente,
+                project_id=self.gcp_project, dataset_id=self.ambiente,
+
+                bq=self.bq,
+
+                spark=self.spark,
+                bucket=self.bucket,
+
+                formatofile_spark=self.formato)
```

### Comparing `challengerteco-0.1.3/PKG-INFO` & `challengerteco-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: challengerteco
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Eduardo Pagnone
 Author-email: mlopsaa@teco.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

