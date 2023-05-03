# Comparing `tmp/LHCbDIRAC-11.0.9.tar.gz` & `tmp/LHCbDIRAC-11.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LHCbDIRAC-11.0.9.tar", last modified: Wed May  3 05:56:13 2023, max compression
+gzip compressed data, was "LHCbDIRAC-11.1.0a1.tar", last modified: Wed Mar 22 15:37:57 2023, max compression
```

## Comparing `LHCbDIRAC-11.0.9.tar` & `LHCbDIRAC-11.1.0a1.tar`

### file list

```diff
@@ -1,544 +1,543 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.908000 LHCbDIRAC-11.0.9/
--rw-r--r--   0 root         (0) root         (0)     1809 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    32452 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2229 2023-05-03 05:56:13.908000 LHCbDIRAC-11.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1561 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/README.rst
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/lhcbdirac.cfg
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/pytest.ini
--rw-r--r--   0 root         (0) root         (0)    12534 2023-05-03 05:56:13.908000 LHCbDIRAC-11.0.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.816000 LHCbDIRAC-11.0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.828000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.828000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.828000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.832000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py
--rw-r--r--   0 root         (0) root         (0)     1726 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.832000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/test/
--rw-r--r--   0 root         (0) root         (0)     2457 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/__init__.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.832000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.832000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/
--rw-r--r--   0 root         (0) root         (0)    17746 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py
--rw-r--r--   0 root         (0) root         (0)    26536 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py
--rw-r--r--   0 root         (0) root         (0)    10573 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py
--rw-r--r--   0 root         (0) root         (0)    26244 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py
--rw-r--r--   0 root         (0) root         (0)    15013 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.832000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/
--rw-r--r--   0 root         (0) root         (0)    29898 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py
--rw-r--r--   0 root         (0) root         (0)    11739 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py
--rw-r--r--   0 root         (0) root         (0)    16950 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py
--rw-r--r--   0 root         (0) root         (0)    34287 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.832000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.836000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/
--rw-r--r--   0 root         (0) root         (0)    38737 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py
--rw-r--r--   0 root         (0) root         (0)    21163 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py
--rw-r--r--   0 root         (0) root         (0)    18511 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py
--rw-r--r--   0 root         (0) root         (0)    81682 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py
--rw-r--r--   0 root         (0) root         (0)    72062 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.836000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/
--rw-r--r--   0 root         (0) root         (0)     6316 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35269 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py
--rw-r--r--   0 root         (0) root         (0)      290 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.840000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/
--rw-r--r--   0 root         (0) root         (0)     2994 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py
--rw-r--r--   0 root         (0) root         (0)   241974 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py
--rw-r--r--   0 root         (0) root         (0)    12488 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py
--rw-r--r--   0 root         (0) root         (0)    16403 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py
--rw-r--r--   0 root         (0) root         (0)     4036 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py
--rwxr-xr-x   0 root         (0) root         (0)      842 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql
--rw-r--r--   0 root         (0) root         (0)    28034 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql
--rw-r--r--   0 root         (0) root         (0)     4705 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql
--rw-r--r--   0 root         (0) root         (0)    12638 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql
--rw-r--r--   0 root         (0) root         (0)    87437 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql
--rw-r--r--   0 root         (0) root         (0)    19607 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.840000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/
--rw-r--r--   0 root         (0) root         (0)    14458 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.840000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py
--rw-r--r--   0 root         (0) root         (0)     8490 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py
--rw-r--r--   0 root         (0) root         (0)     5893 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py
--rw-r--r--   0 root         (0) root         (0)   294418 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.840000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/
--rw-r--r--   0 root         (0) root         (0)    87960 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.844000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.844000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/
--rw-r--r--   0 root         (0) root         (0)     1410 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     1151 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13131 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.844000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/
--rw-r--r--   0 root         (0) root         (0)     1157 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py
--rw-r--r--   0 root         (0) root         (0)    28818 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd
--rw-r--r--   0 root         (0) root         (0)      688 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.844000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/
--rw-r--r--   0 root         (0) root         (0)     7892 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1155 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py
--rwxr-xr-x   0 root         (0) root         (0)     3567 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py
--rwxr-xr-x   0 root         (0) root         (0)     4682 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py
--rwxr-xr-x   0 root         (0) root         (0)     4660 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py
--rwxr-xr-x   0 root         (0) root         (0)     1704 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py
--rwxr-xr-x   0 root         (0) root         (0)     2291 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py
--rwxr-xr-x   0 root         (0) root         (0)     1954 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py
--rwxr-xr-x   0 root         (0) root         (0)     1479 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py
--rwxr-xr-x   0 root         (0) root         (0)     1799 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py
--rwxr-xr-x   0 root         (0) root         (0)     9413 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py
--rwxr-xr-x   0 root         (0) root         (0)     1610 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py
--rwxr-xr-x   0 root         (0) root         (0)     2009 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py
--rwxr-xr-x   0 root         (0) root         (0)     2128 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py
--rwxr-xr-x   0 root         (0) root         (0)     2006 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py
--rwxr-xr-x   0 root         (0) root         (0)     1871 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py
--rwxr-xr-x   0 root         (0) root         (0)     2442 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py
--rwxr-xr-x   0 root         (0) root         (0)     1919 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py
--rwxr-xr-x   0 root         (0) root         (0)     2460 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py
--rwxr-xr-x   0 root         (0) root         (0)     1791 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py
--rwxr-xr-x   0 root         (0) root         (0)     1665 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py
--rwxr-xr-x   0 root         (0) root         (0)     2154 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py
--rwxr-xr-x   0 root         (0) root         (0)     6303 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py
--rwxr-xr-x   0 root         (0) root         (0)     3242 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py
--rwxr-xr-x   0 root         (0) root         (0)     3021 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py
--rwxr-xr-x   0 root         (0) root         (0)     2714 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py
--rwxr-xr-x   0 root         (0) root         (0)     3374 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py
--rwxr-xr-x   0 root         (0) root         (0)     2247 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py
--rwxr-xr-x   0 root         (0) root         (0)     3172 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py
--rwxr-xr-x   0 root         (0) root         (0)     1597 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py
--rwxr-xr-x   0 root         (0) root         (0)     2278 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py
--rwxr-xr-x   0 root         (0) root         (0)     7961 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py
--rwxr-xr-x   0 root         (0) root         (0)     3047 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py
--rwxr-xr-x   0 root         (0) root         (0)    10570 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py
--rwxr-xr-x   0 root         (0) root         (0)     2681 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py
--rwxr-xr-x   0 root         (0) root         (0)     2443 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py
--rwxr-xr-x   0 root         (0) root         (0)     4711 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py
--rwxr-xr-x   0 root         (0) root         (0)     2580 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py
--rwxr-xr-x   0 root         (0) root         (0)     2052 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/
--rw-r--r--   0 root         (0) root         (0)     5412 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/
--rw-r--r--   0 root         (0) root         (0)     9187 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/scripts/
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4493 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.852000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.856000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/
--rw-r--r--   0 root         (0) root         (0)     4957 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/File.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py
--rw-r--r--   0 root         (0) root         (0)    18183 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/HTML.py
--rw-r--r--   0 root         (0) root         (0)     4845 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/LogErr.py
--rw-r--r--   0 root         (0) root         (0)     6813 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py
--rw-r--r--   0 root         (0) root         (0)     1700 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py
--rw-r--r--   0 root         (0) root         (0)    14189 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/ProductionData.py
--rw-r--r--   0 root         (0) root         (0)     4667 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/ResolveSE.py
--rw-r--r--   0 root         (0) root         (0)    11077 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/RunApplication.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/XMLErr.py
--rw-r--r--   0 root         (0) root         (0)    23504 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.856000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/
--rw-r--r--   0 root         (0) root         (0)     5589 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py
--rw-r--r--   0 root         (0) root         (0)    21804 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.856000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4387 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_architecture.py
--rwxr-xr-x   0 root         (0) root         (0)     1972 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py
--rwxr-xr-x   0 root         (0) root         (0)     5967 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py
--rwxr-xr-x   0 root         (0) root         (0)     2958 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py
--rwxr-xr-x   0 root         (0) root         (0)     2352 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py
--rwxr-xr-x   0 root         (0) root         (0)     8040 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_loop.py
--rwxr-xr-x   0 root         (0) root         (0)     1601 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.860000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.860000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/
--rw-r--r--   0 root         (0) root         (0)    14583 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py
--rw-r--r--   0 root         (0) root         (0)    10773 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.860000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-r--r--   0 root         (0) root         (0)     4346 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    64458 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py
--rw-r--r--   0 root         (0) root         (0)    36145 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py
--rw-r--r--   0 root         (0) root         (0)    29277 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py
--rw-r--r--   0 root         (0) root         (0)     9366 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/
--rw-r--r--   0 root         (0) root         (0)    24689 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py
--rw-r--r--   0 root         (0) root         (0)    21905 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py
--rw-r--r--   0 root         (0) root         (0)    61707 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py
--rw-r--r--   0 root         (0) root         (0)    24772 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py
--rwxr-xr-x   0 root         (0) root         (0)    20156 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py
--rwxr-xr-x   0 root         (0) root         (0)    27390 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py
--rw-r--r--   0 root         (0) root         (0)    89823 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/test/
--rw-r--r--   0 root         (0) root         (0)     6621 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/
--rw-r--r--   0 root         (0) root         (0)    15908 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql
--rw-r--r--   0 root         (0) root         (0)    52321 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/
--rw-r--r--   0 root         (0) root         (0)     3136 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py
--rw-r--r--   0 root         (0) root         (0)     6917 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py
--rw-r--r--   0 root         (0) root         (0)    16278 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py
--rw-r--r--   0 root         (0) root         (0)    11871 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Utilities/
--rw-r--r--   0 root         (0) root         (0)     2903 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.864000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/
--rw-r--r--   0 root         (0) root         (0)     5112 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.868000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2049 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py
--rwxr-xr-x   0 root         (0) root         (0)     3160 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py
--rwxr-xr-x   0 root         (0) root         (0)     3026 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py
--rwxr-xr-x   0 root         (0) root         (0)     3631 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py
--rwxr-xr-x   0 root         (0) root         (0)     3885 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py
--rwxr-xr-x   0 root         (0) root         (0)     4627 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py
--rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py
--rwxr-xr-x   0 root         (0) root         (0)    10422 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py
--rwxr-xr-x   0 root         (0) root         (0)     2470 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py
--rwxr-xr-x   0 root         (0) root         (0)     5753 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py
--rwxr-xr-x   0 root         (0) root         (0)     1684 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py
--rwxr-xr-x   0 root         (0) root         (0)     2409 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py
--rwxr-xr-x   0 root         (0) root         (0)     1684 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py
--rwxr-xr-x   0 root         (0) root         (0)     1858 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py
--rwxr-xr-x   0 root         (0) root         (0)     2455 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py
--rwxr-xr-x   0 root         (0) root         (0)     1993 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py
--rwxr-xr-x   0 root         (0) root         (0)     2159 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py
--rwxr-xr-x   0 root         (0) root         (0)     1752 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py
--rwxr-xr-x   0 root         (0) root         (0)     1733 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py
--rwxr-xr-x   0 root         (0) root         (0)     1744 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py
--rwxr-xr-x   0 root         (0) root         (0)     2171 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py
--rwxr-xr-x   0 root         (0) root         (0)     2482 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py
--rwxr-xr-x   0 root         (0) root         (0)     1953 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py
--rwxr-xr-x   0 root         (0) root         (0)     1874 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py
--rwxr-xr-x   0 root         (0) root         (0)     1851 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py
--rwxr-xr-x   0 root         (0) root         (0)     1873 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py
--rwxr-xr-x   0 root         (0) root         (0)    21939 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.872000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.872000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/DB/
--rw-r--r--   0 root         (0) root         (0)     2582 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.872000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.872000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/
--rwxr-xr-x   0 root         (0) root         (0)    42816 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py
--rw-r--r--   0 root         (0) root         (0)    40085 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/DiracProduction.py
--rwxr-xr-x   0 root         (0) root         (0)    26562 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/LHCbJob.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.872000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/test/
--rw-r--r--   0 root         (0) root         (0)     1703 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.876000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1145 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py
--rwxr-xr-x   0 root         (0) root         (0)     2841 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py
--rwxr-xr-x   0 root         (0) root         (0)     1718 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py
--rwxr-xr-x   0 root         (0) root         (0)     2184 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py
--rwxr-xr-x   0 root         (0) root         (0)     2058 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py
--rwxr-xr-x   0 root         (0) root         (0)     2968 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py
--rwxr-xr-x   0 root         (0) root         (0)     1999 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py
--rwxr-xr-x   0 root         (0) root         (0)     1887 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py
--rwxr-xr-x   0 root         (0) root         (0)     1783 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py
--rwxr-xr-x   0 root         (0) root         (0)     1824 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py
--rwxr-xr-x   0 root         (0) root         (0)     1835 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py
--rwxr-xr-x   0 root         (0) root         (0)     1718 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py
--rwxr-xr-x   0 root         (0) root         (0)     1967 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py
--rwxr-xr-x   0 root         (0) root         (0)     2859 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py
--rwxr-xr-x   0 root         (0) root         (0)     1777 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py
--rwxr-xr-x   0 root         (0) root         (0)     1726 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.876000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.876000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/
--rw-r--r--   0 root         (0) root         (0)    12252 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py
--rw-r--r--   0 root         (0) root         (0)     9490 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py
--rw-r--r--   0 root         (0) root         (0)    27726 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py
--rw-r--r--   0 root         (0) root         (0)    13549 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py
--rw-r--r--   0 root         (0) root         (0)    44203 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py
--rw-r--r--   0 root         (0) root         (0)     4656 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py
--rwxr-xr-x   0 root         (0) root         (0)      858 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.876000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/
--rw-r--r--   0 root         (0) root         (0)    10086 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py
--rw-r--r--   0 root         (0) root         (0)    16063 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py
--rw-r--r--   0 root         (0) root         (0)     9518 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.876000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/
--rw-r--r--   0 root         (0) root         (0)    11225 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py
--rw-r--r--   0 root         (0) root         (0)    38168 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py
--rw-r--r--   0 root         (0) root         (0)    36665 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py
--rw-r--r--   0 root         (0) root         (0)    44248 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py
--rwxr-xr-x   0 root         (0) root         (0)      859 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.880000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/
--rw-r--r--   0 root         (0) root         (0)     1344 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py
--rw-r--r--   0 root         (0) root         (0)    96754 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.880000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/
--rw-r--r--   0 root         (0) root         (0)    21033 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.sql
--rw-r--r--   0 root         (0) root         (0)     6783 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py
--rw-r--r--   0 root         (0) root         (0)     2328 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py
--rw-r--r--   0 root         (0) root         (0)     4152 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py
--rw-r--r--   0 root         (0) root         (0)     4335 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py
--rw-r--r--   0 root         (0) root         (0)    64737 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py
--rw-r--r--   0 root         (0) root         (0)     4189 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql
--rwxr-xr-x   0 root         (0) root         (0)      855 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/extra_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.880000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/
--rw-r--r--   0 root         (0) root         (0)    23625 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.880000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/
--rw-r--r--   0 root         (0) root         (0)     2271 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py
--rw-r--r--   0 root         (0) root         (0)    14126 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py
--rw-r--r--   0 root         (0) root         (0)    10794 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py
--rwxr-xr-x   0 root         (0) root         (0)      860 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.880000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/
--rw-r--r--   0 root         (0) root         (0)     2148 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.884000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/
--rw-r--r--   0 root         (0) root         (0)    15147 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py
--rw-r--r--   0 root         (0) root         (0)     9682 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py
--rw-r--r--   0 root         (0) root         (0)    15739 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py
--rw-r--r--   0 root         (0) root         (0)    15012 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.884000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/
--rw-r--r--   0 root         (0) root         (0)     1056 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py
--rw-r--r--   0 root         (0) root         (0)    14092 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py
--rw-r--r--   0 root         (0) root         (0)     5772 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py
--rw-r--r--   0 root         (0) root         (0)     8957 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      852 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.884000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9788 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py
--rw-r--r--   0 root         (0) root         (0)     6964 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py
--rwxr-xr-x   0 root         (0) root         (0)    17423 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.884000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.884000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/
--rw-r--r--   0 root         (0) root         (0)     2980 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py
--rw-r--r--   0 root         (0) root         (0)     9616 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py
--rw-r--r--   0 root         (0) root         (0)     9662 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/
--rw-r--r--   0 root         (0) root         (0)     3837 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/DownHillPropagationPolicy.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py
--rw-r--r--   0 root         (0) root         (0)     5161 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/
--rw-r--r--   0 root         (0) root         (0)     8661 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py
--rw-r--r--   0 root         (0) root         (0)      843 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/test/
--rw-r--r--   0 root         (0) root         (0)    29006 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py
--rw-r--r--   0 root         (0) root         (0)     5037 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/
--rw-r--r--   0 root         (0) root         (0)     5223 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/test/
--rw-r--r--   0 root         (0) root         (0)     8294 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.888000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.892000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/
--rw-r--r--   0 root         (0) root         (0)    19361 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py
--rw-r--r--   0 root         (0) root         (0)    17711 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py
--rw-r--r--   0 root         (0) root         (0)    11910 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py
--rw-r--r--   0 root         (0) root         (0)    17686 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py
--rwxr-xr-x   0 root         (0) root         (0)     7081 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py
--rw-r--r--   0 root         (0) root         (0)    94443 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py
--rwxr-xr-x   0 root         (0) root         (0)     5925 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py
--rwxr-xr-x   0 root         (0) root         (0)      852 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.892000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/
--rw-r--r--   0 root         (0) root         (0)    14547 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py
--rw-r--r--   0 root         (0) root         (0)    14181 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py
--rw-r--r--   0 root         (0) root         (0)    20751 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.892000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.892000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/
--rw-r--r--   0 root         (0) root         (0)     3791 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py
--rw-r--r--   0 root         (0) root         (0)     5035 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2640 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py
--rw-r--r--   0 root         (0) root         (0)     5821 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py
--rw-r--r--   0 root         (0) root         (0)    95672 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py
--rwxr-xr-x   0 root         (0) root         (0)      934 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.892000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/test/
--rw-r--r--   0 root         (0) root         (0)    13054 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.896000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/
--rwxr-xr-x   0 root         (0) root         (0)    34614 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py
--rwxr-xr-x   0 root         (0) root         (0)     4120 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql
--rwxr-xr-x   0 root         (0) root         (0)      930 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.896000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/
--rw-r--r--   0 root         (0) root         (0)     1306 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py
--rw-r--r--   0 root         (0) root         (0)    13013 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py
--rwxr-xr-x   0 root         (0) root         (0)      935 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.896000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/
--rw-r--r--   0 root         (0) root         (0)     5149 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py
--rw-r--r--   0 root         (0) root         (0)    86398 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py
--rw-r--r--   0 root         (0) root         (0)     2604 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.896000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/test/
--rw-r--r--   0 root         (0) root         (0)     3310 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py
--rwxr-xr-x   0 root         (0) root         (0)      927 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.900000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9400 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py
--rwxr-xr-x   0 root         (0) root         (0)    16558 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py
--rwxr-xr-x   0 root         (0) root         (0)     2461 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py
--rwxr-xr-x   0 root         (0) root         (0)     6835 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py
--rwxr-xr-x   0 root         (0) root         (0)     6893 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py
--rwxr-xr-x   0 root         (0) root         (0)     1619 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py
--rwxr-xr-x   0 root         (0) root         (0)    21895 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4906 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py
--rwxr-xr-x   0 root         (0) root         (0)     1773 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py
--rwxr-xr-x   0 root         (0) root         (0)     1703 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py
--rwxr-xr-x   0 root         (0) root         (0)     3127 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py
--rwxr-xr-x   0 root         (0) root         (0)     5972 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py
--rwxr-xr-x   0 root         (0) root         (0)     2651 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py
--rwxr-xr-x   0 root         (0) root         (0)     5057 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py
--rw-r--r--   0 root         (0) root         (0)     3621 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py
--rwxr-xr-x   0 root         (0) root         (0)     5390 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py
--rwxr-xr-x   0 root         (0) root         (0)     2734 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.900000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/
--rw-r--r--   0 root         (0) root         (0)     7856 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py
--rw-r--r--   0 root         (0) root         (0)    10256 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py
--rw-r--r--   0 root         (0) root         (0)    19749 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py
--rw-r--r--   0 root         (0) root         (0)     6567 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py
--rw-r--r--   0 root         (0) root         (0)     5744 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/FileUsage.py
--rwxr-xr-x   0 root         (0) root         (0)     8725 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/MergeMDF.py
--rw-r--r--   0 root         (0) root         (0)    47119 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py
--rw-r--r--   0 root         (0) root         (0)     9180 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py
--rw-r--r--   0 root         (0) root         (0)     4732 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py
--rw-r--r--   0 root         (0) root         (0)    16006 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UploadMC.py
--rw-r--r--   0 root         (0) root         (0)    21211 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py
--rw-r--r--   0 root         (0) root         (0)    15381 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py
--rwxr-xr-x   0 root         (0) root         (0)      838 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12294 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/mock_Commons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/
--rw-r--r--   0 root         (0) root         (0)     2784 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py
--rw-r--r--   0 root         (0) root         (0)    10499 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbAnalyse.py
--rw-r--r--   0 root         (0) root         (0)     5537 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py
--rw-r--r--   0 root         (0) root         (0)    16821 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py
--rw-r--r--   0 root         (0) root         (0)    19227 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Others.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py
--rw-r--r--   0 root         (0) root         (0)    10434 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Uploads.py
--rw-r--r--   0 root         (0) root         (0)     9223 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/Test_Modules_AnalyseFileAccess.py
--rw-r--r--   0 root         (0) root         (0)     2518 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/pool_xml_catalog.xml
--rw-r--r--   0 root         (0) root         (0)     2185 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/summary.xml
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/
--rw-r--r--   0 root         (0) root         (0)     5420 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/
--rw-r--r--   0 root         (0) root         (0)     1281 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.904000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Service/
--rw-r--r--   0 root         (0) root         (0)    15982 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Service/WMSSecureGWHandler.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Service/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.908000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.908000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Utilities/
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14784 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py
--rw-r--r--   0 root         (0) root         (0)     5202 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Workflow.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-03 05:55:52.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:56:13.828000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2229 2023-05-03 05:56:13.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28366 2023-05-03 05:56:13.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:56:13.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    11222 2023-05-03 05:56:13.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:56:12.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-03 05:56:13.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 05:56:13.000000 LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    32452 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      166 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2231 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/README.rst
+-rw-r--r--   0 root         (0) root         (0)       84 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/lhcbdirac.cfg
+-rw-r--r--   0 root         (0) root         (0)      472 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      131 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)    12529 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.956000 LHCbDIRAC-11.1.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.964000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/test/
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/
+-rw-r--r--   0 root         (0) root         (0)    17746 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py
+-rw-r--r--   0 root         (0) root         (0)    26536 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py
+-rw-r--r--   0 root         (0) root         (0)    10573 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py
+-rw-r--r--   0 root         (0) root         (0)    26244 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py
+-rw-r--r--   0 root         (0) root         (0)    15013 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/
+-rw-r--r--   0 root         (0) root         (0)    29898 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py
+-rw-r--r--   0 root         (0) root         (0)    11739 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py
+-rw-r--r--   0 root         (0) root         (0)    16950 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py
+-rw-r--r--   0 root         (0) root         (0)    34287 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py
+-rw-r--r--   0 root         (0) root         (0)      850 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.972000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py
+-rw-r--r--   0 root         (0) root         (0)    21163 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py
+-rw-r--r--   0 root         (0) root         (0)    18511 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py
+-rw-r--r--   0 root         (0) root         (0)    81682 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py
+-rw-r--r--   0 root         (0) root         (0)    72062 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py
+-rw-r--r--   0 root         (0) root         (0)      846 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.972000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/
+-rw-r--r--   0 root         (0) root         (0)     6316 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35269 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py
+-rw-r--r--   0 root         (0) root         (0)      290 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.972000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py
+-rw-r--r--   0 root         (0) root         (0)   241974 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py
+-rw-r--r--   0 root         (0) root         (0)    12488 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py
+-rw-r--r--   0 root         (0) root         (0)    16403 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py
+-rwxr-xr-x   0 root         (0) root         (0)      842 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql
+-rw-r--r--   0 root         (0) root         (0)    28034 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql
+-rw-r--r--   0 root         (0) root         (0)    12638 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql
+-rw-r--r--   0 root         (0) root         (0)    87437 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql
+-rw-r--r--   0 root         (0) root         (0)    19607 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.972000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/
+-rw-r--r--   0 root         (0) root         (0)    14458 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.976000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py
+-rw-r--r--   0 root         (0) root         (0)     8490 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py
+-rw-r--r--   0 root         (0) root         (0)   294418 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.976000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/
+-rw-r--r--   0 root         (0) root         (0)    87960 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.976000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.976000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13131 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.976000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py
+-rw-r--r--   0 root         (0) root         (0)    28818 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd
+-rw-r--r--   0 root         (0) root         (0)      688 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.980000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/
+-rw-r--r--   0 root         (0) root         (0)     7892 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py
+-rw-r--r--   0 root         (0) root         (0)      845 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1155 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py
+-rwxr-xr-x   0 root         (0) root         (0)     3567 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py
+-rwxr-xr-x   0 root         (0) root         (0)     4682 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py
+-rwxr-xr-x   0 root         (0) root         (0)     4660 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py
+-rwxr-xr-x   0 root         (0) root         (0)     1704 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py
+-rwxr-xr-x   0 root         (0) root         (0)     2291 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py
+-rwxr-xr-x   0 root         (0) root         (0)     1954 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py
+-rwxr-xr-x   0 root         (0) root         (0)     1479 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py
+-rwxr-xr-x   0 root         (0) root         (0)     1799 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py
+-rwxr-xr-x   0 root         (0) root         (0)     9413 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py
+-rwxr-xr-x   0 root         (0) root         (0)     1610 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py
+-rwxr-xr-x   0 root         (0) root         (0)     2009 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py
+-rwxr-xr-x   0 root         (0) root         (0)     2128 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py
+-rwxr-xr-x   0 root         (0) root         (0)     2006 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     2442 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py
+-rwxr-xr-x   0 root         (0) root         (0)     1919 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py
+-rwxr-xr-x   0 root         (0) root         (0)     2460 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py
+-rwxr-xr-x   0 root         (0) root         (0)     1791 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py
+-rwxr-xr-x   0 root         (0) root         (0)     1665 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py
+-rwxr-xr-x   0 root         (0) root         (0)     2154 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py
+-rwxr-xr-x   0 root         (0) root         (0)     6303 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     3242 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py
+-rwxr-xr-x   0 root         (0) root         (0)     3021 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py
+-rwxr-xr-x   0 root         (0) root         (0)     2714 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     3374 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py
+-rwxr-xr-x   0 root         (0) root         (0)     2247 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py
+-rwxr-xr-x   0 root         (0) root         (0)     3172 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py
+-rwxr-xr-x   0 root         (0) root         (0)     1597 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py
+-rwxr-xr-x   0 root         (0) root         (0)     2278 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     7961 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py
+-rwxr-xr-x   0 root         (0) root         (0)     3047 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py
+-rwxr-xr-x   0 root         (0) root         (0)    10570 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py
+-rwxr-xr-x   0 root         (0) root         (0)     2681 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     2443 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py
+-rwxr-xr-x   0 root         (0) root         (0)     4711 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py
+-rwxr-xr-x   0 root         (0) root         (0)     2580 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py
+-rwxr-xr-x   0 root         (0) root         (0)     2052 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/
+-rw-r--r--   0 root         (0) root         (0)     5412 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/
+-rw-r--r--   0 root         (0) root         (0)     9187 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/scripts/
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4493 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.984000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.988000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/File.py
+-rw-r--r--   0 root         (0) root         (0)     2856 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py
+-rw-r--r--   0 root         (0) root         (0)    18183 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/HTML.py
+-rw-r--r--   0 root         (0) root         (0)     4845 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/LogErr.py
+-rw-r--r--   0 root         (0) root         (0)     6813 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py
+-rw-r--r--   0 root         (0) root         (0)    14189 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/ProductionData.py
+-rw-r--r--   0 root         (0) root         (0)     4667 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/ResolveSE.py
+-rw-r--r--   0 root         (0) root         (0)    10929 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/RunApplication.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/XMLErr.py
+-rw-r--r--   0 root         (0) root         (0)    23504 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.988000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py
+-rw-r--r--   0 root         (0) root         (0)    21804 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.988000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4387 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_architecture.py
+-rwxr-xr-x   0 root         (0) root         (0)     1972 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py
+-rwxr-xr-x   0 root         (0) root         (0)     5967 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py
+-rwxr-xr-x   0 root         (0) root         (0)     2958 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py
+-rwxr-xr-x   0 root         (0) root         (0)     2352 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     8040 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_loop.py
+-rwxr-xr-x   0 root         (0) root         (0)     1601 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.988000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.988000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/
+-rw-r--r--   0 root         (0) root         (0)    14583 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py
+-rw-r--r--   0 root         (0) root         (0)    10773 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.988000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    64458 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py
+-rw-r--r--   0 root         (0) root         (0)    36145 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py
+-rw-r--r--   0 root         (0) root         (0)    29277 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py
+-rw-r--r--   0 root         (0) root         (0)     9366 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/
+-rw-r--r--   0 root         (0) root         (0)    24689 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py
+-rw-r--r--   0 root         (0) root         (0)    21905 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py
+-rw-r--r--   0 root         (0) root         (0)    61707 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py
+-rw-r--r--   0 root         (0) root         (0)    24772 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py
+-rwxr-xr-x   0 root         (0) root         (0)    20156 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py
+-rwxr-xr-x   0 root         (0) root         (0)    27390 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py
+-rw-r--r--   0 root         (0) root         (0)    89823 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/test/
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/
+-rw-r--r--   0 root         (0) root         (0)    15908 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql
+-rw-r--r--   0 root         (0) root         (0)    52321 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql
+-rw-r--r--   0 root         (0) root         (0)      849 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py
+-rw-r--r--   0 root         (0) root         (0)     6917 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py
+-rw-r--r--   0 root         (0) root         (0)    16278 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py
+-rw-r--r--   0 root         (0) root         (0)      854 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Utilities/
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.992000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/
+-rw-r--r--   0 root         (0) root         (0)     5112 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.996000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2049 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py
+-rwxr-xr-x   0 root         (0) root         (0)     3160 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py
+-rwxr-xr-x   0 root         (0) root         (0)     3026 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py
+-rwxr-xr-x   0 root         (0) root         (0)     3631 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py
+-rwxr-xr-x   0 root         (0) root         (0)     3885 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py
+-rwxr-xr-x   0 root         (0) root         (0)     4627 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py
+-rwxr-xr-x   0 root         (0) root         (0)     2424 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py
+-rwxr-xr-x   0 root         (0) root         (0)    10422 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py
+-rwxr-xr-x   0 root         (0) root         (0)     2470 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py
+-rwxr-xr-x   0 root         (0) root         (0)     5753 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py
+-rwxr-xr-x   0 root         (0) root         (0)     1684 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py
+-rwxr-xr-x   0 root         (0) root         (0)     2409 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py
+-rwxr-xr-x   0 root         (0) root         (0)     1684 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py
+-rwxr-xr-x   0 root         (0) root         (0)     1858 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py
+-rwxr-xr-x   0 root         (0) root         (0)     2455 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py
+-rwxr-xr-x   0 root         (0) root         (0)     1993 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py
+-rwxr-xr-x   0 root         (0) root         (0)     2159 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py
+-rwxr-xr-x   0 root         (0) root         (0)     1752 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py
+-rwxr-xr-x   0 root         (0) root         (0)     1733 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py
+-rwxr-xr-x   0 root         (0) root         (0)     1744 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     2171 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py
+-rwxr-xr-x   0 root         (0) root         (0)     2482 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py
+-rwxr-xr-x   0 root         (0) root         (0)     1953 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py
+-rwxr-xr-x   0 root         (0) root         (0)     1874 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py
+-rwxr-xr-x   0 root         (0) root         (0)     1851 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py
+-rwxr-xr-x   0 root         (0) root         (0)     1873 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py
+-rwxr-xr-x   0 root         (0) root         (0)    21939 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.996000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.996000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/DB/
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.996000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/
+-rwxr-xr-x   0 root         (0) root         (0)    42816 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py
+-rw-r--r--   0 root         (0) root         (0)    40085 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/DiracProduction.py
+-rwxr-xr-x   0 root         (0) root         (0)    26617 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/LHCbJob.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/test/
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1145 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py
+-rwxr-xr-x   0 root         (0) root         (0)     2841 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py
+-rwxr-xr-x   0 root         (0) root         (0)     1718 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py
+-rwxr-xr-x   0 root         (0) root         (0)     2184 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     2058 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     2968 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py
+-rwxr-xr-x   0 root         (0) root         (0)     1999 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py
+-rwxr-xr-x   0 root         (0) root         (0)     1887 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     1783 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py
+-rwxr-xr-x   0 root         (0) root         (0)     1824 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py
+-rwxr-xr-x   0 root         (0) root         (0)     1835 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     1718 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py
+-rwxr-xr-x   0 root         (0) root         (0)     1967 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py
+-rwxr-xr-x   0 root         (0) root         (0)     2859 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py
+-rwxr-xr-x   0 root         (0) root         (0)     1777 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py
+-rwxr-xr-x   0 root         (0) root         (0)     1726 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/
+-rw-r--r--   0 root         (0) root         (0)    12252 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py
+-rw-r--r--   0 root         (0) root         (0)     9490 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py
+-rw-r--r--   0 root         (0) root         (0)    27726 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py
+-rw-r--r--   0 root         (0) root         (0)    13549 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py
+-rw-r--r--   0 root         (0) root         (0)    44203 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py
+-rw-r--r--   0 root         (0) root         (0)     4656 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py
+-rwxr-xr-x   0 root         (0) root         (0)      858 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/
+-rw-r--r--   0 root         (0) root         (0)    10086 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py
+-rw-r--r--   0 root         (0) root         (0)    16063 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py
+-rw-r--r--   0 root         (0) root         (0)     9518 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.004000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/
+-rw-r--r--   0 root         (0) root         (0)     9833 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py
+-rw-r--r--   0 root         (0) root         (0)    38168 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py
+-rw-r--r--   0 root         (0) root         (0)    36665 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py
+-rw-r--r--   0 root         (0) root         (0)    44248 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py
+-rwxr-xr-x   0 root         (0) root         (0)      859 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.004000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py
+-rw-r--r--   0 root         (0) root         (0)    96754 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.004000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/
+-rw-r--r--   0 root         (0) root         (0)    14015 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py
+-rw-r--r--   0 root         (0) root         (0)      198 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.sql
+-rw-r--r--   0 root         (0) root         (0)     6445 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py
+-rw-r--r--   0 root         (0) root         (0)     4152 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py
+-rw-r--r--   0 root         (0) root         (0)    64737 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py
+-rw-r--r--   0 root         (0) root         (0)     4189 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql
+-rwxr-xr-x   0 root         (0) root         (0)      855 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.004000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/
+-rw-r--r--   0 root         (0) root         (0)    20309 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.004000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py
+-rw-r--r--   0 root         (0) root         (0)    14126 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py
+-rw-r--r--   0 root         (0) root         (0)    10009 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py
+-rwxr-xr-x   0 root         (0) root         (0)      860 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.004000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/
+-rw-r--r--   0 root         (0) root         (0)    15147 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py
+-rw-r--r--   0 root         (0) root         (0)     9682 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py
+-rw-r--r--   0 root         (0) root         (0)    15739 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py
+-rw-r--r--   0 root         (0) root         (0)    15012 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py
+-rw-r--r--   0 root         (0) root         (0)    14109 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py
+-rw-r--r--   0 root         (0) root         (0)     8957 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      852 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py
+-rwxr-xr-x   0 root         (0) root         (0)    17423 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py
+-rw-r--r--   0 root         (0) root         (0)     8808 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py
+-rw-r--r--   0 root         (0) root         (0)     9662 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      222 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/DownHillPropagationPolicy.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py
+-rw-r--r--   0 root         (0) root         (0)      846 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.008000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/
+-rw-r--r--   0 root         (0) root         (0)     8661 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/test/
+-rw-r--r--   0 root         (0) root         (0)    29006 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py
+-rw-r--r--   0 root         (0) root         (0)     5037 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/
+-rw-r--r--   0 root         (0) root         (0)     5223 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/test/
+-rw-r--r--   0 root         (0) root         (0)     8294 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/
+-rw-r--r--   0 root         (0) root         (0)    19361 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py
+-rw-r--r--   0 root         (0) root         (0)    17711 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py
+-rw-r--r--   0 root         (0) root         (0)    17686 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py
+-rwxr-xr-x   0 root         (0) root         (0)     7081 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py
+-rw-r--r--   0 root         (0) root         (0)    94443 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     5925 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py
+-rwxr-xr-x   0 root         (0) root         (0)      852 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/
+-rw-r--r--   0 root         (0) root         (0)    14547 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py
+-rw-r--r--   0 root         (0) root         (0)    14181 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py
+-rw-r--r--   0 root         (0) root         (0)    20751 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.012000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.016000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/
+-rw-r--r--   0 root         (0) root         (0)     3791 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py
+-rw-r--r--   0 root         (0) root         (0)    95672 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py
+-rwxr-xr-x   0 root         (0) root         (0)      934 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.016000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/test/
+-rw-r--r--   0 root         (0) root         (0)    13054 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.016000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/
+-rwxr-xr-x   0 root         (0) root         (0)    34614 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py
+-rwxr-xr-x   0 root         (0) root         (0)     4120 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql
+-rwxr-xr-x   0 root         (0) root         (0)      930 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.016000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py
+-rw-r--r--   0 root         (0) root         (0)    13013 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py
+-rwxr-xr-x   0 root         (0) root         (0)      935 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.016000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py
+-rw-r--r--   0 root         (0) root         (0)    86398 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py
+-rw-r--r--   0 root         (0) root         (0)     2604 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.016000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/test/
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py
+-rwxr-xr-x   0 root         (0) root         (0)      927 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.020000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9400 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py
+-rwxr-xr-x   0 root         (0) root         (0)    16558 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py
+-rwxr-xr-x   0 root         (0) root         (0)     2461 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py
+-rwxr-xr-x   0 root         (0) root         (0)     6835 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py
+-rwxr-xr-x   0 root         (0) root         (0)     6893 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py
+-rwxr-xr-x   0 root         (0) root         (0)     1619 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py
+-rwxr-xr-x   0 root         (0) root         (0)    21895 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4906 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     1773 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py
+-rwxr-xr-x   0 root         (0) root         (0)     1703 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py
+-rwxr-xr-x   0 root         (0) root         (0)     3127 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py
+-rwxr-xr-x   0 root         (0) root         (0)     5972 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py
+-rwxr-xr-x   0 root         (0) root         (0)     2651 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py
+-rwxr-xr-x   0 root         (0) root         (0)     5057 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py
+-rwxr-xr-x   0 root         (0) root         (0)     5390 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py
+-rwxr-xr-x   0 root         (0) root         (0)     2734 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.020000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.020000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/
+-rw-r--r--   0 root         (0) root         (0)     7856 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py
+-rw-r--r--   0 root         (0) root         (0)    10256 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py
+-rw-r--r--   0 root         (0) root         (0)    19749 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py
+-rw-r--r--   0 root         (0) root         (0)     6567 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/FileUsage.py
+-rwxr-xr-x   0 root         (0) root         (0)     8725 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/MergeMDF.py
+-rw-r--r--   0 root         (0) root         (0)    47119 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py
+-rw-r--r--   0 root         (0) root         (0)     9180 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py
+-rw-r--r--   0 root         (0) root         (0)    16006 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UploadMC.py
+-rw-r--r--   0 root         (0) root         (0)    21211 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py
+-rwxr-xr-x   0 root         (0) root         (0)      838 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12294 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/mock_Commons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py
+-rw-r--r--   0 root         (0) root         (0)    10499 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbAnalyse.py
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py
+-rw-r--r--   0 root         (0) root         (0)    16821 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py
+-rw-r--r--   0 root         (0) root         (0)    19227 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Others.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Uploads.py
+-rw-r--r--   0 root         (0) root         (0)     9223 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/Test_Modules_AnalyseFileAccess.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/pool_xml_catalog.xml
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/summary.xml
+-rw-r--r--   0 root         (0) root         (0)      955 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py
+-rw-r--r--   0 root         (0) root         (0)      848 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql
+-rw-r--r--   0 root         (0) root         (0)      853 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Service/
+-rw-r--r--   0 root         (0) root         (0)    15982 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Service/WMSSecureGWHandler.py
+-rw-r--r--   0 root         (0) root         (0)      858 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:57.024000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Utilities/
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14784 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Workflow.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-03-22 15:37:40.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:37:56.968000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2231 2023-03-22 15:37:56.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28308 2023-03-22 15:37:56.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 15:37:56.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    11222 2023-03-22 15:37:56.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 15:37:55.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      199 2023-03-22 15:37:56.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-03-22 15:37:56.000000 LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/top_level.txt
```

### Comparing `LHCbDIRAC-11.0.9/CONTRIBUTING.md` & `LHCbDIRAC-11.1.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/LICENSE` & `LHCbDIRAC-11.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/PKG-INFO` & `LHCbDIRAC-11.1.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LHCbDIRAC
-Version: 11.0.9
+Version: 11.1.0a1
 Summary: LHCbDIRAC is the LHCb extension of DIRAC
 Home-page: https://gitlab.cern.ch/lhcb-dirac/LHCbDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LHCbDIRAC-11.0.9/README.rst` & `LHCbDIRAC-11.1.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/setup.cfg` & `LHCbDIRAC-11.1.0a1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 * = ConfigTemplate.cfg, *.sql
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 server = 
-	oracledb <1.3
+	oracledb
 	DIRAC[server]
 	psutil
 	stomp.py
 	suds
 testing = 
 	mock
 	Pillow
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/Client/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/AccountingSystem/private/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/AccountingSystem/private/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/File.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/File.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,18 +60,18 @@
             raise TypeError("Expected List")
         if not len(lfns):
             self.log.warn("No file generated: was expecting a non-empty list")
             raise ValueError("list empty")
 
         try:
             persistency = persistency.upper()
