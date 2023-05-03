# Comparing `tmp/lava_nc-0.7.0.tar.gz` & `tmp/lava_nc-0.7.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lava_nc-0.7.0.tar", max compression
+gzip compressed data, was "lava_nc-0.7.0.post1.tar", max compression
```

## Comparing `lava_nc-0.7.0.tar` & `lava_nc-0.7.0.post1.tar`

### file list

```diff
@@ -1,225 +1,225 @@
--rw-r--r--   0        0        0      333 2023-04-06 01:33:58.675405 lava_nc-0.7.0/LICENSE
--rw-r--r--   0        0        0     4809 2023-05-02 02:50:04.773890 lava_nc-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    26529 2023-04-06 01:33:58.677146 lava_nc-0.7.0/src/lava/magma/compiler/LICENSE
--rw-r--r--   0        0        0     5550 2023-04-06 01:33:58.677313 lava_nc-0.7.0/src/lava/magma/compiler/builders/channel_builder.py
--rw-r--r--   0        0        0     4236 2023-04-06 01:33:58.677430 lava_nc-0.7.0/src/lava/magma/compiler/builders/interfaces.py
--rw-r--r--   0        0        0    15527 2023-05-02 02:26:25.479841 lava_nc-0.7.0/src/lava/magma/compiler/builders/py_builder.py
--rw-r--r--   0        0        0     4937 2023-04-06 01:33:58.677670 lava_nc-0.7.0/src/lava/magma/compiler/builders/runtimeservice_builder.py
--rw-r--r--   0        0        0     4607 2023-04-21 18:31:56.277915 lava_nc-0.7.0/src/lava/magma/compiler/channel_map.py
--rw-r--r--   0        0        0     1372 2023-04-06 01:33:58.677919 lava_nc-0.7.0/src/lava/magma/compiler/channels/interfaces.py
--rw-r--r--   0        0        0    10521 2023-04-21 20:07:13.015569 lava_nc-0.7.0/src/lava/magma/compiler/channels/pypychannel.py
--rw-r--r--   0        0        0    35450 2023-04-06 01:33:58.678374 lava_nc-0.7.0/src/lava/magma/compiler/compiler.py
--rw-r--r--   0        0        0    44872 2023-04-06 01:33:58.678597 lava_nc-0.7.0/src/lava/magma/compiler/compiler_graphs.py
--rw-r--r--   0        0        0     1550 2023-04-06 01:33:58.678711 lava_nc-0.7.0/src/lava/magma/compiler/compiler_utils.py
--rw-r--r--   0        0        0      573 2023-04-06 01:33:58.678794 lava_nc-0.7.0/src/lava/magma/compiler/exceptions.py
--rw-r--r--   0        0        0     1778 2023-04-06 01:33:58.678886 lava_nc-0.7.0/src/lava/magma/compiler/executable.py
--rw-r--r--   0        0        0      721 2023-04-06 01:33:58.678969 lava_nc-0.7.0/src/lava/magma/compiler/mappable_interface.py
--rw-r--r--   0        0        0     7583 2023-04-06 01:33:58.679057 lava_nc-0.7.0/src/lava/magma/compiler/mapper.py
--rw-r--r--   0        0        0     2250 2023-04-06 01:33:58.679131 lava_nc-0.7.0/src/lava/magma/compiler/node.py
--rw-r--r--   0        0        0      514 2023-04-06 01:33:58.679262 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/address.py
--rw-r--r--   0        0        0    10380 2023-04-06 01:33:58.679371 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/channel_builders_factory.py
--rw-r--r--   0        0        0     2390 2023-04-06 01:33:58.679457 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/channel_map_updater.py
--rw-r--r--   0        0        0      696 2023-04-06 01:33:58.679546 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/constants.py
--rw-r--r--   0        0        0      769 2023-04-06 01:33:58.679630 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/exceptions.py
--rw-r--r--   0        0        0     2086 2023-04-06 01:33:58.679719 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/interfaces.py
--rw-r--r--   0        0        0     7543 2023-04-06 01:33:58.679858 lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py
--rw-r--r--   0        0        0     4153 2023-04-06 01:33:58.679947 lava_nc-0.7.0/src/lava/magma/compiler/utils.py
--rw-r--r--   0        0        0     5711 2023-05-02 02:26:25.480541 lava_nc-0.7.0/src/lava/magma/compiler/var_model.py
--rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.680174 lava_nc-0.7.0/src/lava/magma/core/LICENSE
--rw-r--r--   0        0        0     1613 2023-04-06 01:33:58.680260 lava_nc-0.7.0/src/lava/magma/core/callback_fx.py
--rw-r--r--   0        0        0     6408 2023-04-06 01:33:58.680350 lava_nc-0.7.0/src/lava/magma/core/decorator.py
--rw-r--r--   0        0        0     1999 2023-04-06 01:33:58.680477 lava_nc-0.7.0/src/lava/magma/core/learning/constants.py
--rw-r--r--   0        0        0    23198 2023-04-06 01:33:58.680631 lava_nc-0.7.0/src/lava/magma/core/learning/learning_rule.py
--rw-r--r--   0        0        0    12270 2023-04-06 01:33:58.680751 lava_nc-0.7.0/src/lava/magma/core/learning/learning_rule_applier.py
--rw-r--r--   0        0        0    23302 2023-04-06 01:33:58.680867 lava_nc-0.7.0/src/lava/magma/core/learning/product_series.py
--rw-r--r--   0        0        0     4603 2023-04-06 01:33:58.680951 lava_nc-0.7.0/src/lava/magma/core/learning/random.py
--rw-r--r--   0        0        0      685 2023-04-06 01:33:58.681022 lava_nc-0.7.0/src/lava/magma/core/learning/string_symbols.py
--rw-r--r--   0        0        0    23789 2023-04-06 01:33:58.681133 lava_nc-0.7.0/src/lava/magma/core/learning/symbolic_equation.py
--rw-r--r--   0        0        0     2068 2023-04-06 01:33:58.681231 lava_nc-0.7.0/src/lava/magma/core/learning/utils.py
--rw-r--r--   0        0        0     1084 2023-04-06 01:33:58.681344 lava_nc-0.7.0/src/lava/magma/core/model/interfaces.py
--rw-r--r--   0        0        0     5193 2023-04-06 01:33:58.681438 lava_nc-0.7.0/src/lava/magma/core/model/model.py
--rw-r--r--   0        0        0    52944 2023-05-02 02:26:25.481186 lava_nc-0.7.0/src/lava/magma/core/model/py/connection.py
--rw-r--r--   0        0        0    25160 2023-05-02 02:26:25.482275 lava_nc-0.7.0/src/lava/magma/core/model/py/model.py
--rw-r--r--   0        0        0     3100 2023-04-06 01:33:58.681910 lava_nc-0.7.0/src/lava/magma/core/model/py/neuron.py
--rw-r--r--   0        0        0    36060 2023-04-21 19:23:43.524374 lava_nc-0.7.0/src/lava/magma/core/model/py/ports.py
--rw-r--r--   0        0        0      458 2023-04-06 01:33:58.682166 lava_nc-0.7.0/src/lava/magma/core/model/py/type.py
--rw-r--r--   0        0        0      352 2023-04-06 01:33:58.682232 lava_nc-0.7.0/src/lava/magma/core/model/spike_type.py
--rw-r--r--   0        0        0     2914 2023-04-06 01:33:58.682348 lava_nc-0.7.0/src/lava/magma/core/model/sub/model.py
--rw-r--r--   0        0        0     3781 2023-04-06 01:33:58.682462 lava_nc-0.7.0/src/lava/magma/core/process/connection.py
--rw-r--r--   0        0        0     2285 2023-04-06 01:33:58.682537 lava_nc-0.7.0/src/lava/magma/core/process/interfaces.py
--rw-r--r--   0        0        0      194 2023-04-06 01:33:58.682613 lava_nc-0.7.0/src/lava/magma/core/process/message_interface_enum.py
--rw-r--r--   0        0        0     1690 2023-04-06 01:33:58.682686 lava_nc-0.7.0/src/lava/magma/core/process/neuron.py
--rw-r--r--   0        0        0     2763 2023-04-06 01:33:58.682815 lava_nc-0.7.0/src/lava/magma/core/process/ports/exceptions.py
--rw-r--r--   0        0        0    38136 2023-04-06 01:33:58.682963 lava_nc-0.7.0/src/lava/magma/core/process/ports/ports.py
--rw-r--r--   0        0        0      459 2023-04-06 01:33:58.683040 lava_nc-0.7.0/src/lava/magma/core/process/ports/reduce_ops.py
--rw-r--r--   0        0        0    23800 2023-05-01 20:07:22.307395 lava_nc-0.7.0/src/lava/magma/core/process/process.py
--rw-r--r--   0        0        0     7993 2023-05-02 02:26:25.483107 lava_nc-0.7.0/src/lava/magma/core/process/variable.py
--rw-r--r--   0        0        0     3767 2023-04-06 01:33:58.683596 lava_nc-0.7.0/src/lava/magma/core/resources.py
--rw-r--r--   0        0        0     1502 2023-04-06 01:33:58.683683 lava_nc-0.7.0/src/lava/magma/core/run_conditions.py
--rw-r--r--   0        0        0    22433 2023-04-06 01:33:58.683817 lava_nc-0.7.0/src/lava/magma/core/run_configs.py
--rw-r--r--   0        0        0     1506 2023-04-06 01:33:58.683976 lava_nc-0.7.0/src/lava/magma/core/sync/domain.py
--rw-r--r--   0        0        0     1107 2023-04-06 01:33:58.684058 lava_nc-0.7.0/src/lava/magma/core/sync/protocol.py
--rw-r--r--   0        0        0     1523 2023-04-06 01:33:58.684181 lava_nc-0.7.0/src/lava/magma/core/sync/protocols/async_protocol.py
--rw-r--r--   0        0        0     4386 2023-04-06 01:33:58.684278 lava_nc-0.7.0/src/lava/magma/core/sync/protocols/loihi_protocol.py
--rw-r--r--   0        0        0    26529 2023-04-06 01:33:58.684503 lava_nc-0.7.0/src/lava/magma/runtime/LICENSE
--rw-r--r--   0        0        0      720 2023-04-06 01:33:58.684641 lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/factory.py
--rw-r--r--   0        0        0     1790 2023-04-06 01:33:58.684732 lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py
--rw-r--r--   0        0        0     4385 2023-04-06 01:33:58.684846 lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/multiprocessing.py
--rw-r--r--   0        0        0     1452 2023-04-06 01:33:58.684931 lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/nx.py
--rw-r--r--   0        0        0     1005 2023-04-06 01:33:58.685010 lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py
--rw-r--r--   0        0        0     2439 2023-04-06 01:33:58.685090 lava_nc-0.7.0/src/lava/magma/runtime/mgmt_token_enums.py
--rw-r--r--   0        0        0    22602 2023-05-02 02:26:25.483668 lava_nc-0.7.0/src/lava/magma/runtime/runtime.py
--rw-r--r--   0        0        0     8310 2023-04-06 01:33:58.685476 lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py
--rw-r--r--   0        0        0     1324 2023-04-06 01:33:58.685552 lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/enums.py
--rw-r--r--   0        0        0     1159 2023-04-06 01:33:58.685621 lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/interfaces.py
--rw-r--r--   0        0        0    22607 2023-04-21 18:31:56.278483 lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/runtime_service.py
--rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.685914 lava_nc-0.7.0/src/lava/proc/LICENSE
--rw-r--r--   0        0        0     2934 2023-04-06 01:33:58.686050 lava_nc-0.7.0/src/lava/proc/conv/models.py
--rw-r--r--   0        0        0     5954 2023-04-06 01:33:58.686146 lava_nc-0.7.0/src/lava/proc/conv/process.py
--rw-r--r--   0        0        0    16042 2023-04-06 01:33:58.686256 lava_nc-0.7.0/src/lava/proc/conv/utils.py
--rw-r--r--   0        0        0    14321 2023-05-02 02:26:25.484362 lava_nc-0.7.0/src/lava/proc/dense/models.py
--rw-r--r--   0        0        0    11177 2023-04-06 01:33:58.686544 lava_nc-0.7.0/src/lava/proc/dense/process.py
--rw-r--r--   0        0        0      236 2023-04-06 01:33:58.686665 lava_nc-0.7.0/src/lava/proc/io/__init__.py
--rw-r--r--   0        0        0     7532 2023-04-06 01:33:58.686757 lava_nc-0.7.0/src/lava/proc/io/dataloader.py
--rw-r--r--   0        0        0     9449 2023-04-06 01:33:58.686854 lava_nc-0.7.0/src/lava/proc/io/encoder.py
--rw-r--r--   0        0        0     2740 2023-04-06 01:33:58.686934 lava_nc-0.7.0/src/lava/proc/io/reset.py
--rw-r--r--   0        0        0     4831 2023-04-06 01:33:58.687026 lava_nc-0.7.0/src/lava/proc/io/sink.py
--rw-r--r--   0        0        0     2020 2023-04-06 01:33:58.687121 lava_nc-0.7.0/src/lava/proc/io/source.py
--rw-r--r--   0        0        0     3083 2023-04-06 01:33:58.687246 lava_nc-0.7.0/src/lava/proc/learning_rules/r_stdp_learning_rule.py
--rw-r--r--   0        0        0     1991 2023-04-06 01:33:58.687335 lava_nc-0.7.0/src/lava/proc/learning_rules/stdp_learning_rule.py
--rw-r--r--   0        0        0    18980 2023-04-06 01:33:58.687498 lava_nc-0.7.0/src/lava/proc/lif/models.py
--rw-r--r--   0        0        0    12911 2023-04-06 01:33:58.687776 lava_nc-0.7.0/src/lava/proc/lif/process.py
--rw-r--r--   0        0        0     2646 2023-04-06 01:33:58.687985 lava_nc-0.7.0/src/lava/proc/monitor/models.py
--rw-r--r--   0        0        0    11074 2023-04-06 01:33:58.688120 lava_nc-0.7.0/src/lava/proc/monitor/process.py
--rw-r--r--   0        0        0     1074 2023-04-06 01:33:58.688287 lava_nc-0.7.0/src/lava/proc/receiver/models.py
--rw-r--r--   0        0        0     1082 2023-04-06 01:33:58.688388 lava_nc-0.7.0/src/lava/proc/receiver/process.py
--rw-r--r--   0        0        0     5997 2023-04-06 01:33:58.688615 lava_nc-0.7.0/src/lava/proc/rf/models.py
--rw-r--r--   0        0        0     3591 2023-04-06 01:33:58.688718 lava_nc-0.7.0/src/lava/proc/rf/process.py
--rw-r--r--   0        0        0     2464 2023-04-06 01:33:58.688878 lava_nc-0.7.0/src/lava/proc/rf_iz/models.py
--rw-r--r--   0        0        0      181 2023-04-06 01:33:58.688964 lava_nc-0.7.0/src/lava/proc/rf_iz/process.py
--rw-r--r--   0        0        0     9115 2023-04-06 01:33:58.689150 lava_nc-0.7.0/src/lava/proc/sdn/models.py
--rw-r--r--   0        0        0     7382 2023-04-06 01:33:58.689241 lava_nc-0.7.0/src/lava/proc/sdn/process.py
--rw-r--r--   0        0        0     1431 2023-04-06 01:33:58.689397 lava_nc-0.7.0/src/lava/proc/spiker/models.py
--rw-r--r--   0        0        0     1461 2023-04-06 01:33:58.689504 lava_nc-0.7.0/src/lava/proc/spiker/process.py
--rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.689656 lava_nc-0.7.0/src/lava/utils/LICENSE
--rw-r--r--   0        0        0     4282 2023-04-06 01:33:58.689799 lava_nc-0.7.0/src/lava/utils/dataloader/mnist.py
--rw-r--r--   0        0        0     3254 2023-04-06 01:33:58.689888 lava_nc-0.7.0/src/lava/utils/plots.py
--rw-r--r--   0        0        0     1466 2023-04-06 01:33:58.689982 lava_nc-0.7.0/src/lava/utils/profiler.py
--rw-r--r--   0        0        0     1868 2023-04-06 01:33:58.690075 lava_nc-0.7.0/src/lava/utils/system.py
--rw-r--r--   0        0        0     7911 2023-05-02 02:26:25.484917 lava_nc-0.7.0/src/lava/utils/weightutils.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690282 lava_nc-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690406 lava_nc-0.7.0/tests/lava/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690509 lava_nc-0.7.0/tests/lava/magma/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690614 lava_nc-0.7.0/tests/lava/magma/compiler/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690724 lava_nc-0.7.0/tests/lava/magma/compiler/builders/__init__.py
--rw-r--r--   0        0        0    20945 2023-04-06 01:33:58.690880 lava_nc-0.7.0/tests/lava/magma/compiler/builders/test_builder.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690989 lava_nc-0.7.0/tests/lava/magma/compiler/channels/__init__.py
--rw-r--r--   0        0        0     5130 2023-04-06 01:33:58.691110 lava_nc-0.7.0/tests/lava/magma/compiler/channels/test_pypychannel.py
--rw-r--r--   0        0        0      113 2023-04-06 01:33:58.691236 lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/__init__.py
--rw-r--r--   0        0        0      113 2023-04-06 01:33:58.691352 lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/py/__init__.py
--rw-r--r--   0        0        0     8989 2023-04-06 01:33:58.691552 lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py
--rw-r--r--   0        0        0    18797 2023-04-06 01:33:58.691770 lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py
--rw-r--r--   0        0        0     3741 2023-04-06 01:33:58.691902 lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py
--rw-r--r--   0        0        0     2168 2023-04-06 01:33:58.692020 lava_nc-0.7.0/tests/lava/magma/compiler/test_channel_builder.py
--rw-r--r--   0        0        0     5376 2023-04-06 01:33:58.692139 lava_nc-0.7.0/tests/lava/magma/compiler/test_channel_map.py
--rw-r--r--   0        0        0    30646 2023-04-06 01:33:58.692310 lava_nc-0.7.0/tests/lava/magma/compiler/test_compiler.py
--rw-r--r--   0        0        0     2048 2023-04-06 01:33:58.692421 lava_nc-0.7.0/tests/lava/magma/compiler/test_node.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.692521 lava_nc-0.7.0/tests/lava/magma/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.692653 lava_nc-0.7.0/tests/lava/magma/core/learning/__init__.py
--rw-r--r--   0        0        0    50548 2023-04-21 19:48:24.469204 lava_nc-0.7.0/tests/lava/magma/core/learning/test_learning_rule.py
--rw-r--r--   0        0        0     5470 2023-04-06 01:33:58.693000 lava_nc-0.7.0/tests/lava/magma/core/learning/test_learning_rule_applier.py
--rw-r--r--   0        0        0    12737 2023-04-06 01:33:58.693092 lava_nc-0.7.0/tests/lava/magma/core/learning/test_product_series.py
--rw-r--r--   0        0        0     1905 2023-04-06 01:33:58.693182 lava_nc-0.7.0/tests/lava/magma/core/learning/test_random.py
--rw-r--r--   0        0        0    18180 2023-04-06 01:33:58.693301 lava_nc-0.7.0/tests/lava/magma/core/learning/test_symbolic_equation.py
--rw-r--r--   0        0        0     2230 2023-04-06 01:33:58.693422 lava_nc-0.7.0/tests/lava/magma/core/learning/test_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.693514 lava_nc-0.7.0/tests/lava/magma/core/model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.693637 lava_nc-0.7.0/tests/lava/magma/core/model/py/__init__.py
--rw-r--r--   0        0        0     5870 2023-04-06 01:33:58.693768 lava_nc-0.7.0/tests/lava/magma/core/model/py/test_model.py
--rw-r--r--   0        0        0     6898 2023-04-06 01:33:58.693882 lava_nc-0.7.0/tests/lava/magma/core/model/py/test_ports.py
--rw-r--r--   0        0        0     9117 2023-04-06 01:33:58.693984 lava_nc-0.7.0/tests/lava/magma/core/model/test_decorators.py
--rw-r--r--   0        0        0     1552 2023-04-06 01:33:58.694079 lava_nc-0.7.0/tests/lava/magma/core/model/test_sub_model.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.694163 lava_nc-0.7.0/tests/lava/magma/core/process/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.694270 lava_nc-0.7.0/tests/lava/magma/core/process/ports/__init__.py
--rw-r--r--   0        0        0    21231 2023-04-06 01:33:58.694426 lava_nc-0.7.0/tests/lava/magma/core/process/ports/test_ports.py
--rw-r--r--   0        0        0    34827 2023-04-06 01:33:58.694615 lava_nc-0.7.0/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py
--rw-r--r--   0        0        0     1377 2023-04-06 01:33:58.694728 lava_nc-0.7.0/tests/lava/magma/core/process/test_lif_dense_lif.py
--rw-r--r--   0        0        0    12308 2023-05-01 20:07:22.311061 lava_nc-0.7.0/tests/lava/magma/core/process/test_process.py
--rw-r--r--   0        0        0     4635 2023-04-06 01:33:58.694944 lava_nc-0.7.0/tests/lava/magma/core/process/test_variable.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.695026 lava_nc-0.7.0/tests/lava/magma/runtime/__init__.py
--rw-r--r--   0        0        0     3675 2023-04-06 01:33:58.695118 lava_nc-0.7.0/tests/lava/magma/runtime/test_async_protocol.py
--rw-r--r--   0        0        0     5783 2023-04-06 01:33:58.695207 lava_nc-0.7.0/tests/lava/magma/runtime/test_context_manager.py
--rw-r--r--   0        0        0     5174 2023-04-06 01:33:58.695315 lava_nc-0.7.0/tests/lava/magma/runtime/test_exception_handling.py
--rw-r--r--   0        0        0     2038 2023-04-06 01:33:58.695401 lava_nc-0.7.0/tests/lava/magma/runtime/test_get_set_non_determinism.py
--rw-r--r--   0        0        0     7469 2023-04-06 01:33:58.695490 lava_nc-0.7.0/tests/lava/magma/runtime/test_get_set_var.py
--rw-r--r--   0        0        0    10583 2023-04-06 01:33:58.695571 lava_nc-0.7.0/tests/lava/magma/runtime/test_io_ports.py
--rw-r--r--   0        0        0     1216 2023-04-06 01:33:58.695644 lava_nc-0.7.0/tests/lava/magma/runtime/test_leakage.py
--rw-r--r--   0        0        0     2238 2023-04-06 01:33:58.695722 lava_nc-0.7.0/tests/lava/magma/runtime/test_loihi_protocol.py
--rw-r--r--   0        0        0     3661 2023-04-06 01:33:58.695809 lava_nc-0.7.0/tests/lava/magma/runtime/test_loihi_with_async_protocol.py
--rw-r--r--   0        0        0     6682 2023-04-06 01:33:58.695909 lava_nc-0.7.0/tests/lava/magma/runtime/test_pause_requested_from_model.py
--rw-r--r--   0        0        0    14794 2023-04-06 01:33:58.696021 lava_nc-0.7.0/tests/lava/magma/runtime/test_ref_var_ports.py
--rw-r--r--   0        0        0     3822 2023-04-06 01:33:58.696113 lava_nc-0.7.0/tests/lava/magma/runtime/test_run_continuously_and_pause.py
--rw-r--r--   0        0        0     2829 2023-04-06 01:33:58.696205 lava_nc-0.7.0/tests/lava/magma/runtime/test_runtime.py
--rw-r--r--   0        0        0     2903 2023-04-06 01:33:58.696305 lava_nc-0.7.0/tests/lava/magma/runtime/test_runtime_service.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.696394 lava_nc-0.7.0/tests/lava/proc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.696506 lava_nc-0.7.0/tests/lava/proc/conv/__init__.py
--rw-r--r--   0        0        0   559366 2023-04-06 01:33:58.699158 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz
--rw-r--r--   0        0        0   590766 2023-04-06 01:33:58.702025 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz
--rw-r--r--   0        0        0   956638 2023-04-06 01:33:58.706484 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz
--rw-r--r--   0        0        0    68302 2023-04-06 01:33:58.706921 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz
--rw-r--r--   0        0        0   185142 2023-04-06 01:33:58.707804 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz
--rw-r--r--   0        0        0   409190 2023-04-06 01:33:58.709742 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz
--rw-r--r--   0        0        0  1888366 2023-04-06 01:33:58.718461 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz
--rw-r--r--   0        0        0  1790434 2023-04-06 01:33:58.726618 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz
--rw-r--r--   0        0        0   714214 2023-04-06 01:33:58.729733 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz
--rw-r--r--   0        0        0   670702 2023-04-06 01:33:58.732644 lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz
--rw-r--r--   0        0        0      999 2023-04-06 01:33:58.732750 lava_nc-0.7.0/tests/lava/proc/conv/test_process.py
--rw-r--r--   0        0        0     7343 2023-04-06 01:33:58.732856 lava_nc-0.7.0/tests/lava/proc/conv/test_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.732967 lava_nc-0.7.0/tests/lava/proc/dense/__init__.py
--rw-r--r--   0        0        0    53052 2023-04-06 01:33:58.733140 lava_nc-0.7.0/tests/lava/proc/dense/test_learning.py
--rw-r--r--   0        0        0    47972 2023-04-06 01:33:58.733283 lava_nc-0.7.0/tests/lava/proc/dense/test_models.py
--rw-r--r--   0        0        0     3666 2023-04-06 01:33:58.733380 lava_nc-0.7.0/tests/lava/proc/dense/test_process.py
--rw-r--r--   0        0        0    24791 2023-04-06 01:33:58.733484 lava_nc-0.7.0/tests/lava/proc/dense/test_stdp_sim.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.733576 lava_nc-0.7.0/tests/lava/proc/io/__init__.py
--rw-r--r--   0        0        0     7309 2023-04-06 01:33:58.733681 lava_nc-0.7.0/tests/lava/proc/io/test_dataloader.py
--rw-r--r--   0        0        0     2001 2023-04-06 01:33:58.733765 lava_nc-0.7.0/tests/lava/proc/io/test_source_sink.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.733835 lava_nc-0.7.0/tests/lava/proc/lif/__init__.py
--rw-r--r--   0        0        0    38490 2023-04-06 01:33:58.733977 lava_nc-0.7.0/tests/lava/proc/lif/test_models.py
--rw-r--r--   0        0        0     2213 2023-04-06 01:33:58.734066 lava_nc-0.7.0/tests/lava/proc/lif/test_process.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734148 lava_nc-0.7.0/tests/lava/proc/monitor/__init__.py
--rw-r--r--   0        0        0    12959 2023-04-06 01:33:58.734277 lava_nc-0.7.0/tests/lava/proc/monitor/test_monitors.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734365 lava_nc-0.7.0/tests/lava/proc/rf/__init__.py
--rw-r--r--   0        0        0     9354 2023-04-06 01:33:58.734466 lava_nc-0.7.0/tests/lava/proc/rf/test_models.py
--rw-r--r--   0        0        0      868 2023-04-06 01:33:58.734537 lava_nc-0.7.0/tests/lava/proc/rf/test_process.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734608 lava_nc-0.7.0/tests/lava/proc/rf_iz/__init__.py
--rw-r--r--   0        0        0     3563 2023-04-06 01:33:58.734725 lava_nc-0.7.0/tests/lava/proc/rf_iz/test_models.py
--rw-r--r--   0        0        0      901 2023-04-06 01:33:58.734787 lava_nc-0.7.0/tests/lava/proc/rf_iz/test_process.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734866 lava_nc-0.7.0/tests/lava/proc/sdn/__init__.py
--rw-r--r--   0        0        0     7800 2023-04-06 01:33:58.734963 lava_nc-0.7.0/tests/lava/proc/sdn/test_models.py
--rw-r--r--   0        0        0     1457 2023-04-06 01:33:58.735028 lava_nc-0.7.0/tests/lava/proc/sdn/test_process.py
--rw-r--r--   0        0        0     1710 2023-04-06 01:33:58.735146 lava_nc-0.7.0/tests/lava/proc/spiker/test_models.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.735219 lava_nc-0.7.0/tests/lava/test_utils/__init__.py
--rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.735306 lava_nc-0.7.0/tests/lava/test_utils/utils.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.735370 lava_nc-0.7.0/tests/lava/tutorials/__init__.py
--rw-r--r--   0        0        0     9340 2023-04-06 01:33:58.735509 lava_nc-0.7.0/tests/lava/tutorials/test_tutorials.py
--rw-r--r--   0        0        0        0 2023-04-06 01:33:58.735579 lava_nc-0.7.0/tests/lava/utils/__init__.py
--rw-r--r--   0        0        0     2165 2023-04-06 01:33:58.735665 lava_nc-0.7.0/tests/lava/utils/test_plots.py
--rw-r--r--   0        0        0    15761 2023-04-06 01:33:58.735757 lava_nc-0.7.0/tests/lava/utils/test_weightutils.py
--rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.735889 lava_nc-0.7.0/tutorials/LICENSE
--rw-r--r--   0        0        0     9985 2023-04-06 01:33:58.736024 lava_nc-0.7.0/tutorials/end_to_end/convert_params.py
--rw-r--r--   0        0        0   220767 2023-04-06 01:34:02.588053 lava_nc-0.7.0/tutorials/end_to_end/mnist_pretrained.npy
--rw-r--r--   0        0        0   276563 2023-04-21 19:07:38.860825 lava_nc-0.7.0/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb
--rw-r--r--   0        0        0    24427 2023-04-06 01:33:58.939317 lava_nc-0.7.0/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb
--rw-r--r--   0        0        0  1170553 2023-04-06 01:33:58.944705 lava_nc-0.7.0/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb
--rw-r--r--   0        0        0   566145 2023-04-06 01:33:58.947282 lava_nc-0.7.0/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb
--rw-r--r--   0        0        0    10117 2023-04-06 01:33:58.947469 lava_nc-0.7.0/tutorials/in_depth/three_factor_learning/utils.py
--rw-r--r--   0        0        0     6552 2023-04-06 01:33:58.947564 lava_nc-0.7.0/tutorials/in_depth/tutorial01_installing_lava.ipynb
--rw-r--r--   0        0        0    16399 2023-04-06 01:33:58.947718 lava_nc-0.7.0/tutorials/in_depth/tutorial02_processes.ipynb
--rw-r--r--   0        0        0    15539 2023-04-21 19:07:45.551328 lava_nc-0.7.0/tutorials/in_depth/tutorial03_process_models.ipynb
--rw-r--r--   0        0        0    14366 2023-04-06 01:33:58.948013 lava_nc-0.7.0/tutorials/in_depth/tutorial04_execution.ipynb
--rw-r--r--   0        0        0    13442 2023-04-06 01:33:58.948158 lava_nc-0.7.0/tutorials/in_depth/tutorial05_connect_processes.ipynb
--rw-r--r--   0        0        0    21815 2023-04-06 01:33:58.948318 lava_nc-0.7.0/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb
--rw-r--r--   0        0        0    12809 2023-04-06 01:33:58.948449 lava_nc-0.7.0/tutorials/in_depth/tutorial07_remote_memory_access.ipynb
--rw-r--r--   0        0        0    73297 2023-04-06 01:33:58.948782 lava_nc-0.7.0/tutorials/in_depth/tutorial08_stdp.ipynb
--rw-r--r--   0        0        0   137711 2023-04-06 01:33:58.949406 lava_nc-0.7.0/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb
--rw-r--r--   0        0        0   222561 2023-04-06 01:33:58.950407 lava_nc-0.7.0/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb
--rw-r--r--   0        0        0     1847 1970-01-01 00:00:00.000000 lava_nc-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      333 2023-04-06 01:33:58.675405 lava_nc-0.7.0.post1/LICENSE
+-rw-r--r--   0        0        0     4662 2023-05-03 16:41:04.617262 lava_nc-0.7.0.post1/pyproject.toml
+-rw-r--r--   0        0        0    26529 2023-04-06 01:33:58.677146 lava_nc-0.7.0.post1/src/lava/magma/compiler/LICENSE
+-rw-r--r--   0        0        0     5550 2023-04-06 01:33:58.677313 lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/channel_builder.py
+-rw-r--r--   0        0        0     4236 2023-04-06 01:33:58.677430 lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/interfaces.py
+-rw-r--r--   0        0        0    15527 2023-05-02 02:26:25.479841 lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/py_builder.py
+-rw-r--r--   0        0        0     4937 2023-04-06 01:33:58.677670 lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/runtimeservice_builder.py
+-rw-r--r--   0        0        0     4607 2023-04-21 18:31:56.277915 lava_nc-0.7.0.post1/src/lava/magma/compiler/channel_map.py
+-rw-r--r--   0        0        0     1372 2023-04-06 01:33:58.677919 lava_nc-0.7.0.post1/src/lava/magma/compiler/channels/interfaces.py
+-rw-r--r--   0        0        0    10521 2023-04-21 20:07:13.015569 lava_nc-0.7.0.post1/src/lava/magma/compiler/channels/pypychannel.py
+-rw-r--r--   0        0        0    35450 2023-04-06 01:33:58.678374 lava_nc-0.7.0.post1/src/lava/magma/compiler/compiler.py
+-rw-r--r--   0        0        0    44872 2023-04-06 01:33:58.678597 lava_nc-0.7.0.post1/src/lava/magma/compiler/compiler_graphs.py
+-rw-r--r--   0        0        0     1550 2023-04-06 01:33:58.678711 lava_nc-0.7.0.post1/src/lava/magma/compiler/compiler_utils.py
+-rw-r--r--   0        0        0      573 2023-04-06 01:33:58.678794 lava_nc-0.7.0.post1/src/lava/magma/compiler/exceptions.py
+-rw-r--r--   0        0        0     1778 2023-04-06 01:33:58.678886 lava_nc-0.7.0.post1/src/lava/magma/compiler/executable.py
+-rw-r--r--   0        0        0      721 2023-04-06 01:33:58.678969 lava_nc-0.7.0.post1/src/lava/magma/compiler/mappable_interface.py
+-rw-r--r--   0        0        0     7583 2023-04-06 01:33:58.679057 lava_nc-0.7.0.post1/src/lava/magma/compiler/mapper.py
+-rw-r--r--   0        0        0     2250 2023-04-06 01:33:58.679131 lava_nc-0.7.0.post1/src/lava/magma/compiler/node.py
+-rw-r--r--   0        0        0      514 2023-04-06 01:33:58.679262 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/address.py
+-rw-r--r--   0        0        0    10380 2023-04-06 01:33:58.679371 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/channel_builders_factory.py
+-rw-r--r--   0        0        0     2390 2023-04-06 01:33:58.679457 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/channel_map_updater.py
+-rw-r--r--   0        0        0      696 2023-04-06 01:33:58.679546 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/constants.py
+-rw-r--r--   0        0        0      769 2023-04-06 01:33:58.679630 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/exceptions.py
+-rw-r--r--   0        0        0     2086 2023-04-06 01:33:58.679719 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/interfaces.py
+-rw-r--r--   0        0        0     7543 2023-04-06 01:33:58.679858 lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py
+-rw-r--r--   0        0        0     4153 2023-04-06 01:33:58.679947 lava_nc-0.7.0.post1/src/lava/magma/compiler/utils.py
+-rw-r--r--   0        0        0     5711 2023-05-02 02:26:25.480541 lava_nc-0.7.0.post1/src/lava/magma/compiler/var_model.py
+-rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.680174 lava_nc-0.7.0.post1/src/lava/magma/core/LICENSE
+-rw-r--r--   0        0        0     1613 2023-04-06 01:33:58.680260 lava_nc-0.7.0.post1/src/lava/magma/core/callback_fx.py
+-rw-r--r--   0        0        0     6408 2023-04-06 01:33:58.680350 lava_nc-0.7.0.post1/src/lava/magma/core/decorator.py
+-rw-r--r--   0        0        0     1999 2023-04-06 01:33:58.680477 lava_nc-0.7.0.post1/src/lava/magma/core/learning/constants.py
+-rw-r--r--   0        0        0    23198 2023-04-06 01:33:58.680631 lava_nc-0.7.0.post1/src/lava/magma/core/learning/learning_rule.py
+-rw-r--r--   0        0        0    12270 2023-04-06 01:33:58.680751 lava_nc-0.7.0.post1/src/lava/magma/core/learning/learning_rule_applier.py
+-rw-r--r--   0        0        0    23302 2023-04-06 01:33:58.680867 lava_nc-0.7.0.post1/src/lava/magma/core/learning/product_series.py
+-rw-r--r--   0        0        0     4603 2023-04-06 01:33:58.680951 lava_nc-0.7.0.post1/src/lava/magma/core/learning/random.py
+-rw-r--r--   0        0        0      685 2023-04-06 01:33:58.681022 lava_nc-0.7.0.post1/src/lava/magma/core/learning/string_symbols.py
+-rw-r--r--   0        0        0    23789 2023-04-06 01:33:58.681133 lava_nc-0.7.0.post1/src/lava/magma/core/learning/symbolic_equation.py
+-rw-r--r--   0        0        0     2068 2023-04-06 01:33:58.681231 lava_nc-0.7.0.post1/src/lava/magma/core/learning/utils.py
+-rw-r--r--   0        0        0     1084 2023-04-06 01:33:58.681344 lava_nc-0.7.0.post1/src/lava/magma/core/model/interfaces.py
+-rw-r--r--   0        0        0     5193 2023-04-06 01:33:58.681438 lava_nc-0.7.0.post1/src/lava/magma/core/model/model.py
+-rw-r--r--   0        0        0    52944 2023-05-02 02:26:25.481186 lava_nc-0.7.0.post1/src/lava/magma/core/model/py/connection.py
+-rw-r--r--   0        0        0    25160 2023-05-02 02:26:25.482275 lava_nc-0.7.0.post1/src/lava/magma/core/model/py/model.py
+-rw-r--r--   0        0        0     3100 2023-04-06 01:33:58.681910 lava_nc-0.7.0.post1/src/lava/magma/core/model/py/neuron.py
+-rw-r--r--   0        0        0    36060 2023-04-21 19:23:43.524374 lava_nc-0.7.0.post1/src/lava/magma/core/model/py/ports.py
+-rw-r--r--   0        0        0      458 2023-04-06 01:33:58.682166 lava_nc-0.7.0.post1/src/lava/magma/core/model/py/type.py
+-rw-r--r--   0        0        0      352 2023-04-06 01:33:58.682232 lava_nc-0.7.0.post1/src/lava/magma/core/model/spike_type.py
+-rw-r--r--   0        0        0     2914 2023-04-06 01:33:58.682348 lava_nc-0.7.0.post1/src/lava/magma/core/model/sub/model.py
+-rw-r--r--   0        0        0     3781 2023-04-06 01:33:58.682462 lava_nc-0.7.0.post1/src/lava/magma/core/process/connection.py
+-rw-r--r--   0        0        0     2285 2023-04-06 01:33:58.682537 lava_nc-0.7.0.post1/src/lava/magma/core/process/interfaces.py
+-rw-r--r--   0        0        0      194 2023-04-06 01:33:58.682613 lava_nc-0.7.0.post1/src/lava/magma/core/process/message_interface_enum.py
+-rw-r--r--   0        0        0     1690 2023-04-06 01:33:58.682686 lava_nc-0.7.0.post1/src/lava/magma/core/process/neuron.py
+-rw-r--r--   0        0        0     2763 2023-04-06 01:33:58.682815 lava_nc-0.7.0.post1/src/lava/magma/core/process/ports/exceptions.py
+-rw-r--r--   0        0        0    38136 2023-04-06 01:33:58.682963 lava_nc-0.7.0.post1/src/lava/magma/core/process/ports/ports.py
+-rw-r--r--   0        0        0      459 2023-04-06 01:33:58.683040 lava_nc-0.7.0.post1/src/lava/magma/core/process/ports/reduce_ops.py
+-rw-r--r--   0        0        0    23800 2023-05-01 20:07:22.307395 lava_nc-0.7.0.post1/src/lava/magma/core/process/process.py
+-rw-r--r--   0        0        0     7993 2023-05-02 02:26:25.483107 lava_nc-0.7.0.post1/src/lava/magma/core/process/variable.py
+-rw-r--r--   0        0        0     3767 2023-04-06 01:33:58.683596 lava_nc-0.7.0.post1/src/lava/magma/core/resources.py
+-rw-r--r--   0        0        0     1502 2023-04-06 01:33:58.683683 lava_nc-0.7.0.post1/src/lava/magma/core/run_conditions.py
+-rw-r--r--   0        0        0    22433 2023-04-06 01:33:58.683817 lava_nc-0.7.0.post1/src/lava/magma/core/run_configs.py
+-rw-r--r--   0        0        0     1506 2023-04-06 01:33:58.683976 lava_nc-0.7.0.post1/src/lava/magma/core/sync/domain.py
+-rw-r--r--   0        0        0     1107 2023-04-06 01:33:58.684058 lava_nc-0.7.0.post1/src/lava/magma/core/sync/protocol.py
+-rw-r--r--   0        0        0     1523 2023-04-06 01:33:58.684181 lava_nc-0.7.0.post1/src/lava/magma/core/sync/protocols/async_protocol.py
+-rw-r--r--   0        0        0     4386 2023-04-06 01:33:58.684278 lava_nc-0.7.0.post1/src/lava/magma/core/sync/protocols/loihi_protocol.py
+-rw-r--r--   0        0        0    26529 2023-04-06 01:33:58.684503 lava_nc-0.7.0.post1/src/lava/magma/runtime/LICENSE
+-rw-r--r--   0        0        0      720 2023-04-06 01:33:58.684641 lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/factory.py
+-rw-r--r--   0        0        0     1790 2023-04-06 01:33:58.684732 lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py
+-rw-r--r--   0        0        0     4385 2023-04-06 01:33:58.684846 lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/multiprocessing.py
+-rw-r--r--   0        0        0     1452 2023-04-06 01:33:58.684931 lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/nx.py
+-rw-r--r--   0        0        0     1005 2023-04-06 01:33:58.685010 lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py
+-rw-r--r--   0        0        0     2439 2023-04-06 01:33:58.685090 lava_nc-0.7.0.post1/src/lava/magma/runtime/mgmt_token_enums.py
+-rw-r--r--   0        0        0    22602 2023-05-02 02:26:25.483668 lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime.py
+-rw-r--r--   0        0        0     8310 2023-04-06 01:33:58.685476 lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py
+-rw-r--r--   0        0        0     1324 2023-04-06 01:33:58.685552 lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/enums.py
+-rw-r--r--   0        0        0     1159 2023-04-06 01:33:58.685621 lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/interfaces.py
+-rw-r--r--   0        0        0    22607 2023-04-21 18:31:56.278483 lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/runtime_service.py
+-rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.685914 lava_nc-0.7.0.post1/src/lava/proc/LICENSE
+-rw-r--r--   0        0        0     2934 2023-04-06 01:33:58.686050 lava_nc-0.7.0.post1/src/lava/proc/conv/models.py
+-rw-r--r--   0        0        0     5954 2023-04-06 01:33:58.686146 lava_nc-0.7.0.post1/src/lava/proc/conv/process.py
+-rw-r--r--   0        0        0    16042 2023-04-06 01:33:58.686256 lava_nc-0.7.0.post1/src/lava/proc/conv/utils.py
+-rw-r--r--   0        0        0    14321 2023-05-02 02:26:25.484362 lava_nc-0.7.0.post1/src/lava/proc/dense/models.py
+-rw-r--r--   0        0        0    11177 2023-04-06 01:33:58.686544 lava_nc-0.7.0.post1/src/lava/proc/dense/process.py
+-rw-r--r--   0        0        0      236 2023-04-06 01:33:58.686665 lava_nc-0.7.0.post1/src/lava/proc/io/__init__.py
+-rw-r--r--   0        0        0     7532 2023-04-06 01:33:58.686757 lava_nc-0.7.0.post1/src/lava/proc/io/dataloader.py
+-rw-r--r--   0        0        0     9449 2023-04-06 01:33:58.686854 lava_nc-0.7.0.post1/src/lava/proc/io/encoder.py
+-rw-r--r--   0        0        0     2740 2023-04-06 01:33:58.686934 lava_nc-0.7.0.post1/src/lava/proc/io/reset.py
+-rw-r--r--   0        0        0     4831 2023-04-06 01:33:58.687026 lava_nc-0.7.0.post1/src/lava/proc/io/sink.py
+-rw-r--r--   0        0        0     2020 2023-04-06 01:33:58.687121 lava_nc-0.7.0.post1/src/lava/proc/io/source.py
+-rw-r--r--   0        0        0     3083 2023-04-06 01:33:58.687246 lava_nc-0.7.0.post1/src/lava/proc/learning_rules/r_stdp_learning_rule.py
+-rw-r--r--   0        0        0     1991 2023-04-06 01:33:58.687335 lava_nc-0.7.0.post1/src/lava/proc/learning_rules/stdp_learning_rule.py
+-rw-r--r--   0        0        0    18980 2023-04-06 01:33:58.687498 lava_nc-0.7.0.post1/src/lava/proc/lif/models.py
+-rw-r--r--   0        0        0    12911 2023-04-06 01:33:58.687776 lava_nc-0.7.0.post1/src/lava/proc/lif/process.py
+-rw-r--r--   0        0        0     2646 2023-04-06 01:33:58.687985 lava_nc-0.7.0.post1/src/lava/proc/monitor/models.py
+-rw-r--r--   0        0        0    11074 2023-04-06 01:33:58.688120 lava_nc-0.7.0.post1/src/lava/proc/monitor/process.py
+-rw-r--r--   0        0        0     1074 2023-04-06 01:33:58.688287 lava_nc-0.7.0.post1/src/lava/proc/receiver/models.py
+-rw-r--r--   0        0        0     1082 2023-04-06 01:33:58.688388 lava_nc-0.7.0.post1/src/lava/proc/receiver/process.py
+-rw-r--r--   0        0        0     5997 2023-04-06 01:33:58.688615 lava_nc-0.7.0.post1/src/lava/proc/rf/models.py
+-rw-r--r--   0        0        0     3591 2023-04-06 01:33:58.688718 lava_nc-0.7.0.post1/src/lava/proc/rf/process.py
+-rw-r--r--   0        0        0     2464 2023-04-06 01:33:58.688878 lava_nc-0.7.0.post1/src/lava/proc/rf_iz/models.py
+-rw-r--r--   0        0        0      181 2023-04-06 01:33:58.688964 lava_nc-0.7.0.post1/src/lava/proc/rf_iz/process.py
+-rw-r--r--   0        0        0     9115 2023-04-06 01:33:58.689150 lava_nc-0.7.0.post1/src/lava/proc/sdn/models.py
+-rw-r--r--   0        0        0     7382 2023-04-06 01:33:58.689241 lava_nc-0.7.0.post1/src/lava/proc/sdn/process.py
+-rw-r--r--   0        0        0     1431 2023-04-06 01:33:58.689397 lava_nc-0.7.0.post1/src/lava/proc/spiker/models.py
+-rw-r--r--   0        0        0     1461 2023-04-06 01:33:58.689504 lava_nc-0.7.0.post1/src/lava/proc/spiker/process.py
+-rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.689656 lava_nc-0.7.0.post1/src/lava/utils/LICENSE
+-rw-r--r--   0        0        0     4282 2023-04-06 01:33:58.689799 lava_nc-0.7.0.post1/src/lava/utils/dataloader/mnist.py
+-rw-r--r--   0        0        0     3254 2023-04-06 01:33:58.689888 lava_nc-0.7.0.post1/src/lava/utils/plots.py
+-rw-r--r--   0        0        0     1466 2023-04-06 01:33:58.689982 lava_nc-0.7.0.post1/src/lava/utils/profiler.py
+-rw-r--r--   0        0        0     1868 2023-04-06 01:33:58.690075 lava_nc-0.7.0.post1/src/lava/utils/system.py
+-rw-r--r--   0        0        0     7911 2023-05-02 02:26:25.484917 lava_nc-0.7.0.post1/src/lava/utils/weightutils.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690282 lava_nc-0.7.0.post1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690406 lava_nc-0.7.0.post1/tests/lava/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690509 lava_nc-0.7.0.post1/tests/lava/magma/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690614 lava_nc-0.7.0.post1/tests/lava/magma/compiler/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690724 lava_nc-0.7.0.post1/tests/lava/magma/compiler/builders/__init__.py
+-rw-r--r--   0        0        0    20945 2023-04-06 01:33:58.690880 lava_nc-0.7.0.post1/tests/lava/magma/compiler/builders/test_builder.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.690989 lava_nc-0.7.0.post1/tests/lava/magma/compiler/channels/__init__.py
+-rw-r--r--   0        0        0     5130 2023-04-06 01:33:58.691110 lava_nc-0.7.0.post1/tests/lava/magma/compiler/channels/test_pypychannel.py
+-rw-r--r--   0        0        0      113 2023-04-06 01:33:58.691236 lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-06 01:33:58.691352 lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/py/__init__.py
+-rw-r--r--   0        0        0     8989 2023-04-06 01:33:58.691552 lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py
+-rw-r--r--   0        0        0    18797 2023-04-06 01:33:58.691770 lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py
+-rw-r--r--   0        0        0     3741 2023-04-06 01:33:58.691902 lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py
+-rw-r--r--   0        0        0     2168 2023-04-06 01:33:58.692020 lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_channel_builder.py
+-rw-r--r--   0        0        0     5376 2023-04-06 01:33:58.692139 lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_channel_map.py
+-rw-r--r--   0        0        0    30646 2023-04-06 01:33:58.692310 lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_compiler.py
+-rw-r--r--   0        0        0     2048 2023-04-06 01:33:58.692421 lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_node.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.692521 lava_nc-0.7.0.post1/tests/lava/magma/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.692653 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/__init__.py
+-rw-r--r--   0        0        0    50548 2023-04-21 19:48:24.469204 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_learning_rule.py
+-rw-r--r--   0        0        0     5470 2023-04-06 01:33:58.693000 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_learning_rule_applier.py
+-rw-r--r--   0        0        0    12737 2023-04-06 01:33:58.693092 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_product_series.py
+-rw-r--r--   0        0        0     1905 2023-04-06 01:33:58.693182 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_random.py
+-rw-r--r--   0        0        0    18180 2023-04-06 01:33:58.693301 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_symbolic_equation.py
+-rw-r--r--   0        0        0     2230 2023-04-06 01:33:58.693422 lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_utils.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.693514 lava_nc-0.7.0.post1/tests/lava/magma/core/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.693637 lava_nc-0.7.0.post1/tests/lava/magma/core/model/py/__init__.py
+-rw-r--r--   0        0        0     5870 2023-04-06 01:33:58.693768 lava_nc-0.7.0.post1/tests/lava/magma/core/model/py/test_model.py
+-rw-r--r--   0        0        0     6898 2023-04-06 01:33:58.693882 lava_nc-0.7.0.post1/tests/lava/magma/core/model/py/test_ports.py
+-rw-r--r--   0        0        0     9117 2023-04-06 01:33:58.693984 lava_nc-0.7.0.post1/tests/lava/magma/core/model/test_decorators.py
+-rw-r--r--   0        0        0     1552 2023-04-06 01:33:58.694079 lava_nc-0.7.0.post1/tests/lava/magma/core/model/test_sub_model.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.694163 lava_nc-0.7.0.post1/tests/lava/magma/core/process/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.694270 lava_nc-0.7.0.post1/tests/lava/magma/core/process/ports/__init__.py
+-rw-r--r--   0        0        0    21231 2023-04-06 01:33:58.694426 lava_nc-0.7.0.post1/tests/lava/magma/core/process/ports/test_ports.py
+-rw-r--r--   0        0        0    34827 2023-04-06 01:33:58.694615 lava_nc-0.7.0.post1/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py
+-rw-r--r--   0        0        0     1377 2023-04-06 01:33:58.694728 lava_nc-0.7.0.post1/tests/lava/magma/core/process/test_lif_dense_lif.py
+-rw-r--r--   0        0        0    12308 2023-05-01 20:07:22.311061 lava_nc-0.7.0.post1/tests/lava/magma/core/process/test_process.py
+-rw-r--r--   0        0        0     4635 2023-04-06 01:33:58.694944 lava_nc-0.7.0.post1/tests/lava/magma/core/process/test_variable.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.695026 lava_nc-0.7.0.post1/tests/lava/magma/runtime/__init__.py
+-rw-r--r--   0        0        0     3675 2023-04-06 01:33:58.695118 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_async_protocol.py
+-rw-r--r--   0        0        0     5783 2023-04-06 01:33:58.695207 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_context_manager.py
+-rw-r--r--   0        0        0     5174 2023-04-06 01:33:58.695315 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_exception_handling.py
+-rw-r--r--   0        0        0     2038 2023-04-06 01:33:58.695401 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_get_set_non_determinism.py
+-rw-r--r--   0        0        0     7469 2023-04-06 01:33:58.695490 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_get_set_var.py
+-rw-r--r--   0        0        0    10583 2023-04-06 01:33:58.695571 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_io_ports.py
+-rw-r--r--   0        0        0     1216 2023-04-06 01:33:58.695644 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_leakage.py
+-rw-r--r--   0        0        0     2238 2023-04-06 01:33:58.695722 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_loihi_protocol.py
+-rw-r--r--   0        0        0     3661 2023-04-06 01:33:58.695809 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_loihi_with_async_protocol.py
+-rw-r--r--   0        0        0     6682 2023-04-06 01:33:58.695909 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_pause_requested_from_model.py
+-rw-r--r--   0        0        0    14794 2023-04-06 01:33:58.696021 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_ref_var_ports.py
+-rw-r--r--   0        0        0     3822 2023-04-06 01:33:58.696113 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_run_continuously_and_pause.py
+-rw-r--r--   0        0        0     2829 2023-04-06 01:33:58.696205 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_runtime.py
+-rw-r--r--   0        0        0     2903 2023-04-06 01:33:58.696305 lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_runtime_service.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.696394 lava_nc-0.7.0.post1/tests/lava/proc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.696506 lava_nc-0.7.0.post1/tests/lava/proc/conv/__init__.py
+-rw-r--r--   0        0        0   559366 2023-04-06 01:33:58.699158 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz
+-rw-r--r--   0        0        0   590766 2023-04-06 01:33:58.702025 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz
+-rw-r--r--   0        0        0   956638 2023-04-06 01:33:58.706484 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz
+-rw-r--r--   0        0        0    68302 2023-04-06 01:33:58.706921 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz
+-rw-r--r--   0        0        0   185142 2023-04-06 01:33:58.707804 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz
+-rw-r--r--   0        0        0   409190 2023-04-06 01:33:58.709742 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz
+-rw-r--r--   0        0        0  1888366 2023-04-06 01:33:58.718461 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz
+-rw-r--r--   0        0        0  1790434 2023-04-06 01:33:58.726618 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz
+-rw-r--r--   0        0        0   714214 2023-04-06 01:33:58.729733 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz
+-rw-r--r--   0        0        0   670702 2023-04-06 01:33:58.732644 lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz
+-rw-r--r--   0        0        0      999 2023-04-06 01:33:58.732750 lava_nc-0.7.0.post1/tests/lava/proc/conv/test_process.py
+-rw-r--r--   0        0        0     7343 2023-04-06 01:33:58.732856 lava_nc-0.7.0.post1/tests/lava/proc/conv/test_utils.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.732967 lava_nc-0.7.0.post1/tests/lava/proc/dense/__init__.py
+-rw-r--r--   0        0        0    53052 2023-04-06 01:33:58.733140 lava_nc-0.7.0.post1/tests/lava/proc/dense/test_learning.py
+-rw-r--r--   0        0        0    47972 2023-04-06 01:33:58.733283 lava_nc-0.7.0.post1/tests/lava/proc/dense/test_models.py
+-rw-r--r--   0        0        0     3666 2023-04-06 01:33:58.733380 lava_nc-0.7.0.post1/tests/lava/proc/dense/test_process.py
+-rw-r--r--   0        0        0    24791 2023-04-06 01:33:58.733484 lava_nc-0.7.0.post1/tests/lava/proc/dense/test_stdp_sim.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.733576 lava_nc-0.7.0.post1/tests/lava/proc/io/__init__.py
+-rw-r--r--   0        0        0     7309 2023-04-06 01:33:58.733681 lava_nc-0.7.0.post1/tests/lava/proc/io/test_dataloader.py
+-rw-r--r--   0        0        0     2001 2023-04-06 01:33:58.733765 lava_nc-0.7.0.post1/tests/lava/proc/io/test_source_sink.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.733835 lava_nc-0.7.0.post1/tests/lava/proc/lif/__init__.py
+-rw-r--r--   0        0        0    38490 2023-04-06 01:33:58.733977 lava_nc-0.7.0.post1/tests/lava/proc/lif/test_models.py
+-rw-r--r--   0        0        0     2213 2023-04-06 01:33:58.734066 lava_nc-0.7.0.post1/tests/lava/proc/lif/test_process.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734148 lava_nc-0.7.0.post1/tests/lava/proc/monitor/__init__.py
+-rw-r--r--   0        0        0    12959 2023-04-06 01:33:58.734277 lava_nc-0.7.0.post1/tests/lava/proc/monitor/test_monitors.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734365 lava_nc-0.7.0.post1/tests/lava/proc/rf/__init__.py
+-rw-r--r--   0        0        0     9354 2023-04-06 01:33:58.734466 lava_nc-0.7.0.post1/tests/lava/proc/rf/test_models.py
+-rw-r--r--   0        0        0      868 2023-04-06 01:33:58.734537 lava_nc-0.7.0.post1/tests/lava/proc/rf/test_process.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734608 lava_nc-0.7.0.post1/tests/lava/proc/rf_iz/__init__.py
+-rw-r--r--   0        0        0     3563 2023-04-06 01:33:58.734725 lava_nc-0.7.0.post1/tests/lava/proc/rf_iz/test_models.py
+-rw-r--r--   0        0        0      901 2023-04-06 01:33:58.734787 lava_nc-0.7.0.post1/tests/lava/proc/rf_iz/test_process.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.734866 lava_nc-0.7.0.post1/tests/lava/proc/sdn/__init__.py
+-rw-r--r--   0        0        0     7800 2023-04-06 01:33:58.734963 lava_nc-0.7.0.post1/tests/lava/proc/sdn/test_models.py
+-rw-r--r--   0        0        0     1457 2023-04-06 01:33:58.735028 lava_nc-0.7.0.post1/tests/lava/proc/sdn/test_process.py
+-rw-r--r--   0        0        0     1710 2023-04-06 01:33:58.735146 lava_nc-0.7.0.post1/tests/lava/proc/spiker/test_models.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.735219 lava_nc-0.7.0.post1/tests/lava/test_utils/__init__.py
+-rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.735306 lava_nc-0.7.0.post1/tests/lava/test_utils/utils.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.735370 lava_nc-0.7.0.post1/tests/lava/tutorials/__init__.py
+-rw-r--r--   0        0        0     9340 2023-04-06 01:33:58.735509 lava_nc-0.7.0.post1/tests/lava/tutorials/test_tutorials.py
+-rw-r--r--   0        0        0        0 2023-04-06 01:33:58.735579 lava_nc-0.7.0.post1/tests/lava/utils/__init__.py
+-rw-r--r--   0        0        0     2165 2023-04-06 01:33:58.735665 lava_nc-0.7.0.post1/tests/lava/utils/test_plots.py
+-rw-r--r--   0        0        0    15761 2023-04-06 01:33:58.735757 lava_nc-0.7.0.post1/tests/lava/utils/test_weightutils.py
+-rw-r--r--   0        0        0     1525 2023-04-06 01:33:58.735889 lava_nc-0.7.0.post1/tutorials/LICENSE
+-rw-r--r--   0        0        0     9985 2023-04-06 01:33:58.736024 lava_nc-0.7.0.post1/tutorials/end_to_end/convert_params.py
+-rw-r--r--   0        0        0   220767 2023-04-06 01:34:02.588053 lava_nc-0.7.0.post1/tutorials/end_to_end/mnist_pretrained.npy
+-rw-r--r--   0        0        0   276563 2023-04-21 19:07:38.860825 lava_nc-0.7.0.post1/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb
+-rw-r--r--   0        0        0    24427 2023-04-06 01:33:58.939317 lava_nc-0.7.0.post1/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb
+-rw-r--r--   0        0        0  1170553 2023-04-06 01:33:58.944705 lava_nc-0.7.0.post1/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb
+-rw-r--r--   0        0        0   566145 2023-04-06 01:33:58.947282 lava_nc-0.7.0.post1/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb
+-rw-r--r--   0        0        0    10117 2023-04-06 01:33:58.947469 lava_nc-0.7.0.post1/tutorials/in_depth/three_factor_learning/utils.py
+-rw-r--r--   0        0        0     6552 2023-04-06 01:33:58.947564 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial01_installing_lava.ipynb
+-rw-r--r--   0        0        0    16399 2023-04-06 01:33:58.947718 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial02_processes.ipynb
+-rw-r--r--   0        0        0    15539 2023-04-21 19:07:45.551328 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial03_process_models.ipynb
+-rw-r--r--   0        0        0    14366 2023-04-06 01:33:58.948013 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial04_execution.ipynb
+-rw-r--r--   0        0        0    13442 2023-04-06 01:33:58.948158 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial05_connect_processes.ipynb
+-rw-r--r--   0        0        0    21815 2023-04-06 01:33:58.948318 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb
+-rw-r--r--   0        0        0    12809 2023-04-06 01:33:58.948449 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial07_remote_memory_access.ipynb
+-rw-r--r--   0        0        0    73297 2023-04-06 01:33:58.948782 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial08_stdp.ipynb
+-rw-r--r--   0        0        0   137711 2023-04-06 01:33:58.949406 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb
+-rw-r--r--   0        0        0   222561 2023-04-06 01:33:58.950407 lava_nc-0.7.0.post1/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb
+-rw-r--r--   0        0        0     1695 1970-01-01 00:00:00.000000 lava_nc-0.7.0.post1/PKG-INFO
```

### Comparing `lava_nc-0.7.0/pyproject.toml` & `lava_nc-0.7.0.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 [tool.poetry]
 name = "lava-nc"
 packages = [
     {include = "lava", from = "src"},
     {include = "tests"}
 ]
 include = ["tutorials"]
