# Comparing `tmp/thinc-9.0.0.dev2.tar.gz` & `tmp/thinc-9.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinc-9.0.0.dev2.tar", last modified: Thu Jan 12 18:33:43 2023, max compression
+gzip compressed data, was "thinc-9.0.0.dev3.tar", last modified: Wed Mar 22 15:38:49 2023, max compression
```

## Comparing `thinc-9.0.0.dev2.tar` & `thinc-9.0.0.dev3.tar`

### file list

```diff
@@ -1,203 +1,206 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.184612 thinc-9.0.0.dev2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1123 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      222 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    13235 2023-01-12 18:33:43.184612 thinc-9.0.0.dev2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11536 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      248 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3442 2023-01-12 18:33:43.188612 thinc-9.0.0.dev2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     3799 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.132611 thinc-9.0.0.dev2/thinc/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      214 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/about.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5731 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/api.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.140611 thinc-9.0.0.dev2/thinc/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     5404 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2200 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/_cupy_allocators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18263 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/_custom_kernels.cu
--rw-r--r--   0 vsts      (1001) docker     (122)    21936 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/_custom_kernels.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/_murmur3.cu
--rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/_param_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2027 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/cblas.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2052 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/cblas.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    14601 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/cpu_kernels.hh
--rw-r--r--   0 vsts      (1001) docker     (122)    11756 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/cupy_ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)      581 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/mps_ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1989 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/numpy_ops.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    37228 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/numpy_ops.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    58365 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/backends/ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2474 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1280 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3833 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/initializers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.164611 thinc-9.0.0.dev2/thinc/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)     4262 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2246 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/add.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1587 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/array_getitem.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/bidirectional.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1741 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/cauchysimilarity.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3445 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/chain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4447 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/clipped_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)      649 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/clone.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5123 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/concatenate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2113 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/dish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2956 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/dropout.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2691 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/embed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1641 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/expand_window.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2120 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/gelu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2147 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/hard_swish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2194 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/hard_swish_mobilenet.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/hashembed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2535 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/list2array.py
--rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/list2padded.py
--rw-r--r--   0 vsts      (1001) docker     (122)      864 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/list2ragged.py
--rw-r--r--   0 vsts      (1001) docker     (122)      610 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/logistic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6450 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/lstm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1027 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/map_list.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2595 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/maxout.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2270 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/mish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1769 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/multisoftmax.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4299 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/mxnetwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)      703 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/padded2list.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2105 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/parametricattention.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12428 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/pytorchwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/ragged2list.py
--rw-r--r--   0 vsts      (1001) docker     (122)      816 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/reduce_first.py
--rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/reduce_last.py
--rw-r--r--   0 vsts      (1001) docker     (122)      721 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/reduce_max.py
--rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/reduce_mean.py
--rw-r--r--   0 vsts      (1001) docker     (122)      707 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/reduce_sum.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/relu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3091 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/remap_ids.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/residual.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2648 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/resizable.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1615 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/siamese.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1946 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/sigmoid.py
--rw-r--r--   0 vsts      (1001) docker     (122)      652 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/sigmoid_activation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3238 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/softmax.py
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/softmax_activation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8161 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/sparselinear.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      805 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/strings2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2128 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/swish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6516 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/tensorflowwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3286 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/torchscriptwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2018 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/tuplify.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2061 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/uniqued.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3521 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_array.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4080 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_array2d.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1426 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_cpu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1333 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_debug.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_flatten.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1954 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_flatten_v2.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1168 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_getitem.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2893 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_list.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1293 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_nvtx_range.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4857 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_padded.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4070 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_ragged.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_reshape.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1512 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/layers/with_signpost_interval.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.164611 thinc-9.0.0.dev2/thinc/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)      201 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11358 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/legacy/loss.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22962 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/loss.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11366 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/mypy.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14581 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/optimizers.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)     7808 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/schedules.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.164611 thinc-9.0.0.dev2/thinc/shims/
--rw-r--r--   0 vsts      (1001) docker     (122)      463 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4285 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/mxnet.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9354 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/pytorch.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6060 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/pytorch_grad_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2482 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10581 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/tensorflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2261 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/shims/torchscript.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.168611 thinc-9.0.0.dev2/thinc/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.172612 thinc-9.0.0.dev2/thinc/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      358 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/backends/test_mem.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48291 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/backends/test_ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2208 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.180611 thinc-9.0.0.dev2/thinc/tests/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2426 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_basic_tagger.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7807 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_combinators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5439 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_feed_forward.py
--rw-r--r--   0 vsts      (1001) docker     (122)      532 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_hash_embed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9719 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_layers_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7341 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5669 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_lstm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3673 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_mnist.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6275 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_mxnet_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6991 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_pytorch_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3694 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_reduce.py
--rw-r--r--   0 vsts      (1001) docker     (122)      943 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2869 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_softmax.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2289 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_sparse_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13090 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_tensorflow_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      810 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_torchscriptwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1975 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_transforms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_uniqued.py
--rw-r--r--   0 vsts      (1001) docker     (122)      801 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_with_debug.py
--rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_with_flatten.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10166 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/layers/test_with_transforms.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.180611 thinc-9.0.0.dev2/thinc/tests/model/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19914 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/model/test_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1369 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/model/test_validation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.180611 thinc-9.0.0.dev2/thinc/tests/mypy/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.180611 thinc-9.0.0.dev2/thinc/tests/mypy/configs/
--rw-r--r--   0 vsts      (1001) docker     (122)      195 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0 vsts      (1001) docker     (122)      217 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/configs/mypy-plugin.ini
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.180611 thinc-9.0.0.dev2/thinc/tests/mypy/modules/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/modules/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/modules/fail_no_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      565 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/modules/fail_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/modules/success_no_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/modules/success_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.184612 thinc-9.0.0.dev2/thinc/tests/mypy/outputs/
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/outputs/fail-no-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     2416 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/outputs/fail-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      576 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/outputs/success-no-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      494 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/outputs/success-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/mypy/test_mypy.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.184612 thinc-9.0.0.dev2/thinc/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/regression/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.184612 thinc-9.0.0.dev2/thinc/tests/regression/issue519/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/regression/issue519/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/regression/issue519/program.py
--rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/regression/issue519/test_issue519.py
--rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/regression/test_issue208.py
--rw-r--r--   0 vsts      (1001) docker     (122)      520 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/regression/test_issue564.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.184612 thinc-9.0.0.dev2/thinc/tests/shims/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/shims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3349 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/shims/test_pytorch_grad_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3586 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/strategies.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5702 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1749 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1800 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_import__all__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_indexing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      983 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_initializers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    27480 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_loss.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4997 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_optimizers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2528 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_schedules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6771 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1306 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5665 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3598 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)    47781 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20533 2023-01-12 18:33:05.000000 thinc-9.0.0.dev2/thinc/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-12 18:33:43.136611 thinc-9.0.0.dev2/thinc.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    13235 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5323 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)     1092 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-01-12 18:33:43.000000 thinc-9.0.0.dev2/thinc.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1123 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      222 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    13235 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    11536 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      248 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3442 2023-03-22 15:38:49.050978 thinc-9.0.0.dev3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     3829 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.026977 thinc-9.0.0.dev3/thinc/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      214 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/about.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5853 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/api.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.030977 thinc-9.0.0.dev3/thinc/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5404 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2200 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_cupy_allocators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18263 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_custom_kernels.cu
+-rw-r--r--   0 vsts      (1001) docker     (122)    21936 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_custom_kernels.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_murmur3.cu
+-rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_param_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2027 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cblas.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     2052 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cblas.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    14601 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cpu_kernels.hh
+-rw-r--r--   0 vsts      (1001) docker     (122)    11756 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cupy_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      581 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/mps_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1989 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/numpy_ops.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    37228 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/numpy_ops.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    58365 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/ops.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2474 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1280 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3833 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/initializers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.038977 thinc-9.0.0.dev3/thinc/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4315 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2246 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/add.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1587 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/array_getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/bidirectional.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1741 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/cauchysimilarity.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3445 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/chain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4447 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/clipped_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      649 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5181 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/concatenate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2113 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/dish.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2956 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/dropout.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2691 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/embed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1641 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/expand_window.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2120 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/gelu.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2147 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/hard_swish.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2194 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/hard_swish_mobilenet.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/hashembed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2535 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/linear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      878 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/list2array.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/list2padded.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      864 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/list2ragged.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      610 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/logistic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6450 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/lstm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1027 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/map_list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2595 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/maxout.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2270 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/mish.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1769 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/multisoftmax.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4299 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/mxnetwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      703 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/padded2list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2105 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/parametricattention.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/premap_ids.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    12428 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/pytorchwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/ragged2list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      816 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_first.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_last.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      721 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_max.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_mean.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      707 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_sum.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/relu.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3091 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/remap_ids.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/residual.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2755 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/resizable.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1615 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/siamese.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1946 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/sigmoid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      652 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/sigmoid_activation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3238 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/softmax.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/softmax_activation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8161 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/sparselinear.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      805 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/strings2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2128 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/swish.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6516 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/tensorflowwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3286 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/torchscriptwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2018 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/tuplify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2061 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/uniqued.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3579 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_array.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4137 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_array2d.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1426 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_cpu.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1333 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_flatten.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1954 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_flatten_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1168 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2893 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1293 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_nvtx_range.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4857 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_padded.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4447 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_ragged.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_reshape.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1512 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_signpost_interval.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.038977 thinc-9.0.0.dev3/thinc/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)      201 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11358 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/legacy/loss.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22962 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/loss.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11466 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/mypy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14581 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/optimizers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)    11359 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/schedules.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.038977 thinc-9.0.0.dev3/thinc/shims/
+-rw-r--r--   0 vsts      (1001) docker     (122)      463 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4285 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/mxnet.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9354 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/pytorch.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6060 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/pytorch_grad_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2482 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/shim.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10581 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/tensorflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2261 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/torchscript.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.042977 thinc-9.0.0.dev3/thinc/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.042977 thinc-9.0.0.dev3/thinc/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      358 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/backends/test_mem.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48394 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/backends/test_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2208 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2426 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_basic_tagger.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7807 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_combinators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5439 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_feed_forward.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      532 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_hash_embed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9830 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_layers_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7341 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5669 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_lstm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1649 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_mappers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3673 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_mnist.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6275 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_mxnet_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6991 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_pytorch_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3694 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_reduce.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      872 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_resizable.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      943 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2869 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_softmax.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2289 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_sparse_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13090 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_tensorflow_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      810 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_torchscriptwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1975 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_transforms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_uniqued.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      801 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_with_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_with_flatten.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10166 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_with_transforms.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/model/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19914 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/model/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1369 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/model/test_validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/configs/
+-rw-r--r--   0 vsts      (1001) docker     (122)      195 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)      217 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/configs/mypy-plugin.ini
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/modules/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/fail_no_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      565 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/fail_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/success_no_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/success_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/fail-no-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     2416 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/fail-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      576 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/success-no-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      494 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/success-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/test_mypy.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/regression/issue519/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/issue519/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/issue519/program.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/issue519/test_issue519.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/test_issue208.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      520 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/test_issue564.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/shims/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/shims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3349 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/shims/test_pytorch_grad_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3586 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/strategies.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5702 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1749 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1800 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_import__all__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_indexing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      983 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_initializers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    27480 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_loss.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4997 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_optimizers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3491 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6771 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1306 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6573 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3598 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    47781 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20964 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.026977 thinc-9.0.0.dev3/thinc.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    13235 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-03-22 15:38:49.000000 thinc-9.0.0.dev3/thinc.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)     1092 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/top_level.txt
```

### Comparing `thinc-9.0.0.dev2/LICENSE` & `thinc-9.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/PKG-INFO` & `thinc-9.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinc
-Version: 9.0.0.dev2
+Version: 9.0.0.dev3
 Summary: A refreshing functional take on deep learning, compatible with your favorite libraries
 Home-page: https://github.com/explosion/thinc
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev2 Summary: A refreshing
+Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev3 Summary: A refreshing
 functional take on deep learning, compatible with your favorite libraries Home-
 page: https://github.com/explosion/thinc Author: Explosion Author-email:
 contact@explosion.ai License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