-            # Create a fake LFN->PFN dictionary to give the persistency
-            fakePfns = dict.fromkeys(lfns, {"pfntype": persistency})
         except AttributeError:
-            fakePfns = None
+            pass
 
+        # Create a fake LFN->PFN dictionary to give the persistency
+        fakePfns = dict.fromkeys(lfns, {"pfntype": persistency})
         script = LHCB_BKKDBClient().writeJobOptions(
             lfns, optionsFile=self.fileName, catalog=self.xmlcatalog_file, savePfn=fakePfns
         )
         self.log.info(f"Created Ganga data file {self.fileName}")
 
         return script
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/HTML.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/HTML.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/LogErr.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/LogErr.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/ProductionData.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/ProductionData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/ResolveSE.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/RunApplication.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/RunApplication.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 ###############################################################################
 """Utility for invoking running LHCb applications."""
 import asyncio
 import json
 import shlex
 import subprocess
 
-from DIRAC import gLogger, gConfig, S_OK
+from DIRAC import gLogger, S_OK
+from DIRAC.Core.Utilities import DErrno
 from DIRAC.WorkloadManagementSystem.Utilities.RemoteRunner import RemoteRunner
 from LHCbDIRAC.Workflow.Modules.ModulesUtilities import getEventsToProduce
 
 
 class LbRunError(RuntimeError):
     """Exception for lb-run errors."""
 
