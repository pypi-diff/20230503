# Comparing `tmp/datasketches-4.0.1.tar.gz` & `tmp/datasketches-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasketches-4.0.1.tar", last modified: Tue Jan 24 21:15:17 2023, max compression
+gzip compressed data, was "datasketches-4.1.0.tar", last modified: Tue Apr 25 21:59:44 2023, max compression
```

## Comparing `datasketches-4.0.1.tar` & `datasketches-4.1.0.tar`

### file list

```diff
@@ -1,315 +1,349 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.991014 datasketches-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-01-24 21:15:02.000000 datasketches-4.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-01-24 21:15:02.000000 datasketches-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-01-24 21:15:02.000000 datasketches-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-24 21:15:02.000000 datasketches-4.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-01-24 21:15:17.991014 datasketches-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-01-24 21:15:02.000000 datasketches-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.959013 datasketches-4.0.1/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-24 21:15:02.000000 datasketches-4.0.1/cmake/DataSketchesConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.959013 datasketches-4.0.1/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.959013 datasketches-4.0.1/common/include/
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/MurmurHash3.h
--rw-r--r--   0 runner    (1001) docker     (123)    27898 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/binomial_bounds.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/bounds_binomial_proportions.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/ceiling_power_of_2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/common_defs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/conditional_back_inserter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/conditional_forward.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/count_zeros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/inv_pow2_table.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/kolmogorov_smirnov.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/kolmogorov_smirnov_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/memory_operations.hpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     6236 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/quantiles_sorted_view.hpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/quantiles_sorted_view_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/serde.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/include/version.hpp.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.959013 datasketches-4.0.1/common/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/catch_runner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/integration_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/quantiles_sorted_view_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/test_allocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/test_allocator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-01-24 21:15:02.000000 datasketches-4.0.1/common/test/test_type.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.959013 datasketches-4.0.1/cpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.963013 datasketches-4.0.1/cpc/include/
--rw-r--r--   0 runner    (1001) docker     (123)   166721 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/compression_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_compressor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_compressor_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_confidence.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    32415 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_sketch_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_union.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_union_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/cpc_util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/icon_estimator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/kxp_byte_lookup.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/u32_table.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/include/u32_table_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.963013 datasketches-4.0.1/cpc/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/test/compression_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/test/cpc_sketch_allocation_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/test/cpc_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-01-24 21:15:02.000000 datasketches-4.0.1/cpc/test/cpc_union_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.963013 datasketches-4.0.1/fi/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.963013 datasketches-4.0.1/fi/include/
--rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/include/frequent_items_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/include/frequent_items_sketch_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/include/reverse_purge_hash_map.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/include/reverse_purge_hash_map_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.963013 datasketches-4.0.1/fi/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/frequent_items_sketch_custom_type_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/frequent_items_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/items_sketch_string_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/items_sketch_string_utf8_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/longs_sketch_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-24 21:15:02.000000 datasketches-4.0.1/fi/test/reverse_purge_hash_map_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.963013 datasketches-4.0.1/hll/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/hll/include/
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/AuxHashMap-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/AuxHashMap.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    73094 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CompositeInterpolationXTable-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CompositeInterpolationXTable.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CouponHashSet-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CouponHashSet.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CouponList-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CouponList.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CubicInterpolation-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/CubicInterpolation.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HarmonicNumbers-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HarmonicNumbers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/Hll4Array-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/Hll4Array.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/Hll6Array-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/Hll6Array.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/Hll8Array-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/Hll8Array.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllArray-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllArray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllSketch-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllSketchImpl-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllSketchImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllSketchImplFactory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllUnion-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/HllUtil.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/RelativeErrorTables-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/RelativeErrorTables.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/coupon_iterator-internal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/coupon_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/hll.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/include/hll.private.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/hll/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/AuxHashMapTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/CouponHashSetTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/CouponListTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/CrossCountingTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/HllArrayTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/HllSketchTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/HllUnionTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/IsomorphicTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/TablesTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/ToFromByteArrayTest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/array6_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/compact_array4_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/compact_set_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/list_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/updatable_array4_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-24 21:15:02.000000 datasketches-4.0.1/hll/test/updatable_set_from_java.sk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/kll/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/kll/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/include/kll_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/include/kll_helper_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26925 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/include/kll_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    45293 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/include/kll_sketch_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/kll/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/kll_sketch_custom_type_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/kll_sketch_float_one_item_v1.sk
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/kll_sketch_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)    36293 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/kll_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/kll_sketch_validation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-01-24 21:15:02.000000 datasketches-4.0.1/kll/test/kolmogorov_smirnov_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-24 21:15:02.000000 datasketches-4.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.971014 datasketches-4.0.1/python/datasketches/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/datasketches/PySerDe.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/datasketches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.975014 datasketches-4.0.1/python/datasketches.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-01-24 21:15:17.000000 datasketches-4.0.1/python/datasketches.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-01-24 21:15:17.000000 datasketches-4.0.1/python/datasketches.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 21:15:17.000000 datasketches-4.0.1/python/datasketches.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 21:15:17.000000 datasketches-4.0.1/python/datasketches.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 21:15:17.000000 datasketches-4.0.1/python/datasketches.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-24 21:15:17.000000 datasketches-4.0.1/python/datasketches.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.975014 datasketches-4.0.1/python/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/include/py_serde.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.975014 datasketches-4.0.1/python/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/jupyter/CPCSketch.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/jupyter/FrequentItemsSketch.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/jupyter/HLLSketch.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/jupyter/KLLSketch.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/jupyter/ThetaSketchNotebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/pybind11Path.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.975014 datasketches-4.0.1/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/cpc_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/datasketches.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/fi_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/hll_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/kll_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/ks_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/py_serde.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/quantiles_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/req_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/theta_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/vector_of_kll.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/src/vo_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.975014 datasketches-4.0.1/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/cpc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/fi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/hll_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/kll_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/quantiles_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/req_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/theta_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/vector_of_kll_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-01-24 21:15:02.000000 datasketches-4.0.1/python/tests/vo_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.975014 datasketches-4.0.1/quantiles/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1394 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/quantiles/include/
--rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/include/quantiles_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    51084 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/include/quantiles_sketch_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/quantiles/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/test/kolmogorov_smirnov_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/test/quantiles_compatibility_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    39668 2023-01-24 21:15:02.000000 datasketches-4.0.1/quantiles/test/quantiles_sketch_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/req/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/req/include/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1141 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/include/req_common.hpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     5437 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/include/req_compactor.hpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    19485 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/include/req_compactor_impl.hpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    16251 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/include/req_sketch.hpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    32464 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/include/req_sketch_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/req/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_float_empty_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_float_estimation_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_float_exact_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_float_raw_items_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_float_single_item_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_sketch_custom_type_test.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    21901 2023-01-24 21:15:02.000000 datasketches-4.0.1/req/test/req_sketch_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/sampling/include/
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/include/var_opt_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    58878 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/include/var_opt_sketch_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/include/var_opt_union.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/include/var_opt_union_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.979014 datasketches-4.0.1/sampling/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/binaries_from_java.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/var_opt_allocation_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/var_opt_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/var_opt_union_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/varopt_sketch_long_sampling.sk
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/varopt_sketch_string_exact.sk
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-24 21:15:02.000000 datasketches-4.0.1/sampling/test/varopt_union_double_sampling.sk
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 21:15:17.991014 datasketches-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-01-24 21:15:02.000000 datasketches-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.983014 datasketches-4.0.1/theta/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.987014 datasketches-4.0.1/theta/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/bounds_on_ratios_in_sampled_sets.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/bounds_on_ratios_in_theta_sketched_sets.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/compact_theta_sketch_parser.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/compact_theta_sketch_parser_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_a_not_b.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_a_not_b_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_comparators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_intersection_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_intersection_base_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_intersection_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_jaccard_similarity.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_jaccard_similarity_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_set_difference_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_set_difference_base_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_sketch_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_union.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_union_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_union_base_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_union_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_update_sketch_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/include/theta_update_sketch_base_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.987014 datasketches-4.0.1/theta/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_a_not_b_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_empty_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_empty_from_java_v1.sk
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_empty_from_java_v2.sk
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_estimation_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_estimation_from_java_v1.sk
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_estimation_from_java_v2.sk
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_exact_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_compact_single_item_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_intersection_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_jaccard_similarity_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_setop_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    33107 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-01-24 21:15:02.000000 datasketches-4.0.1/theta/test/theta_union_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.987014 datasketches-4.0.1/tuple/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.991014 datasketches-4.0.1/tuple/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_a_not_b.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_a_not_b_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_intersection_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_sketch_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_union.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/array_of_doubles_union_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_a_not_b.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_a_not_b_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_intersection_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_jaccard_similarity.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_sketch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_sketch_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_union.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/include/tuple_union_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 21:15:17.991014 datasketches-4.0.1/tuple/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/aod_1_compact_empty_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)    69496 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/aod_1_compact_estimation_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/aod_1_compact_non_empty_no_entries_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/aod_2_compact_exact_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/aod_3_compact_empty_from_java.sk
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/array_of_doubles_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/engagement_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/tuple_a_not_b_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/tuple_intersection_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/tuple_jaccard_similarity_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/tuple_sketch_allocation_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/tuple_sketch_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-01-24 21:15:02.000000 datasketches-4.0.1/tuple/test/tuple_union_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 21:15:02.000000 datasketches-4.0.1/version.cfg.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.824444 datasketches-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-25 21:59:31.000000 datasketches-4.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-04-25 21:59:31.000000 datasketches-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 21:59:31.000000 datasketches-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-25 21:59:31.000000 datasketches-4.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-25 21:59:44.824444 datasketches-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-25 21:59:31.000000 datasketches-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.756443 datasketches-4.1.0/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-25 21:59:31.000000 datasketches-4.1.0/cmake/DataSketchesConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.756443 datasketches-4.1.0/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.760443 datasketches-4.1.0/common/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/MurmurHash3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27898 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/binomial_bounds.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/bounds_binomial_proportions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/ceiling_power_of_2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/common_defs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/conditional_back_inserter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/conditional_forward.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/count_zeros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/inv_pow2_table.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/kolmogorov_smirnov.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/kolmogorov_smirnov_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/memory_operations.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6236 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/quantiles_sorted_view.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/quantiles_sorted_view_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/serde.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/include/version.hpp.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.760443 datasketches-4.1.0/common/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/catch_runner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/integration_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/quantiles_sorted_view_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/test_allocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/test_allocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-25 21:59:31.000000 datasketches-4.1.0/common/test/test_type.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.760443 datasketches-4.1.0/count/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-25 21:59:31.000000 datasketches-4.1.0/count/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.760443 datasketches-4.1.0/count/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-04-25 21:59:31.000000 datasketches-4.1.0/count/include/count_min.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-04-25 21:59:31.000000 datasketches-4.1.0/count/include/count_min_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.764443 datasketches-4.1.0/count/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-25 21:59:31.000000 datasketches-4.1.0/count/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-25 21:59:31.000000 datasketches-4.1.0/count/test/count_min_allocation_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-25 21:59:31.000000 datasketches-4.1.0/count/test/count_min_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.764443 datasketches-4.1.0/cpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.764443 datasketches-4.1.0/cpc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)   166721 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/compression_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_compressor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_compressor_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_confidence.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32415 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_sketch_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_union.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_union_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/cpc_util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/icon_estimator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/kxp_byte_lookup.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/u32_table.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/include/u32_table_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.768443 datasketches-4.1.0/cpc/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/test/compression_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/test/cpc_sketch_allocation_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/test/cpc_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-25 21:59:31.000000 datasketches-4.1.0/cpc/test/cpc_union_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.768443 datasketches-4.1.0/density/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-25 21:59:31.000000 datasketches-4.1.0/density/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.768443 datasketches-4.1.0/density/include/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7588 2023-04-25 21:59:31.000000 datasketches-4.1.0/density/include/density_sketch.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18302 2023-04-25 21:59:31.000000 datasketches-4.1.0/density/include/density_sketch_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.768443 datasketches-4.1.0/density/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-25 21:59:31.000000 datasketches-4.1.0/density/test/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8044 2023-04-25 21:59:31.000000 datasketches-4.1.0/density/test/density_sketch_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.768443 datasketches-4.1.0/fi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.768443 datasketches-4.1.0/fi/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/include/frequent_items_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/include/frequent_items_sketch_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/include/reverse_purge_hash_map.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/include/reverse_purge_hash_map_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.772443 datasketches-4.1.0/fi/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/frequent_items_sketch_custom_type_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/frequent_items_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/items_sketch_string_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/items_sketch_string_utf8_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/longs_sketch_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-25 21:59:31.000000 datasketches-4.1.0/fi/test/reverse_purge_hash_map_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.772443 datasketches-4.1.0/hll/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.776443 datasketches-4.1.0/hll/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/AuxHashMap-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/AuxHashMap.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    73094 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CompositeInterpolationXTable-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CompositeInterpolationXTable.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CouponHashSet-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CouponHashSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CouponList-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CouponList.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CubicInterpolation-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/CubicInterpolation.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HarmonicNumbers-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HarmonicNumbers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13130 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/Hll4Array-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/Hll4Array.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/Hll6Array-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/Hll6Array.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/Hll8Array-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/Hll8Array.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24850 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllArray-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllArray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllSketch-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllSketchImpl-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllSketchImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllSketchImplFactory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllUnion-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/HllUtil.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/RelativeErrorTables-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/RelativeErrorTables.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/coupon_iterator-internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/coupon_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/hll.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/include/hll.private.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.780443 datasketches-4.1.0/hll/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/AuxHashMapTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/CouponHashSetTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/CouponListTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/CrossCountingTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/HllArrayTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/HllSketchTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/HllUnionTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/IsomorphicTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/TablesTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/ToFromByteArrayTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/array6_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/compact_array4_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/compact_set_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/list_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/updatable_array4_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 21:59:31.000000 datasketches-4.1.0/hll/test/updatable_set_from_java.sk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.780443 datasketches-4.1.0/kll/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.780443 datasketches-4.1.0/kll/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/include/kll_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/include/kll_helper_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/include/kll_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    45256 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/include/kll_sketch_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.784443 datasketches-4.1.0/kll/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/kll_sketch_custom_type_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/kll_sketch_float_one_item_v1.sk
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/kll_sketch_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    36303 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/kll_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/kll_sketch_validation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-25 21:59:31.000000 datasketches-4.1.0/kll/test/kolmogorov_smirnov_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-25 21:59:31.000000 datasketches-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.784443 datasketches-4.1.0/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.784443 datasketches-4.1.0/python/datasketches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/datasketches/DensityWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/datasketches/KernelFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/datasketches/PySerDe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/datasketches/TuplePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/datasketches/TupleWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/datasketches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.788444 datasketches-4.1.0/python/datasketches.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-25 21:59:44.000000 datasketches-4.1.0/python/datasketches.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-25 21:59:44.000000 datasketches-4.1.0/python/datasketches.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:59:44.000000 datasketches-4.1.0/python/datasketches.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:59:44.000000 datasketches-4.1.0/python/datasketches.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 21:59:44.000000 datasketches-4.1.0/python/datasketches.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 21:59:44.000000 datasketches-4.1.0/python/datasketches.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.788444 datasketches-4.1.0/python/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/include/kernel_function.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/include/py_object_lt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/include/py_object_ostream.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/include/py_serde.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/include/quantile_conditional.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/include/tuple_policy.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.788444 datasketches-4.1.0/python/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/jupyter/CPCSketch.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/jupyter/FrequentItemsSketch.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/jupyter/HLLSketch.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18111 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/jupyter/KLLSketch.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/jupyter/ThetaSketchNotebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/pybind11Path.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.796444 datasketches-4.1.0/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/count_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/cpc_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/datasketches.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/density_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/fi_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/hll_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/kll_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/ks_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/py_serde.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/quantiles_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/req_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/theta_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/tuple_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/vector_of_kll.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/src/vo_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.800444 datasketches-4.1.0/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/count_min_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/cpc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/density_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/fi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/hll_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/kll_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/quantiles_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/req_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/theta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/tuple_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/vector_of_kll_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-25 21:59:31.000000 datasketches-4.1.0/python/tests/vo_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.800444 datasketches-4.1.0/quantiles/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1394 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.800444 datasketches-4.1.0/quantiles/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26586 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/include/quantiles_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    51015 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/include/quantiles_sketch_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.800444 datasketches-4.1.0/quantiles/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/test/kolmogorov_smirnov_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/test/quantiles_compatibility_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39673 2023-04-25 21:59:31.000000 datasketches-4.1.0/quantiles/test/quantiles_sketch_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.800444 datasketches-4.1.0/req/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.804444 datasketches-4.1.0/req/include/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1141 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/include/req_common.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5437 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/include/req_compactor.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19465 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/include/req_compactor_impl.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16345 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/include/req_sketch.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32427 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/include/req_sketch_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.804444 datasketches-4.1.0/req/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_float_empty_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_float_estimation_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_float_exact_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_float_raw_items_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_float_single_item_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_sketch_custom_type_test.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21901 2023-04-25 21:59:31.000000 datasketches-4.1.0/req/test/req_sketch_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.804444 datasketches-4.1.0/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.808444 datasketches-4.1.0/sampling/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/include/var_opt_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    59052 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/include/var_opt_sketch_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/include/var_opt_union.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/include/var_opt_union_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.808444 datasketches-4.1.0/sampling/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/binaries_from_java.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/var_opt_allocation_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19657 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/var_opt_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/var_opt_union_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/varopt_sketch_long_sampling.sk
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/varopt_sketch_string_exact.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-25 21:59:31.000000 datasketches-4.1.0/sampling/test/varopt_union_double_sampling.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:59:44.824444 datasketches-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-25 21:59:31.000000 datasketches-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.808444 datasketches-4.1.0/theta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.816444 datasketches-4.1.0/theta/include/
+-rw-r--r--   0 runner    (1001) docker     (123)   169180 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/bit_packing.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/bounds_on_ratios_in_sampled_sets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/bounds_on_ratios_in_theta_sketched_sets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/compact_theta_sketch_parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/compact_theta_sketch_parser_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_a_not_b.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_a_not_b_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_comparators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_intersection_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_intersection_base_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_intersection_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_jaccard_similarity.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_jaccard_similarity_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_set_difference_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_set_difference_base_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31071 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_sketch_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_union.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_union_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_union_base_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_union_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_update_sketch_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/include/theta_update_sketch_base_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.816444 datasketches-4.1.0/theta/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/bit_packing_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_a_not_b_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_empty_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_empty_from_java_v1.sk
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_empty_from_java_v2.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_estimation_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_estimation_from_java_v1.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_estimation_from_java_v2.sk
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_exact_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_compact_single_item_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_intersection_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_jaccard_similarity_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_setop_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34710 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-25 21:59:31.000000 datasketches-4.1.0/theta/test/theta_union_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.820444 datasketches-4.1.0/tuple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.820444 datasketches-4.1.0/tuple/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_a_not_b.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_a_not_b_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_intersection_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_sketch_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_union.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/array_of_doubles_union_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_a_not_b.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_a_not_b_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_intersection_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_jaccard_similarity.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_sketch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_sketch_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_union.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/include/tuple_union_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:59:44.824444 datasketches-4.1.0/tuple/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/aod_1_compact_empty_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    69496 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/aod_1_compact_estimation_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/aod_1_compact_non_empty_no_entries_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/aod_2_compact_exact_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/aod_3_compact_empty_from_java.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/array_of_doubles_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/engagement_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/tuple_a_not_b_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/tuple_intersection_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/tuple_jaccard_similarity_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/tuple_sketch_allocation_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/tuple_sketch_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-25 21:59:31.000000 datasketches-4.1.0/tuple/test/tuple_union_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 21:59:31.000000 datasketches-4.1.0/version.cfg.in
```

### Comparing `datasketches-4.0.1/CMakeLists.txt` & `datasketches-4.1.0/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 include(GNUInstallDirs)
 include(CMakeDependentOption)
 
 ### Require out-of-source builds
 file(TO_CMAKE_PATH "${PROJECT_BINARY_DIR}/CMakeLists.txt" LOC_PATH)
 if(EXISTS "${LOC_PATH}")
-    message(FATAL_ERROR "You cannot build in a source directory (or any directory with a CMakeLists.txt file). Please make a build subdirectory. Feel free to remove CMakeCache.txt and CMakeFiles.")
+  message(FATAL_ERROR "You cannot build in a source directory (or any directory with a CMakeLists.txt file). Please make a build subdirectory. Feel free to remove CMakeCache.txt and CMakeFiles.")
 endif()
 
 # Ensure builds on Windows export all symbols
 set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
 
 #set(CMAKE_VERBOSE_MAKEFILE ON)
 set(CMAKE_MACOSX_RPATH ON)
@@ -65,15 +65,15 @@
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 #list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake)
 
 ###### OPTIONS ######
 # Enable testing
 option(BUILD_TESTS "Build unit tests" ON)
-if (BUILD_TESTS)  
+if (BUILD_TESTS)
   enable_testing()
 endif()
 
 option(COVERAGE "Enable code coverage reporting (g++/clang only)" OFF)
 if(COVERAGE AND CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
   set(CMAKE_BUILD_TYPE "Debug" FORCE)
   add_compile_options(--coverage -O0 -g3)
@@ -89,18 +89,18 @@
 
 # set default build type to Release
 # Derived from: https://blog.kitware.com/cmake-and-the-default-build-type/
 set(default_build_type "Release")
 if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
   message(STATUS "Setting build type to '${default_build_type}' as none was specified.")
   set(CMAKE_BUILD_TYPE "${default_build_type}" CACHE
-      STRING "Choose the type of build." FORCE)
+          STRING "Choose the type of build." FORCE)
   # Set the possible values of build type for cmake-gui
   set_property(CACHE CMAKE_BUILD_TYPE PROPERTY STRINGS
-    "Debug" "Release" "MinSizeRel" "RelWithDebInfo")
+          "Debug" "Release" "MinSizeRel" "RelWithDebInfo")
 endif()
 
 ###### TARGETS ######
 # do we need the next line since we don't actually make a library anymore?
 add_library(datasketches INTERFACE)
 
 target_compile_features(datasketches INTERFACE cxx_std_11)
@@ -111,54 +111,56 @@
 add_subdirectory(kll)
 add_subdirectory(fi)
 add_subdirectory(theta)
 add_subdirectory(sampling)
 add_subdirectory(tuple)
 add_subdirectory(req)
 add_subdirectory(quantiles)
+add_subdirectory(count)
+add_subdirectory(density)
 
 if (WITH_PYTHON)
   add_subdirectory(python)
 endif()
 
-target_link_libraries(datasketches INTERFACE hll cpc kll fi theta sampling req quantiles)
+target_link_libraries(datasketches INTERFACE hll cpc kll fi theta sampling req quantiles count)
 
 if (COVERAGE)
   find_program(LCOV_PATH NAMES "lcov")
   find_program(GENHTML_PATH NAMES "genhtml")
   if (NOT LCOV_PATH-NOTFOUND AND NOT GENHTML_PATH-NOTFOUND)
     add_custom_target(coverage_report
-      COMMAND ${LCOV_PATH} --capture --exclude '*/test/*' --exclude '/Library/*' --exclude '/usr/include/*' --directory . --output-file lcov.info
-      COMMAND ${GENHTML_PATH} --legend lcov.info --output-directory coverage --demangle-cpp)
-    endif()
+            COMMAND ${LCOV_PATH} --capture --exclude '*/test/*' --exclude '/Library/*' --exclude '/usr/include/*' --directory . --output-file lcov.info
+            COMMAND ${GENHTML_PATH} --legend lcov.info --output-directory coverage --demangle-cpp)
+  endif()
 endif()
 
 
 # # Installation
 install(TARGETS datasketches
-  EXPORT ${PROJECT_NAME}
-  PUBLIC_HEADER DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/DataSketches
-  INCLUDES DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/DataSketches
-)
+        EXPORT ${PROJECT_NAME}
+        PUBLIC_HEADER DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/DataSketches
+        INCLUDES DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/DataSketches
+        )
 
 # Packaging
 include(CMakePackageConfigHelpers)
 write_basic_package_version_file(
-    "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfigVersion.cmake"
-    VERSION ${PROJECT_VERSION}
-    COMPATIBILITY SameMajorVersion
+        "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfigVersion.cmake"
+        VERSION ${PROJECT_VERSION}
+        COMPATIBILITY SameMajorVersion
 )
 configure_package_config_file(
-    cmake/DataSketchesConfig.cmake.in
-    "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfig.cmake"
-    INSTALL_DESTINATION lib/DataSketches/cmake
-    PATH_VARS CMAKE_INSTALL_INCLUDEDIR
+        cmake/DataSketchesConfig.cmake.in
+        "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfig.cmake"
+        INSTALL_DESTINATION lib/DataSketches/cmake
+        PATH_VARS CMAKE_INSTALL_INCLUDEDIR
 )
 install(EXPORT ${PROJECT_NAME} DESTINATION lib/DataSketches/cmake)
 install(FILES "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfigVersion.cmake"
-              "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfig.cmake"
+        "${CMAKE_CURRENT_BINARY_DIR}/DataSketchesConfig.cmake"
         DESTINATION lib/DataSketches/cmake)
 
 
 #set(CPACK_PROJECT_NAME ${PROJECT_NAME})
 #set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
 include(CPack)
```

### Comparing `datasketches-4.0.1/LICENSE` & `datasketches-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/MANIFEST.in` & `datasketches-4.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/PKG-INFO` & `datasketches-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasketches
-Version: 4.0.1
+Version: 4.1.0
 Summary: The Apache DataSketches Library for Python
 Home-page: http://datasketches.apache.org
 Author: Apache Software Foundation
 Author-email: dev@datasketches.apache.org
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,23 +20,23 @@
 
 If approximate results are acceptable, there is a class of specialized algorithms, called streaming algorithms, or sketches that can produce results orders-of magnitude faster and with mathematically proven error bounds. For interactive queries there may not be other viable alternatives, and in the case of real-time analysis, sketches are the only known solution.
 
 This package provides a variety of sketches as described below. Wherever a specific type of sketch exists in Apache DataSketches packages for other languages, the sketches will be portable between languages (for platforms with the same endianness).
 
 ## Building and Installation
 