```

### Comparing `thinc-9.0.0.dev2/README.md` & `thinc-9.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/setup.cfg` & `thinc-9.0.0.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/setup.py` & `thinc-9.0.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 PACKAGES = find_packages()
 MOD_NAMES = [
     "thinc.backends.cblas",
     "thinc.backends.numpy_ops",
     "thinc.layers.sparselinear",
+    "thinc.layers.premap_ids"
 ]
 COMPILE_OPTIONS = {
     "msvc": ["/Ox", "/EHsc"],
     "other": ["-O3", "-Wno-strict-prototypes", "-Wno-unused-function", "-std=c++11"],
 }
 COMPILER_DIRECTIVES = {
     "language_level": 3,
```

### Comparing `thinc-9.0.0.dev2/thinc/api.py` & `thinc-9.0.0.dev3/thinc/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .model import Model, serialize_attr, deserialize_attr
 from .model import set_dropout_rate, change_attr_values, wrap_model_recursive
 from .shims import Shim, PyTorchGradScaler, PyTorchShim, TensorFlowShim, keras_model_fns
 from .shims import MXNetShim, TorchScriptShim, maybe_handshake_model
 from .optimizers import Adam, RAdam, SGD, Optimizer
 from .schedules import Schedule, cyclic_triangular, warmup_linear, constant
 from .schedules import constant_then, decaying, slanted_triangular, compounding
+from .schedules import plateau
 from .types import Ragged, Padded, ArgsKwargs, Unserializable
 from .util import fix_random_seed, is_cupy_array, set_active_gpu
 from .util import prefer_gpu, require_gpu, require_cpu
 from .util import DataValidationError, data_validation
 from .util import to_categorical, get_width, get_array_module, to_numpy
 from .util import torch2xp, xp2torch, tensorflow2xp, xp2tensorflow, mxnet2xp, xp2mxnet
 from .util import get_torch_default_device
@@ -35,15 +36,16 @@
 
 from .layers import add, bidirectional, chain, clone, concatenate, noop
 from .layers import residual, uniqued, siamese, list2ragged, ragged2list
 from .layers import map_list
 from .layers import with_array, with_array2d
 from .layers import with_padded, with_list, with_ragged, with_flatten
 from .layers import with_reshape, with_getitem, strings2arrays, list2array
-from .layers import list2ragged, ragged2list, list2padded, padded2list, remap_ids
+from .layers import list2ragged, ragged2list, list2padded, padded2list
+from .layers import remap_ids, remap_ids_v2, premap_ids
 from .layers import array_getitem, with_cpu, with_debug, with_nvtx_range
 from .layers import with_signpost_interval
 from .layers import tuplify, with_flatten_v2
 
 from .layers import reduce_first, reduce_last, reduce_max, reduce_mean, reduce_sum
 
 
@@ -63,15 +65,15 @@
     # .shims
     "Shim", "PyTorchGradScaler", "PyTorchShim", "TensorFlowShim", "keras_model_fns",
     "MXNetShim", "TorchScriptShim", "maybe_handshake_model",
     # .optimizers
     "Adam", "RAdam", "SGD", "Optimizer",
     # .schedules
     "Schedule", "cyclic_triangular", "warmup_linear", "constant", "constant_then",
-    "decaying", "slanted_triangular", "compounding",
+    "decaying", "slanted_triangular", "compounding", "plateau",
     # .types
     "Ragged", "Padded", "ArgsKwargs", "Unserializable",
     # .util
     "fix_random_seed", "is_cupy_array", "set_active_gpu",
     "prefer_gpu", "require_gpu", "require_cpu",
     "DataValidationError", "data_validation",
     "to_categorical", "get_width", "get_array_module", "to_numpy",
@@ -97,15 +99,16 @@
 
     "add", "bidirectional", "chain", "clone", "concatenate", "noop",
     "residual", "uniqued", "siamese", "list2ragged", "ragged2list",
     "map_list",
     "with_array", "with_array2d",
     "with_padded", "with_list", "with_ragged", "with_flatten",
     "with_reshape", "with_getitem", "strings2arrays", "list2array",
-    "list2ragged", "ragged2list", "list2padded", "padded2list", "remap_ids",
+    "list2ragged", "ragged2list", "list2padded", "padded2list", 
+    "remap_ids", "remap_ids_v2", "premap_ids",
     "array_getitem", "with_cpu", "with_debug", "with_nvtx_range",
     "with_signpost_interval",
     "tuplify", "with_flatten_v2",
     "pytorch_to_torchscript_wrapper",
 
     "reduce_first", "reduce_last", "reduce_max", "reduce_mean", "reduce_sum",
 ]