@@ -56,15 +57,14 @@
 
         self.prodConfFileName = "prodConf_{}_{}_{}_{}.json".format(
             self.applicationName,
             gaudiAppModule.production_id,
             gaudiAppModule.prod_job_id,
             gaudiAppModule.step_number,
         )
-        self.numberOfProcessors = gaudiAppModule.numberOfProcessors
         self.applicationLog = gaudiAppModule.applicationLog or "applicationLog.txt"
         self.stdError = gaudiAppModule.stdError or self.applicationLog
 
         # Sanity checks
         if not gaudiAppModule.stepInputData and self.applicationName.lower() != "gauss":
             raise RuntimeError("No MC, but no input data")
         if gaudiAppModule.TCK and gaudiAppModule.mcTCK:
@@ -72,15 +72,15 @@
 
         # Initialise the prodInfo object
         prodInfo = {
             "spec_version": 1,
             "application": {
                 "data_pkgs": [".".join(p) for p in gaudiAppModule.extraPackages],
                 "name": self.applicationName,
-                "number_of_processors": self.numberOfProcessors,
+                "number_of_processors": gaudiAppModule.numberOfProcessors,
                 "version": gaudiAppModule.applicationVersion,
             },
             "options": {},
             "db_tags": {},
             "input": {
                 "files": ["LFN:" + sid for sid in gaudiAppModule.stepInputData],
                 "first_event_number": firstEventNumberGauss,
@@ -180,36 +180,32 @@
             raise LHCbApplicationError(
                 f"{self.applicationName} {self.applicationVersion} exited with status {returncode}"
             )
 
         return S_OK((returncode, stdout, stderr))
 
     async def _runApp(self):
-        command = ["lb-prod-run", self.prodConfFileName, "--prmon", "--verbose"]
+        command = ["lb-prod-run", self.prodConfFileName, "--verbose"]
         if self.applicationName == "Gauss" and self.usePrmon:
             command = [self.prmonPath, "--json-summary", "./prmon_Gauss.json", "--"] + command
         self.log.notice("Running command", shlex.join(command))
 
         stdout = ""
         stderr = ""
-        if gConfig.getValue("/LocalSite/RemoteExecution", False):
-            remoteRunner = RemoteRunner(
-                gConfig.getValue("/LocalSite/Site"),
-                gConfig.getValue("/LocalSite/GridCE"),
-                gConfig.getValue("/LocalSite/CEQueue"),
-            )
-            outputDict = remoteRunner.execute(shlex.join(command), numberOfProcessors=self.numberOfProcessors)
-            if not outputDict["OK"]:
-                returncode = outputDict["Errno"]
-                stderr = outputDict["Message"]
-            else:
+        remoteRunner = RemoteRunner()
+        if remoteRunner.is_remote_execution():
+            outputDict = remoteRunner.execute(shlex.join(command))
+            if outputDict["OK"]:
                 returncode, stdout, stderr = outputDict["Value"]
-
-            self._handleRemoteOutput(stdout, self.applicationLog)
-            self._handleRemoteOutput(stderr, self.stdError)
+                self._handleRemoteOutput(stdout, self.applicationLog)
+                self._handleRemoteOutput(stderr, self.stdError)
+            else:
+                # Sometimes Errno has not been purposely defined and is equal to 0
+                returncode = outputDict["Errno"] if outputDict["Errno"] != 0 else DErrno.ERESGEN
+                stderr = outputDict["Message"]
         else:
             proc = await asyncio.create_subprocess_exec(
                 *command,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             )
             stdout_fh = None
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/XMLErr.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/XMLErr.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_architecture.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_architecture.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/dirac_loop.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/dirac_loop.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/private/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/private/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/FrameworkSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/FrameworkSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/DiracProduction.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/DiracProduction.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/LHCbJob.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/LHCbJob.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,24 +595,26 @@
             if not res["OK"]:
                 return res
 
             typeVersions = res["Value"]
 
             if not typeVersions:
                 self.log.verbose("The requested files do not exist in the BKK")
+                typeVersion = ""
+
             else:
                 self.log.verbose(f"Found file types {typeVersions.values()} for LFNs: {list(typeVersions)}")
                 typeVersionsList = list(set(typeVersions.values()))
                 if len(typeVersionsList) == 1:
-                    persistencyType = typeVersionsList[0]
+                    typeVersion = typeVersionsList[0]
+                else:
+                    typeVersion = ""
 
         if persistencyType:
-            self._addParameter(
-                self.workflow, "persistency", "String", persistencyType, "Persistency type of the inputs"
-            )
+            self._addParameter(self.workflow, "persistency", "String", typeVersion, "Persistency type of the inputs")
 
         return S_OK()
 
     #############################################################################
 
     def setRunMetadata(self, runMetadataDict):
         """set the run metadata."""
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py`

 * *Files 18% similar despite different names*

```diff
@@ -109,47 +109,18 @@
         if url:
             self.setServer(url)
 
     def listAnalyses(self, *, at_time: Opt[datetime] = None):
         """Return the mapping of known WGs to analyses
 
         :param at_time: The datetime at which this query should be ran, defaults to now
-        :returns: ``dict`` mapping the WG name to a list of analyses
+        :returns: `dict` mapping the WG name to a list of analyses
         """
         return self.executeRPC(at_time, call="listAnalyses")
 
-    def listAnalyses2(self, *, at_time: Opt[datetime] = None):
-        """Return the mapping of known WGs to analyses
-
-        :param at_time: The datetime at which this query should be ran, defaults to now
-        :returns: ``list`` with each entry being a ``dict``  of high-level information about each analysis
-        """
-        return self.executeRPC(at_time, call="listAnalyses2")
-
-    def listRequests(self):
-        """Return the mapping of known WGs to analyses
-
-        :returns: ``list`` with each entry being a ``dict``  of high-level information about each sample
-        """
-        return self.executeRPC(call="listRequests")
-
-    def getOwners(self, *, wg: str, analysis: str):
-        """Return the list of owners for a specific analysis
-
-        :returns: ``dict`` mapping the WG name to a list of analyses
-        """
-        return self.executeRPC(wg, analysis, call="getOwners")
-
-    def setOwners(self, *, wg: str, analysis: str, owners: list[str]):
-        """Set the list of owners for a specific analysis
-
-        :returns: ``dict`` mapping the WG name to a list of analyses
-        """
-        return self.executeRPC(wg, analysis, owners, call="setOwners")
-
     def getProductions(
         self,
         *,
         wg: Opt[str] = None,
         analysis: Opt[str] = None,
         version: Opt[str] = None,
         name: Opt[str] = None,
@@ -245,23 +216,21 @@
         """Add a new production to the database
 
         :param requests: List of dictionaries
         :returns: S_OK() || S_ERROR()
         """
         return self.executeRPC(requests, call="registerRequests")
 
-    def addRequestsToAnalysis(self, wg: str, analysis: str, request_ids: list[int]):
+    def registerSamples(self, samples):
         """Add a new production to the database
 
-        :param wg: The WG to which the analysis belongs
-        :param analysis: The analysis which should have the samples added to
-        :param request_ids: List of request IDs
+        :param samples: List of dictionaries
         :returns: S_OK() || S_ERROR()
         """
-        return self.executeRPC(wg, analysis, request_ids, call="addRequestsToAnalysis")
+        return self.executeRPC(samples, call="registerSamples")
 
     def archiveSamples(self, samples):
         """Archive an analysis Sample
 
         :param samples: List of sample IDs
         :returns: S_OK() || S_ERROR()
         """
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 For more information on the meaning of the various objects see :py:mod:`.AnalysisProductionsClient`.
 
 Tables are defined using SQLAlchemy and imported from :py:mod:`.AnalysisProductionsObjects`.
 Example usage of this class can be found in `Test_AnalysisProductionsDB.py`.
 """
 import functools
 from collections import defaultdict
-from copy import deepcopy
 from contextlib import contextmanager
+from copy import deepcopy
 
-from sqlalchemy import create_engine, delete, func, insert, or_, tuple_, select, case, JSON, cast, Integer
-from sqlalchemy.orm.attributes import flag_modified
+from sqlalchemy import create_engine, func, or_, tuple_, select
 from sqlalchemy.orm import Session
+from sqlalchemy.orm.attributes import flag_modified
 
 from DIRAC.ConfigurationSystem.Client.Utilities import getDBParameters
 from DIRAC.Core.Base.DIRACDB import DIRACDB
 from DIRAC.Core.Utilities.ReturnValues import returnValueOrRaise
 
 from LHCbDIRAC.ProductionManagementSystem.DB.AnalysisProductionsObjects import (
     Base,
     AnalysisSample as AP,
     AutoTag,
     Tag,
     Request,
-    AnalysisOwner,
+    User,
 )
-from LHCbDIRAC.ProductionManagementSystem.DB.extra_func import json_group_array, json_group_object
 
 
 def inject_session(func):
     """Decorator to inject the session into a class method
 
     Decorator to start a SQLAlchemy Session and inject it in the wrapped function
     as a keyword argument.
@@ -87,166 +86,23 @@
         query = _filterForTime(session.query(AP.wg, AP.analysis).distinct(), AP, at_time)
         result = defaultdict(list)
         for wg, analysis in query:
             result[wg].append(analysis)
         return dict(result)
 
     @inject_session
-    def listAnalyses2(self, *, at_time=None, session: Session):
-        # Select the owners of the analyses
-        query = select(AnalysisOwner.wg, AnalysisOwner.analysis, AnalysisOwner.username).distinct()
-        owners = defaultdict(lambda: defaultdict(list))
-        for wg, analysis, username in session.execute(query).all():
-            owners[wg][analysis].append(username)
-
-        # Select the analyses and build the list of results
-        query = select(
-            AP.wg,
-            AP.analysis,
-            # Add a column n_{STATE_NAME} containing the number of analyses in each possible state
-            *(
-                # MySQL returns a decimal type from sum() so we need to cast it to an integer
-                cast(func.sum(case((AP.state == state, 1), else_=0)), Integer).label(  # pylint: disable=not-callable
-                    f"n_{state}"
-                )
-                for state in AP.VALID_STATES
-            ),
-            func.count().label("n_total"),  # pylint: disable=not-callable
-        )
-        query = query.group_by(AP.wg, AP.analysis)
-        query = _filterForTime(query, AP, at_time)
-        return [dict(row._mapping) | {"owners": owners[row.wg][row.analysis]} for row in session.execute(query).all()]
-
-    @inject_session
-    def listRequests(self, *, session: Session):
-        analyses = select(
-            AP.request_id,
-            AP.name,
-            AP.version,
-            json_group_array(func.json_array(AP.wg, AP.analysis)).label("analyses"),
-        )
-        analyses = analyses.group_by(AP.request_id, AP.name, AP.version)
-        analyses = _filterForTime(analyses, AP, at_time=None)
-        analyses = analyses.subquery(name="requests")
-
-        autotags = select(
-            Request.request_id,
-            # Can't use AGG_FUNC.filter as it's not supported by mysql
-            case(
-                (
-                    func.sum(AutoTag.name.is_not(None)) == 0,  # pylint: disable=not-callable
-                    func.json_object(type_=JSON),  # pylint: disable=not-callable
-                ),
-                else_=json_group_object(AutoTag.name, AutoTag.value),
-            ).label("autotags"),
-        )
-        autotags = autotags.join(AutoTag, Request.request_id == AutoTag.request_id, isouter=True)
-        autotags = autotags.group_by(Request.request_id)
-        autotags = autotags.subquery(name="autotags")
-
-        tags = select(
-            AP.request_id,
-            # Can't use AGG_FUNC.filter as it's not supported by mysql
-            case(
-                (
-                    func.sum(Tag.name.is_not(None)) == 0,  # pylint: disable=not-callable
-                    func.json_array(type_=JSON),  # pylint: disable=not-callable
-                ),
-                else_=json_group_array(func.json_array(Tag.name, Tag.value)),
-            ).label("tags"),
-        ).distinct()
-        tags = tags.join(Tag, AP.sample_id == Tag.sample_id, isouter=True)
-        tags = tags.group_by(AP.request_id)
-        tags = tags.subquery(name="tags")
-
-        query = select(analyses, autotags.c.autotags, tags.c.tags)
-        query = query.join(autotags, analyses.c.request_id == autotags.c.request_id, isouter=True)
-        query = query.join(tags, analyses.c.request_id == tags.c.request_id, isouter=True)
-        return [dict(row._mapping) for row in session.execute(query).all()]
-
-    @inject_session
-    def getOwners(self, *, wg=None, analysis=None, session: Session):
-        query = select(AnalysisOwner.username)
-        query = query.where(AnalysisOwner.wg == wg)
-        query = query.where(AnalysisOwner.analysis == analysis)
-        return session.execute(query).scalars().all()
-
-    @inject_session
-    def setOwners(self, *, wg=None, analysis=None, owners=None, session: Session):
-        query = select(AnalysisOwner.username)
-        query = query.where(AnalysisOwner.wg == wg)
-        query = query.where(AnalysisOwner.analysis == analysis)
-        existing_owners = session.execute(query).scalars().all()
-
-        new_owners = [
-            {"wg": wg, "analysis": analysis, "username": owner} for owner in owners if owner not in existing_owners
-        ]
-        if new_owners:
-            session.execute(insert(AnalysisOwner).values(new_owners))
-
-        query = delete(AnalysisOwner)
-        query = query.where(AnalysisOwner.wg == wg)
-        query = query.where(AnalysisOwner.analysis == analysis)
-        query = query.where(~AnalysisOwner.username.in_(owners))
-        session.execute(query)
-
-    @inject_session
     def getProductions(
         self, *, wg=None, analysis=None, version=None, name=None, state=None, at_time=None, session: Session
     ):
-        query = select(
-            AP.wg,
-            AP.analysis,
-            AP.sample_id,
-            AP.validity_start,
-            AP.validity_end,
-            AP.name,
-            AP.version,
-            AP.request_id,
-            AP.state,
-            AP.last_state_update,
-            AP.extra_info["transformations"].label("transformations"),
-            AP.progress,
-            AP.extra_info["jira_task"].label("jira_task"),
-            AP.extra_info["merge_request"].label("merge_request"),
-        )
+        query = session.query(AP)
         query = query.filter(*_buildCondition(wg, analysis, name, version))
         if state is not None:
             query = query.filter(AP.state == state)
         query = _filterForTime(query, AP, at_time)
-
-        results = []
-        for row in session.execute(query).all():
-            result = {
-                "name": row.name,
-                "version": row.version,
-                "request_id": row.request_id,
-                "state": row.state,
-                "last_state_update": row.last_state_update,
-                "transformations": row.transformations,
-            }
-            if row.progress is not None:
-                result["progress"] = row.progress
-            if row.jira_task is not None:
-                result["jira_task"] = row.jira_task
-            if row.merge_request is not None:
-                result["merge_request"] = row.merge_request
-            result.update(
-                {
-                    "wg": row.wg,
-                    "analysis": row.analysis,
-                    "sample_id": row.sample_id,
-                    # TODO: Remove
-                    "owners": [],
-                    "validity_start": row.validity_start,
-                    "validity_end": row.validity_end,
-                }
-            )
-            results.append(result)
-        return results
+        return [result.toDict() for result in query]
 
     @inject_session
     def getArchivedRequests(self, *, state=None, session: Session):
         sq = session.query(AP.request_id).filter(AP.validity_end.is_(None)).distinct().subquery()
         query = session.query(Request).filter(~Request.request_id.in_(select(sq)))
         if state is not None:
             query = query.filter(AP.state == state)
@@ -256,14 +112,19 @@
     def getTags(self, wg, analysis, *, at_time=None, session: Session):
         return _getTags(session, wg=wg, analysis=analysis, at_time=at_time)
 
     @inject_session
     def getKnownAutoTags(self, *, session) -> set:
         return _getKnownAutoTags(session)
 
+    # @inject_session
+    # def registerRequest(self, requests, *, session: Session):
+    #     for request in requests:
+    #         session.add(AP(**request))
+
     @inject_session
     def registerTransformations(self, transforms: dict[int, list[dict]], *, session: Session):
         if not transforms:
             raise ValueError("No transforms passed")
         transforms = deepcopy(transforms)
         for request in session.query(Request).filter(Request.request_id.in_(transforms)):
             knownTransforms = {t["id"] for t in request.extra_info["transformations"]}
@@ -316,45 +177,23 @@
                     version=r["version"],
                     wg=r["wg"],
                     analysis=r["analysis"],
                     validity_start=r["validity_start"],
                     extra_info=r["extra_info"],
                     auto_tags=[AutoTag(name=x["name"], value=x["value"]) for x in r["auto_tags"]],
                 )
-                # TODO: Remove
-                # sample.owners = [User(username=x["username"]) for x in r["owners"]]
+                sample.owners = [User(username=x["username"]) for x in r["owners"]]
                 session.add(sample)
 
         with self.session as session:
             query = session.query(AP)
             query = query.filter(AP.request_id.in_(request_ids))
             return [result.toDict() for result in query]
 
     @inject_session
-    def addRequestsToAnalysis(self, wg: str, analysis: str, request_ids: list[id], *, session: Session):
-        self.log.info("Adding samples to analysis", f"({wg}/{analysis}) {','.join(map(str, request_ids))}")
-
-        query = select(AP.request_id, AP.sample_id).filter(
-            AP.wg == wg,
-            AP.analysis == analysis,
-            AP.request_id.in_(request_ids),
-            AP.validity_end.is_(None),
-        )
-        if already_existing := session.execute(query).all():
-            raise ValueError(
-                f"Some requests are already registered for {wg}/{analysis} request_id->sample_id mapping is "
-                f"{ {request_id: sample_id for request_id, sample_id in already_existing} }"
-            )
-
-        query = insert(AP).values(
-            [{"wg": wg, "analysis": analysis, "request_id": request_id} for request_id in request_ids]
-        )
-        session.execute(query)
-
-    @inject_session
     def archiveSamples(self, sample_ids: list[int], *, session: Session):
         self.log.info("Archiving Analysis Productions", ",".join(map(str, sample_ids)))
         query = session.query(AP.sample_id)
         query = query.filter(AP.sample_id.in_(sample_ids))
         known_sample_ids = {i for i, in query}
         if len(known_sample_ids) != len(sample_ids):
             raise ValueError(f"Unknown sample IDs passed {known_sample_ids - set(sample_ids)!r}")
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,15 @@
     def toDict(self):
         result = Request.toDict(self)
         result.update(
             {
                 "wg": self.wg,
                 "analysis": self.analysis,
                 "sample_id": self.sample_id,
-                # TODO: Remove
-                "owners": [],
+                "owners": [o.username for o in self.owners],
                 "validity_start": self.validity_start,
                 "validity_end": self.validity_end,
             }
         )
         return result
 
 
@@ -120,26 +119,14 @@
     validity_end = Column(DateTime(timezone=False), nullable=True)
 
     @validates("username")
     def convert_lower(self, key, value):
         return value.lower()
 
 
-class AnalysisOwner(Base):
-    __tablename__ = "ap_analyis_owners"
-
-    wg = Column(String(16), primary_key=True)
-    analysis = Column(String(256), primary_key=True)
-    username = Column(String(256), primary_key=True)
-
-    @validates("username", "wg", "analysis")
-    def convert_lower(self, key, value):
-        return value.lower()
-
-
 class Publication(Base):
     __tablename__ = "ap_publications"
 
     id = Column(Integer, primary_key=True)
     number = Column(String(64), nullable=False)
     sample_id = Column(Integer, ForeignKey("ap_analysis_samples.sample_id"), nullable=False)
     sample = relationship("AnalysisSample", back_populates="publications", lazy="selectin")
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-from __future__ import annotations
-
 from datetime import datetime, timedelta
 
 import pytest
 
 from LHCbDIRAC.ProductionManagementSystem.DB.AnalysisProductionsDB import AnalysisProductionsDB
 
 
@@ -31,15 +29,15 @@
     "analysis": "MyAnalysis",
     "extra_info": {
         "transformations": [],
         "merge_request": "https://gitlab.cern.ch/lhcb-datapkg/AnalysisProductions/-/merge_requests/0",
         "jira_task": "https://its.cern.ch/jira/browse/WGP-0",
     },
     "validity_start": datetime.now() - timedelta(days=1),
-    "owners": [],
+    "owners": [{"username": "johndoe"}],
     "auto_tags": [
         {"name": "config", "value": "MC"},
         {"name": "polarity", "value": "MagDown"},
         {"name": "eventtype", "value": "23133002"},
         {"name": "datatype", "value": "2012"},
     ],
 }
@@ -52,15 +50,15 @@
     "analysis": "AnotherAnalysis",
     "extra_info": {
         "transformations": [],
         "merge_request": "https://gitlab.cern.ch/lhcb-datapkg/AnalysisProductions/-/merge_requests/0",
         "jira_task": "https://its.cern.ch/jira/browse/WGP-0",
     },
     "validity_start": datetime.now() - timedelta(days=1),
-    "owners": [],
+    "owners": [{"username": "janedoe"}],
     "auto_tags": [
         {"name": "config", "value": "LHCb"},
         {"name": "polarity", "value": "MagUp"},
         {"name": "datatype", "value": "2018"},
     ],
 }
 
