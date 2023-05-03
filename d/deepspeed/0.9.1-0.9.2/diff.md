# Comparing `tmp/deepspeed-0.9.1.tar.gz` & `tmp/deepspeed-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepspeed-0.9.1.tar", last modified: Fri Apr 21 00:48:05 2023, max compression
+gzip compressed data, was "deepspeed-0.9.2.tar", last modified: Wed May  3 17:31:51 2023, max compression
```

## Comparing `deepspeed-0.9.1.tar` & `deepspeed-0.9.2.tar`

### file list

```diff
@@ -1,602 +1,604 @@
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.873510 deepspeed-0.9.1/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.1/LICENSE
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.1/MANIFEST.in
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27276 2023-04-21 00:48:05.873510 deepspeed-0.9.1/PKG-INFO
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26393 2023-04-21 00:47:36.000000 deepspeed-0.9.1/README.md
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.1/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.1/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.1/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/bin/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/deepspeed
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/deepspeed.pt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/ds
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.1/bin/ds_bench
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.1/bin/ds_elastic
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/ds_report
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/ds_ssh
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/dsr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:04.000000 deepspeed-0.9.1/build.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.433510 deepspeed-0.9.1/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.423510 deepspeed-0.9.1/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.483510 deepspeed-0.9.1/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.483510 deepspeed-0.9.1/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.503510 deepspeed-0.9.1/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12223 2023-04-21 00:47:36.000000 deepspeed-0.9.1/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.1/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      264 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.503510 deepspeed-0.9.1/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.513510 deepspeed-0.9.1/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.513510 deepspeed-0.9.1/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.523510 deepspeed-0.9.1/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.433510 deepspeed-0.9.1/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.523510 deepspeed-0.9.1/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.523510 deepspeed-0.9.1/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      833 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.533510 deepspeed-0.9.1/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.433510 deepspeed-0.9.1/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.543510 deepspeed-0.9.1/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16338 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6908 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29045 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22685 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    77643 2023-04-21 00:47:36.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23789 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29531 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.543510 deepspeed-0.9.1/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17739 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8265 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.543510 deepspeed-0.9.1/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed/autotuning/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54204 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/autotuning/autotuner.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.573510 deepspeed-0.9.1/deepspeed/autotuning/config_templates/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero0.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero1.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero2.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero3.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5945 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.573510 deepspeed-0.9.1/deepspeed/autotuning/tuner/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/base_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/cost_model.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/index_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/model_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15054 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.583510 deepspeed-0.9.1/deepspeed/checkpoint/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/checkpoint/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12009 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/deepspeed_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/reshape_3d_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/reshape_meg_2d.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/reshape_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/universal_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      936 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/zero_checkpoint.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.583510 deepspeed-0.9.1/deepspeed/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/backend.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26108 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1256 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10257 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/comm/torch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/comm/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.593510 deepspeed-0.9.1/deepspeed/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36034 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10519 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/compress.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23240 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4959 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12303 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8039 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7814 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.603510 deepspeed-0.9.1/deepspeed/elasticity/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2452 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/elastic_agent.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/elasticity.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4793 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/env_report.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/git_version_info.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed/git_version_info_installed.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.603510 deepspeed-0.9.1/deepspeed/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9506 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/inference/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    28924 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/inference/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/launcher/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/launcher/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      352 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/launcher/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    19078 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/launcher/launch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11952 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/launcher/multinode_runner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23296 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/launcher/runner.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/model_implementations/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/vae.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/model_implementations/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/features/cuda_graph.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.623510 deepspeed-0.9.1/deepspeed/model_implementations/transformers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/clip_encoder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7828 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.633510 deepspeed-0.9.1/deepspeed/module_inject/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4815 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/auto_tp.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.653510 deepspeed-0.9.1/deepspeed/module_inject/containers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      838 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23292 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/base_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3718 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4762 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2807 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/clip.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3137 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/distil_bert.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.653510 deepspeed-0.9.1/deepspeed/module_inject/containers/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      181 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1206 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/features/megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2486 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/features/meta_tensor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2249 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gpt2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3833 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gptj.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4107 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gptneo.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5005 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gptneox.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5045 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3913 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6283 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/vae.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/inject.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3825 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/layers.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14122 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/load_checkpoint.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/module_quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7723 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35947 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/replace_module.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      930 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/replace_policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1653 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.663510 deepspeed-0.9.1/deepspeed/moe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/experts.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/mappings.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/sharded_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/monitor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2529 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/csv_monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/tensorboard.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/wandb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/nebula/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/nebula/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/nebula/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/nebula/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/ops/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/ops/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adagrad/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adagrad/cpu_adagrad.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/adam/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8546 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6878 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/multi_tensor_apply.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/aio/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/aio/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_test/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_test/single_process_config.json
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12223 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      264 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      833 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.713510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.713510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16338 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6908 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29045 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22685 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    77643 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23789 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29531 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.713510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17739 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8265 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.723510 deepspeed-0.9.1/deepspeed/ops/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.723510 deepspeed-0.9.1/deepspeed/ops/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/lamb/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/lamb/fused_lamb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.733510 deepspeed-0.9.1/deepspeed/ops/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.733510 deepspeed-0.9.1/deepspeed/ops/quantizer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/quantizer/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/quantizer/quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.743510 deepspeed-0.9.1/deepspeed/ops/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/random_ltd/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4901 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/random_ltd/dropping_utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.743510 deepspeed-0.9.1/deepspeed/ops/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/matmul.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_attention_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_self_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42462 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparsity_config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.753510 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/matmul.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.753510 deepspeed-0.9.1/deepspeed/ops/transformer/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.763510 deepspeed-0.9.1/deepspeed/ops/transformer/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/bias_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5612 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9986 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4763 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13928 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4585 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18473 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/moe_inference.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      551 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1227 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1007 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1273 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1424 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1215 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/residual_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1059 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1513 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      875 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/triton_ops.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/pipe/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/profiling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1708 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1098 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/profiling/flops_profiler/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/flops_profiler/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47039 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/flops_profiler/profiler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.793510 deepspeed-0.9.1/deepspeed/runtime/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.793510 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/checkpointing.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/bf16_optimizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      654 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4982 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/coalesced_collectives.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/mpi.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/nccl.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/compression/cupy.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39382 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/config_utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12806 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.813510 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.813510 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25015 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/dataloader.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/eigenvalue.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   149903 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.813510 deepspeed-0.9.1/deepspeed/runtime/fp16/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/fused_optimizer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11093 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/loss_scaler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.823510 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/zoadam.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/unfused_optimizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19007 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/hybrid_engine.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/lr_schedules.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.823510 deepspeed-0.9.1/deepspeed/runtime/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56559 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/module.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/p2p.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/schedule.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/topology.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/progressive_layer_drop.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/sparse_tensor.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/state_dict_factory.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.833510 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/aio_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/async_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/optimizer_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35806 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/weight_quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.843510 deepspeed-0.9.1/deepspeed/runtime/zero/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      423 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9996 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/contiguous_memory_allocator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7784 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/offload_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21889 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/parameter_offload.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    71248 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/zero/partition_parameters.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22345 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/partitioned_param_coordinator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   112178 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/stage3.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110183 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/stage_1_and_2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/test.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/tiling.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.863510 deepspeed-0.9.1/deepspeed/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      717 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/comms_logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/debug.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/exceptions.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/groups.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/init_on_device.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/mixed_precision_linkage.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/nvtx.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/tensor_fragment.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8765 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/timer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      200 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/types.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24043 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/utils/zero_to_fp32.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed.egg-info/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27276 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/PKG-INFO
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20079 2023-04-21 00:48:05.000000 deepspeed-0.9.1/deepspeed.egg-info/SOURCES.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/dependency_links.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/entry_points.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1124 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/requires.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/top_level.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.873510 deepspeed-0.9.1/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.1/op_builder/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.1/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.873510 deepspeed-0.9.1/requirements/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-1bit-mpi.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-autotuning-ml.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-autotuning.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      232 2022-11-14 17:49:34.000000 deepspeed-0.9.1/requirements/requirements-dev.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.1/requirements/requirements-inf.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.1/requirements/requirements-readthedocs.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.1/requirements/requirements-sd.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-sparse_attn.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.1/requirements/requirements.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-04-21 00:48:05.873510 deepspeed-0.9.1/setup.cfg
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11318 2023-04-21 00:47:36.000000 deepspeed-0.9.1/setup.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-04-13 15:30:43.000000 deepspeed-0.9.1/version.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.312835 deepspeed-0.9.2/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.2/LICENSE
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.2/MANIFEST.in
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27421 2023-05-03 17:31:51.312835 deepspeed-0.9.2/PKG-INFO
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26538 2023-05-03 17:31:31.000000 deepspeed-0.9.2/README.md
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.822835 deepspeed-0.9.2/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.2/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.2/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.2/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.2/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.832835 deepspeed-0.9.2/bin/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/deepspeed
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/deepspeed.pt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/ds
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.2/bin/ds_bench
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.2/bin/ds_elastic
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/ds_report
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/ds_ssh
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.2/bin/dsr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:49.000000 deepspeed-0.9.2/build.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.782835 deepspeed-0.9.2/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.832835 deepspeed-0.9.2/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.832835 deepspeed-0.9.2/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.772835 deepspeed-0.9.2/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.842835 deepspeed-0.9.2/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.862835 deepspeed-0.9.2/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.862835 deepspeed-0.9.2/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.892835 deepspeed-0.9.2/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.2/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.892835 deepspeed-0.9.2/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.902835 deepspeed-0.9.2/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.902835 deepspeed-0.9.2/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.902835 deepspeed-0.9.2/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.782835 deepspeed-0.9.2/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.912835 deepspeed-0.9.2/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.912835 deepspeed-0.9.2/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.922835 deepspeed-0.9.2/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.782835 deepspeed-0.9.2/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.922835 deepspeed-0.9.2/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18600 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8918 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35842 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    24466 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    78079 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2517 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28591 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    34052 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.2/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18300 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8317 2023-05-03 17:31:31.000000 deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.2/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/deepspeed/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/deepspeed/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.942835 deepspeed-0.9.2/deepspeed/autotuning/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54204 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/autotuning/autotuner.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.952835 deepspeed-0.9.2/deepspeed/autotuning/config_templates/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero0.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero1.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero2.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.2/deepspeed/autotuning/config_templates/template_zero3.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5945 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.952835 deepspeed-0.9.2/deepspeed/autotuning/tuner/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/base_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/cost_model.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/index_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/model_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/tuner/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15054 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/autotuning/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.962835 deepspeed-0.9.2/deepspeed/checkpoint/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/checkpoint/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12009 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/deepspeed_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/reshape_3d_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/reshape_meg_2d.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/reshape_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/universal_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      936 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/checkpoint/zero_checkpoint.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.972835 deepspeed-0.9.2/deepspeed/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/comm/backend.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27476 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/comm/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/comm/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1256 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/comm/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13128 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/comm/torch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/comm/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.982835 deepspeed-0.9.2/deepspeed/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36034 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10519 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/compress.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23240 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4959 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12303 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8039 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7814 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/compression/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.992835 deepspeed-0.9.2/deepspeed/elasticity/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2452 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/elastic_agent.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/elasticity.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/elasticity/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4793 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/env_report.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/git_version_info.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-05-03 17:31:49.000000 deepspeed-0.9.2/deepspeed/git_version_info_installed.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9506 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/inference/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    28924 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/inference/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/launcher/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/launcher/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      352 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/launcher/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    19078 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/launcher/launch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12206 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/launcher/multinode_runner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23389 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/launcher/runner.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/model_implementations/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.002835 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/diffusers/vae.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.012835 deepspeed-0.9.2/deepspeed/model_implementations/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/features/cuda_graph.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.022835 deepspeed-0.9.2/deepspeed/model_implementations/transformers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/clip_encoder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7828 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.032835 deepspeed-0.9.2/deepspeed/module_inject/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4815 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/auto_tp.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.042835 deepspeed-0.9.2/deepspeed/module_inject/containers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      838 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23997 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/base_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3718 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5150 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2807 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/clip.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3137 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/distil_bert.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.052835 deepspeed-0.9.2/deepspeed/module_inject/containers/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      181 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3791 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/features/megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2486 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/features/meta_tensor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2249 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gpt2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4476 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gptj.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4819 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gptneo.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5495 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/gptneox.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5045 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3913 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6280 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/containers/vae.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/inject.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3825 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/layers.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14122 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/load_checkpoint.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/module_quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7723 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/module_inject/policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35871 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/module_inject/replace_module.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      930 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/replace_policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1653 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/module_inject/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.052835 deepspeed-0.9.2/deepspeed/moe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/experts.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/mappings.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/sharded_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/moe/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/monitor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2529 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/csv_monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/tensorboard.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/monitor/wandb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/nebula/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/nebula/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/nebula/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/nebula/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/ops/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.062835 deepspeed-0.9.2/deepspeed/ops/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adagrad/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adagrad/cpu_adagrad.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/adam/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8546 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6878 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/adam/multi_tensor_apply.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/aio/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/aio/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.802835 deepspeed-0.9.2/deepspeed/ops/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.792835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.072835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.082835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.082835 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_test/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_test/single_process_config.json
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.082835 deepspeed-0.9.2/deepspeed/ops/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.092835 deepspeed-0.9.2/deepspeed/ops/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.802835 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.102835 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.802835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18600 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8918 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35842 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    24466 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    78079 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2517 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28591 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    34052 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18300 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8317 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.112835 deepspeed-0.9.2/deepspeed/ops/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/lamb/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/lamb/fused_lamb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.132835 deepspeed-0.9.2/deepspeed/ops/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.142835 deepspeed-0.9.2/deepspeed/ops/quantizer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/quantizer/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/quantizer/quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.142835 deepspeed-0.9.2/deepspeed/ops/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/random_ltd/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4901 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/random_ltd/dropping_utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.152835 deepspeed-0.9.2/deepspeed/ops/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/matmul.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_attention_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_self_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42462 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparsity_config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.152835 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/matmul.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.152835 deepspeed-0.9.2/deepspeed/ops/transformer/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.172835 deepspeed-0.9.2/deepspeed/ops/transformer/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/bias_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5612 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9986 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4763 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13927 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4585 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18473 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/moe_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.182835 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      551 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1227 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1007 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/linear.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1273 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1424 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1215 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/residual_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1059 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1513 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      875 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/inference/triton_ops.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/ops/transformer/transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.182835 deepspeed-0.9.2/deepspeed/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/pipe/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.182835 deepspeed-0.9.2/deepspeed/profiling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1708 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1098 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.192835 deepspeed-0.9.2/deepspeed/profiling/flops_profiler/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/flops_profiler/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47039 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/profiling/flops_profiler/profiler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.212835 deepspeed-0.9.2/deepspeed/runtime/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.222835 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/checkpointing.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.2/deepspeed/runtime/bf16_optimizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.222835 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      654 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4982 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.222835 deepspeed-0.9.2/deepspeed/runtime/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/coalesced_collectives.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/mpi.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/comm/nccl.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.232835 deepspeed-0.9.2/deepspeed/runtime/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/compression/cupy.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39541 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/config_utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12806 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.232835 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.232835 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.242835 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25015 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/dataloader.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/eigenvalue.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   154538 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.252835 deepspeed-0.9.2/deepspeed/runtime/fp16/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/fused_optimizer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11093 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/loss_scaler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.252835 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/zoadam.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/fp16/unfused_optimizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20256 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/hybrid_engine.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/lr_schedules.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.262835 deepspeed-0.9.2/deepspeed/runtime/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56847 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/module.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/p2p.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/schedule.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/pipe/topology.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/progressive_layer_drop.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/sparse_tensor.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/state_dict_factory.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.272835 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/aio_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/async_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/optimizer_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/swap_tensor/utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35806 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/weight_quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.282835 deepspeed-0.9.2/deepspeed/runtime/zero/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/contiguous_memory_allocator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/linear.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21571 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/mics.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/mics_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/offload_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21889 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/zero/parameter_offload.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    72389 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/partition_parameters.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22345 2023-04-13 15:29:56.000000 deepspeed-0.9.2/deepspeed/runtime/zero/partitioned_param_coordinator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   113908 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/stage3.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110844 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/stage_1_and_2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/test.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/runtime/zero/tiling.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/runtime/zero/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.302835 deepspeed-0.9.2/deepspeed/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      717 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/comms_logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/debug.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/exceptions.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/groups.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/init_on_device.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/mixed_precision_linkage.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/nvtx.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/tensor_fragment.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8765 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/timer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      200 2023-04-11 17:18:49.000000 deepspeed-0.9.2/deepspeed/utils/types.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.2/deepspeed/utils/zero_to_fp32.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:50.932835 deepspeed-0.9.2/deepspeed.egg-info/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27421 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/PKG-INFO
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20147 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/entry_points.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1086 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/requires.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-05-03 17:31:50.000000 deepspeed-0.9.2/deepspeed.egg-info/top_level.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.302835 deepspeed-0.9.2/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.2/op_builder/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.2/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.2/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-05-03 17:31:51.312835 deepspeed-0.9.2/requirements/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-1bit-mpi.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-autotuning-ml.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-autotuning.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.2/requirements/requirements-dev.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.2/requirements/requirements-inf.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.2/requirements/requirements-readthedocs.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.2/requirements/requirements-sd.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.2/requirements/requirements-sparse_attn.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.2/requirements/requirements.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-05-03 17:31:51.312835 deepspeed-0.9.2/setup.cfg
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11318 2023-04-21 00:47:36.000000 deepspeed-0.9.2/setup.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-04-21 00:48:17.000000 deepspeed-0.9.2/version.txt
```

### Comparing `deepspeed-0.9.1/LICENSE` & `deepspeed-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/PKG-INFO` & `deepspeed-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.1
+Version: 0.9.2
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: MIT
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -27,14 +27,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
 [![Downloads](https://pepy.tech/badge/deepspeed)](https://pepy.tech/project/deepspeed)
 [![Build](https://badgen.net/badge/build/check-status/blue)](#build-pipeline-status)
+[![Twitter](https://img.shields.io/twitter/follow/MSFTDeepSpeed)](https://twitter.com/intent/follow?screen_name=MSFTDeepSpeed)
 
 
 <div align="center">
  <img src="docs/assets/images/DeepSpeed_light.svg#gh-light-mode-only" width="400px">
  <img src="docs/assets/images/DeepSpeed_dark_transparent.svg#gh-dark-mode-only" width="400px">
 </div>
 
@@ -122,15 +123,15 @@
 DeepSpeed has been integrated with several different popular open-source DL frameworks such as:
 
 |                                                                                                | Documentation                                |
 | ---------------------------------------------------------------------------------------------- | -------------------------------------------- |
 <img src="docs/assets/images/transformers-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/transformers-dark.png#gh-dark-mode-only" width="250px"> | [Transformers with DeepSpeed](https://huggingface.co/docs/transformers/main/main_classes/deepspeed) |
 | <img src="docs/assets/images/accelerate-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/accelerate-dark.png#gh-dark-mode-only" width="250px"> | [Accelerate with DeepSpeed](https://huggingface.co/docs/accelerate/usage_guides/deepspeed) |
 | <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://lightning.ai/docs/pytorch/stable/advanced/model_parallel.html#deepspeed) |
-| <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
+| <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/projects/composer/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
 | <img src="docs/assets/images/determined.svg" width="225px"> | [Determined with DeepSpeed](https://docs.determined.ai/latest/training/apis-howto/deepspeed/overview.html) |
 
 ---
 
 # Build Pipeline Status
 
 | Description | Status |
```

### Comparing `deepspeed-0.9.1/README.md` & `deepspeed-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
 [![Downloads](https://pepy.tech/badge/deepspeed)](https://pepy.tech/project/deepspeed)
 [![Build](https://badgen.net/badge/build/check-status/blue)](#build-pipeline-status)
+[![Twitter](https://img.shields.io/twitter/follow/MSFTDeepSpeed)](https://twitter.com/intent/follow?screen_name=MSFTDeepSpeed)
 
 
 <div align="center">
  <img src="docs/assets/images/DeepSpeed_light.svg#gh-light-mode-only" width="400px">
  <img src="docs/assets/images/DeepSpeed_dark_transparent.svg#gh-dark-mode-only" width="400px">
 </div>
 
@@ -93,15 +94,15 @@
 DeepSpeed has been integrated with several different popular open-source DL frameworks such as:
 
 |                                                                                                | Documentation                                |
 | ---------------------------------------------------------------------------------------------- | -------------------------------------------- |
 <img src="docs/assets/images/transformers-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/transformers-dark.png#gh-dark-mode-only" width="250px"> | [Transformers with DeepSpeed](https://huggingface.co/docs/transformers/main/main_classes/deepspeed) |
 | <img src="docs/assets/images/accelerate-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/accelerate-dark.png#gh-dark-mode-only" width="250px"> | [Accelerate with DeepSpeed](https://huggingface.co/docs/accelerate/usage_guides/deepspeed) |
 | <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://lightning.ai/docs/pytorch/stable/advanced/model_parallel.html#deepspeed) |
-| <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
+| <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/projects/composer/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
 | <img src="docs/assets/images/determined.svg" width="225px"> | [Determined with DeepSpeed](https://docs.determined.ai/latest/training/apis-howto/deepspeed/overview.html) |
 
 ---
 
 # Build Pipeline Status
 
 | Description | Status |
```

### Comparing `deepspeed-0.9.1/accelerator/abstract_accelerator.py` & `deepspeed-0.9.2/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/accelerator/cuda_accelerator.py` & `deepspeed-0.9.2/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/accelerator/real_accelerator.py` & `deepspeed-0.9.2/accelerator/real_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/bin/ds_bench` & `deepspeed-0.9.2/bin/ds_bench`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/bin/ds_elastic` & `deepspeed-0.9.2/bin/ds_elastic`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/bin/ds_ssh` & `deepspeed-0.9.2/bin/ds_ssh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.2/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.2/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.2/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.2/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.2/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.2/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.2/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.2/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.2/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/StopWatch.h` & `deepspeed-0.9.2/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/Timer.h` & `deepspeed-0.9.2/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/context.h` & `deepspeed-0.9.2/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/conversion_utils.h` & `deepspeed-0.9.2/csrc/includes/conversion_utils.h`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,19 @@
 
 /*********************  To Half2 Conversions *********************/
 template <>
 DS_D_INLINE __half2 to(float2 val)
 {
     return __float22half2_rn(val);
 }
+template <>
+DS_D_INLINE __half2 to(float val)
+{
+    return __float2half2_rn(val);
+}
 
 #ifdef BF16_AVAILABLE
 // No direct conversion
 template <>
 DS_D_INLINE __half2 to(__nv_bfloat162 val)
 {
     return to<__half2>(to<float2>(val));
@@ -402,14 +407,19 @@
 #ifdef BF16_AVAILABLE
 template <>
 DS_D_INLINE __nv_bfloat162 to(float2 val)
 {
     return __float22bfloat162_rn(val);
 }
 template <>
+DS_D_INLINE __nv_bfloat162 to(float val)
+{
+    return __float2bfloat162_rn(val);
+}
+template <>
 DS_D_INLINE __nv_bfloat162 to(__half2 val)
 {
     return to<__nv_bfloat162>(to<float2>(val));
 }
 #endif
 
 /*********************  To INT64_T Conversions *********************/
```

### Comparing `deepspeed-0.9.1/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.2/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/cpu_adam.h` & `deepspeed-0.9.2/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.2/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.2/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.2/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/dropout.h` & `deepspeed-0.9.2/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.2/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.2/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/feed_forward.h` & `deepspeed-0.9.2/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/gelu.h` & `deepspeed-0.9.2/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/gemm_test.h` & `deepspeed-0.9.2/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/general_kernels.h` & `deepspeed-0.9.2/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.2/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/normalize_layer.h` & `deepspeed-0.9.2/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/quantization.h` & `deepspeed-0.9.2/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/quantization_utils.h` & `deepspeed-0.9.2/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/reduction_utils.h` & `deepspeed-0.9.2/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/simd.h` & `deepspeed-0.9.2/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/softmax.h` & `deepspeed-0.9.2/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.2/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/includes/type_shim.h` & `deepspeed-0.9.2/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.2/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/quantization/dequantize.cu` & `deepspeed-0.9.2/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.2/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.2/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/quantization/quantize.cu` & `deepspeed-0.9.2/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.2/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.2/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.2/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.2/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.2/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.2/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.2/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.2/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 
 #pragma once
 
 #if __CUDA_ARCH__ >= 530
 #define HALF_PRECISION_AVAILABLE = 1
 #endif
 
+#ifdef __HIP_PLATFORM_HCC__
+#include <hip/hip_cooperative_groups.h>
+#else
 #include <cooperative_groups.h>
+#endif
+
 #include <cuda.h>
 #include <cuda_fp16.h>
 
 /*********** Group Norm Kernels, Structs, and Helpers ************/
 
 struct {
     int64_t batch_size;
```

### Comparing `deepspeed-0.9.1/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.2/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.2/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.2/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.2/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.2/csrc/transformer/general_kernels.cu`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                               int seq_length,
                               int hidden_dim,
                               cudaStream_t& stream)
 {
     int total_count = batch_size * seq_length * hidden_dim / 4;
     dim3 grid_dim = DS_GET_BLOCKS(total_count);  //(batch_size * seq_length);
 
-    dim3 block_dim = DS_CUDA_NUM_THREADS;        //(hidden_dim / 4);
+    dim3 block_dim = DS_CUDA_NUM_THREADS;  //(hidden_dim / 4);
 
     fused_add2_kernel<<<grid_dim, block_dim, 0, stream>>>(total_count, out, inp1, inp2);
 }
 
 template <>
 void launch_fused_add2<__half>(__half* out,
                                const __half* inp1,
@@ -175,15 +175,15 @@
                                int seq_length,
                                int hidden_dim,
                                cudaStream_t& stream)
 {
     int total_count = batch_size * seq_length * hidden_dim / 4;
     dim3 grid_dim = DS_GET_BLOCKS(total_count);  //(batch_size * seq_length);
 
-    dim3 block_dim = DS_CUDA_NUM_THREADS;        //(hidden_dim / 4);
+    dim3 block_dim = DS_CUDA_NUM_THREADS;  //(hidden_dim / 4);
 
     fused_add2_kernel<<<grid_dim, block_dim, 0, stream>>>(total_count, out, inp1, inp2);
 }
 
 __global__ void fused_add3_kernel(float* out,
                                   const float* inp1,
                                   const float* inp2,
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 // Copyright (c) Microsoft Corporation.
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
+#include "conversion_utils.h"
 #include "inference_cuda_layers.h"
 
 #ifndef __HIP_PLATFORM_HCC__
 #include <cuda_profiler_api.h>
 #endif
 
 namespace cg = cooperative_groups;
 namespace cg = cooperative_groups;
 
-__global__ void apply_rotary_pos_emb(float* mixed_query,
-                                     float* key_layer,
+template <typename T>
+__global__ void apply_rotary_pos_emb(T* mixed_query,
+                                     T* key_layer,
                                      unsigned rotary_dim,
                                      unsigned seq_len,
                                      unsigned seq_offset,
                                      unsigned num_heads,
                                      unsigned head_size,
                                      unsigned total_count,
                                      int max_out_tokens)
@@ -36,77 +38,32 @@
     unsigned seq_index = head_id % seq_len;
     unsigned k_offset = (seq_index + (head_id / seq_len) * max_out_tokens) * head_size;
 
     if (head_id < total_count) {
         while (lane < rotary_dim) {
             float inv_freq = (float)((lane / 2) * 2) / (float)rotary_dim;
             inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
-            float q = mixed_query[offset + lane];
-            float k = key_layer[k_offset + lane];
+            float q = conversion::to<float>(mixed_query[offset + lane]);
+            float k = conversion::to<float>(key_layer[k_offset + lane]);
             float rotary_sign = (lane % 2 == 1 ? -1.0 : 1.0);
             float q_rot = (q * rotary_sign);
             float k_rot = (k * rotary_sign);
             q_rot = g.shfl_xor(q_rot, 1);
             k_rot = g.shfl_xor(k_rot, 1);
             q = q * cosf(inv_freq) + q_rot * sinf(inv_freq);
             k = k * cosf(inv_freq) + k_rot * sinf(inv_freq);
 
-            mixed_query[offset + lane] = q;
-            key_layer[k_offset + lane] = k;
+            mixed_query[offset + lane] = conversion::to<T>(q);
+            key_layer[k_offset + lane] = conversion::to<T>(k);
 
             lane += WARP_SIZE;
         }
     }
 }
 
-__global__ void apply_rotary_pos_emb(__half* mixed_query,
-                                     __half* key_layer,
-                                     unsigned rotary_dim,
-                                     unsigned seq_len,
-                                     unsigned seq_offset,
-                                     unsigned num_heads,
-                                     unsigned head_size,
-                                     unsigned total_count,
-                                     int max_out_tokens)
-{
-    cg::thread_block b = cg::this_thread_block();
-    cg::thread_block_tile<WARP_SIZE> g = cg::tiled_partition<WARP_SIZE>(b);
-
-    int id = threadIdx.x;
-    int gid = id >> 5;
-    int lane = id & 0x1f;
-
-    unsigned head_id = blockIdx.x * MAX_WARP_NUM + gid;
-    unsigned offset = head_id * head_size;
-
-    unsigned seq_id = (head_id / num_heads) % seq_len + seq_offset;
-    unsigned seq_index = head_id % seq_len;
-    unsigned k_offset = (seq_index + (head_id / seq_len) * max_out_tokens) * head_size;
-
-    if (head_id < total_count) {
-        while (lane < rotary_dim) {
-            float inv_freq = (float)((lane / 2) * 2) / (float)rotary_dim;
-            inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
-            float q = (float)mixed_query[offset + lane];
-            float k = (float)key_layer[k_offset + lane];
-            float rotary_sign = (lane % 2 == 1 ? -1.0 : 1.0);
-            float q_rot = (q * rotary_sign);
-            float k_rot = (k * rotary_sign);
-            q_rot = g.shfl_xor(q_rot, 1);
-            k_rot = g.shfl_xor(k_rot, 1);
-            q = q * cosf(inv_freq) + q_rot * sinf(inv_freq);
-            k = k * cosf(inv_freq) + k_rot * sinf(inv_freq);
-
-            mixed_query[offset + lane] = (__half)q;
-            key_layer[k_offset + lane] = (__half)k;
-
-            lane += WARP_SIZE;
-        }
-    }
-}
 __global__ void apply_rotary_pos_emb1(float* mixed_query,
                                       float* key_layer,
                                       unsigned rotary_dim,
                                       unsigned seq_len,
                                       unsigned seq_offset,
                                       unsigned num_heads,
                                       unsigned head_size,
@@ -144,16 +101,18 @@
             mixed_query[offset + lane] = q;
             key_layer[k_offset + lane] = k;
 
             lane += WARP_SIZE;
         }
     }
 }
-__global__ void apply_rotary_pos_emb1(__half* mixed_query,
-                                      __half* key_layer,
+
+template <typename T>
+__global__ void apply_rotary_pos_emb1(T* mixed_query,
+                                      T* key_layer,
                                       unsigned rotary_dim,
                                       unsigned seq_len,
                                       unsigned seq_offset,
                                       unsigned num_heads,
                                       unsigned head_size,
                                       unsigned total_count,
                                       int max_out_tokens)
@@ -181,28 +140,28 @@
 
     unsigned seq_id = (head_id % seq_len) + seq_offset;
     unsigned half_dim = rotary_dim >> 1;
     if (head_id < total_count) {
         while (lane < rotary_dim) {
             float inv_freq = (float)((lane % half_dim) * 2) / (float)rotary_dim;
             inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
-            float q = (float)mixed_query[offset + lane];
-            float k = (float)key_layer[k_offset + lane];
+            float q = conversion::to<float>(mixed_query[offset + lane]);
+            float k = conversion::to<float>(key_layer[k_offset + lane]);
             float rotary_sign = (lane > (half_dim - 1) ? -1.0 : 1.0);
             float q_rot = (q * rotary_sign);
             float k_rot = (k * rotary_sign);
             auto q_rot_tmp = lane < half_dim ? __shfl_sync(mask[lane], q_rot, lane + half_dim)
                                              : __shfl_sync(mask[lane], q_rot, lane - half_dim);
             auto k_rot_tmp = lane < half_dim ? __shfl_sync(mask[lane], k_rot, lane + half_dim)
                                              : __shfl_sync(mask[lane], k_rot, lane - half_dim);
             q = q * cosf(inv_freq) + q_rot_tmp * sinf(inv_freq);
             k = k * cosf(inv_freq) + k_rot_tmp * sinf(inv_freq);
 
-            mixed_query[offset + lane] = (__half)q;
-            key_layer[k_offset + lane] = (__half)k;
+            mixed_query[offset + lane] = conversion::to<T>(q);
+            key_layer[k_offset + lane] = conversion::to<T>(k);
 
             lane += WARP_SIZE;
         }
     }
 }
 
 template <typename T>
@@ -252,27 +211,94 @@
                                                  unsigned,
                                                  unsigned,
                                                  unsigned,
                                                  bool,
                                                  bool,
                                                  cudaStream_t,
                                                  int);
+#ifdef BF16_AVAILABLE
+template void launch_apply_rotary_pos_emb<__nv_bfloat16>(__nv_bfloat16*,
+                                                         __nv_bfloat16*,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         bool,
+                                                         bool,
+                                                         cudaStream_t,
+                                                         int);
+#endif
 template void launch_apply_rotary_pos_emb<__half>(__half*,
                                                   __half*,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   bool,
                                                   bool,
                                                   cudaStream_t,
                                                   int);
 
+template __global__ void apply_rotary_pos_emb(float* mixed_query,
+                                              float* key_layer,
+                                              unsigned rotary_dim,
+                                              unsigned seq_len,
+                                              unsigned seq_offset,
+                                              unsigned num_heads,
+                                              unsigned head_size,
+                                              unsigned total_count,
+                                              int max_out_tokens);
+
+#ifdef BF16_AVAILABLE
+template __global__ void apply_rotary_pos_emb(__nv_bfloat16* mixed_query,
+                                              __nv_bfloat16* key_layer,
+                                              unsigned rotary_dim,
+                                              unsigned seq_len,
+                                              unsigned seq_offset,
+                                              unsigned num_heads,
+                                              unsigned head_size,
+                                              unsigned total_count,
+                                              int max_out_tokens);
+#endif
+
+template __global__ void apply_rotary_pos_emb(__half* mixed_query,
+                                              __half* key_layer,
+                                              unsigned rotary_dim,
+                                              unsigned seq_len,
+                                              unsigned seq_offset,
+                                              unsigned num_heads,
+                                              unsigned head_size,
+                                              unsigned total_count,
+                                              int max_out_tokens);
+
+#ifdef BF16_AVAILABLE
+template __global__ void apply_rotary_pos_emb1(__nv_bfloat16* mixed_query,
+                                               __nv_bfloat16* key_layer,
+                                               unsigned rotary_dim,
+                                               unsigned seq_len,
+                                               unsigned seq_offset,
+                                               unsigned num_heads,
+                                               unsigned head_size,
+                                               unsigned total_count,
+                                               int max_out_tokens);
+#endif
+
+template __global__ void apply_rotary_pos_emb1(__half* mixed_query,
+                                               __half* key_layer,
+                                               unsigned rotary_dim,
+                                               unsigned seq_len,
+                                               unsigned seq_offset,
+                                               unsigned num_heads,
+                                               unsigned head_size,
+                                               unsigned total_count,
+                                               int max_out_tokens);
 /*
 __global__ void apply_rotary_pos_emb(float* mixed_query,
 float* key_layer,
 unsigned rotary_dim,
 unsigned seq_len,
 unsigned seq_offset,
 unsigned num_heads,
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/gelu.cu`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 #include "inference_cuda_layers.h"
 #include "memory_access_utils.h"
 
 namespace cg = cooperative_groups;
 #define MAX_CAP 4
 #define MAX_SEQ 2048
 
+// only used to avoid compilation error due to lack of definition.
+#ifndef BF16_AVAILABLE
+using __nv_bfloat162 = __half2;
+#endif
+
 inline __device__ float gelu(const float x)
 {
     const float sqrt_param = 0.79788456080286535587989211986876f;
     const float mul_param = 0.044715;
     return x * 0.5f * (1.0f + tanhf(sqrt_param * (x + mul_param * x * x * x)));
 }
 
@@ -62,14 +67,21 @@
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_gelu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
 template void launch_bias_gelu<float>(float*, const float*, int, int, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_gelu<__nv_bfloat16>(__nv_bfloat16*,
+                                              const __nv_bfloat16*,
+                                              int,
+                                              int,
+                                              cudaStream_t);
+#endif
 template void launch_bias_gelu<__half>(__half*, const __half*, int, int, cudaStream_t);
 
 /*
 In-place channels-last bias add
 */
 template <typename T>
 __global__ void fused_bias_add(T* input, const T* bias, int total_count, int intermediate_size)
@@ -112,14 +124,21 @@
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_add<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
 template void launch_bias_add<float>(float*, const float*, int, int, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_add<__nv_bfloat16>(__nv_bfloat16*,
+                                             const __nv_bfloat16*,
+                                             int,
+                                             int,
+                                             cudaStream_t);
+#endif
 template void launch_bias_add<__half>(__half*, const __half*, int, int, cudaStream_t);
 
 __global__ void fused_bias_residual(float* residual,
                                     const float* hidden_state,
                                     const float* attn,
                                     const float* bias,
                                     const float* attn_bias,
@@ -159,58 +178,61 @@
             res_fl4.z = res_fl4.z + hs_fl4.z + bias_fl4.z;
             res_fl4.w = res_fl4.w + hs_fl4.w + bias_fl4.w;
         }
         res_fl4_ptr[offset] = res_fl4;
     }
 }
 
-__global__ void fused_bias_residual(__half* residual,
-                                    const __half* hidden_state,
-                                    const __half* attn,
-                                    const __half* bias,
-                                    const __half* attn_bias,
+template <typename T>
+__global__ void fused_bias_residual(T* residual,
+                                    const T* hidden_state,
+                                    const T* attn,
+                                    const T* bias,
+                                    const T* attn_bias,
                                     const int total_count,
                                     const int intermediate_size,
                                     const float mp_scale,
                                     const bool preln)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float2* res_fl2_ptr = reinterpret_cast<float2*>(residual);
     const float2* hs_fl2_ptr = reinterpret_cast<const float2*>(hidden_state);
     const float2* attn_fl2_ptr = reinterpret_cast<const float2*>(attn);
     const float2* bias_fl2_ptr = reinterpret_cast<const float2*>(bias);
     const float2* attn_bias_fl2_ptr = reinterpret_cast<const float2*>(attn_bias);
     const int offset = blockIdx.x * blockDim.x + threadIdx.x;
 
     if (offset < total_count) {
         float2 res_fl2 = res_fl2_ptr[offset];
         const float2 hs_fl2 = hs_fl2_ptr[offset];
         const float2 attn_fl2 = attn_fl2_ptr[offset];
         const float2 bias_fl2 = bias_fl2_ptr[offset % intermediate_size];
         const float2 attn_bias_fl2 = attn_bias_fl2_ptr[offset % intermediate_size];
 
-        __half2* res_half2 = reinterpret_cast<__half2*>(&res_fl2);
-        const __half2* hs_half2 = reinterpret_cast<const __half2*>(&hs_fl2);
-        const __half2* attn_half2 = reinterpret_cast<const __half2*>(&attn_fl2);
-        const __half2* bias_half2 = reinterpret_cast<const __half2*>(&bias_fl2);
-        const __half2* attn_bias_half2 = reinterpret_cast<const __half2*>(&attn_bias_fl2);
-
-        float2 res_low = __half22float2(res_half2[0]);
-        float2 res_high = __half22float2(res_half2[1]);
-
-        const float2 hs_low = __half22float2(hs_half2[0]);
-        const float2 hs_high = __half22float2(hs_half2[1]);
+        T2* res_half2 = reinterpret_cast<T2*>(&res_fl2);
+        const T2* hs_half2 = reinterpret_cast<const T2*>(&hs_fl2);
+        const T2* attn_half2 = reinterpret_cast<const T2*>(&attn_fl2);
+        const T2* bias_half2 = reinterpret_cast<const T2*>(&bias_fl2);
+        const T2* attn_bias_half2 = reinterpret_cast<const T2*>(&attn_bias_fl2);
+
+        float2 res_low = conversion::to<float2>(res_half2[0]);
+        float2 res_high = conversion::to<float2>(res_half2[1]);
+
+        const float2 hs_low = conversion::to<float2>(hs_half2[0]);
+        const float2 hs_high = conversion::to<float2>(hs_half2[1]);
 
-        const float2 attn_low = __half22float2(attn_half2[0]);
-        const float2 attn_high = __half22float2(attn_half2[1]);
+        const float2 attn_low = conversion::to<float2>(attn_half2[0]);
+        const float2 attn_high = conversion::to<float2>(attn_half2[1]);
 
-        const float2 bias_low = __half22float2(bias_half2[0]);
-        const float2 bias_high = __half22float2(bias_half2[1]);
+        const float2 bias_low = conversion::to<float2>(bias_half2[0]);
+        const float2 bias_high = conversion::to<float2>(bias_half2[1]);
 
-        const float2 attn_bias_low = __half22float2(attn_bias_half2[0]);
-        const float2 attn_bias_high = __half22float2(attn_bias_half2[1]);
+        const float2 attn_bias_low = conversion::to<float2>(attn_bias_half2[0]);
+        const float2 attn_bias_high = conversion::to<float2>(attn_bias_half2[1]);
 
         if (preln) {
             // residual = (residual + attention + bias + attention_bias) *
             // mp_scale + hidden_state
             res_low.x =
                 (res_low.x + attn_low.x + bias_low.x + attn_bias_low.x) * mp_scale + hs_low.x;
             res_low.y =
@@ -222,16 +244,16 @@
         } else {
             // residual += hidden_state + bias
             res_low.x = (res_low.x + hs_low.x + bias_low.x);
             res_low.y = (res_low.y + hs_low.y + bias_low.y);
             res_high.x = (res_high.x + hs_high.x + bias_high.x);
             res_high.y = (res_high.y + hs_high.y + bias_high.y);
         }
-        res_half2[0] = __float22half2_rn(res_low);
-        res_half2[1] = __float22half2_rn(res_high);
+        res_half2[0] = conversion::to<T2>(res_low);
+        res_half2[1] = conversion::to<T2>(res_high);
 
         res_fl2_ptr[offset] = res_fl2;
     }
 }
 
 template <typename T>
 void launch_bias_residual(T* residual,
@@ -258,17 +280,51 @@
                                                               hidden_dim / 4,
                                                               1.0 / mp_size,
                                                               preln);
 }
 
 template void launch_bias_residual<
     float>(float*, float*, float*, float*, float*, int, int, int, bool, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_residual<__nv_bfloat16>(__nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  int,
+                                                  int,
+                                                  int,
+                                                  bool,
+                                                  cudaStream_t);
+#endif
 template void launch_bias_residual<
     __half>(__half*, __half*, __half*, __half*, __half*, int, int, int, bool, cudaStream_t);
 
+#ifdef BF16_AVAILABLE
+template __global__ void fused_bias_residual(__nv_bfloat16* residual,
+                                             const __nv_bfloat16* hidden_state,
+                                             const __nv_bfloat16* attn,
+                                             const __nv_bfloat16* bias,
+                                             const __nv_bfloat16* attn_bias,
+                                             const int total_count,
+                                             const int intermediate_size,
+                                             const float mp_scale,
+                                             const bool preln);
+#endif
+
+template __global__ void fused_bias_residual(__half* residual,
+                                             const __half* hidden_state,
+                                             const __half* attn,
+                                             const __half* bias,
+                                             const __half* attn_bias,
+                                             const int total_count,
+                                             const int intermediate_size,
+                                             const float mp_scale,
+                                             const bool preln);
+
 __global__ void gptj_residual_add(float* residual,
                                   const float* hidden_state,
                                   const float* attn,
                                   const float* bias,
                                   const float* attn_bias,
                                   const int total_count,
                                   const int intermediate_size,
@@ -301,72 +357,75 @@
         res_fl4.z = hs_fl4.z + attn_fl4.z + (res_fl4.z + bias_fl4.z) * mp_scale;
         res_fl4.w = hs_fl4.w + attn_fl4.w + (res_fl4.w + bias_fl4.w) * mp_scale;
 
         res_fl4_ptr[offset] = res_fl4;
     }
 }
 
-__global__ void gptj_residual_add(__half* residual,
-                                  const __half* hidden_state,
-                                  const __half* attn,
-                                  const __half* bias,
-                                  const __half* attn_bias,
+template <typename T>
+__global__ void gptj_residual_add(T* residual,
+                                  const T* hidden_state,
+                                  const T* attn,
+                                  const T* bias,
+                                  const T* attn_bias,
                                   const int total_count,
                                   const int intermediate_size,
                                   const float mp_scale)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float2* res_fl2_ptr = reinterpret_cast<float2*>(residual);
     const float2* hs_fl2_ptr = reinterpret_cast<const float2*>(hidden_state);
     const float2* attn_fl2_ptr = reinterpret_cast<const float2*>(attn);
     const float2* bias_fl2_ptr = reinterpret_cast<const float2*>(bias);
     const float2* attn_bias_fl2_ptr = reinterpret_cast<const float2*>(attn_bias);
     const int offset = blockIdx.x * blockDim.x + threadIdx.x;
 
     if (offset < total_count) {
         float2 res_fl2 = res_fl2_ptr[offset];
         const float2 hs_fl2 = hs_fl2_ptr[offset];
         const float2 attn_fl2 = attn_fl2_ptr[offset];
         const float2 bias_fl2 = bias_fl2_ptr[offset % intermediate_size];
 
-        __half2* res_half2 = reinterpret_cast<__half2*>(&res_fl2);
-        const __half2* hs_half2 = reinterpret_cast<const __half2*>(&hs_fl2);
-        const __half2* attn_half2 = reinterpret_cast<const __half2*>(&attn_fl2);
-        const __half2* bias_half2 = reinterpret_cast<const __half2*>(&bias_fl2);
-
-        float2 res_low = __half22float2(res_half2[0]);
-        float2 res_high = __half22float2(res_half2[1]);
+        T2* res_half2 = reinterpret_cast<T2*>(&res_fl2);
+        const T2* hs_half2 = reinterpret_cast<const T2*>(&hs_fl2);
+        const T2* attn_half2 = reinterpret_cast<const T2*>(&attn_fl2);
+        const T2* bias_half2 = reinterpret_cast<const T2*>(&bias_fl2);
+
+        float2 res_low = conversion::to<float2>(res_half2[0]);
+        float2 res_high = conversion::to<float2>(res_half2[1]);
 
-        const float2 hs_low = __half22float2(hs_half2[0]);
-        const float2 hs_high = __half22float2(hs_half2[1]);
+        const float2 hs_low = conversion::to<float2>(hs_half2[0]);
+        const float2 hs_high = conversion::to<float2>(hs_half2[1]);
 
-        const float2 attn_low = __half22float2(attn_half2[0]);
-        const float2 attn_high = __half22float2(attn_half2[1]);
+        const float2 attn_low = conversion::to<float2>(attn_half2[0]);
+        const float2 attn_high = conversion::to<float2>(attn_half2[1]);
 
-        const float2 bias_low = __half22float2(bias_half2[0]);
-        const float2 bias_high = __half22float2(bias_half2[1]);
+        const float2 bias_low = conversion::to<float2>(bias_half2[0]);
+        const float2 bias_high = conversion::to<float2>(bias_half2[1]);
 
         if (attn_bias) {
             const float2 attn_bias_fl2 = attn_bias_fl2_ptr[offset % intermediate_size];
-            const __half2* attn_bias_half2 = reinterpret_cast<const __half2*>(&attn_bias_fl2);
-            const float2 attn_bias_low = __half22float2(attn_bias_half2[0]);
-            const float2 attn_bias_high = __half22float2(attn_bias_half2[1]);
+            const T2* attn_bias_half2 = reinterpret_cast<const T2*>(&attn_bias_fl2);
+            const float2 attn_bias_low = conversion::to<float2>(attn_bias_half2[0]);
+            const float2 attn_bias_high = conversion::to<float2>(attn_bias_half2[1]);
             // residual += attention_bias
             res_low.x += attn_bias_low.x;
             res_low.y += attn_bias_low.y;
             res_high.x += attn_bias_high.x;
             res_high.y += attn_bias_high.y;
         }
         // residual = hidden_state + attention + (residual + bias) * mp_scale
         res_low.x = attn_low.x + hs_low.x + (res_low.x + bias_low.x) * mp_scale;
         res_low.y = attn_low.y + hs_low.y + (res_low.y + bias_low.y) * mp_scale;
         res_high.x = attn_high.x + hs_high.x + (res_high.x + bias_high.x) * mp_scale;
         res_high.y = attn_high.y + hs_high.y + (res_high.y + bias_high.y) * mp_scale;
 
-        res_half2[0] = __float22half2_rn(res_low);
-        res_half2[1] = __float22half2_rn(res_high);
+        res_half2[0] = conversion::to<T2>(res_low);
+        res_half2[1] = conversion::to<T2>(res_high);
 
         res_fl2_ptr[offset] = res_fl2;
     }
 }
 
 template <typename T>
 void launch_gptj_residual_add(T* residual,
@@ -392,23 +451,57 @@
                                               float*,
                                               float*,
                                               float*,
                                               int,
                                               int,
                                               int,
                                               cudaStream_t);
+
+#ifdef BF16_AVAILABLE
+template void launch_gptj_residual_add<__nv_bfloat16>(__nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      int,
+                                                      int,
+                                                      int,
+                                                      cudaStream_t);
+#endif
+
 template void launch_gptj_residual_add<__half>(__half*,
                                                __half*,
                                                __half*,
                                                __half*,
                                                __half*,
                                                int,
                                                int,
                                                int,
                                                cudaStream_t);
+
+#ifdef BF16_AVAILABLE
+template __global__ void gptj_residual_add(__nv_bfloat16* residual,
+                                           const __nv_bfloat16* hidden_state,
+                                           const __nv_bfloat16* attn,
+                                           const __nv_bfloat16* bias,
+                                           const __nv_bfloat16* attn_bias,
+                                           const int total_count,
+                                           const int intermediate_size,
+                                           const float mp_scale);
+#endif
+
+template __global__ void gptj_residual_add(__half* residual,
+                                           const __half* hidden_state,
+                                           const __half* attn,
+                                           const __half* bias,
+                                           const __half* attn_bias,
+                                           const int total_count,
+                                           const int intermediate_size,
+                                           const float mp_scale);
+
 template <typename T>
 __global__ void moe_res_matmul(T* residual, T* coef, T* mlp_out, int seq_len, int hidden_dim)
 {
     constexpr int granularity = 16;
     constexpr int vals_per_access = granularity / sizeof(T);
 
     T* residual_seq = residual + blockIdx.x * hidden_dim;
@@ -451,48 +544,60 @@
 
 template void launch_moe_res_matmul(float* residual,
                                     float* coef,
                                     float* mlp_out,
                                     int seq_len,
                                     int hidden_dim,
                                     cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void launch_moe_res_matmul(__nv_bfloat16* residual,
+                                    __nv_bfloat16* coef,
+                                    __nv_bfloat16* mlp_out,
+                                    int seq_len,
+                                    int hidden_dim,
+                                    cudaStream_t stream);
+#endif
+
 template void launch_moe_res_matmul(__half* residual,
                                     __half* coef,
                                     __half* mlp_out,
                                     int seq_len,
                                     int hidden_dim,
                                     cudaStream_t stream);
 
-__global__ void pad_data_kernel(__half* padded_output,
-                                __half* output,
-                                int head_size,
-                                int padded_head_size)
+template <typename T>
+__global__ void pad_data_kernel(T* padded_output, T* output, int head_size, int padded_head_size)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4* padded_output_cast = reinterpret_cast<float4*>(padded_output);
     float4* output_cast = reinterpret_cast<float4*>(output);
     int bid = blockIdx.x * (blockDim.y) + threadIdx.y;
     int idx = threadIdx.x;
     padded_output_cast += (bid * padded_head_size);
     output_cast += (bid * head_size);
     float4 ZERO;
-    const __half2 zero_h = __float2half2_rn(0.f);
-    __half2* ZERO_h = reinterpret_cast<__half2*>(&ZERO);
+    const T2 zero_h = conversion::to<T2>(0.f);
+    T2* ZERO_h = reinterpret_cast<T2*>(&ZERO);
 #pragma unroll
     for (int i = 0; i < 4; i++) ZERO_h[i] = zero_h;
     if (idx < head_size)
         padded_output_cast[idx] = output_cast[idx];
     else
         padded_output_cast[idx] = ZERO;
 }
+
 __global__ void pad_data_kernel(float* padded_output,
                                 float* output,
                                 int head_size,
                                 int padded_head_size)
 {
 }
+
 template <typename T>
 void pad_data(T* padded_output,
               T* output,
               int bsz,
               int head_size,
               int padded_head_size,
               cudaStream_t stream)
@@ -504,54 +609,81 @@
 }
 template void pad_data(__half* padded_output,
                        __half* output,
                        int bsz,
                        int head_size,
                        int padded_head_size,
                        cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void pad_data(__nv_bfloat16* padded_output,
+                       __nv_bfloat16* output,
+                       int bsz,
+                       int head_size,
+                       int padded_head_size,
+                       cudaStream_t stream);
+#endif
+
 template void pad_data(float* padded_output,
                        float* output,
                        int bsz,
                        int head_size,
                        int padded_head_size,
                        cudaStream_t stream);
 
-__global__ void pad_head_seq_kernel(__half* padded_output,
-                                    __half* output,
+#ifdef BF16_AVAILABLE
+template __global__ void pad_data_kernel(__nv_bfloat16* padded_output,
+                                         __nv_bfloat16* output,
+                                         int head_size,
+                                         int padded_head_size);
+#endif
+
+template __global__ void pad_data_kernel(__half* padded_output,
+                                         __half* output,
+                                         int head_size,
+                                         int padded_head_size);
+
+template <typename T>
+__global__ void pad_head_seq_kernel(T* padded_output,
+                                    T* output,
                                     int seq_len,
                                     int padded_seq_len,
                                     int head_size,
                                     int padded_head_size)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4* padded_output_cast = reinterpret_cast<float4*>(padded_output);
     float4* output_cast = reinterpret_cast<float4*>(output);
     int bsz = blockIdx.x;
     int bid = blockIdx.y * (blockDim.y) + threadIdx.y;
     int idx = threadIdx.x;
     padded_output_cast += (bsz * padded_seq_len + bid) * padded_head_size;
     output_cast += (bsz * seq_len + bid) * head_size;
     float4 ZERO;
-    const __half2 zero_h = __float2half2_rn(0.f);
-    __half2* ZERO_h = reinterpret_cast<__half2*>(&ZERO);
+    const T2 zero_h = conversion::to<T2>(0.f);
+    T2* ZERO_h = reinterpret_cast<T2*>(&ZERO);
 #pragma unroll
     for (int i = 0; i < 4; i++) ZERO_h[i] = zero_h;
 
     if (idx < head_size && bid < seq_len)
         padded_output_cast[idx] = output_cast[idx];
     else
         padded_output_cast[idx] = ZERO;
 }
+
 __global__ void pad_head_seq_kernel(float* padded_output,
                                     float* output,
                                     int seq_len,
                                     int padded_seq_len,
                                     int head_size,
                                     int padded_head_size)
 {
 }
+
 template <typename T>
 void pad_head_seq(T* padded_output,
                   T* output,
                   int bsz,
                   int seq_len,
                   int padded_seq_len,
                   int head_size,
@@ -559,22 +691,35 @@
                   cudaStream_t stream)
 {
     dim3 grid_dim(bsz, padded_seq_len / 16);
     dim3 block_dim(padded_head_size / 8, 16);
     pad_head_seq_kernel<<<grid_dim, block_dim, 0, stream>>>(
         padded_output, output, seq_len, padded_seq_len, head_size / 8, padded_head_size / 8);
 }
+
 template void pad_head_seq(__half* padded_output,
                            __half* output,
                            int bsz,
                            int seq_len,
                            int padded_seq_len,
                            int head_size,
                            int padded_head_size,
                            cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void pad_head_seq(__nv_bfloat16* padded_output,
+                           __nv_bfloat16* output,
+                           int bsz,
+                           int seq_len,
+                           int padded_seq_len,
+                           int head_size,
+                           int padded_head_size,
+                           cudaStream_t stream);
+#endif
+
 template void pad_head_seq(float* padded_output,
                            float* output,
                            int bsz,
                            int seq_len,
                            int padded_seq_len,
                            int head_size,
                            int padded_head_size,
@@ -677,8 +822,16 @@
 
 template void launch_fused_bias_geglu(__half*,
                                       const __half*,
                                       const __half*,
                                       int,
                                       int,
                                       cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_fused_bias_geglu(__nv_bfloat16*,
+                                      const __nv_bfloat16*,
+                                      const __nv_bfloat16*,
+                                      int,
+                                      int,
+                                      cudaStream_t);
+#endif
 template void launch_fused_bias_geglu(float*, const float*, const float*, int, int, cudaStream_t);
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,24 @@
                               const __half*,
                               const __half*,
                               const __half*,
                               float,
                               int,
                               int,
                               cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_fused_ln(__nv_bfloat16*,
+                              const __nv_bfloat16*,
+                              const __nv_bfloat16*,
+                              const __nv_bfloat16*,
+                              float,
+                              int,
+                              int,
+                              cudaStream_t);
+#endif
 template void
 launch_fused_ln(float*, const float*, const float*, const float*, float, int, int, cudaStream_t);
 
 /*
 Fused resiual + bias + layer norm implementation. Assumes elems_per_row % 8
 is equal to 0.
 
@@ -489,14 +499,27 @@
                                        const __half*,
                                        const __half*,
                                        float,
                                        int,
                                        int,
                                        cudaStream_t);
 
+#ifdef BF16_AVAILABLE
+template void launch_fused_residual_ln(__nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       float,
+                                       int,
+                                       int,
+                                       cudaStream_t);
+#endif
+
 template void launch_fused_residual_ln(float*,
                                        const float*,
                                        const float*,
                                        const float*,
                                        const float*,
                                        const float*,
                                        float,
@@ -513,14 +536,28 @@
                                                         const __half*,
                                                         const __half*,
                                                         float,
                                                         int,
                                                         int,
                                                         cudaStream_t);
 
+#ifdef BF16_AVAILABLE
+template void launch_fused_residual_ln_store_pre_ln_res(__nv_bfloat16*,
+                                                        __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        float,
+                                                        int,
+                                                        int,
+                                                        cudaStream_t);
+#endif
+
 template void launch_fused_residual_ln_store_pre_ln_res(float*,
                                                         float*,
                                                         const float*,
                                                         const float*,
                                                         const float*,
                                                         const float*,
                                                         const float*,
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1740,87 +1740,75 @@
 
 void ds_release_workspace() { InferenceContext::Instance().release_workspace(); }
 
 bool ds_retake_workspace() { return InferenceContext::Instance().retake_workspace(); }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
-    m.def("softmax_fp32", &ds_softmax<float>, "DeepSpeed SoftMax with fp32 (CUDA)");
-    m.def("softmax_fp16", &ds_softmax<__half>, "DeepSpeed SoftMax with fp16 (CUDA)");
-    m.def(
-        "softmax_context_fp32", &ds_softmax_context<float>, "DeepSpeed attention with fp32 (CUDA)");
-    m.def("softmax_context_fp16",
-          &ds_softmax_context<__half>,
-          "DeepSpeed attention with fp16 (CUDA)");
     m.def("softmax_context_int8",
           &ds_softmax_context1<__half>,
           "DeepSpeed attention with int8 (CUDA)");
-    m.def("bias_gelu_fp32", &ds_bias_gelu<float>, "DeepSpeed Gelu with fp32 (CUDA)");
-    m.def("bias_gelu_fp16", &ds_bias_gelu<__half>, "DeepSpeed Gelu with fp16 (CUDA)");
     m.def("bias_geglu", &ds_bias_geglu, "DeepSpeed Bias GEGLU (CUDA)");
-    m.def("bias_add_fp32", &ds_bias_add<float>, "DeepSpeed Bias Add with fp32 (CUDA)");
-    m.def("bias_add_fp16", &ds_bias_add<__half>, "DeepSpeed Gelu with fp16 (CUDA)");
-    m.def("bias_relu_fp32", &ds_bias_relu<float>, "DeepSpeed ReLU with fp32 (CUDA)");
-    m.def("bias_relu_fp16", &ds_bias_relu<__half>, "DeepSpeed ReLU with fp16 (CUDA)");
-    m.def("bias_residual_fp32",
-          &ds_bias_residual<float>,
-          "DeepSpeed residual-bias add with fp32 (CUDA)");
-    m.def("bias_residual_fp16",
-          &ds_bias_residual<__half>,
-          "DeepSpeed residual-bias add with fp16 (CUDA)");
     m.def("layer_norm", &ds_layer_norm, "DeepSpeed layer norm (CUDA)");
     m.def(
         "_layer_norm_residual", &ds_layer_norm_residual, "DeepSpeed layer norm + residual (CUDA)");
     m.def("layer_norm_residual_store_pre_ln_res",
           &ds_layer_norm_residual_store_pre_ln_res,
           "DeepSpeed layer norm + store pre Layernorm residual (CUDA)");
-    m.def("qkv_gemm_fp32", &ds_qkv_gemm<float>, "DeepSpeed qkv gemm with fp32 (CUDA)");
-    m.def("qkv_gemm_fp16", &ds_qkv_gemm<__half>, "DeepSpeed qkv gemm with fp16 (CUDA)");
     m.def("qkv_gemm_int8", &ds_qkv_gemm_int8<__half>, "DeepSpeed qkv gemm with int8 (CUDA)");
-    m.def("mlp_gemm_fp32", &ds_mlp_gemm<float>, "DeepSpeed mlp with fp32 (CUDA)");
-    m.def("mlp_gemm_fp16", &ds_mlp_gemm<__half>, "DeepSpeed mlp with fp16 (CUDA)");
     m.def("mlp_gemm_int8", &ds_mlp_gemm_int8<__half>, "DeepSpeed mlp with int8 (CUDA)");
-    m.def("vector_matmul_fp32", &ds_vector_matmul<float>, "DeepSpeed vector-MM with fp32 (CUDA)");
-    m.def("vector_matmul_fp16", &ds_vector_matmul<__half>, "DeepSpeed vector-MM with fp16 (CUDA)");
     m.def("vector_matmul_int8",
           &ds_vector_matmul_int8<__half>,
           "DeepSpeed vector-MM with int8 (CUDA)");
-    m.def("linear_layer_fp32", &ds_linear_layer<float>, "DeepSpeed linear_layer with fp32 (CUDA)");
-    m.def("linear_layer_fp16", &ds_linear_layer<__half>, "DeepSpeed linear_layer with fp16 (CUDA)");
     m.def("linear_layer_int8",
           &ds_linear_layer_int8<__half>,
           "DeepSpeed linear_layer with int8 (CUDA)");
-    m.def("fused_gemm_gelu_fp32", &fused_gemm_gelu<float>, "DeepSpeed mlp with fp32 (CUDA)");
-    m.def("fused_gemm_gelu_fp16", &fused_gemm_gelu<__half>, "DeepSpeed mlp with fp16 (CUDA)");
-    m.def("residual_add_bias_fp32",
-          &residual_add_bias<float>,
-          "DeepSpeed residual add with fp32 (CUDA)");
-    m.def("residual_add_bias_fp16",
-          &residual_add_bias<__half>,
-          "DeepSpeed residual add with fp16 (CUDA)");
     m.def("apply_rotary_pos_emb", &apply_rotary_pos_emb, "DeepSpeed mlp with fp16 (CUDA)");
-    m.def("einsum_sec_sm_ecm_fp32",
-          &einsum_sec_sm_ecm<float>,
-          "DeepSpeed vector-MM with fp32 (CUDA)");
-
-    m.def("einsum_sec_sm_ecm_fp16",
-          &einsum_sec_sm_ecm<__half>,
-          "DeepSpeed vector-MM with fp16 (CUDA)");
     m.def("moe_res_matmul", &moe_res_matmul, "DeepSpeed moe residual matmul (CUDA)");
-    m.def("add_padding_fp32", &add_padding<float>, "DeepSpeed residual add with fp32 (CUDA)");
-    m.def("add_padding_fp16", &add_padding<__half>, "DeepSpeed residual add with fp16 (CUDA)");
-    m.def("pad_transform_fp32",
-          &padd_add_transform<float>,
-          "DeepSpeed residual add with fp32 (CUDA)");
-    m.def("pad_transform_fp16",
-          &padd_add_transform<__half>,
-          "DeepSpeed residual add with fp16 (CUDA)");
-    m.def("allocate_workspace_fp32",
-          &allocate_workspace<float>,
-          "DeepSpeed memory allocation for GPT inference with fp32 (CUDA)");
-    m.def("allocate_workspace_fp16",
-          &allocate_workspace<__half>,
-          "DeepSpeed memory allocation for GPT inference with fp16 (CUDA)");
     m.def("reset_cache", &reset_cache, "Reset Cache for generation tasks");
     m.def("release_workspace", &ds_release_workspace, "DeepSpeed Release Workspace");
     m.def("retake_workspace", &ds_retake_workspace, "DeepSpeed Retake Workspace");
+
+#define DEF_OPS(_name, _dtype)                                                                    \
+    m.def("softmax_" #_name, &ds_softmax<_dtype>, "DeepSpeed SoftMax with " #_name " (CUDA)");    \
+    m.def("softmax_context_" #_name,                                                              \
+          &ds_softmax_context<_dtype>,                                                            \
+          "DeepSpeed attention with _name (CUDA)");                                               \
+    m.def("bias_gelu_" #_name, &ds_bias_gelu<_dtype>, "DeepSpeed Gelu with " #_name " (CUDA)");   \
+    m.def("bias_add_" #_name, &ds_bias_add<_dtype>, "DeepSpeed Bias Add with " #_name " (CUDA)"); \
+    m.def("bias_relu_" #_name, &ds_bias_relu<_dtype>, "DeepSpeed ReLU with " #_name " (CUDA)");   \
+    m.def("bias_residual_" #_name,                                                                \
+          &ds_bias_residual<_dtype>,                                                              \
+          "DeepSpeed residual-bias add with " #_name " (CUDA)");                                  \
+    m.def("qkv_gemm_" #_name, &ds_qkv_gemm<_dtype>, "DeepSpeed qkv gemm with " #_name " (CUDA)"); \
+    m.def("mlp_gemm_" #_name, &ds_mlp_gemm<_dtype>, "DeepSpeed mlp with " #_name " (CUDA)");      \
+    m.def("vector_matmul_" #_name,                                                                \
+          &ds_vector_matmul<_dtype>,                                                              \
+          "DeepSpeed vector-MM with " #_name " (CUDA)");                                          \
+    m.def("linear_layer_" #_name,                                                                 \
+          &ds_linear_layer<_dtype>,                                                               \
+          "DeepSpeed linear_layer with " #_name " (CUDA)");                                       \
+    m.def("fused_gemm_gelu_" #_name,                                                              \
+          &fused_gemm_gelu<_dtype>,                                                               \
+          "DeepSpeed mlp with " #_name " (CUDA)");                                                \
+    m.def("residual_add_bias_" #_name,                                                            \
+          &residual_add_bias<_dtype>,                                                             \
+          "DeepSpeed residual add with " #_name " (CUDA)");                                       \
+    m.def("einsum_sec_sm_ecm_" #_name,                                                            \
+          &einsum_sec_sm_ecm<_dtype>,                                                             \
+          "DeepSpeed vector-MM with " #_name " (CUDA)");                                          \
+    m.def("add_padding_" #_name,                                                                  \
+          &add_padding<_dtype>,                                                                   \
+          "DeepSpeed residual add with " #_name " (CUDA)");                                       \
+    m.def("pad_transform_" #_name,                                                                \
+          &padd_add_transform<_dtype>,                                                            \
+          "DeepSpeed residual add with " #_name " (CUDA)");                                       \
+    m.def("allocate_workspace_" #_name,                                                           \
+          &allocate_workspace<_dtype>,                                                            \
+          "DeepSpeed memory allocation for GPT inference with " #_name " (CUDA)")
+
+    DEF_OPS(fp32, float);
+    DEF_OPS(fp16, __half);
+#ifdef BF16_AVAILABLE
+    DEF_OPS(bf16, __nv_bfloat16);
+#endif
 }
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/relu.cu`

 * *Files 7% similar despite different names*

```diff
@@ -57,8 +57,15 @@
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_relu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
 template void launch_bias_relu<float>(float*, const float*, int, int, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_relu<__nv_bfloat16>(__nv_bfloat16*,
+                                              const __nv_bfloat16*,
+                                              int,
+                                              int,
+                                              cudaStream_t);
+#endif
 template void launch_bias_relu<__half>(__half*, const __half*, int, int, cudaStream_t);
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/softmax.cu`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 // Copyright (c) Microsoft Corporation.
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
 #include <limits>
+#include "conversion_utils.h"
 #include "inference_cuda_layers.h"
 
 #ifndef __HIP_PLATFORM_HCC__
 #include <cuda_profiler_api.h>
 #endif
 #include <cstdio>
 #include <cstdlib>
@@ -26,18 +27,18 @@
     throw std::runtime_error("CUDA ERROR!!!\n");
 }
 
 #define CUDA_CHECK_ERROR() CheckCudaErrorAux(__FILE__, __LINE__)
 
 namespace cg = cooperative_groups;
 
-template <int iterations>
-__global__ void attn_softmax_v2(__half* vals,
-                                __half* mask,
-                                __half* alibi,
+template <typename T, int iterations>
+__global__ void attn_softmax_v2(T* vals,
+                                T* mask,
+                                T* alibi,
                                 float layer_scale,
                                 bool triangular,
                                 bool recompute,
                                 bool local_attention,
                                 int window_size,
                                 int total_count,
                                 int heads,
@@ -49,15 +50,15 @@
                                 int reduceWidth)
 {
     cg::thread_block b = cg::this_thread_block();
     cg::thread_block_tile<WARP_SIZE> g = cg::tiled_partition<WARP_SIZE>(b);
 
     float2 low_data[MAX_REG_SIZE];
     float2 high_data[MAX_REG_SIZE];
-    const __half zero_h = __float2half(0.f);
+    const T zero_h = conversion::to<T>(0.f);
 
     int wid = threadIdx.x >> 5;
     int lane = threadIdx.x & 0x1f;
     int warp_num = blockDim.x >> 5;
 
     int reduce_blocks = reduceWidth >> 5;
     int seq_lane = threadIdx.x % reduceWidth;
@@ -97,81 +98,95 @@
                                 (!triangular || ((data_id + reduceWidth * 2) <= seq_id)) &&
                                 ((data_id + reduceWidth * 2) > window_stride);
             bool high_y_check = check && ((data_id + reduceWidth * 3) < sequence_length) &&
                                 (!triangular || ((data_id + reduceWidth * 3) <= seq_id)) &&
                                 ((data_id + reduceWidth * 3) > window_stride);
 
             if (mask && alibi) {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale +
-                                                  (__half2float(alibi[data_id + alibi_offset])) +
-                                                  (__half2float(mask[data_id + mask_offset]))
-                                            : minus_infinity;
+                low_data[i].x = low_x_check
+                                    ? conversion::to<float>(vals[data_id]) * layer_scale +
+                                          (conversion::to<float>(alibi[data_id + alibi_offset])) +
+                                          (conversion::to<float>(mask[data_id + mask_offset]))
+                                    : minus_infinity;
                 low_data[i].y =
-                    low_y_check ? __half2float(vals[data_id + reduceWidth]) * layer_scale +
-                                      (__half2float(alibi[data_id + alibi_offset + reduceWidth])) +
-                                      (__half2float(mask[data_id + mask_offset + reduceWidth]))
-                                : minus_infinity;
+                    low_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale +
+                              (conversion::to<float>(alibi[data_id + alibi_offset + reduceWidth])) +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth]))
+                        : minus_infinity;
                 high_data[i].x =
                     high_x_check
-                        ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 2])) +
-                              (__half2float(mask[data_id + mask_offset + reduceWidth * 2]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 2])) +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 2]))
                         : minus_infinity;
                 high_data[i].y =
                     high_y_check
-                        ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 3])) +
-                              (__half2float(mask[data_id + mask_offset + reduceWidth * 3]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 3])) +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 3]))
                         : minus_infinity;
             } else if (mask) {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale +
-                                                  (__half2float(mask[data_id + mask_offset]))
-                                            : minus_infinity;
-                low_data[i].y = low_y_check
-                                    ? __half2float(vals[data_id + reduceWidth]) * layer_scale +
-                                          (__half2float(mask[data_id + mask_offset + reduceWidth]))
+                low_data[i].x = low_x_check
+                                    ? conversion::to<float>(vals[data_id]) * layer_scale +
+                                          (conversion::to<float>(mask[data_id + mask_offset]))
                                     : minus_infinity;
+                low_data[i].y =
+                    low_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth]))
+                        : minus_infinity;
                 high_data[i].x =
-                    high_x_check ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale +
-                                       (__half2float(mask[data_id + mask_offset + reduceWidth * 2]))
-                                 : minus_infinity;
+                    high_x_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 2]))
+                        : minus_infinity;
                 high_data[i].y =
-                    high_y_check ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale +
-                                       (__half2float(mask[data_id + mask_offset + reduceWidth * 3]))
-                                 : minus_infinity;
+                    high_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 3]))
+                        : minus_infinity;
             } else if (alibi) {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale +
-                                                  (__half2float(alibi[data_id + alibi_offset]))
-                                            : minus_infinity;
+                low_data[i].x = low_x_check
+                                    ? conversion::to<float>(vals[data_id]) * layer_scale +
+                                          (conversion::to<float>(alibi[data_id + alibi_offset]))
+                                    : minus_infinity;
                 low_data[i].y =
-                    low_y_check ? __half2float(vals[data_id + reduceWidth]) * layer_scale +
-                                      (__half2float(alibi[data_id + alibi_offset + reduceWidth]))
-                                : minus_infinity;
+                    low_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale +
+                              (conversion::to<float>(alibi[data_id + alibi_offset + reduceWidth]))
+                        : minus_infinity;
                 high_data[i].x =
                     high_x_check
-                        ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 2]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 2]))
                         : minus_infinity;
                 high_data[i].y =
                     high_y_check
-                        ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 3]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 3]))
                         : minus_infinity;
             } else {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale
+                low_data[i].x = low_x_check ? conversion::to<float>(vals[data_id]) * layer_scale
                                             : minus_infinity;
-                low_data[i].y = low_y_check
-                                    ? __half2float(vals[data_id + reduceWidth]) * layer_scale
-                                    : minus_infinity;
-                high_data[i].x = high_x_check
-                                     ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale
-                                     : minus_infinity;
-                high_data[i].y = high_y_check
-                                     ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale
-                                     : minus_infinity;
+                low_data[i].y =
+                    low_y_check ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale
+                                : minus_infinity;
+                high_data[i].x =
+                    high_x_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale
+                        : minus_infinity;
+                high_data[i].y =
+                    high_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale
+                        : minus_infinity;
             }
 
             // if(lane == 0) printf("%f , %d, %d \n", low_data[i].x, data_id, seq_id);
             max_val = (low_data[i].x > max_val ? low_data[i].x : max_val);
             max_val = (low_data[i].y > max_val ? low_data[i].y : max_val);
             max_val = (high_data[i].x > max_val ? high_data[i].x : max_val);
             max_val = (high_data[i].y > max_val ? high_data[i].y : max_val);
@@ -221,21 +236,21 @@
 
             sum = g.shfl(sum, threadIdx.x / WARP_SIZE);
         }
         sum += 1e-6;
         for (int i = 0; i < iterations; i++) {
             int data_id = i * (reduceWidth << 2) + (seq_lane);
             if (data_id < sequence_length) {
-                vals[data_id] = __float2half(low_data[i].x / sum);
+                vals[data_id] = conversion::to<T>(low_data[i].x / sum);
                 if ((data_id + reduceWidth) < sequence_length)
-                    vals[data_id + reduceWidth] = __float2half(low_data[i].y / sum);
+                    vals[data_id + reduceWidth] = conversion::to<T>(low_data[i].y / sum);
                 if ((data_id + reduceWidth * 2) < sequence_length)
-                    vals[data_id + reduceWidth * 2] = __float2half(high_data[i].x / sum);
+                    vals[data_id + reduceWidth * 2] = conversion::to<T>(high_data[i].x / sum);
                 if ((data_id + reduceWidth * 3) < sequence_length)
-                    vals[data_id + reduceWidth * 3] = __float2half(high_data[i].y / sum);
+                    vals[data_id + reduceWidth * 3] = conversion::to<T>(high_data[i].y / sum);
             }
         }
     }
 }
 
 template <int iterations>
 __global__ void attn_softmax_v2(float* vals,
@@ -385,31 +400,31 @@
                 if ((data_id + reduceWidth * 3) < sequence_length)
                     vals[data_id + reduceWidth * 3] = data[i].w / sum;
             }
         }
     }
 }
 
-#define LAUNCH_ATTN_SOFTMAX_V2(iterations)                                   \
-    attn_softmax_v2<iterations><<<grid, block, 0, stream>>>(vals,            \
-                                                            mask,            \
-                                                            alibi,           \
-                                                            layer_scale,     \
-                                                            triangular,      \
-                                                            recompute,       \
-                                                            local_attention, \
-                                                            window_size,     \
-                                                            total_count,     \
-                                                            heads,           \
-                                                            sequence_length, \
-                                                            num_seq,         \
-                                                            head_offset,     \
-                                                            mask_stride,     \
-                                                            mp_size,         \
-                                                            reduce_width);
+#define LAUNCH_ATTN_SOFTMAX_V2(iterations)                                      \
+    attn_softmax_v2<T, iterations><<<grid, block, 0, stream>>>(vals,            \
+                                                               mask,            \
+                                                               alibi,           \
+                                                               layer_scale,     \
+                                                               triangular,      \
+                                                               recompute,       \
+                                                               local_attention, \
+                                                               window_size,     \
+                                                               total_count,     \
+                                                               heads,           \
+                                                               sequence_length, \
+                                                               num_seq,         \
+                                                               head_offset,     \
+                                                               mask_stride,     \
+                                                               mp_size,         \
+                                                               reduce_width);
 
 template <typename T>
 void launch_attn_softmax_v2(T* vals,
                             T* mask,
                             T* alibi,
                             float layer_scale,
                             bool triangular,
@@ -484,14 +499,34 @@
                                      int heads,
                                      int num_seq,
                                      int sequence_length,
                                      int head_offset,
                                      int mask_stride,
                                      int mp_size,
                                      cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void launch_attn_softmax_v2(__nv_bfloat16* vals,
+                                     __nv_bfloat16* mask,
+                                     __nv_bfloat16* alibi,
+                                     float layer_scale,
+                                     bool triangular,
+                                     bool recompute,
+                                     bool local_attention,
+                                     int window_size,
+                                     int batch_size,
+                                     int heads,
+                                     int num_seq,
+                                     int sequence_length,
+                                     int head_offset,
+                                     int mask_stride,
+                                     int mp_size,
+                                     cudaStream_t stream);
+#endif
+
 template void launch_attn_softmax_v2(__half* vals,
                                      __half* mask,
                                      __half* alibi,
                                      float layer_scale,
                                      bool triangular,
                                      bool recompute,
                                      bool local_attention,
@@ -500,7 +535,57 @@
                                      int heads,
                                      int num_seq,
                                      int sequence_length,
                                      int head_offset,
                                      int mask_stride,
                                      int mp_size,
                                      cudaStream_t stream);
+
+#define DEF_ATTN_SOFTMAX_V2_HALF(_iter)                                           \
+    template __global__ void attn_softmax_v2<__half, _iter>(__half * vals,        \
+                                                            __half * mask,        \
+                                                            __half * alibi,       \
+                                                            float layer_scale,    \
+                                                            bool triangular,      \
+                                                            bool recompute,       \
+                                                            bool local_attention, \
+                                                            int window_size,      \
+                                                            int total_count,      \
+                                                            int heads,            \
+                                                            int sequence_length,  \
+                                                            int num_seq,          \
+                                                            int head_offset,      \
+                                                            int mask_stride,      \
+                                                            int mp_size,          \
+                                                            int reduceWidth)
+
+#define DEF_ATTN_SOFTMAX_V2_BF16(_iter)                                                   \
+    template __global__ void attn_softmax_v2<__nv_bfloat16, _iter>(__nv_bfloat16 * vals,  \
+                                                                   __nv_bfloat16 * mask,  \
+                                                                   __nv_bfloat16 * alibi, \
+                                                                   float layer_scale,     \
+                                                                   bool triangular,       \
+                                                                   bool recompute,        \
+                                                                   bool local_attention,  \
+                                                                   int window_size,       \
+                                                                   int total_count,       \
+                                                                   int heads,             \
+                                                                   int sequence_length,   \
+                                                                   int num_seq,           \
+                                                                   int head_offset,       \
+                                                                   int mask_stride,       \
+                                                                   int mp_size,           \
+                                                                   int reduceWidth)
+
+#define FOREACH_ITERATIONS(cb) \
+    cb(1);                     \
+    cb(2);                     \
+    cb(4);                     \
+    cb(8);                     \
+    cb(16);                    \
+    cb(32);                    \
+    cb(64)
+
+FOREACH_ITERATIONS(DEF_ATTN_SOFTMAX_V2_HALF);
+#ifdef BF16_AVAILABLE
+FOREACH_ITERATIONS(DEF_ATTN_SOFTMAX_V2_BF16);
+#endif
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.2/csrc/transformer/inference/csrc/transform.cu`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
 #ifndef __HIP_PLATFORM_HCC__
 #include <cuda_profiler_api.h>
 #endif
+#include "conversion_utils.h"
 #include "inference_cuda_layers.h"
 namespace cg = cooperative_groups;
 
+// only used to avoid compilation error due to lack of definition.
+#ifndef BF16_AVAILABLE
+using __nv_bfloat162 = __half2;
+#endif
+
 // Bias add
 
 __global__ void bias_add_transform_0213(float* output,
                                         float* k_cache,
                                         float* v_cache,
                                         const float* vals,
                                         const float* bias,
@@ -71,30 +77,33 @@
     } else
         output_vec[d3] = inputs;
 }
 
 #define ATTN_H 3
 #define MAX_SEQ_LINE 10
 
-__global__ void bias_add_transform_0213(__half* output,  // q
-                                        __half* k_cache,
-                                        __half* v_cache,
-                                        const __half* vals,  // qkv
-                                        const __half* bias,
+template <typename T>
+__global__ void bias_add_transform_0213(T* output,  // q
+                                        T* k_cache,
+                                        T* v_cache,
+                                        const T* vals,  // qkv
+                                        const T* bias,
                                         int hidden_dim,
                                         int seq_length,
                                         unsigned seq_offset,
                                         int all_tokens,
                                         int heads,
                                         int rotary_dim,
                                         bool rotate_half,
                                         bool rotate_every_two,
                                         int head_ext,
                                         int max_out_tokens)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     unsigned half_dim = (rotary_dim << 3) >> 1;
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
     int d0 = blockIdx.x;                                                  // Batch
     int d1 = blockIdx.y;                                                  // Sequence ID (0-127)
@@ -104,16 +113,16 @@
 
     int d2_out_stride = d2_stride * (cnt == 0 ? seq_length : max_out_tokens);
     int d0_out_stride = hidden_dim * (cnt == 0 ? seq_length : max_out_tokens);
 
     float4 vals_arr;
     float4 output_arr;
 
-    __half2* vals_half = reinterpret_cast<__half2*>(&vals_arr);
-    __half2* output_half = reinterpret_cast<__half2*>(&output_arr);
+    T2* vals_half = reinterpret_cast<T2*>(&vals_arr);
+    T2* output_half = reinterpret_cast<T2*>(&output_arr);
 
     const float4* vals_vec = reinterpret_cast<const float4*>(vals);
     float4* output_vec =
         reinterpret_cast<float4*>(cnt == 0 ? output : (cnt == 1 ? k_cache : v_cache));
 
     vals_vec += (d0 * d0_stride * (gridDim.z / head_ext));
     vals_vec += (d1 * d1_stride * (gridDim.z / head_ext));
@@ -125,25 +134,27 @@
     output_vec += (d2 * d2_out_stride);
 
     unsigned seq_id = d1 + seq_offset;
 
     int lane = d3 & 0x1f;
     if (cnt < 2 && rotary_dim > 0 && d3 < rotary_dim) {
         float4 q = vals_vec[d3];
-        __half2* q_h = reinterpret_cast<__half2*>(&q);
+        T2* q_h = reinterpret_cast<T2*>(&q);
         if (rotate_every_two) {
 #pragma unroll
             for (int o = 0; o < 4; o++) {
                 float inv_freq = (float)(((d3 << 2) + o) * 2) / (float)(rotary_dim << 3);
                 inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
                 float q_data[2];
-                q_data[0] = (float)q_h[o].x;
-                q_data[1] = (float)q_h[o].y;
-                q_h[o].x = (__half)(-1.0 * q_data[1] * sinf(inv_freq) + q_data[0] * cosf(inv_freq));
-                q_h[o].y = (__half)(q_data[0] * sinf(inv_freq) + q_data[1] * cosf(inv_freq));
+                q_data[0] = conversion::to<float>(q_h[o].x);
+                q_data[1] = conversion::to<float>(q_h[o].y);
+                q_h[o].x = conversion::to<T>(-1.0 * q_data[1] * sinf(inv_freq) +
+                                             q_data[0] * cosf(inv_freq));
+                q_h[o].y =
+                    conversion::to<T>(q_data[0] * sinf(inv_freq) + q_data[1] * cosf(inv_freq));
             }
         }
         output_vec[d3] = q;
     } else
         output_vec[d3] = vals_vec[d3];
 }
 
@@ -184,50 +195,33 @@
                                                                 heads,
                                                                 rotary_dim >> 2,
                                                                 rotate_half,
                                                                 rotate_every_two,
                                                                 head_ext,
                                                                 max_out_tokens);
 }
+
 template <typename T>
-void launch_bias_add_transform_0213(T* outputs,
-                                    T* vals,
-                                    T* vals1,
-                                    const T* vals2,
+void launch_bias_add_transform_0213(T* output,
+                                    T* k_cache,
+                                    T* v_cache,
+                                    const T* vals,
                                     const T* bias,
                                     int batch_size,
                                     int seq_length,
                                     unsigned seq_offset,
-                                    int seq_length1,
+                                    int all_tokens,
                                     int hidden_dim,
                                     int heads,
                                     int rotary_dim,
                                     bool rotate_half,
                                     bool rotate_every_two,
                                     cudaStream_t stream,
                                     int trans_count,
-                                    int max_out_tokens);
-template <>
-void launch_bias_add_transform_0213<__half>(__half* output,
-                                            __half* k_cache,
-                                            __half* v_cache,
-                                            const __half* vals,
-                                            const __half* bias,
-                                            int batch_size,
-                                            int seq_length,
-                                            unsigned seq_offset,
-                                            int all_tokens,
-                                            int hidden_dim,
-                                            int heads,
-                                            int rotary_dim,
-                                            bool rotate_half,
-                                            bool rotate_every_two,
-                                            cudaStream_t stream,
-                                            int trans_count,
-                                            int max_out_tokens)
+                                    int max_out_tokens)
 {
     hidden_dim >>= 3;
     int head_ext = 1;  // (hidden_dim - 1) / MAX_THREADS + 1;
     dim3 block_dim(hidden_dim / heads, (heads / head_ext));
     dim3 grid_dim(batch_size, seq_length, (trans_count * head_ext));
     bias_add_transform_0213<<<grid_dim, block_dim, 0, stream>>>(output,
                                                                 k_cache,
@@ -242,37 +236,78 @@
                                                                 rotary_dim >> 3,
                                                                 rotate_half,
                                                                 rotate_every_two,
                                                                 head_ext,
                                                                 max_out_tokens);
 }
 
+#ifdef BF16_AVAILABLE
+template void launch_bias_add_transform_0213(__nv_bfloat16* output,
+                                             __nv_bfloat16* k_cache,
+                                             __nv_bfloat16* v_cache,
+                                             const __nv_bfloat16* vals,
+                                             const __nv_bfloat16* bias,
+                                             int batch_size,
+                                             int seq_length,
+                                             unsigned seq_offset,
+                                             int all_tokens,
+                                             int hidden_dim,
+                                             int heads,
+                                             int rotary_dim,
+                                             bool rotate_half,
+                                             bool rotate_every_two,
+                                             cudaStream_t stream,
+                                             int trans_count,
+                                             int max_out_tokens);
+#endif
+
+template void launch_bias_add_transform_0213(__half* output,
+                                             __half* k_cache,
+                                             __half* v_cache,
+                                             const __half* vals,
+                                             const __half* bias,
+                                             int batch_size,
+                                             int seq_length,
+                                             unsigned seq_offset,
+                                             int all_tokens,
+                                             int hidden_dim,
+                                             int heads,
+                                             int rotary_dim,
+                                             bool rotate_half,
+                                             bool rotate_every_two,
+                                             cudaStream_t stream,
+                                             int trans_count,
+                                             int max_out_tokens);
+
 // Bias add
 
 __global__ void pad_add_transform_0213(float* output,
                                        const float* vals,
                                        int hidden_dim,
                                        int seq_length,
                                        int padded_seq_len,
                                        int heads,
                                        int padded_head_size)
 {
 }
 
-__global__ void pad_add_transform_0213(__half* output,
-                                       const __half* vals,
+template <typename T>
+__global__ void pad_add_transform_0213(T* output,
+                                       const T* vals,
                                        int hidden_dim,
                                        int seq_length,
                                        int padded_seq_len,
                                        int heads,
                                        int padded_head_size)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4 ZERO;
-    const __half2 zero_h = __float2half2_rn(0.f);
-    __half2* ZERO_h = reinterpret_cast<__half2*>(&ZERO);
+    const T2 zero_h = conversion::to<T2>(0.f);
+    T2* ZERO_h = reinterpret_cast<T2*>(&ZERO);
 #pragma unroll
     for (int i = 0; i < 4; i++) ZERO_h[i] = zero_h;
 
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
@@ -297,56 +332,68 @@
 
     if (d3 < d2_stride && d1 < seq_length)
         output_vec[d3] = vals_vec[d3];
     else
         output_vec[d3] = ZERO;
 }
 
-template <typename T>
-void launch_pad_add_transform_0213(T* output,
-                                   const T* vals,
-                                   int batch_size,
-                                   int hidden_dim,
-                                   int seq_length,
-                                   int padded_seq_len,
-                                   int heads,
-                                   int padded_head_size,
-                                   cudaStream_t stream);
-
 // [B S C*H] - > C * [B A S N]
 template <>
 void launch_pad_add_transform_0213<float>(float* output,
                                           const float* vals,
                                           int batch_size,
                                           int hidden_dim,
                                           int seq_length,
                                           int padded_seq_len,
                                           int heads,
                                           int padded_head_size,
                                           cudaStream_t stream)
 {
 }
-template <>
-void launch_pad_add_transform_0213<__half>(__half* output,
-                                           const __half* vals,
-                                           int batch_size,
-                                           int hidden_dim,
-                                           int seq_length,
-                                           int padded_seq_len,
-                                           int heads,
-                                           int padded_head_size,
-                                           cudaStream_t stream)
+
+template <typename T>
+void launch_pad_add_transform_0213(T* output,
+                                   const T* vals,
+                                   int batch_size,
+                                   int hidden_dim,
+                                   int seq_length,
+                                   int padded_seq_len,
+                                   int heads,
+                                   int padded_head_size,
+                                   cudaStream_t stream)
 {
     hidden_dim >>= 3;
     dim3 block_dim((padded_head_size >> 3), heads, 2);
     dim3 grid_dim(batch_size, padded_seq_len / 2);
     pad_add_transform_0213<<<grid_dim, block_dim, 0, stream>>>(
         output, vals, hidden_dim, seq_length, padded_seq_len, heads, padded_head_size >> 3);
 }
 
+#ifdef BF16_AVAILABLE
+template void launch_pad_add_transform_0213(__nv_bfloat16* output,
+                                            const __nv_bfloat16* vals,
+                                            int batch_size,
+                                            int hidden_dim,
+                                            int seq_length,
+                                            int padded_seq_len,
+                                            int heads,
+                                            int padded_head_size,
+                                            cudaStream_t stream);
+#endif
+
+template void launch_pad_add_transform_0213(__half* output,
+                                            const __half* vals,
+                                            int batch_size,
+                                            int hidden_dim,
+                                            int seq_length,
+                                            int padded_seq_len,
+                                            int heads,
+                                            int padded_head_size,
+                                            cudaStream_t stream);
+
 // Bias add
 template <typename T>
 __global__ void bias_add_transform_0213(T* output,
                                         const T* vals,
                                         const T* bias,
                                         int hidden_dim,
                                         int seq_length,
@@ -390,23 +437,25 @@
     outputs.z = inputs.z + biases.z;
     outputs.w = inputs.w + biases.w;
 
     output_vec[cnt * d0_out_stride * gridDim.x + d0 * d0_out_stride + d1 * d1_out_stride +
                d2 * d2_out_stride + d3] = outputs;
 }
 
-template <>
-__global__ void bias_add_transform_0213<__half>(__half* output,
-                                                const __half* vals,
-                                                const __half* bias,
-                                                int hidden_dim,
-                                                int seq_length,
-                                                int heads,
-                                                int head_ext)
+template <typename T>
+__global__ void bias_add_transform_0213(T* output,
+                                        const T* vals,
+                                        const T* bias,
+                                        int hidden_dim,
+                                        int seq_length,
+                                        int heads,
+                                        int head_ext)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
     int d2_out_stride = d2_stride * seq_length;
 
     int d0 = blockIdx.x;                                                  // Batch
@@ -414,17 +463,17 @@
     int cnt = blockIdx.z / head_ext;                                      // Hidden count
     int d2 = threadIdx.y + (blockIdx.z % head_ext) * (heads / head_ext);  // Head (0-11)
     int d3 = threadIdx.x;                                                 // Values (groups of 4)
 
     float4 vals_arr;
     float4 bias_arr;
     float4 output_arr;
-    __half2* vals_half = reinterpret_cast<__half2*>(&vals_arr);
-    __half2* bias_half = reinterpret_cast<__half2*>(&bias_arr);
-    __half2* output_half = reinterpret_cast<__half2*>(&output_arr);
+    T2* vals_half = reinterpret_cast<T2*>(&vals_arr);
+    T2* bias_half = reinterpret_cast<T2*>(&bias_arr);
+    T2* output_half = reinterpret_cast<T2*>(&output_arr);
 
     const float4* vals_vec = reinterpret_cast<const float4*>(vals);
     const float4* bias_vec = reinterpret_cast<const float4*>(bias);
     float4* output_vec = reinterpret_cast<float4*>(output);
 
     vals_vec += (d0 * d0_stride * (gridDim.z / head_ext));
     vals_vec += (d1 * d1_stride * (gridDim.z / head_ext));
@@ -445,21 +494,24 @@
     output_half[0] = vals_half[0] + bias_half[0];
     output_half[1] = vals_half[1] + bias_half[1];
     output_half[2] = vals_half[2] + bias_half[2];
     output_half[3] = vals_half[3] + bias_half[3];
     output_vec[d3] = output_arr;
 }
 
-__global__ void bias_add_transform_0213_v2(__half* output,
-                                           const __half* vals,
-                                           const __half* bias,
+template <typename T>
+__global__ void bias_add_transform_0213_v2(T* output,
+                                           const T* vals,
+                                           const T* bias,
                                            int hidden_dim,
                                            int seq_length,
                                            int heads)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     __shared__ float4 in_data[3072];
 
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
     int iteration_stride = d1_stride * blockDim.z;  // Hidden * 3 / 8
     int batch_stride = d0_stride * blockDim.z;      // Hidden * S * 3 / 8
@@ -473,17 +525,17 @@
     int cnt = threadIdx.z;  // blockIdx.z; // Hidden count
     int d2 = threadIdx.y;   // Head (0-11)
     int d3 = threadIdx.x;   // Values (groups of 4)
 
     float4 vals_arr[1];
     float4 bias_arr[1];
     float4 output_arr[1];
-    __half2* vals_half = reinterpret_cast<__half2*>(vals_arr);
-    __half2* bias_half = reinterpret_cast<__half2*>(bias_arr);
-    __half2* output_half = reinterpret_cast<__half2*>(output_arr);
+    T2* vals_half = reinterpret_cast<T2*>(vals_arr);
+    T2* bias_half = reinterpret_cast<T2*>(bias_arr);
+    T2* output_half = reinterpret_cast<T2*>(output_arr);
 
     const float4* vals_vec = reinterpret_cast<const float4*>(vals);
     const float4* bias_vec = reinterpret_cast<const float4*>(bias);
     float4* output_vec = reinterpret_cast<float4*>(output);
 
     int iter_index = cnt * d1_stride + d2 * d2_stride + d3;
     int input_offset = d0 * batch_stride + d1 * (iteration_stride << 1);
@@ -515,14 +567,30 @@
         int iter_offset =
             (iter_row % blockDim.y) * d2_out_stride + (iter_row / blockDim.y) * matrix_stride;
         output_vec[out_index + iter_offset] =
             in_data[iter_row * d2_stride + d3 + (d2 % 2) * (d1_stride * blockDim.z)];
     }
 }
 
+template __global__ void bias_add_transform_0213_v2(__half* output,
+                                                    const __half* vals,
+                                                    const __half* bias,
+                                                    int hidden_dim,
+                                                    int seq_length,
+                                                    int heads);
+
+#ifdef BF16_AVAILABLE
+template __global__ void bias_add_transform_0213_v2(__nv_bfloat16* output,
+                                                    const __nv_bfloat16* vals,
+                                                    const __nv_bfloat16* bias,
+                                                    int hidden_dim,
+                                                    int seq_length,
+                                                    int heads);
+#endif
+
 template <typename T>
 __global__ void transform4d_0213(T* out,
                                  const T* in,
                                  int heads,
                                  int seq_length,
                                  int hidden_dim,
                                  int head_ext);
@@ -556,21 +624,21 @@
         float4 vals_vec = in_vec[cnt * d0_stride * gridDim.x + d0 * d0_stride + d1 * d1_stride +
                                  d2 * d2_stride + d3];
         out_vec[d0 * d0_out_stride * gridDim.z + cnt * d2_out_stride + d1 * d1_out_stride +
                 d2 * d2_out_stride * gridDim.z + d3] = vals_vec;
     }
 }
 
-template <>
-__global__ void transform4d_0213<__half>(__half* out,
-                                         const __half* in,
-                                         int heads,
-                                         int seq_length,
-                                         int hidden_dim,
-                                         int head_ext)
+template <typename T>
+__global__ void transform4d_0213(T* out,
+                                 const T* in,
+                                 int heads,
+                                 int seq_length,
+                                 int hidden_dim,
+                                 int head_ext)
 {
     int d0_stride = hidden_dim * (seq_length / head_ext);
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
     int d0 = blockIdx.x;                                                  // Batch
     int d1 = threadIdx.y + (blockIdx.z % head_ext) * (heads / head_ext);  // Head
@@ -590,19 +658,16 @@
     out_vec += (d1 * d2_stride);
     out_vec += (d0 * d0_stride * gridDim.y);
     out_vec += (d2 * d1_stride * gridDim.y);
 
     out_vec[d3] = in_vec[d3];
 }
 
-__global__ void transform4d_0213_v2(__half* out,
-                                    const __half* in,
-                                    int heads,
-                                    int seq_length,
-                                    int hidden_dim)
+template <typename T>
+__global__ void transform4d_0213_v2(T* out, const T* in, int heads, int seq_length, int hidden_dim)
 {
     __shared__ float4 in_data[3072];
 
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
@@ -638,14 +703,28 @@
 #pragma unroll
     for (int iter = 0; iter < 2; iter++) {
         int iter_id = iter * iteration_stride + iter_index;
         out_vec[output_offset + iter_id] = in_data[iter_id];
     }
 }
 
+#ifdef BF16_AVAILABLE
+template __global__ void transform4d_0213_v2(__nv_bfloat16* out,
+                                             const __nv_bfloat16* in,
+                                             int heads,
+                                             int seq_length,
+                                             int hidden_dim);
+#endif
+
+template __global__ void transform4d_0213_v2(__half* out,
+                                             const __half* in,
+                                             int heads,
+                                             int seq_length,
+                                             int hidden_dim);
+
 // 3 * [B A S N] - > [B S C*H]
 template <>
 void launch_transform4d_0213<float>(float* out,
                                     const float* in,
                                     int batch_size,
                                     int heads,
                                     int seq_length,
@@ -656,24 +735,44 @@
     hidden_dim >>= 2;
     dim3 grid_dims(batch_size, heads * ((seq_length - 1) / 8 + 1), trans_count);
     dim3 block_dims(hidden_dim / heads, 8);
     transform4d_0213<float>
         <<<grid_dims, block_dims, 0, stream>>>(out, in, heads, seq_length, hidden_dim, 1);
 }
 
-template <>
-void launch_transform4d_0213<__half>(__half* out,
-                                     const __half* in,
-                                     int batch_size,
-                                     int heads,
-                                     int seq_length,
-                                     int hidden_dim,
-                                     cudaStream_t stream,
-                                     int trans_count)
+template <typename T>
+void launch_transform4d_0213<T>(T* out,
+                                const T* in,
+                                int batch_size,
+                                int heads,
+                                int seq_length,
+                                int hidden_dim,
+                                cudaStream_t stream,
+                                int trans_count)
 {
     hidden_dim >>= 3;
     int head_ext = (hidden_dim - 1) / MAX_THREADS + 1;
     dim3 grid_dims(batch_size, trans_count, (seq_length * head_ext));
     dim3 block_dims(hidden_dim / heads, (heads / head_ext));
-    transform4d_0213<__half>
-        <<<grid_dims, block_dims, 0, stream>>>(out, in, heads, seq_length, hidden_dim, head_ext);
+    transform4d_0213<<<grid_dims, block_dims, 0, stream>>>(
+        out, in, heads, seq_length, hidden_dim, head_ext);
 }
+
+#ifdef BF16_AVAILABLE
+template void launch_transform4d_0213(__nv_bfloat16* out,
+                                      const __nv_bfloat16* in,
+                                      int batch_size,
+                                      int heads,
+                                      int seq_length,
+                                      int hidden_dim,
+                                      cudaStream_t stream,
+                                      int trans_count);
+#endif
+
+template void launch_transform4d_0213(__half* out,
+                                      const __half* in,
+                                      int batch_size,
+                                      int heads,
+                                      int seq_length,
+                                      int hidden_dim,
+                                      cudaStream_t stream,
+                                      int trans_count);
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.2/csrc/transformer/inference/includes/inference_context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/cublas_wrappers.cu`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 // Copyright (c) Microsoft Corporation.
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
-#pragma once
-
-#include <assert.h>
-#include <cublas_v2.h>
-#include <cuda.h>
-#include <cuda_fp16.h>
-#include <cuda_runtime.h>
-#ifndef __HIP_PLATFORM_HCC__
-#include <mma.h>
-#endif
-#include <stdio.h>
+#include "cublas_wrappers.h"
 
 #ifdef __HIP_PLATFORM_HCC__
 int cublas_gemm_ex(rocblas_handle handle,
                    rocblas_operation transa,
                    rocblas_operation transb,
                    int m,
                    int n,
```

### Comparing `deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 // DeepSpeed Team
 
 #pragma once
 
 #include "ds_kernel_utils.h"
 
 #include <cuda.h>
+#ifdef BF16_AVAILABLE
+#include <cuda_bf16.h>
+#endif
 #include <cuda_fp16.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <cassert>
 #include <iostream>
 
 #define MAX_WARP_NUM 32
```

### Comparing `deepspeed-0.9.1/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.2/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.2/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.2/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.2/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/__init__.py` & `deepspeed-0.9.2/deepspeed/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/accelerator/abstract_accelerator.py` & `deepspeed-0.9.2/deepspeed/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/accelerator/cuda_accelerator.py` & `deepspeed-0.9.2/deepspeed/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/accelerator/real_accelerator.py` & `deepspeed-0.9.2/deepspeed/accelerator/real_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/autotuner.py` & `deepspeed-0.9.2/deepspeed/autotuning/autotuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/config.py` & `deepspeed-0.9.2/deepspeed/autotuning/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/constants.py` & `deepspeed-0.9.2/deepspeed/autotuning/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/scheduler.py` & `deepspeed-0.9.2/deepspeed/autotuning/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/tuner/base_tuner.py` & `deepspeed-0.9.2/deepspeed/autotuning/tuner/base_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/tuner/cost_model.py` & `deepspeed-0.9.2/deepspeed/autotuning/tuner/cost_model.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/tuner/index_based_tuner.py` & `deepspeed-0.9.2/deepspeed/autotuning/tuner/index_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/tuner/model_based_tuner.py` & `deepspeed-0.9.2/deepspeed/autotuning/tuner/model_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/tuner/utils.py` & `deepspeed-0.9.2/deepspeed/autotuning/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/autotuning/utils.py` & `deepspeed-0.9.2/deepspeed/autotuning/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/__init__.py` & `deepspeed-0.9.2/deepspeed/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/constants.py` & `deepspeed-0.9.2/deepspeed/checkpoint/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/deepspeed_checkpoint.py` & `deepspeed-0.9.2/deepspeed/checkpoint/deepspeed_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/reshape_3d_utils.py` & `deepspeed-0.9.2/deepspeed/checkpoint/reshape_3d_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/reshape_meg_2d.py` & `deepspeed-0.9.2/deepspeed/checkpoint/reshape_meg_2d.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/reshape_utils.py` & `deepspeed-0.9.2/deepspeed/checkpoint/reshape_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/universal_checkpoint.py` & `deepspeed-0.9.2/deepspeed/checkpoint/universal_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/utils.py` & `deepspeed-0.9.2/deepspeed/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/checkpoint/zero_checkpoint.py` & `deepspeed-0.9.2/deepspeed/checkpoint/zero_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/comm/backend.py` & `deepspeed-0.9.2/deepspeed/comm/backend.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/comm/comm.py` & `deepspeed-0.9.2/deepspeed/comm/comm.py`

 * *Files 3% similar despite different names*

```diff
@@ -436,14 +436,38 @@
                    prof=False,
                    log_name='reduce_scatter',
                    debug=get_caller_func()):
     global cdb
     return cdb.reduce_scatter(output=output, input_list=input_list, op=op, group=group, async_op=async_op)
 
 
+def has_all_reduce_coalesced():
+    """"""
+    global cdb
+    assert cdb is not None and cdb.is_initialized(
+    ), 'DeepSpeed backend not set, please initialize it using init_process_group()'
+    assert cdb.has_all_reduce_coalesced is not None, 'has_all_reduce_coalesced is not yet defined'
+    return cdb.has_all_reduce_coalesced
+
+
+def has_coalescing_manager():
+    global cdb
+    assert cdb is not None and cdb.is_initialized(
+    ), 'DeepSpeed backend not set, please initialize it using init_process_group()'
+    assert cdb.has_coalescing_manager is not None, 'has_coalescing_manager is not yet defined'
+    return cdb.has_coalescing_manager
+
+
+def all_gather_coalesced(output_tensors, input_tensors, group=None, async_op=False):
+    global cdb
+    assert cdb is not None and cdb.is_initialized(
+    ), 'DeepSpeed backend not set, please initialize it using init_process_group()'
+    return cdb.all_gather_coalesced(output_tensors, input_tensors, group=group, async_op=async_op)
+
+
 @timed_op
 def all_reduce(tensor,
                op=ReduceOp.SUM,
                group=None,
                async_op=False,
                prof=False,
                log_name='all_reduce',
@@ -453,14 +477,26 @@
     # timers.start()
     # TensorBoard logging for comm calls.?
     global cdb
     #print(f'op = {op}, cdb= {cdb.name}')
     return cdb.all_reduce(tensor, op, group, async_op)
 
 
+@timed_op
+def all_reduce_coalesced(tensors,
+                         op=ReduceOp.SUM,
+                         group=None,
+                         async_op=False,
+                         prof=False,
+                         log_name='all_reduce',
+                         debug=get_caller_func()):
+    global cbd
+    return cdb.all_reduce_coalesced(tensors, op, group, async_op)
+
+
 def get_world_group():
     global cdb
     assert cdb is not None and cdb.is_initialized(
     ), 'DeepSpeed backend not set, please initialize it using init_process_group()'
     return cdb.get_world_group()
```

### Comparing `deepspeed-0.9.1/deepspeed/comm/config.py` & `deepspeed-0.9.2/deepspeed/comm/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/comm/constants.py` & `deepspeed-0.9.2/deepspeed/comm/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/comm/torch.py` & `deepspeed-0.9.2/deepspeed/comm/torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,54 @@
 
 from deepspeed import utils
 
 from .utils import *
 from .backend import *
 from .comm import *
 
+import torch
+
+
+def is_torch_two():
+    TORCH_MAJOR = int(torch.__version__.split('.')[0])
+    if TORCH_MAJOR >= 2:
+        return True
+    else:
+        return False
+
+
+def has_coalescing_manager():
+    has_c10d = hasattr(torch.distributed, 'distributed_c10d')
+    return has_c10d and hasattr(torch.distributed.distributed_c10d, '_coalescing_manager')
+
+
+def has_all_reduce_coalesced():
+    return hasattr(torch.distributed, "all_reduce_coalesced")
+
+
+def get_coalescing_manager(group, device, reqs):
+    if is_torch_two():
+        return torch.distributed.distributed_c10d._coalescing_manager(group, device=device, reqs=reqs)
+    else:
+        return torch.distributed.distributed_c10d._coalescing_manager(group, reqs)
+
 
 class TorchBackend(Backend):
     """
         A light-weight wrapper class for torch.distributed API.
         Only a subset of functions are wrapped. Once the init_process_group
         is initialized, standard torch.distributed.* can be used directly
         so no need to wrap all the functions. We can keep adding wrappers as
         needed.
     """
 
     def __init__(self, backend, timeout, init_method, rank=-1, world_size=-1, name='torch'):
         super(TorchBackend, self).__init__()
+        self.has_all_reduce_coalesced = has_all_reduce_coalesced()
+        self.has_coalescing_manager = has_coalescing_manager()
         self.all_gather_function = self.get_all_gather_function()
         self.reduce_scatter_function = self.get_reduce_scatter_function()
         self.initialized = True
         self.name = name
         # Future functionality to support ds.initialize() on a single GPU
         # The idea is to fake that dist backend is initialized even when
         # it is not so we can run on a single GPU without doing any init_process_group
@@ -62,14 +90,24 @@
                                                  world_size=world_size)
         self.using_mpi = torch.distributed.get_backend() == 'mpi'
 
     def all_reduce(self, tensor, op=torch.distributed.ReduceOp.SUM, group=None, async_op=False):
         op = self._reduce_op(op)
         return torch.distributed.all_reduce(tensor=tensor, op=op, group=group, async_op=async_op)
 
+    def all_reduce_coalesced(self, tensors, op=torch.distributed.ReduceOp.SUM, group=None, async_op=False):
+        """ proxy func to torch.distributed.all_reduce_coalesced,
+        which is included in PyTorch 1.13 and above
+        """
+        if not self.has_all_reduce_coalesced:
+            raise RuntimeError(f"Current torch version does not have all_reduce_coalesced "
+                               f"api (torch.__version__: {torch.__version__})")
+        op = self._reduce_op(op)
+        return torch.distributed.all_reduce_coalesced(tensors=tensors, op=op, group=group, async_op=async_op)
+
     def reduce(self, tensor, dst, op=ReduceOp.SUM, group=None, async_op=False):
         return torch.distributed.reduce(tensor=tensor, dst=dst, op=self._reduce_op(op), group=group, async_op=async_op)
 
     def reduce_scatter(self, output, input_list, op=ReduceOp.SUM, group=None, async_op=False):
         return torch.distributed.reduce_scatter(output=output,
                                                 input_list=input_list,
                                                 op=self._reduce_op(op),
@@ -85,19 +123,42 @@
     def all_gather_into_tensor(self, output_tensor, input_tensor, group=None, async_op=False):
         if self.has_all_gather_into_tensor():
             return self.all_gather_function(output_tensor=output_tensor,
                                             input_tensor=input_tensor,
                                             group=group,
                                             async_op=async_op)
         else:
-            utils.logger.warning("unable to find torch.distributed.all_gather_into_tensor. will fall back to "
+            utils.logger.warning("unable to find torch.distributed._all_gather_base. will fall back to "
                                  "torch.distributed.all_gather which will result in suboptimal performance. "
                                  "please consider upgrading your pytorch installation.")
             pass
 
+    def all_gather_coalesced(self, output_tensors, input_tensors, group=None, async_op=False):
+        """"""
+        assert len(output_tensors) == len(input_tensors), ""
+        if hasattr(torch.distributed.distributed_c10d, '_all_gather_base_coalesced'):
+            # customized PyTorch
+            return torch.distributed.distributed_c10d._all_gather_base_coalesced(output_tensors,
+                                                                                 input_tensors,
+                                                                                 group=group,
+                                                                                 async_op=async_op)
+        elif has_coalescing_manager():
+            reqs = []
+            with get_coalescing_manager(group, input_tensors[0].device, reqs):
+                for output, input in zip(output_tensors, input_tensors):
+                    handle = torch.distributed.distributed_c10d.all_gather_into_tensor(output,
+                                                                                       input,
+                                                                                       group=group,
+                                                                                       async_op=True)
+                    reqs.append(handle)
+            if async_op:
+                return reqs[-1]
+            else:
+                reqs[-1].wait()
+
     def reduce_scatter_tensor(self, output_tensor, input_tensor, op=ReduceOp.SUM, group=None, async_op=False):
         if self.has_reduce_scatter_tensor():
             return self.reduce_scatter_function(output_tensor,
                                                 input_tensor,
                                                 op=self._reduce_op(op),
                                                 group=group,
                                                 async_op=async_op)
```

### Comparing `deepspeed-0.9.1/deepspeed/comm/utils.py` & `deepspeed-0.9.2/deepspeed/comm/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/basic_layer.py` & `deepspeed-0.9.2/deepspeed/compression/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/compress.py` & `deepspeed-0.9.2/deepspeed/compression/compress.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/config.py` & `deepspeed-0.9.2/deepspeed/compression/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/constants.py` & `deepspeed-0.9.2/deepspeed/compression/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/helper.py` & `deepspeed-0.9.2/deepspeed/compression/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/scheduler.py` & `deepspeed-0.9.2/deepspeed/compression/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/compression/utils.py` & `deepspeed-0.9.2/deepspeed/compression/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/constants.py` & `deepspeed-0.9.2/deepspeed/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/elasticity/config.py` & `deepspeed-0.9.2/deepspeed/elasticity/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/elasticity/constants.py` & `deepspeed-0.9.2/deepspeed/elasticity/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/elasticity/elastic_agent.py` & `deepspeed-0.9.2/deepspeed/elasticity/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/elasticity/elasticity.py` & `deepspeed-0.9.2/deepspeed/elasticity/elasticity.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/env_report.py` & `deepspeed-0.9.2/deepspeed/env_report.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/git_version_info.py` & `deepspeed-0.9.2/deepspeed/git_version_info.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/git_version_info_installed.py` & `deepspeed-0.9.2/deepspeed/git_version_info_installed.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-version='0.9.1'
+version='0.9.2'
 git_hash='unknown'
 git_branch='unknown'
 installed_ops={'async_io': False, 'cpu_adagrad': False, 'cpu_adam': False, 'fused_adam': False, 'fused_lamb': False, 'quantizer': False, 'random_ltd': False, 'sparse_attn': False, 'spatial_inference': False, 'transformer': False, 'stochastic_transformer': False, 'transformer_inference': False, 'utils': False}
 compatible_ops={'async_io': False, 'cpu_adagrad': True, 'cpu_adam': True, 'fused_adam': True, 'fused_lamb': True, 'quantizer': True, 'random_ltd': True, 'sparse_attn': False, 'spatial_inference': True, 'transformer': True, 'stochastic_transformer': True, 'transformer_inference': True, 'utils': True}
 torch_info={'version': '1.9', 'bf16_support': False, 'cuda_version': '10.2', 'nccl_version': '2.7', 'hip_version': '0.0'}
```

### Comparing `deepspeed-0.9.1/deepspeed/inference/config.py` & `deepspeed-0.9.2/deepspeed/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/inference/engine.py` & `deepspeed-0.9.2/deepspeed/inference/engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/launcher/launch.py` & `deepspeed-0.9.2/deepspeed/launcher/launch.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/launcher/multinode_runner.py` & `deepspeed-0.9.2/deepspeed/launcher/multinode_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,33 +180,42 @@
         if self.args.num_nodes != -1 or self.args.num_gpus != -1:
             raise ValueError(f"{self.name} backend does not support limiting num nodes/gpus")
 
     def get_cmd(self, environment, active_resources):
         devices_per_node = self.resource_pool.values()
         total_process_count = sum(devices_per_node)
         process_per_node = list(devices_per_node)[0]
+        hosts = ""
+
+        for i, host in enumerate(self.resource_pool.keys()):
+            if i == 0:
+                hosts = f"{host}"
+            else:
+                hosts += f",{host}"
 
         mpirun_cmd = [
             'mpirun',
             '-n',
             f'{total_process_count}',
             '-ppn',
             f'{process_per_node}',
+            '-hosts',
+            f'{hosts}',
         ] + split(self.args.launcher_args)
         export_cmd = []
 
         for k, v in self.exports.items():
-            export_cmd += ['-x', "{}={}".format(k, v)]
+            export_cmd += ['-genv', "{}={}".format(k, v)]
 
         python_exec = []
         if not self.args.no_python:
             python_exec = [sys.executable, "-u"]
             if self.args.module:
                 python_exec.append("-m")
-        return mpirun_cmd + python_exec + [self.user_script] + self.user_arguments
+        return mpirun_cmd + export_cmd + python_exec + [self.user_script] + self.user_arguments
 
 
 class SlurmRunner(MultiNodeRunner):
 
     def __init__(self, args, world_info_base64, resource_pool):
         super().__init__(args, world_info_base64)
         self.resource_pool = resource_pool
```

### Comparing `deepspeed-0.9.1/deepspeed/launcher/runner.py` & `deepspeed-0.9.2/deepspeed/launcher/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 DEEPSPEED_ENVIRONMENT_NAME = ".deepspeed_env"
 DEEPSPEED_ENVIRONMENT_PATHS = [os.path.expanduser("~"), '.']
 PDSH_MAX_FAN_OUT = 1024
 
 
 def parse_args(args=None):
     parser = argparse.ArgumentParser(description="DeepSpeed runner to help launch distributed "
-                                     "multi-node/multi-gpu training jobs.")
+                                     "multi-node/multi-gpu training jobs.",
+                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument("-H",
                         "--hostfile",
                         type=str,
                         default=DLTS_HOSTFILE,
                         help="Hostfile path (in MPI style) that defines the "
                         "resource pool available to the job (e.g., "
```

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/diffusers/unet.py` & `deepspeed-0.9.2/deepspeed/model_implementations/diffusers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/diffusers/vae.py` & `deepspeed-0.9.2/deepspeed/model_implementations/diffusers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/features/cuda_graph.py` & `deepspeed-0.9.2/deepspeed/model_implementations/features/cuda_graph.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/clip_encoder.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bert.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bloom.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_gpt.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_megatron_gpt.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_opt.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_transformer.py` & `deepspeed-0.9.2/deepspeed/model_implementations/transformers/ds_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/auto_tp.py` & `deepspeed-0.9.2/deepspeed/module_inject/auto_tp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/__init__.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/base.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,20 +210,30 @@
         self.mlp_inter_mp(mp_replace, reversed_dim=reversed_dim)
         self.mlp_output_mp(mp_replace, reversed_dim=reversed_dim)
 
         # Apply weight quantization
         #self.apply_weight_quantization()
 
     def attention_qkv_mp(self, mp_replace, reversed_dim=False):
-        self.module.attention.attn_qkvw = mp_replace.qkv_copy(self.module.attention.attn_qkvw,
-                                                              self.qkvw,
-                                                              int8=reversed_dim)
-        self.module.attention.attn_qkvb = mp_replace.qkv_copy(self.module.attention.attn_qkvb,
-                                                              self.qkvb,
-                                                              int8=reversed_dim)
+        if reversed_dim:
+            self.module.attention.attn_qkvw = mp_replace.qkv_copy(
+                self.module.attention.attn_qkvw[:self.qkvw.shape[0] // mp_replace.mp_size],
+                self.qkvw,
+                int8=reversed_dim)
+            self.module.attention.attn_qkvb = mp_replace.qkv_copy(
+                self.module.attention.attn_qkvb[:self.qkvw.shape[0] // mp_replace.mp_size],
+                self.qkvb,
+                int8=reversed_dim)
+        else:
+            self.module.attention.attn_qkvw = mp_replace.qkv_copy(self.module.attention.attn_qkvw,
+                                                                  self.qkvw,
+                                                                  int8=reversed_dim)
+            self.module.attention.attn_qkvb = mp_replace.qkv_copy(self.module.attention.attn_qkvb,
+                                                                  self.qkvb,
+                                                                  int8=reversed_dim)
 
     def attention_q_k_v_mp(self, mp_replace, reversed_dim=False):
         self.module.attention.attn_qw = mp_replace.copy(self.module.attention.attn_qw[:self.qw.shape[0] //
                                                                                       mp_replace.mp_size],
                                                         self.qw,
                                                         int8=reversed_dim,
                                                         allocat_tensor=reversed_dim)
@@ -233,29 +243,29 @@
                                                         int8=reversed_dim,
                                                         allocat_tensor=reversed_dim)
         self.module.attention.attn_vw = mp_replace.copy(self.module.attention.attn_vw[:self.qw.shape[0] //
                                                                                       mp_replace.mp_size],
                                                         self.vw,
                                                         int8=reversed_dim,
                                                         allocat_tensor=reversed_dim)
-        self.module.attention.attn_qb = mp_replace.copy(self.module.attention.attn_qb[:self.qw.shape[0] //
-                                                                                      mp_replace.mp_size],
-                                                        self.qb,
-                                                        int8=reversed_dim,
-                                                        allocat_tensor=reversed_dim)
-        self.module.attention.attn_kb = mp_replace.copy(self.module.attention.attn_kb[:self.qw.shape[0] //
-                                                                                      mp_replace.mp_size],
-                                                        self.kb,
-                                                        int8=reversed_dim,
-                                                        allocat_tensor=reversed_dim)
-        self.module.attention.attn_vb = mp_replace.copy(self.module.attention.attn_vb[:self.qw.shape[0] //
-                                                                                      mp_replace.mp_size],
-                                                        self.vb,
-                                                        int8=reversed_dim,
-                                                        allocat_tensor=reversed_dim)
+        self.module.attention.attn_qb = mp_replace.copy(
+            self.module.attention.attn_qb[:self.qw.shape[0] // mp_replace.mp_size],
+            self.qb,
+            int8=reversed_dim,
+            allocat_tensor=reversed_dim) if self.module.attention.attn_qb is not None else None
+        self.module.attention.attn_kb = mp_replace.copy(
+            self.module.attention.attn_kb[:self.qw.shape[0] // mp_replace.mp_size],
+            self.kb,
+            int8=reversed_dim,
+            allocat_tensor=reversed_dim) if self.module.attention.attn_kb is not None else None
+        self.module.attention.attn_vb = mp_replace.copy(
+            self.module.attention.attn_vb[:self.qw.shape[0] // mp_replace.mp_size],
+            self.vb,
+            int8=reversed_dim,
+            allocat_tensor=reversed_dim) if self.module.attention.attn_vb is not None else None
 
     def attention_o_mp(self, mp_replace, reversed_dim=False):
         if reversed_dim:
             self.module.attention.attn_ow = mp_replace.copy(self.module.attention.attn_ow[:, :self.dense_w.shape[1] //
                                                                                           mp_replace.mp_size],
                                                             self.dense_w,
                                                             int8=reversed_dim,
@@ -272,19 +282,19 @@
     def mlp_inter_mp(self, mp_replace, reversed_dim=False):
         if reversed_dim:
             self.module.mlp.inter_w = mp_replace.copy(self.module.mlp.inter_w[:self._h4h_w.shape[0] //
                                                                               mp_replace.mp_size],
                                                       self._h4h_w,
                                                       int8=reversed_dim,
                                                       allocat_tensor=reversed_dim)
-            self.module.mlp.inter_b = mp_replace.copy(self.module.mlp.inter_b[:self._h4h_w.shape[0] //
-                                                                              mp_replace.mp_size],
-                                                      self._h4h_b,
-                                                      int8=reversed_dim,
-                                                      allocat_tensor=reversed_dim)
+            self.module.mlp.inter_b = mp_replace.copy(
+                self.module.mlp.inter_b[:self._h4h_w.shape[0] // mp_replace.mp_size],
+                self._h4h_b,
+                int8=reversed_dim,
+                allocat_tensor=reversed_dim) if self.module.mlp.inter_b is not None else None
         else:
             self.module.mlp.inter_w = mp_replace.copy(self.module.mlp.inter_w, self._h4h_w, int8=reversed_dim)
             self.module.mlp.inter_b = mp_replace.copy(self.module.mlp.inter_b, self._h4h_b, int8=reversed_dim)
 
     def mlp_output_mp(self, mp_replace, reversed_dim=False):
         if reversed_dim:
             self.module.mlp.output_w = mp_replace.copy(self.module.mlp.output_w[:, :self._4hh_w.shape[1] //
@@ -298,32 +308,32 @@
                                                    self._4hh_b,
                                                    int8=reversed_dim,
                                                    allocat_tensor=reversed_dim)
 
     def release_qkv(self):
         del self.module.attention.attn_qkvw
         del self.module.attention.attn_qkvb
-        self.module.attention.attn_qkvw = None
-        self.module.attention.attn_qkvb = None
-
-        qkv_data = [self.module.attention.attn_qw.data, \
-                    self.module.attention.attn_qb.data, \
-                    self.module.attention.attn_kw.data, \
-                    self.module.attention.attn_kb.data, \
-                    self.module.attention.attn_vw.data, \
-                    self.module.attention.attn_vb.data]
-        for data in qkv_data:
-            del data
-
-        self.module.attention.attn_qw = self.qw
-        self.module.attention.attn_qb = self.qb
-        self.module.attention.attn_kw = self.kw
-        self.module.attention.attn_kb = self.kb
-        self.module.attention.attn_vw = self.vw
-        self.module.attention.attn_vb = self.vb
+        self.module.attention.attn_qkvw = self.qkvw
+        self.module.attention.attn_qkvb = self.qkvb
+        if self.module.attention.attn_qw is not None:
+            qkv_data = [self.module.attention.attn_qw.data, \
+                        self.module.attention.attn_qb.data if self.module.attention.attn_qb is not None else None, \
+                        self.module.attention.attn_kw.data, \
+                        self.module.attention.attn_kb.data if self.module.attention.attn_kb is not None else None, \
+                        self.module.attention.attn_vw.data, \
+                        self.module.attention.attn_vb.data if self.module.attention.attn_vb is not None else None]
+            for data in qkv_data:
+                del data
+
+            self.module.attention.attn_qw = self.qw
+            self.module.attention.attn_qb = self.qb
+            self.module.attention.attn_kw = self.kw
+            self.module.attention.attn_kb = self.kb
+            self.module.attention.attn_vw = self.vw
+            self.module.attention.attn_vb = self.vb
 
     def release_memory(self):
         self.release_qkv()
         del self.module.attention.attn_ow
         del self.module.attention.attn_ob
         self.module.attention.attn_ow = self.dense_w
         self.module.attention.attn_ob = self.dense_b
@@ -343,14 +353,22 @@
         else:
             self.module.mlp.attn_nw.data.copy_(self.attn_nw.to(get_accelerator().current_device_name()))
             self.module.mlp.attn_nb.data.copy_(self.attn_nb.to(get_accelerator().current_device_name()))
 
         self.module.norm_w.data.copy_(self.input_nw.to(get_accelerator().current_device_name()))
         self.module.norm_b.data.copy_(self.input_nb.to(get_accelerator().current_device_name()))
 
+    def align_merged_qkv(self):
+        if hasattr(self, '_align_merged_qkv'):
+            self._align_merged_qkv()
+
+    def partition_merged_qkv(self):
+        if hasattr(self, '_partition_merged_qkv'):
+            self._partition_merged_qkv()
+
     def transpose(self):
         self.transpose_attention()
         self.transpose_mlp()
 
     def transpose_attention(self):
         if self.attn_linear_layer:
             self.qkvw = self.transpose_impl(self.qkvw.data)
@@ -399,33 +417,36 @@
         self.vb.data = self.module.attention.attn_qkvb.data[2 * self.qw.shape[0]:]
 
         for data in qkv_data:
             del data
 
     def reset_qkv(self):
         self.qkvw.data[:self.qw.shape[0]] = self.qw.data
-        self.qkvb.data[:self.qw.shape[0]] = self.qb.data
         self.qkvw.data[self.qw.shape[0]:2 * self.qw.shape[0]] = self.kw.data
-        self.qkvb.data[self.qw.shape[0]:2 * self.qw.shape[0]] = self.kb.data
         self.qkvw.data[2 * self.qw.shape[0]:] = self.vw.data
-        self.qkvb.data[2 * self.qw.shape[0]:] = self.vb.data
+        if self.qkvb is not None:
+            self.qkvb.data[:self.qw.shape[0]] = self.qb.data
+            self.qkvb.data[self.qw.shape[0]:2 * self.qw.shape[0]] = self.kb.data
+            self.qkvb.data[2 * self.qw.shape[0]:] = self.vb.data
 
         qkv_data = [self.qw.data, \
-                    self.qb.data, \
+                    self.qb.data if self.qb is not None else None, \
                     self.kw.data, \
-                    self.kb.data, \
+                    self.kb.data if self.kb is not None else None, \
                     self.vw.data, \
-                    self.vb.data]
+                    self.vb.data if self.vb is not None else None]
 
         self.qw.data = self.qkvw.data[:self.qw.shape[0]]
-        self.qb.data = self.qkvb.data[:self.qw.shape[0]]
         self.kw.data = self.qkvw.data[self.qw.shape[0]:2 * self.qw.shape[0]]
-        self.kb.data = self.qkvb.data[self.qw.shape[0]:2 * self.qw.shape[0]]
         self.vw.data = self.qkvw.data[2 * self.qw.shape[0]:]
-        self.vb.data = self.qkvb.data[2 * self.qw.shape[0]:]
+
+        if self.qkvb is not None:
+            self.qb.data = self.qkvb.data[:self.qw.shape[0]]
+            self.kb.data = self.qkvb.data[self.qw.shape[0]:2 * self.qw.shape[0]]
+            self.vb.data = self.qkvb.data[2 * self.qw.shape[0]:]
 
         for data in qkv_data:
             del data
 
     def set_params_wo_copy(self, Z3_enabled=False):
         self.module.mlp.attn_nw = self.attn_nw
         self.module.mlp.attn_nb = self.attn_nb
@@ -446,19 +467,20 @@
                 self.module.attention.attn_qb = self.qb
                 self.module.attention.attn_kw = self.kw
                 self.module.attention.attn_kb = self.kb
                 self.module.attention.attn_vw = self.vw
                 self.module.attention.attn_vb = self.vb
             else:
                 self.qw.data = self.qkvw[:self.qw.shape[0], :]
-                self.qb.data = self.qkvb[:self.qw.shape[0]]
                 self.kw.data = self.qkvw[self.qw.shape[0]:2 * self.qw.shape[0], :]
-                self.kb.data = self.qkvb[self.qw.shape[0]:2 * self.qw.shape[0]]
                 self.vw.data = self.qkvw[self.qw.shape[0] * 2:, :]
-                self.vb.data = self.qkvb[self.qw.shape[0] * 2:]
+                if self.qkvb is not None:
+                    self.qb.data = self.qkvb[:self.qw.shape[0]]
+                    self.kb.data = self.qkvb[self.qw.shape[0]:2 * self.qw.shape[0]]
+                    self.vb.data = self.qkvb[self.qw.shape[0] * 2:]
 
     def get_lora_params(self):
         return self.lora_params
 
     def get_all_params(self):
         if self.q_k_v is not None:
             return [
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/base_moe.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/base_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/bert.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/bloom.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/bloom.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from .base import *
 from .features.meta_tensor import MetaTensorContainer
 from deepspeed.model_implementations.transformers.ds_bloom import DeepSpeedBloomInference
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 
+from ..policy import maybe_get_lora
+
 supported_models = {None}
 
 
 class DS_BloomContainer(MetaTensorContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -105,8 +107,16 @@
     def layernorm(self):
         return self.client_module.post_attention_layernorm.weight, \
                self.client_module.post_attention_layernorm.bias, \
                self.client_module.input_layernorm.weight, \
                self.client_module.input_layernorm.bias
 
     def get_lora_params(self):
-        return []
+        all_lora_params = []
+        for p in [
+            self.client_module.mlp.dense_h_to_4h, \
+            self.client_module.mlp.dense_4h_to_h, \
+            self.client_module.self_attention.query_key_value, \
+            self.client_module.self_attention.dense
+            ]:
+            all_lora_params.append(maybe_get_lora(p))
+        return all_lora_params
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/clip.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/clip.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/distil_bert.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/distil_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/features/meta_tensor.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/features/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/gpt2.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/gpt2.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/gptj.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/gptj.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import torch
 from torch.nn.parameter import Parameter
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 from ..policy import maybe_copy_qkv
 
+from ..policy import maybe_get_lora
+
 
 class DS_GPTJContainer(MetaTensorContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
@@ -66,20 +68,25 @@
         try:
             import transformers
             HFGPTJLayerPolicy._orig_layer_class = transformers.models.gptj.modeling_gptj.GPTJBlock
         except:
             HFGPTJLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
-        return self.client_module.attn.q_proj.weight.shape[1], \
+        return self.client_module.attn.embed_dim, \
                 self.client_module.attn.num_attention_heads, \
                 self.client_module.ln_1.eps
 
     def get_q_k_v(self):
-        return None
+        return self.client_module.attn.q_proj.weight, \
+               None, \
+               self.client_module.attn.k_proj.weight, \
+               None, \
+               self.client_module.attn.v_proj.weight, \
+               None
 
     def attention(self, enable_training=False):
         qw = self.client_module.attn.q_proj.weight
         kw = self.client_module.attn.k_proj.weight
         vw = self.client_module.attn.v_proj.weight
 
         qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=enable_training)
@@ -98,8 +105,18 @@
     def layernorm(self):
         return None, \
                None, \
                self.client_module.ln_1.weight, \
                self.client_module.ln_1.bias
 
     def get_lora_params(self):
-        return []
+        all_lora_params = []
+        for p in [
+            self.client_module.mlp.fc_in, \
+            self.client_module.mlp.fc_out, \
+            self.client_module.attn.q_proj, \
+            self.client_module.attn.k_proj, \
+            self.client_module.attn.v_proj, \
+            self.client_module.attn.out_proj, \
+            ]:
+            all_lora_params.append(maybe_get_lora(p))
+        return all_lora_params
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/gptneo.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/gptneo.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import torch
 from torch.nn.parameter import Parameter
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 from ..policy import maybe_copy_qkv
 
+from ..policy import maybe_get_lora
+
 
 class DS_GPTNEOContainer(MetaTensorContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
@@ -68,20 +70,25 @@
         try:
             import transformers
             HFGPTNEOLayerPolicy._orig_layer_class = transformers.models.gpt_neo.modeling_gpt_neo.GPTNeoBlock
         except:
             HFGPTNEOLayerPolicy._orig_layer_class = None
 
     def get_hidden_heads(self):
-        return self.client_module.attn.attention.q_proj.weight.shape[1], \
+        return self.client_module.attn.attention.embed_dim, \
                 self.client_module.attn.attention.num_heads, \
                 self.client_module.ln_1.eps
 
     def get_q_k_v(self):
-        return None
+        return self.client_module.attn.attention.q_proj.weight, \
+               None, \
+               self.client_module.attn.attention.k_proj.weight, \
+               None, \
+               self.client_module.attn.attention.v_proj.weight, \
+               None
 
     def attention(self, enable_training=False):
         qw = self.client_module.attn.attention.q_proj.weight
         kw = self.client_module.attn.attention.k_proj.weight
         vw = self.client_module.attn.attention.v_proj.weight
 
         qkvw = Parameter(torch.cat((qw, kw, vw), dim=0), requires_grad=enable_training)
@@ -100,8 +107,18 @@
     def layernorm(self):
         return self.client_module.ln_2.weight, \
                self.client_module.ln_2.bias, \
                self.client_module.ln_1.weight, \
                self.client_module.ln_1.bias
 
     def get_lora_params(self):
-        return []
+        all_lora_params = []
+        for p in [
+            self.client_module.mlp.c_fc, \
+            self.client_module.mlp.c_proj, \
+            self.client_module.attn.attention.q_proj, \
+            self.client_module.attn.attention.k_proj, \
+            self.client_module.attn.attention.v_proj, \
+            self.client_module.attn.attention.out_proj, \
+            ]:
+            all_lora_params.append(maybe_get_lora(p))
+        return all_lora_params
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/gptneox.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/gptneox.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from deepspeed.model_implementations.transformers.ds_gpt import DeepSpeedGPTInference
 import torch
 from ..policy import TransformerPolicy
 from ..policy import transformer_param_names
 from ..policy import maybe_copy
 from packaging import version as pkg_version
 
+from ..policy import maybe_get_lora
+
 
 class DS_GPTNEOXContainer(MetaTensorContainer, MegatronContainer, BaseTransformerContainer):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # All model specific things should be defined here instead of the base class.
@@ -87,15 +89,15 @@
 
     def get_hidden_heads(self):
         if GPTNEOXLayerPolicy.version == 0:
             attention = self.client_module.attention
         else:
             attention = self.client_module.self_attention
 
-        return self.client_module.attention.query_key_value.weight.shape[1], \
+        return self.client_module.attention.hidden_size, \
                 self.client_module.attention.num_attention_heads, \
                 self.client_module.input_layernorm.eps
 
     def get_q_k_v(self):
         return None
 
     def attention(self, enable_training=False):
@@ -118,8 +120,21 @@
     def layernorm(self):
         return self.client_module.post_attention_layernorm.weight, \
                self.client_module.post_attention_layernorm.bias, \
                self.client_module.input_layernorm.weight, \
                self.client_module.input_layernorm.bias
 
     def get_lora_params(self):
-        return []
+        if GPTNEOXLayerPolicy.version == 0:
+            attention = self.client_module.attention
+        else:
+            attention = self.client_module.self_attention
+
+        all_lora_params = []
+        for p in [
+            self.client_module.mlp.dense_h_to_4h, \
+            self.client_module.mlp.dense_4h_to_h, \
+            attention.query_key_value, \
+            attention.dense
+            ]:
+            all_lora_params.append(maybe_get_lora(p))
+        return all_lora_params
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt_moe.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/megatron_gpt_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/opt.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,22 +79,22 @@
             HFOPTLayerPolicy._orig_layer_class = transformers.models.opt.modeling_opt.OPTDecoderLayer
         except:
             HFOPTLayerPolicy._orig_layer_class = None
 
         if hasattr(TransformerPolicy, "hf_model_config") and hasattr(TransformerPolicy.hf_model_config,
                                                                      "activation_function"):
             if TransformerPolicy.hf_model_config.activation_function == "relu":
-                self.mlp_act_func_type == ActivationFuncType.ReLU
+                self.mlp_act_func_type = ActivationFuncType.ReLU
             elif TransformerPolicy.hf_model_config.activation_function in ["gelu", "gelu_new"]:
-                self.mlp_act_func_type == ActivationFuncType.GELU
+                self.mlp_act_func_type = ActivationFuncType.GELU
             else:
                 raise ValueError("Unsupported activation function: {}".format(
                     TransformerPolicy.hf_model_config.activation_function))
         else:
-            self.mlp_act_func_type == ActivationFuncType.ReLU  # default
+            self.mlp_act_func_type = ActivationFuncType.ReLU  # default
 
     def get_hidden_heads(self):
         return self.client_module.self_attn.embed_dim, \
                 self.client_module.self_attn.num_heads, \
                 self.client_module.self_attn_layer_norm.eps
 
     def get_q_k_v(self):
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/unet.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/containers/vae.py` & `deepspeed-0.9.2/deepspeed/module_inject/containers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/inject.py` & `deepspeed-0.9.2/deepspeed/module_inject/inject.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/layers.py` & `deepspeed-0.9.2/deepspeed/module_inject/layers.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/load_checkpoint.py` & `deepspeed-0.9.2/deepspeed/module_inject/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/module_quantize.py` & `deepspeed-0.9.2/deepspeed/module_inject/module_quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/policy.py` & `deepspeed-0.9.2/deepspeed/module_inject/policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/replace_module.py` & `deepspeed-0.9.2/deepspeed/module_inject/replace_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,53 +38,49 @@
 
     def merge_assert(self, dim1, dim2):
         assert dim1 > dim2, \
             'Merging tensors is not allowed here! Please use deepspeed load_checkpoint\
             for merging your checkpoints before replacing the transformer layer with\
             inference-kernels'
 
-    def qkv_copy(self, dst, src, int8=False):
+    def qkv_copy(self, dst, src, int8=False, allocat_tensor=False):
         if src is None:
             return src
         src_shape = src.shape
         dst_shape = dst.shape
 
         outer_dim = 0 if int8 else -1
         inner_dim = -1 if int8 else 0
 
+        if allocat_tensor:
+            dst = torch.empty_like(dst)
+
         src_split = torch.split(src.data, src.shape[outer_dim] // 3, dim=outer_dim)
         if (len(src_shape) == 2 and len(dst_shape) == 2):
             if src_shape[outer_dim] == dst_shape[self.out_dim]:
                 dst = dst.reshape(-1).data.copy_(src.data.reshape(-1)).reshape(src.shape)
                 dst = torch.nn.parameter.Parameter(dst, requires_grad=False)
                 if hasattr(src, 'scale'):
                     dst.scale = src.scale
                 return dst
-            if self.out_dim == 1:
-                self.merge_assert(src_shape[outer_dim], dst_shape[self.out_dim])
-                qkv_size = dst_shape[self.out_dim] // 3
-                qkv_split = [torch.split(src_s, qkv_size, dim=outer_dim) for src_s in src_split]
-
-                weight_split = [
-                    torch.cat([qkv_s[i] for qkv_s in qkv_split], axis=outer_dim) for i in range(len(qkv_split[0]))
-                ]
-                dst = dst.reshape(-1).data.copy_(weight_split[self.gpu_index].contiguous().reshape(-1)).reshape(
-                    weight_split[self.gpu_index].shape)
-            else:
-                dst.data.copy_(src_split[self.gpu_index].to(get_accelerator().current_device_name()).contiguous())
+            self.merge_assert(src_shape[outer_dim], dst_shape[self.out_dim])
+            qkv_size = dst_shape[self.out_dim] // 3
+            qkv_split = [torch.split(src_s, qkv_size, dim=outer_dim) for src_s in src_split]
+            weight_split = [
+                torch.cat([qkv_s[i] for qkv_s in qkv_split], axis=outer_dim) for i in range(len(qkv_split[0]))
+            ]
+            dst = dst.reshape(-1).data.copy_(weight_split[self.gpu_index].contiguous().reshape(-1)).reshape(
+                weight_split[self.gpu_index].shape)
         else:
             if src_shape[0] == dst_shape[0]:
                 return torch.nn.parameter.Parameter(src)
-            if self.out_dim == 1:
-                qkv_size = dst_shape[0] // 3
-                qkv_split = [torch.split(src_s, qkv_size, dim=0) for src_s in src_split]
-                bias_split = [torch.cat([qkv_s[i] for qkv_s in qkv_split], axis=0) for i in range(len(qkv_split[0]))]
-                dst.data.copy_(bias_split[self.gpu_index].contiguous())
-            else:
-                dst.data.copy_(src_split[self.gpu_index].contiguous())
+            qkv_size = dst_shape[0] // 3
+            qkv_split = [torch.split(src_s, qkv_size, dim=0) for src_s in src_split]
+            bias_split = [torch.cat([qkv_s[i] for qkv_s in qkv_split], axis=0) for i in range(len(qkv_split[0]))]
+            dst.data.copy_(bias_split[self.gpu_index].contiguous())
 
         dst = torch.nn.parameter.Parameter(dst, requires_grad=False)
         if hasattr(src, 'scale'):
             dst.scale = src.scale
         return dst
 
     def copy(self, dst, src, int8=False, allocat_tensor=False):
@@ -229,15 +225,18 @@
         pass
     else:
         if fp16 is False:
             raise ValueError("Generic injection only supported with FP16")
 
         try:
             import diffusers
-            cross_attention = diffusers.models.attention.CrossAttention
+            if hasattr(diffusers.models.attention, 'CrossAttention'):
+                cross_attention = diffusers.models.attention.CrossAttention
+            else:
+                cross_attention = diffusers.models.attention_processor.Attention
             attention_block = diffusers.models.attention.BasicTransformerBlock
             new_policies = {
                 cross_attention: replace_attn,
                 attention_block: replace_attn_block,
             }
         except ImportError:
             new_policies = {}
```

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/replace_policy.py` & `deepspeed-0.9.2/deepspeed/module_inject/replace_policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/module_inject/utils.py` & `deepspeed-0.9.2/deepspeed/module_inject/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/moe/experts.py` & `deepspeed-0.9.2/deepspeed/moe/experts.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/moe/layer.py` & `deepspeed-0.9.2/deepspeed/moe/layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/moe/mappings.py` & `deepspeed-0.9.2/deepspeed/moe/mappings.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/moe/sharded_moe.py` & `deepspeed-0.9.2/deepspeed/moe/sharded_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/moe/utils.py` & `deepspeed-0.9.2/deepspeed/moe/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/monitor/config.py` & `deepspeed-0.9.2/deepspeed/monitor/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/monitor/csv_monitor.py` & `deepspeed-0.9.2/deepspeed/monitor/csv_monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/monitor/monitor.py` & `deepspeed-0.9.2/deepspeed/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/monitor/tensorboard.py` & `deepspeed-0.9.2/deepspeed/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/monitor/utils.py` & `deepspeed-0.9.2/deepspeed/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/monitor/wandb.py` & `deepspeed-0.9.2/deepspeed/monitor/wandb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/nebula/config.py` & `deepspeed-0.9.2/deepspeed/nebula/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/nebula/constants.py` & `deepspeed-0.9.2/deepspeed/nebula/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/adagrad/cpu_adagrad.py` & `deepspeed-0.9.2/deepspeed/ops/adagrad/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/adam/cpu_adam.py` & `deepspeed-0.9.2/deepspeed/ops/adam/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/adam/fused_adam.py` & `deepspeed-0.9.2/deepspeed/ops/adam/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.2/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/StopWatch.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/Timer.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/context.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/conversion_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/conversion_utils.h`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,19 @@
 
 /*********************  To Half2 Conversions *********************/
 template <>
 DS_D_INLINE __half2 to(float2 val)
 {
     return __float22half2_rn(val);
 }
+template <>
+DS_D_INLINE __half2 to(float val)
+{
+    return __float2half2_rn(val);
+}
 
 #ifdef BF16_AVAILABLE
 // No direct conversion
 template <>
 DS_D_INLINE __half2 to(__nv_bfloat162 val)
 {
     return to<__half2>(to<float2>(val));
@@ -402,14 +407,19 @@
 #ifdef BF16_AVAILABLE
 template <>
 DS_D_INLINE __nv_bfloat162 to(float2 val)
 {
     return __float22bfloat162_rn(val);
 }
 template <>
+DS_D_INLINE __nv_bfloat162 to(float val)
+{
+    return __float2bfloat162_rn(val);
+}
+template <>
 DS_D_INLINE __nv_bfloat162 to(__half2 val)
 {
     return to<__nv_bfloat162>(to<float2>(val));
 }
 #endif
 
 /*********************  To INT64_T Conversions *********************/
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adam.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/dropout.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/feed_forward.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/gelu.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/gemm_test.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/general_kernels.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/normalize_layer.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/reduction_utils.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/simd.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/softmax.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/includes/type_shim.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/dequantize.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/quantize.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 
 #pragma once
 
 #if __CUDA_ARCH__ >= 530
 #define HALF_PRECISION_AVAILABLE = 1
 #endif
 
+#ifdef __HIP_PLATFORM_HCC__
+#include <hip/hip_cooperative_groups.h>
+#else
 #include <cooperative_groups.h>
+#endif
+
 #include <cuda.h>
 #include <cuda_fp16.h>
 
 /*********** Group Norm Kernels, Structs, and Helpers ************/
 
 struct {
     int64_t batch_size;
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.2/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 // Copyright (c) Microsoft Corporation.
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
-#include "cublas_wrappers.h"
+#pragma once
+
+#include <assert.h>
+#include <cublas_v2.h>
+#include <cuda.h>
+#include <cuda_bf16.h>
+#include <cuda_fp16.h>
+#include <cuda_runtime.h>
+#ifndef __HIP_PLATFORM_HCC__
+#include <mma.h>
+#endif
+#include <stdio.h>
 
 #ifdef __HIP_PLATFORM_HCC__
 int cublas_gemm_ex(rocblas_handle handle,
                    rocblas_operation transa,
                    rocblas_operation transb,
                    int m,
                    int n,
@@ -92,84 +103,88 @@
                 k,
                 (int)status);
         return EXIT_FAILURE;
     }
     return 0;
 }
 
+template <typename T>
 #ifdef __HIP_PLATFORM_HCC__
 int cublas_gemm_ex(rocblas_handle handle,
                    rocblas_operation transa,
                    rocblas_operation transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
-                   const __half* A,
-                   const __half* B,
-                   __half* C,
+                   const T* A,
+                   const T* B,
+                   T* C,
                    rocblas_gemm_algo algo)
 #else
 int cublas_gemm_ex(cublasHandle_t handle,
                    cublasOperation_t transa,
                    cublasOperation_t transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
-                   const __half* A,
-                   const __half* B,
-                   __half* C,
+                   const T* A,
+                   const T* B,
+                   T* C,
                    cublasGemmAlgo_t algo)
 #endif
 {
 #ifdef __HIP_PLATFORM_HCC__
+    constexpr auto rocblas_dtype_16 = std::is_same<T, __half>::value ? rocblas_datatype_f16_r
+                                                                     : rocblas_datatype_bf16_r;
     rocblas_status status = rocblas_gemm_ex(handle,
                                             transa,
                                             transb,
                                             m,
                                             n,
                                             k,
                                             (const void*)alpha,
                                             (const void*)A,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             (transa == rocblas_operation_none) ? m : k,
                                             (const void*)B,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             (transb == rocblas_operation_none) ? k : n,
                                             (const void*)beta,
                                             (void*)C,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             m,
                                             (void*)C,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             m,
                                             rocblas_datatype_f32_r,
                                             algo,
                                             0,
                                             0);
 #else
+    constexpr auto cublas_dtype_16 = std::is_same<T, __half>::value ? CUDA_R_16F : CUDA_R_16BF;
     cublasStatus_t status = cublasGemmEx(handle,
                                          transa,
                                          transb,
                                          m,
                                          n,
                                          k,
                                          (const void*)alpha,
                                          (const void*)A,
-                                         CUDA_R_16F,
+                                         cublas_dtype_16,
                                          (transa == CUBLAS_OP_N) ? m : k,
                                          (const void*)B,
-                                         CUDA_R_16F,
+                                         cublas_dtype_16,
                                          (transb == CUBLAS_OP_N) ? k : n,
                                          (const void*)beta,
                                          (void*)C,
-                                         CUDA_R_16F,
+                                         cublas_dtype_16,
                                          m,
                                          CUDA_R_32F,
                                          algo);
 #endif
 
 #ifdef __HIP_PLATFORM_HCC__
     if (status != rocblas_status_success) {
@@ -293,100 +308,104 @@
                 k,
                 (int)status);
         return EXIT_FAILURE;
     }
     return 0;
 }
 
+template <typename T>
 #ifdef __HIP_PLATFORM_HCC__
 int cublas_strided_batched_gemm(rocblas_handle handle,
                                 int m,
                                 int n,
                                 int k,
                                 const float* alpha,
                                 const float* beta,
-                                const __half* A,
-                                const __half* B,
-                                __half* C,
+                                const T* A,
+                                const T* B,
+                                T* C,
                                 rocblas_operation op_A,
                                 rocblas_operation op_B,
                                 int stride_A,
                                 int stride_B,
                                 int stride_C,
                                 int batch,
                                 rocblas_gemm_algo algo)
 #else
 int cublas_strided_batched_gemm(cublasHandle_t handle,
                                 int m,
                                 int n,
                                 int k,
                                 const float* alpha,
                                 const float* beta,
-                                const __half* A,
-                                const __half* B,
-                                __half* C,
+                                const T* A,
+                                const T* B,
+                                T* C,
                                 cublasOperation_t op_A,
                                 cublasOperation_t op_B,
                                 int stride_A,
                                 int stride_B,
                                 int stride_C,
                                 int batch,
                                 cublasGemmAlgo_t algo)
 #endif
 {
 #ifdef __HIP_PLATFORM_HCC__
+    constexpr auto rocblas_dtype_16 = std::is_same<T, __half>::value ? rocblas_datatype_f16_r
+                                                                     : rocblas_datatype_bf16_r;
     rocblas_status status =
         rocblas_gemm_strided_batched_ex(handle,
                                         op_A,
                                         op_B,
                                         m,
                                         n,
                                         k,
                                         alpha,
                                         A,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         (op_A == rocblas_operation_none) ? m : k,
                                         stride_A,
                                         B,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         (op_B == rocblas_operation_none) ? k : n,
                                         stride_B,
                                         beta,
                                         C,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         m,
                                         stride_C,
                                         C,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         m,
                                         stride_C,
                                         batch,
                                         rocblas_datatype_f32_r,
                                         algo,
                                         0,
                                         0);
 #else
+    constexpr auto cublas_dtype_16 = std::is_same<T, __half>::value ? CUDA_R_16F : CUDA_R_16BF;
     cublasStatus_t status = cublasGemmStridedBatchedEx(handle,
                                                        op_A,
                                                        op_B,
                                                        m,
                                                        n,
                                                        k,
                                                        alpha,
                                                        A,
-                                                       CUDA_R_16F,
+                                                       cublas_dtype_16,
                                                        (op_A == CUBLAS_OP_N) ? m : k,
                                                        stride_A,
                                                        B,
-                                                       CUDA_R_16F,
+                                                       cublas_dtype_16,
                                                        (op_B == CUBLAS_OP_N) ? k : n,
                                                        stride_B,
                                                        beta,
                                                        C,
-                                                       CUDA_R_16F,
+                                                       cublas_dtype_16,
                                                        m,
                                                        stride_C,
                                                        batch,
                                                        CUDA_R_32F,
                                                        algo);
 #endif
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/general_kernels.cu`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                               int seq_length,
                               int hidden_dim,
                               cudaStream_t& stream)
 {
     int total_count = batch_size * seq_length * hidden_dim / 4;
     dim3 grid_dim = DS_GET_BLOCKS(total_count);  //(batch_size * seq_length);
 
-    dim3 block_dim = DS_CUDA_NUM_THREADS;        //(hidden_dim / 4);
+    dim3 block_dim = DS_CUDA_NUM_THREADS;  //(hidden_dim / 4);
 
     fused_add2_kernel<<<grid_dim, block_dim, 0, stream>>>(total_count, out, inp1, inp2);
 }
 
 template <>
 void launch_fused_add2<__half>(__half* out,
                                const __half* inp1,
@@ -175,15 +175,15 @@
                                int seq_length,
                                int hidden_dim,
                                cudaStream_t& stream)
 {
     int total_count = batch_size * seq_length * hidden_dim / 4;
     dim3 grid_dim = DS_GET_BLOCKS(total_count);  //(batch_size * seq_length);
 
-    dim3 block_dim = DS_CUDA_NUM_THREADS;        //(hidden_dim / 4);
+    dim3 block_dim = DS_CUDA_NUM_THREADS;  //(hidden_dim / 4);
 
     fused_add2_kernel<<<grid_dim, block_dim, 0, stream>>>(total_count, out, inp1, inp2);
 }
 
 __global__ void fused_add3_kernel(float* out,
                                   const float* inp1,
                                   const float* inp2,
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 // Copyright (c) Microsoft Corporation.
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
+#include "conversion_utils.h"
 #include "inference_cuda_layers.h"
 
 #ifndef __HIP_PLATFORM_HCC__
 #include <cuda_profiler_api.h>
 #endif
 
 namespace cg = cooperative_groups;
 namespace cg = cooperative_groups;
 
-__global__ void apply_rotary_pos_emb(float* mixed_query,
-                                     float* key_layer,
+template <typename T>
+__global__ void apply_rotary_pos_emb(T* mixed_query,
+                                     T* key_layer,
                                      unsigned rotary_dim,
                                      unsigned seq_len,
                                      unsigned seq_offset,
                                      unsigned num_heads,
                                      unsigned head_size,
                                      unsigned total_count,
                                      int max_out_tokens)
@@ -36,77 +38,32 @@
     unsigned seq_index = head_id % seq_len;
     unsigned k_offset = (seq_index + (head_id / seq_len) * max_out_tokens) * head_size;
 
     if (head_id < total_count) {
         while (lane < rotary_dim) {
             float inv_freq = (float)((lane / 2) * 2) / (float)rotary_dim;
             inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
-            float q = mixed_query[offset + lane];
-            float k = key_layer[k_offset + lane];
+            float q = conversion::to<float>(mixed_query[offset + lane]);
+            float k = conversion::to<float>(key_layer[k_offset + lane]);
             float rotary_sign = (lane % 2 == 1 ? -1.0 : 1.0);
             float q_rot = (q * rotary_sign);
             float k_rot = (k * rotary_sign);
             q_rot = g.shfl_xor(q_rot, 1);
             k_rot = g.shfl_xor(k_rot, 1);
             q = q * cosf(inv_freq) + q_rot * sinf(inv_freq);
             k = k * cosf(inv_freq) + k_rot * sinf(inv_freq);
 
-            mixed_query[offset + lane] = q;
-            key_layer[k_offset + lane] = k;
+            mixed_query[offset + lane] = conversion::to<T>(q);
+            key_layer[k_offset + lane] = conversion::to<T>(k);
 
             lane += WARP_SIZE;
         }
     }
 }
 
-__global__ void apply_rotary_pos_emb(__half* mixed_query,
-                                     __half* key_layer,
-                                     unsigned rotary_dim,
-                                     unsigned seq_len,
-                                     unsigned seq_offset,
-                                     unsigned num_heads,
-                                     unsigned head_size,
-                                     unsigned total_count,
-                                     int max_out_tokens)
-{
-    cg::thread_block b = cg::this_thread_block();
-    cg::thread_block_tile<WARP_SIZE> g = cg::tiled_partition<WARP_SIZE>(b);
-
-    int id = threadIdx.x;
-    int gid = id >> 5;
-    int lane = id & 0x1f;
-
-    unsigned head_id = blockIdx.x * MAX_WARP_NUM + gid;
-    unsigned offset = head_id * head_size;
-
-    unsigned seq_id = (head_id / num_heads) % seq_len + seq_offset;
-    unsigned seq_index = head_id % seq_len;
-    unsigned k_offset = (seq_index + (head_id / seq_len) * max_out_tokens) * head_size;
-
-    if (head_id < total_count) {
-        while (lane < rotary_dim) {
-            float inv_freq = (float)((lane / 2) * 2) / (float)rotary_dim;
-            inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
-            float q = (float)mixed_query[offset + lane];
-            float k = (float)key_layer[k_offset + lane];
-            float rotary_sign = (lane % 2 == 1 ? -1.0 : 1.0);
-            float q_rot = (q * rotary_sign);
-            float k_rot = (k * rotary_sign);
-            q_rot = g.shfl_xor(q_rot, 1);
-            k_rot = g.shfl_xor(k_rot, 1);
-            q = q * cosf(inv_freq) + q_rot * sinf(inv_freq);
-            k = k * cosf(inv_freq) + k_rot * sinf(inv_freq);
-
-            mixed_query[offset + lane] = (__half)q;
-            key_layer[k_offset + lane] = (__half)k;
-
-            lane += WARP_SIZE;
-        }
-    }
-}
 __global__ void apply_rotary_pos_emb1(float* mixed_query,
                                       float* key_layer,
                                       unsigned rotary_dim,
                                       unsigned seq_len,
                                       unsigned seq_offset,
                                       unsigned num_heads,
                                       unsigned head_size,
@@ -144,16 +101,18 @@
             mixed_query[offset + lane] = q;
             key_layer[k_offset + lane] = k;
 
             lane += WARP_SIZE;
         }
     }
 }
-__global__ void apply_rotary_pos_emb1(__half* mixed_query,
-                                      __half* key_layer,
+
+template <typename T>
+__global__ void apply_rotary_pos_emb1(T* mixed_query,
+                                      T* key_layer,
                                       unsigned rotary_dim,
                                       unsigned seq_len,
                                       unsigned seq_offset,
                                       unsigned num_heads,
                                       unsigned head_size,
                                       unsigned total_count,
                                       int max_out_tokens)
@@ -181,28 +140,28 @@
 
     unsigned seq_id = (head_id % seq_len) + seq_offset;
     unsigned half_dim = rotary_dim >> 1;
     if (head_id < total_count) {
         while (lane < rotary_dim) {
             float inv_freq = (float)((lane % half_dim) * 2) / (float)rotary_dim;
             inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
-            float q = (float)mixed_query[offset + lane];
-            float k = (float)key_layer[k_offset + lane];
+            float q = conversion::to<float>(mixed_query[offset + lane]);
+            float k = conversion::to<float>(key_layer[k_offset + lane]);
             float rotary_sign = (lane > (half_dim - 1) ? -1.0 : 1.0);
             float q_rot = (q * rotary_sign);
             float k_rot = (k * rotary_sign);
             auto q_rot_tmp = lane < half_dim ? __shfl_sync(mask[lane], q_rot, lane + half_dim)
                                              : __shfl_sync(mask[lane], q_rot, lane - half_dim);
             auto k_rot_tmp = lane < half_dim ? __shfl_sync(mask[lane], k_rot, lane + half_dim)
                                              : __shfl_sync(mask[lane], k_rot, lane - half_dim);
             q = q * cosf(inv_freq) + q_rot_tmp * sinf(inv_freq);
             k = k * cosf(inv_freq) + k_rot_tmp * sinf(inv_freq);
 
-            mixed_query[offset + lane] = (__half)q;
-            key_layer[k_offset + lane] = (__half)k;
+            mixed_query[offset + lane] = conversion::to<T>(q);
+            key_layer[k_offset + lane] = conversion::to<T>(k);
 
             lane += WARP_SIZE;
         }
     }
 }
 
 template <typename T>
@@ -252,27 +211,94 @@
                                                  unsigned,
                                                  unsigned,
                                                  unsigned,
                                                  bool,
                                                  bool,
                                                  cudaStream_t,
                                                  int);
+#ifdef BF16_AVAILABLE
+template void launch_apply_rotary_pos_emb<__nv_bfloat16>(__nv_bfloat16*,
+                                                         __nv_bfloat16*,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         unsigned,
+                                                         bool,
+                                                         bool,
+                                                         cudaStream_t,
+                                                         int);
+#endif
 template void launch_apply_rotary_pos_emb<__half>(__half*,
                                                   __half*,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   unsigned,
                                                   bool,
                                                   bool,
                                                   cudaStream_t,
                                                   int);
 
+template __global__ void apply_rotary_pos_emb(float* mixed_query,
+                                              float* key_layer,
+                                              unsigned rotary_dim,
+                                              unsigned seq_len,
+                                              unsigned seq_offset,
+                                              unsigned num_heads,
+                                              unsigned head_size,
+                                              unsigned total_count,
+                                              int max_out_tokens);
+
+#ifdef BF16_AVAILABLE
+template __global__ void apply_rotary_pos_emb(__nv_bfloat16* mixed_query,
+                                              __nv_bfloat16* key_layer,
+                                              unsigned rotary_dim,
+                                              unsigned seq_len,
+                                              unsigned seq_offset,
+                                              unsigned num_heads,
+                                              unsigned head_size,
+                                              unsigned total_count,
+                                              int max_out_tokens);
+#endif
+
+template __global__ void apply_rotary_pos_emb(__half* mixed_query,
+                                              __half* key_layer,
+                                              unsigned rotary_dim,
+                                              unsigned seq_len,
+                                              unsigned seq_offset,
+                                              unsigned num_heads,
+                                              unsigned head_size,
+                                              unsigned total_count,
+                                              int max_out_tokens);
+
+#ifdef BF16_AVAILABLE
+template __global__ void apply_rotary_pos_emb1(__nv_bfloat16* mixed_query,
+                                               __nv_bfloat16* key_layer,
+                                               unsigned rotary_dim,
+                                               unsigned seq_len,
+                                               unsigned seq_offset,
+                                               unsigned num_heads,
+                                               unsigned head_size,
+                                               unsigned total_count,
+                                               int max_out_tokens);
+#endif
+
+template __global__ void apply_rotary_pos_emb1(__half* mixed_query,
+                                               __half* key_layer,
+                                               unsigned rotary_dim,
+                                               unsigned seq_len,
+                                               unsigned seq_offset,
+                                               unsigned num_heads,
+                                               unsigned head_size,
+                                               unsigned total_count,
+                                               int max_out_tokens);
 /*
 __global__ void apply_rotary_pos_emb(float* mixed_query,
 float* key_layer,
 unsigned rotary_dim,
 unsigned seq_len,
 unsigned seq_offset,
 unsigned num_heads,
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 #include "inference_cuda_layers.h"
 #include "memory_access_utils.h"
 
 namespace cg = cooperative_groups;
 #define MAX_CAP 4
 #define MAX_SEQ 2048
 
+// only used to avoid compilation error due to lack of definition.
+#ifndef BF16_AVAILABLE
+using __nv_bfloat162 = __half2;
+#endif
+
 inline __device__ float gelu(const float x)
 {
     const float sqrt_param = 0.79788456080286535587989211986876f;
     const float mul_param = 0.044715;
     return x * 0.5f * (1.0f + tanhf(sqrt_param * (x + mul_param * x * x * x)));
 }
 
@@ -62,14 +67,21 @@
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_gelu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
 template void launch_bias_gelu<float>(float*, const float*, int, int, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_gelu<__nv_bfloat16>(__nv_bfloat16*,
+                                              const __nv_bfloat16*,
+                                              int,
+                                              int,
+                                              cudaStream_t);
+#endif
 template void launch_bias_gelu<__half>(__half*, const __half*, int, int, cudaStream_t);
 
 /*
 In-place channels-last bias add
 */
 template <typename T>
 __global__ void fused_bias_add(T* input, const T* bias, int total_count, int intermediate_size)
@@ -112,14 +124,21 @@
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_add<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
 template void launch_bias_add<float>(float*, const float*, int, int, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_add<__nv_bfloat16>(__nv_bfloat16*,
+                                             const __nv_bfloat16*,
+                                             int,
+                                             int,
+                                             cudaStream_t);
+#endif
 template void launch_bias_add<__half>(__half*, const __half*, int, int, cudaStream_t);
 
 __global__ void fused_bias_residual(float* residual,
                                     const float* hidden_state,
                                     const float* attn,
                                     const float* bias,
                                     const float* attn_bias,
@@ -159,58 +178,61 @@
             res_fl4.z = res_fl4.z + hs_fl4.z + bias_fl4.z;
             res_fl4.w = res_fl4.w + hs_fl4.w + bias_fl4.w;
         }
         res_fl4_ptr[offset] = res_fl4;
     }
 }
 
-__global__ void fused_bias_residual(__half* residual,
-                                    const __half* hidden_state,
-                                    const __half* attn,
-                                    const __half* bias,
-                                    const __half* attn_bias,
+template <typename T>
+__global__ void fused_bias_residual(T* residual,
+                                    const T* hidden_state,
+                                    const T* attn,
+                                    const T* bias,
+                                    const T* attn_bias,
                                     const int total_count,
                                     const int intermediate_size,
                                     const float mp_scale,
                                     const bool preln)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float2* res_fl2_ptr = reinterpret_cast<float2*>(residual);
     const float2* hs_fl2_ptr = reinterpret_cast<const float2*>(hidden_state);
     const float2* attn_fl2_ptr = reinterpret_cast<const float2*>(attn);
     const float2* bias_fl2_ptr = reinterpret_cast<const float2*>(bias);
     const float2* attn_bias_fl2_ptr = reinterpret_cast<const float2*>(attn_bias);
     const int offset = blockIdx.x * blockDim.x + threadIdx.x;
 
     if (offset < total_count) {
         float2 res_fl2 = res_fl2_ptr[offset];
         const float2 hs_fl2 = hs_fl2_ptr[offset];
         const float2 attn_fl2 = attn_fl2_ptr[offset];
         const float2 bias_fl2 = bias_fl2_ptr[offset % intermediate_size];
         const float2 attn_bias_fl2 = attn_bias_fl2_ptr[offset % intermediate_size];
 
-        __half2* res_half2 = reinterpret_cast<__half2*>(&res_fl2);
-        const __half2* hs_half2 = reinterpret_cast<const __half2*>(&hs_fl2);
-        const __half2* attn_half2 = reinterpret_cast<const __half2*>(&attn_fl2);
-        const __half2* bias_half2 = reinterpret_cast<const __half2*>(&bias_fl2);
-        const __half2* attn_bias_half2 = reinterpret_cast<const __half2*>(&attn_bias_fl2);
-
-        float2 res_low = __half22float2(res_half2[0]);
-        float2 res_high = __half22float2(res_half2[1]);
-
-        const float2 hs_low = __half22float2(hs_half2[0]);
-        const float2 hs_high = __half22float2(hs_half2[1]);
+        T2* res_half2 = reinterpret_cast<T2*>(&res_fl2);
+        const T2* hs_half2 = reinterpret_cast<const T2*>(&hs_fl2);
+        const T2* attn_half2 = reinterpret_cast<const T2*>(&attn_fl2);
+        const T2* bias_half2 = reinterpret_cast<const T2*>(&bias_fl2);
+        const T2* attn_bias_half2 = reinterpret_cast<const T2*>(&attn_bias_fl2);
+
+        float2 res_low = conversion::to<float2>(res_half2[0]);
+        float2 res_high = conversion::to<float2>(res_half2[1]);
+
+        const float2 hs_low = conversion::to<float2>(hs_half2[0]);
+        const float2 hs_high = conversion::to<float2>(hs_half2[1]);
 
-        const float2 attn_low = __half22float2(attn_half2[0]);
-        const float2 attn_high = __half22float2(attn_half2[1]);
+        const float2 attn_low = conversion::to<float2>(attn_half2[0]);
+        const float2 attn_high = conversion::to<float2>(attn_half2[1]);
 
-        const float2 bias_low = __half22float2(bias_half2[0]);
-        const float2 bias_high = __half22float2(bias_half2[1]);
+        const float2 bias_low = conversion::to<float2>(bias_half2[0]);
+        const float2 bias_high = conversion::to<float2>(bias_half2[1]);
 
-        const float2 attn_bias_low = __half22float2(attn_bias_half2[0]);
-        const float2 attn_bias_high = __half22float2(attn_bias_half2[1]);
+        const float2 attn_bias_low = conversion::to<float2>(attn_bias_half2[0]);
+        const float2 attn_bias_high = conversion::to<float2>(attn_bias_half2[1]);
 
         if (preln) {
             // residual = (residual + attention + bias + attention_bias) *
             // mp_scale + hidden_state
             res_low.x =
                 (res_low.x + attn_low.x + bias_low.x + attn_bias_low.x) * mp_scale + hs_low.x;
             res_low.y =
@@ -222,16 +244,16 @@
         } else {
             // residual += hidden_state + bias
             res_low.x = (res_low.x + hs_low.x + bias_low.x);
             res_low.y = (res_low.y + hs_low.y + bias_low.y);
             res_high.x = (res_high.x + hs_high.x + bias_high.x);
             res_high.y = (res_high.y + hs_high.y + bias_high.y);
         }
-        res_half2[0] = __float22half2_rn(res_low);
-        res_half2[1] = __float22half2_rn(res_high);
+        res_half2[0] = conversion::to<T2>(res_low);
+        res_half2[1] = conversion::to<T2>(res_high);
 
         res_fl2_ptr[offset] = res_fl2;
     }
 }
 
 template <typename T>
 void launch_bias_residual(T* residual,
@@ -258,17 +280,51 @@
                                                               hidden_dim / 4,
                                                               1.0 / mp_size,
                                                               preln);
 }
 
 template void launch_bias_residual<
     float>(float*, float*, float*, float*, float*, int, int, int, bool, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_residual<__nv_bfloat16>(__nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  __nv_bfloat16*,
+                                                  int,
+                                                  int,
+                                                  int,
+                                                  bool,
+                                                  cudaStream_t);
+#endif
 template void launch_bias_residual<
     __half>(__half*, __half*, __half*, __half*, __half*, int, int, int, bool, cudaStream_t);
 
+#ifdef BF16_AVAILABLE
+template __global__ void fused_bias_residual(__nv_bfloat16* residual,
+                                             const __nv_bfloat16* hidden_state,
+                                             const __nv_bfloat16* attn,
+                                             const __nv_bfloat16* bias,
+                                             const __nv_bfloat16* attn_bias,
+                                             const int total_count,
+                                             const int intermediate_size,
+                                             const float mp_scale,
+                                             const bool preln);
+#endif
+
+template __global__ void fused_bias_residual(__half* residual,
+                                             const __half* hidden_state,
+                                             const __half* attn,
+                                             const __half* bias,
+                                             const __half* attn_bias,
+                                             const int total_count,
+                                             const int intermediate_size,
+                                             const float mp_scale,
+                                             const bool preln);
+
 __global__ void gptj_residual_add(float* residual,
                                   const float* hidden_state,
                                   const float* attn,
                                   const float* bias,
                                   const float* attn_bias,
                                   const int total_count,
                                   const int intermediate_size,
@@ -301,72 +357,75 @@
         res_fl4.z = hs_fl4.z + attn_fl4.z + (res_fl4.z + bias_fl4.z) * mp_scale;
         res_fl4.w = hs_fl4.w + attn_fl4.w + (res_fl4.w + bias_fl4.w) * mp_scale;
 
         res_fl4_ptr[offset] = res_fl4;
     }
 }
 
-__global__ void gptj_residual_add(__half* residual,
-                                  const __half* hidden_state,
-                                  const __half* attn,
-                                  const __half* bias,
-                                  const __half* attn_bias,
+template <typename T>
+__global__ void gptj_residual_add(T* residual,
+                                  const T* hidden_state,
+                                  const T* attn,
+                                  const T* bias,
+                                  const T* attn_bias,
                                   const int total_count,
                                   const int intermediate_size,
                                   const float mp_scale)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float2* res_fl2_ptr = reinterpret_cast<float2*>(residual);
     const float2* hs_fl2_ptr = reinterpret_cast<const float2*>(hidden_state);
     const float2* attn_fl2_ptr = reinterpret_cast<const float2*>(attn);
     const float2* bias_fl2_ptr = reinterpret_cast<const float2*>(bias);
     const float2* attn_bias_fl2_ptr = reinterpret_cast<const float2*>(attn_bias);
     const int offset = blockIdx.x * blockDim.x + threadIdx.x;
 
     if (offset < total_count) {
         float2 res_fl2 = res_fl2_ptr[offset];
         const float2 hs_fl2 = hs_fl2_ptr[offset];
         const float2 attn_fl2 = attn_fl2_ptr[offset];
         const float2 bias_fl2 = bias_fl2_ptr[offset % intermediate_size];
 
-        __half2* res_half2 = reinterpret_cast<__half2*>(&res_fl2);
-        const __half2* hs_half2 = reinterpret_cast<const __half2*>(&hs_fl2);
-        const __half2* attn_half2 = reinterpret_cast<const __half2*>(&attn_fl2);
-        const __half2* bias_half2 = reinterpret_cast<const __half2*>(&bias_fl2);
-
-        float2 res_low = __half22float2(res_half2[0]);
-        float2 res_high = __half22float2(res_half2[1]);
+        T2* res_half2 = reinterpret_cast<T2*>(&res_fl2);
+        const T2* hs_half2 = reinterpret_cast<const T2*>(&hs_fl2);
+        const T2* attn_half2 = reinterpret_cast<const T2*>(&attn_fl2);
+        const T2* bias_half2 = reinterpret_cast<const T2*>(&bias_fl2);
+
+        float2 res_low = conversion::to<float2>(res_half2[0]);
+        float2 res_high = conversion::to<float2>(res_half2[1]);
 
-        const float2 hs_low = __half22float2(hs_half2[0]);
-        const float2 hs_high = __half22float2(hs_half2[1]);
+        const float2 hs_low = conversion::to<float2>(hs_half2[0]);
+        const float2 hs_high = conversion::to<float2>(hs_half2[1]);
 
-        const float2 attn_low = __half22float2(attn_half2[0]);
-        const float2 attn_high = __half22float2(attn_half2[1]);
+        const float2 attn_low = conversion::to<float2>(attn_half2[0]);
+        const float2 attn_high = conversion::to<float2>(attn_half2[1]);
 
-        const float2 bias_low = __half22float2(bias_half2[0]);
-        const float2 bias_high = __half22float2(bias_half2[1]);
+        const float2 bias_low = conversion::to<float2>(bias_half2[0]);
+        const float2 bias_high = conversion::to<float2>(bias_half2[1]);
 
         if (attn_bias) {
             const float2 attn_bias_fl2 = attn_bias_fl2_ptr[offset % intermediate_size];
-            const __half2* attn_bias_half2 = reinterpret_cast<const __half2*>(&attn_bias_fl2);
-            const float2 attn_bias_low = __half22float2(attn_bias_half2[0]);
-            const float2 attn_bias_high = __half22float2(attn_bias_half2[1]);
+            const T2* attn_bias_half2 = reinterpret_cast<const T2*>(&attn_bias_fl2);
+            const float2 attn_bias_low = conversion::to<float2>(attn_bias_half2[0]);
+            const float2 attn_bias_high = conversion::to<float2>(attn_bias_half2[1]);
             // residual += attention_bias
             res_low.x += attn_bias_low.x;
             res_low.y += attn_bias_low.y;
             res_high.x += attn_bias_high.x;
             res_high.y += attn_bias_high.y;
         }
         // residual = hidden_state + attention + (residual + bias) * mp_scale
         res_low.x = attn_low.x + hs_low.x + (res_low.x + bias_low.x) * mp_scale;
         res_low.y = attn_low.y + hs_low.y + (res_low.y + bias_low.y) * mp_scale;
         res_high.x = attn_high.x + hs_high.x + (res_high.x + bias_high.x) * mp_scale;
         res_high.y = attn_high.y + hs_high.y + (res_high.y + bias_high.y) * mp_scale;
 
-        res_half2[0] = __float22half2_rn(res_low);
-        res_half2[1] = __float22half2_rn(res_high);
+        res_half2[0] = conversion::to<T2>(res_low);
+        res_half2[1] = conversion::to<T2>(res_high);
 
         res_fl2_ptr[offset] = res_fl2;
     }
 }
 
 template <typename T>
 void launch_gptj_residual_add(T* residual,
@@ -392,23 +451,57 @@
                                               float*,
                                               float*,
                                               float*,
                                               int,
                                               int,
                                               int,
                                               cudaStream_t);
+
+#ifdef BF16_AVAILABLE
+template void launch_gptj_residual_add<__nv_bfloat16>(__nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      __nv_bfloat16*,
+                                                      int,
+                                                      int,
+                                                      int,
+                                                      cudaStream_t);
+#endif
+
 template void launch_gptj_residual_add<__half>(__half*,
                                                __half*,
                                                __half*,
                                                __half*,
                                                __half*,
                                                int,
                                                int,
                                                int,
                                                cudaStream_t);
+
+#ifdef BF16_AVAILABLE
+template __global__ void gptj_residual_add(__nv_bfloat16* residual,
+                                           const __nv_bfloat16* hidden_state,
+                                           const __nv_bfloat16* attn,
+                                           const __nv_bfloat16* bias,
+                                           const __nv_bfloat16* attn_bias,
+                                           const int total_count,
+                                           const int intermediate_size,
+                                           const float mp_scale);
+#endif
+
+template __global__ void gptj_residual_add(__half* residual,
+                                           const __half* hidden_state,
+                                           const __half* attn,
+                                           const __half* bias,
+                                           const __half* attn_bias,
+                                           const int total_count,
+                                           const int intermediate_size,
+                                           const float mp_scale);
+
 template <typename T>
 __global__ void moe_res_matmul(T* residual, T* coef, T* mlp_out, int seq_len, int hidden_dim)
 {
     constexpr int granularity = 16;
     constexpr int vals_per_access = granularity / sizeof(T);
 
     T* residual_seq = residual + blockIdx.x * hidden_dim;
@@ -451,48 +544,60 @@
 
 template void launch_moe_res_matmul(float* residual,
                                     float* coef,
                                     float* mlp_out,
                                     int seq_len,
                                     int hidden_dim,
                                     cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void launch_moe_res_matmul(__nv_bfloat16* residual,
+                                    __nv_bfloat16* coef,
+                                    __nv_bfloat16* mlp_out,
+                                    int seq_len,
+                                    int hidden_dim,
+                                    cudaStream_t stream);
+#endif
+
 template void launch_moe_res_matmul(__half* residual,
                                     __half* coef,
                                     __half* mlp_out,
                                     int seq_len,
                                     int hidden_dim,
                                     cudaStream_t stream);
 
-__global__ void pad_data_kernel(__half* padded_output,
-                                __half* output,
-                                int head_size,
-                                int padded_head_size)
+template <typename T>
+__global__ void pad_data_kernel(T* padded_output, T* output, int head_size, int padded_head_size)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4* padded_output_cast = reinterpret_cast<float4*>(padded_output);
     float4* output_cast = reinterpret_cast<float4*>(output);
     int bid = blockIdx.x * (blockDim.y) + threadIdx.y;
     int idx = threadIdx.x;
     padded_output_cast += (bid * padded_head_size);
     output_cast += (bid * head_size);
     float4 ZERO;
-    const __half2 zero_h = __float2half2_rn(0.f);
-    __half2* ZERO_h = reinterpret_cast<__half2*>(&ZERO);
+    const T2 zero_h = conversion::to<T2>(0.f);
+    T2* ZERO_h = reinterpret_cast<T2*>(&ZERO);
 #pragma unroll
     for (int i = 0; i < 4; i++) ZERO_h[i] = zero_h;
     if (idx < head_size)
         padded_output_cast[idx] = output_cast[idx];
     else
         padded_output_cast[idx] = ZERO;
 }
+
 __global__ void pad_data_kernel(float* padded_output,
                                 float* output,
                                 int head_size,
                                 int padded_head_size)
 {
 }
+
 template <typename T>
 void pad_data(T* padded_output,
               T* output,
               int bsz,
               int head_size,
               int padded_head_size,
               cudaStream_t stream)
@@ -504,54 +609,81 @@
 }
 template void pad_data(__half* padded_output,
                        __half* output,
                        int bsz,
                        int head_size,
                        int padded_head_size,
                        cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void pad_data(__nv_bfloat16* padded_output,
+                       __nv_bfloat16* output,
+                       int bsz,
+                       int head_size,
+                       int padded_head_size,
+                       cudaStream_t stream);
+#endif
+
 template void pad_data(float* padded_output,
                        float* output,
                        int bsz,
                        int head_size,
                        int padded_head_size,
                        cudaStream_t stream);
 
-__global__ void pad_head_seq_kernel(__half* padded_output,
-                                    __half* output,
+#ifdef BF16_AVAILABLE
+template __global__ void pad_data_kernel(__nv_bfloat16* padded_output,
+                                         __nv_bfloat16* output,
+                                         int head_size,
+                                         int padded_head_size);
+#endif
+
+template __global__ void pad_data_kernel(__half* padded_output,
+                                         __half* output,
+                                         int head_size,
+                                         int padded_head_size);
+
+template <typename T>
+__global__ void pad_head_seq_kernel(T* padded_output,
+                                    T* output,
                                     int seq_len,
                                     int padded_seq_len,
                                     int head_size,
                                     int padded_head_size)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4* padded_output_cast = reinterpret_cast<float4*>(padded_output);
     float4* output_cast = reinterpret_cast<float4*>(output);
     int bsz = blockIdx.x;
     int bid = blockIdx.y * (blockDim.y) + threadIdx.y;
     int idx = threadIdx.x;
     padded_output_cast += (bsz * padded_seq_len + bid) * padded_head_size;
     output_cast += (bsz * seq_len + bid) * head_size;
     float4 ZERO;
-    const __half2 zero_h = __float2half2_rn(0.f);
-    __half2* ZERO_h = reinterpret_cast<__half2*>(&ZERO);
+    const T2 zero_h = conversion::to<T2>(0.f);
+    T2* ZERO_h = reinterpret_cast<T2*>(&ZERO);
 #pragma unroll
     for (int i = 0; i < 4; i++) ZERO_h[i] = zero_h;
 
     if (idx < head_size && bid < seq_len)
         padded_output_cast[idx] = output_cast[idx];
     else
         padded_output_cast[idx] = ZERO;
 }
+
 __global__ void pad_head_seq_kernel(float* padded_output,
                                     float* output,
                                     int seq_len,
                                     int padded_seq_len,
                                     int head_size,
                                     int padded_head_size)
 {
 }
+
 template <typename T>
 void pad_head_seq(T* padded_output,
                   T* output,
                   int bsz,
                   int seq_len,
                   int padded_seq_len,
                   int head_size,
@@ -559,22 +691,35 @@
                   cudaStream_t stream)
 {
     dim3 grid_dim(bsz, padded_seq_len / 16);
     dim3 block_dim(padded_head_size / 8, 16);
     pad_head_seq_kernel<<<grid_dim, block_dim, 0, stream>>>(
         padded_output, output, seq_len, padded_seq_len, head_size / 8, padded_head_size / 8);
 }
+
 template void pad_head_seq(__half* padded_output,
                            __half* output,
                            int bsz,
                            int seq_len,
                            int padded_seq_len,
                            int head_size,
                            int padded_head_size,
                            cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void pad_head_seq(__nv_bfloat16* padded_output,
+                           __nv_bfloat16* output,
+                           int bsz,
+                           int seq_len,
+                           int padded_seq_len,
+                           int head_size,
+                           int padded_head_size,
+                           cudaStream_t stream);
+#endif
+
 template void pad_head_seq(float* padded_output,
                            float* output,
                            int bsz,
                            int seq_len,
                            int padded_seq_len,
                            int head_size,
                            int padded_head_size,
@@ -677,8 +822,16 @@
 
 template void launch_fused_bias_geglu(__half*,
                                       const __half*,
                                       const __half*,
                                       int,
                                       int,
                                       cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_fused_bias_geglu(__nv_bfloat16*,
+                                      const __nv_bfloat16*,
+                                      const __nv_bfloat16*,
+                                      int,
+                                      int,
+                                      cudaStream_t);
+#endif
 template void launch_fused_bias_geglu(float*, const float*, const float*, int, int, cudaStream_t);
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,24 @@
                               const __half*,
                               const __half*,
                               const __half*,
                               float,
                               int,
                               int,
                               cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_fused_ln(__nv_bfloat16*,
+                              const __nv_bfloat16*,
+                              const __nv_bfloat16*,
+                              const __nv_bfloat16*,
+                              float,
+                              int,
+                              int,
+                              cudaStream_t);
+#endif
 template void
 launch_fused_ln(float*, const float*, const float*, const float*, float, int, int, cudaStream_t);
 
 /*
 Fused resiual + bias + layer norm implementation. Assumes elems_per_row % 8
 is equal to 0.
 
@@ -489,14 +499,27 @@
                                        const __half*,
                                        const __half*,
                                        float,
                                        int,
                                        int,
                                        cudaStream_t);
 
+#ifdef BF16_AVAILABLE
+template void launch_fused_residual_ln(__nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       const __nv_bfloat16*,
+                                       float,
+                                       int,
+                                       int,
+                                       cudaStream_t);
+#endif
+
 template void launch_fused_residual_ln(float*,
                                        const float*,
                                        const float*,
                                        const float*,
                                        const float*,
                                        const float*,
                                        float,
@@ -513,14 +536,28 @@
                                                         const __half*,
                                                         const __half*,
                                                         float,
                                                         int,
                                                         int,
                                                         cudaStream_t);
 
+#ifdef BF16_AVAILABLE
+template void launch_fused_residual_ln_store_pre_ln_res(__nv_bfloat16*,
+                                                        __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        const __nv_bfloat16*,
+                                                        float,
+                                                        int,
+                                                        int,
+                                                        cudaStream_t);
+#endif
+
 template void launch_fused_residual_ln_store_pre_ln_res(float*,
                                                         float*,
                                                         const float*,
                                                         const float*,
                                                         const float*,
                                                         const float*,
                                                         const float*,
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1740,87 +1740,75 @@
 
 void ds_release_workspace() { InferenceContext::Instance().release_workspace(); }
 
 bool ds_retake_workspace() { return InferenceContext::Instance().retake_workspace(); }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
-    m.def("softmax_fp32", &ds_softmax<float>, "DeepSpeed SoftMax with fp32 (CUDA)");
-    m.def("softmax_fp16", &ds_softmax<__half>, "DeepSpeed SoftMax with fp16 (CUDA)");
-    m.def(
-        "softmax_context_fp32", &ds_softmax_context<float>, "DeepSpeed attention with fp32 (CUDA)");
-    m.def("softmax_context_fp16",
-          &ds_softmax_context<__half>,
-          "DeepSpeed attention with fp16 (CUDA)");
     m.def("softmax_context_int8",
           &ds_softmax_context1<__half>,
           "DeepSpeed attention with int8 (CUDA)");
-    m.def("bias_gelu_fp32", &ds_bias_gelu<float>, "DeepSpeed Gelu with fp32 (CUDA)");
-    m.def("bias_gelu_fp16", &ds_bias_gelu<__half>, "DeepSpeed Gelu with fp16 (CUDA)");
     m.def("bias_geglu", &ds_bias_geglu, "DeepSpeed Bias GEGLU (CUDA)");
-    m.def("bias_add_fp32", &ds_bias_add<float>, "DeepSpeed Bias Add with fp32 (CUDA)");
-    m.def("bias_add_fp16", &ds_bias_add<__half>, "DeepSpeed Gelu with fp16 (CUDA)");
-    m.def("bias_relu_fp32", &ds_bias_relu<float>, "DeepSpeed ReLU with fp32 (CUDA)");
-    m.def("bias_relu_fp16", &ds_bias_relu<__half>, "DeepSpeed ReLU with fp16 (CUDA)");
-    m.def("bias_residual_fp32",
-          &ds_bias_residual<float>,
-          "DeepSpeed residual-bias add with fp32 (CUDA)");
-    m.def("bias_residual_fp16",
-          &ds_bias_residual<__half>,
-          "DeepSpeed residual-bias add with fp16 (CUDA)");
     m.def("layer_norm", &ds_layer_norm, "DeepSpeed layer norm (CUDA)");
     m.def(
         "_layer_norm_residual", &ds_layer_norm_residual, "DeepSpeed layer norm + residual (CUDA)");
     m.def("layer_norm_residual_store_pre_ln_res",
           &ds_layer_norm_residual_store_pre_ln_res,
           "DeepSpeed layer norm + store pre Layernorm residual (CUDA)");
-    m.def("qkv_gemm_fp32", &ds_qkv_gemm<float>, "DeepSpeed qkv gemm with fp32 (CUDA)");
-    m.def("qkv_gemm_fp16", &ds_qkv_gemm<__half>, "DeepSpeed qkv gemm with fp16 (CUDA)");
     m.def("qkv_gemm_int8", &ds_qkv_gemm_int8<__half>, "DeepSpeed qkv gemm with int8 (CUDA)");
-    m.def("mlp_gemm_fp32", &ds_mlp_gemm<float>, "DeepSpeed mlp with fp32 (CUDA)");
-    m.def("mlp_gemm_fp16", &ds_mlp_gemm<__half>, "DeepSpeed mlp with fp16 (CUDA)");
     m.def("mlp_gemm_int8", &ds_mlp_gemm_int8<__half>, "DeepSpeed mlp with int8 (CUDA)");
-    m.def("vector_matmul_fp32", &ds_vector_matmul<float>, "DeepSpeed vector-MM with fp32 (CUDA)");
-    m.def("vector_matmul_fp16", &ds_vector_matmul<__half>, "DeepSpeed vector-MM with fp16 (CUDA)");
     m.def("vector_matmul_int8",
           &ds_vector_matmul_int8<__half>,
           "DeepSpeed vector-MM with int8 (CUDA)");
-    m.def("linear_layer_fp32", &ds_linear_layer<float>, "DeepSpeed linear_layer with fp32 (CUDA)");
-    m.def("linear_layer_fp16", &ds_linear_layer<__half>, "DeepSpeed linear_layer with fp16 (CUDA)");
     m.def("linear_layer_int8",
           &ds_linear_layer_int8<__half>,
           "DeepSpeed linear_layer with int8 (CUDA)");
-    m.def("fused_gemm_gelu_fp32", &fused_gemm_gelu<float>, "DeepSpeed mlp with fp32 (CUDA)");
-    m.def("fused_gemm_gelu_fp16", &fused_gemm_gelu<__half>, "DeepSpeed mlp with fp16 (CUDA)");
-    m.def("residual_add_bias_fp32",
-          &residual_add_bias<float>,
-          "DeepSpeed residual add with fp32 (CUDA)");
-    m.def("residual_add_bias_fp16",
-          &residual_add_bias<__half>,
-          "DeepSpeed residual add with fp16 (CUDA)");
     m.def("apply_rotary_pos_emb", &apply_rotary_pos_emb, "DeepSpeed mlp with fp16 (CUDA)");
-    m.def("einsum_sec_sm_ecm_fp32",
-          &einsum_sec_sm_ecm<float>,
-          "DeepSpeed vector-MM with fp32 (CUDA)");
-
-    m.def("einsum_sec_sm_ecm_fp16",
-          &einsum_sec_sm_ecm<__half>,
-          "DeepSpeed vector-MM with fp16 (CUDA)");
     m.def("moe_res_matmul", &moe_res_matmul, "DeepSpeed moe residual matmul (CUDA)");
-    m.def("add_padding_fp32", &add_padding<float>, "DeepSpeed residual add with fp32 (CUDA)");
-    m.def("add_padding_fp16", &add_padding<__half>, "DeepSpeed residual add with fp16 (CUDA)");
-    m.def("pad_transform_fp32",
-          &padd_add_transform<float>,
-          "DeepSpeed residual add with fp32 (CUDA)");
-    m.def("pad_transform_fp16",
-          &padd_add_transform<__half>,
-          "DeepSpeed residual add with fp16 (CUDA)");
-    m.def("allocate_workspace_fp32",
-          &allocate_workspace<float>,
-          "DeepSpeed memory allocation for GPT inference with fp32 (CUDA)");
-    m.def("allocate_workspace_fp16",
-          &allocate_workspace<__half>,
-          "DeepSpeed memory allocation for GPT inference with fp16 (CUDA)");
     m.def("reset_cache", &reset_cache, "Reset Cache for generation tasks");
     m.def("release_workspace", &ds_release_workspace, "DeepSpeed Release Workspace");
     m.def("retake_workspace", &ds_retake_workspace, "DeepSpeed Retake Workspace");
+
+#define DEF_OPS(_name, _dtype)                                                                    \
+    m.def("softmax_" #_name, &ds_softmax<_dtype>, "DeepSpeed SoftMax with " #_name " (CUDA)");    \
+    m.def("softmax_context_" #_name,                                                              \
+          &ds_softmax_context<_dtype>,                                                            \
+          "DeepSpeed attention with _name (CUDA)");                                               \
+    m.def("bias_gelu_" #_name, &ds_bias_gelu<_dtype>, "DeepSpeed Gelu with " #_name " (CUDA)");   \
+    m.def("bias_add_" #_name, &ds_bias_add<_dtype>, "DeepSpeed Bias Add with " #_name " (CUDA)"); \
+    m.def("bias_relu_" #_name, &ds_bias_relu<_dtype>, "DeepSpeed ReLU with " #_name " (CUDA)");   \
+    m.def("bias_residual_" #_name,                                                                \
+          &ds_bias_residual<_dtype>,                                                              \
+          "DeepSpeed residual-bias add with " #_name " (CUDA)");                                  \
+    m.def("qkv_gemm_" #_name, &ds_qkv_gemm<_dtype>, "DeepSpeed qkv gemm with " #_name " (CUDA)"); \
+    m.def("mlp_gemm_" #_name, &ds_mlp_gemm<_dtype>, "DeepSpeed mlp with " #_name " (CUDA)");      \
+    m.def("vector_matmul_" #_name,                                                                \
+          &ds_vector_matmul<_dtype>,                                                              \
+          "DeepSpeed vector-MM with " #_name " (CUDA)");                                          \
+    m.def("linear_layer_" #_name,                                                                 \
+          &ds_linear_layer<_dtype>,                                                               \
+          "DeepSpeed linear_layer with " #_name " (CUDA)");                                       \
+    m.def("fused_gemm_gelu_" #_name,                                                              \
+          &fused_gemm_gelu<_dtype>,                                                               \
+          "DeepSpeed mlp with " #_name " (CUDA)");                                                \
+    m.def("residual_add_bias_" #_name,                                                            \
+          &residual_add_bias<_dtype>,                                                             \
+          "DeepSpeed residual add with " #_name " (CUDA)");                                       \
+    m.def("einsum_sec_sm_ecm_" #_name,                                                            \
+          &einsum_sec_sm_ecm<_dtype>,                                                             \
+          "DeepSpeed vector-MM with " #_name " (CUDA)");                                          \
+    m.def("add_padding_" #_name,                                                                  \
+          &add_padding<_dtype>,                                                                   \
+          "DeepSpeed residual add with " #_name " (CUDA)");                                       \
+    m.def("pad_transform_" #_name,                                                                \
+          &padd_add_transform<_dtype>,                                                            \
+          "DeepSpeed residual add with " #_name " (CUDA)");                                       \
+    m.def("allocate_workspace_" #_name,                                                           \
+          &allocate_workspace<_dtype>,                                                            \
+          "DeepSpeed memory allocation for GPT inference with " #_name " (CUDA)")
+
+    DEF_OPS(fp32, float);
+    DEF_OPS(fp16, __half);
+#ifdef BF16_AVAILABLE
+    DEF_OPS(bf16, __nv_bfloat16);
+#endif
 }
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu`

 * *Files 7% similar despite different names*

```diff
@@ -57,8 +57,15 @@
     dim3 grid_dims((total_count + elems_per_block - 1) / elems_per_block);
 
     fused_bias_relu<<<grid_dims, block_dims, 0, stream>>>(
         input, bias, total_count, intermediate_size);
 }
 
 template void launch_bias_relu<float>(float*, const float*, int, int, cudaStream_t);
+#ifdef BF16_AVAILABLE
+template void launch_bias_relu<__nv_bfloat16>(__nv_bfloat16*,
+                                              const __nv_bfloat16*,
+                                              int,
+                                              int,
+                                              cudaStream_t);
+#endif
 template void launch_bias_relu<__half>(__half*, const __half*, int, int, cudaStream_t);
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 // Copyright (c) Microsoft Corporation.
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
 #include <limits>
+#include "conversion_utils.h"
 #include "inference_cuda_layers.h"
 
 #ifndef __HIP_PLATFORM_HCC__
 #include <cuda_profiler_api.h>
 #endif
 #include <cstdio>
 #include <cstdlib>
@@ -26,18 +27,18 @@
     throw std::runtime_error("CUDA ERROR!!!\n");
 }
 
 #define CUDA_CHECK_ERROR() CheckCudaErrorAux(__FILE__, __LINE__)
 
 namespace cg = cooperative_groups;
 
-template <int iterations>
-__global__ void attn_softmax_v2(__half* vals,
-                                __half* mask,
-                                __half* alibi,
+template <typename T, int iterations>
+__global__ void attn_softmax_v2(T* vals,
+                                T* mask,
+                                T* alibi,
                                 float layer_scale,
                                 bool triangular,
                                 bool recompute,
                                 bool local_attention,
                                 int window_size,
                                 int total_count,
                                 int heads,
@@ -49,15 +50,15 @@
                                 int reduceWidth)
 {
     cg::thread_block b = cg::this_thread_block();
     cg::thread_block_tile<WARP_SIZE> g = cg::tiled_partition<WARP_SIZE>(b);
 
     float2 low_data[MAX_REG_SIZE];
     float2 high_data[MAX_REG_SIZE];
-    const __half zero_h = __float2half(0.f);
+    const T zero_h = conversion::to<T>(0.f);
 
     int wid = threadIdx.x >> 5;
     int lane = threadIdx.x & 0x1f;
     int warp_num = blockDim.x >> 5;
 
     int reduce_blocks = reduceWidth >> 5;
     int seq_lane = threadIdx.x % reduceWidth;
@@ -97,81 +98,95 @@
                                 (!triangular || ((data_id + reduceWidth * 2) <= seq_id)) &&
                                 ((data_id + reduceWidth * 2) > window_stride);
             bool high_y_check = check && ((data_id + reduceWidth * 3) < sequence_length) &&
                                 (!triangular || ((data_id + reduceWidth * 3) <= seq_id)) &&
                                 ((data_id + reduceWidth * 3) > window_stride);
 
             if (mask && alibi) {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale +
-                                                  (__half2float(alibi[data_id + alibi_offset])) +
-                                                  (__half2float(mask[data_id + mask_offset]))
-                                            : minus_infinity;
+                low_data[i].x = low_x_check
+                                    ? conversion::to<float>(vals[data_id]) * layer_scale +
+                                          (conversion::to<float>(alibi[data_id + alibi_offset])) +
+                                          (conversion::to<float>(mask[data_id + mask_offset]))
+                                    : minus_infinity;
                 low_data[i].y =
-                    low_y_check ? __half2float(vals[data_id + reduceWidth]) * layer_scale +
-                                      (__half2float(alibi[data_id + alibi_offset + reduceWidth])) +
-                                      (__half2float(mask[data_id + mask_offset + reduceWidth]))
-                                : minus_infinity;
+                    low_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale +
+                              (conversion::to<float>(alibi[data_id + alibi_offset + reduceWidth])) +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth]))
+                        : minus_infinity;
                 high_data[i].x =
                     high_x_check
-                        ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 2])) +
-                              (__half2float(mask[data_id + mask_offset + reduceWidth * 2]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 2])) +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 2]))
                         : minus_infinity;
                 high_data[i].y =
                     high_y_check
-                        ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 3])) +
-                              (__half2float(mask[data_id + mask_offset + reduceWidth * 3]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 3])) +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 3]))
                         : minus_infinity;
             } else if (mask) {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale +
-                                                  (__half2float(mask[data_id + mask_offset]))
-                                            : minus_infinity;
-                low_data[i].y = low_y_check
-                                    ? __half2float(vals[data_id + reduceWidth]) * layer_scale +
-                                          (__half2float(mask[data_id + mask_offset + reduceWidth]))
+                low_data[i].x = low_x_check
+                                    ? conversion::to<float>(vals[data_id]) * layer_scale +
+                                          (conversion::to<float>(mask[data_id + mask_offset]))
                                     : minus_infinity;
+                low_data[i].y =
+                    low_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth]))
+                        : minus_infinity;
                 high_data[i].x =
-                    high_x_check ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale +
-                                       (__half2float(mask[data_id + mask_offset + reduceWidth * 2]))
-                                 : minus_infinity;
+                    high_x_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 2]))
+                        : minus_infinity;
                 high_data[i].y =
-                    high_y_check ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale +
-                                       (__half2float(mask[data_id + mask_offset + reduceWidth * 3]))
-                                 : minus_infinity;
+                    high_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale +
+                              (conversion::to<float>(mask[data_id + mask_offset + reduceWidth * 3]))
+                        : minus_infinity;
             } else if (alibi) {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale +
-                                                  (__half2float(alibi[data_id + alibi_offset]))
-                                            : minus_infinity;
+                low_data[i].x = low_x_check
+                                    ? conversion::to<float>(vals[data_id]) * layer_scale +
+                                          (conversion::to<float>(alibi[data_id + alibi_offset]))
+                                    : minus_infinity;
                 low_data[i].y =
-                    low_y_check ? __half2float(vals[data_id + reduceWidth]) * layer_scale +
-                                      (__half2float(alibi[data_id + alibi_offset + reduceWidth]))
-                                : minus_infinity;
+                    low_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale +
+                              (conversion::to<float>(alibi[data_id + alibi_offset + reduceWidth]))
+                        : minus_infinity;
                 high_data[i].x =
                     high_x_check
-                        ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 2]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 2]))
                         : minus_infinity;
                 high_data[i].y =
                     high_y_check
-                        ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale +
-                              (__half2float(alibi[data_id + alibi_offset + reduceWidth * 3]))
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale +
+                              (conversion::to<float>(
+                                  alibi[data_id + alibi_offset + reduceWidth * 3]))
                         : minus_infinity;
             } else {
-                low_data[i].x = low_x_check ? __half2float(vals[data_id]) * layer_scale
+                low_data[i].x = low_x_check ? conversion::to<float>(vals[data_id]) * layer_scale
                                             : minus_infinity;
-                low_data[i].y = low_y_check
-                                    ? __half2float(vals[data_id + reduceWidth]) * layer_scale
-                                    : minus_infinity;
-                high_data[i].x = high_x_check
-                                     ? __half2float(vals[data_id + reduceWidth * 2]) * layer_scale
-                                     : minus_infinity;
-                high_data[i].y = high_y_check
-                                     ? __half2float(vals[data_id + reduceWidth * 3]) * layer_scale
-                                     : minus_infinity;
+                low_data[i].y =
+                    low_y_check ? conversion::to<float>(vals[data_id + reduceWidth]) * layer_scale
+                                : minus_infinity;
+                high_data[i].x =
+                    high_x_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 2]) * layer_scale
+                        : minus_infinity;
+                high_data[i].y =
+                    high_y_check
+                        ? conversion::to<float>(vals[data_id + reduceWidth * 3]) * layer_scale
+                        : minus_infinity;
             }
 
             // if(lane == 0) printf("%f , %d, %d \n", low_data[i].x, data_id, seq_id);
             max_val = (low_data[i].x > max_val ? low_data[i].x : max_val);
             max_val = (low_data[i].y > max_val ? low_data[i].y : max_val);
             max_val = (high_data[i].x > max_val ? high_data[i].x : max_val);
             max_val = (high_data[i].y > max_val ? high_data[i].y : max_val);
@@ -221,21 +236,21 @@
 
             sum = g.shfl(sum, threadIdx.x / WARP_SIZE);
         }
         sum += 1e-6;
         for (int i = 0; i < iterations; i++) {
             int data_id = i * (reduceWidth << 2) + (seq_lane);
             if (data_id < sequence_length) {
-                vals[data_id] = __float2half(low_data[i].x / sum);
+                vals[data_id] = conversion::to<T>(low_data[i].x / sum);
                 if ((data_id + reduceWidth) < sequence_length)
-                    vals[data_id + reduceWidth] = __float2half(low_data[i].y / sum);
+                    vals[data_id + reduceWidth] = conversion::to<T>(low_data[i].y / sum);
                 if ((data_id + reduceWidth * 2) < sequence_length)
-                    vals[data_id + reduceWidth * 2] = __float2half(high_data[i].x / sum);
+                    vals[data_id + reduceWidth * 2] = conversion::to<T>(high_data[i].x / sum);
                 if ((data_id + reduceWidth * 3) < sequence_length)
-                    vals[data_id + reduceWidth * 3] = __float2half(high_data[i].y / sum);
+                    vals[data_id + reduceWidth * 3] = conversion::to<T>(high_data[i].y / sum);
             }
         }
     }
 }
 
 template <int iterations>
 __global__ void attn_softmax_v2(float* vals,
@@ -385,31 +400,31 @@
                 if ((data_id + reduceWidth * 3) < sequence_length)
                     vals[data_id + reduceWidth * 3] = data[i].w / sum;
             }
         }
     }
 }
 
-#define LAUNCH_ATTN_SOFTMAX_V2(iterations)                                   \
-    attn_softmax_v2<iterations><<<grid, block, 0, stream>>>(vals,            \
-                                                            mask,            \
-                                                            alibi,           \
-                                                            layer_scale,     \
-                                                            triangular,      \
-                                                            recompute,       \
-                                                            local_attention, \
-                                                            window_size,     \
-                                                            total_count,     \
-                                                            heads,           \
-                                                            sequence_length, \
-                                                            num_seq,         \
-                                                            head_offset,     \
-                                                            mask_stride,     \
-                                                            mp_size,         \
-                                                            reduce_width);
+#define LAUNCH_ATTN_SOFTMAX_V2(iterations)                                      \
+    attn_softmax_v2<T, iterations><<<grid, block, 0, stream>>>(vals,            \
+                                                               mask,            \
+                                                               alibi,           \
+                                                               layer_scale,     \
+                                                               triangular,      \
+                                                               recompute,       \
+                                                               local_attention, \
+                                                               window_size,     \
+                                                               total_count,     \
+                                                               heads,           \
+                                                               sequence_length, \
+                                                               num_seq,         \
+                                                               head_offset,     \
+                                                               mask_stride,     \
+                                                               mp_size,         \
+                                                               reduce_width);
 
 template <typename T>
 void launch_attn_softmax_v2(T* vals,
                             T* mask,
                             T* alibi,
                             float layer_scale,
                             bool triangular,
@@ -484,14 +499,34 @@
                                      int heads,
                                      int num_seq,
                                      int sequence_length,
                                      int head_offset,
                                      int mask_stride,
                                      int mp_size,
                                      cudaStream_t stream);
+
+#ifdef BF16_AVAILABLE
+template void launch_attn_softmax_v2(__nv_bfloat16* vals,
+                                     __nv_bfloat16* mask,
+                                     __nv_bfloat16* alibi,
+                                     float layer_scale,
+                                     bool triangular,
+                                     bool recompute,
+                                     bool local_attention,
+                                     int window_size,
+                                     int batch_size,
+                                     int heads,
+                                     int num_seq,
+                                     int sequence_length,
+                                     int head_offset,
+                                     int mask_stride,
+                                     int mp_size,
+                                     cudaStream_t stream);
+#endif
+
 template void launch_attn_softmax_v2(__half* vals,
                                      __half* mask,
                                      __half* alibi,
                                      float layer_scale,
                                      bool triangular,
                                      bool recompute,
                                      bool local_attention,
@@ -500,7 +535,57 @@
                                      int heads,
                                      int num_seq,
                                      int sequence_length,
                                      int head_offset,
                                      int mask_stride,
                                      int mp_size,
                                      cudaStream_t stream);
+
+#define DEF_ATTN_SOFTMAX_V2_HALF(_iter)                                           \
+    template __global__ void attn_softmax_v2<__half, _iter>(__half * vals,        \
+                                                            __half * mask,        \
+                                                            __half * alibi,       \
+                                                            float layer_scale,    \
+                                                            bool triangular,      \
+                                                            bool recompute,       \
+                                                            bool local_attention, \
+                                                            int window_size,      \
+                                                            int total_count,      \
+                                                            int heads,            \
+                                                            int sequence_length,  \
+                                                            int num_seq,          \
+                                                            int head_offset,      \
+                                                            int mask_stride,      \
+                                                            int mp_size,          \
+                                                            int reduceWidth)
+
+#define DEF_ATTN_SOFTMAX_V2_BF16(_iter)                                                   \
+    template __global__ void attn_softmax_v2<__nv_bfloat16, _iter>(__nv_bfloat16 * vals,  \
+                                                                   __nv_bfloat16 * mask,  \
+                                                                   __nv_bfloat16 * alibi, \
+                                                                   float layer_scale,     \
+                                                                   bool triangular,       \
+                                                                   bool recompute,        \
+                                                                   bool local_attention,  \
+                                                                   int window_size,       \
+                                                                   int total_count,       \
+                                                                   int heads,             \
+                                                                   int sequence_length,   \
+                                                                   int num_seq,           \
+                                                                   int head_offset,       \
+                                                                   int mask_stride,       \
+                                                                   int mp_size,           \
+                                                                   int reduceWidth)
+
+#define FOREACH_ITERATIONS(cb) \
+    cb(1);                     \
+    cb(2);                     \
+    cb(4);                     \
+    cb(8);                     \
+    cb(16);                    \
+    cb(32);                    \
+    cb(64)
+
+FOREACH_ITERATIONS(DEF_ATTN_SOFTMAX_V2_HALF);
+#ifdef BF16_AVAILABLE
+FOREACH_ITERATIONS(DEF_ATTN_SOFTMAX_V2_BF16);
+#endif
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 // SPDX-License-Identifier: Apache-2.0
 
 // DeepSpeed Team
 
 #ifndef __HIP_PLATFORM_HCC__
 #include <cuda_profiler_api.h>
 #endif
+#include "conversion_utils.h"
 #include "inference_cuda_layers.h"
 namespace cg = cooperative_groups;
 
+// only used to avoid compilation error due to lack of definition.
+#ifndef BF16_AVAILABLE
+using __nv_bfloat162 = __half2;
+#endif
+
 // Bias add
 
 __global__ void bias_add_transform_0213(float* output,
                                         float* k_cache,
                                         float* v_cache,
                                         const float* vals,
                                         const float* bias,
@@ -71,30 +77,33 @@
     } else
         output_vec[d3] = inputs;
 }
 
 #define ATTN_H 3
 #define MAX_SEQ_LINE 10
 
-__global__ void bias_add_transform_0213(__half* output,  // q
-                                        __half* k_cache,
-                                        __half* v_cache,
-                                        const __half* vals,  // qkv
-                                        const __half* bias,
+template <typename T>
+__global__ void bias_add_transform_0213(T* output,  // q
+                                        T* k_cache,
+                                        T* v_cache,
+                                        const T* vals,  // qkv
+                                        const T* bias,
                                         int hidden_dim,
                                         int seq_length,
                                         unsigned seq_offset,
                                         int all_tokens,
                                         int heads,
                                         int rotary_dim,
                                         bool rotate_half,
                                         bool rotate_every_two,
                                         int head_ext,
                                         int max_out_tokens)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     unsigned half_dim = (rotary_dim << 3) >> 1;
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
     int d0 = blockIdx.x;                                                  // Batch
     int d1 = blockIdx.y;                                                  // Sequence ID (0-127)
@@ -104,16 +113,16 @@
 
     int d2_out_stride = d2_stride * (cnt == 0 ? seq_length : max_out_tokens);
     int d0_out_stride = hidden_dim * (cnt == 0 ? seq_length : max_out_tokens);
 
     float4 vals_arr;
     float4 output_arr;
 
-    __half2* vals_half = reinterpret_cast<__half2*>(&vals_arr);
-    __half2* output_half = reinterpret_cast<__half2*>(&output_arr);
+    T2* vals_half = reinterpret_cast<T2*>(&vals_arr);
+    T2* output_half = reinterpret_cast<T2*>(&output_arr);
 
     const float4* vals_vec = reinterpret_cast<const float4*>(vals);
     float4* output_vec =
         reinterpret_cast<float4*>(cnt == 0 ? output : (cnt == 1 ? k_cache : v_cache));
 
     vals_vec += (d0 * d0_stride * (gridDim.z / head_ext));
     vals_vec += (d1 * d1_stride * (gridDim.z / head_ext));
@@ -125,25 +134,27 @@
     output_vec += (d2 * d2_out_stride);
 
     unsigned seq_id = d1 + seq_offset;
 
     int lane = d3 & 0x1f;
     if (cnt < 2 && rotary_dim > 0 && d3 < rotary_dim) {
         float4 q = vals_vec[d3];
-        __half2* q_h = reinterpret_cast<__half2*>(&q);
+        T2* q_h = reinterpret_cast<T2*>(&q);
         if (rotate_every_two) {
 #pragma unroll
             for (int o = 0; o < 4; o++) {
                 float inv_freq = (float)(((d3 << 2) + o) * 2) / (float)(rotary_dim << 3);
                 inv_freq = 1.0 / powf(10000.0, inv_freq) * (float)seq_id;
                 float q_data[2];
-                q_data[0] = (float)q_h[o].x;
-                q_data[1] = (float)q_h[o].y;
-                q_h[o].x = (__half)(-1.0 * q_data[1] * sinf(inv_freq) + q_data[0] * cosf(inv_freq));
-                q_h[o].y = (__half)(q_data[0] * sinf(inv_freq) + q_data[1] * cosf(inv_freq));
+                q_data[0] = conversion::to<float>(q_h[o].x);
+                q_data[1] = conversion::to<float>(q_h[o].y);
+                q_h[o].x = conversion::to<T>(-1.0 * q_data[1] * sinf(inv_freq) +
+                                             q_data[0] * cosf(inv_freq));
+                q_h[o].y =
+                    conversion::to<T>(q_data[0] * sinf(inv_freq) + q_data[1] * cosf(inv_freq));
             }
         }
         output_vec[d3] = q;
     } else
         output_vec[d3] = vals_vec[d3];
 }
 
@@ -184,50 +195,33 @@
                                                                 heads,
                                                                 rotary_dim >> 2,
                                                                 rotate_half,
                                                                 rotate_every_two,
                                                                 head_ext,
                                                                 max_out_tokens);
 }
+
 template <typename T>
-void launch_bias_add_transform_0213(T* outputs,
-                                    T* vals,
-                                    T* vals1,
-                                    const T* vals2,
+void launch_bias_add_transform_0213(T* output,
+                                    T* k_cache,
+                                    T* v_cache,
+                                    const T* vals,
                                     const T* bias,
                                     int batch_size,
                                     int seq_length,
                                     unsigned seq_offset,
-                                    int seq_length1,
+                                    int all_tokens,
                                     int hidden_dim,
                                     int heads,
                                     int rotary_dim,
                                     bool rotate_half,
                                     bool rotate_every_two,
                                     cudaStream_t stream,
                                     int trans_count,
-                                    int max_out_tokens);
-template <>
-void launch_bias_add_transform_0213<__half>(__half* output,
-                                            __half* k_cache,
-                                            __half* v_cache,
-                                            const __half* vals,
-                                            const __half* bias,
-                                            int batch_size,
-                                            int seq_length,
-                                            unsigned seq_offset,
-                                            int all_tokens,
-                                            int hidden_dim,
-                                            int heads,
-                                            int rotary_dim,
-                                            bool rotate_half,
-                                            bool rotate_every_two,
-                                            cudaStream_t stream,
-                                            int trans_count,
-                                            int max_out_tokens)
+                                    int max_out_tokens)
 {
     hidden_dim >>= 3;
     int head_ext = 1;  // (hidden_dim - 1) / MAX_THREADS + 1;
     dim3 block_dim(hidden_dim / heads, (heads / head_ext));
     dim3 grid_dim(batch_size, seq_length, (trans_count * head_ext));
     bias_add_transform_0213<<<grid_dim, block_dim, 0, stream>>>(output,
                                                                 k_cache,
@@ -242,37 +236,78 @@
                                                                 rotary_dim >> 3,
                                                                 rotate_half,
                                                                 rotate_every_two,
                                                                 head_ext,
                                                                 max_out_tokens);
 }
 
+#ifdef BF16_AVAILABLE
+template void launch_bias_add_transform_0213(__nv_bfloat16* output,
+                                             __nv_bfloat16* k_cache,
+                                             __nv_bfloat16* v_cache,
+                                             const __nv_bfloat16* vals,
+                                             const __nv_bfloat16* bias,
+                                             int batch_size,
+                                             int seq_length,
+                                             unsigned seq_offset,
+                                             int all_tokens,
+                                             int hidden_dim,
+                                             int heads,
+                                             int rotary_dim,
+                                             bool rotate_half,
+                                             bool rotate_every_two,
+                                             cudaStream_t stream,
+                                             int trans_count,
+                                             int max_out_tokens);
+#endif
+
+template void launch_bias_add_transform_0213(__half* output,
+                                             __half* k_cache,
+                                             __half* v_cache,
+                                             const __half* vals,
+                                             const __half* bias,
+                                             int batch_size,
+                                             int seq_length,
+                                             unsigned seq_offset,
+                                             int all_tokens,
+                                             int hidden_dim,
+                                             int heads,
+                                             int rotary_dim,
+                                             bool rotate_half,
+                                             bool rotate_every_two,
+                                             cudaStream_t stream,
+                                             int trans_count,
+                                             int max_out_tokens);
+
 // Bias add
 
 __global__ void pad_add_transform_0213(float* output,
                                        const float* vals,
                                        int hidden_dim,
                                        int seq_length,
                                        int padded_seq_len,
                                        int heads,
                                        int padded_head_size)
 {
 }
 
-__global__ void pad_add_transform_0213(__half* output,
-                                       const __half* vals,
+template <typename T>
+__global__ void pad_add_transform_0213(T* output,
+                                       const T* vals,
                                        int hidden_dim,
                                        int seq_length,
                                        int padded_seq_len,
                                        int heads,
                                        int padded_head_size)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     float4 ZERO;
-    const __half2 zero_h = __float2half2_rn(0.f);
-    __half2* ZERO_h = reinterpret_cast<__half2*>(&ZERO);
+    const T2 zero_h = conversion::to<T2>(0.f);
+    T2* ZERO_h = reinterpret_cast<T2*>(&ZERO);
 #pragma unroll
     for (int i = 0; i < 4; i++) ZERO_h[i] = zero_h;
 
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
@@ -297,56 +332,68 @@
 
     if (d3 < d2_stride && d1 < seq_length)
         output_vec[d3] = vals_vec[d3];
     else
         output_vec[d3] = ZERO;
 }
 
-template <typename T>
-void launch_pad_add_transform_0213(T* output,
-                                   const T* vals,
-                                   int batch_size,
-                                   int hidden_dim,
-                                   int seq_length,
-                                   int padded_seq_len,
-                                   int heads,
-                                   int padded_head_size,
-                                   cudaStream_t stream);
-
 // [B S C*H] - > C * [B A S N]
 template <>
 void launch_pad_add_transform_0213<float>(float* output,
                                           const float* vals,
                                           int batch_size,
                                           int hidden_dim,
                                           int seq_length,
                                           int padded_seq_len,
                                           int heads,
                                           int padded_head_size,
                                           cudaStream_t stream)
 {
 }
-template <>
-void launch_pad_add_transform_0213<__half>(__half* output,
-                                           const __half* vals,
-                                           int batch_size,
-                                           int hidden_dim,
-                                           int seq_length,
-                                           int padded_seq_len,
-                                           int heads,
-                                           int padded_head_size,
-                                           cudaStream_t stream)
+
+template <typename T>
+void launch_pad_add_transform_0213(T* output,
+                                   const T* vals,
+                                   int batch_size,
+                                   int hidden_dim,
+                                   int seq_length,
+                                   int padded_seq_len,
+                                   int heads,
+                                   int padded_head_size,
+                                   cudaStream_t stream)
 {
     hidden_dim >>= 3;
     dim3 block_dim((padded_head_size >> 3), heads, 2);
     dim3 grid_dim(batch_size, padded_seq_len / 2);
     pad_add_transform_0213<<<grid_dim, block_dim, 0, stream>>>(
         output, vals, hidden_dim, seq_length, padded_seq_len, heads, padded_head_size >> 3);
 }
 
+#ifdef BF16_AVAILABLE
+template void launch_pad_add_transform_0213(__nv_bfloat16* output,
+                                            const __nv_bfloat16* vals,
+                                            int batch_size,
+                                            int hidden_dim,
+                                            int seq_length,
+                                            int padded_seq_len,
+                                            int heads,
+                                            int padded_head_size,
+                                            cudaStream_t stream);
+#endif
+
+template void launch_pad_add_transform_0213(__half* output,
+                                            const __half* vals,
+                                            int batch_size,
+                                            int hidden_dim,
+                                            int seq_length,
+                                            int padded_seq_len,
+                                            int heads,
+                                            int padded_head_size,
+                                            cudaStream_t stream);
+
 // Bias add
 template <typename T>
 __global__ void bias_add_transform_0213(T* output,
                                         const T* vals,
                                         const T* bias,
                                         int hidden_dim,
                                         int seq_length,
@@ -390,23 +437,25 @@
     outputs.z = inputs.z + biases.z;
     outputs.w = inputs.w + biases.w;
 
     output_vec[cnt * d0_out_stride * gridDim.x + d0 * d0_out_stride + d1 * d1_out_stride +
                d2 * d2_out_stride + d3] = outputs;
 }
 
-template <>
-__global__ void bias_add_transform_0213<__half>(__half* output,
-                                                const __half* vals,
-                                                const __half* bias,
-                                                int hidden_dim,
-                                                int seq_length,
-                                                int heads,
-                                                int head_ext)
+template <typename T>
+__global__ void bias_add_transform_0213(T* output,
+                                        const T* vals,
+                                        const T* bias,
+                                        int hidden_dim,
+                                        int seq_length,
+                                        int heads,
+                                        int head_ext)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
     int d2_out_stride = d2_stride * seq_length;
 
     int d0 = blockIdx.x;                                                  // Batch
@@ -414,17 +463,17 @@
     int cnt = blockIdx.z / head_ext;                                      // Hidden count
     int d2 = threadIdx.y + (blockIdx.z % head_ext) * (heads / head_ext);  // Head (0-11)
     int d3 = threadIdx.x;                                                 // Values (groups of 4)
 
     float4 vals_arr;
     float4 bias_arr;
     float4 output_arr;
-    __half2* vals_half = reinterpret_cast<__half2*>(&vals_arr);
-    __half2* bias_half = reinterpret_cast<__half2*>(&bias_arr);
-    __half2* output_half = reinterpret_cast<__half2*>(&output_arr);
+    T2* vals_half = reinterpret_cast<T2*>(&vals_arr);
+    T2* bias_half = reinterpret_cast<T2*>(&bias_arr);
+    T2* output_half = reinterpret_cast<T2*>(&output_arr);
 
     const float4* vals_vec = reinterpret_cast<const float4*>(vals);
     const float4* bias_vec = reinterpret_cast<const float4*>(bias);
     float4* output_vec = reinterpret_cast<float4*>(output);
 
     vals_vec += (d0 * d0_stride * (gridDim.z / head_ext));
     vals_vec += (d1 * d1_stride * (gridDim.z / head_ext));
@@ -445,21 +494,24 @@
     output_half[0] = vals_half[0] + bias_half[0];
     output_half[1] = vals_half[1] + bias_half[1];
     output_half[2] = vals_half[2] + bias_half[2];
     output_half[3] = vals_half[3] + bias_half[3];
     output_vec[d3] = output_arr;
 }
 
-__global__ void bias_add_transform_0213_v2(__half* output,
-                                           const __half* vals,
-                                           const __half* bias,
+template <typename T>
+__global__ void bias_add_transform_0213_v2(T* output,
+                                           const T* vals,
+                                           const T* bias,
                                            int hidden_dim,
                                            int seq_length,
                                            int heads)
 {
+    using T2 =
+        typename std::conditional<std::is_same<T, __half>::value, __half2, __nv_bfloat162>::type;
     __shared__ float4 in_data[3072];
 
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
     int iteration_stride = d1_stride * blockDim.z;  // Hidden * 3 / 8
     int batch_stride = d0_stride * blockDim.z;      // Hidden * S * 3 / 8
@@ -473,17 +525,17 @@
     int cnt = threadIdx.z;  // blockIdx.z; // Hidden count
     int d2 = threadIdx.y;   // Head (0-11)
     int d3 = threadIdx.x;   // Values (groups of 4)
 
     float4 vals_arr[1];
     float4 bias_arr[1];
     float4 output_arr[1];
-    __half2* vals_half = reinterpret_cast<__half2*>(vals_arr);
-    __half2* bias_half = reinterpret_cast<__half2*>(bias_arr);
-    __half2* output_half = reinterpret_cast<__half2*>(output_arr);
+    T2* vals_half = reinterpret_cast<T2*>(vals_arr);
+    T2* bias_half = reinterpret_cast<T2*>(bias_arr);
+    T2* output_half = reinterpret_cast<T2*>(output_arr);
 
     const float4* vals_vec = reinterpret_cast<const float4*>(vals);
     const float4* bias_vec = reinterpret_cast<const float4*>(bias);
     float4* output_vec = reinterpret_cast<float4*>(output);
 
     int iter_index = cnt * d1_stride + d2 * d2_stride + d3;
     int input_offset = d0 * batch_stride + d1 * (iteration_stride << 1);
@@ -515,14 +567,30 @@
         int iter_offset =
             (iter_row % blockDim.y) * d2_out_stride + (iter_row / blockDim.y) * matrix_stride;
         output_vec[out_index + iter_offset] =
             in_data[iter_row * d2_stride + d3 + (d2 % 2) * (d1_stride * blockDim.z)];
     }
 }
 
+template __global__ void bias_add_transform_0213_v2(__half* output,
+                                                    const __half* vals,
+                                                    const __half* bias,
+                                                    int hidden_dim,
+                                                    int seq_length,
+                                                    int heads);
+
+#ifdef BF16_AVAILABLE
+template __global__ void bias_add_transform_0213_v2(__nv_bfloat16* output,
+                                                    const __nv_bfloat16* vals,
+                                                    const __nv_bfloat16* bias,
+                                                    int hidden_dim,
+                                                    int seq_length,
+                                                    int heads);
+#endif
+
 template <typename T>
 __global__ void transform4d_0213(T* out,
                                  const T* in,
                                  int heads,
                                  int seq_length,
                                  int hidden_dim,
                                  int head_ext);
@@ -556,21 +624,21 @@
         float4 vals_vec = in_vec[cnt * d0_stride * gridDim.x + d0 * d0_stride + d1 * d1_stride +
                                  d2 * d2_stride + d3];
         out_vec[d0 * d0_out_stride * gridDim.z + cnt * d2_out_stride + d1 * d1_out_stride +
                 d2 * d2_out_stride * gridDim.z + d3] = vals_vec;
     }
 }
 
-template <>
-__global__ void transform4d_0213<__half>(__half* out,
-                                         const __half* in,
-                                         int heads,
-                                         int seq_length,
-                                         int hidden_dim,
-                                         int head_ext)
+template <typename T>
+__global__ void transform4d_0213(T* out,
+                                 const T* in,
+                                 int heads,
+                                 int seq_length,
+                                 int hidden_dim,
+                                 int head_ext)
 {
     int d0_stride = hidden_dim * (seq_length / head_ext);
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
     int d0 = blockIdx.x;                                                  // Batch
     int d1 = threadIdx.y + (blockIdx.z % head_ext) * (heads / head_ext);  // Head
@@ -590,19 +658,16 @@
     out_vec += (d1 * d2_stride);
     out_vec += (d0 * d0_stride * gridDim.y);
     out_vec += (d2 * d1_stride * gridDim.y);
 
     out_vec[d3] = in_vec[d3];
 }
 
-__global__ void transform4d_0213_v2(__half* out,
-                                    const __half* in,
-                                    int heads,
-                                    int seq_length,
-                                    int hidden_dim)
+template <typename T>
+__global__ void transform4d_0213_v2(T* out, const T* in, int heads, int seq_length, int hidden_dim)
 {
     __shared__ float4 in_data[3072];
 
     int d0_stride = hidden_dim * seq_length;
     int d1_stride = hidden_dim;
     int d2_stride = hidden_dim / heads;
 
@@ -638,14 +703,28 @@
 #pragma unroll
     for (int iter = 0; iter < 2; iter++) {
         int iter_id = iter * iteration_stride + iter_index;
         out_vec[output_offset + iter_id] = in_data[iter_id];
     }
 }
 
+#ifdef BF16_AVAILABLE
+template __global__ void transform4d_0213_v2(__nv_bfloat16* out,
+                                             const __nv_bfloat16* in,
+                                             int heads,
+                                             int seq_length,
+                                             int hidden_dim);
+#endif
+
+template __global__ void transform4d_0213_v2(__half* out,
+                                             const __half* in,
+                                             int heads,
+                                             int seq_length,
+                                             int hidden_dim);
+
 // 3 * [B A S N] - > [B S C*H]
 template <>
 void launch_transform4d_0213<float>(float* out,
                                     const float* in,
                                     int batch_size,
                                     int heads,
                                     int seq_length,
@@ -656,24 +735,44 @@
     hidden_dim >>= 2;
     dim3 grid_dims(batch_size, heads * ((seq_length - 1) / 8 + 1), trans_count);
     dim3 block_dims(hidden_dim / heads, 8);
     transform4d_0213<float>
         <<<grid_dims, block_dims, 0, stream>>>(out, in, heads, seq_length, hidden_dim, 1);
 }
 
-template <>
-void launch_transform4d_0213<__half>(__half* out,
-                                     const __half* in,
-                                     int batch_size,
-                                     int heads,
-                                     int seq_length,
-                                     int hidden_dim,
-                                     cudaStream_t stream,
-                                     int trans_count)
+template <typename T>
+void launch_transform4d_0213<T>(T* out,
+                                const T* in,
+                                int batch_size,
+                                int heads,
+                                int seq_length,
+                                int hidden_dim,
+                                cudaStream_t stream,
+                                int trans_count)
 {
     hidden_dim >>= 3;
     int head_ext = (hidden_dim - 1) / MAX_THREADS + 1;
     dim3 grid_dims(batch_size, trans_count, (seq_length * head_ext));
     dim3 block_dims(hidden_dim / heads, (heads / head_ext));
-    transform4d_0213<__half>
-        <<<grid_dims, block_dims, 0, stream>>>(out, in, heads, seq_length, hidden_dim, head_ext);
+    transform4d_0213<<<grid_dims, block_dims, 0, stream>>>(
+        out, in, heads, seq_length, hidden_dim, head_ext);
 }
+
+#ifdef BF16_AVAILABLE
+template void launch_transform4d_0213(__nv_bfloat16* out,
+                                      const __nv_bfloat16* in,
+                                      int batch_size,
+                                      int heads,
+                                      int seq_length,
+                                      int hidden_dim,
+                                      cudaStream_t stream,
+                                      int trans_count);
+#endif
+
+template void launch_transform4d_0213(__half* out,
+                                      const __half* in,
+                                      int batch_size,
+                                      int heads,
+                                      int seq_length,
+                                      int hidden_dim,
+                                      cudaStream_t stream,
+                                      int trans_count);
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 // DeepSpeed Team
 
 #pragma once
 
 #include <assert.h>
 #include <cublas_v2.h>
 #include <cuda.h>
+#include <cuda_bf16.h>
 #include <cuda_fp16.h>
 #include <cuda_runtime.h>
 #ifndef __HIP_PLATFORM_HCC__
 #include <mma.h>
 #endif
 #include <stdio.h>
 
@@ -102,84 +103,88 @@
                 k,
                 (int)status);
         return EXIT_FAILURE;
     }
     return 0;
 }
 
+template <typename T>
 #ifdef __HIP_PLATFORM_HCC__
 int cublas_gemm_ex(rocblas_handle handle,
                    rocblas_operation transa,
                    rocblas_operation transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
-                   const __half* A,
-                   const __half* B,
-                   __half* C,
+                   const T* A,
+                   const T* B,
+                   T* C,
                    rocblas_gemm_algo algo)
 #else
 int cublas_gemm_ex(cublasHandle_t handle,
                    cublasOperation_t transa,
                    cublasOperation_t transb,
                    int m,
                    int n,
                    int k,
                    const float* alpha,
                    const float* beta,
-                   const __half* A,
-                   const __half* B,
-                   __half* C,
+                   const T* A,
+                   const T* B,
+                   T* C,
                    cublasGemmAlgo_t algo)
 #endif
 {
 #ifdef __HIP_PLATFORM_HCC__
+    constexpr auto rocblas_dtype_16 = std::is_same<T, __half>::value ? rocblas_datatype_f16_r
+                                                                     : rocblas_datatype_bf16_r;
     rocblas_status status = rocblas_gemm_ex(handle,
                                             transa,
                                             transb,
                                             m,
                                             n,
                                             k,
                                             (const void*)alpha,
                                             (const void*)A,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             (transa == rocblas_operation_none) ? m : k,
                                             (const void*)B,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             (transb == rocblas_operation_none) ? k : n,
                                             (const void*)beta,
                                             (void*)C,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             m,
                                             (void*)C,
-                                            rocblas_datatype_f16_r,
+                                            rocblas_dtype_16,
                                             m,
                                             rocblas_datatype_f32_r,
                                             algo,
                                             0,
                                             0);
 #else
+    constexpr auto cublas_dtype_16 = std::is_same<T, __half>::value ? CUDA_R_16F : CUDA_R_16BF;
     cublasStatus_t status = cublasGemmEx(handle,
                                          transa,
                                          transb,
                                          m,
                                          n,
                                          k,
                                          (const void*)alpha,
                                          (const void*)A,
-                                         CUDA_R_16F,
+                                         cublas_dtype_16,
                                          (transa == CUBLAS_OP_N) ? m : k,
                                          (const void*)B,
-                                         CUDA_R_16F,
+                                         cublas_dtype_16,
                                          (transb == CUBLAS_OP_N) ? k : n,
                                          (const void*)beta,
                                          (void*)C,
-                                         CUDA_R_16F,
+                                         cublas_dtype_16,
                                          m,
                                          CUDA_R_32F,
                                          algo);
 #endif
 
 #ifdef __HIP_PLATFORM_HCC__
     if (status != rocblas_status_success) {
@@ -303,100 +308,104 @@
                 k,
                 (int)status);
         return EXIT_FAILURE;
     }
     return 0;
 }
 
+template <typename T>
 #ifdef __HIP_PLATFORM_HCC__
 int cublas_strided_batched_gemm(rocblas_handle handle,
                                 int m,
                                 int n,
                                 int k,
                                 const float* alpha,
                                 const float* beta,
-                                const __half* A,
-                                const __half* B,
-                                __half* C,
+                                const T* A,
+                                const T* B,
+                                T* C,
                                 rocblas_operation op_A,
                                 rocblas_operation op_B,
                                 int stride_A,
                                 int stride_B,
                                 int stride_C,
                                 int batch,
                                 rocblas_gemm_algo algo)
 #else
 int cublas_strided_batched_gemm(cublasHandle_t handle,
                                 int m,
                                 int n,
                                 int k,
                                 const float* alpha,
                                 const float* beta,
-                                const __half* A,
-                                const __half* B,
-                                __half* C,
+                                const T* A,
+                                const T* B,
+                                T* C,
                                 cublasOperation_t op_A,
                                 cublasOperation_t op_B,
                                 int stride_A,
                                 int stride_B,
                                 int stride_C,
                                 int batch,
                                 cublasGemmAlgo_t algo)
 #endif
 {
 #ifdef __HIP_PLATFORM_HCC__
+    constexpr auto rocblas_dtype_16 = std::is_same<T, __half>::value ? rocblas_datatype_f16_r
+                                                                     : rocblas_datatype_bf16_r;
     rocblas_status status =
         rocblas_gemm_strided_batched_ex(handle,
                                         op_A,
                                         op_B,
                                         m,
                                         n,
                                         k,
                                         alpha,
                                         A,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         (op_A == rocblas_operation_none) ? m : k,
                                         stride_A,
                                         B,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         (op_B == rocblas_operation_none) ? k : n,
                                         stride_B,
                                         beta,
                                         C,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         m,
                                         stride_C,
                                         C,
-                                        rocblas_datatype_f16_r,
+                                        rocblas_dtype_16,
                                         m,
                                         stride_C,
                                         batch,
                                         rocblas_datatype_f32_r,
                                         algo,
                                         0,
                                         0);
 #else
+    constexpr auto cublas_dtype_16 = std::is_same<T, __half>::value ? CUDA_R_16F : CUDA_R_16BF;
     cublasStatus_t status = cublasGemmStridedBatchedEx(handle,
                                                        op_A,
                                                        op_B,
                                                        m,
                                                        n,
                                                        k,
                                                        alpha,
                                                        A,
-                                                       CUDA_R_16F,
+                                                       cublas_dtype_16,
                                                        (op_A == CUBLAS_OP_N) ? m : k,
                                                        stride_A,
                                                        B,
-                                                       CUDA_R_16F,
+                                                       cublas_dtype_16,
                                                        (op_B == CUBLAS_OP_N) ? k : n,
                                                        stride_B,
                                                        beta,
                                                        C,
-                                                       CUDA_R_16F,
+                                                       cublas_dtype_16,
                                                        m,
                                                        stride_C,
                                                        batch,
                                                        CUDA_R_32F,
                                                        algo);
 #endif
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 // DeepSpeed Team
 
 #pragma once
 
 #include "ds_kernel_utils.h"
 
 #include <cuda.h>
+#ifdef BF16_AVAILABLE
+#include <cuda_bf16.h>
+#endif
 #include <cuda_fp16.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <cassert>
 #include <iostream>
 
 #define MAX_WARP_NUM 32
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.2/deepspeed/ops/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.2/deepspeed/ops/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/lamb/fused_lamb.py` & `deepspeed-0.9.2/deepspeed/ops/lamb/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/__init__.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/all_ops.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/async_io.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/builder.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adagrad.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adam.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/fused_adam.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/fused_lamb.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/quantizer.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/random_ltd.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/sparse_attn.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/spatial_inference.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/stochastic_transformer.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/transformer.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/op_builder/transformer_inference.py` & `deepspeed-0.9.2/deepspeed/ops/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/quantizer/quantizer.py` & `deepspeed-0.9.2/deepspeed/ops/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/random_ltd/dropping_utils.py` & `deepspeed-0.9.2/deepspeed/ops/random_ltd/dropping_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/matmul.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/softmax.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_attention_utils.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_attention_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_self_attention.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparsity_config.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/sparsity_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/__init__.py` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/matmul.tr` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/matmul.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr` & `deepspeed-0.9.2/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/bias_add.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/bias_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/config.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_attention.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_transformer_block.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/diffusers_transformer_block.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_attention.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
                                     num_layers=DeepSpeedSelfAttention.num_layers,
                                     num_heads=self.num_attention_heads_per_partition)
         context_layer, key_layer, value_layer = self.compute_attention(qkv_out=qkv_out,
                                                                        input_mask=input_mask,
                                                                        layer_past=layer_past,
                                                                        alibi=alibi)
         output = self.vector_matmul_func(input=context_layer, weight=self.attn_ow)
-
         inp_norm = qkv_out[-1]
 
         if self.config.mlp_after_attn and self.mp_group is not None and dist.get_world_size(group=self.mp_group) > 1:
             dist.all_reduce(output, group=self.mp_group)
 
         return (output, key_layer, value_layer, context_layer, inp_norm)
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_mlp.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/ds_mlp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/moe_inference.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/moe_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/base.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/base.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 
     def forward(self,
                 input: torch.Tensor,
                 weight: torch.Tensor,
                 bias: torch.Tensor,
                 weight_out: torch.Tensor,
                 async_op: bool = False):
-        output = self.fused_gemm_gelu(input, weight, weight.scale if hasattr(weight, "scale") else torch.empty(1),
+        output = self.fused_gemm_gelu(input, weight, weight.scale if hasattr(weight, 'scale') else torch.empty(1),
                                       bias, weight_out,
-                                      weight_out.scale if hasattr(weight_out, "scale") else torch.empty(1),
+                                      weight_out.scale if hasattr(weight_out, 'scale') else torch.empty(1),
                                       self.config.epsilon, self.config.pre_layer_norm, self.config.q_int8, async_op,
                                       self.config.transposed_mode)
         return output
```

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/linear.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/residual_add.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/residual_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax_context.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/softmax_context.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/inference/triton_ops.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/inference/triton_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/ops/transformer/transformer.py` & `deepspeed-0.9.2/deepspeed/ops/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/profiling/config.py` & `deepspeed-0.9.2/deepspeed/profiling/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/profiling/constants.py` & `deepspeed-0.9.2/deepspeed/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/profiling/flops_profiler/profiler.py` & `deepspeed-0.9.2/deepspeed/profiling/flops_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/checkpointing.py` & `deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/checkpointing.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/config.py` & `deepspeed-0.9.2/deepspeed/runtime/activation_checkpointing/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/bf16_optimizer.py` & `deepspeed-0.9.2/deepspeed/runtime/bf16_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py` & `deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py` & `deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py` & `deepspeed-0.9.2/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/comm/coalesced_collectives.py` & `deepspeed-0.9.2/deepspeed/runtime/comm/coalesced_collectives.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/comm/mpi.py` & `deepspeed-0.9.2/deepspeed/runtime/comm/mpi.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/comm/nccl.py` & `deepspeed-0.9.2/deepspeed/runtime/comm/nccl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/compression/cupy.py` & `deepspeed-0.9.2/deepspeed/runtime/compression/cupy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/config.py` & `deepspeed-0.9.2/deepspeed/runtime/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,14 +775,16 @@
         self.disable_allgather = get_disable_allgather(param_dict)
         self.communication_data_type = get_communication_data_type(param_dict)
         self.prescale_gradients = get_prescale_gradients(param_dict)
         self.gradient_predivide_factor = get_gradient_predivide_factor(param_dict)
         self.sparse_gradients_enabled = get_sparse_gradients_enabled(param_dict)
 
         self.zero_config = get_zero_config(param_dict)
+        self.mics_shard_size = self.zero_config.mics_shard_size
+        self.mics_hierarchial_params_gather = self.zero_config.mics_hierarchical_params_gather
         self.zero_optimization_stage = self.zero_config.stage
         self.zero_enabled = self.zero_optimization_stage > 0
 
         self.activation_checkpointing_config = DeepSpeedActivationCheckpointingConfig(param_dict)
 
         self.comms_config = DeepSpeedCommsConfig(param_dict)
         self.monitor_config = get_monitor_config(param_dict)
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/config_utils.py` & `deepspeed-0.9.2/deepspeed/runtime/config_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/constants.py` & `deepspeed-0.9.2/deepspeed/runtime/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/config.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/constants.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/curriculum_scheduler.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/curriculum_scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/helper.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/scheduler.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/utils.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_routing/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/utils.py` & `deepspeed-0.9.2/deepspeed/runtime/data_pipeline/data_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/dataloader.py` & `deepspeed-0.9.2/deepspeed/runtime/dataloader.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/eigenvalue.py` & `deepspeed-0.9.2/deepspeed/runtime/eigenvalue.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/engine.py` & `deepspeed-0.9.2/deepspeed/runtime/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,14 +687,17 @@
 
     def zero_sub_group_size(self):
         return self._config.zero_config.sub_group_size
 
     def zero_optimization_stage(self):
         return self._config.zero_optimization_stage
 
+    def mics_shard_size(self):
+        return self._config.mics_shard_size
+
     def zero_reduce_bucket_size(self):
         return self._config.zero_config.reduce_bucket_size
 
     def zero_allgather_bucket_size(self):
         return self._config.zero_config.allgather_bucket_size
 
     def zero_optimization_partition_gradients(self):
@@ -774,14 +777,17 @@
         res = self._config.communication_data_type
         if res is not None:
             return res
 
         if self.fp16_enabled():
             return torch.float16
 
+        if self.bfloat16_enabled():
+            return torch.bfloat16
+
         return torch.float32
 
     def postscale_gradients(self):
         return not self._config.prescale_gradients
 
     def gradient_predivide_factor(self):
         return self._config.gradient_predivide_factor
@@ -1190,45 +1196,47 @@
             optimizer_parameters = {}
         # print(optimizer_parameters.keys())
         if "max_grad_norm" in optimizer_parameters.keys():
             raise ValueError(
                 "'max_grad_norm' is not supported as an optimizer parameter, please switch to using the deepspeed parameter 'gradient_clipping' see: https://www.deepspeed.ai/docs/config-json/#gradient-clipping for more details"
             )
 
-        if self.optimizer_name() in [ADAGRAD_OPTIMIZER, ADAM_OPTIMIZER, ADAMW_OPTIMIZER]:
+        if self.optimizer_name() in [ADAM_OPTIMIZER, ADAMW_OPTIMIZER]:
             torch_adam = optimizer_parameters.pop(TORCH_ADAM_PARAM, False)
             adam_w_mode = optimizer_parameters.pop(ADAM_W_MODE, ADAM_W_MODE_DEFAULT)
 
             # Optimizer name of Adam forces AdamW logic unless adam_w_mode is explicitly set
             effective_adam_w_mode = self.optimizer_name() == ADAMW_OPTIMIZER or adam_w_mode
 
             if torch_adam:
                 if not effective_adam_w_mode:
                     optimizer = torch.optim.Adam(model_parameters, **optimizer_parameters)
                 else:
                     optimizer = torch.optim.AdamW(model_parameters, **optimizer_parameters)
             else:
                 if self.zero_use_cpu_optimizer():
-                    if self.optimizer_name() == ADAGRAD_OPTIMIZER:
-                        from deepspeed.ops.adagrad import DeepSpeedCPUAdagrad
-                        optimizer = DeepSpeedCPUAdagrad(model_parameters, **optimizer_parameters)
-                    else:
-                        from deepspeed.ops.adam import DeepSpeedCPUAdam
-                        optimizer = DeepSpeedCPUAdam(model_parameters,
-                                                     **optimizer_parameters,
-                                                     adamw_mode=effective_adam_w_mode)
+                    from deepspeed.ops.adam import DeepSpeedCPUAdam
+                    optimizer = DeepSpeedCPUAdam(model_parameters,
+                                                 **optimizer_parameters,
+                                                 adamw_mode=effective_adam_w_mode)
                 else:
                     from deepspeed.ops.adam import FusedAdam
 
                     optimizer = FusedAdam(
                         model_parameters,
                         **optimizer_parameters,
                         adam_w_mode=effective_adam_w_mode,
                     )
 
+        elif self.optimizer_name() == ADAGRAD_OPTIMIZER:
+            if self.zero_use_cpu_optimizer():
+                from deepspeed.ops.adagrad import DeepSpeedCPUAdagrad
+                optimizer = DeepSpeedCPUAdagrad(model_parameters, **optimizer_parameters)
+            else:
+                optimizer = torch.optim.Adagrad(model_parameters, **optimizer_parameters)
         elif self.optimizer_name() == LAMB_OPTIMIZER:
             from deepspeed.ops.lamb import FusedLamb
 
             optimizer = FusedLamb(model_parameters, **optimizer_parameters)
         elif self.optimizer_name() == ONEBIT_ADAM_OPTIMIZER:
             assert not self.zero_optimization(), "1bit-Adam is not compatible with ZeRO"
             from deepspeed.runtime.fp16.onebit.adam import OnebitAdam
@@ -1361,14 +1369,16 @@
                                    dp_process_group=self.data_parallel_group,
                                    timers=timers)
 
         return optimizer
 
     def _configure_zero_optimizer(self, optimizer):
         zero_stage = self.zero_optimization_stage()
+        mics_shard_size = self.mics_shard_size()
+
         model_dtype, grad_accum_dtype = self.get_data_types()
         timers = self.timers if self.wall_clock_breakdown() else None
 
         if optimizer is None:
             optimizer = DummyOptim(list(self.module.parameters()))
 
         if self.zero_legacy_stage1():
@@ -1436,14 +1446,22 @@
                                                  max_reuse_distance=self.zero_max_reuse_distance(),
                                                  max_live_parameters=self.zero_max_live_parameters(),
                                                  param_persistence_threshold=self.zero_param_persistence_threshold(),
                                                  model_persistence_threshold=self.zero_model_persistence_threshold(),
                                                  offload_param_config=self.zero_offload_param(),
                                                  mpu=self.mpu)
             else:
+                log_dist(
+                    f'Creating fp16 ZeRO stage {zero_stage} optimizer,'
+                    f' MiCS is enabled {mics_shard_size>0},'
+                    f' Hierarchical params gather {self._config.mics_hierarchial_params_gather}',
+                    ranks=[0])
+                if mics_shard_size > 0:
+                    return self._return_mics_optimizer(optimizer, timers)
+
                 log_dist(f'Creating {model_dtype} ZeRO stage {zero_stage} optimizer', ranks=[0])
                 from deepspeed.runtime.zero.stage3 import DeepSpeedZeroOptimizer_Stage3
                 optimizer = DeepSpeedZeroOptimizer_Stage3(
                     self.module,
                     optimizer,
                     timers=timers,
                     ds_config=self.config,
@@ -1472,14 +1490,45 @@
                     communication_data_type=self.communication_data_type)
 
         else:
             raise NotImplementedError("ZeRO stage {} not implemented".format(zero_stage))
 
         return optimizer
 
+    def _return_mics_optimizer(self, basic_optimizer, timers):
+        from deepspeed.runtime.zero.mics import MiCS_Optimizer
+        optimizer = MiCS_Optimizer(self.module,
+                                   basic_optimizer,
+                                   timers=timers,
+                                   ds_config=self.config,
+                                   static_loss_scale=self.loss_scale(),
+                                   dynamic_loss_scale=self.dynamic_loss_scale(),
+                                   dynamic_loss_args=self.dynamic_loss_scale_args(),
+                                   clip_grad=self.gradient_clipping(),
+                                   contiguous_gradients=self.zero_contiguous_gradients(),
+                                   reduce_bucket_size=self.zero_reduce_bucket_size(),
+                                   prefetch_bucket_size=self.zero_prefetch_bucket_size(),
+                                   max_reuse_distance=self.zero_max_reuse_distance(),
+                                   max_live_parameters=self.zero_max_live_parameters(),
+                                   param_persistence_threshold=self.zero_param_persistence_threshold(),
+                                   model_persistence_threshold=self.zero_model_persistence_threshold(),
+                                   dp_process_group=self.data_parallel_group,
+                                   reduce_scatter=self.zero_reduce_scatter(),
+                                   overlap_comm=self.zero_overlap_comm(),
+                                   offload_optimizer_config=self.zero_offload_optimizer(),
+                                   offload_param_config=self.zero_offload_param(),
+                                   sub_group_size=self.zero_sub_group_size(),
+                                   mpu=self.mpu,
+                                   postscale_gradients=self.postscale_gradients(),
+                                   gradient_predivide_factor=self.gradient_predivide_factor(),
+                                   gradient_accumulation_steps=self.gradient_accumulation_steps(),
+                                   aio_config=self.aio_config(),
+                                   communication_data_type=self.communication_data_type)
+        return optimizer
+
     def _configure_eigenvalue(self):
         eigenvalue = Eigenvalue(
             verbose=self.eigenvalue_verbose(),
             max_iter=self.eigenvalue_max_iter(),
             tol=self.eigenvalue_tol(),
             stability=self.eigenvalue_stability(),
             gas_boundary_resolution=self.eigenvalue_gas_boundary_resolution(),
@@ -3017,14 +3066,15 @@
 
         state = dict(module=module,
                      buffer_names=self._get_buffer_names(),
                      optimizer=self.optimizer.state_dict() if self.optimizer and not zero_optimizer_state else None,
                      param_shapes=self._get_zero_param_shapes() if self.optimizer and zero_optimizer_state else None,
                      frozen_param_shapes=self._get_zero_frozen_param_attributes(self._get_param_shape_func)
                      if save_frozen_param else None,
+                     shared_params=self._get_shared_params() if self.optimizer and zero_optimizer_state else None,
                      frozen_param_fragments=self._get_zero_frozen_param_attributes(self._get_param_fragment_func)
                      if save_frozen_param else None,
                      lr_scheduler=self.lr_scheduler.state_dict() if self.lr_scheduler is not None else None,
                      data_sampler=self.training_dataloader.data_sampler.state_dict() if
                      (self.training_dataloader is not None and self.curriculum_learning_enabled()) else None,
                      random_ltd=self.random_ltd_scheduler.state_dict() if self.random_ltd_enabled() else None,
                      sparse_tensor_module_names=self.sparse_tensor_module_names,
@@ -3119,14 +3169,48 @@
                 # uncomment to debug zero_to_fp32.py problems
                 # if self.global_rank == 0: print(f"saving param {name} {shape} (numel={shape.numel()})")
             param_group_shapes.append(param_shapes)
         # if self.global_rank == 0: print(f"Total saved {numel} numels in {cnt} params")
 
         return param_group_shapes
 
+    def _get_shared_params(self):
+        """
+        Returns a dict of shared params, which can later be used to reconstruct the original state dict,
+        e.g. in `zero_to_fp32`. Each dict entry is a pair of param names, where the key is the name
+        of the variable that isn't stored and the value is the actual param holding data.
+        """
+        shared_ds_ids = {}
+        shared_params_by_full_name = {}
+
+        def get_layer_state_dict(module, prefix=""):
+            # handle params
+            for name, param in module.named_parameters(recurse=False):
+                if param is None or not hasattr(param, "ds_id"):
+                    continue
+                key = prefix + name
+                # can't rely on param.data_ptr() as it will be reused as weights gets
+                # gathered and reduced, but param.ds_id is unique across all zero weights
+                # (and shared params will have the same param.ds_id)
+                if param.ds_id in shared_ds_ids:
+                    # shared weights
+                    #print(f"`{key}` is shared with `{shared_ds_ids[param.ds_id]}`")
+                    shared_params_by_full_name[key] = shared_ds_ids[param.ds_id]
+                else:
+                    shared_ds_ids[param.ds_id] = key
+
+            for name, child in module.named_children():
+                if child is not None:
+                    get_layer_state_dict(child, prefix + name + ".")
+
+        if dist.get_rank() == 0:
+            get_layer_state_dict(self.module, prefix="")
+
+        return shared_params_by_full_name
+
     def _copy_recovery_script(self, save_path):
         base_dir = os.path.dirname(os.path.dirname(__file__))
         script = "zero_to_fp32.py"
         src = os.path.join(base_dir, "utils", script)
         dst = os.path.join(save_path, script)
         #logger.info(f"creating recovery script {dst}")
         copyfile(src, dst)
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/fp16/fused_optimizer.py` & `deepspeed-0.9.2/deepspeed/runtime/fp16/fused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/fp16/loss_scaler.py` & `deepspeed-0.9.2/deepspeed/runtime/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/adam.py` & `deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/lamb.py` & `deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/zoadam.py` & `deepspeed-0.9.2/deepspeed/runtime/fp16/onebit/zoadam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/fp16/unfused_optimizer.py` & `deepspeed-0.9.2/deepspeed/runtime/fp16/unfused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/hybrid_engine.py` & `deepspeed-0.9.2/deepspeed/runtime/hybrid_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from deepspeed.module_inject.replace_policy import replace_policies
 from deepspeed.module_inject.utils import policy_to_ds_container
 from .engine import DeepSpeedEngine
 from .utils import TLinear, get_inactive_params
 from deepspeed.runtime.zero import GatheredParameters
 import time
 import gc
-
+import math
 from deepspeed import comm as dist
 from deepspeed.accelerator import get_accelerator
 from torch import nn
 from deepspeed.utils import logger
 
 from deepspeed.ops.op_builder import InferenceBuilder
 
@@ -90,15 +90,23 @@
                                             min_out_tokens=self._config.hybrid_engine.max_out_tokens,
                                             transposed_mode=True),
             model_config=self.module.config if hasattr(self.module, 'config') else None,
             layer_id=layer_id,
             child=orig_layer)
         _container.set_dtype(self._config.fp16_enabled)
 
-        _container.set_tensor_parallel_config(self._config.hybrid_engine.inference_tp_size, self.mp_group)
+        if self.mpu is not None:
+            if hasattr(self.mpu, 'get_model_parallel_world_size'):
+                _container.set_tensor_parallel_config(self.mpu.get_model_parallel_world_size(),
+                                                      self.mpu.get_model_parallel_group())
+            else:
+                _container.set_tensor_parallel_config(self.mpu.get_tensor_model_parallel_world_size(),
+                                                      self.mpu.get_tensor_model_parallel_group())
+        else:
+            _container.set_tensor_parallel_config(self._config.hybrid_engine.inference_tp_size, self.mp_group)
         _container.initialize_tensors(enable_training=True)
         _container.create_ds_model_config()
         _container.create_module()
         _container.set_params_wo_copy(Z3_enabled=self.Z3_enabled)
         return _container
 
     def populate_all_inference_policies(self):
@@ -116,28 +124,28 @@
             nn.LayerNorm: (Normalize, ),
             OPTLearnedPositionalEmbedding: (OPTEmbedding, )
         })
 
     def _fuse_lora(self, params, lora_params):
         maybe_has_lora_params = [p for p in params if len(p.shape) > 1]
         for lora_param, weight in zip(lora_params, maybe_has_lora_params):
-            if len(lora_params) > 0:
+            if len(lora_param) == 3:
                 lora_right_weight, \
                 lora_left_weight, \
                 lora_scaling = lora_param
                 weight.data += lora_scaling * torch.matmul(lora_left_weight.t(), lora_right_weight.t())
 
     def fuse_lora_weight(self):
         for layer_id in range(len(self.layer_params)):
             self._fuse_lora(self.layer_params[layer_id], self.lora_params[layer_id])
 
     def _unfuse_lora(self, params, lora_params):
         maybe_has_lora_params = [p for p in params if len(p.shape) > 1]
         for lora_param, weight in zip(lora_params, maybe_has_lora_params):
-            if len(lora_params) > 0:
+            if len(lora_param) == 3:
                 lora_right_weight, \
                 lora_left_weight, \
                 lora_scaling = lora_param
                 weight.data -= lora_scaling * torch.matmul(lora_left_weight.t(), lora_right_weight.t())
 
     def unfuse_lora_weight(self):
         for layer_id in range(len(self.layer_params)):
@@ -177,30 +185,32 @@
             if self._config.hybrid_engine.inference_tp_size > 1:
                 non_tp_params = []
                 for other_layer in self._other_layers:
                     non_tp_params.extend(list(other_layer.parameters()))
 
                 partition_size = self._config.hybrid_engine.tp_gather_partition_size
 
-                layer_groups = len(self.layer_params) // partition_size
+                layer_groups = math.ceil(len(self.layer_params) / partition_size)
                 for lg in range(layer_groups):
                     non_active_params = []
                     non_active_lora_params = []
                     for layer_id in range(lg * partition_size, min(len(self.layer_params), (lg + 1) * partition_size),
                                           1):
                         non_tp_params.extend(self.layer_params[layer_id][:4])
                         non_active_params.extend(get_inactive_params(self.layer_params[layer_id]))
                         non_active_params.extend(get_inactive_params(self.layer_lora_params[layer_id]))
                     with GatheredParameters(non_active_params):
                         for layer_id in range(lg * partition_size,
                                               min(len(self.layer_params), (lg + 1) * partition_size), 1):
                             if len(self.all_lora_params) > 0:
                                 self._fuse_lora(self.layer_params[layer_id], self.lora_params[layer_id])
-                            self._inference_containers[layer_id].apply_tensor_parallelism(
-                                mp_group=self.mp_group, tp_size=self._config.hybrid_engine.inference_tp_size)
+
+                            if self.mpu is not None:
+                                self._inference_containers[layer_id].apply_tensor_parallelism(
+                                    mp_group=self.mp_group, tp_size=self._config.hybrid_engine.inference_tp_size)
 
                 # TODO(cmikeh2) Evaluate if this can be deferred when release_inference_cache
                 # is enabled.
                 gc.collect()
                 get_accelerator().empty_cache()
 
                 self._gather_latency = time.time() - self._t0
@@ -302,35 +312,40 @@
         self.all_lora_params = []
 
         self._other_layers = []
         self._orig_modules_others = []
         self._orig_fwds_others = []
 
         if self._config.hybrid_engine.inference_tp_size > 1:
-            global_rank = dist.get_rank()
-            world_size = dist.get_world_size()
-            mp_group_id = global_rank // self._config.hybrid_engine.inference_tp_size
-            num_mp_groups = world_size // self._config.hybrid_engine.inference_tp_size
-            for mp_group_id in range(num_mp_groups):
-                ranks = list(
-                    range(mp_group_id * self._config.hybrid_engine.inference_tp_size, \
-                          (mp_group_id + 1) * self._config.hybrid_engine.inference_tp_size, \
-                          1)
-                )
-                mp_group = dist.new_group(ranks)
-                if global_rank in ranks:
-                    self.mp_group = mp_group
+            if self.mpu is not None:
+                global_rank = dist.get_rank()
+                world_size = dist.get_world_size()
+                mp_group_id = global_rank // self._config.hybrid_engine.inference_tp_size
+                num_mp_groups = world_size // self._config.hybrid_engine.inference_tp_size
+                for mp_group_id in range(num_mp_groups):
+                    ranks = list(
+                        range(mp_group_id * self._config.hybrid_engine.inference_tp_size, \
+                            (mp_group_id + 1) * self._config.hybrid_engine.inference_tp_size, \
+                            1)
+                    )
+                    mp_group = dist.new_group(ranks)
+                    if global_rank in ranks:
+                        self.mp_group = mp_group
+            else:
+                self.mp_group = self.mpu.get_model_parallel_group() if hasattr(self.mpu, 'get_model_parallel_group') else \
+                    self.mpu.get_tensor_model_parallel_group()
         else:
             self.mp_group = None
         self.populate_all_inference_policies()
         self.all_layers_params = list(self.module.parameters())
         self.create_inference_containers(self.module)
 
-        self._generate = self.module.generate
-        self.module.generate = self.generate
+        if len(self._inference_containers) > 0:
+            self._generate = self.module.generate
+            self.module.generate = self.generate
 
         self._t0 = time.time()
 
     def _zero3_forward(self, layer_id):
 
         def run_forward(*inputs, **kwargs):
             non_active_params = get_inactive_params(self.layer_params[layer_id])
@@ -370,35 +385,42 @@
             for i, (orig_module, inference_container) in enumerate(zip(self._orig_modules,
                                                                        self._inference_containers)):
                 if self.Z3_enabled and not self.gather_all_layers:
                     orig_module.forward = self._zero3_forward(i)
                 else:
                     orig_module.forward = inference_container.module.forward
 
+                inference_container.align_merged_qkv()
+
             if not self.Z3_enabled or self.gather_all_layers:
                 for orig_module, inference_layer in zip(self._orig_modules_others, self._other_layers):
                     orig_module.forward = inference_layer.forward
         if self.Z3_enabled:
             gc.collect()
             get_accelerator().empty_cache()
         if self._t_start is None:
             self._t_start = time.time()
 
     def train(self, mode=True):
         if mode and len(self._orig_modules) > 0:
-            for orig_module, orig_fwd in zip(self._orig_modules, self._orig_fwds):
+            for inference_container, orig_module, orig_fwd in zip(self._inference_containers, self._orig_modules,
+                                                                  self._orig_fwds):
+                inference_container.partition_merged_qkv()
                 orig_module.forward = orig_fwd
             for orig_module, orig_fwd in zip(self._orig_modules_others, self._orig_fwds_others):
                 orig_module.forward = orig_fwd
         super().train(mode)
         if mode:
             self._training_start_time = time.time()
 
     def step(self, lr_kwargs=None):
         super().step(lr_kwargs=lr_kwargs)
-        if(self._inference_containers[0].module.attention.attn_qkvw is not None and \
-            self._inference_containers[0].q_k_v is not None):
-            for inference_container in self._inference_containers:
-                inference_container.reset_qkv()
+
+        if len(self._inference_containers) > 0:
+            if(self._inference_containers[0].module.attention.attn_qkvw is not None and \
+                self._inference_containers[0].q_k_v is not None):
+                for inference_container in self._inference_containers:
+                    inference_container.reset_qkv()
+
         if self._training_start_time is not None:
             self._training_latency += (time.time() - self._training_start_time)
             self._training_start_time = time.time()
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/lr_schedules.py` & `deepspeed-0.9.2/deepspeed/runtime/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/pipe/engine.py` & `deepspeed-0.9.2/deepspeed/runtime/pipe/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from deepspeed.utils import logger
 from deepspeed.utils.timer import ThroughputTimer
 from deepspeed.accelerator import get_accelerator
 
 from ..engine import DeepSpeedEngine, MEMORY_OPT_ALLREDUCE_SIZE
 from ..utils import PartitionedTensor
 from ..dataloader import RepeatingLoader
+from ..zero.config import ZeroStageEnum
+from ..activation_checkpointing import checkpointing as ds_checkpointing
 
 from .module import PipelineModule, PipelineError
 from . import p2p
 from . import schedule
 
 TARGET_ID = -2
 LOG_STAGE = -2
@@ -237,19 +239,18 @@
             grad = weight._hp_grad if self.bfloat16_enabled() else weight.grad
             dist.all_reduce(grad, group=group)
 
     def _exec_reduce_grads(self):
         self._force_grad_boundary = True
         if self.pipeline_enable_backward_allreduce:
             if self.bfloat16_enabled():
-                if self.zero_optimization_stage() == 0:
+                if self.zero_optimization_stage() < ZeroStageEnum().gradients:
                     self._bf16_reduce_grads()
                 else:
-                    assert self.zero_optimization_stage() == 1, "only bf16 + z1 are supported"
-                    raise NotImplementedError()
+                    raise NotImplementedError("PP+BF16 only work for ZeRO Stage 1")
             else:
                 self.allreduce_gradients(bucket_size=MEMORY_OPT_ALLREDUCE_SIZE)
         self._force_grad_boundary = False
 
     def _bf16_reduce_grads(self):
         # Make our own list of gradients from the optimizer's FP32 grads
         grads = []
@@ -496,15 +497,15 @@
     def _bcast_pipe_scalar(self, data, src_rank=None, dtype=torch.float32):
         # Default to last stage (e.g., for broadcasting loss)
         if src_rank is None:
             src_rank = self.grid.stage_to_global(self.num_stages - 1)
         assert src_rank in self.grid.pp_group
 
         if self.global_rank == src_rank:
-            result = data.clone().detach()
+            result = data.clone().detach().type(dtype).to(self.device)
         else:
             result = torch.Tensor([0.]).type(dtype).to(self.device)
 
         dist.broadcast(tensor=result, src=src_rank, group=self.mpu.get_pipe_parallel_group())
 
         return result
 
@@ -621,14 +622,19 @@
 
         # Zero out the gradients each time we use the tensor because only the data in
         # tensor changes across batches
         self._zero_grads(inputs)
 
         outputs = super().forward(inputs)
 
+        # Reset activation checkpointing buffers.
+        # Need to call this between evaluation iterations
+        if not self.module.training:
+            ds_checkpointing.reset()
+
         # Partition the outputs if we are not the last stage
         if self.is_pipe_partitioned and not self.is_last_stage():
             if isinstance(outputs, tuple):
                 first_output = outputs[0]
                 # TODO: Improve pipe partitioning to pass multiple tensors that require grads
                 assert all([torch.is_tensor(elt) and elt.requires_grad is False for elt in outputs[1:]])
                 outputs_tail = outputs[1:]
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/pipe/module.py` & `deepspeed-0.9.2/deepspeed/runtime/pipe/module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/pipe/p2p.py` & `deepspeed-0.9.2/deepspeed/runtime/pipe/p2p.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/pipe/schedule.py` & `deepspeed-0.9.2/deepspeed/runtime/pipe/schedule.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/pipe/topology.py` & `deepspeed-0.9.2/deepspeed/runtime/pipe/topology.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/progressive_layer_drop.py` & `deepspeed-0.9.2/deepspeed/runtime/progressive_layer_drop.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/quantize.py` & `deepspeed-0.9.2/deepspeed/runtime/quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/sparse_tensor.py` & `deepspeed-0.9.2/deepspeed/runtime/sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/state_dict_factory.py` & `deepspeed-0.9.2/deepspeed/runtime/state_dict_factory.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/aio_config.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/aio_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/async_swapper.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/async_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/constants.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/optimizer_utils.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/utils.py` & `deepspeed-0.9.2/deepspeed/runtime/swap_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/utils.py` & `deepspeed-0.9.2/deepspeed/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/weight_quantizer.py` & `deepspeed-0.9.2/deepspeed/runtime/weight_quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/config.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,17 @@
     """
     Stage 1 and 2 optimization for CPU offloading that parallelizes gradient
     copying to CPU memory among ranks by fine-grained gradient partitioning.
     Performance benefit grows with gradient accumulation steps (more copying
     between optimizer steps) or GPU count (increased parallelism).
     """
 
+    mics_shard_size: int = Field(-1, new_param="mics_shard_size")
+
+    mics_hierarchical_params_gather: bool = False
     memory_efficient_linear: bool = True
     """
     Use memory efficient linear implementation, for Stage 3.
     """
 
     # Validators
     @validator("overlap_comm")
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/contiguous_memory_allocator.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/contiguous_memory_allocator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/linear.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/linear.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 from torch.nn.parameter import Parameter
 from torch.nn import init
 from torch.nn.modules.module import Module
 from deepspeed.runtime.utils import noop_decorator
 from deepspeed import comm as dist
 from deepspeed.accelerator import get_accelerator
 
-tensor_map = {}
-
 
 def print_rank_0(message, debug=False, force=False):
     if dist.get_rank() == 0 and (debug or force):
         print(message)
 
 
 try:
@@ -46,22 +44,15 @@
 
     # Note that both forward and backward are @staticmethods
     @staticmethod
     @autocast_custom_fwd
     # bias is an optional argument
     def forward(ctx, input, weight, bias=None):
 
-        weight_id = id(weight)
-        bias_id = id(bias)
-
-        #ctx.save_for_backward(input, weight, bias)
-        ctx.save_for_backward(input, torch.tensor(weight_id), torch.tensor(bias_id))
-
-        tensor_map[weight_id] = weight
-        tensor_map[bias_id] = bias
+        ctx.save_for_backward(input, weight, bias)
 
         if input.dim() == 2 and bias is not None:
             # fused op is marginally faster
             ret = torch.addmm(bias, input, weight.t())
         else:
             output = input.matmul(weight.t())
             if bias is not None:
@@ -75,19 +66,15 @@
     @autocast_custom_bwd
     def backward(ctx, grad_output):
         # This is a pattern that is very convenient - at the top of backward
         # unpack saved_tensors and initialize all gradients w.r.t. inputs to
         # None. Thanks to the fact that additional trailing Nones are
         # ignored, the return statement is simple even when the function has
         # optional inputs.
-        #input, weight, bias = ctx.saved_tensors
-
-        input, weight_id, bias_id = ctx.saved_tensors
-        weight = tensor_map[weight_id.item()]
-        bias = tensor_map[bias_id.item()]
+        input, weight, bias = ctx.saved_tensors
 
         grad_input = grad_weight = grad_bias = None
 
         #print(f"backward shaped grad_output {grad_output.shape}, input {input.shape}, weight {weight.shape} and bias {bias.shape if bias is not None else None}")
         # These needs_input_grad checks are optional and there only to
         # improve efficiency. If you want to make your code simpler, you can
         # skip them. Returning gradients for inputs that don't require it is
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/offload_config.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/offload_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/parameter_offload.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/parameter_offload.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/partition_parameters.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/partition_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -524,68 +524,70 @@
 
 class AllGatherHandle:
 
     def __init__(self, handle, param: Parameter) -> None:
         if param.ds_status != ZeroParamStatus.INFLIGHT:
             raise RuntimeError(f"expected param {param.ds_summary()} to be available")
 
-        self.__handle = handle
-        self.__param = param
+        self.handle = handle
+        self.param = param
 
     def wait(self) -> None:
-        instrument_w_nvtx(self.__handle.wait)()
-        self.__param.ds_status = ZeroParamStatus.AVAILABLE
+        instrument_w_nvtx(self.handle.wait)()
+        self.param.ds_status = ZeroParamStatus.AVAILABLE
 
 
 class AllGatherCoalescedHandle:
 
     def __init__(
         self,
         allgather_handle,
         params: List[Parameter],
         partitions: List[Tensor],
         world_size: int,
     ) -> None:
-        self.__allgather_handle = allgather_handle
-        self.__params = params
-        self.__partitions = partitions
-        self.__world_size = world_size
-        self.__complete = False
+        # renaming the fields without double underscore to ease
+        # the class inheritance
+        self.allgather_handle = allgather_handle
+        self.params = params
+        self.partitions = partitions
+        self.world_size = world_size
+        self.complete = False
 
-        for param in self.__params:
+        for param in self.params:
             if param.ds_status != ZeroParamStatus.INFLIGHT:
                 raise RuntimeError(f"expected param {param.ds_summary()} to not be available")
 
     @instrument_w_nvtx
     def wait(self) -> None:
-        if self.__complete:
+        if self.complete:
             return
 
-        instrument_w_nvtx(self.__allgather_handle.wait)()
+        instrument_w_nvtx(self.allgather_handle.wait)()
 
         # split the single tensor out into individual tensors
         param_offset = 0
-        for param in self.__params:
+        for param in self.params:
             assert param.ds_status == ZeroParamStatus.INFLIGHT, f"expected param {param.ds_summary()} to be inflight"
             partitions: List[Tensor] = []
-            for rank in range(self.__world_size):
+            for rank in range(self.world_size):
                 param_start = rank * param.ds_tensor.ds_numel
                 if param_start < param.ds_numel:
-                    part_to_copy = self.__partitions[rank].narrow(
+                    part_to_copy = self.partitions[rank].narrow(
                         0, param_offset, min(param.ds_numel - param_start, param.ds_tensor.ds_numel))
                     partitions.append(part_to_copy)
             param.data = instrument_w_nvtx(torch.cat)(partitions).view(param.ds_shape)
             param.ds_status = ZeroParamStatus.AVAILABLE
 
             for part_to_copy in partitions:
                 part_to_copy.record_stream(get_accelerator().current_stream())
 
             param_offset += param.ds_tensor.ds_numel
 
-        self.__complete = True
+        self.complete = True
 
 
 def _no_gather_coalesced(params: Iterable[Parameter]) -> AllGatherCoalescedHandle:
     for param in params:
         if param.ds_status != ZeroParamStatus.NOT_AVAILABLE:
             raise RuntimeError(param.ds_summary())
         param.ds_status = ZeroParamStatus.INFLIGHT
@@ -729,15 +731,15 @@
             assert dist.is_initialized(), "Parameters cannot be scattered without initializing deepspeed.comm"
         if data_parallel_group is None:
             self.ds_process_group = dist.get_world_group()
         else:
             self.ds_process_group = data_parallel_group
 
         self.rank = dist.get_rank(group=self.ds_process_group)
-        self.world_size = dist.get_world_size(group=self.ds_process_group)
+        self.dp_world_size = dist.get_world_size(group=self.ds_process_group)
 
         # Local device is the device where the parameters are consumed, must be default device.
         # It is the device where parameters are fully instantiated using allgather
         self.local_device = torch.device(get_accelerator().device_name(os.environ["LOCAL_RANK"]))
         get_accelerator().set_device(self.local_device)
 
         if _ds_config is not None:
@@ -769,15 +771,15 @@
         self.use_all_gather_into_tensor = dist.has_all_gather_into_tensor()
         if not self.use_all_gather_into_tensor:
             logger.info(f"all_gather_into_tensor API is not available in torch {torch.__version__}")
 
     def _update_persist_config(self, ds_config):
         Init.apply_param_persistence = True
         Init.param_persistence_threshold = ds_config.zero_config.param_persistence_threshold
-        Init.model_persistence_threshold = ds_config.zero_config.model_persistence_threshold // self.world_size
+        Init.model_persistence_threshold = ds_config.zero_config.model_persistence_threshold // self.num_partitions
 
     def _convert_to_zero_parameters(self, param_list):
         for param in param_list:
             if is_zero_param(param):
                 continue
             self._convert_to_deepspeed_param(param)
             param.partition()
@@ -807,15 +809,15 @@
             param_count += param.numel()
             if not is_zero_param(param):
                 self._convert_to_deepspeed_param(param)
                 print_rank_0(
                     f"Partitioning param {debug_param2name_id_shape(param)} module={debug_module2name(module)}")
 
                 if get_accelerator().on_accelerator(param):
-                    dist.broadcast(param, 0, self.ds_process_group)
+                    dist.broadcast(param, 0, self.get_dp_process_group())
                 else:
                     if dist.get_rank() == 0:
                         logger.warn(f"param `{name}` in {module.__class__.__name__} "
                                     f"not on GPU so was not broadcasted from rank 0")
 
                 param.partition()
         see_memory_usage(
@@ -872,15 +874,15 @@
 
         @instrument_w_nvtx
         def all_gather_coalesced(params: Iterable[Parameter], safe_mode: bool = False) -> AllGatherCoalescedHandle:
 
             # fetches from nvme if the partition is not available and in nvme
             self._ensure_availability_of_partitioned_params(params)
 
-            if self.world_size == 1:
+            if self.num_partitions == 1:
                 return _no_gather_coalesced(params)
 
             for param in params:
                 if param.ds_status != ZeroParamStatus.NOT_AVAILABLE:
                     raise RuntimeError(param.ds_summary())
                 param.ds_status = ZeroParamStatus.INFLIGHT
 
@@ -903,42 +905,43 @@
                 # otherwise could mix data between tensors.
                 assert_ints_same_as_other_ranks([p.ds_tensor.ds_numel for p in params])
 
             if len(params) == 1:
                 # have an opportunity to avoid some intermediate memory allocations
                 param, = params
                 param_buffer = torch.empty(
-                    math.ceil(param.ds_numel / self.world_size) * self.world_size,
+                    math.ceil(param.ds_numel / self.num_partitions) * self.num_partitions,
                     dtype=param.dtype,
                     device=get_accelerator().current_device_name(),
                     requires_grad=False,
                 )
                 handle = _dist_allgather_fn(param.ds_tensor.to(get_accelerator().current_device_name()), param_buffer,
-                                            self.ds_process_group)
+                                            self.get_partition_dp_group(param))
                 param.data = param_buffer.narrow(0, 0, param.ds_numel).view(param.ds_shape).to(param.device)
                 return AllGatherHandle(handle, param)
             else:
                 partition_sz = sum(p.ds_tensor.ds_numel for p in params)
-                flat_tensor = torch.empty(partition_sz * self.world_size,
+                flat_tensor = torch.empty(partition_sz * self.num_partitions,
                                           dtype=get_only_unique_item(p.dtype for p in params),
                                           device=get_accelerator().current_device_name(),
                                           requires_grad=False)
                 partitions: List[Parameter] = []
-                for i in range(self.world_size):
+                for i in range(self.num_partitions):
                     partitions.append(flat_tensor.narrow(0, partition_sz * i, partition_sz))
 
                 instrument_w_nvtx(torch.cat)([p.ds_tensor.to(get_accelerator().current_device_name()) for p in params],
-                                             out=partitions[self.rank])
-                handle = _dist_allgather_fn(partitions[self.rank], flat_tensor, self.ds_process_group)
+                                             out=partitions[self.get_partition_rank()])
+                handle = _dist_allgather_fn(partitions[self.get_partition_rank()], flat_tensor,
+                                            self.get_partition_dp_group(params[0]))
 
                 return AllGatherCoalescedHandle(
                     allgather_handle=handle,
                     params=params,
                     partitions=partitions,
-                    world_size=self.world_size,
+                    world_size=self.num_partitions,
                 )
 
         def partition(param_list=None, hierarchy=0, has_been_updated=False):
             cls = param
             print_rank_0(f"{'--'*hierarchy}----Partitioning param {debug_param2name_id_shape_device(cls)}")
             if param_list is None:
                 param_list = [cls]
@@ -985,14 +988,15 @@
                 "ds_numel": slf.ds_numel,
                 "shape": tuple(slf.shape),
                 "ds_shape": tuple(slf.ds_shape),
                 "requires_grad": slf.requires_grad,
                 "grad_shape": tuple(slf.grad.shape) if slf.grad is not None else None,
                 "persist": slf.ds_persist,
                 "active_sub_modules": slf.ds_active_sub_modules,
+                "ds_tensor.shape": slf.ds_tensor.shape if slf.ds_tensor is not None else None
             }
 
         def convert_to_zero_parameters(param_list):
             self._convert_to_zero_parameters(param_list)
 
         def allgather_before(func: Callable) -> Callable:
 
@@ -1021,16 +1025,16 @@
 
         param.convert_to_zero_parameters = convert_to_zero_parameters
 
     def _aligned_size(self, param):
         return param.ds_numel + self._padding_size(param)
 
     def _padding_size(self, param):
-        remainder = param.ds_numel % self.world_size
-        return (self.world_size - remainder) if remainder else 0
+        remainder = param.ds_numel % self.num_partitions
+        return (self.num_partitions - remainder) if remainder else 0
 
     def _partition_numel(self, param):
         return param.ds_tensor.ds_numel
 
     def _ensure_availability_of_partitioned_params(self, params):
         swap_in_list = []
         swap_in_flight = []
@@ -1118,15 +1122,15 @@
                 if param.ds_tensor.final_location == OffloadDeviceEnum.nvme:
                     print_rank_0(f"Param {param.ds_id} partition released since it exists in nvme", force=False)
                     param.nvme_swapper.remove_partition_and_release_buffers([param])
 
                 return
 
             tensor_size = self._aligned_size(param)
-            partition_size = tensor_size // self.world_size
+            partition_size = tensor_size // self.num_partitions
 
             if param.ds_tensor is None:
                 final_location = None
                 if self.remote_device == OffloadDeviceEnum.nvme and self.param_swapper.swappable_tensor(
                         numel=partition_size):
                     final_location = OffloadDeviceEnum.nvme
                     buffer = self.param_swapper.get_buffer(param, partition_size)
@@ -1149,15 +1153,15 @@
 
                 partitioned_tensor.requires_grad = False
                 param.ds_tensor = partitioned_tensor
                 param.ds_tensor.ds_numel = partition_size
                 param.ds_tensor.status = PartitionedParamStatus.AVAILABLE
                 param.ds_tensor.final_location = final_location
 
-            start = partition_size * self.rank
+            start = partition_size * self.get_partition_rank()
             end = start + partition_size
 
             one_dim_param = param.contiguous().view(-1)
 
             if start < param.ds_numel and end <= param.ds_numel:
                 src_tensor = one_dim_param.narrow(0, start, partition_size)
 
@@ -1203,15 +1207,15 @@
                 f"Param id {param.ds_id}, param status: {param.ds_status}, param numel {param.ds_numel}, partitioned ds_tensor {param.ds_tensor}, data numel {param.data.numel()}"
             )
 
     def _allgather_param(self, param, async_op=False, hierarchy=0):
 
         partition_size = param.ds_tensor.ds_numel
 
-        tensor_size = partition_size * self.world_size
+        tensor_size = partition_size * self.num_partitions
         aligned_param_size = self._aligned_size(param)
         assert tensor_size == aligned_param_size, f'param id {param.ds_id} aligned size {aligned_param_size} does not match tensor size {tensor_size}'
 
         print_rank_0(
             f"{'--'* hierarchy}---- Before allocating allgather param {debug_param2name_id_shape_status(param)} partition size={partition_size}"
         )
 
@@ -1231,85 +1235,85 @@
         #        if not flat_tensor.numel() > 100000:
         #            replicated_tensor = flat_tensor.narrow(0,
         #                                                   0,
         #                                                   param.ds_numel).view(param.ds_shape)
         #            param.data = replicated_tensor.data
         #            return None
         if self.use_all_gather_into_tensor:
-            # try the all_gather_into_tensor on PyTorch master branch
             handle = dist.all_gather_into_tensor(flat_tensor,
                                                  param.ds_tensor.to(get_accelerator().device_name()),
-                                                 group=self.ds_process_group,
+                                                 group=self.get_partition_dp_group(param),
                                                  async_op=async_op)
         else:
             partitions = []
-            for i in range(self.world_size):
+            for i in range(self.num_partitions):
                 partitions.append(flat_tensor.narrow(0, partition_size * i, partition_size))
 
-                if i == dist.get_rank(group=self.ds_process_group):
+                if i == dist.get_rank(group=self.get_partition_dp_group(param)):
                     partitions[i].data.copy_(param.ds_tensor.data, non_blocking=True)
 
-            handle = dist.all_gather(partitions, partitions[self.rank], group=self.ds_process_group, async_op=async_op)
+            handle = dist.all_gather(partitions,
+                                     partitions[self.get_partition_rank()],
+                                     group=self.get_partition_dp_group(param),
+                                     async_op=async_op)
 
         replicated_tensor = flat_tensor.narrow(0, 0, param.ds_numel).view(param.ds_shape)
         param.data = replicated_tensor.data
         return handle
 
     def _allgather_params_coalesced(self, param_list, hierarchy=0):
         """ blocking call
         avoid explicit memory copy in _allgather_params
         """
         if len(param_list) == 0:
             return
 
-        if self.world_size == 1:
+        if self.num_partitions == 1:
             handle = _no_gather_coalesced(param_list)
             handle.wait()
             return None
 
         # collect local tensors and partition sizes
         partition_sizes = []
         local_tensors = []
         for param in param_list:
             partition_sizes.append(param.ds_tensor.ds_numel)
             local_tensors.append(param.ds_tensor.to(get_accelerator().device_name()))
 
         # allocate memory for allgather params
         allgather_params = []
         for psize in partition_sizes:
-            tensor_size = psize * self.world_size
+            tensor_size = psize * self.num_partitions
             flat_tensor = torch.empty(tensor_size, dtype=param_list[0].dtype, device=self.local_device).view(-1)
             flat_tensor.requires_grad = False
             allgather_params.append(flat_tensor)
 
         # launch
         launch_handles = []
-        # backend = get_backend(self.ds_process_group)
-        # with _batch_p2p_manager(backend):
         for param_idx, param in enumerate(param_list):
             input_tensor = local_tensors[param_idx].view(-1)
 
             if self.use_all_gather_into_tensor:
-                # try the all_gather_into_tensor from Pytorch master
+                # try the _all_gather_base from Pytorch master
                 h = dist.all_gather_into_tensor(allgather_params[param_idx],
                                                 input_tensor,
-                                                group=self.ds_process_group,
+                                                group=self.get_partition_dp_group(param),
                                                 async_op=True)
             else:
                 output_list = []
-                for i in range(self.world_size):
+                for i in range(self.num_partitions):
                     psize = partition_sizes[param_idx]
                     partition = allgather_params[param_idx].narrow(0, i * psize, psize)
                     output_list.append(partition)
                     if not get_accelerator().on_accelerator(partition):
                         logger.warning(
                             f'param {param_idx}, partition {i} is not on CUDA, partition shape {partition.size()}')
 
-                # back to old all_gather function signature
-                h = dist.all_gather(output_list, input_tensor, group=self.ds_process_group, async_op=True)
+                # back to old all_gather function
+                h = dist.all_gather(output_list, input_tensor, group=self.get_partition_dp_group(param), async_op=True)
             launch_handles.append(h)
 
         # Wait ensures the operation is enqueued, but not necessarily complete.
         launch_handles[-1].wait()
 
         # assign to param.data (not copy)
         for i, param in enumerate(param_list):
@@ -1323,41 +1327,44 @@
 
     def _allgather_params(self, param_list, hierarchy=0):
         if len(param_list) == 0:
             return
 
         partition_size = sum([param.ds_tensor.ds_numel for param in param_list])
 
-        tensor_size = partition_size * self.world_size
+        tensor_size = partition_size * self.num_partitions
         flat_tensor = torch.empty(tensor_size, dtype=param_list[0].dtype, device=self.local_device)
         flat_tensor.requires_grad = False
         partitions = []
-        for i in range(self.world_size):
+        for i in range(self.num_partitions):
             start = partition_size * i
 
             partitions.append(flat_tensor.narrow(0, start, partition_size))
 
-            if i == self.rank:
+            if i == self.get_partition_rank():
                 offset = 0
                 for param in param_list:
                     param_numel = param.ds_tensor.ds_numel
 
                     partitions[i].narrow(0, offset, param_numel).copy_(param.ds_tensor.data)
 
                     offset += param_numel
 
-        dist.all_gather(partitions, partitions[self.rank], group=self.ds_process_group, async_op=False)
+        dist.all_gather(partitions,
+                        partitions[self.get_partition_rank()],
+                        group=self.get_partition_dp_group(param),
+                        async_op=False)
         param_offset = 0
 
         for param in param_list:
             param_partition_size = param.ds_tensor.ds_numel
             param_size = param.ds_numel
             replicated_tensor = torch.empty(param.ds_shape, dtype=param.dtype, device=self.local_device)
 
-            for i in range(self.world_size):
+            for i in range(self.num_partitions):
 
                 start = i * partition_size
 
                 param_start = i * param_partition_size
 
                 if param_start < param_size:
                     numel_to_copy = min(param_size - param_start, param_partition_size)
@@ -1387,30 +1394,30 @@
             if handle is not None:
                 handle.wait()
 
             # some ranks may have partitions that are padded to go beyond the grad size.
             # For these ranks the output of reduce scatter is a separate buffer and needs
             # to be copied in
             partition_size = param.ds_tensor.ds_numel
-            start = self.rank * partition_size
+            start = self.get_partition_rank() * partition_size
             end = start + partition_size
             #print_rank_0("REduce scatter was executed for praam {param.ds_id}")
             if start < param.ds_numel and end > param.ds_numel:
                 elements = param.ds_numel - start
                 param.grad.view(-1).narrow(0, start, elements).copy_(reduced_partition.narrow(0, 0, elements))
 
     def _reduce_scatter_gradient(self, param):
 
         partition_size = param.ds_tensor.ds_numel
         #output = torch.empty(partition_size, dtype=param.dtype, device=param.device)
 
-        total_size = partition_size * self.world_size
+        total_size = partition_size * self.num_partitions
         input_list = []
 
-        for i in range(self.world_size):
+        for i in range(self.num_partitions):
 
             start = i * partition_size
             end = start + partition_size
 
             #print("before reduce scatter gradients")
             if start < param.ds_numel and end <= param.ds_numel:
                 input = param.grad.view(-1).narrow(0, start, partition_size)
@@ -1419,27 +1426,31 @@
 
                 if start < param.ds_numel:
                     elements = param.ds_numel - start
                     input.narrow(0, 0, elements).copy_(param.grad.view(-1).narrow(0, start, elements))
             #print("after reduce scatter gradients")
             input_list.append(input)
 
-        rank = dist.get_rank(group=self.ds_process_group)
-        handle = dist.reduce_scatter(input_list[rank], input_list, group=self.ds_process_group, async_op=True)
+        rank = dist.get_rank(group=self.get_partition_dp_group(param))
+        handle = dist.reduce_scatter(input_list[rank],
+                                     input_list,
+                                     group=self.get_partition_dp_group(param),
+                                     async_op=True)
 
         return handle, input_list[rank]
 
     def _partition_gradients(self, param_list, partition_buffers=None, accumulate=False):
         if partition_buffers is None:
             partition_buffers = [None] * len(param_list)
 
         for param, partition_buffer in zip(param_list, partition_buffers):
             self._partition_gradient(param, partition_buffer=partition_buffer, accumulate=accumulate)
 
     def _partition_gradient(self, param, partition_buffer=None, accumulate=False):
+
         #import pdb;pdb.set_trace()
         # param.grad=None
         # param.grad.test()
         print_rank_0(
             f"Partitioning param {param.ds_id} gradient of size {param.grad.numel()} type {param.grad.dtype} part_size {param.ds_tensor.ds_numel}"
         )
         see_memory_usage("Before partitioning gradients", force=False)
@@ -1448,15 +1459,15 @@
         if partition_buffer is None:
             assert not accumulate, "No buffer to accumulate to"
             partition_buffer = torch.zeros(partition_size, dtype=param.dtype, device=param.device)
         else:
             assert partition_buffer.numel(
             ) >= partition_size, f"The partition buffer size {partition_buffer.numel()} should match the size of param.ds_tensor {partition_size}"
 
-        rank = dist.get_rank(group=self.ds_process_group)
+        rank = dist.get_rank(group=self.get_partition_dp_group(param))
         start = partition_size * rank
         end = start + partition_size
 
         dest_tensor_full_buffer = partition_buffer.view(-1).narrow(0, 0, partition_size)
 
         #print("before partition gradients")
         if start < param.ds_numel:
@@ -1492,14 +1503,30 @@
             #                                             start,
             #                                             elements))
 
         #print("after partition gradients")
         param.grad.data = dest_tensor_full_buffer.data
         see_memory_usage("After partitioning gradients", force=False)
 
+    def get_partition_dp_group(self, param):
+        return param.ds_process_group
+
+    def get_partition_rank(self):
+        """subclass can overload to specify different relative rank in
+        parameter partition group"""
+        return self.rank
+
+    @property
+    def num_partitions(self):
+        return self.dp_world_size
+
+    def get_dp_process_group(self):
+        """ Return the communication group with all data-parallel ranks """
+        return self.ds_process_group
+
 
 class GatheredParameters:
 
     def __init__(self, params, modifier_rank=None, fwd_module=None, enabled=True):
         """A context that collects parameters that were partitioned via a
         :class:`deepspeed.zero.Init` context. The parameters are partitioned
         again upon exit.
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/partitioned_param_coordinator.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/partitioned_param_coordinator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/stage3.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/stage3.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,47 +143,47 @@
         self.offload_optimizer_pin_memory = False
         self.offload_optimizer_fast_init = False
         self.offload_param = False
         self.offload_param_pin_memory = False
         self.params_in_nvme_and_cpu = False
         self.max_params_in_cpu = 0
 
-        self.parameter_offload = DeepSpeedZeRoOffload(module=module,
-                                                      timers=timers,
-                                                      ds_config=ds_config,
-                                                      overlap_comm=overlap_comm,
-                                                      prefetch_bucket_size=prefetch_bucket_size,
-                                                      max_reuse_distance=max_reuse_distance,
-                                                      max_live_parameters=max_live_parameters,
-                                                      param_persistence_threshold=param_persistence_threshold,
-                                                      model_persistence_threshold=model_persistence_threshold,
-                                                      offload_param_config=offload_optimizer_config,
-                                                      mpu=mpu)
+        self.parameter_offload = self.initialize_ds_offload(module=module,
+                                                            timers=timers,
+                                                            ds_config=ds_config,
+                                                            overlap_comm=overlap_comm,
+                                                            prefetch_bucket_size=prefetch_bucket_size,
+                                                            max_reuse_distance=max_reuse_distance,
+                                                            max_live_parameters=max_live_parameters,
+                                                            param_persistence_threshold=param_persistence_threshold,
+                                                            model_persistence_threshold=model_persistence_threshold,
+                                                            offload_optimizer_config=offload_optimizer_config,
+                                                            mpu=mpu)
 
         self.persistent_parameters = self.parameter_offload.persistent_parameters
         self._configure_offloading(offload_optimizer_config, offload_param_config)
 
         self.module = module
         self.elastic_checkpoint = elastic_checkpoint
 
-        self.__inf_or_nan_tracker: Tensor = torch.zeros(1,
-                                                        dtype=torch.bool,
-                                                        device=get_accelerator().current_device_name(),
-                                                        requires_grad=False)
+        self.inf_or_nan_tracker: Tensor = torch.zeros(1,
+                                                      dtype=torch.bool,
+                                                      device=get_accelerator().current_device_name(),
+                                                      requires_grad=False)
 
         self.deepspeed_adam_offload = (self.offload_optimizer and type(init_optimizer) == DeepSpeedCPUAdam)
 
         self.device = get_accelerator().current_device_name() if not self.offload_optimizer else OffloadDeviceEnum.cpu
         ### streams used for overlapping computation with communication
-        self.__reduce_and_partition_stream = get_accelerator().Stream() if overlap_comm else get_accelerator(
+        self.reduce_and_partition_stream = get_accelerator().Stream() if overlap_comm else get_accelerator(
         ).default_stream()
 
         ############################################################################
 
-        self.__n_caching_allocator_flushes = 0
+        self.n_caching_allocator_flushes = 0
 
         #-------------Stage 3 Setup-------------------#
 
         self.timers = timers
 
         self.reduce_scatter = reduce_scatter
 
@@ -257,20 +257,20 @@
         num_fp16_subgroups = len(self.fp16_partitioned_groups_flat)
         see_memory_usage(f"After creating fp16 partitions: {num_fp16_subgroups}", force=True)
 
         # Optimizer tensor swapping
         if self.swap_optimizer:
             self._configure_tensor_swapping(offload_optimizer_config, aio_config)
 
-        self.__params_in_ipg_bucket: List[Parameter] = []
+        self.params_in_ipg_bucket = []
         self.is_gradient_accumulation_boundary: bool = True
 
-        self.__param_reduce_events: Deque[get_accelerator().Event] = collections.deque()
+        self.param_reduce_events: Deque[get_accelerator().Event] = collections.deque()
         # TODO. make this configurable via JSON
-        self.__max_param_reduce_events: int = 2
+        self.max_param_reduce_events: int = 2
 
         self.param_dict = {}
 
         # map between param_id and bool to specify if a param is in this partition
         self.is_param_in_current_partition = {}
 
         self.extra_large_param_to_reduce = None
@@ -336,14 +336,40 @@
 
         if dist.get_rank(group=self.dp_process_group) == 0:
             see_memory_usage(f"After initializing ZeRO optimizer", force=True)
 
     def destroy(self):
         self.parameter_offload.destroy()
 
+    def initialize_ds_offload(
+        self,
+        module,
+        timers,
+        ds_config,
+        overlap_comm,
+        prefetch_bucket_size,
+        max_reuse_distance,
+        max_live_parameters,
+        param_persistence_threshold,
+        model_persistence_threshold,
+        offload_optimizer_config,
+        mpu,
+    ):
+        return DeepSpeedZeRoOffload(module=module,
+                                    timers=timers,
+                                    ds_config=ds_config,
+                                    overlap_comm=overlap_comm,
+                                    prefetch_bucket_size=prefetch_bucket_size,
+                                    max_reuse_distance=max_reuse_distance,
+                                    max_live_parameters=max_live_parameters,
+                                    param_persistence_threshold=param_persistence_threshold,
+                                    model_persistence_threshold=model_persistence_threshold,
+                                    offload_param_config=offload_optimizer_config,
+                                    mpu=mpu)
+
     def _get_trainable_parameter_groups(self):
         param_groups = []
         for param_group in self.optimizer.param_groups:
             trainable_params = {"params": [p for p in param_group["params"] if p.requires_grad]}
             param_groups.append(trainable_params)
         return param_groups
 
@@ -475,15 +501,15 @@
                                               largest_numel=max(self.fp16_partitioned_groups_flat_numel),
                                               device=self.device,
                                               dtype=torch.float32,
                                               timers=self.timers)
 
     @property
     def elements_in_ipg_bucket(self):
-        return sum(p.ds_numel for p in self.__params_in_ipg_bucket)
+        return sum(p.ds_numel for p in self.params_in_ipg_bucket)
 
     def _move_to_flat_buffer(self, param_list, flat_buffer, avoid_copy=False):
         '''If flat buffer is None then the parameters in the param_list are
         not copied to the flat buffer. This is because they exceed the number of max_params_in_cpu
         Some of these parameters may already be in CPU in unflattened buffers
         or they maybe in GPU, or they maybe in NVME. If they are in NVME, then
         they will be marked as NOT_AVAILABLE, and will be moved to CPU when they are
@@ -829,14 +855,18 @@
 
         largest_numel = max([sum([p.ds_numel for p in psg]) for psg in self.fp16_partitioned_groups])
         gradient_dtype = self.fp32_partitioned_groups_flat[0].dtype
         gradient_buffer = torch.zeros(int(largest_numel), dtype=gradient_dtype, device=self.device)
 
         timer_names = set()
 
+        # State initialization for the Adagrad optimizer occurs at construction as opposed to other optimizers
+        # which do lazy initialization of the state at the first call to step.
+        is_adagrad = isinstance(self.optimizer, torch.optim.Adagrad)
+
         if self.swap_optimizer:
             self.optimizer_swapper.init_timers()
 
         INIT_OPTIMIZER_TIMER = 'init_optimizer_state'
         timer_names.add(INIT_OPTIMIZER_TIMER)
         self.start_timers([INIT_OPTIMIZER_TIMER])
 
@@ -858,26 +888,32 @@
                 if self.offload_optimizer_pin_memory:
                     subgroup_gradient_buffer = get_accelerator().pin_memory(subgroup_gradient_buffer)
 
                 self.fp32_partitioned_groups_flat[i].grad = subgroup_gradient_buffer
             else:
                 self.fp32_partitioned_groups_flat[i].grad = gradient_buffer.narrow(0, 0, num_elements)
 
-            self._optimizer_step(i)
+            # Initialize the optimizer states with the flattended fp32 partition.
+            if not is_adagrad:
+                self._optimizer_step(i)
 
             if swappable_param_subgroup:
                 self._partitioned_params_swap_out(i)
 
             if swappable_optimizer_subgroup:
                 self._optimizer_states_and_gradient_swap_out(i, timer_names)
 
             see_memory_usage(
                 f'[End] Initialize optimizer states {i} / {num_subgroups} subgroups, num_elems: {num_elements}, swappable opt/param:{swappable_optimizer_subgroup}/{swappable_param_subgroup}',
                 force=False)
 
+        # Initialize the optimizer states with the flattended fp32 partition.
+        if is_adagrad:
+            self.optimizer = torch.optim.Adagrad(self.fp32_partitioned_groups_flat, **self.optimizer.defaults)
+
         self.stop_timers([INIT_OPTIMIZER_TIMER])
         self.log_timers(timer_names)
 
         if self.swap_optimizer:
             self.optimizer_swapper.log_timers()
 
         if not self.offload_optimizer:
@@ -924,15 +960,15 @@
 
     @instrument_w_nvtx
     def independent_gradient_partition_epilogue(self):
         self.report_ipg_memory_usage(f"In ipg_epilogue before reduce_ipg_grads", 0)
         self.__reduce_and_partition_ipg_grads()
         self.report_ipg_memory_usage(f"In ipg_epilogue after reduce_ipg_grads", 0)
 
-        self.__reduce_and_partition_stream.synchronize()
+        self.reduce_and_partition_stream.synchronize()
 
         # if dist.get_rank() == 0:
         #    logger.info("Params already reduced %s", self.params_already_reduced)
         for i in range(len(self.params_already_reduced)):
             self.params_already_reduced[i] = False
 
         #in case of cpu offload, averaged gradients are already in fp32_partitioned_groups_flat.grad
@@ -1022,60 +1058,60 @@
             Multiple gradient reduction is currently not supported"
 
         self.__add_grad_to_ipg_bucket(param)
 
     @instrument_w_nvtx
     @torch.no_grad()
     def __add_grad_to_ipg_bucket(self, param: Parameter) -> None:
-        self.__reduce_and_partition_stream.wait_stream(get_accelerator().default_stream())
+        self.reduce_and_partition_stream.wait_stream(get_accelerator().default_stream())
 
         if self.contiguous_gradients and self.elements_in_ipg_bucket + param.grad.numel() < self.reduce_bucket_size:
             # move the gradient to a contiguous buffer
-            with get_accelerator().stream(self.__reduce_and_partition_stream):
+            with get_accelerator().stream(self.reduce_and_partition_stream):
                 # move the parameter's gradient to the contiguous flat buffer
                 new_grad_tensor = self.__ipg_bucket_flat_buffer.narrow(0, self.elements_in_ipg_bucket,
                                                                        param.grad.numel()).view_as(param.grad)
                 new_grad_tensor.copy_(param.grad, non_blocking=True)
                 param.grad.record_stream(get_accelerator().current_stream())
                 param.grad.data = new_grad_tensor
 
-        self.__params_in_ipg_bucket.append(param)
+        self.params_in_ipg_bucket.append(param)
 
     @instrument_w_nvtx
     @torch.no_grad()
     def __reduce_and_partition_ipg_grads(self, safe_mode: bool = False) -> None:
-        if not self.__params_in_ipg_bucket:
+        if not self.params_in_ipg_bucket:
             return
 
-        for param in self.__params_in_ipg_bucket:
+        for param in self.params_in_ipg_bucket:
             if param.grad.numel() != param.ds_numel:
                 raise RuntimeError(f"{param.grad.numel()} != {param.ds_numel} Cannot reduce scatter "
                                    f"gradients whose size is not same as the params")
 
-        self.__params_in_ipg_bucket.sort(key=lambda p: p.ds_id)
+        self.params_in_ipg_bucket.sort(key=lambda p: p.ds_id)
 
-        assert len(set(p.ds_id for p in self.__params_in_ipg_bucket)) == len(self.__params_in_ipg_bucket)
+        assert len(set(p.ds_id for p in self.params_in_ipg_bucket)) == len(self.params_in_ipg_bucket)
 
-        while self.__param_reduce_events and self.__param_reduce_events[0].query():
-            self.__param_reduce_events.popleft()
-        if len(self.__param_reduce_events) > self.__max_param_reduce_events:
-            self.__param_reduce_events.popleft().synchronize()
+        while self.param_reduce_events and self.param_reduce_events[0].query():
+            self.param_reduce_events.popleft()
+        if len(self.param_reduce_events) > self.max_param_reduce_events:
+            self.param_reduce_events.popleft().synchronize()
 
-        with get_accelerator().stream(self.__reduce_and_partition_stream):
+        with get_accelerator().stream(self.reduce_and_partition_stream):
             if safe_mode:
-                assert_ints_same_as_other_ranks([p.ds_id for p in self.__params_in_ipg_bucket])
+                assert_ints_same_as_other_ranks([p.ds_id for p in self.params_in_ipg_bucket])
 
-            grad_partitions = self.__avg_scatter_grads(self.__params_in_ipg_bucket)
-            self.__partition_grads(self.__params_in_ipg_bucket, grad_partitions)
+            grad_partitions = self.__avg_scatter_grads(self.params_in_ipg_bucket)
+            self.partition_grads(self.params_in_ipg_bucket, grad_partitions)
 
-            self.__params_in_ipg_bucket.clear()
+            self.params_in_ipg_bucket.clear()
 
             event = get_accelerator().Event()
             event.record()
-            self.__param_reduce_events.append(event)
+            self.param_reduce_events.append(event)
 
     @instrument_w_nvtx
     def __avg_scatter_grads(self, params_to_reduce: List[Parameter]) -> List[Tensor]:
         """average gradients and scatter partitions across ranks"""
 
         full_grads_for_rank = [p.grad for p in params_to_reduce]
         if self.communication_data_type != self.dtype:
@@ -1150,27 +1186,29 @@
 
         if total_norm == float('inf') or total_norm == -float('inf') or total_norm != total_norm:
             total_norm = -1
 
         return total_norm
 
     @instrument_w_nvtx
-    def __partition_grads(self, params_to_release: List[Parameter], grad_partitions: List[Tensor]) -> None:
+    def partition_grads(self, params_to_release: List[Parameter], grad_partitions: List[Tensor]) -> None:
         offload_fp32_gradients = {}
         offload_fp32_offsets = {}
+        buffers = []
         for param, grad_partition in zip(params_to_release, grad_partitions):
 
             contains_real_data = param.partition_numel() * dist.get_rank(self.dp_process_group) < param.ds_numel
             if not contains_real_data:
                 # this grad partition is empty - don't need to do anything
                 param.grad = None
                 continue
 
             # move or accumulate gradient partition to target buffer
             grad_buffer = self.__param_id_to_grad_partition[param.ds_id].narrow(0, 0, grad_partition.numel())
+            buffers.append(grad_buffer)
             if self.micro_step_id == 0:  # don't accumulate
                 grad_buffer.copy_(grad_partition, non_blocking=True)
                 # ensure grad buffer is a CUDA buffer to speed up the next few
                 # operations and so it can be used asynchronously
                 grad_buffer = grad_buffer.to(grad_partition.device, non_blocking=True)
             elif get_accelerator().on_accelerator(grad_buffer):
                 grad_buffer.add_(grad_partition)
@@ -1180,22 +1218,22 @@
                 cuda_grad_buffer = grad_buffer.to(grad_partition.device, non_blocking=True)
                 cuda_grad_buffer.add_(grad_partition)
                 grad_buffer.copy_(cuda_grad_buffer, non_blocking=True)
                 # ensure grad buffer is a CUDA buffer to speed up the next few
                 # operations and so it can be used asynchronously
                 grad_buffer = cuda_grad_buffer
 
-            if hasattr(self.__inf_or_nan_tracker, "logical_or_"):
-                self.__inf_or_nan_tracker.logical_or_(torch.isinf(grad_buffer).any())
-                self.__inf_or_nan_tracker.logical_or_(torch.isnan(grad_buffer).any())
+            if hasattr(self.inf_or_nan_tracker, "logical_or_"):
+                self.inf_or_nan_tracker.logical_or_(torch.isinf(grad_buffer).any())
+                self.inf_or_nan_tracker.logical_or_(torch.isnan(grad_buffer).any())
             else:
                 # logical_or_ not available in older versions of pytorch
-                self.__inf_or_nan_tracker += torch.isinf(grad_buffer).any()
-                self.__inf_or_nan_tracker += torch.isnan(grad_buffer).any()
-                self.__inf_or_nan_tracker = self.__inf_or_nan_tracker > 0
+                self.inf_or_nan_tracker += torch.isinf(grad_buffer).any()
+                self.inf_or_nan_tracker += torch.isnan(grad_buffer).any()
+                self.inf_or_nan_tracker = self.inf_or_nan_tracker > 0
 
             # offload the gradient partition if applicable
             if self.offload_optimizer:
                 i, dest_offset, _ = self.grad_position[self.get_param_id(param)]
 
                 if self.is_gradient_accumulation_boundary:
                     self.norm_for_param_grads[self.get_param_id(param)] = self._constant_buffered_norm2(grad_buffer)
@@ -1217,14 +1255,15 @@
             param.grad = None
 
         if self.offload_optimizer and self.swap_optimizer:
             for i in offload_fp32_gradients.keys():
                 self.optimizer_swapper.swap_out_gradients(parameter=self.fp32_partitioned_groups_flat[i],
                                                           gradient_offsets=offload_fp32_offsets[i],
                                                           gradient_tensors=offload_fp32_gradients[i])
+        return buffers
 
     def reduce_ready_partitions_and_remove_grads(self, param, i):
         #print_rank_0(f"Backward {debug_param2name_id_shape(param)}", force=True)
         self.reduce_independent_p_g_buckets_and_remove_grads(param, i)
 
     def zero_reduced_gradients(self, partition_id, i):
 
@@ -1778,26 +1817,26 @@
         self.stop_timers(['optimizer_step'])
 
         self._post_step(timer_names)
 
         # warn user about caching allocator flushes
         memory_stats = get_accelerator().memory_stats()
         alloc_retries = memory_stats["num_alloc_retries"] if memory_stats != None else 0
-        if alloc_retries > self.__n_caching_allocator_flushes:
+        if alloc_retries > self.n_caching_allocator_flushes:
             if dist.get_rank() == 0:
                 logger.warning(
                     "%d pytorch allocator cache flushes since last step. this happens "
                     "when there is high memory pressure and is detrimental to "
                     "performance. if this is happening frequently consider adjusting "
                     "settings to reduce memory consumption. If you are unable to "
                     "make the cache flushes go away consider adding "
                     "get_accelerator().empty_cache() calls in your training loop to ensure "
                     "that all ranks flush their caches at the same time",
-                    alloc_retries - self.__n_caching_allocator_flushes)
-            self.__n_caching_allocator_flushes = alloc_retries
+                    alloc_retries - self.n_caching_allocator_flushes)
+            self.n_caching_allocator_flushes = alloc_retries
 
     def dump_pre_step_gradients(self, debug_fp32_grads):
         # Dump gradient norms for debugging
         for i, _ in enumerate(self.fp16_groups):
             print(f'Pre-Step Dump Norms for Group {i} FP16P, FP16G, FP32G, FP32GUC')
             for fp16_param, fp32_grad in zip(self.fp16_groups[i], debug_fp32_grads[i]):
                 param_id = self.get_param_id(fp16_param)
@@ -1851,17 +1890,17 @@
                 if grad is not None and self._has_inf_or_nan(grad.data, j):
                     return True
         return False
 
     @instrument_w_nvtx
     def has_overflow(self, partition_gradients=True):
         if partition_gradients:
-            with get_accelerator().stream(self.__reduce_and_partition_stream):
-                self.local_overflow = bool(self.__inf_or_nan_tracker.item())
-                self.__inf_or_nan_tracker.zero_()
+            with get_accelerator().stream(self.reduce_and_partition_stream):
+                self.local_overflow = bool(self.inf_or_nan_tracker.item())
+                self.inf_or_nan_tracker.zero_()
 
             overflow = self.local_overflow
             #overflow = self.has_overflow_partitioned_grads_serial()
             overflow_gpu = get_accelerator().ByteTensor([overflow])
             dist.all_reduce(overflow_gpu, op=dist.ReduceOp.MAX, group=self.dp_process_group)
 
         else:
@@ -1927,15 +1966,15 @@
         if self.swap_optimizer:
             self.optimizer_swapper.post_backward()
 
     def get_fp32_grad_partitions(self) -> Dict[int, Dict[int, Tensor]]:
         """get fp32 gradient partition dictionary
         accessed as grad_dict[parameter_group_index][parameter_index]
         """
-        self.__reduce_and_partition_stream.synchronize()
+        self.reduce_and_partition_stream.synchronize()
         grad_dict = collections.defaultdict(dict)
         if self.offload_optimizer:
             for group in self.fp16_groups:
                 for param_idx, param in enumerate(group):
                     group_idx, dest_offset, num_elements = self.grad_position[self.get_param_id(param)]
                     fp32_grad = self.fp32_partitioned_groups_flat[group_idx].grad.narrow(0, dest_offset, num_elements)
                     grad_dict[group_idx][param_idx] = fp32_grad
@@ -1961,30 +2000,30 @@
 
         return reduce_buffer.narrow(0, 0, param.ds_numel).view(param.ds_shape)
 
     def get_fp32_grad_for_param(self, param) -> Tensor:
         if not param.requires_grad:
             return None
 
-        self.__reduce_and_partition_stream.synchronize()
+        self.reduce_and_partition_stream.synchronize()
 
         if self.offload_optimizer:
             group_idx, dest_offset, num_elements = self.grad_position[self.get_param_id(param)]
             fp32_grad = self.fp32_partitioned_groups_flat[group_idx].grad.narrow(0, dest_offset,
                                                                                  num_elements).to(device=param.device)
         else:
             fp32_grad = self.__param_id_to_grad_partition[param.ds_id].float()
 
         return self._fp32_state_allgather(param, fp32_grad)
 
     def get_full_hp_param(self, param, optim_state_key=None) -> Tensor:
         if not param.requires_grad:
             return None
 
-        self.__reduce_and_partition_stream.synchronize()
+        self.reduce_and_partition_stream.synchronize()
         group_idx, dest_offset, num_elements = self.grad_position[self.get_param_id(param)]
 
         if self._swappable_optimizer_subgroup(group_idx):
             self._optimizer_states_and_gradient_swap_in(group_idx)
 
         fp32_param = self.fp32_partitioned_groups_flat[group_idx]
         if optim_state_key is None:
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/stage_1_and_2.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/stage_1_and_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,15 +607,21 @@
         for i, group in enumerate(self.bit16_groups):
             single_grad_partition = torch.zeros(int(self.partition_size[i]),
                                                 dtype=self.single_partition_of_fp32_groups[i].dtype,
                                                 device=self.device)
             self.single_partition_of_fp32_groups[i].grad = get_accelerator().pin_memory(
                 single_grad_partition) if self.cpu_offload else single_grad_partition
 
-        self.optimizer.step()
+        # Initialize the optimizer states with the flattended fp32 partition.
+        # State initialization for the Adagrad optimizer occurs at construction as opposed to other optimizers
+        # which do lazy initialization of the state at the first call to step.
+        if isinstance(self.optimizer, torch.optim.Adagrad):
+            self.optimizer = torch.optim.Adagrad(self.single_partition_of_fp32_groups, **self.optimizer.defaults)
+        else:
+            self.optimizer.step()
 
         if not self.cpu_offload:
             for group in self.single_partition_of_fp32_groups:
                 group.grad = None  #class init
 
         return
 
@@ -835,22 +841,22 @@
 
         param_id = self.get_param_id(param)
         assert self.params_already_reduced[param_id] == False, \
             f"The parameter {param_id} has already been reduced. \
             Gradient computed twice for this partition. \
             Multiple gradient reduction is currently not supported"
 
-        if param.numel() > self.reduce_bucket_size:
-            self.extra_large_param_to_reduce = param
-
-        elif self.contiguous_gradients:
-            # keeping the gradients contiguous to prevent memory fragmentation, and avoid flattening
-            new_grad_tensor = self.ipg_buffer[self.ipg_index].narrow(0, self.elements_in_ipg_bucket, param.numel())
-            new_grad_tensor.copy_(param.grad.view(-1))
-            param.grad.data = new_grad_tensor.data.view_as(param.grad)
+        if self.contiguous_gradients:
+            if param.numel() > self.reduce_bucket_size:
+                self.extra_large_param_to_reduce = param
+            else:
+                # keeping the gradients contiguous to prevent memory fragmentation, and avoid flattening
+                new_grad_tensor = self.ipg_buffer[self.ipg_index].narrow(0, self.elements_in_ipg_bucket, param.numel())
+                new_grad_tensor.copy_(param.grad.view(-1))
+                param.grad.data = new_grad_tensor.data.view_as(param.grad)
 
         self.elements_in_ipg_bucket += param.numel()
 
         assert param.grad is not None, f"rank {dist.get_rank()} - Invalid to reduce Param {param_id} with None gradient"
 
         self.grads_in_ipg_bucket.append(param.grad)
         self.params_in_ipg_bucket.append((i, param, param_id))
@@ -1661,26 +1667,29 @@
             see_memory_usage('After overflow after clearing gradients')
 
             self.start_timers(timer_names)
             self.stop_timers(timer_names)
             return
 
         # Step 1:- Calculate gradient norm using fp-16 grads
-        see_memory_usage('Before norm calculation')
-        scaled_global_grad_norm = self.scaled_global_norm()
-        self._global_grad_norm = scaled_global_grad_norm / prev_scale
+        if self.dtype == torch.float16:
+            see_memory_usage('Before norm calculation')
+            scaled_global_grad_norm = self.scaled_global_norm()
+            self._global_grad_norm = scaled_global_grad_norm / prev_scale
+            see_memory_usage('After norm before optimizer')
 
-        see_memory_usage('After norm before optimizer')
         # Step 2:- run optimizer and upscaling simultaneously
         for i, group in enumerate(self.bit16_groups):
             self.start_timers([OPTIMIZER_GRADIENTS])
             partition_id = dist.get_rank(group=self.real_dp_process_group[i])
             if self.cpu_offload:
                 single_grad_partition = self.single_partition_of_fp32_groups[i].grad
-                self.unscale_and_clip_grads([single_grad_partition], scaled_global_grad_norm)
+                if self.dtype == torch.float16:
+                    self.unscale_and_clip_grads([single_grad_partition], scaled_global_grad_norm)
+
                 self.stop_timers([OPTIMIZER_GRADIENTS])
                 self.start_timers([OPTIMIZER_STEP])
                 self._optimizer_step(i)
 
                 # Disabled, this is not currently working
                 #from deepspeed.ops.adam import DeepSpeedCPUAdam
                 #if not (type(self.optimizer) == DeepSpeedCPUAdam and self.dtype == torch.half):
@@ -1711,15 +1720,17 @@
 
                 self.single_partition_of_fp32_groups[i].grad = single_grad_partition
                 # release all the gradient since we have already created a necessary copy in dp_grad_partition(ZeRO stage2)
                 self.free_grad_in_param_list(self.params_in_partition[i])
 
                 self.averaged_gradients[i] = None
 
-                self.unscale_and_clip_grads([single_grad_partition], scaled_global_grad_norm)
+                if self.dtype == torch.float16:
+                    self.unscale_and_clip_grads([single_grad_partition], scaled_global_grad_norm)
+
                 self.stop_timers([OPTIMIZER_GRADIENTS])
 
                 # Step 3:- run the optimizer if no offloading
                 self.start_timers([OPTIMIZER_STEP])
                 self._optimizer_step(i)
                 # Step 4:- get rid of the fp32 gradients. Not needed anymore
                 self.single_partition_of_fp32_groups[i].grad = None
```

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/test.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/test.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/tiling.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/tiling.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/runtime/zero/utils.py` & `deepspeed-0.9.2/deepspeed/runtime/zero/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 from typing import List
 
 import torch
 from deepspeed import comm as dist
 from deepspeed.utils import logger
 from deepspeed.ops.adam import DeepSpeedCPUAdam
+from deepspeed.ops.adagrad import DeepSpeedCPUAdagrad
 from deepspeed.ops.adam import FusedAdam
 from deepspeed.utils.nvtx import instrument_w_nvtx
 from deepspeed.accelerator import get_accelerator
 
 
 def _initialize_parameter_parallel_groups(parameter_parallel_size=None):
     data_parallel_size = int(dist.get_world_size())
@@ -31,15 +32,17 @@
     return my_group
 
 
 class ZeRORuntimeException(Exception):
     pass
 
 
-ZERO_SUPPORTED_OPTIMIZERS = [torch.optim.Adam, torch.optim.AdamW, FusedAdam, DeepSpeedCPUAdam]
+ZERO_SUPPORTED_OPTIMIZERS = [
+    torch.optim.Adam, torch.optim.AdamW, FusedAdam, DeepSpeedCPUAdam, torch.optim.Adagrad, DeepSpeedCPUAdagrad
+]
 
 # Add apex FusedAdam to supported list if apex is installed
 try:
     import apex
     if hasattr(apex, 'optimizers') and hasattr(apex.optimizers, 'FusedAdam'):
         ZERO_SUPPORTED_OPTIMIZERS.append(apex.optimizers.FusedAdam)
 except ImportError:
```

### Comparing `deepspeed-0.9.1/deepspeed/utils/__init__.py` & `deepspeed-0.9.2/deepspeed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/comms_logging.py` & `deepspeed-0.9.2/deepspeed/utils/comms_logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/debug.py` & `deepspeed-0.9.2/deepspeed/utils/debug.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/groups.py` & `deepspeed-0.9.2/deepspeed/utils/groups.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/init_on_device.py` & `deepspeed-0.9.2/deepspeed/utils/init_on_device.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/logging.py` & `deepspeed-0.9.2/deepspeed/utils/logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/mixed_precision_linkage.py` & `deepspeed-0.9.2/deepspeed/utils/mixed_precision_linkage.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/tensor_fragment.py` & `deepspeed-0.9.2/deepspeed/utils/tensor_fragment.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/timer.py` & `deepspeed-0.9.2/deepspeed/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/deepspeed/utils/zero_to_fp32.py` & `deepspeed-0.9.2/deepspeed/utils/zero_to_fp32.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,24 +116,16 @@
         # update with frozen parameters
         frozen_param_shapes = state_dict.get(FROZEN_PARAM_SHAPES, None)
         if frozen_param_shapes is not None:
             if debug:
                 print(f"Found frozen_param_shapes: {frozen_param_shapes}")
             param_names += list(frozen_param_shapes.keys())
 
-        # record shared parameters so that they can be recovered based on partners
-        # this is because such parameters holding reference only are not saved by optimizer
-        shared_params = []
-        for param in state_dict["module"]:
-            if param not in [*param_names, *buffer_names]:
-                for share_param in state_dict["module"]:
-                    if (state_dict["module"][share_param].data_ptr() == state_dict["module"][param].data_ptr()
-                            and share_param != param):
-                        shared_params.append([param, share_param])
-                        break
+        # handle shared params
+        shared_params = [[k, v] for k, v in state_dict["shared_params"].items()]
 
         ds_version = state_dict.get(DS_VERSION, None)
 
         frozen_param_fragments = state_dict.get(FROZEN_PARAM_FRAGMENTS, None)
 
         z_model_state = zero_model_state(buffers=buffers,
                                          param_shapes=param_shapes,
@@ -336,15 +328,16 @@
 
     _zero2_merge_frozen_params(state_dict, zero_model_states)
 
     _zero2_merge_trainable_params(state_dict, world_size, fp32_flat_groups, zero_model_states)
 
     # recover shared parameters
     for pair in zero_model_states[0].shared_params:
-        state_dict[pair[0]] = state_dict[pair[1]]
+        if pair[1] in state_dict:
+            state_dict[pair[0]] = state_dict[pair[1]]
 
     return state_dict
 
 
 def zero3_partitioned_param_info(unpartitioned_numel, world_size):
     remainder = unpartitioned_numel % world_size
     padding_numel = (world_size - remainder) if remainder else 0
@@ -453,15 +446,16 @@
 
     _zero3_merge_frozen_params(state_dict, world_size, zero_model_states)
 
     _zero3_merge_trainable_params(state_dict, world_size, fp32_flat_groups, zero_model_states)
 
     # recover shared parameters
     for pair in zero_model_states[0].shared_params:
-        state_dict[pair[0]] = state_dict[pair[1]]
+        if pair[1] in state_dict:
+            state_dict[pair[0]] = state_dict[pair[1]]
 
     return state_dict
 
 
 def get_fp32_state_dict_from_zero_checkpoint(checkpoint_dir, tag=None):
     """
     Convert ZeRO 2 or 3 checkpoint into a single fp32 consolidated state_dict that can be loaded with
```

### Comparing `deepspeed-0.9.1/deepspeed.egg-info/PKG-INFO` & `deepspeed-0.9.2/deepspeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.1
+Version: 0.9.2
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: MIT
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -27,14 +27,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
 [![Downloads](https://pepy.tech/badge/deepspeed)](https://pepy.tech/project/deepspeed)
 [![Build](https://badgen.net/badge/build/check-status/blue)](#build-pipeline-status)
+[![Twitter](https://img.shields.io/twitter/follow/MSFTDeepSpeed)](https://twitter.com/intent/follow?screen_name=MSFTDeepSpeed)
 
 
 <div align="center">
  <img src="docs/assets/images/DeepSpeed_light.svg#gh-light-mode-only" width="400px">
  <img src="docs/assets/images/DeepSpeed_dark_transparent.svg#gh-dark-mode-only" width="400px">
 </div>
 
@@ -122,15 +123,15 @@
 DeepSpeed has been integrated with several different popular open-source DL frameworks such as:
 
 |                                                                                                | Documentation                                |
 | ---------------------------------------------------------------------------------------------- | -------------------------------------------- |
 <img src="docs/assets/images/transformers-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/transformers-dark.png#gh-dark-mode-only" width="250px"> | [Transformers with DeepSpeed](https://huggingface.co/docs/transformers/main/main_classes/deepspeed) |
 | <img src="docs/assets/images/accelerate-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/accelerate-dark.png#gh-dark-mode-only" width="250px"> | [Accelerate with DeepSpeed](https://huggingface.co/docs/accelerate/usage_guides/deepspeed) |
 | <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://lightning.ai/docs/pytorch/stable/advanced/model_parallel.html#deepspeed) |
-| <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
+| <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/projects/composer/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
 | <img src="docs/assets/images/determined.svg" width="225px"> | [Determined with DeepSpeed](https://docs.determined.ai/latest/training/apis-howto/deepspeed/overview.html) |
 
 ---
 
 # Build Pipeline Status
 
 | Description | Status |
```

### Comparing `deepspeed-0.9.1/deepspeed.egg-info/SOURCES.txt` & `deepspeed-0.9.2/deepspeed.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -450,14 +450,16 @@
 deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
 deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
 deepspeed/runtime/swap_tensor/utils.py
 deepspeed/runtime/zero/__init__.py
 deepspeed/runtime/zero/config.py
 deepspeed/runtime/zero/contiguous_memory_allocator.py
 deepspeed/runtime/zero/linear.py
+deepspeed/runtime/zero/mics.py
+deepspeed/runtime/zero/mics_utils.py
 deepspeed/runtime/zero/offload_config.py
 deepspeed/runtime/zero/parameter_offload.py
 deepspeed/runtime/zero/partition_parameters.py
 deepspeed/runtime/zero/partitioned_param_coordinator.py
 deepspeed/runtime/zero/stage3.py
 deepspeed/runtime/zero/stage_1_and_2.py
 deepspeed/runtime/zero/test.py
```

### Comparing `deepspeed-0.9.1/deepspeed.egg-info/requires.txt` & `deepspeed-0.9.2/deepspeed.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,64 +10,62 @@
 
 [1bit]
 
 [1bit_mpi]
 mpi4py
 
 [all]
-pytest-xdist
+diffusers
 pytest
-torchvision
-packaging
-hjson
+sphinx
+future
+sphinx-rtd-theme
+psutil
+lm-eval==0.3.0
+triton==1.0.0
 torch
+transformers[sentencepiece]
+recommonmark
 protobuf
-tensorboard
-mpi4py
+tqdm
 google
-xgboost
-py-cpuinfo
-diffusers
+pydantic<2.0.0
+mpi4py
+clang-format==16.0.2
 pytest-forked
-triton==1.0.0
-pytest-randomly
-future
-sphinx-rtd-theme
-importlib-metadata>=4
-tqdm
 docutils<0.18
 wandb
-recommonmark
-triton==2.0.0.dev20221202
-megatron-lm==1.1.5
-pydantic<2.0.0
-pre-commit>=2.20.0
-sphinx
-transformers
-transformers[sentencepiece]
-psutil
-clang-format>=14.0.6
-lm-eval==0.3.0
+pytest-xdist
+packaging
+importlib-metadata>=4
+xgboost
 autodoc_pydantic<2.0.0
+torchvision
 tabulate
+py-cpuinfo
+pytest-randomly
+triton==2.0.0.dev20221202
+hjson
+transformers
+tensorboard
+pre-commit>=2.20.0
 
 [autotuning]
 tabulate
 
 [autotuning_ml]
 hjson
 tabulate
 xgboost
 
 [dev]
-clang-format>=14.0.6
+clang-format==16.0.2
 docutils<0.18
 future
 importlib-metadata>=4
-megatron-lm==1.1.5
 pre-commit>=2.20.0
 pytest
 pytest-forked
 pytest-randomly
 pytest-xdist
 recommonmark
 sphinx
```

### Comparing `deepspeed-0.9.1/op_builder/__init__.py` & `deepspeed-0.9.2/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/all_ops.py` & `deepspeed-0.9.2/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/async_io.py` & `deepspeed-0.9.2/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/builder.py` & `deepspeed-0.9.2/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/cpu_adagrad.py` & `deepspeed-0.9.2/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/cpu_adam.py` & `deepspeed-0.9.2/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/fused_adam.py` & `deepspeed-0.9.2/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/fused_lamb.py` & `deepspeed-0.9.2/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/quantizer.py` & `deepspeed-0.9.2/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/random_ltd.py` & `deepspeed-0.9.2/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/sparse_attn.py` & `deepspeed-0.9.2/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/spatial_inference.py` & `deepspeed-0.9.2/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/stochastic_transformer.py` & `deepspeed-0.9.2/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/transformer.py` & `deepspeed-0.9.2/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/op_builder/transformer_inference.py` & `deepspeed-0.9.2/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.1/setup.py` & `deepspeed-0.9.2/setup.py`

 * *Files identical despite different names*