```

### Comparing `thinc-9.0.0.dev2/thinc/backends/__init__.py` & `thinc-9.0.0.dev3/thinc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/_cupy_allocators.py` & `thinc-9.0.0.dev3/thinc/backends/_cupy_allocators.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/_custom_kernels.cu` & `thinc-9.0.0.dev3/thinc/backends/_custom_kernels.cu`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/_custom_kernels.py` & `thinc-9.0.0.dev3/thinc/backends/_custom_kernels.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/_murmur3.cu` & `thinc-9.0.0.dev3/thinc/backends/_murmur3.cu`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/_param_server.py` & `thinc-9.0.0.dev3/thinc/backends/_param_server.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/cblas.pxd` & `thinc-9.0.0.dev3/thinc/backends/cblas.pxd`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/cblas.pyx` & `thinc-9.0.0.dev3/thinc/backends/cblas.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/cpu_kernels.hh` & `thinc-9.0.0.dev3/thinc/backends/cpu_kernels.hh`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/cupy_ops.py` & `thinc-9.0.0.dev3/thinc/backends/cupy_ops.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/mps_ops.py` & `thinc-9.0.0.dev3/thinc/backends/mps_ops.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/numpy_ops.pxd` & `thinc-9.0.0.dev3/thinc/backends/numpy_ops.pxd`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/numpy_ops.pyx` & `thinc-9.0.0.dev3/thinc/backends/numpy_ops.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/backends/ops.py` & `thinc-9.0.0.dev3/thinc/backends/ops.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/compat.py` & `thinc-9.0.0.dev3/thinc/compat.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/config.py` & `thinc-9.0.0.dev3/thinc/config.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/initializers.py` & `thinc-9.0.0.dev3/thinc/initializers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/__init__.py` & `thinc-9.0.0.dev3/thinc/layers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 # Data-type transfers
 from .list2array import list2array
 from .list2ragged import list2ragged
 from .list2padded import list2padded
 from .ragged2list import ragged2list
 from .padded2list import padded2list
 from .remap_ids import remap_ids, remap_ids_v2
+from .premap_ids import premap_ids
 from .strings2arrays import strings2arrays
 from .with_array import with_array
 from .with_array2d import with_array2d
 from .with_cpu import with_cpu
 from .with_flatten import with_flatten
 from .with_flatten_v2 import with_flatten_v2
 from .with_padded import with_padded
@@ -137,14 +138,15 @@
     "with_flatten",
     "with_flatten_v2",
     "with_debug",
     "with_nvtx_range",
     "with_signpost_interval",
     "remap_ids",
     "remap_ids_v2",
+    "premap_ids",
     "softmax_activation",
     "Logistic",
     "Sigmoid",
     "ClippedLinear",
     "ReluK",
     "HardTanh",
     "HardSigmoid",
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/add.py` & `thinc-9.0.0.dev3/thinc/layers/add.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/array_getitem.py` & `thinc-9.0.0.dev3/thinc/layers/array_getitem.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/bidirectional.py` & `thinc-9.0.0.dev3/thinc/layers/bidirectional.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/cauchysimilarity.py` & `thinc-9.0.0.dev3/thinc/layers/cauchysimilarity.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/chain.py` & `thinc-9.0.0.dev3/thinc/layers/chain.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/clipped_linear.py` & `thinc-9.0.0.dev3/thinc/layers/clipped_linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/clone.py` & `thinc-9.0.0.dev3/thinc/layers/clone.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/concatenate.py` & `thinc-9.0.0.dev3/thinc/layers/concatenate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import Any, List, Tuple, Callable, Optional
 from typing import TypeVar, cast, Dict, Union, Sequence
+
+from ..backends import NumpyOps
 from ..model import Model
 from ..config import registry
 from ..types import Array2d, Ragged
 from ..util import get_width
 from .noop import noop
 from ..types import XY_XY_OutT
 
 
+NUMPY_OPS = NumpyOps()
+
+
 InT = TypeVar("InT", bound=Any)
 OutT = TypeVar("OutT", bound=Union[Array2d, Sequence[Array2d], Ragged])
 
 
 @registry.layers("concatenate.v1")
 def concatenate(*layers: Model) -> Model[InT, XY_XY_OutT]:
     """Compose two or more models `f`, `g`, etc, such that their outputs are
@@ -116,15 +121,15 @@
         for bwd, width in zip(callbacks[1:], widths[1:]):
             dY = model.ops.as_contig(d_out_array[:, start : start + width])
             dY = model.ops.unflatten(dY, lengths)
             dX += bwd(dY)
             start += width
         return dX
 
-    lengths = model.ops.asarray1i([len(x) for x in X])
+    lengths = NUMPY_OPS.asarray1i([len(x) for x in X])
     Ys = [model.ops.xp.concatenate(Y, axis=0) for Y in Ys]
     widths = [Y.shape[1] for Y in Ys]
     out_array = model.ops.xp.hstack(Ys)
     return model.ops.unflatten(out_array, lengths), backprop
 
 
 def init(
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/dish.py` & `thinc-9.0.0.dev3/thinc/layers/dish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/dropout.py` & `thinc-9.0.0.dev3/thinc/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/embed.py` & `thinc-9.0.0.dev3/thinc/layers/embed.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/expand_window.py` & `thinc-9.0.0.dev3/thinc/layers/expand_window.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/gelu.py` & `thinc-9.0.0.dev3/thinc/layers/gelu.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/hard_swish.py` & `thinc-9.0.0.dev3/thinc/layers/hard_swish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/hard_swish_mobilenet.py` & `thinc-9.0.0.dev3/thinc/layers/hard_swish_mobilenet.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/hashembed.py` & `thinc-9.0.0.dev3/thinc/layers/hashembed.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/layernorm.py` & `thinc-9.0.0.dev3/thinc/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/linear.py` & `thinc-9.0.0.dev3/thinc/layers/linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/list2array.py` & `thinc-9.0.0.dev3/thinc/layers/list2array.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from typing import Tuple, Callable, TypeVar, List, Union, cast
+from typing import Tuple, Callable, TypeVar, List
 
+from ..backends import NumpyOps
 from ..model import Model
 from ..config import registry
 from ..types import Array2d
 
 
+NUMPY_OPS = NumpyOps()
+
+
 OutT = TypeVar("OutT", bound=Array2d)
 InT = List[OutT]
 
 
 @registry.layers("list2array.v1")
 def list2array() -> Model[InT, OutT]:
     """Transform sequences to ragged arrays if necessary and return the data
     from the ragged array. If sequences are already ragged, do nothing. A
     ragged array is a tuple (data, lengths), where data is the concatenated data.
     """
     return Model("list2array", forward)
 
 
 def forward(model: Model[InT, OutT], Xs: InT, is_train: bool) -> Tuple[OutT, Callable]:
-    lengths = model.ops.asarray1i([len(x) for x in Xs])
+    lengths = NUMPY_OPS.asarray1i([len(x) for x in Xs])
 
     def backprop(dY: OutT) -> InT:
         return model.ops.unflatten(dY, lengths)
 
     return model.ops.flatten(Xs), backprop
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/list2padded.py` & `thinc-9.0.0.dev3/thinc/layers/list2padded.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/list2ragged.py` & `thinc-9.0.0.dev3/thinc/layers/list2ragged.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/logistic.py` & `thinc-9.0.0.dev3/thinc/layers/logistic.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/lstm.py` & `thinc-9.0.0.dev3/thinc/layers/lstm.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/map_list.py` & `thinc-9.0.0.dev3/thinc/layers/map_list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/maxout.py` & `thinc-9.0.0.dev3/thinc/layers/maxout.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/mish.py` & `thinc-9.0.0.dev3/thinc/layers/mish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/multisoftmax.py` & `thinc-9.0.0.dev3/thinc/layers/multisoftmax.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/mxnetwrapper.py` & `thinc-9.0.0.dev3/thinc/layers/mxnetwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/noop.py` & `thinc-9.0.0.dev3/thinc/layers/noop.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/padded2list.py` & `thinc-9.0.0.dev3/thinc/layers/padded2list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/parametricattention.py` & `thinc-9.0.0.dev3/thinc/layers/parametricattention.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/pytorchwrapper.py` & `thinc-9.0.0.dev3/thinc/layers/pytorchwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/ragged2list.py` & `thinc-9.0.0.dev3/thinc/layers/ragged2list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/reduce_first.py` & `thinc-9.0.0.dev3/thinc/layers/reduce_first.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/reduce_last.py` & `thinc-9.0.0.dev3/thinc/layers/reduce_last.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/reduce_max.py` & `thinc-9.0.0.dev3/thinc/layers/reduce_max.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/reduce_mean.py` & `thinc-9.0.0.dev3/thinc/layers/reduce_mean.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/reduce_sum.py` & `thinc-9.0.0.dev3/thinc/layers/reduce_sum.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/relu.py` & `thinc-9.0.0.dev3/thinc/layers/relu.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/remap_ids.py` & `thinc-9.0.0.dev3/thinc/layers/remap_ids.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/residual.py` & `thinc-9.0.0.dev3/thinc/layers/residual.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/resizable.py` & `thinc-9.0.0.dev3/thinc/layers/resizable.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
     # return the original layer if it wasn't initialized or if nO didn't change
     if layer.has_dim("nO") is None:
         layer.set_dim("nO", new_nO)
         return layer
     elif new_nO == layer.get_dim("nO"):
         return layer
+    elif layer.has_dim("nI") is None:
+        layer.set_dim("nO", new_nO, force=True)
+        return layer
 
     dims = {name: layer.maybe_get_dim(name) for name in layer.dim_names}
     dims["nO"] = new_nO
     new_layer: Model[Floats2d, Floats2d] = Model(
         layer.name,
         layer._func,
         dims=dims,
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/siamese.py` & `thinc-9.0.0.dev3/thinc/layers/siamese.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/sigmoid.py` & `thinc-9.0.0.dev3/thinc/layers/sigmoid.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/sigmoid_activation.py` & `thinc-9.0.0.dev3/thinc/layers/sigmoid_activation.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/softmax.py` & `thinc-9.0.0.dev3/thinc/layers/softmax.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/softmax_activation.py` & `thinc-9.0.0.dev3/thinc/layers/softmax_activation.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/sparselinear.pyx` & `thinc-9.0.0.dev3/thinc/layers/sparselinear.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/strings2arrays.py` & `thinc-9.0.0.dev3/thinc/layers/strings2arrays.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/swish.py` & `thinc-9.0.0.dev3/thinc/layers/swish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/tensorflowwrapper.py` & `thinc-9.0.0.dev3/thinc/layers/tensorflowwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/torchscriptwrapper.py` & `thinc-9.0.0.dev3/thinc/layers/torchscriptwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/tuplify.py` & `thinc-9.0.0.dev3/thinc/layers/tuplify.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/uniqued.py` & `thinc-9.0.0.dev3/thinc/layers/uniqued.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_array.py` & `thinc-9.0.0.dev3/thinc/layers/with_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import Tuple, Callable, Optional, TypeVar, Union, cast
 
+from ..backends import NumpyOps
 from ..model import Model
 from ..config import registry
 from ..types import Padded, Ragged, ArrayXd, Array3d, ListXd
 
+
+NUMPY_OPS = NumpyOps()
+
+
 ArrayTXd = TypeVar("ArrayTXd", bound=ArrayXd)
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, ListXd, ArrayXd])
 
 
 @registry.layers("with_array.v1")
 def with_array(layer: Model[ArrayTXd, ArrayTXd], pad: int = 0) -> Model[SeqT, SeqT]:
     """Transform sequence data into a contiguous array on the way into and
@@ -64,15 +69,15 @@
 
 
 def _list_forward(
     model: Model[SeqT, SeqT], Xs: ListXd, is_train: bool
 ) -> Tuple[ListXd, Callable]:
     layer: Model[ArrayXd, ArrayXd] = model.layers[0]
     pad = model.attrs["pad"]
-    lengths = layer.ops.asarray1i([len(seq) for seq in Xs])
+    lengths = NUMPY_OPS.asarray1i([len(seq) for seq in Xs])
     Xf = layer.ops.flatten(Xs, pad=pad)
     Yf, get_dXf = layer(Xf, is_train)
 
     def backprop(dYs: ListXd) -> ListXd:
         dYf = layer.ops.flatten(dYs, pad=pad)
         dXf = get_dXf(dYf)
         return layer.ops.unflatten(dXf, lengths, pad=pad)
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_array2d.py` & `thinc-9.0.0.dev3/thinc/layers/with_array2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Tuple, Callable, Optional, TypeVar, cast, List, Union
 
+from ..backends import NumpyOps
 from ..model import Model
 from ..config import registry
 from ..types import Array2d, Floats2d, List2d, Padded, Ragged
 
 
+NUMPY_OPS = NumpyOps()
+
+
 ValT = TypeVar("ValT", bound=Array2d)
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, List2d, Array2d])
 
 
 @registry.layers("with_array2d.v1")
 def with_array2d(layer: Model[ValT, ValT], pad: int = 0) -> Model[SeqT, SeqT]:
     """Transform sequence data into a contiguous 2d array on the way into and
@@ -67,15 +71,15 @@
 
 
 def _list_forward(
     model: Model[SeqT, SeqT], Xs: List2d, is_train: bool
 ) -> Tuple[List2d, Callable]:
     layer: Model[Array2d, Array2d] = model.layers[0]
     pad = model.attrs["pad"]
-    lengths = layer.ops.asarray1i([len(seq) for seq in Xs])
+    lengths = NUMPY_OPS.asarray1i([len(seq) for seq in Xs])
     Xf = layer.ops.flatten(Xs, pad=pad)
     Yf, get_dXf = layer(Xf, is_train)
 
     def backprop(dYs: List2d) -> List2d:
         dYf = layer.ops.flatten(dYs, pad=pad)
         dXf = get_dXf(dYf)
         return layer.ops.unflatten(dXf, lengths, pad=pad)
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_cpu.py` & `thinc-9.0.0.dev3/thinc/layers/with_cpu.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_debug.py` & `thinc-9.0.0.dev3/thinc/layers/with_debug.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_flatten.py` & `thinc-9.0.0.dev3/thinc/layers/with_flatten.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_flatten_v2.py` & `thinc-9.0.0.dev3/thinc/layers/with_flatten_v2.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_getitem.py` & `thinc-9.0.0.dev3/thinc/layers/with_getitem.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_list.py` & `thinc-9.0.0.dev3/thinc/layers/with_list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_nvtx_range.py` & `thinc-9.0.0.dev3/thinc/layers/with_nvtx_range.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_padded.py` & `thinc-9.0.0.dev3/thinc/layers/with_padded.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_ragged.py` & `thinc-9.0.0.dev3/thinc/layers/with_ragged.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import Tuple, Callable, Optional, TypeVar, cast, List, Union
 
+from ..backends import NumpyOps
 from ..types import Padded, Ragged, Array2d, ListXd, List2d, Ints1d
 from ..model import Model
 from ..config import registry
 
+
+NUMPY_OPS = NumpyOps()
+
+
 RaggedData = Tuple[Array2d, Ints1d]
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, ListXd, RaggedData])
 
 
 @registry.layers("with_ragged.v1")
 def with_ragged(layer: Model[Ragged, Ragged]) -> Model[SeqT, SeqT]:
     return Model(f"with_ragged({layer.name})", forward, init=init, layers=[layer])
@@ -85,17 +90,20 @@
     flatten = layer.ops.flatten
     # It's worth being a bit careful about memory here, as the activations
     # are potentially large on GPU. So we make nested function calls instead
     # of assigning to temporaries where possible, so memory can be reclaimed
     # sooner.
     Xs = padded2list(Xp)
     # Bit annoying here: padded is in a different order, so we need to make new
-    # lengths.
-    lengths = layer.ops.asarray1i([len(x) for x in Xs])
-    Yr, get_dXr = layer(Ragged(flatten(Xs), lengths), is_train)
+    # lengths. The lengths are unconditionally allocated in CPU memory, because
+    # otherwire unflatten would move GPU allocations to the CPU again. For the
+    # ragged arrays we let the layer's ops determine how lengths should be
+    # stored to ensure that the array and lengths use the same type of memory.
+    lengths = NUMPY_OPS.asarray1i([len(x) for x in Xs])
+    Yr, get_dXr = layer(Ragged(flatten(Xs), layer.ops.asarray1i(lengths)), is_train)
 
     def backprop(dYp: Padded):
         flattened = flatten(padded2list(dYp))
         dXr = get_dXr(Ragged(flattened, lengths))
         return list2padded(unflatten(dXr.data, lengths))
 
     return (
@@ -107,15 +115,15 @@
 def _list_forward(
     layer: Model[Ragged, Ragged], Xs: List, is_train: bool
 ) -> Tuple[List, Callable]:
     # Assign these to locals, to keep code a bit shorter.
     flatten = layer.ops.flatten
     unflatten = layer.ops.unflatten
 
-    lengths = layer.ops.asarray1i([len(x) for x in Xs])
-    Yr, get_dXr = layer(Ragged(flatten(Xs), lengths), is_train)
+    lengths = [len(x) for x in Xs]
+    Yr, get_dXr = layer(Ragged(flatten(Xs), layer.ops.asarray1i(lengths)), is_train)
 
     def backprop(dYs):
         flattened = flatten(dYs)
         return unflatten(get_dXr(Ragged(flattened, lengths)).data, lengths)
 
     return unflatten(Yr.data, Yr.lengths), backprop
```

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_reshape.py` & `thinc-9.0.0.dev3/thinc/layers/with_reshape.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/layers/with_signpost_interval.py` & `thinc-9.0.0.dev3/thinc/layers/with_signpost_interval.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/legacy/loss.py` & `thinc-9.0.0.dev3/thinc/legacy/loss.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/loss.py` & `thinc-9.0.0.dev3/thinc/loss.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/model.py` & `thinc-9.0.0.dev3/thinc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         example input and output data to perform shape inference."""
         if DATA_VALIDATION.get():
             validate_fwd_input_output(self.name, self._func, X, Y)
         if self.init is not None:
             self.init(self, X=X, Y=Y)
         return self
 
-    def begin_update(self, X: InT) -> Tuple[OutT, Callable[[InT], OutT]]:
+    def begin_update(self, X: InT) -> Tuple[OutT, Callable[[OutT], InT]]:
         """Run the model over a batch of data, returning the output and a
         callback to complete the backward pass. A tuple (Y, finish_update),
         where Y is a batch of output data, and finish_update is a callback that
         takes the gradient with respect to the output and an optimizer function,
         and returns the gradient with respect to the input.
         """
         return self._func(self, X, is_train=True)
```

### Comparing `thinc-9.0.0.dev2/thinc/mypy.py` & `thinc-9.0.0.dev3/thinc/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,10 +253,13 @@
         self,
         errors: Errors,
         modules: Dict[str, MypyFile],
         options: Options,
         tree: MypyFile,
         path: str,
         plugin: Plugin,
+        per_line_checking_time_ns: Dict[int, int],
     ):
         self._error_messages: List[str] = []
-        super().__init__(errors, modules, options, tree, path, plugin)
+        super().__init__(
+            errors, modules, options, tree, path, plugin, per_line_checking_time_ns
+        )
```

### Comparing `thinc-9.0.0.dev2/thinc/optimizers.py` & `thinc-9.0.0.dev3/thinc/optimizers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/shims/mxnet.py` & `thinc-9.0.0.dev3/thinc/shims/mxnet.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/shims/pytorch.py` & `thinc-9.0.0.dev3/thinc/shims/pytorch.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/shims/pytorch_grad_scaler.py` & `thinc-9.0.0.dev3/thinc/shims/pytorch_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/shims/shim.py` & `thinc-9.0.0.dev3/thinc/shims/shim.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/shims/tensorflow.py` & `thinc-9.0.0.dev3/thinc/shims/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/shims/torchscript.py` & `thinc-9.0.0.dev3/thinc/shims/torchscript.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/backends/test_ops.py` & `thinc-9.0.0.dev3/thinc/tests/backends/test_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Tuple, cast
 
 import pytest
 import numpy
+import platform
 from hypothesis import given, settings
 from hypothesis.strategies import composite, integers
 from numpy.testing import assert_allclose
 from packaging.version import Version
 from thinc.api import NumpyOps, CupyOps, Ops, get_ops
 from thinc.api import get_current_ops, use_ops
 from thinc.util import torch2xp, xp2torch
@@ -1256,14 +1257,15 @@
     reference = reference_ops.lstm_forward_training(params, H0, C0, X, size_at_t)
     Y, fwd_state = ops.lstm_forward_training(params, H0, C0, X, size_at_t)
     assert_allclose(fwd_state[2], reference[1][2], atol=1e-4, rtol=1e-3)
     assert_allclose(fwd_state[1], reference[1][1], atol=1e-4, rtol=1e-3)
     assert_allclose(Y, reference[0], atol=1e-4, rtol=1e-3)
 
 
+@pytest.mark.skipif(platform.machine() == "aarch64", reason="Flaky, skip temporarily")
 @pytest.mark.parametrize("ops", XP_OPS)
 @settings(max_examples=MAX_EXAMPLES, deadline=None)
 @given(args=draw_lstm_args())
 def test_lstm_forward_training_fuzz(ops, args):
     params, H0, C0, X, size_at_t = args
     reference_ops = Ops()
     reference = reference_ops.lstm_forward_training(params, H0, C0, X, size_at_t)
```

### Comparing `thinc-9.0.0.dev2/thinc/tests/conftest.py` & `thinc-9.0.0.dev3/thinc/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_basic_tagger.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_basic_tagger.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_combinators.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_combinators.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_feed_forward.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_hash_embed.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_hash_embed.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_layers_api.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_layers_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,16 @@
     ("HashEmbed.v1", {"nO": 1, "nV": 2}, array1dint, array2d),
     ("MultiSoftmax.v1", {"nOs": (1, 3)}, array2d, array2d),
     # ("CauchySimilarity.v1", {}, (array2d, array2d), array1d),
     ("ParametricAttention.v1", {}, ragged, ragged),
     ("SparseLinear.v1", {}, (numpy.asarray([1, 2, 3], dtype="uint64"), array1d, numpy.asarray([1, 1], dtype="i")), array2d),
     ("SparseLinear.v2", {}, (numpy.asarray([1, 2, 3], dtype="uint64"), array1d, numpy.asarray([1, 1], dtype="i")), array2d),
     ("remap_ids.v1", {"dtype": "f"}, ["a", 1, 5.0], array2dint),
-    ("remap_ids.v2", {"mapping_table": {}, "column": 1}, numpy.array([[1, 2, 3], [4, 5, 6]]).T, array2dint)
+    ("remap_ids.v2", {"mapping_table": {}, "column": 1}, numpy.array([[1, 2, 3], [4, 5, 6]]).T, array2dint),
+    ("premap_ids.v1", {"mapping_table": {}, "column": 1}, numpy.array([[1, 2, 3], [4, 5, 6]]).T, array2dint),
     # fmt: on
 ]
 
 
 @pytest.mark.parametrize("name,kwargs,in_data,out_data", TEST_CASES)
 def test_layers_from_config(name, kwargs, in_data, out_data):
     cfg = {"@layers": name, **kwargs}
```

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_linear.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_lstm.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_lstm.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_mnist.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_mnist.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_mxnet_wrapper.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_mxnet_wrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_pytorch_wrapper.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_reduce.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_reduce.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_shim.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_shim.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_softmax.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_softmax.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_sparse_linear.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_sparse_linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_tensorflow_wrapper.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_tensorflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_torchscriptwrapper.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_torchscriptwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_transforms.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_transforms.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_uniqued.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_uniqued.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_with_debug.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_with_debug.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_with_flatten.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_with_flatten.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/layers/test_with_transforms.py` & `thinc-9.0.0.dev3/thinc/tests/layers/test_with_transforms.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/model/test_model.py` & `thinc-9.0.0.dev3/thinc/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/model/test_validation.py` & `thinc-9.0.0.dev3/thinc/tests/model/test_validation.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/mypy/modules/fail_plugin.py` & `thinc-9.0.0.dev3/thinc/tests/mypy/modules/fail_plugin.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/mypy/modules/success_plugin.py` & `thinc-9.0.0.dev3/thinc/tests/mypy/modules/success_plugin.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/mypy/outputs/fail-plugin.txt` & `thinc-9.0.0.dev3/thinc/tests/mypy/outputs/fail-plugin.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/mypy/outputs/success-no-plugin.txt` & `thinc-9.0.0.dev3/thinc/tests/mypy/outputs/success-no-plugin.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/mypy/test_mypy.py` & `thinc-9.0.0.dev3/thinc/tests/mypy/test_mypy.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/regression/issue519/test_issue519.py` & `thinc-9.0.0.dev3/thinc/tests/regression/issue519/test_issue519.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/regression/test_issue564.py` & `thinc-9.0.0.dev3/thinc/tests/regression/test_issue564.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/shims/test_pytorch_grad_scaler.py` & `thinc-9.0.0.dev3/thinc/tests/shims/test_pytorch_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/strategies.py` & `thinc-9.0.0.dev3/thinc/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_config.py` & `thinc-9.0.0.dev3/thinc/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_examples.py` & `thinc-9.0.0.dev3/thinc/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_import__all__.py` & `thinc-9.0.0.dev3/thinc/tests/test_import__all__.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_indexing.py` & `thinc-9.0.0.dev3/thinc/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_initializers.py` & `thinc-9.0.0.dev3/thinc/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_loss.py` & `thinc-9.0.0.dev3/thinc/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_optimizers.py` & `thinc-9.0.0.dev3/thinc/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_serialize.py` & `thinc-9.0.0.dev3/thinc/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_types.py` & `thinc-9.0.0.dev3/thinc/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/tests/test_util.py` & `thinc-9.0.0.dev3/thinc/tests/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import pytest
 import numpy
 from hypothesis import given
 from thinc.api import get_width, Ragged, Padded
 from thinc.util import get_array_module, is_numpy_array, to_categorical
 from thinc.util import is_cupy_array
 from thinc.util import convert_recursive
+from thinc.util import smooth_one_hot
 from thinc.types import ArgsKwargs
 
+
 from . import strategies
 
 ALL_XP = [numpy]
 try:
     import cupy
 
     ALL_XP.append(cupy)
@@ -141,14 +143,34 @@
     with pytest.raises(ValueError, match=r"label_smoothing parameter"):
         to_categorical(numpy.asarray([0, 1, 2, 3, 4]), label_smoothing=0.8)
 
     with pytest.raises(ValueError, match=r"label_smoothing parameter"):
         to_categorical(numpy.asarray([0, 1, 2, 3, 4]), label_smoothing=0.88)
 
 
+@given(
+    n_classes=strategies.lengths(lo=2, hi=100),
+    n_samples=strategies.lengths(lo=1, hi=100),
+    label_smoothing=strategies.floats(min_value=0.0, max_value=1.0)
+)
+def test_smooth_one_hot(n_samples, n_classes, label_smoothing):
+    one_hot = numpy.zeros((n_samples, n_classes))
+    labels = numpy.random.randint(0, n_classes, (n_samples,))
+    one_hot[numpy.arange(n_samples), labels] = 1
+    max_smooth = (n_classes - 1) / n_classes
+    if label_smoothing >= max_smooth:
+        with pytest.raises(ValueError, match=r"label_smoothing parameter has to be less than"):
+            smooth_one_hot(one_hot, label_smoothing)
+    else:
+        smoothed = smooth_one_hot(one_hot, label_smoothing)
+        assert numpy.all(numpy.argmax(smoothed, axis=1) == labels)
+        assert smoothed.shape == one_hot.shape
+        assert numpy.allclose(smoothed.sum(1), 1.0)
+
+
 def test_convert_recursive():
     is_match = lambda obj: obj == "foo"
     convert_item = lambda obj: obj.upper()
     obj = {
         "a": {("b", "foo"): {"c": "foo", "d": ["foo", {"e": "foo", "f": (1, "foo")}]}}
     }
     result = convert_recursive(is_match, convert_item, obj)
```

### Comparing `thinc-9.0.0.dev2/thinc/tests/util.py` & `thinc-9.0.0.dev3/thinc/tests/util.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/types.py` & `thinc-9.0.0.dev3/thinc/types.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev2/thinc/util.py` & `thinc-9.0.0.dev3/thinc/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,22 +253,33 @@
     return label_distr[Y]
 
 
 def smooth_one_hot(X: Floats2d, label_smoothing: float) -> Floats2d:
     """
     Apply label-smoothing to one-hot array.
     """
-    if not 0.0 <= label_smoothing < 0.5:
+    n_classes = X.shape[1]
+    max_smooth = (n_classes - 1) / n_classes
+    if label_smoothing < 0.0:
         raise ValueError(
-            "label_smoothing should be greater or "
-            "equal to 0.0 and less than 0.5, "
-            f"but {label_smoothing} was provided."
+            "Label-smoothing parameter has to be greater than or equal to 0"
+        )
+    if not n_classes > 1:
+        raise ValueError(
+            "n_classes should be greater than 1 when label smoothing is enabled,"
+            f"but {n_classes} was provided."
+        )
+    if label_smoothing >= max_smooth:
+        raise ValueError(
+            f"For {n_classes} classes "
+            "label_smoothing parameter has to be less than "
+            f"{max_smooth}, but found {label_smoothing}."
         )
     X[X == 1] = 1 - label_smoothing
-    X[X == 0] = label_smoothing / (X.shape[1] - 1)
+    X[X == 0] = label_smoothing / (n_classes - 1)
     return X
 
 
 def get_width(
     X: Union[ArrayXd, Ragged, Padded, Sequence[ArrayXd]], *, dim: int = -1
 ) -> int:
     """Infer the 'width' of a batch of data, which could be any of: Array,