@@ -72,15 +70,15 @@
     "analysis": "MyAnalysis",
     "extra_info": {
         "transformations": [],
         "merge_request": "https://gitlab.cern.ch/lhcb-datapkg/AnalysisProductions/-/merge_requests/0",
         "jira_task": "https://its.cern.ch/jira/browse/WGP-0",
     },
     "validity_start": datetime.now() - timedelta(days=1),
-    "owners": [],
+    "owners": [{"username": "janedoe"}],
     "auto_tags": [
         {"name": "config", "value": "LHCb"},
         {"name": "polarity", "value": "MagUp"},
         {"name": "datatype", "value": "2018"},
     ],
 }
 
@@ -121,16 +119,15 @@
     assert orig["wg"].lower() == new["wg"]
     assert orig["analysis"].lower() == new["analysis"]
     assert orig["version"].lower() == new["version"]
     assert orig["name"].lower() == new["name"]
     assert orig["extra_info"]["jira_task"] == new["jira_task"]
     assert orig["extra_info"]["merge_request"] == new["merge_request"]
 
-    assert orig["owners"] == []
-    assert new["owners"] == []
+    assert {x["username"].lower() for x in orig["owners"]} == set(new["owners"])
     assert orig["extra_info"]["transformations"] == new["transformations"]
 
     assert orig["validity_start"] == new["validity_start"]
     assert new["validity_end"] is None
     assert new["last_state_update"] is not None
 
 