-Once cloned, the library can be installed by running `python3 -m pip install .` in the project root directory -- not the python subdirectory -- which will also install the necessary dependencies, namely numpy and [pybind11[global]](https://github.com/pybind/pybind11).
+Once cloned, the library can be installed by running `python3 -m pip install .` in the project root directory -- not the python subdirectory -- which will also install the necessary dependencies, namely NumPy and [pybind11[global]](https://github.com/pybind/pybind11).
 
-If you prefer to call the `setup.py` build script directly, which is discoraged, you must first install `pybind11[global]`, as well as any other dependencies listed under the build-system section in `pyproject.toml`.
+If you prefer to call the `setup.py` build script directly, which is discouraged, you must first install `pybind11[global]`, as well as any other dependencies listed under the build-system section in `pyproject.toml`.
 
 The library is also available from PyPI via `python3 -m pip install datasketches`.
 
 ## Usage
 
-Having installed the library, loading the Apache Datasketches Library in Python is simple: `import datasketches`.
+Having installed the library, loading the Apache DataSketches Library in Python is simple: `import datasketches`.
 
 The unit tests are mostly structured in a tutorial style and can be used as a reference example for how to feed data into and query the different types of sketches.
 
 ## Available Sketch Classes
 
 - KLL (Absolute Error Quantiles)
   - `kll_ints_sketch`
@@ -84,14 +84,14 @@
 
 ## Developer Instructions
 
 The only developer-specific instructions relate to running unit tests.
 
 ### Unit tests
 
-The Python unit tests are run via `tox`, with no arguments, from the project root directory -- not the python subdirectory. Tox creates a temporary virtual environment in which to build and run the unit tests. In the event you are missing the necessary pacakge, tox may be installed with `python3 -m pip install --upgrade tox`.
+The Python unit tests are run via `tox`, with no arguments, from the project root directory -- not the python subdirectory. Tox creates a temporary virtual environment in which to build and run the unit tests. In the event you are missing the necessary package, tox may be installed with `python3 -m pip install --upgrade tox`.
 
 ## License
 
-The Apache DataSketches Library is distrubted under an Apache 2.0 License.
+The Apache DataSketches Library is distributed under the Apache 2.0 License.
 
 There may be precompiled binaries provided as a convenience and distributed through PyPI via [https://pypi.org/project/datasketches/] contain compiled code from [pybind11](https://github.com/pybind/pybind11), which is distributed under a BSD license.
```

### Comparing `datasketches-4.0.1/README.md` & `datasketches-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/CMakeLists.txt` & `datasketches-4.1.0/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/MurmurHash3.h` & `datasketches-4.1.0/common/include/MurmurHash3.h`

 * *Files 12% similar despite different names*

```diff
@@ -25,45 +25,38 @@
 
 #if defined(_MSC_VER)
 
 typedef unsigned char uint8_t;
 typedef unsigned int uint32_t;
 typedef unsigned __int64 uint64_t;
 
-#define FORCE_INLINE	__forceinline
+#define MURMUR3_FORCE_INLINE	__forceinline
 
 #include <stdlib.h>
 
-#define ROTL32(x,y)	_rotl(x,y)
-#define ROTL64(x,y)	_rotl64(x,y)
+#define MURMUR3_ROTL64(x,y)	_rotl64(x,y)
 
-#define BIG_CONSTANT(x) (x)
+#define MURMUR3_BIG_CONSTANT(x) (x)
 
 // Other compilers
 
 #else   // defined(_MSC_VER)
 
 #include <stdint.h>
 
-#define	FORCE_INLINE inline __attribute__((always_inline))
-
-inline uint32_t rotl32 ( uint32_t x, int8_t r )
-{
-  return (x << r) | (x >> (32 - r));
-}
+#define	MURMUR3_FORCE_INLINE inline __attribute__((always_inline))
 
 inline uint64_t rotl64 ( uint64_t x, int8_t r )
 {
   return (x << r) | (x >> (64 - r));
 }
 
-#define	ROTL32(x,y)	rotl32(x,y)
-#define ROTL64(x,y)	rotl64(x,y)
+#define MURMUR3_ROTL64(x,y)	rotl64(x,y)
 
-#define BIG_CONSTANT(x) (x##LLU)
+#define MURMUR3_BIG_CONSTANT(x) (x##LLU)
 
 #endif // !defined(_MSC_VER)
 
 //-----------------------------------------------------------------------------
 
 //-----------------------------------------------------------------------------
 // Return type - Using C++ reference for return type which should allow better
@@ -74,38 +67,39 @@
 } HashState;
 
 
 //-----------------------------------------------------------------------------
 // Block read - if your platform needs to do endian-swapping or can only
 // handle aligned reads, do the conversion here
 
-FORCE_INLINE uint64_t getblock64 ( const uint64_t * p, size_t i )
+MURMUR3_FORCE_INLINE uint64_t getblock64 ( const uint64_t * p, size_t i )
 {
   uint64_t res;
   memcpy(&res, p + i, sizeof(res));
   return res;
 }
 
 //-----------------------------------------------------------------------------
 // Finalization mix - force all bits of a hash block to avalanche
 
-FORCE_INLINE uint64_t fmix64 ( uint64_t k )
+MURMUR3_FORCE_INLINE uint64_t fmix64 ( uint64_t k )
 {
   k ^= k >> 33;
-  k *= BIG_CONSTANT(0xff51afd7ed558ccd);
+  k *= MURMUR3_BIG_CONSTANT(0xff51afd7ed558ccd);
   k ^= k >> 33;
-  k *= BIG_CONSTANT(0xc4ceb9fe1a85ec53);
+  k *= MURMUR3_BIG_CONSTANT(0xc4ceb9fe1a85ec53);
   k ^= k >> 33;
 
   return k;
 }
 
-FORCE_INLINE void MurmurHash3_x64_128(const void* key, size_t lenBytes, uint64_t seed, HashState& out) {
-  static const uint64_t c1 = BIG_CONSTANT(0x87c37b91114253d5);
-  static const uint64_t c2 = BIG_CONSTANT(0x4cf5ad432745937f);
+MURMUR3_FORCE_INLINE void MurmurHash3_x64_128(const void* key, size_t lenBytes,
+                                              uint64_t seed, HashState& out) {
+  static const uint64_t c1 = MURMUR3_BIG_CONSTANT(0x87c37b91114253d5);
+  static const uint64_t c2 = MURMUR3_BIG_CONSTANT(0x4cf5ad432745937f);
 
   const uint8_t* data = (const uint8_t*)key;
 
   out.h1 = seed;
   out.h2 = seed;
 
   // Number of full 128-bit blocks of 16 bytes.
@@ -114,21 +108,21 @@
 
   // Process the 128-bit blocks (the body) into the hash
   const uint64_t* blocks = (const uint64_t*)(data);
   for (size_t i = 0; i < nblocks; ++i) { // 16 bytes per block
     uint64_t k1 = getblock64(blocks, i * 2 + 0);
     uint64_t k2 = getblock64(blocks, i * 2 + 1);
 
-    k1 *= c1; k1  = ROTL64(k1,31); k1 *= c2; out.h1 ^= k1;
-    out.h1 = ROTL64(out.h1,27);
+    k1 *= c1; k1  = MURMUR3_ROTL64(k1,31); k1 *= c2; out.h1 ^= k1;
+    out.h1 = MURMUR3_ROTL64(out.h1,27);
     out.h1 += out.h2;
     out.h1 = out.h1*5+0x52dce729;
 
-    k2 *= c2; k2  = ROTL64(k2,33); k2 *= c1; out.h2 ^= k2;
-    out.h2 = ROTL64(out.h2,31);
+    k2 *= c2; k2  = MURMUR3_ROTL64(k2,33); k2 *= c1; out.h2 ^= k2;
+    out.h2 = MURMUR3_ROTL64(out.h2,31);
     out.h2 += out.h1;
     out.h2 = out.h2*5+0x38495ab5;
   }
 
   // tail
   const uint8_t * tail = (const uint8_t*)(data + (nblocks << 4));
 
@@ -140,25 +134,25 @@
   case 15: k2 ^= ((uint64_t)tail[14]) << 48; // falls through
   case 14: k2 ^= ((uint64_t)tail[13]) << 40; // falls through
   case 13: k2 ^= ((uint64_t)tail[12]) << 32; // falls through
   case 12: k2 ^= ((uint64_t)tail[11]) << 24; // falls through
   case 11: k2 ^= ((uint64_t)tail[10]) << 16; // falls through
   case 10: k2 ^= ((uint64_t)tail[ 9]) << 8;  // falls through
   case  9: k2 ^= ((uint64_t)tail[ 8]) << 0;
-           k2 *= c2; k2  = ROTL64(k2,33); k2 *= c1; out.h2 ^= k2;
+           k2 *= c2; k2  = MURMUR3_ROTL64(k2,33); k2 *= c1; out.h2 ^= k2;
            // falls through
   case  8: k1 ^= ((uint64_t)tail[ 7]) << 56; // falls through
   case  7: k1 ^= ((uint64_t)tail[ 6]) << 48; // falls through
   case  6: k1 ^= ((uint64_t)tail[ 5]) << 40; // falls through
   case  5: k1 ^= ((uint64_t)tail[ 4]) << 32; // falls through
   case  4: k1 ^= ((uint64_t)tail[ 3]) << 24; // falls through
   case  3: k1 ^= ((uint64_t)tail[ 2]) << 16; // falls through
   case  2: k1 ^= ((uint64_t)tail[ 1]) << 8; // falls through
   case  1: k1 ^= ((uint64_t)tail[ 0]) << 0;
-           k1 *= c1; k1  = ROTL64(k1,31); k1 *= c2; out.h1 ^= k1;
+           k1 *= c1; k1  = MURMUR3_ROTL64(k1,31); k1 *= c2; out.h1 ^= k1;
   };
 
   //----------
   // finalization
 
   out.h1 ^= lenBytes;
   out.h2 ^= lenBytes;
@@ -171,14 +165,18 @@
 
   out.h1 += out.h2;
   out.h2 += out.h1;
 }
 
 //-----------------------------------------------------------------------------
 
-FORCE_INLINE uint16_t compute_seed_hash(uint64_t seed) {
+MURMUR3_FORCE_INLINE uint16_t compute_seed_hash(uint64_t seed) {
   HashState hashes;
   MurmurHash3_x64_128(&seed, sizeof(seed), 0, hashes);
   return static_cast<uint16_t>(hashes.h1 & 0xffff);
 }
 
+#undef MURMUR3_FORCE_INLINE
+#undef MURMUR3_ROTL64
+#undef MURMUR3_BIG_CONSTANT
+
 #endif // _MURMURHASH3_H_
```

### Comparing `datasketches-4.0.1/common/include/binomial_bounds.hpp` & `datasketches-4.1.0/common/include/binomial_bounds.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/bounds_binomial_proportions.hpp` & `datasketches-4.1.0/common/include/bounds_binomial_proportions.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/ceiling_power_of_2.hpp` & `datasketches-4.1.0/common/include/ceiling_power_of_2.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/common_defs.hpp` & `datasketches-4.1.0/common/include/common_defs.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -22,33 +22,35 @@
 
 #include <cstdint>
 #include <string>
 #include <memory>
 #include <iostream>
 #include <random>
 #include <chrono>
+#include <thread>
 
 namespace datasketches {
 
 static const uint64_t DEFAULT_SEED = 9001;
 
 enum resize_factor { X1 = 0, X2, X4, X8 };
 
 template<typename A> using AllocChar = typename std::allocator_traits<A>::template rebind_alloc<char>;
 template<typename A> using string = std::basic_string<char, std::char_traits<char>, AllocChar<A>>;
 
-// random bit
-static std::independent_bits_engine<std::mt19937, 1, uint32_t>
-  random_bit(static_cast<uint32_t>(std::chrono::system_clock::now().time_since_epoch().count()));
+// thread-safe random bit
+static thread_local std::independent_bits_engine<std::mt19937, 1, uint32_t>
+  random_bit(static_cast<uint32_t>(std::chrono::system_clock::now().time_since_epoch().count() 
+    + std::hash<std::thread::id>{}(std::this_thread::get_id())));
 
 // common random declarations
 namespace random_utils {
   static std::random_device rd; // possibly unsafe in MinGW with GCC < 9.2
-  static std::mt19937_64 rand(rd());
-  static std::uniform_real_distribution<> next_double(0.0, 1.0);
+  static thread_local std::mt19937_64 rand(rd());
+  static thread_local std::uniform_real_distribution<> next_double(0.0, 1.0);
 }
 
 
 // utility function to hide unused compiler warning
 // usually has no additional cost
 template<typename T> void unused(T&&...) {}
 
@@ -73,15 +75,15 @@
 
 template<typename T>
 static inline void read(std::istream& is, T* ptr, size_t size_bytes) {
   is.read(reinterpret_cast<char*>(ptr), size_bytes);
 }
 
 template<typename T>
-static inline void write(std::ostream& os, T& value) {
+static inline void write(std::ostream& os, T value) {
   os.write(reinterpret_cast<const char*>(&value), sizeof(T));
 }
 
 template<typename T>
 static inline void write(std::ostream& os, const T* ptr, size_t size_bytes) {
   os.write(reinterpret_cast<const char*>(ptr), size_bytes);
 }
```

### Comparing `datasketches-4.0.1/common/include/conditional_back_inserter.hpp` & `datasketches-4.1.0/common/include/conditional_back_inserter.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/conditional_forward.hpp` & `datasketches-4.1.0/common/include/conditional_forward.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/count_zeros.hpp` & `datasketches-4.1.0/common/include/count_zeros.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,25 @@
     return 40 + byte_leading_zeros_table[(input >> 16) & FCLZ_MASK_08];
   if (input > FCLZ_MASK_08)
     return 48 + byte_leading_zeros_table[(input >>  8) & FCLZ_MASK_08];
   if (true)
     return 56 + byte_leading_zeros_table[(input      ) & FCLZ_MASK_08];
 }
 
+static inline uint8_t count_leading_zeros_in_u32(uint32_t input) {
+  if (input > FCLZ_MASK_24)
+    return      byte_leading_zeros_table[(input >> 24) & FCLZ_MASK_08];
+  if (input > FCLZ_MASK_16)
+    return 8 + byte_leading_zeros_table[(input >> 16) & FCLZ_MASK_08];
+  if (input > FCLZ_MASK_08)
+    return 16 + byte_leading_zeros_table[(input >>  8) & FCLZ_MASK_08];
+  if (true)
+    return 24 + byte_leading_zeros_table[(input      ) & FCLZ_MASK_08];
+}
+
 static inline uint8_t count_trailing_zeros_in_u32(uint32_t input) {
   for (int i = 0; i < 4; i++) {
     const int byte = input & 0xff;
     if (byte != 0) return static_cast<uint8_t>((i << 3) + byte_trailing_zeros_table[byte]);
     input >>= 8;
   }
   return 32;
```

### Comparing `datasketches-4.0.1/common/include/inv_pow2_table.hpp` & `datasketches-4.1.0/common/include/inv_pow2_table.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/kolmogorov_smirnov.hpp` & `datasketches-4.1.0/common/include/kolmogorov_smirnov.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/kolmogorov_smirnov_impl.hpp` & `datasketches-4.1.0/common/include/kolmogorov_smirnov_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/memory_operations.hpp` & `datasketches-4.1.0/common/include/memory_operations.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #ifndef _MEMORY_OPERATIONS_HPP_
 #define _MEMORY_OPERATIONS_HPP_
 
 #include <memory>
 #include <exception>
 #include <iostream>
 #include <string>
+#include <cstring>
 
 namespace datasketches {
 
 static inline void ensure_minimum_memory(size_t bytes_available, size_t min_needed) {
   if (bytes_available < min_needed) {
     throw std::out_of_range("Insufficient buffer size detected: bytes available "
     + std::to_string(bytes_available) + ", minimum needed " + std::to_string(min_needed));
@@ -50,21 +51,21 @@
 // note: size is in bytes, not items
 static inline size_t copy_to_mem(const void* src, void* dst, size_t size) {
   memcpy(dst, src, size);
   return size;
 }
 
 template<typename T>
-static inline size_t copy_to_mem(const T& item, void* dst) {
-  memcpy(dst, &item, sizeof(T));
+static inline size_t copy_from_mem(const void* src, T& item) {
+  memcpy(&item, src, sizeof(T));
   return sizeof(T);
 }
 
 template<typename T>
-static inline size_t copy_from_mem(const void* src, T& item) {
-  memcpy(&item, src, sizeof(T));
+static inline size_t copy_to_mem(T item, void* dst) {
+  memcpy(dst, &item, sizeof(T));
   return sizeof(T);
 }
 
 } // namespace
 
 #endif // _MEMORY_OPERATIONS_HPP_
```

### Comparing `datasketches-4.0.1/common/include/quantiles_sorted_view.hpp` & `datasketches-4.1.0/common/include/quantiles_sorted_view.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/quantiles_sorted_view_impl.hpp` & `datasketches-4.1.0/common/include/quantiles_sorted_view_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/serde.hpp` & `datasketches-4.1.0/common/include/serde.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/include/version.hpp.in` & `datasketches-4.1.0/common/include/version.hpp.in`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/test/CMakeLists.txt` & `datasketches-4.1.0/common/test/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   PRIVATE
     quantiles_sorted_view_test.cpp
 )
 
 # now the integration test part
 add_executable(integration_test)
 
-target_link_libraries(integration_test cpc fi hll kll req sampling theta tuple common_test_lib)
+target_link_libraries(integration_test count cpc density fi hll kll req sampling theta tuple common_test_lib)
 
 set_target_properties(integration_test PROPERTIES
   CXX_STANDARD 11
   CXX_STANDARD_REQUIRED YES
 )
 
 add_test(
```

### Comparing `datasketches-4.0.1/common/test/catch_runner.cpp` & `datasketches-4.1.0/common/test/catch_runner.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/test/integration_test.cpp` & `datasketches-4.1.0/common/test/integration_test.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
 #include <catch2/catch.hpp>
 
+#include "count_min.hpp"
 #include "cpc_sketch.hpp"
 #include "cpc_union.hpp"
+#include "density_sketch.hpp"
 #include "frequent_items_sketch.hpp"
 #include "hll.hpp"
 #include "kll_sketch.hpp"
 #include "req_sketch.hpp"
 #include "var_opt_sketch.hpp"
 #include "var_opt_union.hpp"
 #include "theta_sketch.hpp"
@@ -44,17 +46,21 @@
     summary -= other;
   }
 };
 
 using tuple_intersection_float = tuple_intersection<float, subtracting_intersection_policy<float>>;
 
 TEST_CASE("integration: declare all sketches", "[integration]") {
+  count_min_sketch<double> cm(5, 128);
+
   cpc_sketch cpc(12);
   cpc_union cpc_u(12);
 
+  density_sketch<double> ds(32, 3);
+
   frequent_items_sketch<std::string> fi(100);
 
   hll_sketch hll(13);
   hll_union hll_u(13);
 
   kll_sketch<double> kll(200);
```

### Comparing `datasketches-4.0.1/common/test/quantiles_sorted_view_test.cpp` & `datasketches-4.1.0/common/test/quantiles_sorted_view_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/test/test_allocator.cpp` & `datasketches-4.1.0/common/test/test_allocator.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/test/test_allocator.hpp` & `datasketches-4.1.0/common/test/test_allocator.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/common/test/test_type.hpp` & `datasketches-4.1.0/common/test/test_type.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/CMakeLists.txt` & `datasketches-4.1.0/cpc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/compression_data.hpp` & `datasketches-4.1.0/cpc/include/compression_data.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_common.hpp` & `datasketches-4.1.0/cpc/include/cpc_common.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_compressor.hpp` & `datasketches-4.1.0/cpc/include/cpc_compressor.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_compressor_impl.hpp` & `datasketches-4.1.0/cpc/include/cpc_compressor_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_confidence.hpp` & `datasketches-4.1.0/cpc/include/cpc_confidence.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #include <stdexcept>
 
 #include "cpc_sketch.hpp"
 
 namespace datasketches {
 
 // ln 2.0
-static const double ICON_ERROT_CONSTANT = 0.693147180559945286;
+static const double ICON_ERROR_CONSTANT = 0.693147180559945286;
 
 //  1,    2,    3, // kappa
 static const int16_t ICON_LOW_SIDE_DATA [33] = {   // Empirically measured at N = 1000 * K.
  6037, 5720, 5328, // 4 1000000
  6411, 6262, 5682, // 5 1000000
  6724, 6403, 6127, // 6 1000000
  6665, 6411, 6208, // 7 1000000
@@ -98,15 +98,15 @@
 template<typename A>
 double get_icon_confidence_lb(const cpc_sketch_alloc<A>& sketch, int kappa) {
   if (sketch.get_num_coupons() == 0) return 0.0;
   const int lg_k = sketch.get_lg_k();
   const long k = 1 << lg_k;
   if (lg_k < 4) throw std::logic_error("lgk < 4");
   if (kappa < 1 || kappa > 3) throw std::invalid_argument("kappa must be between 1 and 3");
-  double x = ICON_ERROT_CONSTANT;
+  double x = ICON_ERROR_CONSTANT;
   if (lg_k <= 14) x = ((double) ICON_HIGH_SIDE_DATA[3 * (lg_k - 4) + (kappa - 1)]) / 10000.0;
   const double rel = x / sqrt(k);
   const double eps = kappa * rel;
   const double est = sketch.get_icon_estimate();
   double result = est / (1.0 + eps);
   const double check = sketch.get_num_coupons();
   if (result < check) result = check;
@@ -116,15 +116,15 @@
 template<typename A>
 double get_icon_confidence_ub(const cpc_sketch_alloc<A>& sketch, int kappa) {
   if (sketch.get_num_coupons() == 0) return 0.0;
   const int lg_k = sketch.get_lg_k();
   const long k = 1 << lg_k;
   if (lg_k < 4) throw std::logic_error("lgk < 4");
   if (kappa < 1 || kappa > 3) throw std::invalid_argument("kappa must be between 1 and 3");
-  double x = ICON_ERROT_CONSTANT;
+  double x = ICON_ERROR_CONSTANT;
   if (lg_k <= 14) x = ((double) ICON_LOW_SIDE_DATA[3 * (lg_k - 4) + (kappa - 1)]) / 10000.0;
   const double rel = x / sqrt(k);
   const double eps = kappa * rel;
   const double est = sketch.get_icon_estimate();
   const double result = est / (1.0 - eps);
   return ceil(result); // widening for coverage
 }
```

### Comparing `datasketches-4.0.1/cpc/include/cpc_sketch.hpp` & `datasketches-4.1.0/cpc/include/cpc_sketch.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_sketch_impl.hpp` & `datasketches-4.1.0/cpc/include/cpc_sketch_impl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 // so that it will reflect changes that were previously outside the mantissa.
 template<typename A>
 void cpc_sketch_alloc<A>::refresh_kxp(const uint64_t* bit_matrix) {
   const uint32_t k = 1 << lg_k;
 
   // for improved numerical accuracy, we separately sum the bytes of the U64's
   double byte_sums[8]; // allocating on the stack
-  std::fill(byte_sums, &byte_sums[8], 0);
+  std::fill(byte_sums, byte_sums + 8, 0);
 
   for (size_t i = 0; i < k; i++) {
     uint64_t word = bit_matrix[i];
     for (unsigned j = 0; j < 8; j++) {
       const uint8_t byte = word & 0xff;
       byte_sums[j] += KXP_BYTE_TABLE[byte];
       word >>= 8;
```

### Comparing `datasketches-4.0.1/cpc/include/cpc_union.hpp` & `datasketches-4.1.0/cpc/include/cpc_union.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_union_impl.hpp` & `datasketches-4.1.0/cpc/include/cpc_union_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/cpc_util.hpp` & `datasketches-4.1.0/cpc/include/cpc_util.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -85,44 +85,52 @@
     count += warren_bit_count(array[i]);
   }
   return count;
 }
 
 // This code is Figure 5-9 in "Hacker's Delight" by Henry S. Warren.
 
-#define CSA(h,l,a,b,c) {uint64_t u = a ^ b; uint64_t v = c; h = (a & b) | (u & v); l = u ^ v;}
+#define DATASKETCHES_CSA(h, l, a, b, c) \
+  {                                     \
+    uint64_t u = a ^ b;                 \
+    uint64_t v = c;                     \
+    h = (a & b) | (u & v);              \
+    l = u ^ v;                          \
+  }
 
 static inline uint32_t count_bits_set_in_matrix(const uint64_t* a, uint32_t length) {
   if ((length & 0x7) != 0) throw std::invalid_argument("the length of the array must be a multiple of 8");
   uint32_t total = 0;
   uint64_t ones, twos, twos_a, twos_b, fours, fours_a, fours_b, eights;
   fours = twos = ones = 0;
 
   for (uint32_t i = 0; i <= length - 8; i += 8) {
-    CSA(twos_a, ones, ones, a[i+0], a[i+1]);
-    CSA(twos_b, ones, ones, a[i+2], a[i+3]);
-    CSA(fours_a, twos, twos, twos_a, twos_b);
-
-    CSA(twos_a, ones, ones, a[i+4], a[i+5]);
-    CSA(twos_b, ones, ones, a[i+6], a[i+7]);
-    CSA(fours_b, twos, twos, twos_a, twos_b);
+    DATASKETCHES_CSA(twos_a, ones, ones, a[i+0], a[i+1]);
+    DATASKETCHES_CSA(twos_b, ones, ones, a[i+2], a[i+3]);
+    DATASKETCHES_CSA(fours_a, twos, twos, twos_a, twos_b);
+
+    DATASKETCHES_CSA(twos_a, ones, ones, a[i+4], a[i+5]);
+    DATASKETCHES_CSA(twos_b, ones, ones, a[i+6], a[i+7]);
+    DATASKETCHES_CSA(fours_b, twos, twos, twos_a, twos_b);
 
-    CSA(eights, fours, fours, fours_a, fours_b);
+    DATASKETCHES_CSA(eights, fours, fours, fours_a, fours_b);
 
     total += warren_bit_count(eights);
   }
   total = 8 * total + 4 * warren_bit_count(fours) + 2 * warren_bit_count(twos) + warren_bit_count(ones);
 
   // Because I still don't fully trust this fancy version
   // assert(total == wegner_count_bits_set_in_matrix(A, length));
   //if (total != wegner_count_bits_set_in_matrix(a, length)) throw std::logic_error("count_bits_set_in_matrix error");
 
   return total;
 }
 
+#undef DATASKETCHES_CSA
+
 // Here are some timings made with quickTestMerge.c
 // for the "5 5" case:
 
 // Wegner CountBitsTime 29.3
 // Warren CountBitsTime  5.3
 // CSA    CountBitsTime  4.3
```

### Comparing `datasketches-4.0.1/cpc/include/icon_estimator.hpp` & `datasketches-4.1.0/cpc/include/icon_estimator.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/kxp_byte_lookup.hpp` & `datasketches-4.1.0/cpc/include/kxp_byte_lookup.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/u32_table.hpp` & `datasketches-4.1.0/cpc/include/u32_table.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/include/u32_table_impl.hpp` & `datasketches-4.1.0/cpc/include/u32_table_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/test/CMakeLists.txt` & `datasketches-4.1.0/cpc/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/test/compression_test.cpp` & `datasketches-4.1.0/cpc/test/compression_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/test/cpc_sketch_allocation_test.cpp` & `datasketches-4.1.0/cpc/test/cpc_sketch_allocation_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/test/cpc_sketch_test.cpp` & `datasketches-4.1.0/cpc/test/cpc_sketch_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/cpc/test/cpc_union_test.cpp` & `datasketches-4.1.0/cpc/test/cpc_union_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/CMakeLists.txt` & `datasketches-4.1.0/fi/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/include/frequent_items_sketch.hpp` & `datasketches-4.1.0/fi/include/frequent_items_sketch.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/include/frequent_items_sketch_impl.hpp` & `datasketches-4.1.0/fi/include/frequent_items_sketch_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/include/reverse_purge_hash_map.hpp` & `datasketches-4.1.0/fi/include/reverse_purge_hash_map.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -87,32 +87,38 @@
   V resize_or_purge_if_needed();
   void resize(uint8_t lg_new_size);
   V purge();
 };
 
 // This iterator uses strides based on golden ratio to avoid clustering during merge
 template<typename K, typename V, typename H, typename E, typename A>
-class reverse_purge_hash_map<K, V, H, E, A>::iterator: public std::iterator<std::input_iterator_tag, K> {
+class reverse_purge_hash_map<K, V, H, E, A>::iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = std::pair<K&, V>;
+  using difference_type = void;
+  using pointer = void;
+  using reference = const value_type;
+
   friend class reverse_purge_hash_map<K, V, H, E, A>;
   iterator& operator++() {
     ++count;
     if (count < map->num_active_) {
       const uint32_t mask = (1 << map->lg_cur_size_) - 1;
       do {
         index = (index + stride) & mask;
       } while (!map->is_active(index));
     }
     return *this;
   }
   iterator operator++(int) { iterator tmp(*this); operator++(); return tmp; }
   bool operator==(const iterator& rhs) const { return count == rhs.count; }
   bool operator!=(const iterator& rhs) const { return count != rhs.count; }
-  const std::pair<K&, V> operator*() const {
-    return std::pair<K&, V>(map->keys_[index], map->values_[index]);
+  reference operator*() const {
+    return value_type(map->keys_[index], map->values_[index]);
   }
 private:
   static constexpr double GOLDEN_RATIO_RECIPROCAL = 0.6180339887498949; // = (sqrt(5) - 1) / 2
   const reverse_purge_hash_map<K, V, H, E, A>* map;
   uint32_t index;
   uint32_t count;
   uint32_t stride;
```

### Comparing `datasketches-4.0.1/fi/include/reverse_purge_hash_map_impl.hpp` & `datasketches-4.1.0/fi/include/reverse_purge_hash_map_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/test/CMakeLists.txt` & `datasketches-4.1.0/fi/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/test/frequent_items_sketch_custom_type_test.cpp` & `datasketches-4.1.0/fi/test/frequent_items_sketch_custom_type_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/test/frequent_items_sketch_test.cpp` & `datasketches-4.1.0/fi/test/frequent_items_sketch_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/fi/test/reverse_purge_hash_map_test.cpp` & `datasketches-4.1.0/fi/test/reverse_purge_hash_map_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/CMakeLists.txt` & `datasketches-4.1.0/hll/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/AuxHashMap-internal.hpp` & `datasketches-4.1.0/hll/include/AuxHashMap-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/AuxHashMap.hpp` & `datasketches-4.1.0/hll/include/AuxHashMap.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CompositeInterpolationXTable-internal.hpp` & `datasketches-4.1.0/hll/include/CompositeInterpolationXTable-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CompositeInterpolationXTable.hpp` & `datasketches-4.1.0/hll/include/CompositeInterpolationXTable.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CouponHashSet-internal.hpp` & `datasketches-4.1.0/hll/include/CouponHashSet-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CouponHashSet.hpp` & `datasketches-4.1.0/hll/include/CouponHashSet.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CouponList-internal.hpp` & `datasketches-4.1.0/hll/include/CouponList-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CouponList.hpp` & `datasketches-4.1.0/hll/include/CouponList.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CubicInterpolation-internal.hpp` & `datasketches-4.1.0/hll/include/CubicInterpolation-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/CubicInterpolation.hpp` & `datasketches-4.1.0/hll/include/CubicInterpolation.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/HarmonicNumbers-internal.hpp` & `datasketches-4.1.0/hll/include/HarmonicNumbers-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/HarmonicNumbers.hpp` & `datasketches-4.1.0/hll/include/HarmonicNumbers.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/Hll4Array-internal.hpp` & `datasketches-4.1.0/hll/include/Hll4Array-internal.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,30 @@
     auxHashMap_ = that.auxHashMap_->copy();
   } else {
     auxHashMap_ = nullptr;
   }
 }
 
 template<typename A>
+Hll4Array<A>::Hll4Array(const HllArray<A>& other) :
+  HllArray<A>(other.getLgConfigK(), target_hll_type::HLL_4, other.isStartFullSize(), other.getAllocator()),
+  auxHashMap_(nullptr)
+{
+  const int numBytes = this->hll4ArrBytes(this->lgConfigK_);
+  this->hllByteArr_.resize(numBytes, 0);
+  this->oooFlag_ = other.isOutOfOrderFlag();
+
+  for (const auto coupon : other) { // all = false, so skip empty values
+    internalCouponUpdate(coupon); // updates KxQ registers
+  }
+  this->hipAccum_ = other.getHipAccum();
+  this->rebuild_kxq_curmin_ = false;
+}
+
+template<typename A>
 Hll4Array<A>::~Hll4Array() {
   // hllByteArr deleted in parent
   if (auxHashMap_ != nullptr) {
     AuxHashMap<A>::make_deleter()(auxHashMap_);
   }
 }
 
@@ -110,18 +126,17 @@
   if ((slotNo & 1) > 0) { // odd?
     return byte >> 4;
   }
   return byte & hll_constants::loNibbleMask;
 }
 
 template<typename A>
-uint8_t Hll4Array<A>::get_value(uint32_t index) const {
-  const uint8_t value = getSlot(index);
+uint8_t Hll4Array<A>::adjustRawValue(uint32_t slot, uint8_t value) const {
   if (value != hll_constants::AUX_TOKEN) return value + this->curMin_;
-  return auxHashMap_->mustFindValueFor(index);
+  return auxHashMap_->mustFindValueFor(slot);
 }
 
 template<typename A>
 HllSketchImpl<A>* Hll4Array<A>::couponUpdate(uint32_t coupon) {
   internalCouponUpdate(coupon);
   return this;
 }
@@ -206,15 +221,15 @@
           // We just overwrite the 4-bit array with the shifted new value.
           putSlot(slotNo, shiftedNewValue);
         }
       }
 
       // we just increased a pair value, so it might be time to change curMin
       if (actualOldValue == this->curMin_) { // 908
-        this->decNumAtCurMin();
+        --(this->numAtCurMin_);
         while (this->numAtCurMin_ == 0) {
           shiftToBiggerCurMin(); // increases curMin by 1, builds a new aux table
           // shifts values in 4-bit table and recounts curMin
         }
       }
     } // end newVal <= actualOldValue
   } // end newValue <= lbOnOldValue -> return, no need to update array
@@ -324,17 +339,10 @@
 
 template<typename A>
 typename HllArray<A>::const_iterator Hll4Array<A>::end() const {
   return typename HllArray<A>::const_iterator(this->hllByteArr_.data(), 1 << this->lgConfigK_, 1 << this->lgConfigK_,
       this->tgtHllType_, auxHashMap_, this->curMin_, false);
 }
 
-template<typename A>
-void Hll4Array<A>::mergeHll(const HllArray<A>& src) {
-  for (const auto coupon: src) {
-    internalCouponUpdate(coupon);
-  }
-}
-
 }
 
 #endif // _HLL4ARRAY_INTERNAL_HPP_
```

### Comparing `datasketches-4.0.1/hll/include/Hll4Array.hpp` & `datasketches-4.1.0/hll/include/Hll4Array.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -22,36 +22,33 @@
 
 #include "AuxHashMap.hpp"
 #include "HllArray.hpp"
 
 namespace datasketches {
 
 template<typename A>
-class Hll4Iterator;
-
-template<typename A>
 class Hll4Array final : public HllArray<A> {
   public:
     explicit Hll4Array(uint8_t lgConfigK, bool startFullSize, const A& allocator);
     explicit Hll4Array(const Hll4Array<A>& that);
+    explicit Hll4Array(const HllArray<A>& that);
 
     virtual ~Hll4Array();
     virtual std::function<void(HllSketchImpl<A>*)> get_deleter() const;
 
     virtual Hll4Array* copy() const;
 
     inline uint8_t getSlot(uint32_t slotNo) const;
     inline void putSlot(uint32_t slotNo, uint8_t value);
-    inline uint8_t get_value(uint32_t index) const;
+    inline uint8_t adjustRawValue(uint32_t index, uint8_t value) const;
 
     virtual uint32_t getUpdatableSerializationBytes() const;
     virtual uint32_t getHllByteArrBytes() const;
 
     virtual HllSketchImpl<A>* couponUpdate(uint32_t coupon) final;
-    void mergeHll(const HllArray<A>& src);
 
     virtual AuxHashMap<A>* getAuxHashMap() const;
     // does *not* delete old map if overwriting
     void putAuxHashMap(AuxHashMap<A>* auxHashMap);
 
     virtual typename HllArray<A>::const_iterator begin(bool all = false) const;
     virtual typename HllArray<A>::const_iterator end() const;
```

### Comparing `datasketches-4.0.1/hll/include/Hll6Array-internal.hpp` & `datasketches-4.1.0/hll/include/Hll6Array-internal.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -31,14 +31,33 @@
 HllArray<A>(lgConfigK, target_hll_type::HLL_6, startFullSize, allocator)
 {
   const int numBytes = this->hll6ArrBytes(lgConfigK);
   this->hllByteArr_.resize(numBytes, 0);
 }
 
 template<typename A>
+Hll6Array<A>::Hll6Array(const HllArray<A>& other) :
+  HllArray<A>(other.getLgConfigK(), target_hll_type::HLL_6, other.isStartFullSize(), other.getAllocator())
+{
+  const int numBytes = this->hll6ArrBytes(this->lgConfigK_);
+  this->hllByteArr_.resize(numBytes, 0);
+  this->oooFlag_ = other.isOutOfOrderFlag();
+  uint32_t num_zeros = 1 << this->lgConfigK_;
+  
+  for (const auto coupon : other) { // all = false, so skip empty values
+    num_zeros--;
+    internalCouponUpdate(coupon); // updates KxQ registers
+  }
+  
+  this->numAtCurMin_ = num_zeros;
+  this->hipAccum_ = other.getHipAccum();
+  this->rebuild_kxq_curmin_ = false;
+}
+
+template<typename A>
 std::function<void(HllSketchImpl<A>*)> Hll6Array<A>::get_deleter() const {
   return [](HllSketchImpl<A>* ptr) {
     using Hll6Alloc = typename std::allocator_traits<A>::template rebind_alloc<Hll6Array<A>>;
     Hll6Array<A>* hll = static_cast<Hll6Array<A>*>(ptr);
     Hll6Alloc hll6Alloc(hll->getAllocator());
     hll->~Hll6Array();
     hll6Alloc.deallocate(hll, 1);
@@ -97,17 +116,10 @@
     this->hipAndKxQIncrementalUpdate(curVal, newVal);
     if (curVal == 0) {
       this->numAtCurMin_--; // interpret numAtCurMin as num zeros
     }
   }
 }
 
-template<typename A>
-void Hll6Array<A>::mergeHll(const HllArray<A>& src) {
-  for (const auto coupon: src) {
-    internalCouponUpdate(coupon);
-  }
-}
-
 }
 
 #endif // _HLL6ARRAY_INTERNAL_HPP_
```

### Comparing `datasketches-4.0.1/hll/include/Hll6Array.hpp` & `datasketches-4.1.0/hll/include/Hll6Array.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 template<typename A>
 class Hll6Iterator;
 
 template<typename A>
 class Hll6Array final : public HllArray<A> {
   public:
     Hll6Array(uint8_t lgConfigK, bool startFullSize, const A& allocator);
+    explicit Hll6Array(const HllArray<A>& that);
 
     virtual ~Hll6Array() = default;
     virtual std::function<void(HllSketchImpl<A>*)> get_deleter() const;
 
     virtual Hll6Array* copy() const;
 
     inline uint8_t getSlot(uint32_t slotNo) const;
     inline void putSlot(uint32_t slotNo, uint8_t value);
 
     virtual HllSketchImpl<A>* couponUpdate(uint32_t coupon) final;
-    void mergeHll(const HllArray<A>& src);
 
     virtual uint32_t getHllByteArrBytes() const;
 
   private:
     void internalCouponUpdate(uint32_t coupon);
 };
```

### Comparing `datasketches-4.0.1/hll/include/Hll8Array.hpp` & `datasketches-4.1.0/hll/include/Hll8Array.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 template<typename A>
 class Hll8Iterator;
 
 template<typename A>
 class Hll8Array final : public HllArray<A> {
   public:
     Hll8Array(uint8_t lgConfigK, bool startFullSize, const A& allocator);
+    explicit Hll8Array(const HllArray<A>& that);
 
     virtual ~Hll8Array() = default;
     virtual std::function<void(HllSketchImpl<A>*)> get_deleter() const;
 
     virtual Hll8Array<A>* copy() const;
 
     inline uint8_t getSlot(uint32_t slotNo) const;
@@ -44,12 +45,13 @@
     void mergeList(const CouponList<A>& src);
     void mergeHll(const HllArray<A>& src);
 
     virtual uint32_t getHllByteArrBytes() const;
 
   private:
     inline void internalCouponUpdate(uint32_t coupon);
+    inline void processValue(uint32_t slot, uint32_t mask, uint8_t new_val);
 };
 
 }
 
 #endif /* _HLL8ARRAY_HPP_ */
```

### Comparing `datasketches-4.0.1/hll/include/HllArray-internal.hpp` & `datasketches-4.1.0/hll/include/HllArray-internal.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -39,28 +39,52 @@
 HllSketchImpl<A>(lgConfigK, tgtHllType, hll_mode::HLL, startFullSize),
 hipAccum_(0.0),
 kxq0_(1 << lgConfigK),
 kxq1_(0.0),
 hllByteArr_(allocator),
 curMin_(0),
 numAtCurMin_(1 << lgConfigK),
-oooFlag_(false)
+oooFlag_(false),
+rebuild_kxq_curmin_(false)
+{}
+
+template<typename A>
+HllArray<A>::HllArray(const HllArray& other, target_hll_type tgtHllType) :
+  HllSketchImpl<A>(other.getLgConfigK(), tgtHllType, hll_mode::HLL, other.isStartFullSize()),
+  // remaining fields are initialized to empty sketch defaults
+  // and left to subclass constructor to populate
+  hipAccum_(0.0),
+  kxq0_(1 << other.getLgConfigK()),
+  kxq1_(0.0),
+  hllByteArr_(other.getAllocator()),
+  curMin_(0),
+  numAtCurMin_(1 << other.getLgConfigK()),
+  oooFlag_(false),
+  rebuild_kxq_curmin_(false)
 {}
 
 template<typename A>
 HllArray<A>* HllArray<A>::copyAs(target_hll_type tgtHllType) const {
-  if (tgtHllType == this->getTgtHllType()) {
+  // we may need to recompute KxQ and curMin data for a union gadget,
+  // so only use a direct copy if we have a valid sketch
+  if (tgtHllType == this->getTgtHllType() && !this->isRebuildKxqCurminFlag()) {
     return static_cast<HllArray*>(copy());
   }
-  if (tgtHllType == target_hll_type::HLL_4) {
-    return HllSketchImplFactory<A>::convertToHll4(*this);
-  } else if (tgtHllType == target_hll_type::HLL_6) {
-    return HllSketchImplFactory<A>::convertToHll6(*this);
-  } else { // tgtHllType == HLL_8
-    return HllSketchImplFactory<A>::convertToHll8(*this);
+  
+  // the factory methods replay the coupons and will always rebuild
+  // the sketch in a consistent way
+  switch (tgtHllType) {
+    case target_hll_type::HLL_4:
+      return HllSketchImplFactory<A>::convertToHll4(*this);
+    case target_hll_type::HLL_6:
+      return HllSketchImplFactory<A>::convertToHll6(*this);
+    case target_hll_type::HLL_8:
+      return HllSketchImplFactory<A>::convertToHll8(*this);
+    default:
+      throw std::invalid_argument("Invalid target HLL type"); 
   }
 }
 
 template<typename A>
 HllArray<A>* HllArray<A>::newHll(const void* bytes, size_t len, const A& allocator) {
   if (len < hll_constants::HLL_BYTE_ARR_START) {
     throw std::out_of_range("Input data length insufficient to hold HLL array");
@@ -295,15 +319,15 @@
 }
 
 template<typename A>
 double HllArray<A>::getEstimate() const {
   if (oooFlag_) {
     return getCompositeEstimate();
   }
-  return getHipAccum();
+  return hipAccum_;
 }
 
 // HLL UPPER AND LOWER BOUNDS
 
 /*
  * The upper and lower bounds are not symmetric and thus are treated slightly differently.
  * For the lower bound, when the unique count is <= k, LB >= numNonZeros, where
@@ -318,62 +342,28 @@
  * the very small values <= k where curMin = 0 still apply.
  */
 template<typename A>
 double HllArray<A>::getLowerBound(uint8_t numStdDev) const {
   HllUtil<A>::checkNumStdDev(numStdDev);
   const uint32_t configK = 1 << this->lgConfigK_;
   const double numNonZeros = ((curMin_ == 0) ? (configK - numAtCurMin_) : configK);
-
-  double estimate;
-  double rseFactor;
-  if (oooFlag_) {
-    estimate = getCompositeEstimate();
-    rseFactor = hll_constants::HLL_NON_HIP_RSE_FACTOR;
-  } else {
-    estimate = hipAccum_;
-    rseFactor = hll_constants::HLL_HIP_RSE_FACTOR;
-  }
-
-  double relErr;
-  if (this->lgConfigK_ > 12) {
-    relErr = (numStdDev * rseFactor) / sqrt(configK);
-  } else {
-    relErr = HllUtil<A>::getRelErr(false, oooFlag_, this->lgConfigK_, numStdDev);
-  }
-  return fmax(estimate / (1.0 + relErr), numNonZeros);
+  const double relErr = HllUtil<A>::getRelErr(false, this->oooFlag_, this->lgConfigK_, numStdDev);
+  return fmax(getEstimate() / (1.0 + relErr), numNonZeros);
 }
 
 template<typename A>
 double HllArray<A>::getUpperBound(uint8_t numStdDev) const {
   HllUtil<A>::checkNumStdDev(numStdDev);
-  const uint32_t configK = 1 << this->lgConfigK_;
-
-  double estimate;
-  double rseFactor;
-  if (oooFlag_) {
-    estimate = getCompositeEstimate();
-    rseFactor = hll_constants::HLL_NON_HIP_RSE_FACTOR;
-  } else {
-    estimate = hipAccum_;
-    rseFactor = hll_constants::HLL_HIP_RSE_FACTOR;
-  }
-
-  double relErr;
-  if (this->lgConfigK_ > 12) {
-    relErr = (-1.0) * (numStdDev * rseFactor) / sqrt(configK);
-  } else {
-    relErr = HllUtil<A>::getRelErr(true, oooFlag_, this->lgConfigK_, numStdDev);
-  }
-  return estimate / (1.0 + relErr);
+  const double relErr = HllUtil<A>::getRelErr(true, this->oooFlag_, this->lgConfigK_, numStdDev);
+  return getEstimate() / (1.0 + relErr);
 }
 
 /**
  * This is the (non-HIP) estimator.
  * It is called "composite" because multiple estimators are pasted together.
- * @param absHllArr an instance of the AbstractHllArray class.
  * @return the composite estimate
  */
 // Original C: again-two-registers.c hhb_get_composite_estimate L1489
 template<typename A>
 double HllArray<A>::getCompositeEstimate() const {
   const double rawEst = getHllRawEstimate();
 
@@ -465,32 +455,22 @@
 
 template<typename A>
 void HllArray<A>::putNumAtCurMin(uint32_t numAtCurMin) {
   numAtCurMin_ = numAtCurMin;
 }
 
 template<typename A>
-void HllArray<A>::decNumAtCurMin() {
-  --numAtCurMin_;
-}
-
-template<typename A>
-void HllArray<A>::addToHipAccum(double delta) {
-  hipAccum_ += delta;
-}
-
-template<typename A>
 bool HllArray<A>::isCompact() const {
   return false;
 }
 
 template<typename A>
 bool HllArray<A>::isEmpty() const {
   const uint32_t configK = 1 << this->lgConfigK_;
-  return (getCurMin() == 0) && (getNumAtCurMin() == configK);
+  return (curMin_ == 0) && (numAtCurMin_ == configK);
 }
 
 template<typename A>
 void HllArray<A>::putOutOfOrderFlag(bool flag) {
   oooFlag_ = flag;
 }
 
@@ -553,14 +533,19 @@
 
 template<typename A>
 AuxHashMap<A>* HllArray<A>::getAuxHashMap() const {
   return nullptr;
 }
 
 template<typename A>
+const vector_u8<A>& HllArray<A>::getHllArray() const {
+  return hllByteArr_;
+}
+
+template<typename A>
 void HllArray<A>::hipAndKxQIncrementalUpdate(uint8_t oldValue, uint8_t newValue) {
   const uint32_t configK = 1 << this->getLgConfigK();
   // update hip BEFORE updating kxq
   if (!oooFlag_) hipAccum_ += configK / (kxq0_ + kxq1_);
   // update kxq0 and kxq1; subtract first, then add
   if (oldValue < 32) { kxq0_ -= INVERSE_POWERS_OF_2[oldValue]; }
   else               { kxq1_ -= INVERSE_POWERS_OF_2[oldValue]; }
@@ -598,14 +583,60 @@
   else if (this->lgConfigK_ == 6) { correctionFactor = 0.709; }
   else { correctionFactor = 0.7213 / (1.0 + (1.079 / configK)); }
   const double hyperEst = (correctionFactor * configK * configK) / (kxq0_ + kxq1_);
   return hyperEst;
 }
 
 template<typename A>
+void HllArray<A>::setRebuildKxqCurminFlag(bool rebuild) {
+  rebuild_kxq_curmin_ = rebuild;
+}
+
+template<typename A>
+bool HllArray<A>::isRebuildKxqCurminFlag() const {
+  return rebuild_kxq_curmin_;
+}
+
+template<typename A>
+void HllArray<A>::check_rebuild_kxq_cur_min() {
+  if (!rebuild_kxq_curmin_) { return; }
+
+  uint8_t cur_min = 64;
+  uint32_t num_at_cur_min = 0;
+  double kxq0 = 1 << this->lgConfigK_;
+  double kxq1 = 0;
+
+  auto it = this->begin(true); // want all points to adjust cur_min
+  const auto end = this->end();
+  while (it != end) {
+    uint8_t v = HllUtil<A>::getValue(*it);
+    if (v > 0) {
+      if (v < 32) { kxq0 += INVERSE_POWERS_OF_2[v] - 1.0; }
+      else        { kxq1 += INVERSE_POWERS_OF_2[v] - 1.0; }
+    }
+    if (v > cur_min) { ++it; continue; }
+    if (v < cur_min) {
+      cur_min = v;
+      num_at_cur_min = 1;
+    } else {
+      ++num_at_cur_min;
+    }    
+    ++it;
+  }
+
+  kxq0_ = kxq0;
+  kxq1_ = kxq1;
+  curMin_ = cur_min;
+  numAtCurMin_ = num_at_cur_min;
+  rebuild_kxq_curmin_ = false;
+  // HipAccum is not affected
+
+}
+
+template<typename A>
 typename HllArray<A>::const_iterator HllArray<A>::begin(bool all) const {
   return const_iterator(hllByteArr_.data(), 1 << this->lgConfigK_, 0, this->tgtHllType_, nullptr, 0, all);
 }
 
 template<typename A>
 typename HllArray<A>::const_iterator HllArray<A>::end() const {
   return const_iterator(hllByteArr_.data(), 1 << this->lgConfigK_, 1 << this->lgConfigK_, this->tgtHllType_, nullptr, 0, false);
@@ -633,20 +664,22 @@
 
 template<typename A>
 bool HllArray<A>::const_iterator::operator!=(const const_iterator& other) const {
   return index_ != other.index_;
 }
 
 template<typename A>
-uint32_t HllArray<A>::const_iterator::operator*() const {
+auto HllArray<A>::const_iterator::operator*() const -> reference {
   return HllUtil<A>::pair(index_, value_);
 }
 
 template<typename A>
 uint8_t HllArray<A>::const_iterator::get_value(const uint8_t* array, uint32_t index, target_hll_type hll_type, const AuxHashMap<A>* exceptions, uint8_t offset) {
+  // TODO: we should be able to improve efficiency here by reading multiple bytes at a time
+  //       for HLL4 and HLL6
   if (hll_type == target_hll_type::HLL_4) {
     uint8_t value = array[index >> 1];
     if ((index & 1) > 0) { // odd
         value >>= 4;
     } else {
       value &= hll_constants::loNibbleMask;
     }
```

### Comparing `datasketches-4.0.1/hll/include/HllArray.hpp` & `datasketches-4.1.0/hll/include/HllArray.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 template<typename A>
 class AuxHashMap;
 
 template<typename A>
 class HllArray : public HllSketchImpl<A> {
   public:
     HllArray(uint8_t lgConfigK, target_hll_type tgtHllType, bool startFullSize, const A& allocator);
+    explicit HllArray(const HllArray& other, target_hll_type tgtHllType);
 
     static HllArray* newHll(const void* bytes, size_t len, const A& allocator);
     static HllArray* newHll(std::istream& is, const A& allocator);
 
     virtual vector_u8<A> serialize(bool compact, unsigned header_size_bytes) const;
     virtual void serialize(std::ostream& os, bool compact) const;
 
@@ -48,18 +49,14 @@
     virtual HllSketchImpl<A>* couponUpdate(uint32_t coupon) = 0;
 
     virtual double getEstimate() const;
     virtual double getCompositeEstimate() const;
     virtual double getLowerBound(uint8_t numStdDev) const;
     virtual double getUpperBound(uint8_t numStdDev) const;
 
-    inline void addToHipAccum(double delta);
-
-    inline void decNumAtCurMin();
-
     inline uint8_t getCurMin() const;
     inline uint32_t getNumAtCurMin() const;
     inline double getHipAccum() const;
 
     virtual uint32_t getHllByteArrBytes() const = 0;
 
     virtual uint32_t getUpdatableSerializationBytes() const;
@@ -86,43 +83,56 @@
     static uint32_t hllArrBytes(target_hll_type tgtHllType, uint8_t lgConfigK);
     static uint32_t hll4ArrBytes(uint8_t lgConfigK);
     static uint32_t hll6ArrBytes(uint8_t lgConfigK);
     static uint32_t hll8ArrBytes(uint8_t lgConfigK);
 
     virtual AuxHashMap<A>* getAuxHashMap() const;
 
+    void setRebuildKxqCurminFlag(bool rebuild);
+    bool isRebuildKxqCurminFlag() const;
+    void check_rebuild_kxq_cur_min();
+
     class const_iterator;
     virtual const_iterator begin(bool all = false) const;
     virtual const_iterator end() const;
 
     virtual A getAllocator() const;
 
+    const vector_u8<A>& getHllArray() const;
+
   protected:
     void hipAndKxQIncrementalUpdate(uint8_t oldValue, uint8_t newValue);
     double getHllBitMapEstimate() const;
     double getHllRawEstimate() const;
 
     double hipAccum_;
     double kxq0_;
     double kxq1_;
     vector_u8<A> hllByteArr_; //init by sub-classes
     uint8_t curMin_; //always zero for Hll6 and Hll8, only tracked by Hll4Array
     uint32_t numAtCurMin_; //interpreted as num zeros when curMin == 0
     bool oooFlag_; //Out-Of-Order Flag
+    bool rebuild_kxq_curmin_; // flag to recompute
 
     friend class HllSketchImplFactory<A>;
 };
 
 template<typename A>
-class HllArray<A>::const_iterator: public std::iterator<std::input_iterator_tag, uint32_t> {
+class HllArray<A>::const_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = uint32_t;
+  using difference_type = void;
+  using pointer = uint32_t*;
+  using reference = uint32_t;
+
   const_iterator(const uint8_t* array, uint32_t array_slze, uint32_t index, target_hll_type hll_type, const AuxHashMap<A>* exceptions, uint8_t offset, bool all);
   const_iterator& operator++();
   bool operator!=(const const_iterator& other) const;
-  uint32_t operator*() const;
+  reference operator*() const;
 private:
   const uint8_t* array_;
   uint32_t array_size_;
   uint32_t index_;
   target_hll_type hll_type_;
   const AuxHashMap<A>* exceptions_;
   uint8_t offset_;
```

### Comparing `datasketches-4.0.1/hll/include/HllSketch-internal.hpp` & `datasketches-4.1.0/hll/include/HllSketch-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/HllSketchImpl-internal.hpp` & `datasketches-4.1.0/hll/include/HllSketchImpl-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/HllSketchImpl.hpp` & `datasketches-4.1.0/hll/include/HllSketchImpl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/HllSketchImplFactory.hpp` & `datasketches-4.1.0/hll/include/HllSketchImplFactory.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -132,44 +132,26 @@
     impl->get_deleter()(impl);
     return cl;
   }
 }
 
 template<typename A>
 Hll4Array<A>* HllSketchImplFactory<A>::convertToHll4(const HllArray<A>& srcHllArr) {
-  const uint8_t lgConfigK = srcHllArr.getLgConfigK();
   using Hll4Alloc = typename std::allocator_traits<A>::template rebind_alloc<Hll4Array<A>>;
-  Hll4Array<A>* hll4Array = new (Hll4Alloc(srcHllArr.getAllocator()).allocate(1))
-      Hll4Array<A>(lgConfigK, srcHllArr.isStartFullSize(), srcHllArr.getAllocator());
-  hll4Array->putOutOfOrderFlag(srcHllArr.isOutOfOrderFlag());
-  hll4Array->mergeHll(srcHllArr);
-  hll4Array->putHipAccum(srcHllArr.getHipAccum());
-  return hll4Array;
+  return new (Hll4Alloc(srcHllArr.getAllocator()).allocate(1)) Hll4Array<A>(srcHllArr);
 }
 
 template<typename A>
 Hll6Array<A>* HllSketchImplFactory<A>::convertToHll6(const HllArray<A>& srcHllArr) {
-  const uint8_t lgConfigK = srcHllArr.getLgConfigK();
   using Hll6Alloc = typename std::allocator_traits<A>::template rebind_alloc<Hll6Array<A>>;
-  Hll6Array<A>* hll6Array = new (Hll6Alloc(srcHllArr.getAllocator()).allocate(1))
-      Hll6Array<A>(lgConfigK, srcHllArr.isStartFullSize(), srcHllArr.getAllocator());
-  hll6Array->putOutOfOrderFlag(srcHllArr.isOutOfOrderFlag());
-  hll6Array->mergeHll(srcHllArr);
-  hll6Array->putHipAccum(srcHllArr.getHipAccum());
-  return hll6Array;
+  return new (Hll6Alloc(srcHllArr.getAllocator()).allocate(1)) Hll6Array<A>(srcHllArr);
 }
 
 template<typename A>
 Hll8Array<A>* HllSketchImplFactory<A>::convertToHll8(const HllArray<A>& srcHllArr) {
-  const uint8_t lgConfigK = srcHllArr.getLgConfigK();
   using Hll8Alloc = typename std::allocator_traits<A>::template rebind_alloc<Hll8Array<A>>;
-  Hll8Array<A>* hll8Array = new (Hll8Alloc(srcHllArr.getAllocator()).allocate(1))
-      Hll8Array<A>(lgConfigK, srcHllArr.isStartFullSize(), srcHllArr.getAllocator());
-  hll8Array->putOutOfOrderFlag(srcHllArr.isOutOfOrderFlag());
-  hll8Array->mergeHll(srcHllArr);
-  hll8Array->putHipAccum(srcHllArr.getHipAccum());
-  return hll8Array;
+  return new (Hll8Alloc(srcHllArr.getAllocator()).allocate(1)) Hll8Array<A>(srcHllArr);
 }
 
 }
 
 #endif /* _HLLSKETCHIMPLFACTORY_HPP_ */
```

### Comparing `datasketches-4.0.1/hll/include/HllUnion-internal.hpp` & `datasketches-4.1.0/hll/include/HllUnion-internal.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -127,29 +127,37 @@
     if (gadget_.sketch_impl != nullptr) { gadget_.sketch_impl->get_deleter()(gadget_.sketch_impl); }
     gadget_.sketch_impl = result;
   }
 }
 
 template<typename A>
 double hll_union_alloc<A>::get_estimate() const {
+  if (gadget_.sketch_impl->getCurMode() == hll_mode::HLL)
+    static_cast<HllArray<A>*>(gadget_.sketch_impl)->check_rebuild_kxq_cur_min();
   return gadget_.get_estimate();
 }
 
 template<typename A>
 double hll_union_alloc<A>::get_composite_estimate() const {
+  if (gadget_.sketch_impl->getCurMode() == hll_mode::HLL)
+    static_cast<HllArray<A>*>(gadget_.sketch_impl)->check_rebuild_kxq_cur_min();
   return gadget_.get_composite_estimate();
 }
 
 template<typename A>
 double hll_union_alloc<A>::get_lower_bound(uint8_t num_std_dev) const {
+  if (gadget_.sketch_impl->getCurMode() == hll_mode::HLL)
+    static_cast<HllArray<A>*>(gadget_.sketch_impl)->check_rebuild_kxq_cur_min();
   return gadget_.get_lower_bound(num_std_dev);
 }
 
 template<typename A>
 double hll_union_alloc<A>::get_upper_bound(uint8_t num_std_dev) const {
+  if (gadget_.sketch_impl->getCurMode() == hll_mode::HLL)
+    static_cast<HllArray<A>*>(gadget_.sketch_impl)->check_rebuild_kxq_cur_min();
   return gadget_.get_upper_bound(num_std_dev);
 }
 
 template<typename A>
 uint8_t hll_union_alloc<A>::get_lg_config_k() const {
   return gadget_.get_lg_config_k();
 }
```

### Comparing `datasketches-4.0.1/hll/include/HllUtil.hpp` & `datasketches-4.1.0/hll/include/HllUtil.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -149,29 +149,37 @@
 
 template<typename A>
 inline void HllUtil<A>::hash(const void* key, size_t keyLen, uint64_t seed, HashState& result) {
   MurmurHash3_x64_128(key, keyLen, seed, result);
 }
 
 template<typename A>
-inline double HllUtil<A>::getRelErr(bool upperBound, bool unioned,
-                                    uint8_t lgConfigK, uint8_t numStdDev) {
-  return RelativeErrorTables<A>::getRelErr(upperBound, unioned, lgConfigK, numStdDev);
-}
-
-template<typename A>
 inline uint8_t HllUtil<A>::checkLgK(uint8_t lgK) {
   if ((lgK >= hll_constants::MIN_LOG_K) && (lgK <= hll_constants::MAX_LOG_K)) {
     return lgK;
   } else {
     throw std::invalid_argument("Invalid value of k: " + std::to_string(lgK));
   }
 }
 
 template<typename A>
+inline double HllUtil<A>::getRelErr(bool upperBound, bool unioned,
+                                    uint8_t lgConfigK, uint8_t numStdDev) {
+  checkLgK(lgConfigK);
+  if (lgConfigK > 12) {
+    const double rseFactor = unioned ?
+        hll_constants::HLL_NON_HIP_RSE_FACTOR : hll_constants::HLL_HIP_RSE_FACTOR;
+    const uint32_t configK = 1 << lgConfigK;
+    return (upperBound ? -1 : 1) * (numStdDev * rseFactor) / sqrt(configK);
+  } else {
+    return RelativeErrorTables<A>::getRelErr(upperBound, unioned, lgConfigK, numStdDev);
+  }
+}
+
+template<typename A>
 inline void HllUtil<A>::checkMemSize(uint64_t minBytes, uint64_t capBytes) {
   if (capBytes < minBytes) {
     throw std::invalid_argument("Given destination array is not large enough: " + std::to_string(capBytes));
   }
 }
 
 template<typename A>
```

### Comparing `datasketches-4.0.1/hll/include/RelativeErrorTables-internal.hpp` & `datasketches-4.1.0/hll/include/RelativeErrorTables-internal.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/RelativeErrorTables.hpp` & `datasketches-4.1.0/hll/include/RelativeErrorTables.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/include/coupon_iterator-internal.hpp` & `datasketches-4.1.0/hll/include/coupon_iterator-internal.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,14 @@
 
 template<typename A>
 bool coupon_iterator<A>::operator!=(const coupon_iterator& other) const {
   return index_ != other.index_;
 }
 
 template<typename A>
-uint32_t coupon_iterator<A>::operator*() const {
+auto coupon_iterator<A>::operator*() const -> reference {
   return array_[index_];
 }
 
 }
 
 #endif // _INTARRAYPAIRITERATOR_INTERNAL_HPP_
```

### Comparing `datasketches-4.0.1/hll/include/coupon_iterator.hpp` & `datasketches-4.1.0/hll/include/coupon_iterator.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,26 @@
 
 #ifndef _INTARRAYPAIRITERATOR_HPP_
 #define _INTARRAYPAIRITERATOR_HPP_
 
 namespace datasketches {
 
 template<typename A>
-class coupon_iterator: public std::iterator<std::input_iterator_tag, uint32_t> {
+class coupon_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = uint32_t;
+  using difference_type = void;
+  using pointer = uint32_t*;
+  using reference = uint32_t;
+
   coupon_iterator(const uint32_t* array, size_t array_slze, size_t index, bool all);
   coupon_iterator& operator++();
   bool operator!=(const coupon_iterator& other) const;
-  uint32_t operator*() const;
+  reference operator*() const;
 private:
   const uint32_t* array_;
   size_t array_size_;
   size_t index_;
   bool all_;
 };
```

### Comparing `datasketches-4.0.1/hll/include/hll.hpp` & `datasketches-4.1.0/hll/include/hll.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 
 #ifndef _HLL_HPP_
 #define _HLL_HPP_
 
 #include "common_defs.hpp"
 #include "HllUtil.hpp"
 
-#include <memory>
 #include <iostream>
+#include <memory>
+#include <string>
 #include <vector>
 
 namespace datasketches {
 
   /**
  * This is a high performance implementation of Phillipe Flajolet&#8217;s HLL sketch but with
  * significantly improved error behavior.  If the ONLY use case for sketching is counting
@@ -140,15 +141,15 @@
      * Reconstructs a sketch from a serialized image on a stream.
      * @param is An input stream with a binary image of a sketch
      */
     static hll_sketch_alloc deserialize(std::istream& is, const A& allocator = A());
 
     /**
      * Reconstructs a sketch from a serialized image in a byte array.
-     * @param is bytes An input array with a binary image of a sketch
+     * @param bytes An input array with a binary image of a sketch
      * @param len Length of the input array, in bytes
      */
     static hll_sketch_alloc deserialize(const void* bytes, size_t len, const A& allocator = A());
 
     //! Class destructor
     virtual ~hll_sketch_alloc();
 
@@ -193,15 +194,15 @@
      */
     void serialize_updatable(std::ostream& os) const;
 
     /**
      * Human readable summary with optional detail
      * @param summary if true, output the sketch summary
      * @param detail if true, output the internal data array
-     * @param auxDetail if true, output the internal Aux array, if it exists.
+     * @param aux_detail if true, output the internal Aux array, if it exists.
      * @param all if true, outputs all entries including empty ones
      * @return human readable string with optional detail.
      */
     string<A> to_string(bool summary = true,
                         bool detail = false,
                         bool aux_detail = false,
                         bool all = false) const;
@@ -354,15 +355,15 @@
 
     /**
      * Returns the maximum size in bytes that this sketch can grow to
      * given lg_config_k.  However, for the HLL_4 sketch type, this
      * value can be exceeded in extremely rare cases.  If exceeded, it
      * will be larger by only a few percent.
      *
-     * @param lg_config_k The Log2 of K for the target HLL sketch. This value must be
+     * @param lg_k The Log2 of K for the target HLL sketch. This value must be
      *        between 4 and 21 inclusively.
      * @param tgt_type the desired Hll type
      * @return the maximum size in bytes that this sketch can grow to.
      */
     static uint32_t get_max_updatable_serialization_bytes(uint8_t lg_k, target_hll_type tgt_type);
   
     /**
@@ -491,28 +492,28 @@
      * Does not re-use existing internal objects.
      */
     void reset();
 
     /**
      * Returns the result of this union operator with the specified
      * #tgt_hll_type.
-     * @param The tgt_hll_type enum value of the desired result (Default: HLL_4)
+     * @param tgt_type The tgt_hll_type enum value of the desired result (Default: HLL_4)
      * @return The result of this union with the specified tgt_hll_type
      */
     hll_sketch_alloc<A> get_result(target_hll_type tgt_type = HLL_4) const;
 
     /**
      * Update this union operator with the given sketch.
-     * @param The given sketch.
+     * @param sketch The given sketch.
      */
     void update(const hll_sketch_alloc<A>& sketch);
 
     /**
      * Update this union operator with the given temporary sketch.
-     * @param The given sketch.
+     * @param sketch The given sketch.
      */
     void update(hll_sketch_alloc<A>&& sketch);
   
     /**
      * Present the given std::string as a potential unique item.
      * The string is converted to a byte array using UTF8 encoding.
      * If the string is null or empty no update attempt is made and the method returns.
@@ -604,15 +605,15 @@
 
    /**
     * Union the given source and destination sketches. This method examines the state of
     * the current internal gadget and the incoming sketch and determines the optimal way to
     * perform the union. This may involve swapping, down-sampling, transforming, and / or
     * copying one of the arguments and may completely replace the internals of the union.
     *
-    * @param incoming_impl the given incoming sketch, which may not be modified.
+    * @param sketch the given incoming sketch, which may not be modified.
     * @param lg_max_k the maximum value of log2 K for this union.
     */
     inline void union_impl(const hll_sketch_alloc<A>& sketch, uint8_t lg_max_k);
 
     static HllSketchImpl<A>* copy_or_downsample(const HllSketchImpl<A>* src_impl, uint8_t tgt_lg_k);
 
     void coupon_update(uint32_t coupon);
```

### Comparing `datasketches-4.0.1/hll/include/hll.private.hpp` & `datasketches-4.1.0/hll/include/hll.private.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/AuxHashMapTest.cpp` & `datasketches-4.1.0/hll/test/AuxHashMapTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/CMakeLists.txt` & `datasketches-4.1.0/hll/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/CouponHashSetTest.cpp` & `datasketches-4.1.0/hll/test/CouponHashSetTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/CouponListTest.cpp` & `datasketches-4.1.0/hll/test/CouponListTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/CrossCountingTest.cpp` & `datasketches-4.1.0/hll/test/CrossCountingTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/HllArrayTest.cpp` & `datasketches-4.1.0/hll/test/HllArrayTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/HllSketchTest.cpp` & `datasketches-4.1.0/hll/test/HllSketchTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/HllUnionTest.cpp` & `datasketches-4.1.0/hll/test/HllUnionTest.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,24 @@
   for (uint64_t i = 0; i < n2; ++i) {
     h2.update(v + i);
     control.update(v + i);
   }
   v += n2;
 
   hll_union u(lgMaxK);
-  u.update(std::move(h1));
+  u.update(h1);
   u.update(h2);
 
   hll_sketch result = u.get_result(resultType);
 
+  // ensure we check a direct union estimate, without first caling get_result()
+  u.reset();
+  u.update(std::move(h1));
+  u.update(h2);
+
   // force non-HIP estimates to avoid issues with in- vs out-of-order
   double uEst = result.get_composite_estimate();
   double uUb = result.get_upper_bound(2);
   double uLb = result.get_lower_bound(2);
   //double rerr = ((uEst/tot) - 1.0) * 100;
 
   double controlEst = control.get_composite_estimate();
@@ -70,14 +75,15 @@
 
   REQUIRE((controlUb - controlEst) >= 0.0);
   REQUIRE((uUb - uEst) >= 0.0);
   REQUIRE((controlEst - controlLb) >= 0.0);
   REQUIRE((uEst - uLb) >= 0.0);
 
   REQUIRE(controlEst == uEst);
+  REQUIRE(controlEst == u.get_composite_estimate());
 }
 
 /**
  * The task here is to check the transition boundaries as the sketch morphs between LIST to
  * SET to HLL modes. The transition points vary as a function of lgConfigK. In addition,
  * this checks that the union operation is operating properly based on the order the
  * sketches are presented to the union.
```

### Comparing `datasketches-4.0.1/hll/test/IsomorphicTest.cpp` & `datasketches-4.1.0/hll/test/IsomorphicTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/TablesTest.cpp` & `datasketches-4.1.0/hll/test/TablesTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/hll/test/ToFromByteArrayTest.cpp` & `datasketches-4.1.0/hll/test/ToFromByteArrayTest.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/CMakeLists.txt` & `datasketches-4.1.0/kll/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/include/kll_helper.hpp` & `datasketches-4.1.0/kll/include/kll_helper.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
  * specific language governing permissions and limitations
  * under the License.
  */
 
 #ifndef KLL_HELPER_HPP_
 #define KLL_HELPER_HPP_
 
-#include <random>
 #include <stdexcept>
 
 namespace datasketches {
 
 #ifdef KLL_VALIDATION
 extern uint32_t kll_next_offset;
 #endif
```

### Comparing `datasketches-4.0.1/kll/include/kll_helper_impl.hpp` & `datasketches-4.1.0/kll/include/kll_helper_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/include/kll_sketch.hpp` & `datasketches-4.1.0/kll/include/kll_sketch.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -582,24 +582,29 @@
     template<typename TT, typename CC, typename AA> friend class kll_sketch;
 
     void setup_sorted_view() const; // modifies mutable state
     void reset_sorted_view();
 };
 
 template<typename T, typename C, typename A>
-class kll_sketch<T, C, A>::const_iterator: public std::iterator<std::input_iterator_tag, T> {
+class kll_sketch<T, C, A>::const_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
   using value_type = std::pair<const T&, const uint64_t>;
+  using difference_type = void;
+  using pointer = const return_value_holder<value_type>;
+  using reference = const value_type;
+
   friend class kll_sketch<T, C, A>;
   const_iterator& operator++();
   const_iterator& operator++(int);
   bool operator==(const const_iterator& other) const;
   bool operator!=(const const_iterator& other) const;
-  const value_type operator*() const;
-  const return_value_holder<value_type> operator->() const;
+  reference operator*() const;
+  pointer operator->() const;
 private:
   const T* items;
   const uint32_t* levels;
   const uint8_t num_levels;
   uint32_t index;
   uint8_t level;
   uint64_t weight;
```

### Comparing `datasketches-4.0.1/kll/include/kll_sketch_impl.hpp` & `datasketches-4.1.0/kll/include/kll_sketch_impl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1101,19 +1101,19 @@
 
 template<typename T, typename C, typename A>
 bool kll_sketch<T, C, A>::const_iterator::operator!=(const const_iterator& other) const {
   return !operator==(other);
 }
 
 template<typename T, typename C, typename A>
-auto kll_sketch<T, C, A>::const_iterator::operator*() const -> const value_type {
+auto kll_sketch<T, C, A>::const_iterator::operator*() const -> reference {
   return value_type(items[index], weight);
 }
 
 template<typename T, typename C, typename A>
-auto kll_sketch<T, C, A>::const_iterator::operator->() const -> const return_value_holder<value_type> {
+auto kll_sketch<T, C, A>::const_iterator::operator->() const -> pointer {
   return **this;
 }
 
 } /* namespace datasketches */
 
 #endif
```

### Comparing `datasketches-4.0.1/kll/test/CMakeLists.txt` & `datasketches-4.1.0/kll/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/test/kll_sketch_custom_type_test.cpp` & `datasketches-4.1.0/kll/test/kll_sketch_custom_type_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/test/kll_sketch_from_java.sk` & `datasketches-4.1.0/kll/test/kll_sketch_from_java.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/test/kll_sketch_test.cpp` & `datasketches-4.1.0/kll/test/kll_sketch_test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -238,30 +238,30 @@
 
       double subtotal_pmf = 0;
       for (int i = 0; i < n; i++) {
         if (sketch.get_rank(values[i], false) != ranks[i]) {
           FAIL("checking rank vs CDF for value " + std::to_string(i));
         }
         subtotal_pmf += pmf[i];
-        if (abs(ranks[i] - subtotal_pmf) > NUMERIC_NOISE_TOLERANCE) {
+        if (std::abs(ranks[i] - subtotal_pmf) > NUMERIC_NOISE_TOLERANCE) {
           FAIL("CDF vs PMF for value " + std::to_string(i));
         }
       }
     }
     {  // inclusive=true (default)
       const auto ranks(sketch.get_CDF(values, n));
       const auto pmf(sketch.get_PMF(values, n));
 
       double subtotal_pmf = 0;
       for (int i = 0; i < n; i++) {
         if (sketch.get_rank(values[i]) != ranks[i]) {
           FAIL("checking rank vs CDF for value " + std::to_string(i));
         }
         subtotal_pmf += pmf[i];
-        if (abs(ranks[i] - subtotal_pmf) > NUMERIC_NOISE_TOLERANCE) {
+        if (std::abs(ranks[i] - subtotal_pmf) > NUMERIC_NOISE_TOLERANCE) {
           FAIL("CDF vs PMF for value " + std::to_string(i));
         }
       }
     }
   }
 
   SECTION("deserialize from java") {
```

### Comparing `datasketches-4.0.1/kll/test/kll_sketch_validation.cpp` & `datasketches-4.1.0/kll/test/kll_sketch_validation.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/kll/test/kolmogorov_smirnov_test.cpp` & `datasketches-4.1.0/kll/test/kolmogorov_smirnov_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/pyproject.toml` & `datasketches-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/CMakeLists.txt` & `datasketches-4.1.0/python/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,17 +38,20 @@
   PRIVATE
     common
     hll
     kll
     cpc
     fi
     theta
+    tuple
     sampling
     req
     quantiles
+    count
+    density
     pybind11::module
 )
 
 set_target_properties(python PROPERTIES
   PREFIX ""
   OUTPUT_NAME _datasketches
 )
@@ -68,14 +71,17 @@
   PRIVATE
     src/datasketches.cpp
     src/hll_wrapper.cpp
     src/kll_wrapper.cpp
     src/cpc_wrapper.cpp
     src/fi_wrapper.cpp
     src/theta_wrapper.cpp
+    src/tuple_wrapper.cpp
     src/vo_wrapper.cpp
     src/req_wrapper.cpp
     src/quantiles_wrapper.cpp
+    src/density_wrapper.cpp
     src/ks_wrapper.cpp
+    src/count_wrapper.cpp
     src/vector_of_kll.cpp
     src/py_serde.cpp
 )
```

### Comparing `datasketches-4.0.1/python/README.md` & `datasketches-4.1.0/python/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 If approximate results are acceptable, there is a class of specialized algorithms, called streaming algorithms, or sketches that can produce results orders-of magnitude faster and with mathematically proven error bounds. For interactive queries there may not be other viable alternatives, and in the case of real-time analysis, sketches are the only known solution.
 
 This package provides a variety of sketches as described below. Wherever a specific type of sketch exists in Apache DataSketches packages for other languages, the sketches will be portable between languages (for platforms with the same endianness).
 
 ## Building and Installation
 
-Once cloned, the library can be installed by running `python3 -m pip install .` in the project root directory -- not the python subdirectory -- which will also install the necessary dependencies, namely numpy and [pybind11[global]](https://github.com/pybind/pybind11).
+Once cloned, the library can be installed by running `python3 -m pip install .` in the project root directory -- not the python subdirectory -- which will also install the necessary dependencies, namely NumPy and [pybind11[global]](https://github.com/pybind/pybind11).
 
-If you prefer to call the `setup.py` build script directly, which is discoraged, you must first install `pybind11[global]`, as well as any other dependencies listed under the build-system section in `pyproject.toml`.
+If you prefer to call the `setup.py` build script directly, which is discouraged, you must first install `pybind11[global]`, as well as any other dependencies listed under the build-system section in `pyproject.toml`.
 
 The library is also available from PyPI via `python3 -m pip install datasketches`.
 
 ## Usage
 
-Having installed the library, loading the Apache Datasketches Library in Python is simple: `import datasketches`.
+Having installed the library, loading the Apache DataSketches Library in Python is simple: `import datasketches`.
 
 The unit tests are mostly structured in a tutorial style and can be used as a reference example for how to feed data into and query the different types of sketches.
 
 ## Available Sketch Classes
 
 - KLL (Absolute Error Quantiles)
   - `kll_ints_sketch`
@@ -72,14 +72,14 @@
 
 ## Developer Instructions
 
 The only developer-specific instructions relate to running unit tests.
 
 ### Unit tests
 
-The Python unit tests are run via `tox`, with no arguments, from the project root directory -- not the python subdirectory. Tox creates a temporary virtual environment in which to build and run the unit tests. In the event you are missing the necessary pacakge, tox may be installed with `python3 -m pip install --upgrade tox`.
+The Python unit tests are run via `tox`, with no arguments, from the project root directory -- not the python subdirectory. Tox creates a temporary virtual environment in which to build and run the unit tests. In the event you are missing the necessary package, tox may be installed with `python3 -m pip install --upgrade tox`.
 
 ## License
 
-The Apache DataSketches Library is distrubted under an Apache 2.0 License.
+The Apache DataSketches Library is distributed under the Apache 2.0 License.
 
 There may be precompiled binaries provided as a convenience and distributed through PyPI via [https://pypi.org/project/datasketches/] contain compiled code from [pybind11](https://github.com/pybind/pybind11), which is distributed under a BSD license.
```

### Comparing `datasketches-4.0.1/python/datasketches/PySerDe.py` & `datasketches-4.1.0/python/datasketches/PySerDe.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,55 +50,61 @@
   def from_bytes(self, data: bytes, offset: int):
     num_chars = int.from_bytes(data[offset:offset+3], 'little')
     if (num_chars < 0 or num_chars > offset + len(data)):
         raise IndexError(f'num_chars read must be non-negative and not larger than the buffer. Found {num_chars}')
     str = data[offset+4:offset+4+num_chars].decode()
     return (str, 4+num_chars)
 
-# Implements an integer-encoding scheme where each integer is written
+# Implements an integer encoding scheme where each integer is written
 # as a 32-bit (4 byte) little-endian value.
 class PyIntsSerDe(PyObjectSerDe):
   def get_size(self, item):
     return int(4)
 
   def to_bytes(self, item):
-    return struct.pack('i', item)
+    return struct.pack('<i', item)
 
   def from_bytes(self, data: bytes, offset: int):
-    val = struct.unpack_from('i', data, offset)[0]
+    val = struct.unpack_from('<i', data, offset)[0]
     return (val, 4)
 
 
+# Implements an integer encoding scheme where each integer is written
+# as a 64-bit (8 byte) little-endian value.
 class PyLongsSerDe(PyObjectSerDe):
   def get_size(self, item):
     return int(8)
 
   def to_bytes(self, item):
-    return struct.pack('l', item)
+    return struct.pack('<l', item)
 
   def from_bytes(self, data: bytes, offset: int):
-    val = struct.unpack_from('l', data, offset)[0]
+    val = struct.unpack_from('<l', data, offset)[0]
     return (val, 8)
 
 
+# Implements a floating point encoding scheme where each value is written
+# as a 32-bit floating point value.
 class PyFloatsSerDe(PyObjectSerDe):
   def get_size(self, item):
     return int(4)
 
   def to_bytes(self, item):
-    return struct.pack('f', item)
+    return struct.pack('<f', item)
 
   def from_bytes(self, data: bytes, offset: int):
-    val = struct.unpack_from('f', data, offset)[0]
+    val = struct.unpack_from('<f', data, offset)[0]
     return (val, 4)
 
 
+# Implements a floating point encoding scheme where each value is written
+# as a 64-bit floating point value.
 class PyDoublesSerDe(PyObjectSerDe):
   def get_size(self, item):
     return int(8)
 
   def to_bytes(self, item):
-    return struct.pack('d', item)
+    return struct.pack('<d', item)
 
   def from_bytes(self, data: bytes, offset: int):
-    val = struct.unpack_from('d', data, offset)[0]
+    val = struct.unpack_from('<d', data, offset)[0]
     return (val, 8)
```

### Comparing `datasketches-4.0.1/python/datasketches/__init__.py` & `datasketches-4.1.0/python/src/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-name = 'datasketches'
-
-from .PySerDe import *
-
-from _datasketches import *
+name = "datasketches"
```

### Comparing `datasketches-4.0.1/python/datasketches.egg-info/PKG-INFO` & `datasketches-4.1.0/python/datasketches.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasketches
-Version: 4.0.1
+Version: 4.1.0
 Summary: The Apache DataSketches Library for Python
 Home-page: http://datasketches.apache.org
 Author: Apache Software Foundation
 Author-email: dev@datasketches.apache.org
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,23 +20,23 @@
 
 If approximate results are acceptable, there is a class of specialized algorithms, called streaming algorithms, or sketches that can produce results orders-of magnitude faster and with mathematically proven error bounds. For interactive queries there may not be other viable alternatives, and in the case of real-time analysis, sketches are the only known solution.
 
 This package provides a variety of sketches as described below. Wherever a specific type of sketch exists in Apache DataSketches packages for other languages, the sketches will be portable between languages (for platforms with the same endianness).
 
 ## Building and Installation
 
-Once cloned, the library can be installed by running `python3 -m pip install .` in the project root directory -- not the python subdirectory -- which will also install the necessary dependencies, namely numpy and [pybind11[global]](https://github.com/pybind/pybind11).
+Once cloned, the library can be installed by running `python3 -m pip install .` in the project root directory -- not the python subdirectory -- which will also install the necessary dependencies, namely NumPy and [pybind11[global]](https://github.com/pybind/pybind11).
 
-If you prefer to call the `setup.py` build script directly, which is discoraged, you must first install `pybind11[global]`, as well as any other dependencies listed under the build-system section in `pyproject.toml`.
+If you prefer to call the `setup.py` build script directly, which is discouraged, you must first install `pybind11[global]`, as well as any other dependencies listed under the build-system section in `pyproject.toml`.
 
 The library is also available from PyPI via `python3 -m pip install datasketches`.
 
 ## Usage
 
-Having installed the library, loading the Apache Datasketches Library in Python is simple: `import datasketches`.
+Having installed the library, loading the Apache DataSketches Library in Python is simple: `import datasketches`.
 
 The unit tests are mostly structured in a tutorial style and can be used as a reference example for how to feed data into and query the different types of sketches.
 
 ## Available Sketch Classes
 
 - KLL (Absolute Error Quantiles)
   - `kll_ints_sketch`
@@ -84,14 +84,14 @@
 
 ## Developer Instructions
 
 The only developer-specific instructions relate to running unit tests.
 
 ### Unit tests
 
-The Python unit tests are run via `tox`, with no arguments, from the project root directory -- not the python subdirectory. Tox creates a temporary virtual environment in which to build and run the unit tests. In the event you are missing the necessary pacakge, tox may be installed with `python3 -m pip install --upgrade tox`.
+The Python unit tests are run via `tox`, with no arguments, from the project root directory -- not the python subdirectory. Tox creates a temporary virtual environment in which to build and run the unit tests. In the event you are missing the necessary package, tox may be installed with `python3 -m pip install --upgrade tox`.
 
 ## License
 
-The Apache DataSketches Library is distrubted under an Apache 2.0 License.
+The Apache DataSketches Library is distributed under the Apache 2.0 License.
 
 There may be precompiled binaries provided as a convenience and distributed through PyPI via [https://pypi.org/project/datasketches/] contain compiled code from [pybind11](https://github.com/pybind/pybind11), which is distributed under a BSD license.
```

### Comparing `datasketches-4.0.1/python/datasketches.egg-info/SOURCES.txt` & `datasketches-4.1.0/python/datasketches.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 common/test/CMakeLists.txt
 common/test/catch_runner.cpp
 common/test/integration_test.cpp
 common/test/quantiles_sorted_view_test.cpp
 common/test/test_allocator.cpp
 common/test/test_allocator.hpp
 common/test/test_type.hpp
+count/CMakeLists.txt
+count/include/count_min.hpp
+count/include/count_min_impl.hpp
+count/test/CMakeLists.txt
+count/test/count_min_allocation_test.cpp
+count/test/count_min_test.cpp
 cpc/CMakeLists.txt
 cpc/include/compression_data.hpp
 cpc/include/cpc_common.hpp
 cpc/include/cpc_compressor.hpp
 cpc/include/cpc_compressor_impl.hpp
 cpc/include/cpc_confidence.hpp
 cpc/include/cpc_sketch.hpp
@@ -47,14 +53,19 @@
 cpc/include/u32_table.hpp
 cpc/include/u32_table_impl.hpp
 cpc/test/CMakeLists.txt
 cpc/test/compression_test.cpp
 cpc/test/cpc_sketch_allocation_test.cpp
 cpc/test/cpc_sketch_test.cpp
 cpc/test/cpc_union_test.cpp
+density/CMakeLists.txt
+density/include/density_sketch.hpp
+density/include/density_sketch_impl.hpp
+density/test/CMakeLists.txt
+density/test/density_sketch_test.cpp
 fi/CMakeLists.txt
 fi/include/frequent_items_sketch.hpp
 fi/include/frequent_items_sketch_impl.hpp
 fi/include/reverse_purge_hash_map.hpp
 fi/include/reverse_purge_hash_map_impl.hpp
 fi/test/CMakeLists.txt
 fi/test/frequent_items_sketch_custom_type_test.cpp
@@ -124,49 +135,64 @@
 kll/test/kll_sketch_from_java.sk
 kll/test/kll_sketch_test.cpp
 kll/test/kll_sketch_validation.cpp
 kll/test/kolmogorov_smirnov_test.cpp
 python/CMakeLists.txt
 python/README.md
 python/pybind11Path.cmd
+python/datasketches/DensityWrapper.py
+python/datasketches/KernelFunction.py
 python/datasketches/PySerDe.py
+python/datasketches/TuplePolicy.py
+python/datasketches/TupleWrapper.py
 python/datasketches/__init__.py
 python/datasketches.egg-info/PKG-INFO
 python/datasketches.egg-info/SOURCES.txt
 python/datasketches.egg-info/dependency_links.txt
 python/datasketches.egg-info/not-zip-safe
 python/datasketches.egg-info/requires.txt
 python/datasketches.egg-info/top_level.txt
+python/include/kernel_function.hpp
+python/include/py_object_lt.hpp
+python/include/py_object_ostream.hpp
 python/include/py_serde.hpp
+python/include/quantile_conditional.hpp
+python/include/tuple_policy.hpp
 python/jupyter/CPCSketch.ipynb
 python/jupyter/FrequentItemsSketch.ipynb
 python/jupyter/HLLSketch.ipynb
 python/jupyter/KLLSketch.ipynb
 python/jupyter/ThetaSketchNotebook.ipynb
 python/src/__init__.py
+python/src/count_wrapper.cpp
 python/src/cpc_wrapper.cpp
 python/src/datasketches.cpp
+python/src/density_wrapper.cpp
 python/src/fi_wrapper.cpp
 python/src/hll_wrapper.cpp
 python/src/kll_wrapper.cpp
 python/src/ks_wrapper.cpp
 python/src/py_serde.cpp
 python/src/quantiles_wrapper.cpp
 python/src/req_wrapper.cpp
 python/src/theta_wrapper.cpp
+python/src/tuple_wrapper.cpp
 python/src/vector_of_kll.cpp
 python/src/vo_wrapper.cpp
 python/tests/__init__.py
+python/tests/count_min_test.py
 python/tests/cpc_test.py
+python/tests/density_test.py
 python/tests/fi_test.py
 python/tests/hll_test.py
 python/tests/kll_test.py
 python/tests/quantiles_test.py
 python/tests/req_test.py
 python/tests/theta_test.py
+python/tests/tuple_test.py
 python/tests/vector_of_kll_test.py
 python/tests/vo_test.py
 quantiles/CMakeLists.txt
 quantiles/include/quantiles_sketch.hpp
 quantiles/include/quantiles_sketch_impl.hpp
 quantiles/test/CMakeLists.txt
 quantiles/test/kolmogorov_smirnov_test.cpp
@@ -196,14 +222,15 @@
 sampling/test/var_opt_allocation_test.cpp
 sampling/test/var_opt_sketch_test.cpp
 sampling/test/var_opt_union_test.cpp
 sampling/test/varopt_sketch_long_sampling.sk
 sampling/test/varopt_sketch_string_exact.sk
 sampling/test/varopt_union_double_sampling.sk
 theta/CMakeLists.txt
+theta/include/bit_packing.hpp
 theta/include/bounds_on_ratios_in_sampled_sets.hpp
 theta/include/bounds_on_ratios_in_theta_sketched_sets.hpp
 theta/include/compact_theta_sketch_parser.hpp
 theta/include/compact_theta_sketch_parser_impl.hpp
 theta/include/theta_a_not_b.hpp
 theta/include/theta_a_not_b_impl.hpp
 theta/include/theta_comparators.hpp
@@ -222,14 +249,15 @@
 theta/include/theta_union.hpp
 theta/include/theta_union_base.hpp
 theta/include/theta_union_base_impl.hpp
 theta/include/theta_union_impl.hpp
 theta/include/theta_update_sketch_base.hpp
 theta/include/theta_update_sketch_base_impl.hpp
 theta/test/CMakeLists.txt
+theta/test/bit_packing_test.cpp
 theta/test/theta_a_not_b_test.cpp
 theta/test/theta_compact_empty_from_java.sk
 theta/test/theta_compact_empty_from_java_v1.sk
 theta/test/theta_compact_empty_from_java_v2.sk
 theta/test/theta_compact_estimation_from_java.sk
 theta/test/theta_compact_estimation_from_java_v1.sk
 theta/test/theta_compact_estimation_from_java_v2.sk
```

### Comparing `datasketches-4.0.1/python/include/py_serde.hpp` & `datasketches-4.1.0/python/include/py_serde.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/jupyter/CPCSketch.ipynb` & `datasketches-4.1.0/python/jupyter/CPCSketch.ipynb`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/jupyter/FrequentItemsSketch.ipynb` & `datasketches-4.1.0/python/jupyter/FrequentItemsSketch.ipynb`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/jupyter/HLLSketch.ipynb` & `datasketches-4.1.0/python/jupyter/HLLSketch.ipynb`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/jupyter/KLLSketch.ipynb` & `datasketches-4.1.0/python/jupyter/KLLSketch.ipynb`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/jupyter/ThetaSketchNotebook.ipynb` & `datasketches-4.1.0/python/jupyter/ThetaSketchNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/pybind11Path.cmd` & `datasketches-4.1.0/python/pybind11Path.cmd`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/src/__init__.py` & `datasketches-4.1.0/python/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,9 +10,7 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
-name = "datasketches"
```

### Comparing `datasketches-4.0.1/python/src/cpc_wrapper.cpp` & `datasketches-4.1.0/python/src/cpc_wrapper.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -13,78 +13,64 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-#include <sstream>
 #include <pybind11/pybind11.h>
 
 #include "cpc_sketch.hpp"
 #include "cpc_union.hpp"
 #include "cpc_common.hpp"
 #include "common_defs.hpp"
 
 namespace py = pybind11;
 
-namespace datasketches {
-namespace python {
-
-cpc_sketch* cpc_sketch_deserialize(py::bytes skBytes) {
-  std::string skStr = skBytes; // implicit cast
-  return new cpc_sketch(cpc_sketch::deserialize(skStr.c_str(), skStr.length()));
-}
-
-py::object cpc_sketch_serialize(const cpc_sketch& sk) {
-  auto serResult = sk.serialize();
-  return py::bytes((char*)serResult.data(), serResult.size());
-}
-
-cpc_sketch* cpc_union_get_result(const cpc_union& u) {
-  return new cpc_sketch(u.get_result());
-}
-
-}
-}
-
-namespace dspy = datasketches::python;
-
 void init_cpc(py::module &m) {
   using namespace datasketches;
 
   py::class_<cpc_sketch>(m, "cpc_sketch")
     .def(py::init<uint8_t, uint64_t>(), py::arg("lg_k")=cpc_constants::DEFAULT_LG_K, py::arg("seed")=DEFAULT_SEED)
     .def(py::init<const cpc_sketch&>())
     .def("__str__", &cpc_sketch::to_string,
          "Produces a string summary of the sketch")
     .def("to_string", &cpc_sketch::to_string,
          "Produces a string summary of the sketch")
-    .def("serialize", &dspy::cpc_sketch_serialize,
-         "Serializes the sketch into a bytes object")
-    .def_static("deserialize", &dspy::cpc_sketch_deserialize,
-         "Reads a bytes object and returns the corresponding cpc_sketch")
     .def<void (cpc_sketch::*)(uint64_t)>("update", &cpc_sketch::update, py::arg("datum"),
          "Updates the sketch with the given 64-bit integer value")
     .def<void (cpc_sketch::*)(double)>("update", &cpc_sketch::update, py::arg("datum"),
          "Updates the sketch with the given 64-bit floating point")
     .def<void (cpc_sketch::*)(const std::string&)>("update", &cpc_sketch::update, py::arg("datum"),
          "Updates the sketch with the given string")
     .def("is_empty", &cpc_sketch::is_empty,
-         "Returns True if the sketch is empty, otherwise Dalse")
+         "Returns True if the sketch is empty, otherwise False")
     .def("get_estimate", &cpc_sketch::get_estimate,
          "Estimate of the distinct count of the input stream")
     .def("get_lower_bound", &cpc_sketch::get_lower_bound, py::arg("kappa"),
          "Returns an approximate lower bound on the estimate for kappa values in {1, 2, 3}, roughly corresponding to standard deviations")
     .def("get_upper_bound", &cpc_sketch::get_upper_bound, py::arg("kappa"),
          "Returns an approximate upper bound on the estimate for kappa values in {1, 2, 3}, roughly corresponding to standard deviations")
-    ;
+    .def(
+        "serialize",
+        [](const cpc_sketch& sk) {
+          auto bytes = sk.serialize();
+          return py::bytes(reinterpret_cast<const char*>(bytes.data()), bytes.size());
+        },
+        "Serializes the sketch into a bytes object"
+    )
+    .def_static(
+        "deserialize",
+        [](const std::string& bytes) { return cpc_sketch::deserialize(bytes.data(), bytes.size()); },
+        py::arg("bytes"),
+        "Reads a bytes object and returns the corresponding cpc_sketch"
+    );
 
   py::class_<cpc_union>(m, "cpc_union")
     .def(py::init<uint8_t, uint64_t>(), py::arg("lg_k"), py::arg("seed")=DEFAULT_SEED)
     .def(py::init<const cpc_union&>())
     .def("update", (void (cpc_union::*)(const cpc_sketch&)) &cpc_union::update, py::arg("sketch"),
          "Updates the union with the provided CPC sketch")
-    .def("get_result", &dspy::cpc_union_get_result,
+    .def("get_result", &cpc_union::get_result,
          "Returns a CPC sketch with the result of the union")
     ;
 }
```

### Comparing `datasketches-4.0.1/python/src/datasketches.cpp` & `datasketches-4.1.0/python/src/datasketches.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -23,30 +23,36 @@
 
 // sketches
 void init_hll(py::module& m);
 void init_kll(py::module& m);
 void init_fi(py::module& m);
 void init_cpc(py::module& m);
 void init_theta(py::module& m);
+void init_tuple(py::module& m);
 void init_vo(py::module& m);
 void init_req(py::module& m);
 void init_quantiles(py::module& m);
+void init_count_min(py::module& m);
+void init_density(py::module& m);
 void init_vector_of_kll(py::module& m);
 
 // supporting objects
 void init_kolmogorov_smirnov(py::module& m);
 void init_serde(py::module& m);
 
 PYBIND11_MODULE(_datasketches, m) {
   init_hll(m);
   init_kll(m);
   init_fi(m);
   init_cpc(m);
   init_theta(m);
+  init_tuple(m);
   init_vo(m);
   init_req(m);
   init_quantiles(m);
+  init_count_min(m);
+  init_density(m);
   init_vector_of_kll(m);
 
   init_kolmogorov_smirnov(m);
   init_serde(m);
 }
```

### Comparing `datasketches-4.0.1/python/src/hll_wrapper.cpp` & `datasketches-4.1.0/python/src/hll_wrapper.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -13,62 +13,33 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-#include "hll.hpp"
-
 #include <pybind11/pybind11.h>
 
-namespace py = pybind11;
-
-namespace datasketches {
-namespace python {
-
-hll_sketch hll_sketch_deserialize(py::bytes skBytes) {
-  std::string skStr = skBytes; // implicit cast  
-  return hll_sketch::deserialize(skStr.c_str(), skStr.length());
-}
-
-py::object hll_sketch_serialize_compact(const hll_sketch& sk) {
-  auto serResult = sk.serialize_compact();
-  return py::bytes((char*)serResult.data(), serResult.size());
-}
-
-py::object hll_sketch_serialize_updatable(const hll_sketch& sk) {
-  auto serResult = sk.serialize_updatable();
-  return py::bytes((char*)serResult.data(), serResult.size());
-}
-
-}
-}
+#include "hll.hpp"
 
-namespace dspy = datasketches::python;
+namespace py = pybind11;
 
 void init_hll(py::module &m) {
   using namespace datasketches;
 
   py::enum_<target_hll_type>(m, "tgt_hll_type", "Target HLL flavor")
     .value("HLL_4", HLL_4)
     .value("HLL_6", HLL_6)
     .value("HLL_8", HLL_8)
     .export_values();
 
   py::class_<hll_sketch>(m, "hll_sketch")
     .def(py::init<uint8_t>(), py::arg("lg_k"))
     .def(py::init<uint8_t, target_hll_type>(), py::arg("lg_k"), py::arg("tgt_type"))
     .def(py::init<uint8_t, target_hll_type, bool>(), py::arg("lg_k"), py::arg("tgt_type"), py::arg("start_max_size")=false)
-    .def_static("deserialize", &dspy::hll_sketch_deserialize,
-         "Reads a bytes object and returns the corresponding hll_sketch")
-    .def("serialize_compact", &dspy::hll_sketch_serialize_compact,
-         "Serializes the sketch into a bytes object, compressiong the exception table if HLL_4")
-    .def("serialize_updatable", &dspy::hll_sketch_serialize_updatable,
-         "Serializes the sketch into a bytes object")
     .def("__str__", (std::string (hll_sketch::*)(bool,bool,bool,bool) const) &hll_sketch::to_string,
          py::arg("summary")=true, py::arg("detail")=false, py::arg("aux_detail")=false, py::arg("all")=false,
          "Produces a string summary of the sketch")
     .def("to_string", (std::string (hll_sketch::*)(bool,bool,bool,bool) const) &hll_sketch::to_string,
          py::arg("summary")=true, py::arg("detail")=false, py::arg("aux_detail")=false, py::arg("all")=false,
          "Produces a string summary of the sketch")
     .def_property_readonly("lg_config_k", &hll_sketch::get_lg_config_k, "Configured lg_k value for the sketch")
@@ -84,28 +55,49 @@
     .def("is_empty", &hll_sketch::is_empty,
          "True if the sketch is empty, otherwise False")
     .def("get_updatable_serialization_bytes", &hll_sketch::get_updatable_serialization_bytes,
          "Returns the size of the serialized sketch")
     .def("get_compact_serialization_bytes", &hll_sketch::get_compact_serialization_bytes,
          "Returns the size of the serialized sketch when compressing the exception table if HLL_4")
     .def("reset", &hll_sketch::reset,
-         "Resets the sketch to the empty state in coupon colleciton mode")
+         "Resets the sketch to the empty state in coupon collection mode")
     .def("update", (void (hll_sketch::*)(int64_t)) &hll_sketch::update, py::arg("datum"),
          "Updates the sketch with the given integral value")
     .def("update", (void (hll_sketch::*)(double)) &hll_sketch::update, py::arg("datum"),
          "Updates the sketch with the given floating point value")
     .def("update", (void (hll_sketch::*)(const std::string&)) &hll_sketch::update, py::arg("datum"),
          "Updates the sketch with the given string value")
     .def_static("get_max_updatable_serialization_bytes", &hll_sketch::get_max_updatable_serialization_bytes,
          py::arg("lg_k"), py::arg("tgt_type"),
-         "Provides a likely upper bound on serialization size for the given paramters")
+         "Provides a likely upper bound on serialization size for the given parameters")
     .def_static("get_rel_err", &hll_sketch::get_rel_err,
          py::arg("upper_bound"), py::arg("unioned"), py::arg("lg_k"), py::arg("num_std_devs"),
-         "Retuns the a priori relative error bound for the given parameters")
-    ;
+         "Returns the a priori relative error bound for the given parameters")
+    .def(
+        "serialize_compact",
+        [](const hll_sketch& sk) {
+          auto bytes = sk.serialize_compact();
+          return py::bytes(reinterpret_cast<const char*>(bytes.data()), bytes.size());
+        },
+        "Serializes the sketch into a bytes object, compressing the exception table if HLL_4"
+    )
+    .def(
+        "serialize_updatable",
+        [](const hll_sketch& sk) {
+          auto bytes = sk.serialize_updatable();
+          return py::bytes(reinterpret_cast<const char*>(bytes.data()), bytes.size());
+        },
+        "Serializes the sketch into a bytes object"
+    )
+    .def_static(
+        "deserialize",
+        [](const std::string& bytes) { return hll_sketch::deserialize(bytes.data(), bytes.size()); },
+        py::arg("bytes"),
+        "Reads a bytes object and returns the corresponding hll_sketch"
+    );
 
   py::class_<hll_union>(m, "hll_union")
     .def(py::init<uint8_t>(), py::arg("lg_max_k"))
     .def_property_readonly("lg_config_k", &hll_union::get_lg_config_k, "Configured lg_k value for the union")
     .def_property_readonly("tgt_type", &hll_union::get_target_type, "Returns the HLL type (4, 6, or 8) when in estimation mode")
     .def("get_estimate", &hll_union::get_estimate,
          "Estimate of the distinct count of the input stream")
@@ -125,10 +117,10 @@
          "Updates the union with the given integral value")
     .def<void (hll_union::*)(double)>("update", &hll_union::update, py::arg("datum"),
          "Updates the union with the given floating point value")
     .def<void (hll_union::*)(const std::string&)>("update", &hll_union::update, py::arg("datum"),
          "Updates the union with the given string value")
     .def_static("get_rel_err", &hll_union::get_rel_err,
          py::arg("upper_bound"), py::arg("unioned"), py::arg("lg_k"), py::arg("num_std_devs"),
-         "Retuns the a priori relative error bound for the given parameters")
+         "Returns the a priori relative error bound for the given parameters")
     ;
 }
```

### Comparing `datasketches-4.0.1/python/src/kll_wrapper.cpp` & `datasketches-4.1.0/python/src/kll_wrapper.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -13,198 +13,146 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
+#include "py_object_lt.hpp"
+#include "py_object_ostream.hpp"
+#include "quantile_conditional.hpp"
 #include "kll_sketch.hpp"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
-#include <pybind11/numpy.h>
-#include <sstream>
 #include <vector>
 #include <stdexcept>
 
 namespace py = pybind11;
 
-namespace datasketches {
-
-namespace python {
-
-template<typename T>
-kll_sketch<T> kll_sketch_deserialize(py::bytes skBytes) {
-  std::string skStr = skBytes; // implicit cast  
-  return kll_sketch<T>::deserialize(skStr.c_str(), skStr.length());
-}
-
-template<typename T>
-py::object kll_sketch_serialize(const kll_sketch<T>& sk) {
-  auto serResult = sk.serialize();
-  return py::bytes((char*)serResult.data(), serResult.size());
-}
-
-// maybe possible to disambiguate the static vs method rank error calls, but
-// this is easier for now
-template<typename T>
-double kll_sketch_generic_normalized_rank_error(uint16_t k, bool pmf) {
-  return kll_sketch<T>::get_normalized_rank_error(k, pmf);
-}
-
-template<typename T>
-py::list kll_sketch_get_quantiles(const kll_sketch<T>& sk,
-                                  std::vector<double>& ranks,
-                                  bool inclusive) {
-  size_t nQuantiles = ranks.size();
-  auto result = sk.get_quantiles(ranks.data(), nQuantiles, inclusive);
-  // returning as std::vector<> would copy values to a list anyway
-  py::list list(nQuantiles);
-  for (size_t i = 0; i < nQuantiles; ++i) {
-      list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-py::list kll_sketch_get_pmf(const kll_sketch<T>& sk,
-                            std::vector<T>& split_points,
-                            bool inclusive) {
-  size_t nPoints = split_points.size();
-  auto result = sk.get_PMF(split_points.data(), nPoints, inclusive);
-  py::list list(nPoints + 1);
-  for (size_t i = 0; i <= nPoints; ++i) {
-    list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-py::list kll_sketch_get_cdf(const kll_sketch<T>& sk,
-                            std::vector<T>& split_points,
-                            bool inclusive) {
-  size_t nPoints = split_points.size();
-  auto result = sk.get_CDF(split_points.data(), nPoints, inclusive);
-  py::list list(nPoints + 1);
-  for (size_t i = 0; i <= nPoints; ++i) {
-    list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-void kll_sketch_update(kll_sketch<T>& sk, py::array_t<T, py::array::c_style | py::array::forcecast> items) {
-  if (items.ndim() != 1) {
-    throw std::invalid_argument("input data must have only one dimension. Found: "
-          + std::to_string(items.ndim()));
-  }
-  
-  auto data = items.template unchecked<1>();
-  for (uint32_t i = 0; i < data.size(); ++i) {
-    sk.update(data(i));
-  }
-}
-
-}
-}
-
-namespace dspy = datasketches::python;
-
-template<typename T>
+template<typename T, typename C>
 void bind_kll_sketch(py::module &m, const char* name) {
   using namespace datasketches;
 
-  py::class_<kll_sketch<T>>(m, name)
+  auto kll_class = py::class_<kll_sketch<T, C>>(m, name)
     .def(py::init<uint16_t>(), py::arg("k")=kll_constants::DEFAULT_K)
-    .def(py::init<const kll_sketch<T>&>())
-    .def("update", (void (kll_sketch<T>::*)(const T&)) &kll_sketch<T>::update, py::arg("item"),
-         "Updates the sketch with the given value")
-    .def("update", &dspy::kll_sketch_update<T>, py::arg("array"),
-         "Updates the sketch with the values in the given array")
-    .def("merge", (void (kll_sketch<T>::*)(const kll_sketch<T>&)) &kll_sketch<T>::merge, py::arg("sketch"),
-         "Merges the provided sketch into the this one")
-    .def("__str__", &kll_sketch<T>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
-         "Produces a string summary of the sketch")
-    .def("to_string", &kll_sketch<T>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
-         "Produces a string summary of the sketch")
-    .def("is_empty", &kll_sketch<T>::is_empty,
-         "Returns True if the sketch is empty, otherwise False")
-    .def("get_k", &kll_sketch<T>::get_k,
-         "Returns the configured parameter k")
-    .def("get_n", &kll_sketch<T>::get_n,
-         "Returns the length of the input stream")
-    .def("get_num_retained", &kll_sketch<T>::get_num_retained,
-         "Returns the number of retained items (samples) in the sketch")
-    .def("is_estimation_mode", &kll_sketch<T>::is_estimation_mode,
-         "Returns True if the sketch is in estimation mode, otherwise False")
-    .def("get_min_value", &kll_sketch<T>::get_min_item,
-         "Returns the minimum value from the stream. If empty, kll_floats_sketch returns nan; kll_ints_sketch throws a RuntimeError")
-    .def("get_max_value", &kll_sketch<T>::get_max_item,
-         "Returns the maximum value from the stream. If empty, kll_floats_sketch returns nan; kll_ints_sketch throws a RuntimeError")
-    .def("get_quantile", &kll_sketch<T>::get_quantile, py::arg("rank"), py::arg("inclusive")=false,
-         "Returns an approximation to the data value "
-         "associated with the given normalized rank in a hypothetical sorted "
-         "version of the input stream so far.\n"
-         "For kll_floats_sketch: if the sketch is empty this returns nan. "
-         "For kll_ints_sketch: if the sketch is empty this throws a RuntimeError.")
-    .def("get_quantiles", &dspy::kll_sketch_get_quantiles<T>, py::arg("ranks"), py::arg("inclusive")=false,
-         "This returns an array that could have been generated by using get_quantile() for each "
-         "normalized rank separately.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "Deprecated. Will be removed in the next major version. Use get_quantile() instead.")
-    .def("get_rank", &kll_sketch<T>::get_rank, py::arg("value"), py::arg("inclusive")=false,
+    .def(py::init<const kll_sketch<T, C>&>())
+    .def(
+        "update",
+        static_cast<void (kll_sketch<T, C>::*)(const T&)>(&kll_sketch<T, C>::update),
+        py::arg("item"),
+        "Updates the sketch with the given value"
+    )
+    .def("merge", (void (kll_sketch<T, C>::*)(const kll_sketch<T, C>&)) &kll_sketch<T, C>::merge, py::arg("sketch"),
+        "Merges the provided sketch into this one")
+    .def("__str__", &kll_sketch<T, C>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
+        "Produces a string summary of the sketch")
+    .def("to_string", &kll_sketch<T, C>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
+        "Produces a string summary of the sketch")
+    .def("is_empty", &kll_sketch<T, C>::is_empty,
+        "Returns True if the sketch is empty, otherwise False")
+    .def("get_k", &kll_sketch<T, C>::get_k,
+        "Returns the configured parameter k")
+    .def("get_n", &kll_sketch<T, C>::get_n,
+        "Returns the length of the input stream")
+    .def("get_num_retained", &kll_sketch<T, C>::get_num_retained,
+        "Returns the number of retained items (samples) in the sketch")
+    .def("is_estimation_mode", &kll_sketch<T, C>::is_estimation_mode,
+        "Returns True if the sketch is in estimation mode, otherwise False")
+    .def("get_min_value", &kll_sketch<T, C>::get_min_item,
+        "Returns the minimum value from the stream. If empty, kll_floats_sketch returns nan; kll_ints_sketch throws a RuntimeError")
+    .def("get_max_value", &kll_sketch<T, C>::get_max_item,
+        "Returns the maximum value from the stream. If empty, kll_floats_sketch returns nan; kll_ints_sketch throws a RuntimeError")
+    .def("get_quantile", &kll_sketch<T, C>::get_quantile, py::arg("rank"), py::arg("inclusive")=false,
+        "Returns an approximation to the data value "
+        "associated with the given normalized rank in a hypothetical sorted "
+        "version of the input stream so far.\n"
+        "For kll_floats_sketch: if the sketch is empty this returns nan. "
+        "For kll_ints_sketch: if the sketch is empty this throws a RuntimeError.")
+    .def(
+        "get_quantiles",
+        [](const kll_sketch<T, C>& sk, const std::vector<double>& ranks, bool inclusive) {
+          return sk.get_quantiles(ranks.data(), ranks.size(), inclusive);
+        },
+        py::arg("ranks"), py::arg("inclusive")=false,
+        "This returns an array that could have been generated by using get_quantile() for each "
+        "normalized rank separately.\n"
+        "If the sketch is empty this returns an empty vector.\n"
+        "Deprecated. Will be removed in the next major version. Use get_quantile() instead."
+    )
+    .def("get_rank", &kll_sketch<T, C>::get_rank, py::arg("value"), py::arg("inclusive")=false,
          "Returns an approximation to the normalized rank of the given value from 0 to 1, inclusive.\n"
          "The resulting approximation has a probabilistic guarantee that can be obtained from the "
          "get_normalized_rank_error(False) function.\n"
          "With the parameter inclusive=true the weight of the given value is included into the rank."
          "Otherwise the rank equals the sum of the weights of values less than the given value.\n"
          "If the sketch is empty this returns nan.")
-    .def("get_pmf", &dspy::kll_sketch_get_pmf<T>, py::arg("split_points"), py::arg("inclusive")=false,
-         "Returns an approximation to the Probability Mass Function (PMF) of the input stream "
-         "given a set of split points (values).\n"
-         "The resulting approximations have a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(True) function.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "split_points is an array of m unique, monotonically increasing float values "
-         "that divide the real number line into m+1 consecutive disjoint intervals.\n"
-         "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
-         "exclusive of the right split point, with the exception that the last interval will include "
-         "the maximum value.\n"
-         "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
-         "inclusive of the right split point.\n"
-         "It is not necessary to include either the min or max values in these split points.")
-    .def("get_cdf", &dspy::kll_sketch_get_cdf<T>, py::arg("split_points"), py::arg("inclusive")=false,
-         "Returns an approximation to the Cumulative Distribution Function (CDF), which is the "
-         "cumulative analog of the PMF, of the input stream given a set of split points (values).\n"
-         "The resulting approximations have a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(True) function.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "split_points is an array of m unique, monotonically increasing float values "
-         "that divide the real number line into m+1 consecutive disjoint intervals.\n"
-         "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
-         "exclusive of the right split point, with the exception that the last interval will include "
-         "the maximum value.\n"
-         "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
-         "inclusive of the right split point.\n"
-         "It is not necessary to include either the min or max values in these split points.")
-    .def("normalized_rank_error", (double (kll_sketch<T>::*)(bool) const) &kll_sketch<T>::get_normalized_rank_error,
+    .def(
+        "get_pmf",
+        [](const kll_sketch<T, C>& sk, const std::vector<T>& split_points, bool inclusive) {
+          return sk.get_PMF(split_points.data(), split_points.size(), inclusive);
+        },
+        py::arg("split_points"), py::arg("inclusive")=false,
+        "Returns an approximation to the Probability Mass Function (PMF) of the input stream "
+        "given a set of split points (values).\n"
+        "The resulting approximations have a probabilistic guarantee that can be obtained from the "
+        "get_normalized_rank_error(True) function.\n"
+        "If the sketch is empty this returns an empty vector.\n"
+        "split_points is an array of m unique, monotonically increasing float values "
+        "that divide the real number line into m+1 consecutive disjoint intervals.\n"
+        "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
+        "exclusive of the right split point, with the exception that the last interval will include "
+        "the maximum value.\n"
+        "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
+        "inclusive of the right split point.\n"
+        "It is not necessary to include either the min or max values in these split points."
+    )
+    .def(
+        "get_cdf",
+        [](const kll_sketch<T, C>& sk, const std::vector<T>& split_points, bool inclusive) {
+          return sk.get_CDF(split_points.data(), split_points.size(), inclusive);
+        },
+        py::arg("split_points"), py::arg("inclusive")=false,
+        "Returns an approximation to the Cumulative Distribution Function (CDF), which is the "
+        "cumulative analog of the PMF, of the input stream given a set of split points (values).\n"
+        "The resulting approximations have a probabilistic guarantee that can be obtained from the "
+        "get_normalized_rank_error(True) function.\n"
+        "If the sketch is empty this returns an empty vector.\n"
+        "split_points is an array of m unique, monotonically increasing float values "
+        "that divide the real number line into m+1 consecutive disjoint intervals.\n"
+        "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
+        "exclusive of the right split point, with the exception that the last interval will include "
+        "the maximum value.\n"
+        "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
+        "inclusive of the right split point.\n"
+        "It is not necessary to include either the min or max values in these split points."
+    )
+    .def(
+        "normalized_rank_error",
+        static_cast<double (kll_sketch<T, C>::*)(bool) const>(&kll_sketch<T, C>::get_normalized_rank_error),
          py::arg("as_pmf"),
          "Gets the normalized rank error for this sketch.\n"
          "If pmf is True, returns the 'double-sided' normalized rank error for the get_PMF() function.\n"
          "Otherwise, it is the 'single-sided' normalized rank error for all the other queries.\n"
-         "Constants were derived as the best fit to 99 percentile empirically measured max error in thousands of trials")
-    .def_static("get_normalized_rank_error", &dspy::kll_sketch_generic_normalized_rank_error<T>,
+         "Constants were derived as the best fit to 99 percentile empirically measured max error in thousands of trials"
+    )
+    .def_static(
+        "get_normalized_rank_error",
+        [](uint16_t k, bool pmf) { return kll_sketch<T, C>::get_normalized_rank_error(k, pmf); },
          py::arg("k"), py::arg("as_pmf"),
          "Gets the normalized rank error given parameters k and the pmf flag.\n"
          "If pmf is True, returns the 'double-sided' normalized rank error for the get_PMF() function.\n"
          "Otherwise, it is the 'single-sided' normalized rank error for all the other queries.\n"
-         "Constants were derived as the best fit to 99 percentile empirically measured max error in thousands of trials")
-    .def("serialize", &dspy::kll_sketch_serialize<T>, "Serializes the sketch into a bytes object")
-    .def_static("deserialize", &dspy::kll_sketch_deserialize<T>, "Deserializes the sketch from a bytes object")
-    ;
+         "Constants were derived as the best fit to 99 percentile empirically measured max error in thousands of trials"
+    )
+    .def("__iter__", [](const kll_sketch<T, C>& s) { return py::make_iterator(s.begin(), s.end()); });
+
+    add_serialization<T>(kll_class);
+    add_vector_update<T>(kll_class);
 }
 
 void init_kll(py::module &m) {
-  bind_kll_sketch<int>(m, "kll_ints_sketch");
-  bind_kll_sketch<float>(m, "kll_floats_sketch");
-  bind_kll_sketch<double>(m, "kll_doubles_sketch");
+  bind_kll_sketch<int, std::less<int>>(m, "kll_ints_sketch");
+  bind_kll_sketch<float, std::less<float>>(m, "kll_floats_sketch");
+  bind_kll_sketch<double, std::less<double>>(m, "kll_doubles_sketch");
+  bind_kll_sketch<py::object, py_object_lt>(m, "kll_items_sketch");
 }
```

### Comparing `datasketches-4.0.1/python/src/ks_wrapper.cpp` & `datasketches-4.1.0/python/src/ks_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/src/py_serde.cpp` & `datasketches-4.1.0/python/src/py_serde.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 #include "py_serde.hpp"
 
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 
 void init_serde(py::module& m) {
-  py::class_<datasketches::py_object_serde, datasketches::PyObjectSerDe /* <--- trampoline*/>(m, "PyObjectSerDe")
+  using namespace datasketches;
+  py::class_<py_object_serde, PyObjectSerDe /* <--- trampoline*/>(m, "PyObjectSerDe")
     .def(py::init<>())
-    .def("get_size", &datasketches::py_object_serde::get_size, py::arg("item"),
+    .def("get_size", &py_object_serde::get_size, py::arg("item"),
         "Returns the size in bytes of an item")
-    .def("to_bytes", &datasketches::py_object_serde::to_bytes, py::arg("item"),
+    .def("to_bytes", &py_object_serde::to_bytes, py::arg("item"),
         "Retuns a bytes object with a serialized version of an item")
-    .def("from_bytes", &datasketches::py_object_serde::from_bytes, py::arg("data"), py::arg("offset"),
+    .def("from_bytes", &py_object_serde::from_bytes, py::arg("data"), py::arg("offset"),
         "Reads a bytes object starting from the given offest and returns a tuple of the reconstructed "
         "object and the number of additional bytes read")
     ;
 }    
 
 namespace datasketches {
   size_t py_object_serde::size_of_item(const py::object& item) const {
```

### Comparing `datasketches-4.0.1/python/src/quantiles_wrapper.cpp` & `datasketches-4.1.0/python/src/req_wrapper.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -13,192 +13,142 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-#include "quantiles_sketch.hpp"
+#include "py_object_lt.hpp"
+#include "py_object_ostream.hpp"
+#include "quantile_conditional.hpp"
+#include "req_sketch.hpp"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 #include <vector>
+#include <stdexcept>
 
 namespace py = pybind11;
 
-namespace datasketches {
-
-namespace python {
-
-template<typename T>
-quantiles_sketch<T> quantiles_sketch_deserialize(py::bytes sk_bytes) {
-  std::string sk_str = sk_bytes; // implicit cast  
-  return quantiles_sketch<T>::deserialize(sk_str.c_str(), sk_str.length());
-}
-
-template<typename T>
-py::object quantiles_sketch_serialize(const quantiles_sketch<T>& sk) {
-  auto ser_result = sk.serialize();
-  return py::bytes((char*)ser_result.data(), ser_result.size());
-}
-
-// maybe possible to disambiguate the static vs method rank error calls, but
-// this is easier for now
-template<typename T>
-double quantiles_sketch_generic_normalized_rank_error(uint16_t k, bool pmf) {
-  return quantiles_sketch<T>::get_normalized_rank_error(k, pmf);
-}
-
-template<typename T>
-py::list quantiles_sketch_get_quantiles(const quantiles_sketch<T>& sk,
-                                        std::vector<double>& ranks,
-                                        bool inclusive) {
-  size_t n_quantiles = ranks.size();
-  auto result = sk.get_quantiles(ranks.data(), static_cast<uint32_t>(n_quantiles), inclusive);
-  // returning as std::vector<> would copy values to a list anyway
-  py::list list(n_quantiles);
-  for (size_t i = 0; i < n_quantiles; ++i) {
-      list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-py::list quantiles_sketch_get_pmf(const quantiles_sketch<T>& sk,
-                                  std::vector<T>& split_points,
-                                  bool inclusive) {
-  size_t n_points = split_points.size();
-  auto result = sk.get_PMF(split_points.data(), n_points, inclusive);
-  py::list list(n_points + 1);
-  for (size_t i = 0; i <= n_points; ++i) {
-    list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-py::list quantiles_sketch_get_cdf(const quantiles_sketch<T>& sk,
-                                  std::vector<T>& split_points,
-                                  bool inclusive) {
-  size_t n_points = split_points.size();
-  auto result = sk.get_CDF(split_points.data(), n_points, inclusive);
-  py::list list(n_points + 1);
-  for (size_t i = 0; i <= n_points; ++i) {
-    list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-void quantiles_sketch_update(quantiles_sketch<T>& sk, py::array_t<T, py::array::c_style | py::array::forcecast> items) {
-  if (items.ndim() != 1) {
-    throw std::invalid_argument("input data must have only one dimension. Found: "
-          + std::to_string(items.ndim()));
-  }
-  
-  auto data = items.template unchecked<1>();
-  for (uint32_t i = 0; i < data.size(); ++i) {
-    sk.update(data(i));
-  }
-}
-
-}
-}
-
-namespace dspy = datasketches::python;
-
-template<typename T>
-void bind_quantiles_sketch(py::module &m, const char* name) {
+template<typename T, typename C>
+void bind_req_sketch(py::module &m, const char* name) {
   using namespace datasketches;
 
-  py::class_<quantiles_sketch<T>>(m, name)
-    .def(py::init<uint16_t>(), py::arg("k")=quantiles_constants::DEFAULT_K)
-    .def(py::init<const quantiles_sketch<T>&>())
-    .def("update", (void (quantiles_sketch<T>::*)(const T&)) &quantiles_sketch<T>::update, py::arg("item"),
-         "Updates the sketch with the given value")
-    .def("update", &dspy::quantiles_sketch_update<T>, py::arg("array"),
-         "Updates the sketch with the values in the given array")
-    .def("merge", (void (quantiles_sketch<T>::*)(const quantiles_sketch<T>&)) &quantiles_sketch<T>::merge, py::arg("sketch"),
-         "Merges the provided sketch into the this one")
-    .def("__str__", &quantiles_sketch<T>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
-         "Produces a string summary of the sketch")
-    .def("to_string", &quantiles_sketch<T>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
-         "Produces a string summary of the sketch")
-    .def("is_empty", &quantiles_sketch<T>::is_empty,
-         "Returns True if the sketch is empty, otherwise False")
-    .def("get_k", &quantiles_sketch<T>::get_k,
-         "Returns the configured parameter k")
-    .def("get_n", &quantiles_sketch<T>::get_n,
-         "Returns the length of the input stream")
-    .def("get_num_retained", &quantiles_sketch<T>::get_num_retained,
-         "Returns the number of retained items (samples) in the sketch")
-    .def("is_estimation_mode", &quantiles_sketch<T>::is_estimation_mode,
-         "Returns True if the sketch is in estimation mode, otherwise False")
-    .def("get_min_value", &quantiles_sketch<T>::get_min_item,
-         "Returns the minimum value from the stream. If empty, quantiles_floats_sketch returns nan; quantiles_ints_sketch throws a RuntimeError")
-    .def("get_max_value", &quantiles_sketch<T>::get_max_item,
-         "Returns the maximum value from the stream. If empty, quantiles_floats_sketch returns nan; quantiles_ints_sketch throws a RuntimeError")
-    .def("get_quantile", &quantiles_sketch<T>::get_quantile, py::arg("rank"), py::arg("inclusive")=false,
-         "Returns an approximation to the data value "
-         "associated with the given rank in a hypothetical sorted "
-         "version of the input stream so far.\n"
-         "For quantiles_floats_sketch: if the sketch is empty this returns nan. "
-         "For quantiles_ints_sketch: if the sketch is empty this throws a RuntimeError.")
-    .def("get_quantiles", &dspy::quantiles_sketch_get_quantiles<T>, py::arg("ranks"), py::arg("inclusive")=false,
-         "This returns an array that could have been generated by using get_quantile() for each "
-         "normalized rank separately.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "Deprecated. Will be removed in the next major version. Use get_quantile() instead.")
-    .def("get_rank", &quantiles_sketch<T>::get_rank, py::arg("value"), py::arg("inclusive")=false,
-         "Returns an approximation to the normalized rank of the given value from 0 to 1, inclusive.\n"
-         "The resulting approximation has a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(False) function.\n"
-         "With the parameter inclusive=true the weight of the given value is included into the rank."
-         "Otherwise the rank equals the sum of the weights of values less than the given value.\n"
-         "If the sketch is empty this returns nan.")
-    .def("get_pmf", &dspy::quantiles_sketch_get_pmf<T>, py::arg("split_points"), py::arg("inclusive")=false,
-         "Returns an approximation to the Probability Mass Function (PMF) of the input stream "
-         "given a set of split points (values).\n"
-         "The resulting approximations have a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(True) function.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "split_points is an array of m unique, monotonically increasing float values "
-         "that divide the real number line into m+1 consecutive disjoint intervals.\n"
-         "The definition of an 'interval' is inclusive of the left split point (or minimum value) and "
-         "exclusive of the right split point, with the exception that the last interval will include "
-         "the maximum value.\n"
-         "It is not necessary to include either the min or max values in these split points.")
-    .def("get_cdf", &dspy::quantiles_sketch_get_cdf<T>, py::arg("split_points"), py::arg("inclusive")=false,
-         "Returns an approximation to the Cumulative Distribution Function (CDF), which is the "
-         "cumulative analog of the PMF, of the input stream given a set of split points (values).\n"
-         "The resulting approximations have a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(True) function.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "split_points is an array of m unique, monotonically increasing float values "
-         "that divide the real number line into m+1 consecutive disjoint intervals.\n"
-         "The definition of an 'interval' is inclusive of the left split point (or minimum value) and "
-         "exclusive of the right split point, with the exception that the last interval will include "
-         "the maximum value.\n"
-         "It is not necessary to include either the min or max values in these split points.")
-    .def("normalized_rank_error", (double (quantiles_sketch<T>::*)(bool) const) &quantiles_sketch<T>::get_normalized_rank_error,
-         py::arg("as_pmf"),
-         "Gets the normalized rank error for this sketch.\n"
-         "If pmf is True, returns the 'double-sided' normalized rank error for the get_PMF() function.\n"
-         "Otherwise, it is the 'single-sided' normalized rank error for all the other queries.\n"
-         "Constants were derived as the best fit to 99 percentile empirically measured max error in thousands of trials")
-    .def_static("get_normalized_rank_error", &dspy::quantiles_sketch_generic_normalized_rank_error<T>,
-         py::arg("k"), py::arg("as_pmf"),
-         "Gets the normalized rank error given parameters k and the pmf flag.\n"
-         "If pmf is True, returns the 'double-sided' normalized rank error for the get_PMF() function.\n"
-         "Otherwise, it is the 'single-sided' normalized rank error for all the other queries.\n"
-         "Constants were derived as the best fit to 99 percentile empirically measured max error in thousands of trials")
-    .def("serialize", &dspy::quantiles_sketch_serialize<T>, "Serializes the sketch into a bytes object")
-    .def_static("deserialize", &dspy::quantiles_sketch_deserialize<T>, "Deserializes the sketch from a bytes object")
-    ;
-}
-
-void init_quantiles(py::module &m) {
-  bind_quantiles_sketch<int>(m, "quantiles_ints_sketch");
-  bind_quantiles_sketch<float>(m, "quantiles_floats_sketch");
-  bind_quantiles_sketch<double>(m, "quantiles_doubles_sketch");
+  auto req_class = py::class_<req_sketch<T, C>>(m, name)
+    .def(py::init<uint16_t, bool>(), py::arg("k")=12, py::arg("is_hra")=true)
+    .def(py::init<const req_sketch<T, C>&>())
+    .def("update", (void (req_sketch<T, C>::*)(const T&)) &req_sketch<T, C>::update, py::arg("item"),
+        "Updates the sketch with the given value")
+    .def("merge", (void (req_sketch<T, C>::*)(const req_sketch<T, C>&)) &req_sketch<T, C>::merge, py::arg("sketch"),
+        "Merges the provided sketch into this one")
+    .def("__str__", &req_sketch<T, C>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
+        "Produces a string summary of the sketch")
+    .def("to_string", &req_sketch<T, C>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
+        "Produces a string summary of the sketch")
+    .def("is_hra", &req_sketch<T, C>::is_HRA,
+        "Returns True if the sketch is in High Rank Accuracy mode, otherwise False")
+    .def("is_empty", &req_sketch<T, C>::is_empty,
+        "Returns True if the sketch is empty, otherwise False")
+    .def("get_k", &req_sketch<T, C>::get_k,
+        "Returns the configured parameter k")
+    .def("get_n", &req_sketch<T, C>::get_n,
+        "Returns the length of the input stream")
+    .def("get_num_retained", &req_sketch<T, C>::get_num_retained,
+        "Returns the number of retained items (samples) in the sketch")
+    .def("is_estimation_mode", &req_sketch<T, C>::is_estimation_mode,
+        "Returns True if the sketch is in estimation mode, otherwise False")
+    .def("get_min_value", &req_sketch<T, C>::get_min_item,
+        "Returns the minimum value from the stream. If empty, req_floats_sketch returns nan; req_ints_sketch throws a RuntimeError")
+    .def("get_max_value", &req_sketch<T, C>::get_max_item,
+        "Returns the maximum value from the stream. If empty, req_floats_sketch returns nan; req_ints_sketch throws a RuntimeError")
+    .def("get_quantile", &req_sketch<T, C>::get_quantile, py::arg("rank"), py::arg("inclusive")=false,
+        "Returns an approximation to the data value "
+        "associated with the given normalized rank in a hypothetical sorted "
+        "version of the input stream so far.\n"
+        "For req_floats_sketch: if the sketch is empty this returns nan. "
+        "For req_ints_sketch: if the sketch is empty this throws a RuntimeError.")
+    .def(
+        "get_quantiles",
+        [](const req_sketch<T, C>& sk, const std::vector<double>& ranks, bool inclusive) {
+          return sk.get_quantiles(ranks.data(), ranks.size(), inclusive);
+        },
+        py::arg("ranks"), py::arg("inclusive")=false,
+        "This returns an array that could have been generated by using get_quantile() for each "
+        "normalized rank separately.\n"
+        "If the sketch is empty this returns an empty vector.\n"
+        "Deprecated. Will be removed in the next major version. Use get_quantile() instead."
+    )
+    .def("get_rank", &req_sketch<T, C>::get_rank, py::arg("value"), py::arg("inclusive")=false,
+        "Returns an approximation to the normalized rank of the given value from 0 to 1, inclusive.\n"
+        "The resulting approximation has a probabilistic guarantee that can be obtained from the "
+        "get_normalized_rank_error(False) function.\n"
+        "With the parameter inclusive=true the weight of the given value is included into the rank."
+        "Otherwise the rank equals the sum of the weights of values less than the given value.\n"
+        "If the sketch is empty this returns nan.")
+    .def(
+        "get_pmf",
+        [](const req_sketch<T, C>& sk, const std::vector<T>& split_points, bool inclusive) {
+          return sk.get_PMF(split_points.data(), split_points.size(), inclusive);
+        },
+        py::arg("split_points"), py::arg("inclusive")=false,
+        "Returns an approximation to the Probability Mass Function (PMF) of the input stream "
+        "given a set of split points (values).\n"
+        "The resulting approximations have a probabilistic guarantee that can be obtained from the "
+        "get_normalized_rank_error(True) function.\n"
+        "If the sketch is empty this returns an empty vector.\n"
+        "split_points is an array of m unique, monotonically increasing float values "
+        "that divide the real number line into m+1 consecutive disjoint intervals.\n"
+        "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
+        "exclusive of the right split point, with the exception that the last interval will include "
+        "the maximum value.\n"
+        "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
+        "inclusive of the right split point.\n"
+        "It is not necessary to include either the min or max values in these split points."
+    )
+    .def(
+        "get_cdf",
+        [](const req_sketch<T, C>& sk, const std::vector<T>& split_points, bool inclusive) {
+          return sk.get_CDF(split_points.data(), split_points.size(), inclusive);
+        },
+        py::arg("split_points"), py::arg("inclusive")=false,
+        "Returns an approximation to the Cumulative Distribution Function (CDF), which is the "
+        "cumulative analog of the PMF, of the input stream given a set of split points (values).\n"
+        "The resulting approximations have a probabilistic guarantee that can be obtained from the "
+        "get_normalized_rank_error(True) function.\n"
+        "If the sketch is empty this returns an empty vector.\n"
+        "split_points is an array of m unique, monotonically increasing float values "
+        "that divide the real number line into m+1 consecutive disjoint intervals.\n"
+        "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
+        "exclusive of the right split point, with the exception that the last interval will include "
+        "the maximum value.\n"
+        "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
+        "inclusive of the right split point.\n"
+        "It is not necessary to include either the min or max values in these split points."
+    )
+    .def("get_rank_lower_bound", &req_sketch<T, C>::get_rank_lower_bound, py::arg("rank"), py::arg("num_std_dev"),
+        "Returns an approximate lower bound on the given normalized rank.\n"
+        "Normalized rank must be a value between 0.0 and 1.0 (inclusive); "
+        "the number of standard deviations must be 1, 2, or 3.")
+    .def("get_rank_upper_bound", &req_sketch<T, C>::get_rank_upper_bound, py::arg("rank"), py::arg("num_std_dev"),
+        "Returns an approximate upper bound on the given normalized rank.\n"
+        "Normalized rank must be a value between 0.0 and 1.0 (inclusive); "
+        "the number of standard deviations must be 1, 2, or 3.")
+    .def_static("get_RSE", &req_sketch<T, C>::get_RSE,
+        py::arg("k"), py::arg("rank"), py::arg("is_hra"), py::arg("n"),
+        "Returns an a priori estimate of relative standard error (RSE, expressed as a number in [0,1]). "
+        "Derived from Lemma 12 in http://arxiv.org/abs/2004.01668v2, but the constant factors have been "
+        "modified based on empirical measurements, for a given value of parameter k.\n"
+        "Normalized rank must be a value between 0.0 and 1.0 (inclusive). If is_hra is True, uses high "
+        "rank accuracy mode, else low rank accuracy. N is an estimate of the total number of points "
+        "provided to the sketch.")
+    .def("__iter__", [](const req_sketch<T, C>& s) { return py::make_iterator(s.begin(), s.end()); });
+
+    add_serialization<T>(req_class);
+    add_vector_update<T>(req_class);
+}
+
+void init_req(py::module &m) {
+  bind_req_sketch<int, std::less<int>>(m, "req_ints_sketch");
+  bind_req_sketch<float, std::less<float>>(m, "req_floats_sketch");
+  bind_req_sketch<py::object, py_object_lt>(m, "req_items_sketch");
 }
```

### Comparing `datasketches-4.0.1/python/src/req_wrapper.cpp` & `datasketches-4.1.0/python/src/tuple_wrapper.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -13,203 +13,203 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-#include "req_sketch.hpp"
-
+#include <memory>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
-#include <pybind11/numpy.h>
-#include <sstream>
-#include <vector>
-#include <stdexcept>
-
-namespace py = pybind11;
-
-namespace datasketches {
-
-namespace python {
-
-template<typename T>
-req_sketch<T> req_sketch_deserialize(py::bytes sk_bytes) {
-  std::string sk_str = sk_bytes; // implicit cast  
-  return req_sketch<T>::deserialize(sk_str.c_str(), sk_str.length());
-}
-
-template<typename T>
-py::object req_sketch_serialize(const req_sketch<T>& sk) {
-  auto ser_result = sk.serialize();
-  return py::bytes((char*)ser_result.data(), ser_result.size());
-}
-
-// maybe possible to disambiguate the static vs method rank error calls, but
-// this is easier for now
-template<typename T>
-double req_sketch_generic_normalized_rank_error(uint16_t k, bool pmf) {
-  return req_sketch<T>::get_normalized_rank_error(k, pmf);
-}
-
-template<typename T>
-py::list req_sketch_get_quantiles(const req_sketch<T>& sk,
-                                  std::vector<double>& ranks,
-                                  bool inclusive) {
-  size_t n_quantiles = ranks.size();
-  auto result = sk.get_quantiles(ranks.data(), n_quantiles, inclusive);
-  // returning as std::vector<> would copy values to a list anyway
-  py::list list(n_quantiles);
-  for (size_t i = 0; i < n_quantiles; ++i) {
-      list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-py::list req_sketch_get_pmf(const req_sketch<T>& sk,
-                            std::vector<T>& split_points,
-                            bool inclusive) {
-  size_t n_points = split_points.size();
-  auto result = sk.get_PMF(split_points.data(), n_points, inclusive);
-  py::list list(n_points + 1);
-  for (size_t i = 0; i <= n_points; ++i) {
-    list[i] = result[i];
-  }
-  return list;
-}
 
-template<typename T>
-py::list req_sketch_get_cdf(const req_sketch<T>& sk,
-                            std::vector<T>& split_points,
-                            bool inclusive) {
-  size_t n_points = split_points.size();
-  auto result = sk.get_CDF(split_points.data(), n_points, inclusive);
-  py::list list(n_points + 1);
-  for (size_t i = 0; i <= n_points; ++i) {
-    list[i] = result[i];
-  }
-  return list;
-}
-
-template<typename T>
-void req_sketch_update(req_sketch<T>& sk, py::array_t<T, py::array::c_style | py::array::forcecast> items) {
-  if (items.ndim() != 1) {
-    throw std::invalid_argument("input data must have only one dimension. Found: "
-          + std::to_string(items.ndim()));
-  }
-  
-  auto data = items.template unchecked<1>();
-  for (uint32_t i = 0; i < data.size(); ++i) {
-    sk.update(data(i));
-  }
-}
+#include "theta_sketch.hpp"
+#include "tuple_sketch.hpp"
+#include "tuple_union.hpp"
+#include "tuple_intersection.hpp"
+#include "tuple_a_not_b.hpp"
+#include "theta_jaccard_similarity_base.hpp"
+#include "common_defs.hpp"
 
-}
-}
+#include "py_serde.hpp"
+#include "tuple_policy.hpp"
 
-namespace dspy = datasketches::python;
+namespace py = pybind11;
 
-template<typename T>
-void bind_req_sketch(py::module &m, const char* name) {
+void init_tuple(py::module &m) {
   using namespace datasketches;
 
-  py::class_<req_sketch<T>>(m, name)
-    .def(py::init<uint16_t, bool>(), py::arg("k")=12, py::arg("is_hra")=true)
-    .def(py::init<const req_sketch<T>&>())
-    .def("update", (void (req_sketch<T>::*)(const T&)) &req_sketch<T>::update, py::arg("item"),
-         "Updates the sketch with the given value")
-    .def("update", &dspy::req_sketch_update<T>, py::arg("array"),
-         "Updates the sketch with the values in the given array")
-    .def("merge", (void (req_sketch<T>::*)(const req_sketch<T>&)) &req_sketch<T>::merge, py::arg("sketch"),
-         "Merges the provided sketch into the this one")
-    .def("__str__", &req_sketch<T>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
+  // generic tuple_policy:
+  // * update sketch policy uses create_summary and update_summary
+  // * set operation policies all use __call__
+  py::class_<tuple_policy, TuplePolicy, std::shared_ptr<tuple_policy>>(m, "TuplePolicy")
+    .def(py::init())
+    .def("create_summary", &tuple_policy::create_summary)
+    .def("update_summary", &tuple_policy::update_summary, py::arg("summary"), py::arg("update"))
+    .def("__call__", &tuple_policy::operator(), py::arg("summary"), py::arg("update"))
+  ;
+
+  // potentially useful for debugging but not needed as a permanent
+  // object type in the library
+  /*
+  py::class_<tuple_policy_holder>(m, "TuplePolicyHolder")
+    .def(py::init<std::shared_ptr<tuple_policy>>(), py::arg("policy"))
+    .def("create", &tuple_policy_holder::create, "Creates a new Summary object")
+    .def("update", &tuple_policy_holder::update, py::arg("summary"), py::arg("update"),
+         "Updates the provided summary using the data in update")
+  ;
+  */
+
+  using py_tuple_sketch = tuple_sketch<py::object>;
+  using py_update_tuple = update_tuple_sketch<py::object, py::object, tuple_policy_holder>;
+  using py_compact_tuple = compact_tuple_sketch<py::object>;
+  using py_tuple_union = tuple_union<py::object, tuple_policy_holder>;
+  using py_tuple_intersection = tuple_intersection<py::object, tuple_policy_holder>;
+  using py_tuple_a_not_b = tuple_a_not_b<py::object>;
+  using py_tuple_jaccard_similarity = jaccard_similarity_base<tuple_union<py::object, dummy_jaccard_policy>, tuple_intersection<py::object, dummy_jaccard_policy>, pair_extract_key<uint64_t, py::object>>;
+
+  py::class_<py_tuple_sketch>(m, "_tuple_sketch")
+    .def("__str__", &py_tuple_sketch::to_string, py::arg("print_items")=false,
          "Produces a string summary of the sketch")
-    .def("to_string", &req_sketch<T>::to_string, py::arg("print_levels")=false, py::arg("print_items")=false,
+    .def("to_string", &py_tuple_sketch::to_string, py::arg("print_items")=false,
          "Produces a string summary of the sketch")
-    .def("is_hra", &req_sketch<T>::is_HRA,
-         "Returns True if the sketch is in High Rank Accuracy mode, otherwise False")
-    .def("is_empty", &req_sketch<T>::is_empty,
+    .def("is_empty", &py_tuple_sketch::is_empty,
          "Returns True if the sketch is empty, otherwise False")
-    .def("get_k", &req_sketch<T>::get_k,
-         "Returns the configured parameter k")
-    .def("get_n", &req_sketch<T>::get_n,
-         "Returns the length of the input stream")
-    .def("get_num_retained", &req_sketch<T>::get_num_retained,
-         "Returns the number of retained items (samples) in the sketch")
-    .def("is_estimation_mode", &req_sketch<T>::is_estimation_mode,
-         "Returns True if the sketch is in estimation mode, otherwise False")
-    .def("get_min_value", &req_sketch<T>::get_min_item,
-         "Returns the minimum value from the stream. If empty, req_floats_sketch returns nan; req_ints_sketch throws a RuntimeError")
-    .def("get_max_value", &req_sketch<T>::get_max_item,
-         "Returns the maximum value from the stream. If empty, req_floats_sketch returns nan; req_ints_sketch throws a RuntimeError")
-    .def("get_quantile", &req_sketch<T>::get_quantile, py::arg("rank"), py::arg("inclusive")=false,
-         "Returns an approximation to the data value "
-         "associated with the given normalized rank in a hypothetical sorted "
-         "version of the input stream so far.\n"
-         "For req_floats_sketch: if the sketch is empty this returns nan. "
-         "For req_ints_sketch: if the sketch is empty this throws a RuntimeError.")
-    .def("get_quantiles", &dspy::req_sketch_get_quantiles<T>, py::arg("ranks"), py::arg("inclusive")=false,
-         "This returns an array that could have been generated by using get_quantile() for each "
-         "normalized rank separately.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "Deprecated. Will be removed in the next major version. Use get_quantile() instead.")
-    .def("get_rank", &req_sketch<T>::get_rank, py::arg("value"), py::arg("inclusive")=false,
-         "Returns an approximation to the normalized rank of the given value from 0 to 1, inclusive.\n"
-         "The resulting approximation has a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(False) function.\n"
-         "With the parameter inclusive=true the weight of the given value is included into the rank."
-         "Otherwise the rank equals the sum of the weights of values less than the given value.\n"
-         "If the sketch is empty this returns nan.")
-    .def("get_pmf", &dspy::req_sketch_get_pmf<T>, py::arg("split_points"), py::arg("inclusive")=false,
-         "Returns an approximation to the Probability Mass Function (PMF) of the input stream "
-         "given a set of split points (values).\n"
-         "The resulting approximations have a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(True) function.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "split_points is an array of m unique, monotonically increasing float values "
-         "that divide the real number line into m+1 consecutive disjoint intervals.\n"
-         "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
-         "exclusive of the right split point, with the exception that the last interval will include "
-         "the maximum value.\n"
-         "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
-         "inclusive of the right split point.\n"
-         "It is not necessary to include either the min or max values in these split points.")
-    .def("get_cdf", &dspy::req_sketch_get_cdf<T>, py::arg("split_points"), py::arg("inclusive")=false,
-         "Returns an approximation to the Cumulative Distribution Function (CDF), which is the "
-         "cumulative analog of the PMF, of the input stream given a set of split points (values).\n"
-         "The resulting approximations have a probabilistic guarantee that can be obtained from the "
-         "get_normalized_rank_error(True) function.\n"
-         "If the sketch is empty this returns an empty vector.\n"
-         "split_points is an array of m unique, monotonically increasing float values "
-         "that divide the real number line into m+1 consecutive disjoint intervals.\n"
-         "If the parameter inclusive=false, the definition of an 'interval' is inclusive of the left split point (or minimum value) and "
-         "exclusive of the right split point, with the exception that the last interval will include "
-         "the maximum value.\n"
-         "If the parameter inclusive=true, the definition of an 'interval' is exclusive of the left split point (or minimum value) and "
-         "inclusive of the right split point.\n"
-         "It is not necessary to include either the min or max values in these split points.")
-    .def("get_rank_lower_bound", &req_sketch<T>::get_rank_lower_bound, py::arg("rank"), py::arg("num_std_dev"),
-         "Returns an approximate lower bound on the given normalized rank.\n"
-         "Normalized rank must be a value between 0.0 and 1.0 (inclusive); "
-         "the number of standard deviations must be 1, 2, or 3.")
-    .def("get_rank_upper_bound", &req_sketch<T>::get_rank_upper_bound, py::arg("rank"), py::arg("num_std_dev"),
-         "Returns an approximate upper bound on the given normalized rank.\n"
-         "Normalized rank must be a value between 0.0 and 1.0 (inclusive); "
-         "the number of standard deviations must be 1, 2, or 3.")
-    .def_static("get_RSE", &req_sketch<T>::get_RSE,
-         py::arg("k"), py::arg("rank"), py::arg("is_hra"), py::arg("n"),
-         "Returns an a priori estimate of relative standard error (RSE, expressed as a number in [0,1]). "
-         "Derived from Lemma 12 in http://arxiv.org/abs/2004.01668v2, but the constant factors have been "
-         "modified based on empirical measurements, for a given value of parameter k.\n"
-         "Normalized rank must be a value between 0.0 and 1.0 (inclusive). If is_hra is True, uses high "
-         "rank accuracy mode, else low rank accuracy. N is an estimate of the total number of points "
-         "provided to the sketch.")
-    .def("serialize", &dspy::req_sketch_serialize<T>, "Serializes the sketch into a bytes object")
-    .def_static("deserialize", &dspy::req_sketch_deserialize<T>, "Deserializes the sketch from a bytes object")
-    ;
-}
-
-void init_req(py::module &m) {
-  bind_req_sketch<int>(m, "req_ints_sketch");
-  bind_req_sketch<float>(m, "req_floats_sketch");
+    .def("get_estimate", &py_tuple_sketch::get_estimate,
+         "Estimate of the distinct count of the input stream")
+    .def("get_upper_bound", static_cast<double (py_tuple_sketch::*)(uint8_t) const>(&py_tuple_sketch::get_upper_bound), py::arg("num_std_devs"),
+         "Returns an approximate upper bound on the estimate at standard deviations in {1, 2, 3}")
+    .def("get_lower_bound", static_cast<double (py_tuple_sketch::*)(uint8_t) const>(&py_tuple_sketch::get_lower_bound), py::arg("num_std_devs"),
+         "Returns an approximate lower bound on the estimate at standard deviations in {1, 2, 3}")
+    .def("is_estimation_mode", &py_tuple_sketch::is_estimation_mode,
+         "Returns True if sketch is in estimation mode, otherwise False")
+    .def("get_theta", &py_tuple_sketch::get_theta,
+         "Returns theta (effective sampling rate) as a fraction from 0 to 1")
+    .def("get_theta64", &py_tuple_sketch::get_theta64,
+         "Returns theta as 64-bit value")
+    .def("get_num_retained", &py_tuple_sketch::get_num_retained,
+         "Returns the number of items currently in the sketch")
+    .def("get_seed_hash", [](const py_tuple_sketch& sk) { return sk.get_seed_hash(); }, // why does regular call not work??
+         "Returns a hash of the seed used in the sketch")
+    .def("is_ordered", &py_tuple_sketch::is_ordered,
+         "Returns True if the sketch entries are sorted, otherwise False")
+    .def("__iter__", [](const py_tuple_sketch& s) { return py::make_iterator(s.begin(), s.end()); })
+    .def_property_readonly_static("DEFAULT_SEED", [](py::object /* self */) { return DEFAULT_SEED; });
+  ;
+
+  py::class_<py_compact_tuple, py_tuple_sketch>(m, "_compact_tuple_sketch")
+    .def(py::init<const py_compact_tuple&>(), py::arg("other"))
+    .def(py::init<const py_tuple_sketch&, bool>(), py::arg("other"), py::arg("ordered")=true)
+    .def(py::init<const theta_sketch&, py::object&>(), py::arg("other"), py::arg("summary"),
+         "Creates a compact tuple sketch from a theta sketch using a fixed summary value.")
+    .def(
+        "serialize",
+        [](const py_compact_tuple& sk, py_object_serde& serde) {
+          auto bytes = sk.serialize(0, serde);
+          return py::bytes(reinterpret_cast<const char*>(bytes.data()), bytes.size());
+        }, py::arg("serde"),
+        "Serializes the sketch into a bytes object"
+    )
+    .def_static(
+        "deserialize",
+        [](const std::string& bytes, py_object_serde& serde, uint64_t seed) {
+          return py_compact_tuple::deserialize(bytes.data(), bytes.size(), seed, serde);
+        },
+        py::arg("bytes"), py::arg("serde"), py::arg("seed")=DEFAULT_SEED,
+        "Reads a bytes object and returns the corresponding compact_tuple_sketch"
+    );
+
+  py::class_<py_update_tuple, py_tuple_sketch>(m, "_update_tuple_sketch")
+    .def(
+        py::init([](std::shared_ptr<tuple_policy> policy, uint8_t lg_k, double p, uint64_t seed) {
+          tuple_policy_holder holder(policy);
+          return py_update_tuple::builder(holder).set_lg_k(lg_k).set_p(p).set_seed(seed).build();
+        }),
+        py::arg("policy"), py::arg("lg_k")=theta_constants::DEFAULT_LG_K, py::arg("p")=1.0, py::arg("seed")=DEFAULT_SEED
+    )
+    .def(py::init<const py_update_tuple&>())
+    .def("update", static_cast<void (py_update_tuple::*)(int64_t, py::object&)>(&py_update_tuple::update),
+         py::arg("datum"), py::arg("value"),
+         "Updates the sketch with the given integral item and summary value")
+    .def("update", static_cast<void (py_update_tuple::*)(double, py::object&)>(&py_update_tuple::update),
+         py::arg("datum"), py::arg("value"),
+         "Updates the sketch with the given floating point item and summary value")
+    .def("update", static_cast<void (py_update_tuple::*)(const std::string&, py::object&)>(&py_update_tuple::update),
+         py::arg("datum"), py::arg("value"),
+         "Updates the sketch with the given string item and summary value")
+    .def("compact", &py_update_tuple::compact, py::arg("ordered")=true,
+         "Returns a compacted form of the sketch, optionally sorting it")
+    .def("reset", &py_update_tuple::reset, "Resets the sketch to the initial empty state")
+  ;
+
+  py::class_<py_tuple_union>(m, "_tuple_union")
+    .def(
+        py::init([](std::shared_ptr<tuple_policy> policy, uint8_t lg_k, double p, uint64_t seed) {
+          tuple_policy_holder holder(policy);
+          return py_tuple_union::builder(holder).set_lg_k(lg_k).set_p(p).set_seed(seed).build();
+        }),
+        py::arg("policy"), py::arg("lg_k")=theta_constants::DEFAULT_LG_K, py::arg("p")=1.0, py::arg("seed")=DEFAULT_SEED
+    )
+    .def("update", &py_tuple_union::update<const py_tuple_sketch&>, py::arg("sketch"),
+         "Updates the union with the given sketch")
+    .def("get_result", &py_tuple_union::get_result, py::arg("ordered")=true,
+         "Returns the sketch corresponding to the union result")
+    .def("reset", &py_tuple_union::reset,
+         "Resets the sketch to the initial empty")
+  ;
+
+  py::class_<py_tuple_intersection>(m, "_tuple_intersection")
+    .def(
+        py::init([](std::shared_ptr<tuple_policy> policy, uint64_t seed) {
+          tuple_policy_holder holder(policy);
+          return py_tuple_intersection(seed, holder);
+        }),
+        py::arg("policy"), py::arg("seed")=DEFAULT_SEED)
+    .def("update", &py_tuple_intersection::update<const py_tuple_sketch&>, py::arg("sketch"),
+         "Intersects the provided sketch with the current intersection state")
+    .def("get_result", &py_tuple_intersection::get_result, py::arg("ordered")=true,
+         "Returns the sketch corresponding to the intersection result")
+    .def("has_result", &py_tuple_intersection::has_result,
+         "Returns True if the intersection has a valid result, otherwise False")
+  ;
+
+  py::class_<py_tuple_a_not_b>(m, "_tuple_a_not_b")
+    .def(py::init<uint64_t>(), py::arg("seed")=DEFAULT_SEED)
+    .def(
+        "compute",
+        &py_tuple_a_not_b::compute<const py_tuple_sketch&, const py_tuple_sketch&>,
+        py::arg("a"), py::arg("b"), py::arg("ordered")=true,
+        "Returns a sketch with the result of applying the A-not-B operation on the given inputs"
+    )
+  ;
+
+  py::class_<py_tuple_jaccard_similarity>(m, "_tuple_jaccard_similarity")
+    .def_static(
+        "jaccard",
+        [](const py_tuple_sketch& sketch_a, const py_tuple_sketch& sketch_b, uint64_t seed) {
+          return py_tuple_jaccard_similarity::jaccard(sketch_a, sketch_b, seed);
+        },
+        py::arg("sketch_a"), py::arg("sketch_b"), py::arg("seed")=DEFAULT_SEED,
+        "Returns a list with {lower_bound, estimate, upper_bound} of the Jaccard similarity between sketches"
+    )
+    .def_static(
+        "exactly_equal",
+        &py_tuple_jaccard_similarity::exactly_equal<const py_tuple_sketch&, const py_tuple_sketch&>,
+        py::arg("sketch_a"), py::arg("sketch_b"), py::arg("seed")=DEFAULT_SEED,
+        "Returns True if sketch_a and sketch_b are equivalent, otherwise False"
+    )
+    .def_static(
+        "similarity_test",
+        &py_tuple_jaccard_similarity::similarity_test<const py_tuple_sketch&, const py_tuple_sketch&>,
+        py::arg("actual"), py::arg("expected"), py::arg("threshold"), py::arg("seed")=DEFAULT_SEED,
+        "Tests similarity of an actual sketch against an expected sketch. Computes the lower bound of the Jaccard "
+        "index J_{LB} of the actual and expected sketches. If J_{LB} >= threshold, then the sketches are considered "
+        "to be similar with a confidence of 97.7% and returns True, otherwise False.")
+    .def_static(
+        "dissimilarity_test",
+        &py_tuple_jaccard_similarity::dissimilarity_test<const py_tuple_sketch&, const py_tuple_sketch&>,
+        py::arg("actual"), py::arg("expected"), py::arg("threshold"), py::arg("seed")=DEFAULT_SEED,
+        "Tests dissimilarity of an actual sketch against an expected sketch. Computes the upper bound of the Jaccard "
+        "index J_{UB} of the actual and expected sketches. If J_{UB} <= threshold, then the sketches are considered "
+        "to be dissimilar with a confidence of 97.7% and returns True, otherwise False."
+    )
+  ;
 }
```

### Comparing `datasketches-4.0.1/python/src/theta_wrapper.cpp` & `datasketches-4.1.0/python/src/theta_wrapper.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -13,70 +13,26 @@
  * software distributed under the License is distributed on an
  * "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  * KIND, either express or implied.  See the License for the
  * specific language governing permissions and limitations
  * under the License.
  */
 
-#include <sstream>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
 #include "theta_sketch.hpp"
 #include "theta_union.hpp"
 #include "theta_intersection.hpp"
 #include "theta_a_not_b.hpp"
 #include "theta_jaccard_similarity.hpp"
 #include "common_defs.hpp"
 
-
 namespace py = pybind11;
 
-namespace datasketches {
-namespace python {
-
-update_theta_sketch update_theta_sketch_factory(uint8_t lg_k, double p, uint64_t seed) {
-  update_theta_sketch::builder builder;
-  builder.set_lg_k(lg_k);
-  builder.set_p(p);
-  builder.set_seed(seed);
-  return builder.build();
-}
-
-theta_union theta_union_factory(uint8_t lg_k, double p, uint64_t seed) {
-  theta_union::builder builder;
-  builder.set_lg_k(lg_k);
-  builder.set_p(p);
-  builder.set_seed(seed);
-  return builder.build();
-}
-
-uint16_t theta_sketch_get_seed_hash(const theta_sketch& sk) {
-  return sk.get_seed_hash();
-}
-
-py::object compact_theta_sketch_serialize(const compact_theta_sketch& sk) {
-  auto serResult = sk.serialize();
-  return py::bytes((char*)serResult.data(), serResult.size());
-}
-
-compact_theta_sketch compact_theta_sketch_deserialize(py::bytes skBytes, uint64_t seed) {
-  std::string skStr = skBytes; // implicit cast  
-  return compact_theta_sketch::deserialize(skStr.c_str(), skStr.length(), seed);
-}
-
-py::list theta_jaccard_sim_computation(const theta_sketch& sketch_a, const theta_sketch& sketch_b, uint64_t seed) {
-  return py::cast(theta_jaccard_similarity::jaccard(sketch_a, sketch_b, seed));
-}
-
-}
-}
-
-namespace dspy = datasketches::python;
-
 void init_theta(py::module &m) {
   using namespace datasketches;
 
   py::class_<theta_sketch>(m, "theta_sketch")
     .def("__str__", &theta_sketch::to_string, py::arg("print_items")=false,
          "Produces a string summary of the sketch")
     .def("to_string", &theta_sketch::to_string, py::arg("print_items")=false,
@@ -89,49 +45,70 @@
          "Returns an approximate upper bound on the estimate at standard deviations in {1, 2, 3}")
     .def("get_lower_bound", &theta_sketch::get_lower_bound, py::arg("num_std_devs"),
          "Returns an approximate lower bound on the estimate at standard deviations in {1, 2, 3}")
     .def("is_estimation_mode", &theta_sketch::is_estimation_mode,
          "Returns True if sketch is in estimation mode, otherwise False")
     .def("get_theta", &theta_sketch::get_theta,
          "Returns theta (effective sampling rate) as a fraction from 0 to 1")
+    .def("get_theta64", &theta_sketch::get_theta64,
+         "Returns theta as 64-bit value")
     .def("get_num_retained", &theta_sketch::get_num_retained,
-         "Retunrs the number of items currently in the sketch")
-    .def("get_seed_hash", &dspy::theta_sketch_get_seed_hash,
+         "Returns the number of items currently in the sketch")
+    .def("get_seed_hash", &theta_sketch::get_seed_hash,
          "Returns a hash of the seed used in the sketch")
     .def("is_ordered", &theta_sketch::is_ordered,
          "Returns True if the sketch entries are sorted, otherwise False")
+    .def("__iter__", [](const theta_sketch& s) { return py::make_iterator(s.begin(), s.end()); })
   ;
 
   py::class_<update_theta_sketch, theta_sketch>(m, "update_theta_sketch")
-    .def(py::init(&dspy::update_theta_sketch_factory),
-         py::arg("lg_k")=theta_constants::DEFAULT_LG_K, py::arg("p")=1.0, py::arg("seed")=DEFAULT_SEED)
+    .def(
+        py::init([](uint8_t lg_k, double p, uint64_t seed) {
+          return update_theta_sketch::builder().set_lg_k(lg_k).set_p(p).set_seed(seed).build();
+        }),
+        py::arg("lg_k")=theta_constants::DEFAULT_LG_K, py::arg("p")=1.0, py::arg("seed")=DEFAULT_SEED
+    )
     .def(py::init<const update_theta_sketch&>())
     .def("update", (void (update_theta_sketch::*)(int64_t)) &update_theta_sketch::update, py::arg("datum"),
          "Updates the sketch with the given integral value")
     .def("update", (void (update_theta_sketch::*)(double)) &update_theta_sketch::update, py::arg("datum"),
          "Updates the sketch with the given floating point value")
     .def("update", (void (update_theta_sketch::*)(const std::string&)) &update_theta_sketch::update, py::arg("datum"),
          "Updates the sketch with the given string")
     .def("compact", &update_theta_sketch::compact, py::arg("ordered")=true,
          "Returns a compacted form of the sketch, optionally sorting it")
   ;
 
   py::class_<compact_theta_sketch, theta_sketch>(m, "compact_theta_sketch")
     .def(py::init<const compact_theta_sketch&>())
     .def(py::init<const theta_sketch&, bool>())
-    .def("serialize", &dspy::compact_theta_sketch_serialize,
-        "Serializes the sketch into a bytes object")
-    .def_static("deserialize", &dspy::compact_theta_sketch_deserialize,
+    .def(
+        "serialize",
+        [](const compact_theta_sketch& sk) {
+          auto bytes = sk.serialize();
+          return py::bytes(reinterpret_cast<const char*>(bytes.data()), bytes.size());
+        },
+        "Serializes the sketch into a bytes object"
+    )
+    .def_static(
+        "deserialize",
+        [](const std::string& bytes, uint64_t seed) {
+          return compact_theta_sketch::deserialize(bytes.data(), bytes.size(), seed);
+        },
         py::arg("bytes"), py::arg("seed")=DEFAULT_SEED,
-        "Reads a bytes object and returns the corresponding compact_theta_sketch")        
-  ;
+        "Reads a bytes object and returns the corresponding compact_theta_sketch"
+    );
 
   py::class_<theta_union>(m, "theta_union")
-    .def(py::init(&dspy::theta_union_factory),
-         py::arg("lg_k")=theta_constants::DEFAULT_LG_K, py::arg("p")=1.0, py::arg("seed")=DEFAULT_SEED)
+    .def(
+        py::init([](uint8_t lg_k, double p, uint64_t seed) {
+          return theta_union::builder().set_lg_k(lg_k).set_p(p).set_seed(seed).build();
+        }),
+        py::arg("lg_k")=theta_constants::DEFAULT_LG_K, py::arg("p")=1.0, py::arg("seed")=DEFAULT_SEED
+    )
     .def("update", &theta_union::update<const theta_sketch&>, py::arg("sketch"),
          "Updates the union with the given sketch")
     .def("get_result", &theta_union::get_result, py::arg("ordered")=true,
          "Returns the sketch corresponding to the union result")
   ;
 
   py::class_<theta_intersection>(m, "theta_intersection")
@@ -143,30 +120,47 @@
          "Returns the sketch corresponding to the intersection result")
     .def("has_result", &theta_intersection::has_result,
          "Returns True if the intersection has a valid result, otherwise False")
   ;
 
   py::class_<theta_a_not_b>(m, "theta_a_not_b")
     .def(py::init<uint64_t>(), py::arg("seed")=DEFAULT_SEED)
-    .def("compute", &theta_a_not_b::compute<const theta_sketch&, const theta_sketch&>, py::arg("a"), py::arg("b"), py::arg("ordered")=true,
-         "Returns a sketch with the reuslt of appying the A-not-B operation on the given inputs")
+    .def(
+        "compute",
+        &theta_a_not_b::compute<const theta_sketch&, const theta_sketch&>,
+        py::arg("a"), py::arg("b"), py::arg("ordered")=true,
+        "Returns a sketch with the result of applying the A-not-B operation on the given inputs"
+    )
   ;
   
   py::class_<theta_jaccard_similarity>(m, "theta_jaccard_similarity")
-     .def_static("jaccard", &dspy::theta_jaccard_sim_computation,
-                 py::arg("sketch_a"), py::arg("sketch_b"), py::arg("seed")=DEFAULT_SEED,
-                 "Returns a list with {lower_bound, estimate, upper_bound} of the Jaccard similarity between sketches")
-     .def_static("exactly_equal", &theta_jaccard_similarity::exactly_equal<const theta_sketch&, const theta_sketch&>,
-                 py::arg("sketch_a"), py::arg("sketch_b"), py::arg("seed")=DEFAULT_SEED,
-                 "Returns True if sketch_a and sketch_b are equivalent, otherwise False")
-     .def_static("similarity_test", &theta_jaccard_similarity::similarity_test<const theta_sketch&, const theta_sketch&>,
-                 py::arg("actual"), py::arg("expected"), py::arg("threshold"), py::arg("seed")=DEFAULT_SEED,
-                 "Tests similarity of an actual sketch against an expected sketch. Computers the lower bound of the Jaccard "
-                 "index J_{LB} of the actual and expected sketches. If J_{LB} >= threshold, then the sketches are considered "
-                 "to be similar sith a confidence of 97.7% and returns True, otherwise False.")
-     .def_static("dissimilarity_test", &theta_jaccard_similarity::dissimilarity_test<const theta_sketch&, const theta_sketch&>,
-                 py::arg("actual"), py::arg("expected"), py::arg("threshold"), py::arg("seed")=DEFAULT_SEED,
-                 "Tests dissimilarity of an actual sketch against an expected sketch. Computers the lower bound of the Jaccard "
-                 "index J_{UB} of the actual and expected sketches. If J_{UB} <= threshold, then the sketches are considered "
-                 "to be dissimilar sith a confidence of 97.7% and returns True, otherwise False.")            
+    .def_static(
+        "jaccard",
+        [](const theta_sketch& sketch_a, const theta_sketch& sketch_b, uint64_t seed) {
+          return theta_jaccard_similarity::jaccard(sketch_a, sketch_b, seed);
+        },
+        py::arg("sketch_a"), py::arg("sketch_b"), py::arg("seed")=DEFAULT_SEED,
+        "Returns a list with {lower_bound, estimate, upper_bound} of the Jaccard similarity between sketches"
+    )
+    .def_static(
+        "exactly_equal",
+        &theta_jaccard_similarity::exactly_equal<const theta_sketch&, const theta_sketch&>,
+        py::arg("sketch_a"), py::arg("sketch_b"), py::arg("seed")=DEFAULT_SEED,
+        "Returns True if sketch_a and sketch_b are equivalent, otherwise False"
+    )
+    .def_static(
+        "similarity_test",
+        &theta_jaccard_similarity::similarity_test<const theta_sketch&, const theta_sketch&>,
+        py::arg("actual"), py::arg("expected"), py::arg("threshold"), py::arg("seed")=DEFAULT_SEED,
+        "Tests similarity of an actual sketch against an expected sketch. Computers the lower bound of the Jaccard "
+        "index J_{LB} of the actual and expected sketches. If J_{LB} >= threshold, then the sketches are considered "
+        "to be similar with a confidence of 97.7% and returns True, otherwise False.")
+    .def_static(
+        "dissimilarity_test",
+        &theta_jaccard_similarity::dissimilarity_test<const theta_sketch&, const theta_sketch&>,
+        py::arg("actual"), py::arg("expected"), py::arg("threshold"), py::arg("seed")=DEFAULT_SEED,
+        "Tests dissimilarity of an actual sketch against an expected sketch. Computers the lower bound of the Jaccard "
+        "index J_{UB} of the actual and expected sketches. If J_{UB} <= threshold, then the sketches are considered "
+        "to be dissimilar with a confidence of 97.7% and returns True, otherwise False."
+    )
   ;     
 }
```

### Comparing `datasketches-4.0.1/python/src/vector_of_kll.cpp` & `datasketches-4.1.0/python/src/vector_of_kll.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/src/vo_wrapper.cpp` & `datasketches-4.1.0/python/src/vo_wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
          "Applies a provided predicate to the sketch and returns the estimated total weight matching the predicate, as well "
          "as upper and lower bounds on the estimate and the total weight processed by the sketch")
     .def("get_serialized_size_bytes", &dspy::vo_sketch_size_bytes<T>, py::arg("serde"),
         "Computes the size in bytes needed to serialize the current sketch")
     .def("serialize", &dspy::vo_sketch_serialize<T>, py::arg("serde"), "Serialize the var opt sketch using the provided serde")
     .def_static("deserialize", &dspy::vo_sketch_deserialize<T>, py::arg("bytes"), py::arg("serde"),
         "Constructs a var opt sketch from the given bytes using the provided serde")
-    ;
+    .def("__iter__", [](const var_opt_sketch<T>& sk) { return py::make_iterator(sk.begin(), sk.end()); });
 }
 
 template<typename T>
 void bind_vo_union(py::module &m, const char* name) {
   using namespace datasketches;
 
   py::class_<var_opt_union<T>>(m, name)
```

### Comparing `datasketches-4.0.1/python/tests/__init__.py` & `datasketches-4.1.0/density/test/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -10,7 +10,26 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+
+add_executable(density_test)
+
+target_link_libraries(density_test density common_test_lib)
+
+set_target_properties(density_test PROPERTIES
+  CXX_STANDARD 11
+  CXX_STANDARD_REQUIRED YES
+)
+
+add_test(
+  NAME density_test
+  COMMAND density_test
+)
+
+target_sources(density_test
+  PRIVATE
+    density_sketch_test.cpp
+)
```

### Comparing `datasketches-4.0.1/python/tests/cpc_test.py` & `datasketches-4.1.0/python/tests/cpc_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,55 +10,55 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-  
+
 import unittest
 from datasketches import cpc_sketch, cpc_union
 
 class CpcTest(unittest.TestCase):
   def test_cpc_example(self):
-    k = 12      # 2^k = 4096 rows in the table
-    n = 1 << 18 # ~256k unique values
+    lgk = 12    # 2^k = 4096 rows in the table
+    n = 1 << 18 # ~256k distinct values
 
     # create a couple sketches and inject some values
     # we'll have 1/4 of the values overlap
-    cpc  = cpc_sketch(k)
-    cpc2 = cpc_sketch(k)
+    cpc  = cpc_sketch(lgk)
+    cpc2 = cpc_sketch(lgk)
     offset = int(3 * n / 4) # it's a float w/o cast
     # because we hash on the bits, not an abstract numeric value,
     # cpc.update(1) and cpc.update(1.0) give different results.
     for i in range(0, n):
         cpc.update(i)
         cpc2.update(i + offset)
-        
+
     # although we provide get_composite_estimate() and get_estimate(),
     # the latter will always give the best available estimate.  we
     # recommend using get_estimate().
     # we can check that the upper and lower bounds bracket the
     # estimate, without needing to know the exact value.
     self.assertLessEqual(cpc.get_lower_bound(1), cpc.get_estimate())
     self.assertGreaterEqual(cpc.get_upper_bound(1), cpc.get_estimate())
 
-    # unioning uses a separate class, but we need to get_result()
-    # tp query the unioned sketches
-    union = cpc_union(k)
+    # union is a separate class, so we need to get_result()
+    # to query the unioned sketches
+    union = cpc_union(lgk)
     union.update(cpc)
     union.update(cpc2)
     result = union.get_result()
 
     # since our process here (including post-union CPC) is
     # deterministic, we have checked and know the exact
     # answer is within one standard deviation of the estimate
     self.assertLessEqual(result.get_lower_bound(1), 7 * n / 4)
     self.assertGreaterEqual(result.get_upper_bound(1), 7 * n / 4)
-     
+
     # serialize for storage and reconstruct
     sk_bytes = result.serialize()
     new_cpc = cpc_sketch.deserialize(sk_bytes)
     self.assertFalse(new_cpc.is_empty())
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `datasketches-4.0.1/python/tests/fi_test.py` & `datasketches-4.1.0/python/tests/fi_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
  
 import unittest
-from datasketches import frequent_strings_sketch, frequent_items_error_type
+from datasketches import frequent_strings_sketch, frequent_items_sketch
+from datasketches import frequent_items_error_type, PyIntsSerDe
 
 class FiTest(unittest.TestCase):
-  def test_fi_example(self):
+  def test_fi_strings_example(self):
     k = 3  # a small value so we can easily fill the sketch
     fi = frequent_strings_sketch(k)
 
     # we'll use a small number of distinct items so we
     # can use exponentially increasing weights and have
     # some frequent items, decreasing so we have some
     # small items inserted after a purge
@@ -89,14 +90,52 @@
     new_fi = frequent_strings_sketch.deserialize(fi_bytes)
 
     # and now interrogate the sketch
     self.assertFalse(new_fi.is_empty())
     self.assertGreater(new_fi.get_num_active_items(), 0)
     self.assertEqual(5 * wt, new_fi.get_total_weight())
 
+  # This example uses generic objects but is otherwise identical
+  def test_fi_items_example(self):
+    k = 3  # a small value so we can easily fill the sketch
+    fi = frequent_items_sketch(k)
+
+    # as above, but in this case inserting ints
+    n = 8
+    for i in range(0, n):
+      fi.update(i, 2 ** (n - i))
+
+    # everything else works identically, so let's jump straight
+    # to merging and serialization
+
+    # now create a second sketch with a lot of unique
+    # values but all with equal weight (of 1) such that
+    # the total weight is much larger than the first sketch
+    fi2 = frequent_items_sketch(k)
+    wt = fi.get_total_weight()
+    for i in range(0, 4*wt):
+      fi2.update(i)
+
+    # merge the second sketch into the first
+    fi.merge(fi2)
+
+    # we can see that the weight is much larger
+    self.assertEqual(5 * wt, fi.get_total_weight())
+
+    # finally, serialize and reconstruct -- now we need a serde to tell
+    # (de)serialization how to interpret the objects
+    fi_bytes = fi.serialize(PyIntsSerDe())
+    self.assertEqual(len(fi_bytes), fi.get_serialized_size_bytes(PyIntsSerDe()))
+    new_fi = frequent_items_sketch.deserialize(fi_bytes, PyIntsSerDe())
+
+    # and again interrogate the sketch to check that it's what we serialized
+    self.assertFalse(new_fi.is_empty())
+    self.assertGreater(new_fi.get_num_active_items(), 0)
+    self.assertEqual(5 * wt, new_fi.get_total_weight())
+
 
   def test_fi_sketch(self):
     # only testing a few things not used in the above example
     k = 12
     wt = 10000
     fi = frequent_strings_sketch(k)
```

### Comparing `datasketches-4.0.1/python/tests/hll_test.py` & `datasketches-4.1.0/python/tests/hll_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
- 
+
 import unittest
 from datasketches import hll_sketch, hll_union, tgt_hll_type
 
 class HllTest(unittest.TestCase):
     def test_hll_example(self):
-        k = 12      # 2^k = 4096 rows in the table
+        lgk = 12    # 2^k = 4096 rows in the table
         n = 1 << 18 # ~256k unique values
 
         # create a couple sketches and inject some values
         # we'll have 1/4 of the values overlap
-        hll  = hll_sketch(k, tgt_hll_type.HLL_8)
-        hll2 = hll_sketch(k, tgt_hll_type.HLL_6)
+        hll  = hll_sketch(lgk, tgt_hll_type.HLL_8)
+        hll2 = hll_sketch(lgk, tgt_hll_type.HLL_6)
         offset = int(3 * n / 4) # it's a float w/o cast
         # because we hash on the bits, not an abstract numeric value,
         # hll.update(1) and hll.update(1.0) give different results.
         for i in range(0, n):
             hll.update(i)
             hll2.update(i + offset)
-        
+
         # we can check that the upper and lower bounds bracket the
         # estimate, without needing to know the exact value.
         self.assertLessEqual(hll.get_lower_bound(1), hll.get_estimate())
         self.assertGreaterEqual(hll.get_upper_bound(1), hll.get_estimate())
 
-        # unioning uses a separate class, and we can either get a result
+        # union is a separate class, and we can either get a result
         # sketch or query the union object directly
-        union = hll_union(k)
+        union = hll_union(lgk)
         union.update(hll)
         union.update(hll2)
         result = union.get_result()
         self.assertEqual(result.get_estimate(), union.get_estimate())
 
         # since our process here (including post-union HLL) is
         # deterministic, we have checked and know the exact
@@ -55,33 +55,33 @@
 
         # serialize for storage and reconstruct
         sk_bytes = result.serialize_compact()
         self.assertEqual(len(sk_bytes), result.get_compact_serialization_bytes())
         new_hll = hll_sketch.deserialize(sk_bytes)
 
         # the sketch can self-report its configuration and status
-        self.assertEqual(new_hll.lg_config_k, k)
+        self.assertEqual(new_hll.lg_config_k, lgk)
         self.assertEqual(new_hll.tgt_type, tgt_hll_type.HLL_4)
         self.assertFalse(new_hll.is_empty())
 
         # if we want to reduce some object overhead, we can also reset
         new_hll.reset()
         self.assertTrue(new_hll.is_empty())
 
     def test_hll_sketch(self):
-        k = 8
+        lgk = 8
         n = 117
-        hll = self.generate_sketch(n, k, tgt_hll_type.HLL_6)
+        hll = self.generate_sketch(n, lgk, tgt_hll_type.HLL_6)
         hll.update('string data')
         hll.update(3.14159) # double data
 
         self.assertLessEqual(hll.get_lower_bound(1), hll.get_estimate())
         self.assertGreaterEqual(hll.get_upper_bound(1), hll.get_estimate())
 
-        self.assertEqual(hll.lg_config_k, k)
+        self.assertEqual(hll.lg_config_k, lgk)
         self.assertEqual(hll.tgt_type, tgt_hll_type.HLL_6)
 
         bytes_compact = hll.serialize_compact()
         bytes_update = hll.serialize_updatable()
         self.assertEqual(len(bytes_compact), hll.get_compact_serialization_bytes())
         self.assertEqual(len(bytes_update), hll.get_updatable_serialization_bytes())
 
@@ -94,37 +94,36 @@
         self.assertIsNotNone(hll_sketch.get_rel_err(True, False, 12, 1))
         self.assertIsNotNone(hll_sketch.get_max_updatable_serialization_bytes(20, tgt_hll_type.HLL_6))
 
         hll.reset()
         self.assertTrue(hll.is_empty())
 
     def test_hll_union(self):
-        k = 7
+        lgk = 7
         n = 53
-        union = hll_union(k)
+        union = hll_union(lgk)
 
-        sk = self.generate_sketch(n, k, tgt_hll_type.HLL_4, 0)
+        sk = self.generate_sketch(n, lgk, tgt_hll_type.HLL_4, 0)
         union.update(sk)
-        sk = self.generate_sketch(3 * n, k, tgt_hll_type.HLL_4, n)
+        sk = self.generate_sketch(3 * n, lgk, tgt_hll_type.HLL_4, n)
         union.update(sk)
         union.update('string data')
         union.update(1.4142136)
 
         self.assertLessEqual(union.get_lower_bound(1), union.get_estimate())
         self.assertGreaterEqual(union.get_upper_bound(1), union.get_estimate())
 
-        self.assertEqual(union.lg_config_k, k)
+        self.assertEqual(union.lg_config_k, lgk)
         self.assertFalse(union.is_empty())
 
         sk = union.get_result()
         self.assertTrue(isinstance(sk, hll_sketch))
         self.assertEqual(sk.tgt_type, tgt_hll_type.HLL_4)
         
-    def generate_sketch(self, n, k, sk_type=tgt_hll_type.HLL_4, st_idx=0):
-        sk = hll_sketch(k, sk_type)
+    def generate_sketch(self, n, lgk, sk_type=tgt_hll_type.HLL_4, st_idx=0):
+        sk = hll_sketch(lgk, sk_type)
         for i in range(st_idx, st_idx + n):
             sk.update(i)
         return sk
-        
-        
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `datasketches-4.0.1/python/tests/kll_test.py` & `datasketches-4.1.0/python/tests/kll_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import unittest
-from datasketches import kll_ints_sketch, kll_floats_sketch, kll_doubles_sketch, ks_test
+from datasketches import kll_ints_sketch, kll_floats_sketch, kll_doubles_sketch
+from datasketches import kll_items_sketch, ks_test, PyStringsSerDe
 import numpy as np
 
 class KllTest(unittest.TestCase):
-    def test_kll_example(self):
+    def test_kll_floats_example(self):
       k = 160
       n = 2 ** 20
 
       # create a sketch and inject ~1 million N(0,1) points as an array and as a single item
       kll = kll_floats_sketch(k)
       kll.update(np.random.normal(size=n-1))
       kll.update(0.0)
@@ -57,31 +58,39 @@
       self.assertFalse(kll.is_empty())
       self.assertTrue(kll.is_estimation_mode())
       self.assertEqual(kll.get_n(), n)
       self.assertEqual(kll.get_k(), k)
       self.assertLess(kll.get_num_retained(), n)
 
       # merging itself will double the number of items the sketch has seen
-      kll.merge(kll)
+      # but need to do that with a copy
+      kll_copy = kll_floats_sketch(kll)
+      kll.merge(kll_copy)
       self.assertEqual(kll.get_n(), 2*n)
 
       # we can then serialize and reconstruct the sketch
       kll_bytes = kll.serialize()
-      new_kll = kll.deserialize(kll_bytes)
+      new_kll = kll_floats_sketch.deserialize(kll_bytes)
       self.assertEqual(kll.get_num_retained(), new_kll.get_num_retained())
       self.assertEqual(kll.get_min_value(), new_kll.get_min_value())
       self.assertEqual(kll.get_max_value(), new_kll.get_max_value())
       self.assertEqual(kll.get_quantile(0.7), new_kll.get_quantile(0.7))
       self.assertEqual(kll.get_rank(0.0), new_kll.get_rank(0.0))
 
       # A Kolmogorov-Smirnov Test of kll and new_kll should match, even for
       # a fairly small p-value -- cannot reject the null hypothesis that
       # they come from the same distribution (since they do)
       self.assertFalse(ks_test(kll, new_kll, 0.001))
 
+      total_weight = 0
+      for tuple in kll:
+        item = tuple[0]
+        weight = tuple[1]
+        total_weight = total_weight + weight
+      self.assertEqual(total_weight, kll.get_n())
 
     def test_kll_ints_sketch(self):
         k = 100
         n = 10
         kll = kll_ints_sketch(k)
         for i in range(0, n):
           kll.update(i)
@@ -104,22 +113,47 @@
         self.assertEqual(kll.get_quantile(0.5), round(n/2))
         quants = kll.get_quantiles([0.25, 0.5, 0.75])
         self.assertIsNotNone(quants)
         self.assertEqual(len(quants), 3)
 
         self.assertEqual(kll.get_rank(round(n/2)), 0.5)
 
-        # merge self
-        kll.merge(kll)
+        # merge copy of self
+        kll_copy = kll_ints_sketch(kll)
+        kll.merge(kll_copy)
         self.assertEqual(kll.get_n(), 2 * n)
 
         sk_bytes = kll.serialize()
         self.assertTrue(isinstance(kll_ints_sketch.deserialize(sk_bytes), kll_ints_sketch))
 
     def test_kll_doubles_sketch(self):
       # already tested float and ints and it's templatized, so just make sure it instantiates properly
       k = 75
       kll = kll_doubles_sketch(k)
       self.assertTrue(kll.is_empty())
 
+    def test_kll_items_sketch(self):
+      # most functionality has been tested, but we need to ensure objects and sorting work
+      # as well as serialization
+      k = 100
+      n = 2 ** 16
+
+      # create a sketch and inject enough points to force compaction
+      kll = kll_items_sketch(k)
+      for i in range(0, n):
+        kll.update(str(i))
+      
+      kll_copy = kll_items_sketch(kll)
+      kll.merge(kll_copy)
+      self.assertEqual(kll.get_n(), 2 * n)
+      
+      kll_bytes = kll.serialize(PyStringsSerDe())
+      new_kll = kll_items_sketch.deserialize(kll_bytes, PyStringsSerDe())
+      self.assertEqual(kll.get_num_retained(), new_kll.get_num_retained())
+      self.assertEqual(kll.get_min_value(), new_kll.get_min_value())
+      self.assertEqual(kll.get_max_value(), new_kll.get_max_value())
+      self.assertEqual(kll.get_quantile(0.7), new_kll.get_quantile(0.7))
+      self.assertEqual(kll.get_rank(str(n/4)), new_kll.get_rank(str(n/4)))
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `datasketches-4.0.1/python/tests/quantiles_test.py` & `datasketches-4.1.0/python/tests/quantiles_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import unittest
-from datasketches import quantiles_ints_sketch, quantiles_floats_sketch, quantiles_doubles_sketch, ks_test
+from datasketches import quantiles_ints_sketch, quantiles_floats_sketch, quantiles_doubles_sketch
+from datasketches import quantiles_items_sketch, ks_test, PyStringsSerDe
 import numpy as np
 
 class QuantilesTest(unittest.TestCase):
-    def test_quantiles_example(self):
+    def test_quantiles_floats_example(self):
       k = 128
       n = 2 ** 20
 
       # create a sketch and inject ~1 million N(0,1) points as an array and as a single item
       quantiles = quantiles_floats_sketch(k)
       quantiles.update(np.random.normal(size=n-1))
       quantiles.update(0.0)
@@ -57,33 +58,41 @@
       self.assertFalse(quantiles.is_empty())
       self.assertTrue(quantiles.is_estimation_mode())
       self.assertEqual(quantiles.get_n(), n)
       self.assertEqual(quantiles.get_k(), k)
       self.assertLess(quantiles.get_num_retained(), n)
 
       # merging itself will double the number of items the sketch has seen
-      quantiles.merge(quantiles)
+      quantiles_copy = quantiles_floats_sketch(quantiles)
+      quantiles.merge(quantiles_copy)
       self.assertEqual(quantiles.get_n(), 2*n)
 
       # we can then serialize and reconstruct the sketch
       quantiles_bytes = quantiles.serialize()
-      new_quantiles = quantiles.deserialize(quantiles_bytes)
+      new_quantiles = quantiles_floats_sketch.deserialize(quantiles_bytes)
       self.assertEqual(quantiles.get_num_retained(), new_quantiles.get_num_retained())
       self.assertEqual(quantiles.get_min_value(), new_quantiles.get_min_value())
       self.assertEqual(quantiles.get_max_value(), new_quantiles.get_max_value())
       self.assertEqual(quantiles.get_quantile(0.7), new_quantiles.get_quantile(0.7))
       self.assertEqual(quantiles.get_rank(0.0), new_quantiles.get_rank(0.0))
 
       # If we create a new sketch with a very different distribution, a Kolmogorov-Smirnov Test
       # of the two should return True: we can reject the null hypothesis that the sketches
       # come from the same distributions.
       unif_quantiles = quantiles_floats_sketch(k)
       unif_quantiles.update(np.random.uniform(10, 20, size=n-1))
       self.assertTrue(ks_test(quantiles, unif_quantiles, 0.001))
 
+      total_weight = 0
+      for tuple in quantiles:
+        item = tuple[0]
+        weight = tuple[1]
+        total_weight = total_weight + weight
+      self.assertEqual(total_weight, quantiles.get_n())
+
     def test_quantiles_ints_sketch(self):
         k = 128
         n = 10
         quantiles = quantiles_ints_sketch(k)
         for i in range(0, n):
           quantiles.update(i)
 
@@ -106,21 +115,46 @@
         quants = quantiles.get_quantiles([0.25, 0.5, 0.75])
         self.assertIsNotNone(quants)
         self.assertEqual(len(quants), 3)
 
         self.assertEqual(quantiles.get_rank(round(n/2)), 0.5)
 
         # merge self
-        quantiles.merge(quantiles)
+        quantiles_copy = quantiles_ints_sketch(quantiles)
+        quantiles.merge(quantiles_copy)
         self.assertEqual(quantiles.get_n(), 2 * n)
 
         sk_bytes = quantiles.serialize()
         self.assertTrue(isinstance(quantiles_ints_sketch.deserialize(sk_bytes), quantiles_ints_sketch))
 
     def test_quantiles_doubles_sketch(self):
       # already tested floats and ints and it's templatized, so just make sure it instantiates properly
       k = 128
       quantiles = quantiles_doubles_sketch(k)
       self.assertTrue(quantiles.is_empty())
 
+    def test_quantiles_items_sketch(self):
+      # most functionality has been tested, but we need to ensure objects and sorting work
+      # as well as serialization
+      k = 128
+      n = 2 ** 16
+
+      # create a sketch and inject enough points to force compaction
+      quantiles = quantiles_items_sketch(k)
+      for i in range(0, n):
+        quantiles.update(str(i))
+      
+      quantiles_copy = quantiles_items_sketch(quantiles)
+      quantiles.merge(quantiles_copy)
+      self.assertEqual(quantiles.get_n(), 2 * n)
+      
+      quantiles_bytes = quantiles.serialize(PyStringsSerDe())
+      new_quantiles = quantiles_items_sketch.deserialize(quantiles_bytes, PyStringsSerDe())
+      self.assertEqual(quantiles.get_num_retained(), new_quantiles.get_num_retained())
+      self.assertEqual(quantiles.get_min_value(), new_quantiles.get_min_value())
+      self.assertEqual(quantiles.get_max_value(), new_quantiles.get_max_value())
+      self.assertEqual(quantiles.get_quantile(0.7), new_quantiles.get_quantile(0.7))
+      self.assertEqual(quantiles.get_rank(str(n/4)), new_quantiles.get_rank(str(n/4)))
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `datasketches-4.0.1/python/tests/req_test.py` & `datasketches-4.1.0/python/tests/req_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import unittest
-from datasketches import req_ints_sketch, req_floats_sketch
+from datasketches import req_ints_sketch, req_floats_sketch, req_items_sketch, PyStringsSerDe
 import numpy as np
 
 class reqTest(unittest.TestCase):
     def test_req_example(self):
       k = 12
       n = 2 ** 20
 
@@ -63,26 +63,34 @@
       self.assertFalse(req.is_empty())
       self.assertTrue(req.is_estimation_mode())
       self.assertEqual(req.get_n(), n)
       self.assertLess(req.get_num_retained(), n)
       self.assertEqual(req.get_k(), k)
 
       # merging itself will double the number of items the sketch has seen
-      req.merge(req)
+      req_copy = req_floats_sketch(req)
+      req.merge(req_copy)
       self.assertEqual(req.get_n(), 2*n)
 
       # we can then serialize and reconstruct the sketch
       req_bytes = req.serialize()
-      new_req = req.deserialize(req_bytes)
+      new_req = req_floats_sketch.deserialize(req_bytes)
       self.assertEqual(req.get_num_retained(), new_req.get_num_retained())
       self.assertEqual(req.get_min_value(), new_req.get_min_value())
       self.assertEqual(req.get_max_value(), new_req.get_max_value())
       self.assertEqual(req.get_quantile(0.7), new_req.get_quantile(0.7))
       self.assertEqual(req.get_rank(0.0), new_req.get_rank(0.0))
 
+      total_weight = 0
+      for tuple in req:
+        item = tuple[0]
+        weight = tuple[1]
+        total_weight = total_weight + weight
+      self.assertEqual(total_weight, req.get_n())
+
     def test_req_ints_sketch(self):
         k = 100
         n = 10
         req = req_ints_sketch(k)
         for i in range(0, n):
           req.update(i)
 
@@ -105,22 +113,47 @@
         quants = req.get_quantiles([0.25, 0.5, 0.75])
         self.assertIsNotNone(quants)
         self.assertEqual(len(quants), 3)
 
         self.assertEqual(req.get_rank(round(n/2)), 0.5)
 
         # merge self
-        req.merge(req)
+        req_copy = req_ints_sketch(req)
+        req.merge(req_copy)
         self.assertEqual(req.get_n(), 2 * n)
 
         sk_bytes = req.serialize()
         self.assertTrue(isinstance(req_ints_sketch.deserialize(sk_bytes), req_ints_sketch))
 
     def test_req_floats_sketch(self):
-      # already tested ints and it's templatized, so just make sure it instantiates properly
+      # already tested floats with LRA so just check that HRA works
       k = 75
       req = req_floats_sketch(k, False) # low rank accuracy
       self.assertTrue(req.is_empty())
       self.assertFalse(req.is_hra())
 
+    def test_req_items_sketch(self):
+      # most functionality has been tested, but we need to ensure objects and sorting work
+      # as well as serialization
+      k = 100
+      n = 2 ** 16
+
+      # create a sketch and inject enough points to force compaction
+      req = req_items_sketch(k)
+      for i in range(0, n):
+        req.update(str(i))
+      
+      req_copy = req_items_sketch(req)
+      req.merge(req_copy)
+      self.assertEqual(req.get_n(), 2 * n)
+      
+      req_bytes = req.serialize(PyStringsSerDe())
+      new_req = req_items_sketch.deserialize(req_bytes, PyStringsSerDe())
+      self.assertEqual(req.get_num_retained(), new_req.get_num_retained())
+      self.assertEqual(req.get_min_value(), new_req.get_min_value())
+      self.assertEqual(req.get_max_value(), new_req.get_max_value())
+      self.assertEqual(req.get_quantile(0.7), new_req.get_quantile(0.7))
+      self.assertEqual(req.get_rank(str(n/4)), new_req.get_rank(str(n/4)))
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `datasketches-4.0.1/python/tests/theta_test.py` & `datasketches-4.1.0/python/tests/theta_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
- 
+
 import unittest
 
 from datasketches import theta_sketch, update_theta_sketch
 from datasketches import compact_theta_sketch, theta_union
 from datasketches import theta_intersection, theta_a_not_b
 from datasketches import theta_jaccard_similarity
 
 class ThetaTest(unittest.TestCase):
     def test_theta_basic_example(self):
-        k = 12      # 2^k = 4096 rows in the table
+        lgk = 12    # 2^k = 4096 rows in the table
         n = 1 << 18 # ~256k unique values
 
         # create a sketch and inject some values
-        sk = self.generate_theta_sketch(n, k)
+        sk = self.generate_theta_sketch(n, lgk)
 
         # we can check that the upper and lower bounds bracket the
         # estimate, without needing to know the exact value.
         self.assertLessEqual(sk.get_lower_bound(1), sk.get_estimate())
         self.assertGreaterEqual(sk.get_upper_bound(1), sk.get_estimate())
 
         # because this sketch is deterministically generated, we can
@@ -44,28 +44,34 @@
         sk_bytes = sk.compact().serialize()
         new_sk = compact_theta_sketch.deserialize(sk_bytes)
 
         # estimate remains unchanged
         self.assertFalse(sk.is_empty())
         self.assertEqual(sk.get_estimate(), new_sk.get_estimate())
 
+        count = 0
+        for hash in new_sk:
+          self.assertLess(hash, new_sk.get_theta64())
+          count = count + 1
+        self.assertEqual(count, new_sk.get_num_retained())
+
     def test_theta_set_operations(self):
-        k = 12      # 2^k = 4096 rows in the table
+        lgk = 12    # 2^k = 4096 rows in the table
         n = 1 << 18 # ~256k unique values
 
         # we'll have 1/4 of the values overlap
         offset = int(3 * n / 4) # it's a float w/o cast
 
         # create a couple sketches and inject some values
-        sk1 = self.generate_theta_sketch(n, k)
-        sk2 = self.generate_theta_sketch(n, k, offset)
+        sk1 = self.generate_theta_sketch(n, lgk)
+        sk2 = self.generate_theta_sketch(n, lgk, offset)
 
         # UNIONS
         # create a union object
-        union = theta_union(k)
+        union = theta_union(lgk)
         union.update(sk1)
         union.update(sk2)
 
         # getting result from union returns a compact_theta_sketch
         # compact theta sketches can be used in additional unions
         # or set operations but cannot accept further item updates
         result = union.get_result()
@@ -73,15 +79,14 @@
 
         # since our process here is deterministic, we have
         # checked and know the exact answer is within one
         # standard deviation of the estimate
         self.assertLessEqual(result.get_lower_bound(1), 7 * n / 4)
         self.assertGreaterEqual(result.get_upper_bound(1), 7 * n / 4)
 
-
         # INTERSECTIONS
         # create an intersection object
         intersect = theta_intersection() # no lg_k
         intersect.update(sk1)
         intersect.update(sk2)
 
         # has_result() indicates the intersection has been used,
@@ -92,15 +97,14 @@
         result = intersect.get_result()
         self.assertTrue(isinstance(result, compact_theta_sketch))
 
         # we know the sets overlap by 1/4
         self.assertLessEqual(result.get_lower_bound(1), n / 4)
         self.assertGreaterEqual(result.get_upper_bound(1), n / 4)
 
-
         # A NOT B
         # create an a_not_b object
         anb = theta_a_not_b() # no lg_k
         result = anb.compute(sk1, sk2)
 
         # as with unions, the result is a compact sketch
         self.assertTrue(isinstance(result, compact_theta_sketch))
@@ -130,17 +134,15 @@
         self.assertTrue(theta_jaccard_similarity.dissimilarity_test(sk1, sk2, 0.2))
 
         # check that the Jaccard Index is at least (lower bound) 0.7
         # exact result would be 3/4, using result from A NOT B test
         self.assertTrue(theta_jaccard_similarity.similarity_test(sk1, result, 0.7))
 
 
-    def generate_theta_sketch(self, n, k, offset=0):
-      sk = update_theta_sketch(k)
+    def generate_theta_sketch(self, n, lgk, offset=0):
+      sk = update_theta_sketch(lgk)
       for i in range(0, n):
         sk.update(i + offset)
       return sk
-        
+
 if __name__ == '__main__':
     unittest.main()
-
-
```

### Comparing `datasketches-4.0.1/python/tests/vector_of_kll_test.py` & `datasketches-4.1.0/python/tests/vector_of_kll_test.py`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/python/tests/vo_test.py` & `datasketches-4.1.0/python/tests/vo_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,21 @@
     self.assertEqual(n + 1, vo.n)
     self.assertFalse(vo.is_empty())
 
     # we can easily get the list of items in the sample
     items = vo.get_samples()
     self.assertEqual(len(items), k)
 
+    count = 0
+    for tuple in vo:
+      sample = tuple[0]
+      weight = tuple[1]
+      count = count + 1
+    self.assertEqual(count, vo.num_samples)
+
     # we can also apply a predicate to the sketch to get an estimate
     # (with optimally minimal variance) of the subset sum of items
     # matching that predicate among the entire population
 
     # we'll use a lambda here, but any function operating on a single
     # item which returns a boolean value should work
     summary = vo.estimate_subset_sum(lambda x: x < 0)
```

### Comparing `datasketches-4.0.1/quantiles/CMakeLists.txt` & `datasketches-4.1.0/quantiles/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/quantiles/include/quantiles_sketch.hpp` & `datasketches-4.1.0/quantiles/include/quantiles_sketch.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -576,23 +576,28 @@
   static inline bool check_update_item(TT) {
     return true;
   }
 };
 
 
 template<typename T, typename C, typename A>
-class quantiles_sketch<T, C, A>::const_iterator: public std::iterator<std::input_iterator_tag, T> {
+class quantiles_sketch<T, C, A>::const_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
   using value_type = std::pair<const T&, const uint64_t>;
+  using difference_type = void;
+  using pointer = const return_value_holder<value_type>;
+  using reference = const value_type;
+
   const_iterator& operator++();
   const_iterator& operator++(int);
   bool operator==(const const_iterator& other) const;
   bool operator!=(const const_iterator& other) const;
-  const value_type operator*() const;
-  const return_value_holder<value_type> operator->() const;
+  reference operator*() const;
+  pointer operator->() const;
 private:
   friend class quantiles_sketch<T, C, A>;
   using Level = std::vector<T, A>;
   using AllocLevel = typename std::allocator_traits<A>::template rebind_alloc<Level>;
   Level base_buffer_;
   std::vector<Level, AllocLevel> levels_;
   int level_;
```

### Comparing `datasketches-4.0.1/quantiles/include/quantiles_sketch_impl.hpp` & `datasketches-4.1.0/quantiles/include/quantiles_sketch_impl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -641,20 +641,20 @@
   }
 
   if (print_items) {
     os << "### Quantiles Sketch data:" << std::endl;
     uint8_t level = 0;
     os << " BB:" << std::endl;
     for (const T& item : base_buffer_) {
-      os << "    " << std::to_string(item) << std::endl;
+      os << "    " << item << std::endl;
     }
     for (uint8_t i = 0; i < levels_.size(); ++i) {
       os << " level " << static_cast<unsigned int>(level) << ":" << std::endl;
       for (const T& item : levels_[i]) {
-        os << "   " << std::to_string(item) << std::endl;
+        os << "   " << item << std::endl;
       }
     }
     os << "### End sketch data" << std::endl;
   }
   return string<A>(os.str().c_str(), allocator_);
 }
 
@@ -1350,19 +1350,19 @@
 
 template<typename T, typename C, typename A>
 bool quantiles_sketch<T, C, A>::const_iterator::operator!=(const const_iterator& other) const {
   return !operator==(other);
 }
 
 template<typename T, typename C, typename A>
-auto quantiles_sketch<T, C, A>::const_iterator::operator*() const -> const value_type {
+auto quantiles_sketch<T, C, A>::const_iterator::operator*() const -> reference {
   return value_type(level_ == -1 ? base_buffer_[index_] : levels_[level_][index_], weight_);
 }
 
 template<typename T, typename C, typename A>
-auto quantiles_sketch<T, C, A>::const_iterator::operator->() const -> const return_value_holder<value_type> {
+auto quantiles_sketch<T, C, A>::const_iterator::operator->() const -> pointer {
   return **this;
 }
 
 } /* namespace datasketches */
 
 #endif // _QUANTILES_SKETCH_IMPL_HPP_
```

### Comparing `datasketches-4.0.1/quantiles/test/CMakeLists.txt` & `datasketches-4.1.0/quantiles/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/quantiles/test/kolmogorov_smirnov_test.cpp` & `datasketches-4.1.0/quantiles/test/kolmogorov_smirnov_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/quantiles/test/quantiles_compatibility_test.cpp` & `datasketches-4.1.0/quantiles/test/quantiles_compatibility_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/quantiles/test/quantiles_sketch_test.cpp` & `datasketches-4.1.0/quantiles/test/quantiles_sketch_test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     double subtotal_pmf(0);
     for (int i = 0; i < n; i++) {
       if (sketch.get_rank(values[i]) != ranks[i]) {
         std::cerr << "checking rank vs CDF for value " << i << std::endl;
         REQUIRE(sketch.get_rank(values[i]) == ranks[i]);
       }
       subtotal_pmf += pmf[i];
-      if (abs(ranks[i] - subtotal_pmf) > NUMERIC_NOISE_TOLERANCE) {
+      if (std::abs(ranks[i] - subtotal_pmf) > NUMERIC_NOISE_TOLERANCE) {
         std::cerr << "CDF vs PMF for value " << i << std::endl;
         REQUIRE(ranks[i] == Approx(subtotal_pmf).margin(NUMERIC_NOISE_TOLERANCE));
       }
     }
   }
 
   SECTION("inclusive true vs false") {
```

### Comparing `datasketches-4.0.1/req/CMakeLists.txt` & `datasketches-4.1.0/req/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/req/include/req_common.hpp` & `datasketches-4.1.0/req/include/req_common.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/req/include/req_compactor.hpp` & `datasketches-4.1.0/req/include/req_compactor.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/req/include/req_compactor_impl.hpp` & `datasketches-4.1.0/req/include/req_compactor_impl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 #include <cmath>
 #include <algorithm>
 
 #include "count_zeros.hpp"
 #include "conditional_forward.hpp"
 #include "common_defs.hpp"
 
-#include <iomanip>
-
 namespace datasketches {
 
 template<typename T, typename C, typename A>
 req_compactor<T, C, A>::req_compactor(bool hra, uint8_t lg_weight, uint32_t section_size,
     const C& comparator, const A& allocator, bool sorted):
 comparator_(comparator),
 allocator_(allocator),
```

### Comparing `datasketches-4.0.1/req/include/req_sketch.hpp` & `datasketches-4.1.0/req/include/req_sketch.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -395,23 +395,28 @@
   }
 
   // for type converting constructor
   template<typename TT, typename CC, typename AA> friend class req_sketch;
 };
 
 template<typename T, typename C, typename A>
-class req_sketch<T, C, A>::const_iterator: public std::iterator<std::input_iterator_tag, T> {
+class req_sketch<T, C, A>::const_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
   using value_type = std::pair<const T&, const uint64_t>;
+  using difference_type = void;
+  using pointer = const return_value_holder<value_type>;
+  using reference = const value_type;
+
   const_iterator& operator++();
   const_iterator& operator++(int);
   bool operator==(const const_iterator& other) const;
   bool operator!=(const const_iterator& other) const;
-  const value_type operator*() const;
-  const return_value_holder<value_type> operator->() const;
+  reference operator*() const;
+  pointer operator->() const;
 private:
   using LevelsIterator = typename std::vector<Compactor, AllocCompactor>::const_iterator;
   LevelsIterator levels_it_;
   LevelsIterator levels_end_;
   const T* compactor_it_;
   friend class req_sketch<T, C, A>;
   const_iterator(LevelsIterator begin, LevelsIterator end);
```

### Comparing `datasketches-4.0.1/req/include/req_sketch_impl.hpp` & `datasketches-4.1.0/req/include/req_sketch_impl.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -844,19 +844,19 @@
 
 template<typename T, typename C, typename A>
 bool req_sketch<T, C, A>::const_iterator::operator!=(const const_iterator& other) const {
   return !operator==(other);
 }
 
 template<typename T, typename C, typename A>
-auto req_sketch<T, C, A>::const_iterator::operator*() const -> const value_type {
+auto req_sketch<T, C, A>::const_iterator::operator*() const -> reference {
   return value_type(*compactor_it_, 1ULL << (*levels_it_).get_lg_weight());
 }
 
 template<typename T, typename C, typename A>
-auto req_sketch<T, C, A>::const_iterator::operator->() const -> const return_value_holder<value_type> {
+auto req_sketch<T, C, A>::const_iterator::operator->() const -> pointer {
   return **this;
 }
 
 } /* namespace datasketches */
 
 #endif
```

### Comparing `datasketches-4.0.1/req/test/CMakeLists.txt` & `datasketches-4.1.0/req/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/req/test/req_float_estimation_from_java.sk` & `datasketches-4.1.0/req/test/req_float_estimation_from_java.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/req/test/req_sketch_custom_type_test.cpp` & `datasketches-4.1.0/req/test/req_sketch_custom_type_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/req/test/req_sketch_test.cpp` & `datasketches-4.1.0/req/test/req_sketch_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/CMakeLists.txt` & `datasketches-4.1.0/sampling/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/include/var_opt_sketch.hpp` & `datasketches-4.1.0/sampling/include/var_opt_sketch.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -342,53 +342,67 @@
     static inline uint32_t next_int(uint32_t max_value);
     static inline double next_double_exclude_zero();
 
     class iterator;
 };
 
 template<typename T, typename A>
-class var_opt_sketch<T, A>::const_iterator : public std::iterator<std::input_iterator_tag, T> {
+class var_opt_sketch<T, A>::const_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = std::pair<const T&, const double>;
+  using difference_type = void;
+  using pointer = const return_value_holder<value_type>;
+  using reference = const value_type;
+
   const_iterator(const const_iterator& other);
   const_iterator& operator++();
   const_iterator& operator++(int);
   bool operator==(const const_iterator& other) const;
   bool operator!=(const const_iterator& other) const;
-  const std::pair<const T&, const double> operator*() const;
+  reference operator*() const;
+  pointer operator->() const;
 
 private:
   friend class var_opt_sketch<T, A>;
   friend class var_opt_union<T, A>;
 
   // default iterator over full sketch
   const_iterator(const var_opt_sketch<T, A>& sk, bool is_end);
   
-  // iterates over only one of the H or R region, optionally applying weight correction
-  // to R region (can correct for numerical precision issues)
+  // iterates over only one of the H or R regions
+  // does not apply weight correction
   const_iterator(const var_opt_sketch<T, A>& sk, bool is_end, bool use_r_region);
 
   bool get_mark() const;
 
   const var_opt_sketch<T, A>* sk_;
   double cum_r_weight_; // used for weight correction
   double r_item_wt_;
   size_t idx_;
   const size_t final_idx_;
 };
 
 // non-const iterator for internal use
 template<typename T, typename A>
-class var_opt_sketch<T, A>::iterator : public std::iterator<std::input_iterator_tag, T> {
+class var_opt_sketch<T, A>::iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = std::pair<T&, double>;
+  using difference_type = void;
+  using pointer = return_value_holder<value_type>;
+  using reference = value_type;
+
   iterator(const iterator& other);
   iterator& operator++();
   iterator& operator++(int);
   bool operator==(const iterator& other) const;
   bool operator!=(const iterator& other) const;
-  std::pair<T&, double> operator*();
+  reference operator*();
+  pointer operator->();
 
 private:
   friend class var_opt_sketch<T, A>;
   friend class var_opt_union<T, A>;
   
   // iterates over only one of the H or R region, applying weight correction
   // if iterating over R region (can correct for numerical precision issues)
```

### Comparing `datasketches-4.0.1/sampling/include/var_opt_sketch_impl.hpp` & `datasketches-4.1.0/sampling/include/var_opt_sketch_impl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -185,24 +185,24 @@
 template<typename T, typename A>
 var_opt_sketch<T, A>::~var_opt_sketch() {
   if (data_ != nullptr) {
     if (filled_data_) {
       // destroy everything
       const size_t num_to_destroy = std::min(k_ + 1, curr_items_alloc_);
       for (size_t i = 0; i < num_to_destroy; ++i) {
-        allocator_.destroy(data_ + i);
+        data_[i].~T();
       }
     } else {
       // skip gap or anything unused at the end
       for (size_t i = 0; i < h_; ++i) {
-        allocator_.destroy(data_+ i);
+        data_[i].~T();
       }
     
       for (size_t i = h_ + 1; i < h_ + r_ + 1; ++i) {
-        allocator_.destroy(data_ + i);
+        data_[i].~T();
       }
     }
     allocator_.deallocate(data_, curr_items_alloc_);
   }
 
   if (weights_ != nullptr) {
     AllocDouble(allocator_).deallocate(weights_, curr_items_alloc_);
@@ -654,22 +654,22 @@
     ++curr_items_alloc_;
   }
 
   if (filled_data_) {
     // destroy everything
     const size_t num_to_destroy = std::min(k_ + 1, prev_alloc);
     for (size_t i = 0; i < num_to_destroy; ++i) 
-      allocator_.destroy(data_ + i);
+      data_[i].~T();
   } else {
     // skip gap or anything unused at the end
     for (size_t i = 0; i < h_; ++i)
-      allocator_.destroy(data_+ i);
+      data_[i].~T();
     
     for (size_t i = h_ + 1; i < h_ + r_ + 1; ++i)
-      allocator_.destroy(data_ + i);
+      data_[i].~T();
   }
 
   if (curr_items_alloc_ < prev_alloc) {
     const bool is_gadget = (marks_ != nullptr);
   
     allocator_.deallocate(data_, prev_alloc);
     AllocDouble(allocator_).deallocate(weights_, prev_alloc);
@@ -750,18 +750,18 @@
   // Using a temporary stream for implementation here does not comply with AllocatorAwareContainer requirements.
   // The stream does not support passing an allocator instance, and alternatives are complicated.
   std::ostringstream os;
   os << "### Sketch Items" << std::endl;
   const uint32_t array_length = (n_ < k_ ? n_ : k_ + 1);
   for (uint32_t i = 0, display_idx = 0; i < array_length; ++i) {
     if (i == h_ && print_gap) {
-      os << i << ": GAP" << std::endl;
+      os << display_idx << ": GAP" << std::endl;
       ++display_idx;
     } else {
-      os << i << ": " << data_[i] << "\twt = ";
+      os << display_idx << ": " << data_[i] << "\twt = ";
       if (weights_[i] == -1.0) {
         os << get_tau() << "\t(-1.0)" << std::endl;
       } else {
         os << weights_[i] << std::endl;
       }
       ++display_idx;
     }
@@ -986,15 +986,15 @@
     filled_data_ = false;
 
     T* tmp_data = allocator_.allocate(curr_items_alloc_);
     double* tmp_weights = AllocDouble(allocator_).allocate(curr_items_alloc_);
 
     for (uint32_t i = 0; i < prev_size; ++i) {
       new (&tmp_data[i]) T(std::move(data_[i]));
-      allocator_.destroy(data_ + i);
+      data_[i].~T();
       tmp_weights[i] = weights_[i];
     }
 
     allocator_.deallocate(data_, prev_size);
     AllocDouble(allocator_).deallocate(weights_, prev_size);
 
     data_ = tmp_data;
@@ -1527,35 +1527,36 @@
     idx_ = (is_end ? sk.h_ : 0);
   }
   
   // unlike in full iterator case, may happen even if sketch is not empty
   if (idx_ == final_idx_) { sk_ = nullptr; }
 }
 
-
 template<typename T, typename A>
 var_opt_sketch<T, A>::const_iterator::const_iterator(const const_iterator& other) :
   sk_(other.sk_),
   cum_r_weight_(other.cum_r_weight_),
   r_item_wt_(other.r_item_wt_),
   idx_(other.idx_),
   final_idx_(other.final_idx_)
 {}
 
 template<typename T, typename A>
 typename var_opt_sketch<T, A>::const_iterator& var_opt_sketch<T, A>::const_iterator::operator++() {
+  // accumulate weight already visited
+  if (idx_ > sk_->h_) { cum_r_weight_ += r_item_wt_; }
+
   ++idx_;
   
   if (idx_ == final_idx_) {
     sk_ = nullptr;
     return *this;
   } else if (idx_ == sk_->h_ && sk_->r_ > 0) { // check for the gap
     ++idx_;
   }
-  if (idx_ > sk_->h_) { cum_r_weight_ += r_item_wt_; }
   return *this;
 }
 
 template<typename T, typename A>
 typename var_opt_sketch<T, A>::const_iterator& var_opt_sketch<T, A>::const_iterator::operator++(int) {
   const_iterator tmp(*this);
   operator++();
@@ -1571,22 +1572,27 @@
 
 template<typename T, typename A>
 bool var_opt_sketch<T, A>::const_iterator::operator!=(const const_iterator& other) const {
   return !operator==(other);
 }
 
 template<typename T, typename A>
-const std::pair<const T&, const double> var_opt_sketch<T, A>::const_iterator::operator*() const {
+auto var_opt_sketch<T, A>::const_iterator::operator*() const -> reference {
   double wt;
   if (idx_ < sk_->h_) {
     wt = sk_->weights_[idx_];
   } else {
     wt = r_item_wt_;
   }
-  return std::pair<const T&, const double>(sk_->data_[idx_], wt);
+  return value_type(sk_->data_[idx_], wt);
+}
+
+template<typename T, typename A>
+auto var_opt_sketch<T, A>::const_iterator::operator->() const -> pointer {
+  return **this;
 }
 
 template<typename T, typename A>
 bool var_opt_sketch<T, A>::const_iterator::get_mark() const {
   return sk_->marks_ == nullptr ? false : sk_->marks_[idx_];
 }
 
@@ -1618,23 +1624,26 @@
   r_item_wt_(other.r_item_wt_),
   idx_(other.idx_),
   final_idx_(other.final_idx_)
 {}
 
 template<typename T, typename A>
 typename var_opt_sketch<T, A>::iterator& var_opt_sketch<T, A>::iterator::operator++() {
+  // accumulate weight already visited
+  if (idx_ > sk_->h_) { cum_r_weight_ += r_item_wt_; }
+
   ++idx_;
   
   if (idx_ == final_idx_) {
     sk_ = nullptr;
     return *this;
   } else if (idx_ == sk_->h_ && sk_->r_ > 0) { // check for the gap
     ++idx_;
   }
-  if (idx_ > sk_->h_) { cum_r_weight_ += r_item_wt_; }
+
   return *this;
 }
 
 template<typename T, typename A>
 typename var_opt_sketch<T, A>::iterator& var_opt_sketch<T, A>::iterator::operator++(int) {
   const_iterator tmp(*this);
   operator++();
@@ -1650,24 +1659,29 @@
 
 template<typename T, typename A>
 bool var_opt_sketch<T, A>::iterator::operator!=(const iterator& other) const {
   return !operator==(other);
 }
 
 template<typename T, typename A>
-std::pair<T&, double> var_opt_sketch<T, A>::iterator::operator*() {
+auto var_opt_sketch<T, A>::iterator::operator*() -> reference {
   double wt;
   if (idx_ < sk_->h_) {
     wt = sk_->weights_[idx_];
   } else if (idx_ == final_idx_ - 1) {
     wt = sk_->total_wt_r_ - cum_r_weight_;
   } else {
     wt = r_item_wt_;
   }
-  return std::pair<T&, double>(sk_->data_[idx_], wt);
+  return value_type(sk_->data_[idx_], wt);
+}
+
+template<typename T, typename A>
+auto var_opt_sketch<T, A>::iterator::operator->() -> pointer {
+  return **this;
 }
 
 template<typename T, typename A>
 bool var_opt_sketch<T, A>::iterator::get_mark() const {
   return sk_->marks_ == nullptr ? false : sk_->marks_[idx_];
 }
```

### Comparing `datasketches-4.0.1/sampling/include/var_opt_union.hpp` & `datasketches-4.1.0/sampling/include/var_opt_union.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -149,14 +149,16 @@
    * Prints a summary of the union as a string.
    * @return the summary as a string
    */
   string<A> to_string() const;
 
 private:
   typedef typename std::allocator_traits<A>::template rebind_alloc<var_opt_sketch<T, A>> AllocSketch;
+  typedef typename std::allocator_traits<A>::template rebind_alloc<double> AllocDouble;
+  typedef typename std::allocator_traits<A>::template rebind_alloc<bool> AllocBool;
 
   static const uint8_t PREAMBLE_LONGS_EMPTY = 1;
   static const uint8_t PREAMBLE_LONGS_NON_EMPTY = 4;
   static const uint8_t SER_VER = 2;
   static const uint8_t FAMILY_ID = 14;
   static const uint8_t EMPTY_FLAG_MASK  = 4;
 
@@ -166,18 +168,20 @@
   double outer_tau_numer_; // total weight of all input R-zones where tau = outer_tau
 
   // total cardinality of the same R-zones, or zero if no input sketch was in estimation mode
   uint64_t outer_tau_denom_;
 
   uint32_t max_k_;
 
+  A allocator_;
+
   var_opt_sketch<T, A> gadget_;
 
   var_opt_union(uint64_t n, double outer_tau_numer, uint64_t outer_tau_denom,
-                uint32_t max_k, var_opt_sketch<T, A>&& gadget);
+                uint32_t max_k, var_opt_sketch<T, A>&& gadget, const A& allocator = A());
 
   /*
    IMPORTANT NOTE: the "gadget" in the union object appears to be a varopt sketch,
    but in fact is NOT because it doesn't satisfy the mathematical definition
    of a varopt sketch of the concatenated input streams. Therefore it could be different
    from a true varopt sketch with that value of K, in which case it could easily provide
    worse estimation accuracy for subset-sum queries.
```

### Comparing `datasketches-4.0.1/sampling/include/var_opt_union_impl.hpp` & `datasketches-4.1.0/sampling/include/var_opt_union_impl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,65 +30,71 @@
 
 template<typename T, typename A>
 var_opt_union<T, A>::var_opt_union(uint32_t max_k, const A& allocator) :
   n_(0),
   outer_tau_numer_(0.0),
   outer_tau_denom_(0),
   max_k_(max_k),
+  allocator_(allocator),
   gadget_(max_k, var_opt_sketch<T, A>::DEFAULT_RESIZE_FACTOR, true, allocator)
 {}
 
 template<typename T, typename A>
 var_opt_union<T, A>::var_opt_union(const var_opt_union& other) :
   n_(other.n_),
   outer_tau_numer_(other.outer_tau_numer_),
   outer_tau_denom_(other.outer_tau_denom_),
   max_k_(other.max_k_),
+  allocator_(other.allocator_),
   gadget_(other.gadget_)
 {}
 
 template<typename T, typename A>
 var_opt_union<T, A>::var_opt_union(var_opt_union&& other) noexcept :
   n_(other.n_),
   outer_tau_numer_(other.outer_tau_numer_),
   outer_tau_denom_(other.outer_tau_denom_),
   max_k_(other.max_k_),
+  allocator_(other.allocator_),
   gadget_(std::move(other.gadget_))
 {}
 
 template<typename T, typename A>
 var_opt_union<T, A>::var_opt_union(uint64_t n, double outer_tau_numer, uint64_t outer_tau_denom,
-                                    uint32_t max_k, var_opt_sketch<T, A>&& gadget) :
+                                    uint32_t max_k, var_opt_sketch<T, A>&& gadget, const A& allocator) :
   n_(n),
   outer_tau_numer_(outer_tau_numer),
   outer_tau_denom_(outer_tau_denom),
   max_k_(max_k),
+  allocator_(allocator),
   gadget_(gadget)
 {}
 
 template<typename T, typename A>
 var_opt_union<T, A>::~var_opt_union() {}
 
 template<typename T, typename A>
 var_opt_union<T, A>& var_opt_union<T, A>::operator=(const var_opt_union& other) {
   var_opt_union union_copy(other);
   std::swap(n_, union_copy.n_);
   std::swap(outer_tau_numer_, union_copy.outer_tau_numer_);
   std::swap(outer_tau_denom_, union_copy.outer_tau_denom_);
   std::swap(max_k_, union_copy.max_k_);
+  std::swap(allocator_, other.allocator_);
   std::swap(gadget_, union_copy.gadget_);
   return *this;
 }
 
 template<typename T, typename A>
 var_opt_union<T, A>& var_opt_union<T, A>::operator=(var_opt_union&& other) {
   std::swap(n_, other.n_);
   std::swap(outer_tau_numer_, other.outer_tau_numer_);
   std::swap(outer_tau_denom_, other.outer_tau_denom_);
   std::swap(max_k_, other.max_k_);
+  std::swap(allocator_, other.allocator_);
   std::swap(gadget_, other.gadget_);
   return *this;
 }
 
 /*
  * An empty union requires 8 bytes.
  *
@@ -158,15 +164,15 @@
   const auto outer_tau_denom = read<uint64_t>(is);
 
   var_opt_sketch<T, A> gadget = var_opt_sketch<T, A>::deserialize(is, sd, allocator);
 
   if (!is.good())
     throw std::runtime_error("error reading from std::istream"); 
 
-  return var_opt_union(items_seen, outer_tau_numer, outer_tau_denom, max_k, std::move(gadget));
+  return var_opt_union(items_seen, outer_tau_numer, outer_tau_denom, max_k, std::move(gadget), allocator);
 }
 
 template<typename T, typename A>
 template<typename SerDe>
 var_opt_union<T, A> var_opt_union<T, A>::deserialize(const void* bytes, size_t size, const SerDe& sd, const A& allocator) {
   ensure_minimum_memory(size, 8);
   const char* ptr = static_cast<const char*>(bytes);
@@ -200,15 +206,15 @@
   ptr += copy_from_mem(ptr, outer_tau_numer);
   uint64_t outer_tau_denom;
   ptr += copy_from_mem(ptr, outer_tau_denom);
 
   const size_t gadget_size = size - (PREAMBLE_LONGS_NON_EMPTY << 3);
   var_opt_sketch<T, A> gadget = var_opt_sketch<T, A>::deserialize(ptr, gadget_size, sd, allocator);
 
-  return var_opt_union(items_seen, outer_tau_numer, outer_tau_denom, max_k, std::move(gadget));
+  return var_opt_union(items_seen, outer_tau_numer, outer_tau_denom, max_k, std::move(gadget), allocator);
 }
 
 template<typename T, typename A>
 template<typename SerDe>
 size_t var_opt_union<T, A>::get_serialized_size_bytes(const SerDe& sd) const {
   if (n_ == 0) {
     return PREAMBLE_LONGS_EMPTY << 3;
@@ -504,65 +510,63 @@
 void var_opt_union<T, A>::mark_moving_gadget_coercer(var_opt_sketch<T, A>& sk) const {
   const uint32_t result_k = gadget_.h_ + gadget_.r_;
 
   uint32_t result_h = 0;
   uint32_t result_r = 0;
   size_t next_r_pos = result_k; // = (result_k+1)-1, to fill R region from back to front
 
-  typedef typename std::allocator_traits<A>::template rebind_alloc<double> AllocDouble;
-  double* wts = AllocDouble().allocate(result_k + 1);
-  T* data     = A().allocate(result_k + 1);
+  double* wts = AllocDouble(allocator_).allocate(result_k + 1);
+  T* data     = A(allocator_).allocate(result_k + 1);
     
   // insert R region items, ignoring weights
   // Currently (May 2017) this next block is unreachable; this coercer is used only in the
   // pseudo-exact case in which case there are no items natively in R, only marked items in H
   // that will be moved into R as part of the coercion process.
   // Addedndum (Jan 2020): Cleanup at end of method assumes R count is 0
   const size_t final_idx = gadget_.get_num_samples();
   for (size_t idx = gadget_.h_ + 1; idx <= final_idx; ++idx) {
-    A().construct(&data[next_r_pos], T(gadget_.data_[idx]));
+    new (&data[next_r_pos]) T(gadget_.data_[idx]);
     wts[next_r_pos]  = gadget_.weights_[idx];
     ++result_r;
     --next_r_pos;
   }
   
   double transferred_weight = 0;
 
   // insert H region items
   for (size_t idx = 0; idx < gadget_.h_; ++idx) {
     if (gadget_.marks_[idx]) {
-      A().construct(&data[next_r_pos], T(gadget_.data_[idx]));
+      new (&data[next_r_pos]) T(gadget_.data_[idx]);
       wts[next_r_pos] = -1.0;
       transferred_weight += gadget_.weights_[idx];
       ++result_r;
       --next_r_pos;
     } else {
-      A().construct(&data[result_h], T(gadget_.data_[idx]));
+      new (&data[result_h]) T(gadget_.data_[idx]);
       wts[result_h] = gadget_.weights_[idx];
       ++result_h;
     }
   }
 
   if (result_h + result_r != result_k) throw std::logic_error("H + R counts must equal k");
-  if (fabs(transferred_weight - outer_tau_numer_) > 1e-10) {
+  if (std::abs(transferred_weight - outer_tau_numer_) > 1e-10) {
     throw std::logic_error("uexpected mismatch in transferred weight");
   }
 
   const double result_r_weight = gadget_.total_wt_r_ + transferred_weight;
   const uint64_t result_n = n_;
     
   // explicitly set weight value for the gap
   wts[result_h] = -1.0;
 
   // clean up arrays in input sketch, replace with new values
-  typedef typename std::allocator_traits<A>::template rebind_alloc<bool> AllocBool;
-  AllocBool().deallocate(sk.marks_, sk.curr_items_alloc_);
-  AllocDouble().deallocate(sk.weights_, sk.curr_items_alloc_);
-  for (size_t i = 0; i < result_k; ++i) { A().destroy(sk.data_ + i); } // assumes everything in H region, no gap
-  A().deallocate(sk.data_, sk.curr_items_alloc_);
+  AllocBool(allocator_).deallocate(sk.marks_, sk.curr_items_alloc_);
+  AllocDouble(allocator_).deallocate(sk.weights_, sk.curr_items_alloc_);
+  for (size_t i = 0; i < result_k; ++i) { sk.data_[i].~T(); } // assumes everything in H region, no gap
+  A(allocator_).deallocate(sk.data_, sk.curr_items_alloc_);
 
   sk.data_ = data;
   sk.weights_ = wts;
   sk.marks_ = nullptr;
   sk.num_marks_in_h_ = 0;
   sk.curr_items_alloc_ = result_k + 1;
   sk.k_ = result_k;
```

### Comparing `datasketches-4.0.1/sampling/test/CMakeLists.txt` & `datasketches-4.1.0/sampling/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/test/binaries_from_java.txt` & `datasketches-4.1.0/sampling/test/binaries_from_java.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/test/var_opt_allocation_test.cpp` & `datasketches-4.1.0/sampling/test/var_opt_allocation_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/test/var_opt_sketch_test.cpp` & `datasketches-4.1.0/sampling/test/var_opt_sketch_test.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -48,25 +48,23 @@
 }
 
 template<typename T, typename A>
 static void check_if_equal(var_opt_sketch<T, A>& sk1, var_opt_sketch<T, A>& sk2) {
   REQUIRE(sk1.get_k() == sk2.get_k());
   REQUIRE(sk1.get_n() == sk2.get_n());
   REQUIRE(sk1.get_num_samples() == sk2.get_num_samples());
-      
+
   auto it1 = sk1.begin();
   auto it2 = sk2.begin();
-  size_t i = 0;
 
   while ((it1 != sk1.end()) && (it2 != sk2.end())) {
-    const std::pair<const T&, const double> p1 = *it1;
-    const std::pair<const T&, const double> p2 = *it2;
+    auto p1 = *it1;
+    auto p2 = *it2;
     REQUIRE(p1.first == p2.first);   // data values
     REQUIRE(p1.second == p2.second); // weights
-    ++i;
     ++it1;
     ++it2;
   }
 
   REQUIRE((it1 == sk1.end() && it2 == sk2.end())); // iterators must end at the same time
 }
 
@@ -178,15 +176,15 @@
   REQUIRE_THROWS_AS(var_opt_sketch<std::string>::deserialize(bytes.data(), bytes.size()), std::invalid_argument);
 }
 
 TEST_CASE("varopt sketch: invalid weight", "[var_opt_sketch]") {
   var_opt_sketch<std::string> sk(100, resize_factor::X2);
   REQUIRE_THROWS_AS(sk.update("invalid_weight", -1.0), std::invalid_argument);
 
-  // should not throw but sketch shoulds till be empty
+  // should not throw but sketch should still be empty
   sk.update("zero weight", 0.0);
   REQUIRE(sk.is_empty());
 }
 
 TEST_CASE("varopt sketch: corrupt serialized weight", "[var_opt_sketch]") {
   var_opt_sketch<int> sk = create_unweighted_sketch(100, 20);
   auto bytes = sk.serialize();
@@ -209,28 +207,28 @@
 
   std::random_device rd; // possibly unsafe in MinGW with GCC < 9.2
   std::mt19937_64 rand(rd());
   std::normal_distribution<double> N(0.0, 1.0);
 
   double input_sum = 0.0;
   for (size_t i = 0; i < n; ++i) {
-    // generate weights aboev and below 1.0 using w ~ exp(5*N(0,1))
+    // generate weights above and below 1.0 using w ~ exp(5*N(0,1))
     // which covers about 10 orders of magnitude
     double w = std::exp(5 * N(rand));
     input_sum += w;
     sk.update(static_cast<int>(i), w);
   }
 
   double output_sum = 0.0;
-  for (auto it : sk) { // std::pair<int, weight>
-    output_sum += it.second;
+  for (auto pair : sk) { // std::pair<int, weight>
+    output_sum += pair.second;
   }
     
   double weight_ratio = output_sum / input_sum;
-  REQUIRE(std::abs(weight_ratio - 1.0) == Approx(0).margin(EPS));
+  REQUIRE(weight_ratio == Approx(1.0).margin(EPS));
 }
 
 TEST_CASE("varopt sketch: under-full sketch serialization", "[var_opt_sketch]") {
   var_opt_sketch<int> sk = create_unweighted_sketch(100, 10); // need n < k
 
   auto bytes = sk.serialize();
   var_opt_sketch<int> sk_from_bytes = var_opt_sketch<int>::deserialize(bytes.data(), bytes.size());
@@ -271,34 +269,46 @@
 }
 
 TEST_CASE("varopt sketch: full sketch serialization", "[var_opt_sketch]") {
   var_opt_sketch<int> sk = create_unweighted_sketch(32, 32);
   sk.update(100, 100.0);
   sk.update(101, 101.0);
 
+  subset_summary summary = sk.estimate_subset_sum([](int){ return true; });
+  double total_weight = summary.total_sketch_weight;
+  double cum_weight = 0.0;
+  for (auto pair : sk) {
+    cum_weight += pair.second;
+  }
+  double weight_ratio = cum_weight / total_weight;
+  REQUIRE(weight_ratio == Approx(1.0).margin(EPS));
+
   // first 2 entries should be heavy and in heap order (smallest at root)
   auto it = sk.begin();
-  const std::pair<const int, const double> p1 = *it;
+  auto p1 = *it;
   ++it;
-  const std::pair<const int, const double> p2 = *it;
+  auto p2 = *it;
   REQUIRE(p1.second == Approx(100.0).margin(EPS));
   REQUIRE(p2.second == Approx(101.0).margin(EPS));
   REQUIRE(p1.first == 100);
   REQUIRE(p2.first == 101);
+  // using operator ->
+  REQUIRE(it->first == p2.first);
+  REQUIRE(it->second == p2.second);
 
   // check for 4 preamble longs
   auto bytes = sk.serialize();
   REQUIRE((bytes.data()[0] & 0x3f) == 4);; // PREAMBLE_LONGS_WARMUP
 
-  var_opt_sketch<int> sk_from_bytes = var_opt_sketch<int>::deserialize(bytes.data(), bytes.size());
+  auto sk_from_bytes = var_opt_sketch<int>::deserialize(bytes.data(), bytes.size());
   check_if_equal(sk, sk_from_bytes);
 
   std::stringstream ss(std::ios::in | std::ios::out | std::ios::binary);
   sk.serialize(ss);
-  var_opt_sketch<int> sk_from_stream = var_opt_sketch<int>::deserialize(ss);
+  auto sk_from_stream = var_opt_sketch<int>::deserialize(ss);
   check_if_equal(sk, sk_from_stream);
 
   // ensure we unroll properly
   REQUIRE_THROWS_AS(var_opt_sketch<int>::deserialize(bytes.data(), bytes.size() - 100), std::out_of_range);
   std::string str_trunc((char*)&bytes[0], bytes.size() - 100);
   ss.str(str_trunc);
   REQUIRE_THROWS_AS(var_opt_sketch<int>::deserialize(ss), std::runtime_error);
@@ -336,14 +346,23 @@
 
   // check the first weight, assuming all k items are unweighted
   // (and consequently in R).
   // Expected: (k + 2) / |R| = (k + 2) / k
   auto it = sk.begin();
   double wt = (*it).second;
   REQUIRE(wt == Approx((k + 2.0) / k).margin(EPS));
+
+  subset_summary summary = sk.estimate_subset_sum([](int){ return true; });
+  double total_weight = summary.total_sketch_weight;
+  double cum_weight = 0.0;
+  for (auto pair : sk) {
+    cum_weight += pair.second;
+  }
+  double weight_ratio = cum_weight / total_weight;
+  REQUIRE(weight_ratio == Approx(1.0).margin(EPS));
 }
 
 TEST_CASE("varopt sketch: pseudo-heavy update", "[var_opt_sketch]") {
   uint32_t k = 1024;
   double wt_scale = 10.0 * k;
   var_opt_sketch<int> sk = create_unweighted_sketch(k, k + 1);
```

### Comparing `datasketches-4.0.1/sampling/test/var_opt_union_test.cpp` & `datasketches-4.1.0/sampling/test/var_opt_union_test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -53,24 +53,22 @@
 static void check_if_equal(var_opt_sketch<T, A>& sk1, var_opt_sketch<T, A>& sk2, bool exact_compare = true) {
   REQUIRE(sk1.get_k() == sk2.get_k());
   REQUIRE(sk1.get_n() == sk2.get_n());
   REQUIRE(sk1.get_num_samples() == sk2.get_num_samples());
       
   auto it1 = sk1.begin();
   auto it2 = sk2.begin();
-  size_t i = 0;
 
   while ((it1 != sk1.end()) && (it2 != sk2.end())) {
     const std::pair<const T&, const double> p1 = *it1;
     const std::pair<const T&, const double> p2 = *it2;
     if (exact_compare) {
       REQUIRE(p1.first == p2.first); // data values
     }
     REQUIRE(p1.second == p2.second); // weight values
-    ++i;
     ++it1;
     ++it2;
   }
 
   REQUIRE((it1 == sk1.end() && it2 == sk2.end())); // iterators must end at the same time
 }
```

### Comparing `datasketches-4.0.1/sampling/test/varopt_sketch_long_sampling.sk` & `datasketches-4.1.0/sampling/test/varopt_sketch_long_sampling.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/test/varopt_sketch_string_exact.sk` & `datasketches-4.1.0/sampling/test/varopt_sketch_string_exact.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/sampling/test/varopt_union_double_sampling.sk` & `datasketches-4.1.0/sampling/test/varopt_union_double_sampling.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/setup.py` & `datasketches-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     author='Apache Software Foundation',
     author_email='dev@datasketches.apache.org',
     description='The Apache DataSketches Library for Python',
     license='Apache License 2.0',
     url='http://datasketches.apache.org',
     long_description=open('python/README.md').read(),
     long_description_content_type='text/markdown',
-    packages=find_packages(where='python',exclude=['src','*tests*']), # src not needed if only the .so
+    packages=find_packages(where='python',exclude=['src','include','*tests*']), # src not needed if only the .so
     package_dir={'':'python'},
     # may need to add all source paths for sdist packages w/o MANIFEST.in
     ext_modules=[CMakeExtension('datasketches')],
     cmdclass={'build_ext': CMakeBuild},
     install_requires=['numpy'],
     zip_safe=False
 )
```

### Comparing `datasketches-4.0.1/theta/CMakeLists.txt` & `datasketches-4.1.0/theta/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,8 +58,9 @@
 			include/theta_set_difference_base.hpp
 			include/theta_set_difference_base_impl.hpp
 			include/theta_jaccard_similarity_base.hpp
 			include/bounds_on_ratios_in_sampled_sets.hpp
 			include/bounds_on_ratios_in_theta_sketched_sets.hpp
 			include/compact_theta_sketch_parser.hpp
 			include/compact_theta_sketch_parser_impl.hpp
+			include/bit_packing.hpp
   DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}/DataSketches")
```

### Comparing `datasketches-4.0.1/theta/include/bounds_on_ratios_in_sampled_sets.hpp` & `datasketches-4.1.0/theta/include/bounds_on_ratios_in_sampled_sets.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/bounds_on_ratios_in_theta_sketched_sets.hpp` & `datasketches-4.1.0/theta/include/bounds_on_ratios_in_theta_sketched_sets.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/compact_theta_sketch_parser.hpp` & `datasketches-4.1.0/theta/include/compact_theta_sketch_parser.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -16,51 +16,57 @@
  * specific language governing permissions and limitations
  * under the License.
  */
 
 #ifndef COMPACT_THETA_SKETCH_PARSER_HPP_
 #define COMPACT_THETA_SKETCH_PARSER_HPP_
 
-#include <stdint.h>
+#include <cstdint>
 
 namespace datasketches {
 
 template<bool dummy>
 class compact_theta_sketch_parser {
 public:
   struct compact_theta_sketch_data {
     bool is_empty;
     bool is_ordered;
     uint16_t seed_hash;
     uint32_t num_entries;
     uint64_t theta;
-    const uint64_t* entries;
+    const void* entries_start_ptr;
+    uint8_t entry_bits;
   };
 
   static compact_theta_sketch_data parse(const void* ptr, size_t size, uint64_t seed, bool dump_on_error = false);
 
 private:
   // offsets are in sizeof(type)
   static const size_t COMPACT_SKETCH_PRE_LONGS_BYTE = 0;
   static const size_t COMPACT_SKETCH_SERIAL_VERSION_BYTE = 1;
   static const size_t COMPACT_SKETCH_TYPE_BYTE = 2;
   static const size_t COMPACT_SKETCH_FLAGS_BYTE = 5;
   static const size_t COMPACT_SKETCH_SEED_HASH_U16 = 3;
-  static const size_t COMPACT_SKETCH_NUM_ENTRIES_U32 = 2;
-  static const size_t COMPACT_SKETCH_SINGLE_ENTRY_U64 = 1;
-  static const size_t COMPACT_SKETCH_ENTRIES_EXACT_U64 = 2;
-  static const size_t COMPACT_SKETCH_THETA_U64 = 2;
-  static const size_t COMPACT_SKETCH_ENTRIES_ESTIMATION_U64 = 3;
+  static const size_t COMPACT_SKETCH_SINGLE_ENTRY_U64 = 1; // ver 3
+  static const size_t COMPACT_SKETCH_NUM_ENTRIES_U32 = 2; // ver 1-3
+  static const size_t COMPACT_SKETCH_ENTRIES_EXACT_U64 = 2; // ver 1-3
+  static const size_t COMPACT_SKETCH_ENTRIES_ESTIMATION_U64 = 3; // ver 1-3
+  static const size_t COMPACT_SKETCH_THETA_U64 = 2; // ver 1-3
+  static const size_t COMPACT_SKETCH_V4_ENTRY_BITS_BYTE = 3;
+  static const size_t COMPACT_SKETCH_V4_NUM_ENTRIES_BYTES_BYTE = 4;
+  static const size_t COMPACT_SKETCH_V4_THETA_U64 = 1;
+  static const size_t COMPACT_SKETCH_V4_PACKED_DATA_EXACT_BYTE = 8;
+  static const size_t COMPACT_SKETCH_V4_PACKED_DATA_ESTIMATION_BYTE = 16;
 
   static const uint8_t COMPACT_SKETCH_IS_EMPTY_FLAG = 2;
   static const uint8_t COMPACT_SKETCH_IS_ORDERED_FLAG = 4;
 
-  static const uint8_t COMPACT_SKETCH_SERIAL_VERSION = 3;
   static const uint8_t COMPACT_SKETCH_TYPE = 3;
 
+  static void check_memory_size(const void* ptr, size_t actual_bytes, size_t expected_bytes, bool dump_on_error);
   static std::string hex_dump(const uint8_t* ptr, size_t size);
 };
 
 } /* namespace datasketches */
 
 #include "compact_theta_sketch_parser_impl.hpp"
```

### Comparing `datasketches-4.0.1/theta/include/compact_theta_sketch_parser_impl.hpp` & `datasketches-4.1.0/theta/include/compact_theta_sketch_parser_impl.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -22,115 +22,129 @@
 
 #include <iostream>
 #include <iomanip>
 #include <stdexcept>
 
 namespace datasketches {
 
+template<typename T>
+T whole_bytes_to_hold_bits(T bits) {
+  static_assert(std::is_integral<T>::value, "integral type expected");
+  return (bits >> 3) + ((bits & 7) > 0);
+}
+
 template<bool dummy>
 auto compact_theta_sketch_parser<dummy>::parse(const void* ptr, size_t size, uint64_t seed, bool dump_on_error) -> compact_theta_sketch_data {
-  if (size < 8) throw std::out_of_range("at least 8 bytes expected, actual " + std::to_string(size)
-      + (dump_on_error ? (", sketch dump: " + hex_dump(reinterpret_cast<const uint8_t*>(ptr), size)) : ""));
-
+  check_memory_size(ptr, size, 8, dump_on_error);
+  checker<true>::check_sketch_type(reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_TYPE_BYTE], COMPACT_SKETCH_TYPE);
   uint8_t serial_version = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_SERIAL_VERSION_BYTE];
-
   switch(serial_version) {
-  case COMPACT_SKETCH_SERIAL_VERSION: {
-      checker<true>::check_sketch_type(reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_TYPE_BYTE], COMPACT_SKETCH_TYPE);
+  case 4: {
+    // version 4 sketches are ordered and always have entries (single item in exact mode is v3)
+    const uint16_t seed_hash = reinterpret_cast<const uint16_t*>(ptr)[COMPACT_SKETCH_SEED_HASH_U16];
+    checker<true>::check_seed_hash(seed_hash, compute_seed_hash(seed));
+    const bool has_theta = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_PRE_LONGS_BYTE] > 1;
+    uint64_t theta = theta_constants::MAX_THETA;
+    if (has_theta) {
+      check_memory_size(ptr, size, 16, dump_on_error);
+      theta = reinterpret_cast<const uint64_t*>(ptr)[COMPACT_SKETCH_V4_THETA_U64];
+    }
+    const uint8_t num_entries_bytes = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_V4_NUM_ENTRIES_BYTES_BYTE];
+    size_t data_offset_bytes = has_theta ? COMPACT_SKETCH_V4_PACKED_DATA_ESTIMATION_BYTE : COMPACT_SKETCH_V4_PACKED_DATA_EXACT_BYTE;
+    check_memory_size(ptr, size, data_offset_bytes + num_entries_bytes, dump_on_error);
+    uint32_t num_entries = 0;
+    const uint8_t* num_entries_ptr = reinterpret_cast<const uint8_t*>(ptr) + data_offset_bytes;
+    for (unsigned i = 0; i < num_entries_bytes; ++i) {
+      num_entries |= (*num_entries_ptr++) << (i << 3);
+    }
+    data_offset_bytes += num_entries_bytes;
+    const uint8_t entry_bits = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_V4_ENTRY_BITS_BYTE];
+    const size_t expected_bits = entry_bits * num_entries;
+    const size_t expected_size_bytes = data_offset_bytes + whole_bytes_to_hold_bits(expected_bits);
+    check_memory_size(ptr, size, expected_size_bytes, dump_on_error);
+    return {false, true, seed_hash, num_entries, theta,
+      reinterpret_cast<const uint8_t*>(ptr) + data_offset_bytes, entry_bits};
+  }
+  case 3: {
       uint64_t theta = theta_constants::MAX_THETA;
       const uint16_t seed_hash = reinterpret_cast<const uint16_t*>(ptr)[COMPACT_SKETCH_SEED_HASH_U16];
       if (reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_FLAGS_BYTE] & (1 << COMPACT_SKETCH_IS_EMPTY_FLAG)) {
-        return {true, true, seed_hash, 0, theta, nullptr};
+        return {true, true, seed_hash, 0, theta, nullptr, 64};
       }
       checker<true>::check_seed_hash(seed_hash, compute_seed_hash(seed));
       const bool has_theta = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_PRE_LONGS_BYTE] > 2;
       if (has_theta) {
-        if (size < 16) throw std::out_of_range("at least 16 bytes expected, actual " + std::to_string(size));
+        check_memory_size(ptr, size, (COMPACT_SKETCH_THETA_U64 + 1) * sizeof(uint64_t), dump_on_error);
         theta = reinterpret_cast<const uint64_t*>(ptr)[COMPACT_SKETCH_THETA_U64];
       }
       if (reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_PRE_LONGS_BYTE] == 1) {
-        if (size < 16) throw std::out_of_range("at least 16 bytes expected, actual " + std::to_string(size));
-        return {false, true, seed_hash, 1, theta, reinterpret_cast<const uint64_t*>(ptr) + COMPACT_SKETCH_SINGLE_ENTRY_U64};
+        check_memory_size(ptr, size, 16, dump_on_error);
+        return {false, true, seed_hash, 1, theta, reinterpret_cast<const uint64_t*>(ptr) + COMPACT_SKETCH_SINGLE_ENTRY_U64, 64};
       }
       const uint32_t num_entries = reinterpret_cast<const uint32_t*>(ptr)[COMPACT_SKETCH_NUM_ENTRIES_U32];
       const size_t entries_start_u64 = has_theta ? COMPACT_SKETCH_ENTRIES_ESTIMATION_U64 : COMPACT_SKETCH_ENTRIES_EXACT_U64;
       const uint64_t* entries = reinterpret_cast<const uint64_t*>(ptr) + entries_start_u64;
       const size_t expected_size_bytes = (entries_start_u64 + num_entries) * sizeof(uint64_t);
-      if (size < expected_size_bytes) {
-        throw std::out_of_range(std::to_string(expected_size_bytes) + " bytes expected, actual " + std::to_string(size)
-            + (dump_on_error ? (", sketch dump: " + hex_dump(reinterpret_cast<const uint8_t*>(ptr), size)) : ""));
-      }
+      check_memory_size(ptr, size, expected_size_bytes, dump_on_error);
       const bool is_ordered = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_FLAGS_BYTE] & (1 << COMPACT_SKETCH_IS_ORDERED_FLAG);
-      return {false, is_ordered, seed_hash, num_entries, theta, entries};
+      return {false, is_ordered, seed_hash, num_entries, theta, entries, 64};
   }
   case 1:  {
       uint16_t seed_hash = compute_seed_hash(seed);
-      checker<true>::check_sketch_type(reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_TYPE_BYTE], COMPACT_SKETCH_TYPE);
       const uint32_t num_entries = reinterpret_cast<const uint32_t*>(ptr)[COMPACT_SKETCH_NUM_ENTRIES_U32];
       uint64_t theta = reinterpret_cast<const uint64_t*>(ptr)[COMPACT_SKETCH_THETA_U64];
       bool is_empty = (num_entries == 0) && (theta == theta_constants::MAX_THETA);
-      if (is_empty) {
-          return {true, true, seed_hash, 0, theta, nullptr};
-      }
+      if (is_empty) return {true, true, seed_hash, 0, theta, nullptr, 64};
       const uint64_t* entries = reinterpret_cast<const uint64_t*>(ptr) + COMPACT_SKETCH_ENTRIES_ESTIMATION_U64;
       const size_t expected_size_bytes = (COMPACT_SKETCH_ENTRIES_ESTIMATION_U64 + num_entries) * sizeof(uint64_t);
-      if (size < expected_size_bytes) {
-        throw std::out_of_range(std::to_string(expected_size_bytes) + " bytes expected, actual " + std::to_string(size)
-            + (dump_on_error ? (", sketch dump: " + hex_dump(reinterpret_cast<const uint8_t*>(ptr), size)) : ""));
-      }
-      return {false, true, seed_hash, num_entries, theta, entries};
+      check_memory_size(ptr, size, expected_size_bytes, dump_on_error);
+      return {false, true, seed_hash, num_entries, theta, entries, 64};
   }
   case 2:  {
-      uint8_t preamble_size =  reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_PRE_LONGS_BYTE];
-      checker<true>::check_sketch_type(reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_TYPE_BYTE], COMPACT_SKETCH_TYPE);
+      uint8_t preamble_size = reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_PRE_LONGS_BYTE];
       const uint16_t seed_hash = reinterpret_cast<const uint16_t*>(ptr)[COMPACT_SKETCH_SEED_HASH_U16];
       checker<true>::check_seed_hash(seed_hash, compute_seed_hash(seed));
       if (preamble_size == 1) {
-          return {true, true, seed_hash, 0, theta_constants::MAX_THETA, nullptr};
+          return {true, true, seed_hash, 0, theta_constants::MAX_THETA, nullptr, 64};
       } else if (preamble_size == 2) {
           const uint32_t num_entries = reinterpret_cast<const uint32_t*>(ptr)[COMPACT_SKETCH_NUM_ENTRIES_U32];
           if (num_entries == 0) {
-              return {true, true, seed_hash, 0, theta_constants::MAX_THETA, nullptr};
+              return {true, true, seed_hash, 0, theta_constants::MAX_THETA, nullptr, 64};
           } else {
               const size_t expected_size_bytes = (preamble_size + num_entries) << 3;
-              if (size < expected_size_bytes) {
-                  throw std::out_of_range(std::to_string(expected_size_bytes) + " bytes expected, actual " + std::to_string(size)
-                      + (dump_on_error ? (", sketch dump: " + hex_dump(reinterpret_cast<const uint8_t*>(ptr), size)) : ""));
-              }
+              check_memory_size(ptr, size, expected_size_bytes, dump_on_error);
               const uint64_t* entries = reinterpret_cast<const uint64_t*>(ptr) + COMPACT_SKETCH_ENTRIES_EXACT_U64;
-              return {false, true, seed_hash, num_entries, theta_constants::MAX_THETA, entries};
+              return {false, true, seed_hash, num_entries, theta_constants::MAX_THETA, entries, 64};
           }
       } else if (preamble_size == 3) {
           const uint32_t num_entries = reinterpret_cast<const uint32_t*>(ptr)[COMPACT_SKETCH_NUM_ENTRIES_U32];
           uint64_t theta = reinterpret_cast<const uint64_t*>(ptr)[COMPACT_SKETCH_THETA_U64];
           bool is_empty = (num_entries == 0) && (theta == theta_constants::MAX_THETA);
-          if (is_empty) {
-              return {true, true, seed_hash, 0, theta, nullptr};
-          }
+          if (is_empty) return {true, true, seed_hash, 0, theta, nullptr, 64};
           const uint64_t* entries = reinterpret_cast<const uint64_t*>(ptr) + COMPACT_SKETCH_ENTRIES_ESTIMATION_U64;
           const size_t expected_size_bytes = (COMPACT_SKETCH_ENTRIES_ESTIMATION_U64 + num_entries) * sizeof(uint64_t);
-          if (size < expected_size_bytes) {
-            throw std::out_of_range(std::to_string(expected_size_bytes) + " bytes expected, actual " + std::to_string(size)
-                + (dump_on_error ? (", sketch dump: " + hex_dump(reinterpret_cast<const uint8_t*>(ptr), size)) : ""));
-          }
-          return {false, true, seed_hash, num_entries, theta, entries};
+          check_memory_size(ptr, size, expected_size_bytes, dump_on_error);
+          return {false, true, seed_hash, num_entries, theta, entries, 64};
       } else {
           throw std::invalid_argument(std::to_string(preamble_size) + " longs of premable, but expected 1, 2, or 3");
       }
   }
   default:
-      // this should always fail since the valid cases are handled above
-      checker<true>::check_serial_version(reinterpret_cast<const uint8_t*>(ptr)[COMPACT_SKETCH_SERIAL_VERSION_BYTE], COMPACT_SKETCH_SERIAL_VERSION);
-      // this throw is never reached, because check_serial_version will throw an informative exception.
-      // This is only here to avoid a compiler warning about a path without a return value.
-      throw std::invalid_argument("unexpected sketch serialization version");
+    throw std::invalid_argument("unsupported serial version " + std::to_string(serial_version));
   }
 }
 
 template<bool dummy>
+void compact_theta_sketch_parser<dummy>::check_memory_size(const void* ptr, size_t actual_bytes, size_t expected_bytes, bool dump_on_error) {
+  if (actual_bytes < expected_bytes) throw std::out_of_range("at least " + std::to_string(expected_bytes)
+      + " bytes expected, actual " + std::to_string(actual_bytes)
+      + (dump_on_error ? (", sketch dump: " + hex_dump(reinterpret_cast<const uint8_t*>(ptr), actual_bytes)) : ""));
+}
+
+template<bool dummy>
 std::string compact_theta_sketch_parser<dummy>::hex_dump(const uint8_t* ptr, size_t size) {
   std::stringstream s;
   s << std::hex << std::setfill('0') << std::uppercase;
   for (size_t i = 0; i < size; ++i) s << std::setw(2) << (ptr[i] & 0xff);
   return s.str();
 }
```

### Comparing `datasketches-4.0.1/theta/include/theta_a_not_b.hpp` & `datasketches-4.1.0/theta/include/theta_a_not_b.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_a_not_b_impl.hpp` & `datasketches-4.1.0/theta/include/theta_a_not_b_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_comparators.hpp` & `datasketches-4.1.0/theta/include/theta_comparators.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_constants.hpp` & `datasketches-4.1.0/theta/include/theta_constants.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_helpers.hpp` & `datasketches-4.1.0/theta/include/theta_helpers.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,18 @@
  * specific language governing permissions and limitations
  * under the License.
  */
 
 #ifndef THETA_HELPERS_HPP_
 #define THETA_HELPERS_HPP_
 
-#include <string>
 #include <stdexcept>
+#include <string>
+
+#include "theta_constants.hpp"
 
 namespace datasketches {
 
 template<typename T>
 static void check_value(T actual, T expected, const char* description) {
   if (actual != expected) {
     throw std::invalid_argument(std::string(description) + " mismatch: expected " + std::to_string(expected) + ", actual " + std::to_string(actual));
@@ -51,15 +53,15 @@
 
 template<bool dummy>
 class theta_build_helper{
 public:
   // consistent way of initializing theta from p
   // avoids multiplication if p == 1 since it might not yield MAX_THETA exactly
   static uint64_t starting_theta_from_p(float p) {
-    if (p < 1) return static_cast<uint64_t>(theta_constants::MAX_THETA * p);
+    if (p < 1) return static_cast<float>(theta_constants::MAX_THETA) * p;
     return theta_constants::MAX_THETA;
   }
 
   static uint8_t starting_sub_multiple(uint8_t lg_tgt, uint8_t lg_min, uint8_t lg_rf) {
     return (lg_tgt <= lg_min) ? lg_min : (lg_rf == 0) ? lg_tgt : ((lg_tgt - lg_min) % lg_rf) + lg_min;
   }
 };
```

### Comparing `datasketches-4.0.1/theta/include/theta_intersection.hpp` & `datasketches-4.1.0/theta/include/theta_intersection.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_intersection_base.hpp` & `datasketches-4.1.0/theta/include/theta_intersection_base.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_intersection_base_impl.hpp` & `datasketches-4.1.0/theta/include/theta_intersection_base_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_intersection_impl.hpp` & `datasketches-4.1.0/theta/include/theta_intersection_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_jaccard_similarity.hpp` & `datasketches-4.1.0/theta/include/theta_jaccard_similarity.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_jaccard_similarity_base.hpp` & `datasketches-4.1.0/theta/include/theta_jaccard_similarity_base.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_set_difference_base.hpp` & `datasketches-4.1.0/theta/include/theta_set_difference_base.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_set_difference_base_impl.hpp` & `datasketches-4.1.0/theta/include/theta_set_difference_base_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_sketch.hpp` & `datasketches-4.1.0/theta/include/theta_sketch.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
  * under the License.
  */
 
 #ifndef THETA_SKETCH_HPP_
 #define THETA_SKETCH_HPP_
 
 #include "theta_update_sketch_base.hpp"
+#include "compact_theta_sketch_parser.hpp"
 
 namespace datasketches {
 
 template<typename Allocator = std::allocator<uint64_t>>
 class base_theta_sketch_alloc {
 public:
 
@@ -313,15 +314,16 @@
 public:
   using Base = theta_sketch_alloc<Allocator>;
   using iterator = typename Base::iterator;
   using const_iterator = typename Base::const_iterator;
   using AllocBytes = typename std::allocator_traits<Allocator>::template rebind_alloc<uint8_t>;
   using vector_bytes = std::vector<uint8_t, AllocBytes>;
 
-  static const uint8_t SERIAL_VERSION = 3;
+  static const uint8_t UNCOMPRESSED_SERIAL_VERSION = 3;
+  static const uint8_t COMPRESSED_SERIAL_VERSION = 4;
   static const uint8_t SKETCH_TYPE = 3;
 
   // Instances of this type can be obtained:
   // - by compacting an update_theta_sketch_alloc
   // - as a result of a set operation
   // - by deserializing a previously serialized compact sketch
 
@@ -351,14 +353,33 @@
    * An optional header can be reserved in front of the sketch.
    * It is an uninitialized space of a given size.
    * This header is used in Datasketches PostgreSQL extension.
    * @param header_size_bytes space to reserve in front of the sketch
    */
   vector_bytes serialize(unsigned header_size_bytes = 0) const;
 
+  /**
+   * This method serializes the sketch into a given stream in a compressed binary form.
+   * Compression is applied to ordered sketches except empty and single item.
+   * For unordered, empty and single item sketches this method is equivalent to serialize()
+   * @param os output stream
+   */
+  void serialize_compressed(std::ostream& os) const;
+
+  /**
+   * This method serializes the sketch as a vector of bytes.
+   * An optional header can be reserved in front of the sketch.
+   * It is an uninitialized space of a given size.
+   * This header is used in Datasketches PostgreSQL extension.
+   * Compression is applied to ordered sketches except empty and single item.
+   * For unordered, empty and single item sketches this method is equivalent to serialize()
+   * @param header_size_bytes space to reserve in front of the sketch
+   */
+  vector_bytes serialize_compressed(unsigned header_size_bytes = 0) const;
+
   virtual iterator begin();
   virtual iterator end();
   virtual const_iterator begin() const;
   virtual const_iterator end() const;
 
   /**
    * This method deserializes a sketch from a given stream.
@@ -387,14 +408,24 @@
 
   bool is_empty_;
   bool is_ordered_;
   uint16_t seed_hash_;
   uint64_t theta_;
   std::vector<uint64_t, Allocator> entries_;
 
+  bool is_suitable_for_compression() const;
+  uint8_t compute_min_leading_zeros() const;
+  void serialize_version_4(std::ostream& os) const;
+  vector_bytes serialize_version_4(unsigned header_size_bytes = 0) const;
+
+  static compact_theta_sketch_alloc deserialize_v1(uint8_t preamble_longs, std::istream& is, uint64_t seed, const Allocator& allocator);
+  static compact_theta_sketch_alloc deserialize_v2(uint8_t preamble_longs, std::istream& is, uint64_t seed, const Allocator& allocator);
+  static compact_theta_sketch_alloc deserialize_v3(uint8_t preamble_longs, std::istream& is, uint64_t seed, const Allocator& allocator);
+  static compact_theta_sketch_alloc deserialize_v4(uint8_t preamble_longs, std::istream& is, uint64_t seed, const Allocator& allocator);
+
   virtual void print_specifics(std::ostringstream& os) const;
 };
 
 template<typename Allocator>
 class update_theta_sketch_alloc<Allocator>::builder: public theta_base_builder<builder, Allocator> {
 public:
     builder(const Allocator& allocator = Allocator());
@@ -403,15 +434,15 @@
 
 // This is to wrap a buffer containing a serialized compact sketch and use it in a set operation avoiding some cost of deserialization.
 // It does not take the ownership of the buffer.
 
 template<typename Allocator = std::allocator<uint64_t>>
 class wrapped_compact_theta_sketch_alloc : public base_theta_sketch_alloc<Allocator> {
 public:
-  using const_iterator = const uint64_t*;
+  class const_iterator;
 
   Allocator get_allocator() const;
   bool is_empty() const;
   bool is_ordered() const;
   uint64_t get_theta64() const;
   uint32_t get_num_retained() const;
   uint16_t get_seed_hash() const;
@@ -429,23 +460,40 @@
   static const wrapped_compact_theta_sketch_alloc wrap(const void* bytes, size_t size, uint64_t seed = DEFAULT_SEED, bool dump_on_error = false);
 
 protected:
   virtual void print_specifics(std::ostringstream& os) const;
   virtual void print_items(std::ostringstream& os) const;
 
 private:
-  bool is_empty_;
-  bool is_ordered_;
-  uint16_t seed_hash_;
-  uint32_t num_entries_;
-  uint64_t theta_;
-  const uint64_t* entries_;
+  using data_type = compact_theta_sketch_parser<true>::compact_theta_sketch_data;
+  data_type data_;
 
-  wrapped_compact_theta_sketch_alloc(bool is_empty, bool is_ordered, uint16_t seed_hash, uint32_t num_entries,
-      uint64_t theta, const uint64_t* entries);
+  wrapped_compact_theta_sketch_alloc(const data_type& data);
+};
+
+template<typename Allocator>
+class wrapped_compact_theta_sketch_alloc<Allocator>::const_iterator: public std::iterator<std::input_iterator_tag, uint64_t> {
+public:
+  const_iterator(const void* ptr, uint8_t entry_bits, uint32_t num_entries, uint32_t index);
+  const_iterator& operator++();
+  const_iterator operator++(int);
+  bool operator==(const const_iterator& other) const;
+  bool operator!=(const const_iterator& other) const;
+  const uint64_t& operator*() const;
+  const uint64_t* operator->() const;
+private:
+  const void* ptr_;
+  uint8_t entry_bits_;
+  uint32_t num_entries_;
+  uint32_t index_;
+  uint64_t previous_;
+  bool is_block_mode_;
+  uint8_t buf_i_;
+  uint8_t offset_;
+  uint64_t buffer_[8];
 };
 
 // aliases with default allocator for convenience
 using theta_sketch = theta_sketch_alloc<std::allocator<uint64_t>>;
 using update_theta_sketch = update_theta_sketch_alloc<std::allocator<uint64_t>>;
 using compact_theta_sketch = compact_theta_sketch_alloc<std::allocator<uint64_t>>;
 using wrapped_compact_theta_sketch = wrapped_compact_theta_sketch_alloc<std::allocator<uint64_t>>;
```

### Comparing `datasketches-4.0.1/theta/include/theta_union.hpp` & `datasketches-4.1.0/theta/include/theta_union.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_union_base.hpp` & `datasketches-4.1.0/theta/include/theta_union_base.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_union_base_impl.hpp` & `datasketches-4.1.0/theta/include/theta_union_base_impl.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -37,48 +37,48 @@
 
 template<typename EN, typename EK, typename P, typename S, typename CS, typename A>
 template<typename SS>
 void theta_union_base<EN, EK, P, S, CS, A>::update(SS&& sketch) {
   if (sketch.is_empty()) return;
   if (sketch.get_seed_hash() != compute_seed_hash(table_.seed_)) throw std::invalid_argument("seed hash mismatch");
   table_.is_empty_ = false;
-  if (sketch.get_theta64() < union_theta_) union_theta_ = sketch.get_theta64();
+  union_theta_ = std::min(union_theta_, sketch.get_theta64());
   for (auto& entry: sketch) {
     const uint64_t hash = EK()(entry);
     if (hash < union_theta_ && hash < table_.theta_) {
       auto result = table_.find(hash);
       if (!result.second) {
         table_.insert(result.first, conditional_forward<SS>(entry));
       } else {
         policy_(*result.first, conditional_forward<SS>(entry));
       }
     } else {
       if (sketch.is_ordered()) break; // early stop
     }
   }
-  if (table_.theta_ < union_theta_) union_theta_ = table_.theta_;
+  union_theta_ = std::min(union_theta_, table_.theta_);
 }
 
 template<typename EN, typename EK, typename P, typename S, typename CS, typename A>
 CS theta_union_base<EN, EK, P, S, CS, A>::get_result(bool ordered) const {
   std::vector<EN, A> entries(table_.allocator_);
   if (table_.is_empty_) return CS(true, true, compute_seed_hash(table_.seed_), union_theta_, std::move(entries));
   entries.reserve(table_.num_entries_);
   uint64_t theta = std::min(union_theta_, table_.theta_);
   const uint32_t nominal_num = 1 << table_.lg_nom_size_;
-  if (union_theta_ >= theta && table_.num_entries_ <= nominal_num) {
+  if (union_theta_ >= table_.theta_) {
     std::copy_if(table_.begin(), table_.end(), std::back_inserter(entries), key_not_zero<EN, EK>());
   } else {
     std::copy_if(table_.begin(), table_.end(), std::back_inserter(entries), key_not_zero_less_than<uint64_t, EN, EK>(theta));
-    if (entries.size() > nominal_num) {
-      std::nth_element(entries.begin(), entries.begin() + nominal_num, entries.end(), comparator());
-      theta = EK()(entries[nominal_num]);
-      entries.erase(entries.begin() + nominal_num, entries.end());
-      entries.shrink_to_fit();
-    }
+  }
+  if (entries.size() > nominal_num) {
+    std::nth_element(entries.begin(), entries.begin() + nominal_num, entries.end(), comparator());
+    theta = EK()(entries[nominal_num]);
+    entries.erase(entries.begin() + nominal_num, entries.end());
+    entries.shrink_to_fit();
   }
   if (ordered) std::sort(entries.begin(), entries.end(), comparator());
   return CS(table_.is_empty_, ordered, compute_seed_hash(table_.seed_), theta, std::move(entries));
 }
 
 template<typename EN, typename EK, typename P, typename S, typename CS, typename A>
 const P& theta_union_base<EN, EK, P, S, CS, A>::get_policy() const {
```

### Comparing `datasketches-4.0.1/theta/include/theta_union_impl.hpp` & `datasketches-4.1.0/theta/include/theta_union_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/include/theta_update_sketch_base.hpp` & `datasketches-4.1.0/theta/include/theta_update_sketch_base.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 #ifndef THETA_UPDATE_SKETCH_BASE_HPP_
 #define THETA_UPDATE_SKETCH_BASE_HPP_
 
 #include <vector>
 #include <climits>
 #include <cmath>
+#include <iterator>
 
-#include "common_defs.hpp"
 #include "MurmurHash3.h"
 #include "theta_comparators.hpp"
 #include "theta_constants.hpp"
 
 namespace datasketches {
 
 template<
@@ -181,38 +181,50 @@
   MurmurHash3_x64_128(data, length, seed, hashes);
   return (hashes.h1 >> 1); // Java implementation does unsigned shift >>> to make values positive
 }
 
 // iterators
 
 template<typename Entry, typename ExtractKey>
-class theta_iterator: public std::iterator<std::input_iterator_tag, Entry> {
+class theta_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = Entry;
+  using difference_type = std::ptrdiff_t;
+  using pointer = Entry*;
+  using reference = Entry&;
+
   theta_iterator(Entry* entries, uint32_t size, uint32_t index);
   theta_iterator& operator++();
   theta_iterator operator++(int);
   bool operator==(const theta_iterator& other) const;
   bool operator!=(const theta_iterator& other) const;
   Entry& operator*() const;
 
 private:
   Entry* entries_;
   uint32_t size_;
   uint32_t index_;
 };
 
 template<typename Entry, typename ExtractKey>
-class theta_const_iterator: public std::iterator<std::input_iterator_tag, Entry> {
+class theta_const_iterator {
 public:
+  using iterator_category = std::input_iterator_tag;
+  using value_type = const Entry;
+  using difference_type = std::ptrdiff_t;
+  using pointer = const Entry*;
+  using reference = const Entry&;
+
   theta_const_iterator(const Entry* entries, uint32_t size, uint32_t index);
   theta_const_iterator& operator++();
   theta_const_iterator operator++(int);
   bool operator==(const theta_const_iterator& other) const;
   bool operator!=(const theta_const_iterator& other) const;
-  const Entry& operator*() const;
+  reference operator*() const;
 
 private:
   const Entry* entries_;
   uint32_t size_;
   uint32_t index_;
 };
```

### Comparing `datasketches-4.0.1/theta/include/theta_update_sketch_base_impl.hpp` & `datasketches-4.1.0/theta/include/theta_update_sketch_base_impl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 template<typename EN, typename EK, typename A>
 auto theta_update_sketch_base<EN, EK, A>::begin() const -> iterator {
   return entries_;
 }
 
 template<typename EN, typename EK, typename A>
 auto theta_update_sketch_base<EN, EK, A>::end() const -> iterator {
-  return &entries_[1ULL << lg_cur_size_];
+  return entries_ + (1ULL << lg_cur_size_);
 }
 
 template<typename EN, typename EK, typename A>
 uint32_t theta_update_sketch_base<EN, EK, A>::get_capacity(uint8_t lg_cur_size, uint8_t lg_nom_size) {
   const double fraction = (lg_cur_size <= lg_nom_size) ? RESIZE_THRESHOLD : REBUILD_THRESHOLD;
   return static_cast<uint32_t>(std::floor(fraction * (1 << lg_cur_size)));
 }
@@ -378,15 +378,15 @@
 
 template<typename Entry, typename ExtractKey>
 bool theta_iterator<Entry, ExtractKey>::operator==(const theta_iterator& other) const {
   return index_ == other.index_;
 }
 
 template<typename Entry, typename ExtractKey>
-auto theta_iterator<Entry, ExtractKey>::operator*() const -> Entry& {
+auto theta_iterator<Entry, ExtractKey>::operator*() const -> reference {
   return entries_[index_];
 }
 
 // const iterator
 
 template<typename Entry, typename ExtractKey>
 theta_const_iterator<Entry, ExtractKey>::theta_const_iterator(const Entry* entries, uint32_t size, uint32_t index):
```

### Comparing `datasketches-4.0.1/theta/test/CMakeLists.txt` & `datasketches-4.1.0/theta/test/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,9 @@
   PRIVATE
     theta_sketch_test.cpp
     theta_union_test.cpp
     theta_intersection_test.cpp
     theta_a_not_b_test.cpp
     theta_jaccard_similarity_test.cpp
     theta_setop_test.cpp
+    bit_packing_test.cpp
 )
```

### Comparing `datasketches-4.0.1/theta/test/theta_a_not_b_test.cpp` & `datasketches-4.1.0/theta/test/theta_a_not_b_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_compact_estimation_from_java.sk` & `datasketches-4.1.0/theta/test/theta_compact_estimation_from_java.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_compact_estimation_from_java_v1.sk` & `datasketches-4.1.0/theta/test/theta_compact_estimation_from_java_v1.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_compact_estimation_from_java_v2.sk` & `datasketches-4.1.0/theta/test/theta_compact_estimation_from_java_v2.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_compact_exact_from_java.sk` & `datasketches-4.1.0/theta/test/theta_compact_exact_from_java.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_intersection_test.cpp` & `datasketches-4.1.0/theta/test/theta_intersection_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_jaccard_similarity_test.cpp` & `datasketches-4.1.0/theta/test/theta_jaccard_similarity_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_setop_test.cpp` & `datasketches-4.1.0/theta/test/theta_setop_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/theta/test/theta_sketch_test.cpp` & `datasketches-4.1.0/theta/test/theta_sketch_test.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -603,15 +603,15 @@
   REQUIRE(sketch.get_lower_bound(2) == Approx(update_sketch.get_lower_bound(2)).margin(1e-10));
   REQUIRE(sketch.get_upper_bound(2) == Approx(update_sketch.get_upper_bound(2)).margin(1e-10));
   REQUIRE(sketch.get_lower_bound(3) == Approx(update_sketch.get_lower_bound(3)).margin(1e-10));
   REQUIRE(sketch.get_upper_bound(3) == Approx(update_sketch.get_upper_bound(3)).margin(1e-10));
   compact_theta_sketch compact_sketch = update_sketch.compact();
   // the sketches are ordered, so the iteration sequence must match exactly
   auto iter = sketch.begin();
-  for (const auto& key: compact_sketch) {
+  for (const auto key: compact_sketch) {
     REQUIRE(*iter == key);
     ++iter;
   }
 }
 
 TEST_CASE("theta sketch: wrap compact v1 estimation from java", "[theta_sketch]") {
   std::ifstream is;
@@ -648,15 +648,15 @@
   REQUIRE(sketch.get_lower_bound(2) == Approx(update_sketch.get_lower_bound(2)).margin(1e-10));
   REQUIRE(sketch.get_upper_bound(2) == Approx(update_sketch.get_upper_bound(2)).margin(1e-10));
   REQUIRE(sketch.get_lower_bound(3) == Approx(update_sketch.get_lower_bound(3)).margin(1e-10));
   REQUIRE(sketch.get_upper_bound(3) == Approx(update_sketch.get_upper_bound(3)).margin(1e-10));
   compact_theta_sketch compact_sketch = update_sketch.compact();
   // the sketches are ordered, so the iteration sequence must match exactly
   auto iter = sketch.begin();
-  for (const auto& key: compact_sketch) {
+  for (const auto key: compact_sketch) {
     REQUIRE(*iter == key);
     ++iter;
   }
 }
 
 TEST_CASE("theta sketch: wrap compact v2 estimation from java", "[theta_sketch]") {
   std::ifstream is;
@@ -693,14 +693,53 @@
   REQUIRE(sketch.get_lower_bound(2) == Approx(update_sketch.get_lower_bound(2)).margin(1e-10));
   REQUIRE(sketch.get_upper_bound(2) == Approx(update_sketch.get_upper_bound(2)).margin(1e-10));
   REQUIRE(sketch.get_lower_bound(3) == Approx(update_sketch.get_lower_bound(3)).margin(1e-10));
   REQUIRE(sketch.get_upper_bound(3) == Approx(update_sketch.get_upper_bound(3)).margin(1e-10));
   compact_theta_sketch compact_sketch = update_sketch.compact();
   // the sketches are ordered, so the iteration sequence must match exactly
   auto iter = sketch.begin();
-  for (const auto& key: compact_sketch) {
+  for (const auto key: compact_sketch) {
+    REQUIRE(*iter == key);
+    ++iter;
+  }
+}
+
+TEST_CASE("theta sketch: serialize deserialize compressed", "[theta_sketch]") {
+  auto update_sketch = update_theta_sketch::builder().build();
+  for (int i = 0; i < 10000; i++) update_sketch.update(i);
+  auto compact_sketch = update_sketch.compact();
+
+  auto bytes = compact_sketch.serialize_compressed();
+  { // deserialize bytes
+    auto deserialized_sketch = compact_theta_sketch::deserialize(bytes.data(), bytes.size());
+    REQUIRE(deserialized_sketch.get_num_retained() == compact_sketch.get_num_retained());
+    REQUIRE(deserialized_sketch.get_theta() == compact_sketch.get_theta());
+    auto iter = deserialized_sketch.begin();
+    for (const auto key: compact_sketch) {
+      REQUIRE(*iter == key);
+      ++iter;
+    }
+  }
+  { // wrap bytes
+    auto wrapped_sketch = wrapped_compact_theta_sketch::wrap(bytes.data(), bytes.size());
+    REQUIRE(wrapped_sketch.get_num_retained() == compact_sketch.get_num_retained());
+    REQUIRE(wrapped_sketch.get_theta() == compact_sketch.get_theta());
+    auto iter = wrapped_sketch.begin();
+    for (const auto key: compact_sketch) {
+      REQUIRE(*iter == key);
+      ++iter;
+    }
+  }
+
+  std::stringstream s(std::ios::in | std::ios::out | std::ios::binary);
+  compact_sketch.serialize_compressed(s);
+  auto deserialized_sketch = compact_theta_sketch::deserialize(s);
+  REQUIRE(deserialized_sketch.get_num_retained() == compact_sketch.get_num_retained());
+  REQUIRE(deserialized_sketch.get_theta() == compact_sketch.get_theta());
+  auto iter = deserialized_sketch.begin();
+  for (const auto key: compact_sketch) {
     REQUIRE(*iter == key);
     ++iter;
   }
 }
 
 } /* namespace datasketches */
```

### Comparing `datasketches-4.0.1/theta/test/theta_union_test.cpp` & `datasketches-4.1.0/theta/test/theta_union_test.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -124,8 +124,33 @@
 TEST_CASE("theta union: seed mismatch", "[theta_union]") {
   update_theta_sketch sketch = update_theta_sketch::builder().build();
   sketch.update(1); // non-empty should not be ignored
   theta_union u = theta_union::builder().set_seed(123).build();
   REQUIRE_THROWS_AS(u.update(sketch), std::invalid_argument);
 }
 
+TEST_CASE("theta union: larger K", "[theta_union]") {
+  auto update_sketch1 = datasketches::update_theta_sketch::builder().set_lg_k(14).build();
+  for(int i = 0; i < 16384; ++i) update_sketch1.update(i);
+
+  auto update_sketch2 = datasketches::update_theta_sketch::builder().set_lg_k(14).build();
+  for(int i = 0; i < 26384; ++i) update_sketch2.update(i);
+
+  auto update_sketch3 = datasketches::update_theta_sketch::builder().set_lg_k(14).build();
+  for(int i = 0; i < 86384; ++i) update_sketch3.update(i);
+
+  auto union1 = datasketches::theta_union::builder().set_lg_k(16).build();
+  union1.update(update_sketch2);
+  union1.update(update_sketch1);
+  union1.update(update_sketch3);
+  auto result1 = union1.get_result();
+  REQUIRE(result1.get_estimate() == update_sketch3.get_estimate());
+
+  auto union2 = datasketches::theta_union::builder().set_lg_k(16).build();
+  union2.update(update_sketch1);
+  union2.update(update_sketch3);
+  union2.update(update_sketch2);
+  auto result2 = union2.get_result();
+  REQUIRE(result2.get_estimate() == update_sketch3.get_estimate());
+}
+
 } /* namespace datasketches */
```

### Comparing `datasketches-4.0.1/tuple/CMakeLists.txt` & `datasketches-4.1.0/tuple/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_a_not_b.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_a_not_b.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_a_not_b_impl.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_a_not_b_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_intersection.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_intersection.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_intersection_impl.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_intersection_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_sketch.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_sketch.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_sketch_impl.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_sketch_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_union.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_union.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/array_of_doubles_union_impl.hpp` & `datasketches-4.1.0/tuple/include/array_of_doubles_union_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_a_not_b.hpp` & `datasketches-4.1.0/tuple/include/tuple_a_not_b.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_a_not_b_impl.hpp` & `datasketches-4.1.0/tuple/include/tuple_a_not_b_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_intersection.hpp` & `datasketches-4.1.0/tuple/include/tuple_intersection.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_intersection_impl.hpp` & `datasketches-4.1.0/tuple/include/tuple_intersection_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_jaccard_similarity.hpp` & `datasketches-4.1.0/tuple/include/tuple_jaccard_similarity.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_sketch.hpp` & `datasketches-4.1.0/tuple/include/tuple_sketch.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_sketch_impl.hpp` & `datasketches-4.1.0/tuple/include/tuple_sketch_impl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 template<typename S, typename A>
 bool tuple_sketch<S, A>::is_estimation_mode() const {
   return get_theta64() < theta_constants::MAX_THETA && !is_empty();
 }
 
 template<typename S, typename A>
 double tuple_sketch<S, A>::get_theta() const {
-  return static_cast<double>(get_theta64()) / theta_constants::MAX_THETA;
+  return static_cast<double>(get_theta64()) /
+         static_cast<double>(theta_constants::MAX_THETA);
 }
 
 template<typename S, typename A>
 double tuple_sketch<S, A>::get_estimate() const {
   return get_num_retained() / get_theta();
 }
```

### Comparing `datasketches-4.0.1/tuple/include/tuple_union.hpp` & `datasketches-4.1.0/tuple/include/tuple_union.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/include/tuple_union_impl.hpp` & `datasketches-4.1.0/tuple/include/tuple_union_impl.hpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/CMakeLists.txt` & `datasketches-4.1.0/tuple/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/aod_1_compact_estimation_from_java.sk` & `datasketches-4.1.0/tuple/test/aod_1_compact_estimation_from_java.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/aod_2_compact_exact_from_java.sk` & `datasketches-4.1.0/tuple/test/aod_2_compact_exact_from_java.sk`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/array_of_doubles_sketch_test.cpp` & `datasketches-4.1.0/tuple/test/array_of_doubles_sketch_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/engagement_test.cpp` & `datasketches-4.1.0/tuple/test/engagement_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/tuple_a_not_b_test.cpp` & `datasketches-4.1.0/tuple/test/tuple_a_not_b_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/tuple_intersection_test.cpp` & `datasketches-4.1.0/tuple/test/tuple_intersection_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/tuple_jaccard_similarity_test.cpp` & `datasketches-4.1.0/tuple/test/tuple_jaccard_similarity_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/tuple_sketch_allocation_test.cpp` & `datasketches-4.1.0/tuple/test/tuple_sketch_allocation_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/tuple_sketch_test.cpp` & `datasketches-4.1.0/tuple/test/tuple_sketch_test.cpp`

 * *Files identical despite different names*

### Comparing `datasketches-4.0.1/tuple/test/tuple_union_test.cpp` & `datasketches-4.1.0/tuple/test/tuple_union_test.cpp`

 * *Files identical despite different names*