@@ -627,14 +638,15 @@
     "is_cupy_array",
     "is_numpy_array",
     "set_active_gpu",
     "prefer_gpu",
     "require_gpu",
     "copy_array",
     "to_categorical",
+    "smooth_one_hot",
     "get_width",
     "xp2torch",
     "torch2xp",
     "tensorflow2xp",
     "xp2tensorflow",
     "validate_fwd_input_output",
     "DataValidationError",
```

### Comparing `thinc-9.0.0.dev2/thinc.egg-info/PKG-INFO` & `thinc-9.0.0.dev3/thinc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinc
-Version: 9.0.0.dev2
+Version: 9.0.0.dev3
 Summary: A refreshing functional take on deep learning, compatible with your favorite libraries
 Home-page: https://github.com/explosion/thinc
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev2 Summary: A refreshing
+Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev3 Summary: A refreshing
 functional take on deep learning, compatible with your favorite libraries Home-
 page: https://github.com/explosion/thinc Author: Explosion Author-email:
 contact@explosion.ai License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
```

### Comparing `thinc-9.0.0.dev2/thinc.egg-info/SOURCES.txt` & `thinc-9.0.0.dev3/thinc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 thinc/layers/maxout.py
 thinc/layers/mish.py
 thinc/layers/multisoftmax.py
 thinc/layers/mxnetwrapper.py
 thinc/layers/noop.py
 thinc/layers/padded2list.py
 thinc/layers/parametricattention.py