@@ -147,61 +144,25 @@
     assert apdb.getProductions(at_time=datetime.now()) == []
 
     assert apdb.getArchivedRequests() == []
     assert apdb.getArchivedRequests(state="waiting") == []
     assert apdb.getArchivedRequests(state="ready") == []
 
 
-def test_ownership(apdb):
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis") == []
-    apdb.setOwners(wg="mywg", analysis="myanalysis", owners=["auser"])
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis") == ["auser"]
-
-    assert apdb.getOwners(wg="mywg2", analysis="myanalysis") == []
-    apdb.setOwners(wg="mywg2", analysis="myanalysis", owners=["user2"])
-    assert apdb.getOwners(wg="mywg2", analysis="myanalysis") == ["user2"]
-
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis2") == []
-    apdb.setOwners(wg="mywg", analysis="myanalysis2", owners=["user3"])
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis2") == ["user3"]
-
-    apdb.setOwners(wg="mywg", analysis="myanalysis2", owners=[])
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis2") == []
-
-    apdb.setOwners(wg="mywg", analysis="myanalysis", owners=["user4", "user5"])
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis") == ["user4", "user5"]
-
-    apdb.setOwners(wg="mywg", analysis="myanalysis", owners=[])
-    assert apdb.getOwners(wg="mywg", analysis="myanalysis") == []
-
-
 def test_registerNew(apdb):
     newRequests = apdb.registerRequests([REQUEST_1])
     assert len(newRequests) == 1
 
     newRequest = newRequests[0]
     assert newRequest["sample_id"] == 1
     assert newRequest["state"] == "waiting"
     _compareRequest(REQUEST_1, newRequest)
 
     assert apdb.listAnalyses() == {"mywg": ["myanalysis"]}
 