-version = "0.7.0"
+version = "0.7.0.post1"
 description = "A Software Framework for Neuromorphic Computing"
 homepage = "https://lava-nc.org/"
 repository = "https://github.com/lava-nc/lava"
 authors = [ 
     "Intel's Neuromorphic Computing Lab and the open source community <lava@intel.com>"
 ]
-license = "Lava uses multiple licenses and is licensed under BSD-3-Clause or LGPL-2.1-or-later"
+license = "(BSD-3-Clause), (LGPL-2.1-or-later)"
 keywords = [
     "neuromorphic",
     "ai",
     "artificial intelligence",
     "neural models",
     "spiking neural networks"
 ]
@@ -29,16 +29,15 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "License :: OSI Approved :: BSD License",
-    "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+    "License :: OSI Approved",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.urls]
 "Issue and Bug Tracker" = "https://github.com/lava-nc/lava/issues"
 "Questions and Answers" = "https://github.com/lava-nc/lava/discussions/categories/q-a"
 "Frequently Asked Questions" = "https://github.com/lava-nc/lava/wiki/Frequently-Asked-Questions-(FAQ)"
```

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/LICENSE` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/builders/channel_builder.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/channel_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/builders/interfaces.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/builders/py_builder.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/py_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/builders/runtimeservice_builder.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/builders/runtimeservice_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/channel_map.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/channel_map.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/channels/interfaces.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/channels/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/channels/pypychannel.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/channels/pypychannel.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/compiler.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/compiler_graphs.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/compiler_graphs.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/compiler_utils.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/compiler_utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/exceptions.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/executable.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/executable.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/mappable_interface.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/mappable_interface.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/mapper.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/mapper.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/node.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/node.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/address.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/address.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/channel_builders_factory.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/channel_builders_factory.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/channel_map_updater.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/channel_map_updater.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/constants.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/constants.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/exceptions.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/exceptions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/interfaces.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/subcompilers/py/pyproc_compiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/utils.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/compiler/var_model.py` & `lava_nc-0.7.0.post1/src/lava/magma/compiler/var_model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/LICENSE` & `lava_nc-0.7.0.post1/src/lava/magma/core/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/callback_fx.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/callback_fx.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/decorator.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/decorator.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/constants.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/constants.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/learning_rule.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/learning_rule_applier.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/learning_rule_applier.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/product_series.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/product_series.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/random.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/random.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/string_symbols.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/string_symbols.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/symbolic_equation.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/symbolic_equation.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/learning/utils.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/learning/utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/interfaces.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/model.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/py/connection.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/py/connection.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/py/model.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/py/model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/py/neuron.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/py/neuron.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/py/ports.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/py/ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/model/sub/model.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/model/sub/model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/connection.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/connection.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/interfaces.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/neuron.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/neuron.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/ports/exceptions.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/ports/exceptions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/ports/ports.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/ports/ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/process.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/process/variable.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/process/variable.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/resources.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/resources.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/run_conditions.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/run_conditions.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/run_configs.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/run_configs.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/sync/domain.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/sync/domain.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/sync/protocol.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/sync/protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/sync/protocols/async_protocol.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/sync/protocols/async_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/core/sync/protocols/loihi_protocol.py` & `lava_nc-0.7.0.post1/src/lava/magma/core/sync/protocols/loihi_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/LICENSE` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/factory.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/factory.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/message_infrastructure_interface.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/multiprocessing.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/nx.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/nx.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/message_infrastructure/shared_memory_manager.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/mgmt_token_enums.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/mgmt_token_enums.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/runtime.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/channel_broker/channel_broker.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/enums.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/enums.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/interfaces.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/interfaces.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/magma/runtime/runtime_services/runtime_service.py` & `lava_nc-0.7.0.post1/src/lava/magma/runtime/runtime_services/runtime_service.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/LICENSE` & `lava_nc-0.7.0.post1/src/lava/proc/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/conv/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/conv/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/conv/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/conv/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/conv/utils.py` & `lava_nc-0.7.0.post1/src/lava/proc/conv/utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/dense/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/dense/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/dense/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/dense/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/io/dataloader.py` & `lava_nc-0.7.0.post1/src/lava/proc/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/io/encoder.py` & `lava_nc-0.7.0.post1/src/lava/proc/io/encoder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/io/reset.py` & `lava_nc-0.7.0.post1/src/lava/proc/io/reset.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/io/sink.py` & `lava_nc-0.7.0.post1/src/lava/proc/io/sink.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/io/source.py` & `lava_nc-0.7.0.post1/src/lava/proc/io/source.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/learning_rules/r_stdp_learning_rule.py` & `lava_nc-0.7.0.post1/src/lava/proc/learning_rules/r_stdp_learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/learning_rules/stdp_learning_rule.py` & `lava_nc-0.7.0.post1/src/lava/proc/learning_rules/stdp_learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/lif/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/lif/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/lif/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/lif/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/monitor/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/monitor/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/monitor/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/monitor/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/receiver/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/receiver/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/receiver/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/receiver/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/rf/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/rf/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/rf/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/rf/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/rf_iz/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/rf_iz/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/sdn/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/sdn/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/sdn/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/sdn/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/spiker/models.py` & `lava_nc-0.7.0.post1/src/lava/proc/spiker/models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/proc/spiker/process.py` & `lava_nc-0.7.0.post1/src/lava/proc/spiker/process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/utils/LICENSE` & `lava_nc-0.7.0.post1/src/lava/utils/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/utils/dataloader/mnist.py` & `lava_nc-0.7.0.post1/src/lava/utils/dataloader/mnist.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/utils/plots.py` & `lava_nc-0.7.0.post1/src/lava/utils/plots.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/utils/profiler.py` & `lava_nc-0.7.0.post1/src/lava/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/utils/system.py` & `lava_nc-0.7.0.post1/src/lava/utils/system.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/src/lava/utils/weightutils.py` & `lava_nc-0.7.0.post1/src/lava/utils/weightutils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/builders/test_builder.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/builders/test_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/channels/test_pypychannel.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/channels/test_pypychannel.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/py/test_pyproc_compiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/test_channel_builders_factory.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/subcompilers/test_channel_map_updater.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/test_channel_builder.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_channel_builder.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/test_channel_map.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_channel_map.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/test_compiler.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/compiler/test_node.py` & `lava_nc-0.7.0.post1/tests/lava/magma/compiler/test_node.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/learning/test_learning_rule.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_learning_rule.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/learning/test_learning_rule_applier.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_learning_rule_applier.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/learning/test_product_series.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_product_series.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/learning/test_random.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_random.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/learning/test_symbolic_equation.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_symbolic_equation.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/learning/test_utils.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/learning/test_utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/model/py/test_model.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/model/py/test_model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/model/py/test_ports.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/model/py/test_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/model/test_decorators.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/model/test_decorators.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/model/test_sub_model.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/model/test_sub_model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/process/ports/test_ports.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/process/ports/test_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/process/ports/test_virtual_ports_in_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/process/test_lif_dense_lif.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/process/test_lif_dense_lif.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/process/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/process/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/core/process/test_variable.py` & `lava_nc-0.7.0.post1/tests/lava/magma/core/process/test_variable.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_async_protocol.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_async_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_context_manager.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_exception_handling.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_exception_handling.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_get_set_non_determinism.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_get_set_non_determinism.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_get_set_var.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_get_set_var.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_io_ports.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_io_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_leakage.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_leakage.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_loihi_protocol.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_loihi_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_loihi_with_async_protocol.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_loihi_with_async_protocol.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_pause_requested_from_model.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_pause_requested_from_model.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_ref_var_ports.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_ref_var_ports.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_run_continuously_and_pause.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_run_continuously_and_pause.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_runtime.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_runtime.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/magma/runtime/test_runtime_service.py` & `lava_nc-0.7.0.post1/tests/lava/magma/runtime/test_runtime_service.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_0.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_1.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_2.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_3.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_4.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_5.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_6.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_7.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_8.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/ground_truth/gt_conv_paris_9.npz`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/conv/test_utils.py` & `lava_nc-0.7.0.post1/tests/lava/proc/conv/test_utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/dense/test_learning.py` & `lava_nc-0.7.0.post1/tests/lava/proc/dense/test_learning.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/dense/test_models.py` & `lava_nc-0.7.0.post1/tests/lava/proc/dense/test_models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/dense/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/proc/dense/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/dense/test_stdp_sim.py` & `lava_nc-0.7.0.post1/tests/lava/proc/dense/test_stdp_sim.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/io/test_dataloader.py` & `lava_nc-0.7.0.post1/tests/lava/proc/io/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/io/test_source_sink.py` & `lava_nc-0.7.0.post1/tests/lava/proc/io/test_source_sink.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/lif/test_models.py` & `lava_nc-0.7.0.post1/tests/lava/proc/lif/test_models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/lif/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/proc/lif/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/monitor/test_monitors.py` & `lava_nc-0.7.0.post1/tests/lava/proc/monitor/test_monitors.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/rf/test_models.py` & `lava_nc-0.7.0.post1/tests/lava/proc/rf/test_models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/rf/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/proc/rf/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/rf_iz/test_models.py` & `lava_nc-0.7.0.post1/tests/lava/proc/rf_iz/test_models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/rf_iz/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/proc/rf_iz/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/sdn/test_models.py` & `lava_nc-0.7.0.post1/tests/lava/proc/sdn/test_models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/sdn/test_process.py` & `lava_nc-0.7.0.post1/tests/lava/proc/sdn/test_process.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/proc/spiker/test_models.py` & `lava_nc-0.7.0.post1/tests/lava/proc/spiker/test_models.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/test_utils/utils.py` & `lava_nc-0.7.0.post1/tests/lava/test_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/tutorials/test_tutorials.py` & `lava_nc-0.7.0.post1/tests/lava/tutorials/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/utils/test_plots.py` & `lava_nc-0.7.0.post1/tests/lava/utils/test_plots.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tests/lava/utils/test_weightutils.py` & `lava_nc-0.7.0.post1/tests/lava/utils/test_weightutils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/LICENSE` & `lava_nc-0.7.0.post1/tutorials/LICENSE`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/end_to_end/convert_params.py` & `lava_nc-0.7.0.post1/tutorials/end_to_end/convert_params.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/end_to_end/mnist_pretrained.npy` & `lava_nc-0.7.0.post1/tutorials/end_to_end/mnist_pretrained.npy`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb` & `lava_nc-0.7.0.post1/tutorials/end_to_end/tutorial00_tour_through_lava.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb` & `lava_nc-0.7.0.post1/tutorials/end_to_end/tutorial01_mnist_digit_classification.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb` & `lava_nc-0.7.0.post1/tutorials/end_to_end/tutorial02_excitatory_inhibitory_network.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/three_factor_learning/tutorial01_Reward_Modulated_STDP.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/three_factor_learning/utils.py` & `lava_nc-0.7.0.post1/tutorials/in_depth/three_factor_learning/utils.py`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial01_installing_lava.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial01_installing_lava.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial02_processes.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial02_processes.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial03_process_models.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial03_process_models.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial04_execution.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial04_execution.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial05_connect_processes.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial05_connect_processes.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial06_hierarchical_processes.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial07_remote_memory_access.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial07_remote_memory_access.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial08_stdp.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial08_stdp.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial09_custom_learning_rules.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb` & `lava_nc-0.7.0.post1/tutorials/in_depth/tutorial10_sigma_delta_neurons.ipynb`

 * *Files identical despite different names*

### Comparing `lava_nc-0.7.0/PKG-INFO` & `lava_nc-0.7.0.post1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: lava-nc
-Version: 0.7.0
+Version: 0.7.0.post1
 Summary: A Software Framework for Neuromorphic Computing
 Home-page: https://lava-nc.org/
-License: Lava uses multiple licenses and is licensed under BSD-3-Clause or LGPL-2.1-or-later
+License: (BSD-3-Clause), (LGPL-2.1-or-later)
 Keywords: neuromorphic,ai,artificial intelligence,neural models,spiking neural networks
 Author: Intel's Neuromorphic Computing Lab and the open source community
 Author-email: lava@intel.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: License :: OSI Approved
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