+thinc/layers/premap_ids.pyx
 thinc/layers/pytorchwrapper.py
 thinc/layers/ragged2list.py
 thinc/layers/reduce_first.py
 thinc/layers/reduce_last.py
 thinc/layers/reduce_max.py
 thinc/layers/reduce_mean.py
 thinc/layers/reduce_sum.py
@@ -140,18 +141,20 @@
 thinc/tests/layers/test_basic_tagger.py
 thinc/tests/layers/test_combinators.py
 thinc/tests/layers/test_feed_forward.py
 thinc/tests/layers/test_hash_embed.py
 thinc/tests/layers/test_layers_api.py
 thinc/tests/layers/test_linear.py
 thinc/tests/layers/test_lstm.py
+thinc/tests/layers/test_mappers.py
 thinc/tests/layers/test_mnist.py
 thinc/tests/layers/test_mxnet_wrapper.py
 thinc/tests/layers/test_pytorch_wrapper.py
 thinc/tests/layers/test_reduce.py
+thinc/tests/layers/test_resizable.py
 thinc/tests/layers/test_shim.py
 thinc/tests/layers/test_softmax.py
 thinc/tests/layers/test_sparse_linear.py
 thinc/tests/layers/test_tensorflow_wrapper.py
 thinc/tests/layers/test_torchscriptwrapper.py
 thinc/tests/layers/test_transforms.py
 thinc/tests/layers/test_uniqued.py
```

### Comparing `thinc-9.0.0.dev2/thinc.egg-info/requires.txt` & `thinc-9.0.0.dev3/thinc.egg-info/requires.txt`

 * *Files identical despite different names*