-    assert apdb.listAnalyses2() == [
-        {
-            "analysis": "myanalysis",
-            "n_active": 0,
-            "n_ready": 0,
-            "n_replicating": 0,
-            "n_total": 1,
-            "n_waiting": 1,
-            "owners": [],
-            "wg": "mywg",
-        }
-    ]
-
     assert apdb.getProductions() == [newRequest]
     assert apdb.getProductions(wg="mywg", analysis="myanalysis") == [newRequest]
     assert apdb.getProductions(wg="MYWG", analysis="MYANALYSIS") == [newRequest]
     assert apdb.getProductions(name="mysample") == [newRequest]
     assert apdb.getProductions(name="MySample") == [newRequest]
     assert apdb.getProductions(name="anothersample") == []
     assert apdb.getProductions(state="waiting") == [newRequest]
@@ -222,56 +183,14 @@
 
 def test_duplicate(apdb):
     apdb.registerRequests([REQUEST_1])
     with pytest.raises(ValueError, match=f"Already registered.*{REQUEST_1['request_id']}.*"):
         apdb.registerRequests([REQUEST_1])
 
 
-def test_listRequests(apdb):
-    assert apdb.listRequests() == []
-    apdb.registerRequests([REQUEST_1, REQUEST_2, REQUEST_3])
-    requests = apdb.listRequests()
-    assert len(requests) == 3
-    for request in requests:
-        assert request["tags"] == []
-        assert isinstance(request["autotags"], dict)
-        if "eventtype" in request["autotags"]:
-            assert {"config", "datatype", "polarity", "eventtype"} == set(request["autotags"])
-        else:
-            assert {"config", "datatype", "polarity"} == set(request["autotags"])
-
-    apdb.archiveSamples([apdb.getProductions()[0]["sample_id"]])
-
-    requests = apdb.listRequests()
-    assert len(requests) == 2
-
-
-def test_multiple_samples_per_request(apdb: AnalysisProductionsDB):
-    apdb.registerRequests([REQUEST_1, REQUEST_2, REQUEST_3])
-    assert {"myanalysis", "anotheranalysis"} == {x["analysis"] for x in apdb.listAnalyses2()}
-    orig1 = apdb.getProductions(wg=REQUEST_1["wg"], analysis=REQUEST_1["analysis"], name=REQUEST_1["name"])
-    assert len(orig1) == 1
-
-    apdb.addRequestsToAnalysis("newwg", "newanalysis", [REQUEST_1["request_id"]])
-    assert {"newanalysis", "myanalysis", "anotheranalysis"} == {x["analysis"] for x in apdb.listAnalyses2()}
-
-    with pytest.raises(ValueError, match="Some requests are already registered"):
-        apdb.addRequestsToAnalysis("newwg", "newanalysis", [REQUEST_1["request_id"], REQUEST_2["request_id"]])
-    assert len(apdb.getProductions(wg="newwg", analysis="newanalysis")) == 1
-
-    apdb.addRequestsToAnalysis("newwg", "newanalysis", [REQUEST_2["request_id"], REQUEST_3["request_id"]])
-    assert len(apdb.getProductions(wg="newwg", analysis="newanalysis")) == 3
-
-    ref1 = apdb.getProductions(wg="newwg", analysis="newanalysis", name=REQUEST_1["name"])
-    assert len(ref1) == 1
-    for key in set(orig1[0]) | set(ref1[0]):
-        if key not in {"validity_start", "wg", "analysis", "sample_id"}:
-            assert orig1[0][key] == ref1[0][key], key
-
-
 def test_archival(apdb):
     apdb.registerRequests([REQUEST_1, REQUEST_2, REQUEST_3])
 
     assert apdb.getArchivedRequests() == []
     assert apdb.getArchivedRequests(state="waiting") == []
     assert apdb.getArchivedRequests(state="ready") == []
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,42 +44,14 @@
     types_listAnalyses = [optDate]
 
     @convertToReturnValue
     def export_listAnalyses(self, at_time):
         """See :meth:`~.AnalysisProductionsClient.listAnalyses`"""
         return self._db.listAnalyses(at_time=at_time)
 
