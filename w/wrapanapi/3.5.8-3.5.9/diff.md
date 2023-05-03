# Comparing `tmp/wrapanapi-3.5.8.tar.gz` & `tmp/wrapanapi-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wrapanapi-3.5.8.tar", last modified: Fri Apr 23 14:22:09 2021, max compression
+gzip compressed data, was "dist/wrapanapi-3.5.9.tar", last modified: Fri Jun 11 11:44:58 2021, max compression
```

## Comparing `wrapanapi-3.5.8.tar` & `wrapanapi-3.5.9.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1624 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      843 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/AUTHORS
--rw-rw-r--   0 travis    (2000) travis    (2000)     3799 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/ChangeLog
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5770 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/requirements-test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1240 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/alerts/
--rw-rw-r--   0 travis    (2000) travis    (2000)   162076 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/alerts/events.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Datasource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Datasource/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Deployment/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Domain WildFly Server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Domain WildFly Server/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Host Controller/
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Host Controller/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Queue/
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Queue/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Topic/
--rw-rw-r--   0 travis    (2000) travis    (2000)      896 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Topic/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/SubDeployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/SubDeployment/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/WildFly Server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/WildFly Server/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/XA Datasource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/XA Datasource/resources.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1736 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      473 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Datasource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Datasource/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7854 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Deployment/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Domain WildFly Server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Domain WildFly Server/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Host Controller/
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Host Controller/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Queue/
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Queue/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Topic/
--rw-rw-r--   0 travis    (2000) travis    (2000)      896 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Topic/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/SubDeployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1796 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/SubDeployment/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/WildFly Server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      416 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/WildFly Server/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/XA Datasource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/XA Datasource/resources.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3469 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      465 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      465 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDS/data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      398 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Datasource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Datasource/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Deployment/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Domain WildFly Server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Domain WildFly Server/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Host Controller/
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Host Controller/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Queue/
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Queue/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Topic/
--rw-rw-r--   0 travis    (2000) travis    (2000)      896 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Topic/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/SubDeployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/SubDeployment/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/WildFly Server/
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/WildFly Server/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/XA Datasource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/XA Datasource/resources.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1736 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      473 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/Domain Server Group/
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/Domain Server Group/resources.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Host Controller/
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Host Controller/data.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Local~~/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Local~~/Local~%2Fserver-group%3Dmain-server-group/
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Local~~/Local~%2Fserver-group%3Dmain-server-group/data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      238 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/inventory/status.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/resources/hawkular/metrics/status.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    13600 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/test_hawkular.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6236 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tests/test_vm_and_template_systems.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/tox.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      960 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi/clients/
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/clients/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5941 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/clients/rest_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5712 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/clients/websocket_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/const.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi/entities/
--rw-rw-r--   0 travis    (2000) travis    (2000)      568 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9068 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      435 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/instance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/network.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      861 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/physical_container.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3471 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1962 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/stack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2295 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17241 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/vm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/entities/volume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4524 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi/systems/
--rw-rw-r--   0 travis    (2000) travis    (2000)      715 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi/systems/container/
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/container/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72678 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/container/rhopenshift.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58372 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/ec2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32887 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/google.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80282 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/hawkular.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22267 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/lenovo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49344 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/msazure.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3911 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/nuage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47192 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/openstack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5961 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/openstack_infra.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14739 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/redfish.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50079 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/rhevm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30185 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/scvmm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2701 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/vcloud.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52698 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/systems/virtualcenter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      217 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2376 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/utils/json_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/utils/logger_mixin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      163 2021-04-23 14:20:09.000000 wrapanapi-3.5.8/wrapanapi/utils/random.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5770 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8344 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/pbr.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      581 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-04-23 14:22:09.000000 wrapanapi-3.5.8/wrapanapi.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1624 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      872 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/AUTHORS
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3816 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/ChangeLog
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4813 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/requirements-test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1240 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       54 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/alerts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   162076 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/alerts/events.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Datasource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Datasource/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Deployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Deployment/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Domain WildFly Server/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      468 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Domain WildFly Server/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Host Controller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Host Controller/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Queue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Queue/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Topic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      896 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Topic/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/SubDeployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/SubDeployment/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/WildFly Server/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/WildFly Server/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/XA Datasource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/XA Datasource/resources.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1736 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      473 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      477 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/WildfyServerOne~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      366 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resources/WildfyServerOne~~/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Datasource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Datasource/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Deployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7854 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Deployment/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Domain WildFly Server/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Domain WildFly Server/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Host Controller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Host Controller/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Queue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Queue/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Topic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      896 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Topic/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/SubDeployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1796 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/SubDeployment/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/WildFly Server/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      416 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/WildFly Server/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/XA Datasource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      508 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/XA Datasource/resources.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3469 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/Local~%2Fsubsystem%3Ddatasources%2Fdata-source%3DKeycloakDS/data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      398 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resources/Local~~/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Datasource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Datasource/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Deployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Deployment/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Domain WildFly Server/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      468 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Domain WildFly Server/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Host Controller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Host Controller/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Queue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Queue/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Topic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      896 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Topic/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/SubDeployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        4 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/SubDeployment/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/WildFly Server/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/WildFly Server/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/XA Datasource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/XA Datasource/resources.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1736 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      473 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      477 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADSMWTest/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleDS/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/WildfyServerTwo~%2Fsubsystem%3Ddatasources%2Fdata-source%3DExampleXADS/data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resources/WildfyServerTwo~~/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/Domain Server Group/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/Domain Server Group/resources.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Host Controller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Host Controller/data.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Local~~/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Local~~/Local~%2Fserver-group%3Dmain-server-group/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      366 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resources/Local~~/Local~%2Fserver-group%3Dmain-server-group/data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      238 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/inventory/status.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/tests/resources/hawkular/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/resources/hawkular/metrics/status.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13600 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/test_hawkular.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6236 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tests/test_vm_and_template_systems.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      960 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi/clients/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/clients/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5941 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/clients/rest_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5712 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/clients/websocket_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       42 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/const.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi/entities/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      568 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9068 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      435 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/instance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/network.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      861 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/physical_container.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3471 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/server.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1962 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/stack.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2295 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17241 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/vm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/entities/volume.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4524 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi/systems/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      715 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/base.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi/systems/container/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/container/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72678 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/container/rhopenshift.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60244 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/ec2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32887 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/google.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80282 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/hawkular.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22267 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/lenovo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49344 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/msazure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3911 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/nuage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47192 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/openstack.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5961 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/openstack_infra.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14739 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/redfish.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50079 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/rhevm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30185 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/scvmm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2701 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/vcloud.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52698 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/systems/virtualcenter.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      217 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2376 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/utils/json_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/utils/logger_mixin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      163 2021-06-11 11:43:03.000000 wrapanapi-3.5.9/wrapanapi/utils/random.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4813 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8344 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/pbr.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      581 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-06-11 11:44:58.000000 wrapanapi-3.5.9/wrapanapi.egg-info/top_level.txt
```

### Comparing `wrapanapi-3.5.8/.travis.yml` & `wrapanapi-3.5.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/AUTHORS` & `wrapanapi-3.5.9/AUTHORS`

 * *Files 11% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 Nikhil Dhandre <ndhandre@redhat.com>
 Pavel Šimovec <52415835+psimovec@users.noreply.github.com>
 Tomas Strych <tomas.strych2@gmail.com>
 Yadnyawalkya Tale <10824880+Yadnyawalkya@users.noreply.github.com>
 izapolsk <izapolsk@redhat.com>
 john-dupuy <44065123+john-dupuy@users.noreply.github.com>
 john-dupuy <jdupuy@redhat.com>
+jyejare <jyejare@redhat.com>
 mmojzis <mmojzis@redhat.com>
 mnadeem92 <mnadeem@redhat.com>
```