-    types_listAnalyses2 = [optDate]
-
-    @convertToReturnValue
-    def export_listAnalyses2(self, at_time):
-        """See :meth:`~.AnalysisProductionsClient.listAnalyses2`"""
-        return self._db.listAnalyses2(at_time=at_time)
-
-    types_listRequests = [optDate]
-
-    @convertToReturnValue
-    def export_listRequests(self):
-        """See :meth:`~.AnalysisProductionsClient.listRequests`"""
-        return self._db.listRequests()
-
-    types_getOwners = [str, str]
-
-    @convertToReturnValue
-    def export_getOwners(self, wg, analysis):
-        """See :meth:`~.AnalysisProductionsClient.getOwners`"""
-        return self._db.getOwners(wg=wg, analysis=analysis)
-
-    types_setOwners = [str, str, list]
-
-    @convertToReturnValue
-    def export_setOwners(self, wg, analysis, owners):
-        """See :meth:`~.AnalysisProductionsClient.setOwners`"""
-        return self._db.setOwners(wg=wg, analysis=analysis, owners=owners)
-
     types_getProductions = [optString, optString, optString, optString, optString, bool, bool, bool, optDate]
 
     @convertToReturnValue
     def export_getProductions(
         self, wg, analysis, version, name, state, with_lfns, with_pfns, with_transformations, at_time
     ):
         """See :meth:`~.AnalysisProductionsClient.getProductions`"""
@@ -112,14 +84,20 @@
     types_getKnownAutoTags = []
 
     @convertToReturnValue
     def export_getKnownAutoTags(self):
         """See :meth:`~.AnalysisProductionsClient.getKnownAutoTags`"""
         return list(self._db.getKnownAutoTags())
 
+    # types_registerRequest = [list]
+    # auth should be PRODUCTION_MANAGEMENT!
+    # @convertToReturnValue
+    # def export_registerRequest(self, requests):
+    #     return self._db.registerRequest(requests)
+
     types_registerTransformations = [dict]
 
     @convertToReturnValue
     def export_registerTransformations(self, transforms):
         """See :meth:`~.AnalysisProductionsClient.registerTransformations`"""
         transforms = {int(k): v for k, v in transforms.items()}
         return self._db.registerTransformations(transforms)
@@ -136,20 +114,19 @@
 
     @convertToReturnValue
     def export_registerRequests(self, requests):
         """See :meth:`~.AnalysisProductionsClient.registerRequests`"""
         results = self._db.registerRequests(requests)
         return _queryToResults(results, with_lfns=False, with_pfns=False, with_transformations=False)
 
-    types_addRequestsToAnalysis = [str, str, list]
-
-    @convertToReturnValue
-    def export_addRequestsToAnalysis(self, wg, analysis, request_ids):
-        """See :meth:`~.AnalysisProductionsClient.addRequestsToAnalysis`"""
-        return self._db.addRequestsToAnalysis(wg, analysis, request_ids)
+    # types_registerSamples = [list]
+    # auth should be PRODUCTION_MANAGEMENT!
+    # @convertToReturnValue
+    # def export_registerSamples(self, samples):
+    #   """See :meth:`~.AnalysisProductionsClient.registerSamples`"""
 
     types_archiveSamples = [list]
 
     @convertToReturnValue
     def export_archiveSamples(self, sample_ids):
         """See :meth:`~.AnalysisProductionsClient.archiveSamples`"""
         return self._db.archiveSamples(sample_ids)
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         "ProcessingPass": step.processing_pass,
         "StepName": step.name,
         "isMulticore": "Y" if step.multicore else "N",
         # TODO: Really old steps have Visible = None?
         "Visible": "Y" if step.visible else "N",
         # TODO: Appears to have never been used
         # TODO: Required for running local tests
-        "mcTCK": "",
+        # 'mcTCK': self.mc_tck or '',
         # 'DQTag': step.dbtags.DQ or '',
         # TODO: Get rid of RuntimeProjects from the database
     }
     if step.application.nightly is not None:
         result["ApplicationVersion"] = step.application.json()
     if step.id is not None:
         result["StepId"] = step.id
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,14 @@
     yamlPath, name, eventType, inputFiles, useCfgOverride = parseArgs()
 
     if useCfgOverride:
         return _runWithConfigOverride(sys.argv + ["--no-cfg-override"])
 
     productionRequests = defaultdict(list)
     for spec in yaml.safe_load(yamlPath.read_text()):
-        if spec.get("author") is None:  # can occur when testing files produce by LbMCSubmit
-            spec["author"] = "local_user"
         productionRequest = parse_obj(spec)
         productionRequests[productionRequest.name] += [productionRequest]
 
     if name is None:
         if len(productionRequests) == 1:
             name = list(productionRequests)[0]
         else:
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,16 @@
 """LHCbDIRAC.ResourceStatusSystem.Agent.NagiosTopologyAgent.
 
 NagiosTopologyAgent.__bases__: DIRAC.Core.Base.AgentModule.AgentModule
 
 xml_append
 """
 import os
-import socket
 import json
 
-from urllib.parse import urlparse
-from typing import Optional
-
 from DIRAC import S_OK, gConfig, rootPath
 from DIRAC.ConfigurationSystem.Client.Helpers.Resources import getSites
 from DIRAC.ConfigurationSystem.Client.Helpers.Path import cfgPath
 from DIRAC.Core.Base.AgentModule import AgentModule
 from DIRAC.Resources.Storage.StorageElement import StorageElement
 
 AGENT_NAME = "ResourceStatus/NagiosTopologyAgent"
@@ -41,30 +37,14 @@
     "cloud": "CLOUD",
     "boinc": "BOINC",
     "vcycle": "VCYCLE",
     "dirac": "DIRAC",
 }
 
 
-def isHostIPV6(host: str) -> Optional[bool]:
-    """Test if the given host is ipv6 capable.
-
-    :returns: True if IPv6 capable, False if only IPv4, None in case of resolution problem
-    """
-    try:  # First try IPV6
-        socket.getaddrinfo(host, None, socket.AF_INET6)
-        return True
-    except socket.gaierror:  # No IPv6 address
-        try:  # Next try IPv4
-            socket.getaddrinfo(host, None, socket.AF_INET)
-            return False
-        except socket.gaierror:  # The host does not exist (no IPv6 or IPv4 address)
-            return None
-
-
 class NagiosTopologyAgent(AgentModule):
     """This agent loops over the Dirac CS and extracts the necessary information
     to create a "topology map" which is used by the IT provided Nagios system to
     test Grid sites. The topology information defines the services to be tested.
 
     NagiosTopologyAgent, writes the xml topology consumed by Nagios to run
     the tests.
@@ -131,15 +111,14 @@
 
                     ceDetailsInCS = res["Value"]
                     ceDetails = dict()
                     ceDetails["type"] = "compute"
                     ceDetails["access_points"] = dict()
                     ceDetails["access_points"][ce] = dict()
                     ceDetails["access_points"][ce]["endpoint_url"] = ce
-                    ceDetails["access_points"][ce]["ipv6_status"] = isHostIPV6(ce)
                     ceDetails["access_points"][ce]["type"] = MAPPING_CE_TYPE.get(
                         ceDetailsInCS["CEType"].lower(), "UNDEFINED"
                     )
                     ceDetails["access_points"][ce]["monitored"] = "yes" if wlcgName else "no"
                     ceDetails["access_points"][ce]["quality_level"] = "production"
                     # queues
                     res = gConfig.getSections(cfgPath("Resources", "Sites", grid, site, "CEs", ce, "Queues"), [])
@@ -173,15 +152,14 @@
                         + "://"
                         + diracSEoption["Host"].strip("/")
                         + ":"
                         + diracSEoption["Port"],
                         diracSEoption["Path"].strip("/"),
                     )
                     seDetails["endpoint_url"] = ep
-                    seDetails["ipv6_status"] = isHostIPV6(urlparse(ep).hostname)
                     seDetails["interface_type"] = diracSEoption["Protocol"]
                     seDetails["monitored"] = "yes" if wlcgName else "no"
                     seDetails["quality_level"] = "production"
 
                     dseep = "_".join([se, diracSEoption["Protocol"]])  # just a unique name e.g. 'CERN-DST-EOS_root'
                     seDetailsForDIRACSE[dseep] = seDetails
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/DownHillPropagationPolicy.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/DownHillPropagationPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/ResourceStatusSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/ResourceStatusSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Resources/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Resources/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/DB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Service/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/FileUsage.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/FileUsage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/MergeMDF.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/MergeMDF.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UploadMC.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UploadMC.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/mock_Commons.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/mock_Commons.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbAnalyse.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbAnalyse.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Others.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Others.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Uploads.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Uploads.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/Test_Modules_AnalyseFileAccess.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/Test_Modules_AnalyseFileAccess.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/pool_xml_catalog.xml` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/pool_xml_catalog.xml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/summary.xml` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/summary.xml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/Workflow/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/Workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Service/WMSSecureGWHandler.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Service/WMSSecureGWHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/Service/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Utilities/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/Workflow.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/Workflow.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC/tests/__init__.py` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/PKG-INFO` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LHCbDIRAC
-Version: 11.0.9
+Version: 11.1.0a1
 Summary: LHCbDIRAC is the LHCb extension of DIRAC
 Home-page: https://gitlab.cern.ch/lhcb-dirac/LHCbDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/SOURCES.txt` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,14 @@
 src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py
 src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py
 src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py
 src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py
 src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py
 src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql
 src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py
-src/LHCbDIRAC/ProductionManagementSystem/DB/extra_func.py
 src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py
 src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py
 src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py
 src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py
 src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py
 src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py
 src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py
```

### Comparing `LHCbDIRAC-11.0.9/src/LHCbDIRAC.egg-info/entry_points.txt` & `LHCbDIRAC-11.1.0a1/src/LHCbDIRAC.egg-info/entry_points.txt`

 * *Files identical despite different names*