### Comparing `wrapanapi-3.5.8/ChangeLog` & `wrapanapi-3.5.9/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+3.5.9
+-----
+
+* EC2: Remove all unused Volumes, IPs and NICs from a region
+
 3.5.8
 -----
 
 * Remove all unused Disks, PIPs and NICs from a resource group
 * update botocore version
 
 3.5.7
@@ -151,18 +156,13 @@
 -----
 
 * [RFR] Add ability to create a snapshot for SCVirtualMachine (#374)
 
 3.1.3
 -----
 
-* Fix TypeError when listing IPs in rhv 4.3
 * Fixes required for test\_provision\_with\_boot\_volume
 
 3.1.2
 -----
 
 * [RFR] Add Support For Datastore Clusters for Vmware (#368)
-
-3.1.1
------
-
```

### Comparing `wrapanapi-3.5.8/LICENSE` & `wrapanapi-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/PKG-INFO` & `wrapanapi-3.5.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,142 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: wrapanapi
-Version: 3.5.8
+Version: 3.5.9
 Summary: A base system for provider management
 Home-page: UNKNOWN
 Author: Peter Savage
 Author-email: psavage@redhat.com
 License: UNKNOWN
-Description: .. image:: https://landscape.io/github/ManageIQ/wrapanapi/master/landscape.svg?style=fla
-           :scale: 50 %
-           :alt: Health Status
-           :align: left
-           :target: (https://landscape.io/github/ManageIQ/wrapanapi/master
-        .. image:: https://coveralls.io/repos/ManageIQ/wrapanapi/badge.svg?branch=master&service=github
-           :scale: 50 %
-           :alt: Coverage Status
-           :align: left
-           :target: https://coveralls.io/github/ManageIQ/wrapanapi?branch=master
-        .. image:: https://travis-ci.org/ManageIQ/wrapanapi.svg
-           :scale: 50 %
-           :alt: Build Status
-           :align: left
-           :target: https://travis-ci.org/ManageIQ/wrapanapi
-        .. image:: https://img.shields.io/pypi/pyversions/wrapanapi.svg
-           :scale: 50 %
-           :alt: Python Supported Versions
-           :align: left
-           :target: https://pypi.org/project/wrapanapi/
-        
-        
-        wrapanapi
-        ==========
-        
-        Introduction
-        ------------
-        wrapanapi is a simple virtualization client with support (in varying degrees) for the following
-        
-        * Red Hat Enterprize Virtualization (RHEV)
-        * Red Hat Openstack (RHOS)
-        * Red Hat Openshift
-        * Openshift
-        * VMware vCenter
-        * Microsoft SCVMM
-        * Microsoft Azure
-        * Google Compute Engine
-        * Hawkular
-        * Amazon EC2
-        
-        It can be used to control virtualization clients and offers operations such as
-        
-        * list_vm (returns a list of vm_names)
-        * list_template (returns a list of templates/images)
-        * start_vm (starts a vm)
-        * stop_vm (stops a vm)
-        
-        Though conceptually names differ between cloud and infrastructure virtualization technologies (e.g. instance/vm)
-        it was decided to stick to one representation in the codebase and interface to give a singlar API across
-        all systems.
-        
-        Installation
-        ------------
-        
-        Wrapanapi can be installed via `pip` as `pip install wrapanapi`
-        It is always a good idea to use virtualenv to install pip packages.
-        
-        For Linux Users, Depending on the distribution you are using, you may need to install following packages
-        (or similar for your distribution of linux):
-        
-        * libcurl-devel
-        * openssl-devel
-        * libxml2-devel
-        * libxml2-static
-        * gcc
-        
-        If you are in doubt if you really need these packages, you will hit errors during installation that will make it
-        apparent for you to figure out that you need it.
-        Pycurl is a one such package that requires you to install packages like ones listed above, you can read more about it at
-        http://pycurl.io/docs/latest/install.html
-        
-        Usage
-        -----
-        Each management system is invoked usually with a hostname and some credentials
-        
-        .. code-block:: python
-        
-          from wrapanapi.virtualcenter import VMWareSystem
-          
-          system = VMWareSystem(hostname='10.0.0.0', username="root", password="password")
-          system.list_vm()
-        
-        Adding a new Management System
-        ------------------------------
-        A management system should extend the Base class, and supply "Not Implemented" raises for items which
-        it doesn't support. This behaviour may change in the future as more and more diverse management systems.
-        
-        .. code-block:: python
-        
-          from base import WrapanapiAPIBase
-        
-          class RHEVMSystem(WrapanapiAPIBase):
-          
-            _stats_available = {
-              'num_vm': lambda self: self.api.get_summary().get_vms().total,
-              'num_host': lambda self: len(self.list_host()),
-              'num_cluster': lambda self: len(self.list_cluster()),
-              'num_template': lambda self: len(self.list_template()),
-              'num_datastore': lambda self: len(self.list_datastore()),
-            }
-          
-            def __init__(self, hostname, username, password, **kwargs):
-              super(RHEVMSystem, self).__init__(kwargs)
-        
-        The call to ``super`` is necessary to set up the logger if noe has not been passed in with the ``logger``
-        keyword.
-        
-        The developer can then add their own methods to interact with their own management system. Commonly accessible
-        statistics are generally all named the same across management systems. In this way we can treat multiple management
-        systems the same and use an identical method to check the number of vms on a RHEV system, to a VMware system.
-        
-        Exceptions currently sit in a single module, this will probably change later with each management system having it's own
-        package and exceptions stored there.
-        
-        This module was originally developed for assisting in the ManageIQ testing team.
-        
-        Contributing
-        ------------
-        The guidelines to follow for this project can be found in the 
-        cfme `dev_guide <http://cfme-tests.readthedocs.org/guides/dev_guide.html>`_.
-        
-        
 Keywords: setup,distutils
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+.. image:: https://landscape.io/github/ManageIQ/wrapanapi/master/landscape.svg?style=fla
+   :scale: 50 %
+   :alt: Health Status
+   :align: left
+   :target: (https://landscape.io/github/ManageIQ/wrapanapi/master
+.. image:: https://coveralls.io/repos/ManageIQ/wrapanapi/badge.svg?branch=master&service=github
+   :scale: 50 %
+   :alt: Coverage Status
+   :align: left
+   :target: https://coveralls.io/github/ManageIQ/wrapanapi?branch=master
+.. image:: https://travis-ci.org/ManageIQ/wrapanapi.svg
+   :scale: 50 %
+   :alt: Build Status
+   :align: left
+   :target: https://travis-ci.org/ManageIQ/wrapanapi
+.. image:: https://img.shields.io/pypi/pyversions/wrapanapi.svg
+   :scale: 50 %
+   :alt: Python Supported Versions
+   :align: left
+   :target: https://pypi.org/project/wrapanapi/
+
+
+wrapanapi
+==========
+
+Introduction
+------------
+wrapanapi is a simple virtualization client with support (in varying degrees) for the following
+
+* Red Hat Enterprize Virtualization (RHEV)
+* Red Hat Openstack (RHOS)
+* Red Hat Openshift
+* Openshift
+* VMware vCenter
+* Microsoft SCVMM
+* Microsoft Azure
+* Google Compute Engine
+* Hawkular
+* Amazon EC2
+
+It can be used to control virtualization clients and offers operations such as
+
+* list_vm (returns a list of vm_names)
+* list_template (returns a list of templates/images)
+* start_vm (starts a vm)
+* stop_vm (stops a vm)
+
+Though conceptually names differ between cloud and infrastructure virtualization technologies (e.g. instance/vm)
+it was decided to stick to one representation in the codebase and interface to give a singlar API across
+all systems.
+
+Installation
+------------
+
+Wrapanapi can be installed via `pip` as `pip install wrapanapi`
+It is always a good idea to use virtualenv to install pip packages.
+
+For Linux Users, Depending on the distribution you are using, you may need to install following packages
+(or similar for your distribution of linux):
+
+* libcurl-devel
+* openssl-devel
+* libxml2-devel
+* libxml2-static
+* gcc
+
+If you are in doubt if you really need these packages, you will hit errors during installation that will make it
+apparent for you to figure out that you need it.
+Pycurl is a one such package that requires you to install packages like ones listed above, you can read more about it at
+http://pycurl.io/docs/latest/install.html
+
+Usage
+-----
+Each management system is invoked usually with a hostname and some credentials
+
+.. code-block:: python
+
+  from wrapanapi.virtualcenter import VMWareSystem
+  
+  system = VMWareSystem(hostname='10.0.0.0', username="root", password="password")
+  system.list_vm()
+
+Adding a new Management System
+------------------------------
+A management system should extend the Base class, and supply "Not Implemented" raises for items which
+it doesn't support. This behaviour may change in the future as more and more diverse management systems.
+
+.. code-block:: python
+
+  from base import WrapanapiAPIBase
+
+  class RHEVMSystem(WrapanapiAPIBase):
+  
+    _stats_available = {
+      'num_vm': lambda self: self.api.get_summary().get_vms().total,
+      'num_host': lambda self: len(self.list_host()),
+      'num_cluster': lambda self: len(self.list_cluster()),
+      'num_template': lambda self: len(self.list_template()),
+      'num_datastore': lambda self: len(self.list_datastore()),
+    }
+  
+    def __init__(self, hostname, username, password, **kwargs):
+      super(RHEVMSystem, self).__init__(kwargs)
+
+The call to ``super`` is necessary to set up the logger if noe has not been passed in with the ``logger``
+keyword.
+
+The developer can then add their own methods to interact with their own management system. Commonly accessible
+statistics are generally all named the same across management systems. In this way we can treat multiple management
+systems the same and use an identical method to check the number of vms on a RHEV system, to a VMware system.
+
+Exceptions currently sit in a single module, this will probably change later with each management system having it's own
+package and exceptions stored there.
+
+This module was originally developed for assisting in the ManageIQ testing team.
+
+Contributing
+------------
+The guidelines to follow for this project can be found in the 
+cfme `dev_guide <http://cfme-tests.readthedocs.org/guides/dev_guide.html>`_.
+
+
+
```

### Comparing `wrapanapi-3.5.8/README.rst` & `wrapanapi-3.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/setup.cfg` & `wrapanapi-3.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/alerts/events.json` & `wrapanapi-3.5.9/tests/resources/hawkular/alerts/events.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Datasource/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/Datasource/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Queue/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Queue/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Topic/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/JMS Topic/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/XA Datasource/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes/XA Datasource/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/328c17e1-c97f-4583-89d8-73feb0cf47f6/resourceTypes.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Datasource/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Datasource/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Deployment/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/Deployment/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Queue/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Queue/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Topic/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/JMS Topic/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/SubDeployment/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes/SubDeployment/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/5ea2d44a-6b07-424b-b54e-0b4c798d1353/resourceTypes.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Datasource/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/Datasource/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Queue/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Queue/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Topic/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/JMS Topic/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/XA Datasource/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes/XA Datasource/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/c22fb9d6-0ffc-42cd-bf5b-e1d046398fe5/resourceTypes.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/Domain Server Group/resources.json` & `wrapanapi-3.5.9/tests/resources/hawkular/inventory/feeds/master.eap7%20domain/resourceTypes/Domain Server Group/resources.json`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/test_hawkular.py` & `wrapanapi-3.5.9/tests/test_hawkular.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/tests/test_vm_and_template_systems.py` & `wrapanapi-3.5.9/tests/test_vm_and_template_systems.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/__init__.py` & `wrapanapi-3.5.9/wrapanapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/clients/rest_client.py` & `wrapanapi-3.5.9/wrapanapi/clients/rest_client.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/clients/websocket_client.py` & `wrapanapi-3.5.9/wrapanapi/clients/websocket_client.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/__init__.py` & `wrapanapi-3.5.9/wrapanapi/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/base.py` & `wrapanapi-3.5.9/wrapanapi/entities/base.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/network.py` & `wrapanapi-3.5.9/wrapanapi/entities/network.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/physical_container.py` & `wrapanapi-3.5.9/wrapanapi/entities/physical_container.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/server.py` & `wrapanapi-3.5.9/wrapanapi/entities/server.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/stack.py` & `wrapanapi-3.5.9/wrapanapi/entities/stack.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/template.py` & `wrapanapi-3.5.9/wrapanapi/entities/template.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/vm.py` & `wrapanapi-3.5.9/wrapanapi/entities/vm.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/entities/volume.py` & `wrapanapi-3.5.9/wrapanapi/entities/volume.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/exceptions.py` & `wrapanapi-3.5.9/wrapanapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/__init__.py` & `wrapanapi-3.5.9/wrapanapi/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/base.py` & `wrapanapi-3.5.9/wrapanapi/systems/base.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/container/rhopenshift.py` & `wrapanapi-3.5.9/wrapanapi/systems/container/rhopenshift.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/ec2.py` & `wrapanapi-3.5.9/wrapanapi/systems/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1536,7 +1536,62 @@
                                                                     }
                                                             }
                                                         ])
             return ami_id
         except Exception:
             self.logger.exception("Creation of image from snapshot '%s' failed.", snapshot_id)
             return False
+
+    def remove_network_interface_by_id(self, nic_id):
+        try:
+            self.ec2_connection.delete_network_interface(NetworkInterfaceId=nic_id)
+            return True
+        except Exception:
+            self.logger.exception(f"Removal of Network interface id {nic_id} failed.")
+            return False
+
+    def remove_volume_by_id(self, volume_id):
+        try:
+            self.ec2_connection.delete_volume(VolumeId=volume_id)
+            return True
+        except Exception:
+            self.logger.exception(f"Removal of Volume by id {volume_id} failed.")
+            return False
+
+    def remove_all_unused_nics(self):
+        """
+        Remove all unused Network interfaces in given region
+
+        Returns: None
+        """
+        all_unused_nics = self.get_all_unused_network_interfaces()
+        for nic in all_unused_nics:
+            self.remove_network_interface_by_id(nic_id=nic['NetworkInterfaceId'])
+
+    def remove_all_unused_volumes(self):
+        """
+        Remove all unused Volumes in given region
+
+        Returns: None
+        """
+        all_unused_volumes = self.get_all_unattached_volumes()
+        for volume in all_unused_volumes:
+            self.remove_volume_by_id(volume_id=volume['VolumeId'])
+
+    def remove_all_unused_ips(self):
+        """
+        Remove all disassociated addresses in given region
+
+        Returns: None
+        """
+        all_unused_ips = self.get_all_disassociated_addresses()
+        for ip in all_unused_ips:
+            self.release_vpc_address(alloc_id=ip['AllocationId'])
+
+    def cleanup_resources(self):
+        """
+        Removes all unused NICs, Volumes and IP addresses
+        """
+        self.logger.info("cleanup: Removing all unused NICs/Volumes/IPs in resource group")
+        self.remove_all_unused_nics()
+        self.remove_all_unused_volumes()
+        self.remove_all_unused_ips()
```

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/google.py` & `wrapanapi-3.5.9/wrapanapi/systems/google.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/hawkular.py` & `wrapanapi-3.5.9/wrapanapi/systems/hawkular.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/lenovo.py` & `wrapanapi-3.5.9/wrapanapi/systems/lenovo.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/msazure.py` & `wrapanapi-3.5.9/wrapanapi/systems/msazure.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/nuage.py` & `wrapanapi-3.5.9/wrapanapi/systems/nuage.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/openstack.py` & `wrapanapi-3.5.9/wrapanapi/systems/openstack.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/openstack_infra.py` & `wrapanapi-3.5.9/wrapanapi/systems/openstack_infra.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/redfish.py` & `wrapanapi-3.5.9/wrapanapi/systems/redfish.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/rhevm.py` & `wrapanapi-3.5.9/wrapanapi/systems/rhevm.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/scvmm.py` & `wrapanapi-3.5.9/wrapanapi/systems/scvmm.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/vcloud.py` & `wrapanapi-3.5.9/wrapanapi/systems/vcloud.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/systems/virtualcenter.py` & `wrapanapi-3.5.9/wrapanapi/systems/virtualcenter.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/utils/json_utils.py` & `wrapanapi-3.5.9/wrapanapi/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi/utils/logger_mixin.py` & `wrapanapi-3.5.9/wrapanapi/utils/logger_mixin.py`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi.egg-info/PKG-INFO` & `wrapanapi-3.5.9/wrapanapi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,142 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: wrapanapi
-Version: 3.5.8
+Version: 3.5.9
 Summary: A base system for provider management
 Home-page: UNKNOWN
 Author: Peter Savage
 Author-email: psavage@redhat.com
 License: UNKNOWN
-Description: .. image:: https://landscape.io/github/ManageIQ/wrapanapi/master/landscape.svg?style=fla
-           :scale: 50 %
-           :alt: Health Status
-           :align: left
-           :target: (https://landscape.io/github/ManageIQ/wrapanapi/master
-        .. image:: https://coveralls.io/repos/ManageIQ/wrapanapi/badge.svg?branch=master&service=github
-           :scale: 50 %
-           :alt: Coverage Status
-           :align: left
-           :target: https://coveralls.io/github/ManageIQ/wrapanapi?branch=master
-        .. image:: https://travis-ci.org/ManageIQ/wrapanapi.svg
-           :scale: 50 %
-           :alt: Build Status
-           :align: left
-           :target: https://travis-ci.org/ManageIQ/wrapanapi
-        .. image:: https://img.shields.io/pypi/pyversions/wrapanapi.svg
-           :scale: 50 %
-           :alt: Python Supported Versions
-           :align: left
-           :target: https://pypi.org/project/wrapanapi/
-        
-        
-        wrapanapi
-        ==========
-        
-        Introduction
-        ------------
-        wrapanapi is a simple virtualization client with support (in varying degrees) for the following
-        
-        * Red Hat Enterprize Virtualization (RHEV)
-        * Red Hat Openstack (RHOS)
-        * Red Hat Openshift
-        * Openshift
-        * VMware vCenter
-        * Microsoft SCVMM
-        * Microsoft Azure
-        * Google Compute Engine
-        * Hawkular
-        * Amazon EC2
-        
-        It can be used to control virtualization clients and offers operations such as
-        
-        * list_vm (returns a list of vm_names)
-        * list_template (returns a list of templates/images)
-        * start_vm (starts a vm)
-        * stop_vm (stops a vm)
-        
-        Though conceptually names differ between cloud and infrastructure virtualization technologies (e.g. instance/vm)
-        it was decided to stick to one representation in the codebase and interface to give a singlar API across
-        all systems.
-        
-        Installation
-        ------------
-        
-        Wrapanapi can be installed via `pip` as `pip install wrapanapi`
-        It is always a good idea to use virtualenv to install pip packages.
-        
-        For Linux Users, Depending on the distribution you are using, you may need to install following packages
-        (or similar for your distribution of linux):
-        
-        * libcurl-devel
-        * openssl-devel
-        * libxml2-devel
-        * libxml2-static
-        * gcc
-        
-        If you are in doubt if you really need these packages, you will hit errors during installation that will make it
-        apparent for you to figure out that you need it.
-        Pycurl is a one such package that requires you to install packages like ones listed above, you can read more about it at
-        http://pycurl.io/docs/latest/install.html
-        
-        Usage
-        -----
-        Each management system is invoked usually with a hostname and some credentials
-        
-        .. code-block:: python
-        
-          from wrapanapi.virtualcenter import VMWareSystem
-          
-          system = VMWareSystem(hostname='10.0.0.0', username="root", password="password")
-          system.list_vm()
-        
-        Adding a new Management System
-        ------------------------------
-        A management system should extend the Base class, and supply "Not Implemented" raises for items which
-        it doesn't support. This behaviour may change in the future as more and more diverse management systems.
-        
-        .. code-block:: python
-        
-          from base import WrapanapiAPIBase
-        
-          class RHEVMSystem(WrapanapiAPIBase):
-          
-            _stats_available = {
-              'num_vm': lambda self: self.api.get_summary().get_vms().total,
-              'num_host': lambda self: len(self.list_host()),
-              'num_cluster': lambda self: len(self.list_cluster()),
-              'num_template': lambda self: len(self.list_template()),
-              'num_datastore': lambda self: len(self.list_datastore()),
-            }
-          
-            def __init__(self, hostname, username, password, **kwargs):
-              super(RHEVMSystem, self).__init__(kwargs)
-        
-        The call to ``super`` is necessary to set up the logger if noe has not been passed in with the ``logger``
-        keyword.
-        
-        The developer can then add their own methods to interact with their own management system. Commonly accessible
-        statistics are generally all named the same across management systems. In this way we can treat multiple management
-        systems the same and use an identical method to check the number of vms on a RHEV system, to a VMware system.
-        
-        Exceptions currently sit in a single module, this will probably change later with each management system having it's own
-        package and exceptions stored there.
-        
-        This module was originally developed for assisting in the ManageIQ testing team.
-        
-        Contributing
-        ------------
-        The guidelines to follow for this project can be found in the 
-        cfme `dev_guide <http://cfme-tests.readthedocs.org/guides/dev_guide.html>`_.
-        
-        
 Keywords: setup,distutils
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+.. image:: https://landscape.io/github/ManageIQ/wrapanapi/master/landscape.svg?style=fla
+   :scale: 50 %
+   :alt: Health Status
+   :align: left
+   :target: (https://landscape.io/github/ManageIQ/wrapanapi/master
+.. image:: https://coveralls.io/repos/ManageIQ/wrapanapi/badge.svg?branch=master&service=github
+   :scale: 50 %
+   :alt: Coverage Status
+   :align: left
+   :target: https://coveralls.io/github/ManageIQ/wrapanapi?branch=master
+.. image:: https://travis-ci.org/ManageIQ/wrapanapi.svg
+   :scale: 50 %
+   :alt: Build Status
+   :align: left
+   :target: https://travis-ci.org/ManageIQ/wrapanapi
+.. image:: https://img.shields.io/pypi/pyversions/wrapanapi.svg
+   :scale: 50 %
+   :alt: Python Supported Versions
+   :align: left
+   :target: https://pypi.org/project/wrapanapi/
+
+
+wrapanapi
+==========
+
+Introduction
+------------
+wrapanapi is a simple virtualization client with support (in varying degrees) for the following
+
+* Red Hat Enterprize Virtualization (RHEV)
+* Red Hat Openstack (RHOS)
+* Red Hat Openshift
+* Openshift
+* VMware vCenter
+* Microsoft SCVMM
+* Microsoft Azure
+* Google Compute Engine
+* Hawkular
+* Amazon EC2
+
+It can be used to control virtualization clients and offers operations such as
+
+* list_vm (returns a list of vm_names)
+* list_template (returns a list of templates/images)
+* start_vm (starts a vm)
+* stop_vm (stops a vm)
+
+Though conceptually names differ between cloud and infrastructure virtualization technologies (e.g. instance/vm)
+it was decided to stick to one representation in the codebase and interface to give a singlar API across
+all systems.
+
+Installation
+------------
+
+Wrapanapi can be installed via `pip` as `pip install wrapanapi`
+It is always a good idea to use virtualenv to install pip packages.
+
+For Linux Users, Depending on the distribution you are using, you may need to install following packages
+(or similar for your distribution of linux):
+
+* libcurl-devel
+* openssl-devel
+* libxml2-devel
+* libxml2-static
+* gcc
+
+If you are in doubt if you really need these packages, you will hit errors during installation that will make it
+apparent for you to figure out that you need it.
+Pycurl is a one such package that requires you to install packages like ones listed above, you can read more about it at
+http://pycurl.io/docs/latest/install.html
+
+Usage
+-----
+Each management system is invoked usually with a hostname and some credentials
+
+.. code-block:: python
+
+  from wrapanapi.virtualcenter import VMWareSystem
+  
+  system = VMWareSystem(hostname='10.0.0.0', username="root", password="password")
+  system.list_vm()
+
+Adding a new Management System
+------------------------------
+A management system should extend the Base class, and supply "Not Implemented" raises for items which
+it doesn't support. This behaviour may change in the future as more and more diverse management systems.
+
+.. code-block:: python
+
+  from base import WrapanapiAPIBase
+
+  class RHEVMSystem(WrapanapiAPIBase):
+  
+    _stats_available = {
+      'num_vm': lambda self: self.api.get_summary().get_vms().total,
+      'num_host': lambda self: len(self.list_host()),
+      'num_cluster': lambda self: len(self.list_cluster()),
+      'num_template': lambda self: len(self.list_template()),
+      'num_datastore': lambda self: len(self.list_datastore()),
+    }
+  
+    def __init__(self, hostname, username, password, **kwargs):
+      super(RHEVMSystem, self).__init__(kwargs)
+
+The call to ``super`` is necessary to set up the logger if noe has not been passed in with the ``logger``
+keyword.
+
+The developer can then add their own methods to interact with their own management system. Commonly accessible
+statistics are generally all named the same across management systems. In this way we can treat multiple management
+systems the same and use an identical method to check the number of vms on a RHEV system, to a VMware system.
+
+Exceptions currently sit in a single module, this will probably change later with each management system having it's own
+package and exceptions stored there.
+
+This module was originally developed for assisting in the ManageIQ testing team.
+
+Contributing
+------------
+The guidelines to follow for this project can be found in the 
+cfme `dev_guide <http://cfme-tests.readthedocs.org/guides/dev_guide.html>`_.
+
+
+
```

### Comparing `wrapanapi-3.5.8/wrapanapi.egg-info/SOURCES.txt` & `wrapanapi-3.5.9/wrapanapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wrapanapi-3.5.8/wrapanapi.egg-info/requires.txt` & `wrapanapi-3.5.9/wrapanapi.egg-info/requires.txt`

 * *Files identical despite different names*

