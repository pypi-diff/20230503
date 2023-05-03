# Comparing `tmp/mosaicml-0.8.2.tar.gz` & `tmp/mosaicml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-0.8.2.tar", last modified: Wed Jul 27 23:19:11 2022, max compression
+gzip compressed data, was "mosaicml-0.9.0.tar", last modified: Tue Aug 16 05:07:37 2022, max compression
```

## Comparing `mosaicml-0.8.2.tar` & `mosaicml-0.9.0.tar`

### file list

```diff
@@ -1,386 +1,394 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.565238 mosaicml-0.8.2/
--rw-r--r--   0 root         (0) root         (0)    10770 2022-07-27 23:17:12.000000 mosaicml-0.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       54 2022-07-27 23:17:12.000000 mosaicml-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    21478 2022-07-27 23:19:11.565238 mosaicml-0.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21236 2022-07-27 23:17:12.000000 mosaicml-0.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/
--rw-r--r--   0 root         (0) root         (0)      569 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/algorithms/
--rw-r--r--   0 root         (0) root         (0)     3764 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2428 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/algorithm_hparams_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/algorithms/alibi/
--rw-r--r--   0 root         (0) root         (0)      621 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3009 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/alibi/_gpt2_alibi.py
--rw-r--r--   0 root         (0) root         (0)    15944 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/alibi/alibi.py
--rw-r--r--   0 root         (0) root         (0)      506 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/algorithms/augmix/
--rw-r--r--   0 root         (0) root         (0)      587 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12125 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 root         (0) root         (0)      499 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/algorithms/blurpool/
--rw-r--r--   0 root         (0) root         (0)     1095 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7710 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 root         (0) root         (0)    12655 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 root         (0) root         (0)      510 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/algorithms/channels_last/
--rw-r--r--   0 root         (0) root         (0)      515 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 root         (0) root         (0)      585 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/algorithms/colout/
--rw-r--r--   0 root         (0) root         (0)      665 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/colout/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13894 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/colout/colout.py
--rw-r--r--   0 root         (0) root         (0)      504 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/cutmix/
--rw-r--r--   0 root         (0) root         (0)      630 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15069 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 root         (0) root         (0)      531 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/cutout/
--rw-r--r--   0 root         (0) root         (0)      485 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5765 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 root         (0) root         (0)      458 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/ema/
--rw-r--r--   0 root         (0) root         (0)      411 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/ema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12263 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/ema/ema.py
--rw-r--r--   0 root         (0) root         (0)      494 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/factorize/
--rw-r--r--   0 root         (0) root         (0)     1218 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12412 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 root         (0) root         (0)    15567 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 root         (0) root         (0)    22318 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 root         (0) root         (0)      421 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/fused_layernorm/
--rw-r--r--   0 root         (0) root         (0)      566 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/fused_layernorm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4029 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/fused_layernorm/fused_layernorm.py
--rw-r--r--   0 root         (0) root         (0)      542 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/fused_layernorm/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/gated_linear_units/
--rw-r--r--   0 root         (0) root         (0)      586 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2473 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 root         (0) root         (0)     8465 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 root         (0) root         (0)      548 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 root         (0) root         (0)      644 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8167 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 root         (0) root         (0)      552 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/gradient_clipping/
--rw-r--r--   0 root         (0) root         (0)      435 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8996 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 root         (0) root         (0)      556 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/label_smoothing/
--rw-r--r--   0 root         (0) root         (0)      592 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4836 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 root         (0) root         (0)      600 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/layer_freezing/
--rw-r--r--   0 root         (0) root         (0)      497 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9111 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 root         (0) root         (0)      597 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/mixup/
--rw-r--r--   0 root         (0) root         (0)      476 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 root         (0) root         (0)     9983 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/no_op_model/
--rw-r--r--   0 root         (0) root         (0)      711 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      266 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 root         (0) root         (0)     2608 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/progressive_resizing/
--rw-r--r--   0 root         (0) root         (0)      931 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      639 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 root         (0) root         (0)    13609 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/randaugment/
--rw-r--r--   0 root         (0) root         (0)      491 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 root         (0) root         (0)      659 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 root         (0) root         (0)     8993 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/sam/
--rw-r--r--   0 root         (0) root         (0)      573 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/sam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      387 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/sam/metadata.json
--rw-r--r--   0 root         (0) root         (0)     6353 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/selective_backprop/
--rw-r--r--   0 root         (0) root         (0)     1155 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 root         (0) root         (0)      523 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 root         (0) root         (0)    11924 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 root         (0) root         (0)      439 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 root         (0) root         (0)    11869 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/squeeze_excite/
--rw-r--r--   0 root         (0) root         (0)      861 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 root         (0) root         (0)      483 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 root         (0) root         (0)     7962 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.549238 mosaicml-0.8.2/composer/algorithms/stochastic_depth/
--rw-r--r--   0 root         (0) root         (0)      697 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      604 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 root         (0) root         (0)    12448 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 root         (0) root         (0)     4552 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/algorithms/swa/
--rw-r--r--   0 root         (0) root         (0)      468 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/swa/__init__.py
--rw-r--r--   0 root         (0) root         (0)      464 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/swa/metadata.json
--rw-r--r--   0 root         (0) root         (0)    12773 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/algorithms/utils/
--rw-r--r--   0 root         (0) root         (0)      234 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3584 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 root         (0) root         (0)    11941 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 root         (0) root         (0)      772 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/algorithms/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/callbacks/
--rw-r--r--   0 root         (0) root         (0)     1053 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/callback_hparams_registry.py
--rw-r--r--   0 root         (0) root         (0)    21022 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 root         (0) root         (0)     6889 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/early_stopper.py
--rw-r--r--   0 root         (0) root         (0)     3461 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/grad_monitor.py
--rw-r--r--   0 root         (0) root         (0)    11164 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/image_visualizer.py
--rw-r--r--   0 root         (0) root         (0)     2206 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/lr_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5443 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/memory_monitor.py
--rw-r--r--   0 root         (0) root         (0)    17084 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/mlperf.py
--rw-r--r--   0 root         (0) root         (0)     7021 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/speed_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5588 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/cli/
--rw-r--r--   0 root         (0) root         (0)      102 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      181 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/cli/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)    21982 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/cli/launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/core/
--rw-r--r--   0 root         (0) root         (0)     1141 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4986 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/algorithm.py
--rw-r--r--   0 root         (0) root         (0)    14442 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/callback.py
--rw-r--r--   0 root         (0) root         (0)    10507 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/data_spec.py
--rw-r--r--   0 root         (0) root         (0)    19338 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/engine.py
--rw-r--r--   0 root         (0) root         (0)     7204 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     8743 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/event.py
--rw-r--r--   0 root         (0) root         (0)     2637 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/precision.py
--rw-r--r--   0 root         (0) root         (0)      858 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/serializable.py
--rw-r--r--   0 root         (0) root         (0)    28332 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/state.py
--rw-r--r--   0 root         (0) root         (0)    30185 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/time.py
--rw-r--r--   0 root         (0) root         (0)     2435 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/core/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/datasets/
--rw-r--r--   0 root         (0) root         (0)      918 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16445 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/ade20k.py
--rw-r--r--   0 root         (0) root         (0)    11014 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/ade20k_hparams.py
--rw-r--r--   0 root         (0) root         (0)     7776 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/brats.py
--rw-r--r--   0 root         (0) root         (0)     1940 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/brats_hparams.py
--rw-r--r--   0 root         (0) root         (0)    18947 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/c4.py
--rw-r--r--   0 root         (0) root         (0)    11225 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/c4_hparams.py
--rw-r--r--   0 root         (0) root         (0)     3531 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/cifar.py
--rw-r--r--   0 root         (0) root         (0)     9955 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/cifar_hparams.py
--rw-r--r--   0 root         (0) root         (0)     7791 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/coco.py
--rw-r--r--   0 root         (0) root         (0)     4308 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/coco_hparams.py
--rw-r--r--   0 root         (0) root         (0)     6252 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/dataset_hparams.py
--rw-r--r--   0 root         (0) root         (0)     1520 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/dataset_hparams_registry.py
--rw-r--r--   0 root         (0) root         (0)     4622 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/evaluator_hparams.py
--rw-r--r--   0 root         (0) root         (0)     3286 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/ffcv_utils.py
--rw-r--r--   0 root         (0) root         (0)     7149 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/glue_hparams.py
--rw-r--r--   0 root         (0) root         (0)     4336 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/imagenet.py
--rw-r--r--   0 root         (0) root         (0)    12371 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/imagenet_hparams.py
--rw-r--r--   0 root         (0) root         (0)     9526 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/lm_dataset_hparams.py
--rw-r--r--   0 root         (0) root         (0)     2910 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/mnist_hparams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.553238 mosaicml-0.8.2/composer/datasets/streaming/
--rw-r--r--   0 root         (0) root         (0)     1682 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/streaming/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14267 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/streaming/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6359 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/streaming/download.py
--rw-r--r--   0 root         (0) root         (0)    15121 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/streaming/format.py
--rw-r--r--   0 root         (0) root         (0)     3505 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/streaming/world.py
--rw-r--r--   0 root         (0) root         (0)     5962 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/streaming/writer.py
--rw-r--r--   0 root         (0) root         (0)    10208 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/synthetic.py
--rw-r--r--   0 root         (0) root         (0)     2000 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/synthetic_hparams.py
--rw-r--r--   0 root         (0) root         (0)    10230 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/synthetic_lm.py
--rw-r--r--   0 root         (0) root         (0)     6803 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/datasets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/functional/
--rw-r--r--   0 root         (0) root         (0)     2548 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/loggers/
--rw-r--r--   0 root         (0) root         (0)     1339 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12692 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/file_logger.py
--rw-r--r--   0 root         (0) root         (0)     5902 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/in_memory_logger.py
--rw-r--r--   0 root         (0) root         (0)     6355 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/logger.py
--rw-r--r--   0 root         (0) root         (0)     5222 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/logger_destination.py
--rw-r--r--   0 root         (0) root         (0)     4004 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/logger_hparams_registry.py
--rw-r--r--   0 root         (0) root         (0)    23287 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/object_store_logger.py
--rw-r--r--   0 root         (0) root         (0)    16070 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 root         (0) root         (0)     5906 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 root         (0) root         (0)     8854 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/loss/
--rw-r--r--   0 root         (0) root         (0)      398 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8795 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loss/loss.py
--rw-r--r--   0 root         (0) root         (0)     3262 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/loss/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/metrics/
--rw-r--r--   0 root         (0) root         (0)      472 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/metrics/metrics.py
--rw-r--r--   0 root         (0) root         (0)     9197 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/metrics/nlp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/
--rw-r--r--   0 root         (0) root         (0)     2627 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8868 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/bert/
--rw-r--r--   0 root         (0) root         (0)      571 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5941 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/bert/bert_hparams.py
--rw-r--r--   0 root         (0) root         (0)     4599 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/bert/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/classify_mnist/
--rw-r--r--   0 root         (0) root         (0)      584 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/classify_mnist/__init__.py
--rw-r--r--   0 root         (0) root         (0)      908 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/classify_mnist/mnist_hparams.py
--rw-r--r--   0 root         (0) root         (0)     2323 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/classify_mnist/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/deeplabv3/
--rw-r--r--   0 root         (0) root         (0)      355 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/deeplabv3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9373 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/deeplabv3/deeplabv3.py
--rw-r--r--   0 root         (0) root         (0)     3038 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/deeplabv3/deeplabv3_hparams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/efficientnetb0/
--rw-r--r--   0 root         (0) root         (0)     1008 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/efficientnetb0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9915 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/efficientnetb0/_layers.py
--rw-r--r--   0 root         (0) root         (0)     1283 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/efficientnetb0/efficientnetb0_hparams.py
--rw-r--r--   0 root         (0) root         (0)     9543 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/efficientnetb0/efficientnets.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/efficientnetb0/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/gpt2/
--rw-r--r--   0 root         (0) root         (0)     1445 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/gpt2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2817 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/gpt2/gpt2_hparams.py
--rw-r--r--   0 root         (0) root         (0)     3564 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/gpt2/model.py
--rw-r--r--   0 root         (0) root         (0)     2103 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     2668 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/initializers.py
--rw-r--r--   0 root         (0) root         (0)     1392 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/model_hparams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/resnet/
--rw-r--r--   0 root         (0) root         (0)     2012 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2995 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet/model.py
--rw-r--r--   0 root         (0) root         (0)     3016 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet/resnet_hparams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/resnet_cifar/
--rw-r--r--   0 root         (0) root         (0)     1253 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet_cifar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1884 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet_cifar/model.py
--rw-r--r--   0 root         (0) root         (0)     1685 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet_cifar/resnet_cifar_hparams.py
--rw-r--r--   0 root         (0) root         (0)     6518 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/resnet_cifar/resnets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/ssd/
--rw-r--r--   0 root         (0) root         (0)      326 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/ssd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4859 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/ssd/base_model.py
--rw-r--r--   0 root         (0) root         (0)     6337 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/ssd/ssd.py
--rw-r--r--   0 root         (0) root         (0)     5160 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/ssd/ssd300.py
--rw-r--r--   0 root         (0) root         (0)     1723 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/ssd/ssd_hparams.py
--rw-r--r--   0 root         (0) root         (0)    15692 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/ssd/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/tasks/
--rw-r--r--   0 root         (0) root         (0)      322 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3800 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/tasks/classification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.557238 mosaicml-0.8.2/composer/models/timm/
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/timm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2963 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/timm/model.py
--rw-r--r--   0 root         (0) root         (0)     3837 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/timm/timm_hparams.py
--rw-r--r--   0 root         (0) root         (0)     2276 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/transformer_hparams.py
--rw-r--r--   0 root         (0) root         (0)     5362 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/transformer_shared.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/models/unet/
--rw-r--r--   0 root         (0) root         (0)      566 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/unet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5168 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/unet/_layers.py
--rw-r--r--   0 root         (0) root         (0)     4418 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/unet/model.py
--rw-r--r--   0 root         (0) root         (0)     3921 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/unet/unet.py
--rw-r--r--   0 root         (0) root         (0)      860 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/unet/unet_hparams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/models/vit_small_patch16/
--rw-r--r--   0 root         (0) root         (0)      504 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/vit_small_patch16/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2271 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/vit_small_patch16/hparams.py
--rw-r--r--   0 root         (0) root         (0)     1699 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/models/vit_small_patch16/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/optim/
--rw-r--r--   0 root         (0) root         (0)     1744 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12757 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 root         (0) root         (0)     8542 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/optim/optimizer_hparams_registry.py
--rw-r--r--   0 root         (0) root         (0)    35588 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/optim/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1469 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/optim/scheduler_hparams_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/profiler/
--rw-r--r--   0 root         (0) root         (0)     1377 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21039 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/json_trace_handler.py
--rw-r--r--   0 root         (0) root         (0)     6282 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/json_trace_merger.py
--rw-r--r--   0 root         (0) root         (0)     8866 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/marker.py
--rw-r--r--   0 root         (0) root         (0)    11847 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/profiler.py
--rw-r--r--   0 root         (0) root         (0)      976 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/profiler_action.py
--rw-r--r--   0 root         (0) root         (0)     1052 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/profiler_hparams.py
--rw-r--r--   0 root         (0) root         (0)     2862 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/profiler_schedule.py
--rw-r--r--   0 root         (0) root         (0)     5397 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/system_profiler.py
--rw-r--r--   0 root         (0) root         (0)    12259 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/torch_profiler.py
--rw-r--r--   0 root         (0) root         (0)     4036 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/profiler/trace_handler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/trainer/
--rw-r--r--   0 root         (0) root         (0)      257 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7555 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/_deepspeed.py
--rw-r--r--   0 root         (0) root         (0)     3552 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/_scale_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6422 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/_scaler.py
--rw-r--r--   0 root         (0) root         (0)     5535 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/ddp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/trainer/devices/
--rw-r--r--   0 root         (0) root         (0)      493 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3604 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/devices/device.py
--rw-r--r--   0 root         (0) root         (0)     1079 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/devices/device_cpu.py
--rw-r--r--   0 root         (0) root         (0)     2229 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/devices/device_gpu.py
--rw-r--r--   0 root         (0) root         (0)      559 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/devices/device_hparams_registry.py
--rw-r--r--   0 root         (0) root         (0)   107799 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/trainer.py
--rw-r--r--   0 root         (0) root         (0)    41168 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/trainer/trainer_hparams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/utils/
--rw-r--r--   0 root         (0) root         (0)     1807 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7991 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/batch_helpers.py
--rw-r--r--   0 root         (0) root         (0)    23264 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/checkpoint.py
--rw-r--r--   0 root         (0) root         (0)    13989 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/collect_env.py
--rw-r--r--   0 root         (0) root         (0)    16940 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/dist.py
--rw-r--r--   0 root         (0) root         (0)    22921 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/file_helpers.py
--rw-r--r--   0 root         (0) root         (0)    13407 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/fx_utils.py
--rw-r--r--   0 root         (0) root         (0)     2373 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/import_helpers.py
--rw-r--r--   0 root         (0) root         (0)     4093 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/iter_helpers.py
--rw-r--r--   0 root         (0) root         (0)      335 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)    19674 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/module_surgery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.561238 mosaicml-0.8.2/composer/utils/object_store/
--rw-r--r--   0 root         (0) root         (0)      567 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/object_store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7763 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 root         (0) root         (0)     5677 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/object_store/object_store.py
--rw-r--r--   0 root         (0) root         (0)    12986 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/object_store/object_store_hparams.py
--rw-r--r--   0 root         (0) root         (0)     7103 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 root         (0) root         (0)    10601 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 root         (0) root         (0)     7504 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/reproducibility.py
--rw-r--r--   0 root         (0) root         (0)     3325 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/retrying.py
--rw-r--r--   0 root         (0) root         (0)     4113 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/utils/string_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.545238 mosaicml-0.8.2/composer/yamls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.565238 mosaicml-0.8.2/composer/yamls/models/
--rw-r--r--   0 root         (0) root         (0)     2334 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/bert-base.yaml
--rw-r--r--   0 root         (0) root         (0)      669 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/classify_mnist.yaml
--rw-r--r--   0 root         (0) root         (0)      669 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/classify_mnist_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)      930 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/deeplabv3_ade20k_optimized.yaml
--rw-r--r--   0 root         (0) root         (0)      933 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/deeplabv3_ade20k_unoptimized.yaml
--rw-r--r--   0 root         (0) root         (0)     1212 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/deeplabv3_streaming_ade20k_optimized.yaml
--rw-r--r--   0 root         (0) root         (0)      756 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/efficientnetb0.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.565238 mosaicml-0.8.2/composer/yamls/models/glue/
--rw-r--r--   0 root         (0) root         (0)     1207 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/cola.yaml
--rw-r--r--   0 root         (0) root         (0)     1515 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/mnli.yaml
--rw-r--r--   0 root         (0) root         (0)     1223 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/mrpc.yaml
--rw-r--r--   0 root         (0) root         (0)     1200 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/qnli.yaml
--rw-r--r--   0 root         (0) root         (0)     1220 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/qqp.yaml
--rw-r--r--   0 root         (0) root         (0)     1196 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/rte.yaml
--rw-r--r--   0 root         (0) root         (0)     1198 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/sst-2.yaml
--rw-r--r--   0 root         (0) root         (0)     1207 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/glue/stsb.yaml
--rw-r--r--   0 root         (0) root         (0)     1853 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_1,3b.yaml
--rw-r--r--   0 root         (0) root         (0)     2009 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_125m.yaml
--rw-r--r--   0 root         (0) root         (0)     1854 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_13b.yaml
--rw-r--r--   0 root         (0) root         (0)     1854 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_2,7b.yaml
--rw-r--r--   0 root         (0) root         (0)     1851 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_350m.yaml
--rw-r--r--   0 root         (0) root         (0)     2005 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_52m.yaml
--rw-r--r--   0 root         (0) root         (0)     1854 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_6,7b.yaml
--rw-r--r--   0 root         (0) root         (0)     1851 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_760m.yaml
--rw-r--r--   0 root         (0) root         (0)     2007 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt2_83m.yaml
--rw-r--r--   0 root         (0) root         (0)     2044 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt3_125m.yaml
--rw-r--r--   0 root         (0) root         (0)     2047 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt3_350m.yaml
--rw-r--r--   0 root         (0) root         (0)     2045 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/gpt3_760m.yaml
--rw-r--r--   0 root         (0) root         (0)      823 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet101.yaml
--rw-r--r--   0 root         (0) root         (0)      864 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet101_synthetic.yaml
--rw-r--r--   0 root         (0) root         (0)      823 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet152.yaml
--rw-r--r--   0 root         (0) root         (0)      864 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet152_synthetic.yaml
--rw-r--r--   0 root         (0) root         (0)      820 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet18.yaml
--rw-r--r--   0 root         (0) root         (0)      861 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet18_synthetic.yaml
--rw-r--r--   0 root         (0) root         (0)      791 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet20_cifar10.yaml
--rw-r--r--   0 root         (0) root         (0)      822 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet34.yaml
--rw-r--r--   0 root         (0) root         (0)      863 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet34_synthetic.yaml
--rw-r--r--   0 root         (0) root         (0)      822 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet50.yaml
--rw-r--r--   0 root         (0) root         (0)      981 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet50_streaming.yaml
--rw-r--r--   0 root         (0) root         (0)      863 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet50_synthetic.yaml
--rw-r--r--   0 root         (0) root         (0)      791 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet56_cifar10.yaml
--rw-r--r--   0 root         (0) root         (0)      834 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet56_cifar10_synthetic.yaml
--rw-r--r--   0 root         (0) root         (0)      896 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet56_streaming_cifar10.yaml
--rw-r--r--   0 root         (0) root         (0)      830 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/resnet9_cifar10.yaml
--rw-r--r--   0 root         (0) root         (0)      762 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/timm_resnet50_imagenet.yaml
--rw-r--r--   0 root         (0) root         (0)      868 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/timm_vit_small_patch16.yaml
--rw-r--r--   0 root         (0) root         (0)      617 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/unet.yaml
--rw-r--r--   0 root         (0) root         (0)      875 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/models/vit_small_patch16.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.565238 mosaicml-0.8.2/composer/yamls/recipes/
--rw-r--r--   0 root         (0) root         (0)     2058 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/recipes/resnet50_medium.yaml
--rw-r--r--   0 root         (0) root         (0)     1945 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/recipes/resnet50_mild.yaml
--rw-r--r--   0 root         (0) root         (0)     2118 2022-07-27 23:17:12.000000 mosaicml-0.8.2/composer/yamls/recipes/resnet50_spicy.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 23:19:11.565238 mosaicml-0.8.2/mosaicml.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21478 2022-07-27 23:19:11.000000 mosaicml-0.8.2/mosaicml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12262 2022-07-27 23:19:11.000000 mosaicml-0.8.2/mosaicml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-07-27 23:19:11.000000 mosaicml-0.8.2/mosaicml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2022-07-27 23:19:11.000000 mosaicml-0.8.2/mosaicml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     2494 2022-07-27 23:19:11.000000 mosaicml-0.8.2/mosaicml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-07-27 23:19:11.000000 mosaicml-0.8.2/mosaicml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    33879 2022-07-27 23:17:12.000000 mosaicml-0.8.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-27 23:19:11.565238 mosaicml-0.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7574 2022-07-27 23:17:12.000000 mosaicml-0.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.481744 mosaicml-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10770 2022-08-16 05:05:44.000000 mosaicml-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       54 2022-08-16 05:05:44.000000 mosaicml-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21603 2022-08-16 05:07:37.481744 mosaicml-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21361 2022-08-16 05:05:44.000000 mosaicml-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.457744 mosaicml-0.9.0/composer/
+-rw-r--r--   0 root         (0) root         (0)      588 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      146 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      133 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.457744 mosaicml-0.9.0/composer/algorithms/
+-rw-r--r--   0 root         (0) root         (0)     3636 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/algorithm_hparams_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.457744 mosaicml-0.9.0/composer/algorithms/alibi/
+-rw-r--r--   0 root         (0) root         (0)      556 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8345 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 root         (0) root         (0)      630 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8143 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 root         (0) root         (0)    10272 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 root         (0) root         (0)      506 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/augmix/
+-rw-r--r--   0 root         (0) root         (0)      587 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12071 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 root         (0) root         (0)      499 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/blurpool/
+-rw-r--r--   0 root         (0) root         (0)     1095 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7690 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 root         (0) root         (0)    12674 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 root         (0) root         (0)      510 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/channels_last/
+-rw-r--r--   0 root         (0) root         (0)      515 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 root         (0) root         (0)      585 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/colout/
+-rw-r--r--   0 root         (0) root         (0)      665 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13854 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/colout/colout.py
+-rw-r--r--   0 root         (0) root         (0)      504 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/cutmix/
+-rw-r--r--   0 root         (0) root         (0)      630 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17450 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 root         (0) root         (0)      531 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/cutout/
+-rw-r--r--   0 root         (0) root         (0)      485 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 root         (0) root         (0)      458 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/ema/
+-rw-r--r--   0 root         (0) root         (0)      411 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12263 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/ema/ema.py
+-rw-r--r--   0 root         (0) root         (0)      494 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/factorize/
+-rw-r--r--   0 root         (0) root         (0)     1218 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12392 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 root         (0) root         (0)    15567 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 root         (0) root         (0)    22318 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 root         (0) root         (0)      421 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/fused_layernorm/
+-rw-r--r--   0 root         (0) root         (0)      566 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/fused_layernorm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/fused_layernorm/fused_layernorm.py
+-rw-r--r--   0 root         (0) root         (0)      542 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/fused_layernorm/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 root         (0) root         (0)      586 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 root         (0) root         (0)     8747 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 root         (0) root         (0)      548 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 root         (0) root         (0)      644 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8147 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)      552 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 root         (0) root         (0)      435 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8996 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 root         (0) root         (0)      556 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/label_smoothing/
+-rw-r--r--   0 root         (0) root         (0)      592 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 root         (0) root         (0)      600 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/layer_freezing/
+-rw-r--r--   0 root         (0) root         (0)      497 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9091 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 root         (0) root         (0)      597 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/mixup/
+-rw-r--r--   0 root         (0) root         (0)      476 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      517 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     9983 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/no_op_model/
+-rw-r--r--   0 root         (0) root         (0)      667 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      266 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     2695 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 root         (0) root         (0)      931 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      639 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 root         (0) root         (0)    13609 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.461743 mosaicml-0.9.0/composer/algorithms/randaugment/
+-rw-r--r--   0 root         (0) root         (0)      491 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      659 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     8973 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/sam/
+-rw-r--r--   0 root         (0) root         (0)      573 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      387 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     6333 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/selective_backprop/
+-rw-r--r--   0 root         (0) root         (0)     1115 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      523 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 root         (0) root         (0)    11924 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 root         (0) root         (0)      439 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      565 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 root         (0) root         (0)    17632 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 root         (0) root         (0)      861 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      483 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     7942 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 root         (0) root         (0)      697 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      604 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 root         (0) root         (0)    12408 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/swa/
+-rw-r--r--   0 root         (0) root         (0)      468 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      464 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 root         (0) root         (0)    12773 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/algorithms/utils/
+-rw-r--r--   0 root         (0) root         (0)      234 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 root         (0) root         (0)    11941 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 root         (0) root         (0)      772 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/algorithms/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     1166 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/callback_hparams_registry.py
+-rw-r--r--   0 root         (0) root         (0)    21137 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 root         (0) root         (0)     6889 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/early_stopper.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/grad_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    11164 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5419 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    17084 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/mlperf.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5588 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/cli/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      181 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/cli/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21771 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/cli/launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.465743 mosaicml-0.9.0/composer/core/
+-rw-r--r--   0 root         (0) root         (0)     1141 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    14743 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/callback.py
+-rw-r--r--   0 root         (0) root         (0)    10929 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/data_spec.py
+-rw-r--r--   0 root         (0) root         (0)    20149 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/engine.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9339 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/event.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/passes.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/precision.py
+-rw-r--r--   0 root         (0) root         (0)      858 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/serializable.py
+-rw-r--r--   0 root         (0) root         (0)    28076 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/state.py
+-rw-r--r--   0 root         (0) root         (0)    30185 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/time.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/core/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/datasets/
+-rw-r--r--   0 root         (0) root         (0)      918 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/ade20k.py
+-rw-r--r--   0 root         (0) root         (0)    11156 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/ade20k_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/brats.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/brats_hparams.py
+-rw-r--r--   0 root         (0) root         (0)    18947 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/c4.py
+-rw-r--r--   0 root         (0) root         (0)    11225 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/c4_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/cifar.py
+-rw-r--r--   0 root         (0) root         (0)     9955 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/cifar_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     7791 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/coco.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/coco_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     6252 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/dataset_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/dataset_hparams_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/evaluator_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/ffcv_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7149 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/glue_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     4336 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/imagenet.py
+-rw-r--r--   0 root         (0) root         (0)    12451 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/imagenet_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     9526 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/lm_dataset_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/mnist_hparams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/datasets/streaming/
+-rw-r--r--   0 root         (0) root         (0)     1682 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/streaming/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15715 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/streaming/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5822 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/streaming/download.py
+-rw-r--r--   0 root         (0) root         (0)    16413 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/streaming/format.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/streaming/world.py
+-rw-r--r--   0 root         (0) root         (0)     9388 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/streaming/writer.py
+-rw-r--r--   0 root         (0) root         (0)    10208 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/synthetic.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/synthetic_hparams.py
+-rw-r--r--   0 root         (0) root         (0)    10230 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/synthetic_lm.py
+-rw-r--r--   0 root         (0) root         (0)     6803 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/datasets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/functional/
+-rw-r--r--   0 root         (0) root         (0)     2548 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/loggers/
+-rw-r--r--   0 root         (0) root         (0)     1339 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12675 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/file_logger.py
+-rw-r--r--   0 root         (0) root         (0)     5902 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6898 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/logger_destination.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/logger_hparams_registry.py
+-rw-r--r--   0 root         (0) root         (0)    24946 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/object_store_logger.py
+-rw-r--r--   0 root         (0) root         (0)    16111 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6061 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 root         (0) root         (0)    11006 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/loss/
+-rw-r--r--   0 root         (0) root         (0)      450 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13759 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loss/loss.py
+-rw-r--r--   0 root         (0) root         (0)     4858 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/loss/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/metrics/
+-rw-r--r--   0 root         (0) root         (0)      472 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/metrics/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     9197 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/metrics/nlp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/
+-rw-r--r--   0 root         (0) root         (0)     2592 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8848 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/bert/
+-rw-r--r--   0 root         (0) root         (0)      715 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/bert/bert_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     8554 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/bert/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/classify_mnist/
+-rw-r--r--   0 root         (0) root         (0)      569 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/classify_mnist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      886 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/classify_mnist/mnist_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/classify_mnist/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/deeplabv3/
+-rw-r--r--   0 root         (0) root         (0)      354 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/deeplabv3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/deeplabv3/deeplabv3_hparams.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/deeplabv3/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/efficientnetb0/
+-rw-r--r--   0 root         (0) root         (0)     1035 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/efficientnetb0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9915 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/efficientnetb0/_layers.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/efficientnetb0/efficientnetb0_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     9543 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/efficientnetb0/efficientnets.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/efficientnetb0/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/gpt2/
+-rw-r--r--   0 root         (0) root         (0)     1451 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/gpt2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/gpt2/gpt2_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/gpt2/model.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/initializers.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/model_hparams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.469744 mosaicml-0.9.0/composer/models/resnet/
+-rw-r--r--   0 root         (0) root         (0)     1996 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet/model.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet/resnet_hparams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/models/resnet_cifar/
+-rw-r--r--   0 root         (0) root         (0)     1259 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet_cifar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet_cifar/model.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet_cifar/resnet_cifar_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     6518 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/resnet_cifar/resnets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/models/ssd/
+-rw-r--r--   0 root         (0) root         (0)      326 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/ssd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/ssd/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/ssd/ssd.py
+-rw-r--r--   0 root         (0) root         (0)     5160 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/ssd/ssd300.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/ssd/ssd_hparams.py
+-rw-r--r--   0 root         (0) root         (0)    15692 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/ssd/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/models/tasks/
+-rw-r--r--   0 root         (0) root         (0)      322 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/tasks/classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/models/timm/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/timm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/timm/model.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/timm/timm_hparams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/models/unet/
+-rw-r--r--   0 root         (0) root         (0)      566 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/unet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5168 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/unet/_layers.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/unet/model.py
+-rw-r--r--   0 root         (0) root         (0)     3921 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/unet/unet.py
+-rw-r--r--   0 root         (0) root         (0)      860 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/unet/unet_hparams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/models/vit_small_patch16/
+-rw-r--r--   0 root         (0) root         (0)      567 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/vit_small_patch16/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/vit_small_patch16/hparams.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/models/vit_small_patch16/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/optim/
+-rw-r--r--   0 root         (0) root         (0)     1744 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14960 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 root         (0) root         (0)     8542 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/optim/optimizer_hparams_registry.py
+-rw-r--r--   0 root         (0) root         (0)    35799 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/optim/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/optim/scheduler_hparams_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/profiler/
+-rw-r--r--   0 root         (0) root         (0)     1377 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21009 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6585 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 root         (0) root         (0)     8825 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/marker.py
+-rw-r--r--   0 root         (0) root         (0)    11822 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/profiler.py
+-rw-r--r--   0 root         (0) root         (0)      976 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/profiler_action.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/profiler_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     5347 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/system_profiler.py
+-rw-r--r--   0 root         (0) root         (0)    12179 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/torch_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/profiler/trace_handler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/trainer/
+-rw-r--r--   0 root         (0) root         (0)      257 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7530 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/_deepspeed.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     5510 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/ddp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.473744 mosaicml-0.9.0/composer/trainer/devices/
+-rw-r--r--   0 root         (0) root         (0)      636 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/device.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/device_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/device_gpu.py
+-rw-r--r--   0 root         (0) root         (0)      719 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/device_hparams_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/device_mps.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/devices/device_tpu.py
+-rw-r--r--   0 root         (0) root         (0)   116181 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/trainer.py
+-rw-r--r--   0 root         (0) root         (0)    41506 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/trainer/trainer_hparams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.477744 mosaicml-0.9.0/composer/utils/
+-rw-r--r--   0 root         (0) root         (0)     1985 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7991 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/batch_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    23365 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/checkpoint.py
+-rw-r--r--   0 root         (0) root         (0)    14771 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/collect_env.py
+-rw-r--r--   0 root         (0) root         (0)    18181 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/dist.py
+-rw-r--r--   0 root         (0) root         (0)    22921 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/file_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    13407 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/fx_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/import_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    11674 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/inference.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/iter_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)    18073 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/module_surgery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.477744 mosaicml-0.9.0/composer/utils/object_store/
+-rw-r--r--   0 root         (0) root         (0)      567 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/object_store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7763 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 root         (0) root         (0)     5677 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/object_store/object_store.py
+-rw-r--r--   0 root         (0) root         (0)    12986 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/object_store/object_store_hparams.py
+-rw-r--r--   0 root         (0) root         (0)     7103 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 root         (0) root         (0)    11261 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/reproducibility.py
+-rw-r--r--   0 root         (0) root         (0)     3325 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/retrying.py
+-rw-r--r--   0 root         (0) root         (0)     4113 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/utils/string_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.457744 mosaicml-0.9.0/composer/yamls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.477744 mosaicml-0.9.0/composer/yamls/models/
+-rw-r--r--   0 root         (0) root         (0)     2292 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/bert-base.yaml
+-rw-r--r--   0 root         (0) root         (0)      669 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/classify_mnist.yaml
+-rw-r--r--   0 root         (0) root         (0)      669 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/classify_mnist_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)      856 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/deeplabv3_ade20k_optimized.yaml
+-rw-r--r--   0 root         (0) root         (0)      859 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/deeplabv3_ade20k_unoptimized.yaml
+-rw-r--r--   0 root         (0) root         (0)     1082 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/deeplabv3_streaming_ade20k_optimized.yaml
+-rw-r--r--   0 root         (0) root         (0)      756 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/efficientnetb0.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.477744 mosaicml-0.9.0/composer/yamls/models/glue/
+-rw-r--r--   0 root         (0) root         (0)     1132 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/cola.yaml
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/mnli.yaml
+-rw-r--r--   0 root         (0) root         (0)     1146 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/mrpc.yaml
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/qnli.yaml
+-rw-r--r--   0 root         (0) root         (0)     1143 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/qqp.yaml
+-rw-r--r--   0 root         (0) root         (0)     1121 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/rte.yaml
+-rw-r--r--   0 root         (0) root         (0)     1123 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/sst-2.yaml
+-rw-r--r--   0 root         (0) root         (0)     1132 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/glue/stsb.yaml
+-rw-r--r--   0 root         (0) root         (0)     1853 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_1,3b.yaml
+-rw-r--r--   0 root         (0) root         (0)     2009 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_125m.yaml
+-rw-r--r--   0 root         (0) root         (0)     1854 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_13b.yaml
+-rw-r--r--   0 root         (0) root         (0)     1854 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_2,7b.yaml
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_350m.yaml
+-rw-r--r--   0 root         (0) root         (0)     2005 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_52m.yaml
+-rw-r--r--   0 root         (0) root         (0)     1854 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_6,7b.yaml
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_760m.yaml
+-rw-r--r--   0 root         (0) root         (0)     2007 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt2_83m.yaml
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt3_125m.yaml
+-rw-r--r--   0 root         (0) root         (0)     2047 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt3_350m.yaml
+-rw-r--r--   0 root         (0) root         (0)     2045 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/gpt3_760m.yaml
+-rw-r--r--   0 root         (0) root         (0)      823 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet101.yaml
+-rw-r--r--   0 root         (0) root         (0)      864 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet101_synthetic.yaml
+-rw-r--r--   0 root         (0) root         (0)      823 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet152.yaml
+-rw-r--r--   0 root         (0) root         (0)      864 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet152_synthetic.yaml
+-rw-r--r--   0 root         (0) root         (0)      820 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet18.yaml
+-rw-r--r--   0 root         (0) root         (0)      861 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet18_synthetic.yaml
+-rw-r--r--   0 root         (0) root         (0)      791 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet20_cifar10.yaml
+-rw-r--r--   0 root         (0) root         (0)      822 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet34.yaml
+-rw-r--r--   0 root         (0) root         (0)      863 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet34_synthetic.yaml
+-rw-r--r--   0 root         (0) root         (0)      822 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet50.yaml
+-rw-r--r--   0 root         (0) root         (0)      917 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet50_streaming.yaml
+-rw-r--r--   0 root         (0) root         (0)      863 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet50_synthetic.yaml
+-rw-r--r--   0 root         (0) root         (0)      791 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet56_cifar10.yaml
+-rw-r--r--   0 root         (0) root         (0)      834 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet56_cifar10_synthetic.yaml
+-rw-r--r--   0 root         (0) root         (0)      838 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet56_streaming_cifar10.yaml
+-rw-r--r--   0 root         (0) root         (0)      830 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/resnet9_cifar10.yaml
+-rw-r--r--   0 root         (0) root         (0)      762 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/timm_resnet50_imagenet.yaml
+-rw-r--r--   0 root         (0) root         (0)      870 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/timm_vit_small_patch16.yaml
+-rw-r--r--   0 root         (0) root         (0)      617 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/unet.yaml
+-rw-r--r--   0 root         (0) root         (0)      877 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/models/vit_small_patch16.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.477744 mosaicml-0.9.0/composer/yamls/recipes/
+-rw-r--r--   0 root         (0) root         (0)     2122 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/recipes/resnet50_medium.yaml
+-rw-r--r--   0 root         (0) root         (0)     1995 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/recipes/resnet50_mild.yaml
+-rw-r--r--   0 root         (0) root         (0)     2212 2022-08-16 05:05:44.000000 mosaicml-0.9.0/composer/yamls/recipes/resnet50_spicy.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 05:07:37.481744 mosaicml-0.9.0/mosaicml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21603 2022-08-16 05:07:37.000000 mosaicml-0.9.0/mosaicml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12589 2022-08-16 05:07:37.000000 mosaicml-0.9.0/mosaicml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2022-08-16 05:07:37.000000 mosaicml-0.9.0/mosaicml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2022-08-16 05:07:37.000000 mosaicml-0.9.0/mosaicml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     2551 2022-08-16 05:07:37.000000 mosaicml-0.9.0/mosaicml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-08-16 05:07:37.000000 mosaicml-0.9.0/mosaicml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    33770 2022-08-16 05:05:44.000000 mosaicml-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-16 05:07:37.481744 mosaicml-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8055 2022-08-16 05:05:44.000000 mosaicml-0.9.0/setup.py
```

### Comparing `mosaicml-0.8.2/LICENSE` & `mosaicml-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/PKG-INFO` & `mosaicml-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml
-Version: 0.8.2
+Version: 0.9.0
 Summary: Composer provides well-engineered implementations of efficient training methods to give the tools that help you train a better model for cheaper.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -97,21 +97,21 @@
 <!-- end numbers -->
 
 # 🚀 Quickstart
 
 ## 💾 Installation
 Composer is available with Pip:
 
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.skip-->
 ```bash
 pip install mosaicml
 ```
 Alternatively, install Composer with Conda:
 
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.skip-->
 ```bash
 conda install -c mosaicml mosaicml
 ```
 ---
 
 ## 🚌 Usage
 
@@ -142,39 +142,48 @@
 For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/latest/functional_api.html).
 
 ### Example: Trainer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/getting_started.ipynb)
 
 For the best experience and the most efficient possible training, we recommend using Composer's built-in trainer, which automatically takes care of the low-level details of using speedup methods and provides useful abstractions that facilitate rapid experimentation.
 
 <!-- begin_example_2 --->
-<!-- TODO: Address timeouts -->
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.gpu-->
+<!--pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')-->
+<!--
+```python
+import torch
+
+# adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
+torch.use_deterministic_algorithms(False)
+
+```
+-->
+<!--pytest-codeblocks:cont-->
 ```python
 from torch.utils.data import DataLoader
 from torchvision import datasets, transforms
 
 from composer import Trainer
-from composer.algorithms import BlurPool, ChannelsLast, CutMix, LabelSmoothing
-from composer.models import MNIST_Classifier
+from composer.algorithms import ChannelsLast, CutMix, LabelSmoothing
+from composer.models import mnist_model
 
 transform = transforms.Compose([transforms.ToTensor()])
 train_dataset = datasets.MNIST("data", download=True, train=True, transform=transform)
 eval_dataset = datasets.MNIST("data", download=True, train=False, transform=transform)
 train_dataloader = DataLoader(train_dataset, batch_size=128)
 eval_dataloader = DataLoader(eval_dataset, batch_size=128)
 
 trainer = Trainer(
-    model=MNIST_Classifier(num_classes=10),
+    model=mnist_model(),
     train_dataloader=train_dataloader,
     eval_dataloader=eval_dataloader,
     max_duration="2ep",
     algorithms=[
-        BlurPool(replace_convs=True, replace_maxpools=True, blur_first=True),
         ChannelsLast(),
-        CutMix(num_classes=10),
+        CutMix(alpha=1.0),
         LabelSmoothing(smoothing=0.1),
     ]
 )
 trainer.fit()
 ```
 <!-- end_example_2 -->
 
@@ -368,15 +377,15 @@
   <tr>
     <td><a href="https://mosaicml.com/jobs" target="_blank" rel="noopener noreferrer">We're Hiring!</a></td>
     <td>Join us! 🤩</td>
   </tr>
 </tbody>
 </table>
 
-If you have any questions, please feel free to reach out to us on [Twitter](https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg)!
+If you have any questions, please feel free to reach out to us on [Twitter](https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-1dc6mo5wg-arlv6Oo9JjEn_g4d5s7PXQ)!
 
 # 💫 Contributors
 Composer is part of the broader Machine Learning community, and we welcome any contributions, pull requests, or issues!
 
 To start contributing, see our [Contributing](https://github.com/mosaicml/composer/blob/dev/CONTRIBUTING.md) page.
 
 # ✍️ Citation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml Version: 0.8.2 Summary: Composer provides
+Metadata-Version: 2.1 Name: mosaicml Version: 0.9.0 Summary: Composer provides
 well-engineered implementations of efficient training methods to give the tools
 that help you train a better model for cheaper. Home-page: https://github.com/
 mosaicml/composer Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: base Provides-Extra: dev Provides-
@@ -61,35 +61,33 @@
 functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/
 latest/functional_api.html). ### Example: Trainer [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 getting_started.ipynb) For the best experience and the most efficient possible
 training, we recommend using Composer's built-in trainer, which automatically
 takes care of the low-level details of using speedup methods and provides
-useful abstractions that facilitate rapid experimentation.    ```python from
+useful abstractions that facilitate rapid experimentation.      ```python from
 torch.utils.data import DataLoader from torchvision import datasets, transforms
-from composer import Trainer from composer.algorithms import BlurPool,
-ChannelsLast, CutMix, LabelSmoothing from composer.models import
-MNIST_Classifier transform = transforms.Compose([transforms.ToTensor()])
-train_dataset = datasets.MNIST("data", download=True, train=True,
-transform=transform) eval_dataset = datasets.MNIST("data", download=True,
-train=False, transform=transform) train_dataloader = DataLoader(train_dataset,
-batch_size=128) eval_dataloader = DataLoader(eval_dataset, batch_size=128)
-trainer = Trainer( model=MNIST_Classifier(num_classes=10),
-train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
-max_duration="2ep", algorithms=[ BlurPool(replace_convs=True,
-replace_maxpools=True, blur_first=True), ChannelsLast(), CutMix
-(num_classes=10), LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```
-Composer's built-in [trainer](https://docs.mosaicml.com/en/stable/trainer/
-using_the_trainer.html) makes it easy to **add multiple speedup methods in a
-single line of code!** Trying out new methods or combinations of methods is as
-easy as changing a single list. As we continually implement more methods, they
-will be easy for you to add to your code. For concrete examples of methods in
-Composer, here are some ([_see here for all_](https://docs.mosaicml.com/en/
-latest/trainer/algorithms.html)) speedup methods currently in Composer:
+from composer import Trainer from composer.algorithms import ChannelsLast,
+CutMix, LabelSmoothing from composer.models import mnist_model transform =
+transforms.Compose([transforms.ToTensor()]) train_dataset = datasets.MNIST
+("data", download=True, train=True, transform=transform) eval_dataset =
+datasets.MNIST("data", download=True, train=False, transform=transform)
+train_dataloader = DataLoader(train_dataset, batch_size=128) eval_dataloader =
+DataLoader(eval_dataset, batch_size=128) trainer = Trainer( model=mnist_model
+(), train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
+max_duration="2ep", algorithms=[ ChannelsLast(), CutMix(alpha=1.0),
+LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```  Composer's built-in
+[trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html)
+makes it easy to **add multiple speedup methods in a single line of code!**
+Trying out new methods or combinations of methods is as easy as changing a
+single list. As we continually implement more methods, they will be easy for
+you to add to your code. For concrete examples of methods in Composer, here are
+some ([_see here for all_](https://docs.mosaicml.com/en/latest/trainer/
+algorithms.html)) speedup methods currently in Composer:
 Name|Attribution|tl;dr|Example Benchmark|Speed Up*| ----|-----------|-----|----
 -----|---------| [Alibi](https://github.com/mosaicml/composer/tree/dev/
 composer/algorithms/alibi)|[Press et al, 2021](https://arxiv.org/abs/
 2108.12409)|Replace attention with AliBi.|GPT-2|1.5x [BlurPool](https://
 github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|[Zhang,
 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter before
 every downsampling operation.|ResNet-101|1.2x [ChannelsLast](https://
@@ -238,14 +236,14 @@
                                         An interactive Colab Notebook aimed at
 Training_BERTs_with_Composer            helping users learn how to train BERT
                                         models with Composer!
 We're_Hiring!                           Join us! ð¤©
 If you have any questions, please feel free to reach out to us on [Twitter]
 (https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our
 [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-
-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg)! # ð« Contributors Composer is part of the
+1dc6mo5wg-arlv6Oo9JjEn_g4d5s7PXQ)! # ð« Contributors Composer is part of the
 broader Machine Learning community, and we welcome any contributions, pull
 requests, or issues! To start contributing, see our [Contributing](https://
 github.com/mosaicml/composer/blob/dev/CONTRIBUTING.md) page. # âï¸ Citation
 ``` @misc{mosaicml2022composer, author = {The Mosaic ML Team}, title =
 {composer}, year = {2021}, howpublished = {\url{https://github.com/mosaicml/
 composer/}}, } ```
```

### Comparing `mosaicml-0.8.2/README.md` & `mosaicml-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,21 @@
 <!-- end numbers -->
 
 # 🚀 Quickstart
 
 ## 💾 Installation
 Composer is available with Pip:
 
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.skip-->
 ```bash
 pip install mosaicml
 ```
 Alternatively, install Composer with Conda:
 
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.skip-->
 ```bash
 conda install -c mosaicml mosaicml
 ```
 ---
 
 ## 🚌 Usage
 
@@ -120,39 +120,48 @@
 For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/latest/functional_api.html).
 
 ### Example: Trainer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/getting_started.ipynb)
 
 For the best experience and the most efficient possible training, we recommend using Composer's built-in trainer, which automatically takes care of the low-level details of using speedup methods and provides useful abstractions that facilitate rapid experimentation.
 
 <!-- begin_example_2 --->
-<!-- TODO: Address timeouts -->
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.gpu-->
+<!--pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')-->
+<!--
+```python
+import torch
+
+# adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
+torch.use_deterministic_algorithms(False)
+
+```
+-->
+<!--pytest-codeblocks:cont-->
 ```python
 from torch.utils.data import DataLoader
 from torchvision import datasets, transforms
 
 from composer import Trainer
-from composer.algorithms import BlurPool, ChannelsLast, CutMix, LabelSmoothing
-from composer.models import MNIST_Classifier
+from composer.algorithms import ChannelsLast, CutMix, LabelSmoothing
+from composer.models import mnist_model
 
 transform = transforms.Compose([transforms.ToTensor()])
 train_dataset = datasets.MNIST("data", download=True, train=True, transform=transform)
 eval_dataset = datasets.MNIST("data", download=True, train=False, transform=transform)
 train_dataloader = DataLoader(train_dataset, batch_size=128)
 eval_dataloader = DataLoader(eval_dataset, batch_size=128)
 
 trainer = Trainer(
-    model=MNIST_Classifier(num_classes=10),
+    model=mnist_model(),
     train_dataloader=train_dataloader,
     eval_dataloader=eval_dataloader,
     max_duration="2ep",
     algorithms=[
-        BlurPool(replace_convs=True, replace_maxpools=True, blur_first=True),
         ChannelsLast(),
-        CutMix(num_classes=10),
+        CutMix(alpha=1.0),
         LabelSmoothing(smoothing=0.1),
     ]
 )
 trainer.fit()
 ```
 <!-- end_example_2 -->
 
@@ -346,15 +355,15 @@
   <tr>
     <td><a href="https://mosaicml.com/jobs" target="_blank" rel="noopener noreferrer">We're Hiring!</a></td>
     <td>Join us! 🤩</td>
   </tr>
 </tbody>
 </table>
 
-If you have any questions, please feel free to reach out to us on [Twitter](https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg)!
+If you have any questions, please feel free to reach out to us on [Twitter](https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-1dc6mo5wg-arlv6Oo9JjEn_g4d5s7PXQ)!
 
 # 💫 Contributors
 Composer is part of the broader Machine Learning community, and we welcome any contributions, pull requests, or issues!
 
 To start contributing, see our [Contributing](https://github.com/mosaicml/composer/blob/dev/CONTRIBUTING.md) page.
 
 # ✍️ Citation
```

#### html2text {}

```diff
@@ -53,35 +53,33 @@
 functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/
 latest/functional_api.html). ### Example: Trainer [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 getting_started.ipynb) For the best experience and the most efficient possible
 training, we recommend using Composer's built-in trainer, which automatically
 takes care of the low-level details of using speedup methods and provides
-useful abstractions that facilitate rapid experimentation.    ```python from
+useful abstractions that facilitate rapid experimentation.      ```python from
 torch.utils.data import DataLoader from torchvision import datasets, transforms
-from composer import Trainer from composer.algorithms import BlurPool,
-ChannelsLast, CutMix, LabelSmoothing from composer.models import
-MNIST_Classifier transform = transforms.Compose([transforms.ToTensor()])
-train_dataset = datasets.MNIST("data", download=True, train=True,
-transform=transform) eval_dataset = datasets.MNIST("data", download=True,
-train=False, transform=transform) train_dataloader = DataLoader(train_dataset,
-batch_size=128) eval_dataloader = DataLoader(eval_dataset, batch_size=128)
-trainer = Trainer( model=MNIST_Classifier(num_classes=10),
-train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
-max_duration="2ep", algorithms=[ BlurPool(replace_convs=True,
-replace_maxpools=True, blur_first=True), ChannelsLast(), CutMix
-(num_classes=10), LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```
-Composer's built-in [trainer](https://docs.mosaicml.com/en/stable/trainer/
-using_the_trainer.html) makes it easy to **add multiple speedup methods in a
-single line of code!** Trying out new methods or combinations of methods is as
-easy as changing a single list. As we continually implement more methods, they
-will be easy for you to add to your code. For concrete examples of methods in
-Composer, here are some ([_see here for all_](https://docs.mosaicml.com/en/
-latest/trainer/algorithms.html)) speedup methods currently in Composer:
+from composer import Trainer from composer.algorithms import ChannelsLast,
+CutMix, LabelSmoothing from composer.models import mnist_model transform =
+transforms.Compose([transforms.ToTensor()]) train_dataset = datasets.MNIST
+("data", download=True, train=True, transform=transform) eval_dataset =
+datasets.MNIST("data", download=True, train=False, transform=transform)
+train_dataloader = DataLoader(train_dataset, batch_size=128) eval_dataloader =
+DataLoader(eval_dataset, batch_size=128) trainer = Trainer( model=mnist_model
+(), train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
+max_duration="2ep", algorithms=[ ChannelsLast(), CutMix(alpha=1.0),
+LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```  Composer's built-in
+[trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html)
+makes it easy to **add multiple speedup methods in a single line of code!**
+Trying out new methods or combinations of methods is as easy as changing a
+single list. As we continually implement more methods, they will be easy for
+you to add to your code. For concrete examples of methods in Composer, here are
+some ([_see here for all_](https://docs.mosaicml.com/en/latest/trainer/
+algorithms.html)) speedup methods currently in Composer:
 Name|Attribution|tl;dr|Example Benchmark|Speed Up*| ----|-----------|-----|----
 -----|---------| [Alibi](https://github.com/mosaicml/composer/tree/dev/
 composer/algorithms/alibi)|[Press et al, 2021](https://arxiv.org/abs/
 2108.12409)|Replace attention with AliBi.|GPT-2|1.5x [BlurPool](https://
 github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|[Zhang,
 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter before
 every downsampling operation.|ResNet-101|1.2x [ChannelsLast](https://
@@ -230,14 +228,14 @@
                                         An interactive Colab Notebook aimed at
 Training_BERTs_with_Composer            helping users learn how to train BERT
                                         models with Composer!
 We're_Hiring!                           Join us! ð¤©
 If you have any questions, please feel free to reach out to us on [Twitter]
 (https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our
 [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-
-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg)! # ð« Contributors Composer is part of the
+1dc6mo5wg-arlv6Oo9JjEn_g4d5s7PXQ)! # ð« Contributors Composer is part of the
 broader Machine Learning community, and we welcome any contributions, pull
 requests, or issues! To start contributing, see our [Contributing](https://
 github.com/mosaicml/composer/blob/dev/CONTRIBUTING.md) page. # âï¸ Citation
 ``` @misc{mosaicml2022composer, author = {The Mosaic ML Team}, title =
 {composer}, year = {2021}, howpublished = {\url{https://github.com/mosaicml/
 composer/}}, } ```
```

### Comparing `mosaicml-0.8.2/composer/__init__.py` & `mosaicml-0.9.0/composer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Composer."""
 
+from composer._version import __version__
 from composer.core import Algorithm, Callback, DataSpec, Engine, Evaluator, Event, State, Time, Timestamp, TimeUnit
 from composer.loggers import Logger
 from composer.models import ComposerModel
 from composer.trainer import Trainer
 
 __all__ = [
     'Algorithm',
@@ -19,9 +20,7 @@
     'Time',
     'Timestamp',
     'TimeUnit',
     'Logger',
     'ComposerModel',
     'Trainer',
 ]
-
-__version__ = '0.8.2'
```

### Comparing `mosaicml-0.8.2/composer/algorithms/__init__.py` & `mosaicml-0.9.0/composer/algorithms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Efficiency methods for training.
 
-Examples include :class:`~composer.algorithms.label_smoothing.LabelSmoothing`
-and adding :class:`~composer.algorithms.squeeze_excite.SqueezeExcite` blocks,
+Examples include :class:`.LabelSmoothing` and adding :class:`.SqueezeExcite` blocks,
 among many others.
 
 Algorithms are implemented in both a standalone functional form (see :mod:`composer.functional`)
 and as subclasses of :class:`Algorithm` for integration in the Composer :class:`Trainer`.
 The former are easier to integrate piecemeal into an existing codebase.
 The latter are easier to compose together, since they all have the same public interface
-and work automatically with the Composer :py:class:`~composer.trainer.Trainer`.
+and work automatically with the Composer :py:class:`.Trainer`.
 
 For ease of composability, algorithms in our Trainer are based on the two-way callbacks concept from
 `Howard et al, 2020 <https://arxiv.org/abs/2002.04688>`_. Each algorithm implements two methods:
 
 * :meth:`Algorithm.match`: returns ``True`` if the algorithm should be run given the current
-  :class:`State` and :class:`~composer.core.event.Event`.
+  :class:`State` and :class:`.Event`.
 * :meth:`Algorithm.apply`: performs an in-place modification of the given
   :class:`State`
 
 For example, a simple algorithm that shortens training:
 
 .. code-block:: python
 
@@ -31,15 +30,15 @@
 
         def match(self, state: State, event: Event, logger: Logger) -> bool:
             return event == Event.INIT
 
         def apply(self, state: State, event: Event, logger: Logger):
             state.max_duration /= 2  # cut training time in half
 
-For more information about events, see :class:`~composer.core.event.Event`.
+For more information about events, see :class:`.Event`.
 """
 
 from composer.algorithms.alibi import Alibi
 from composer.algorithms.augmix import AugmentAndMixTransform, AugMix
 from composer.algorithms.blurpool import BlurPool
 from composer.algorithms.channels_last import ChannelsLast
 from composer.algorithms.colout import ColOut, ColOutTransform
```

### Comparing `mosaicml-0.8.2/composer/algorithms/algorithm_hparams_registry.py` & `mosaicml-0.9.0/composer/algorithms/algorithm_hparams_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/alibi/__init__.py` & `mosaicml-0.9.0/composer/algorithms/alibi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,11 +4,10 @@
 """ALiBi (Attention with Linear Biases; `Press et al, 2021 <https://arxiv.org/abs/2108.12409>`_) dispenses with position
 embeddings for tokens in transformer-based NLP models, instead encoding position information by biasing the query-key
 attention scores proportionally to each token pair's distance.
 
 See the :doc:`Method Card </method_cards/alibi>` for more details.
 """
 
-from composer.algorithms.alibi import _gpt2_alibi as _gpt2_alibi
 from composer.algorithms.alibi.alibi import Alibi, apply_alibi
 
 __all__ = ['Alibi', 'apply_alibi']
```

### Comparing `mosaicml-0.8.2/composer/algorithms/alibi/_gpt2_alibi.py` & `mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,44 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-# _attn is used by the yaml codepath, even though it is private
-# pyright: reportUnusedFunction=none
+from types import MethodType
 from typing import Tuple
 
 import torch
+from transformers.models.gpt2.modeling_gpt2 import GPT2Attention, GPT2Model
+
+from composer.algorithms.alibi.attention_surgery_functions.utils import (policy_registry, register_alibi,
+                                                                         zero_and_freeze_expand_position_embeddings)
+
+
+@policy_registry.register(GPT2Model)
+def gpt2_embedding_converter(module: torch.nn.Module, module_index: int, max_sequence_length: int) -> torch.nn.Module:
+    """Removes positional embeddings."""
+    assert isinstance(module, GPT2Model)
+    del module_index  # unused
+
+    zero_and_freeze_expand_position_embeddings(module, max_sequence_length, position_embedding_attribute='wpe')
+    return module
+
+
+@policy_registry.register(GPT2Attention)
+def gpt2_attention_converter(module: torch.nn.Module, module_index: int, max_sequence_length: int) -> torch.nn.Module:
+    """Adds ALiBi to GPT2Attention and replaces the attention mask to support `max_sequence_length` tokens."""
+
+    assert isinstance(module, GPT2Attention)
+    del module_index  # unused
+    module = register_alibi(module=module,
+                            n_heads=int(module.num_heads),
+                            max_token_length=max_sequence_length,
+                            causal=True)
+    setattr(module, '_attn', MethodType(_attn, module))
+
+    module = enlarge_mask(module, max_sequence_length)
+    return module
 
 
 def _attn(self, query, key, value, attention_mask=None, head_mask=None) -> Tuple[torch.Tensor, torch.Tensor]:
     """Replication of identically-named attention function function ("_attn") in Composer/HuggingFace GPT2 model's
     GPT2Attention (:func:`transformers.models.gpt2.modeling_gpt2.GPT2Attention._attn`; `GitHub link <https://\\
     github.com/huggingface/transformers/blob/2e11a043374a6229ec129a4765ee4ba7517832b9/src/transformers/models/\\
     gpt2/modeling_gpt2.py#L192>`_), but this function implements ALiBi and will be used to replace the default attention
```

### Comparing `mosaicml-0.8.2/composer/algorithms/augmix/__init__.py` & `mosaicml-0.9.0/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/augmix/augmix.py` & `mosaicml-0.9.0/composer/algorithms/augmix/augmix.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                  alpha: float = 1.0,
                  augmentation_set: List = augmentation_sets['all']) -> ImgT:
     r"""Applies the AugMix (`Hendrycks et al, 2020 <http://arxiv.org/abs/1912.02781>`_) data augmentation.
 
     This function works on a single image or batch of images. See :class:`.AugMix` and
     the :doc:`Method Card </method_cards/augmix>` for details. This function only acts on a
     single image (or batch) per call and is unlikely to be used in a training loop.
-    Use :class:`~composer.algorithms.augmix.augmix.AugmentAndMixTransform` to use AugMix as
+    Use :class:`.AugmentAndMixTransform` to use AugMix as
     part of a :class:`torchvision.datasets.VisionDataset`\'s ``transform``.
 
     Example:
         .. testcode::
 
             import composer.functional as cf
 
@@ -170,15 +170,15 @@
 
     AugMix (`Hendrycks et al, 2020 <http://arxiv.org/abs/1912.02781>`_) creates ``width`` sequences of ``depth``
     image augmentations, applies each sequence with random intensity, and returns a convex combination of the ``width``
     augmented images and the original image.  The coefficients for mixing the augmented images are drawn from a uniform
     ``Dirichlet(alpha, alpha, ...)`` distribution. The coefficient for mixing the combined augmented image and the
     original image is drawn from a ``Beta(alpha, alpha)`` distribution, using the same ``alpha``.
 
-    This algorithm runs on on :attr:`~composer.core.event.Event.FIT_START` to insert a dataset transformation.
+    This algorithm runs on on :attr:`.Event.FIT_START` to insert a dataset transformation.
     It is a no-op if this algorithm already applied itself on the :attr:`State.train_dataloader.dataset`.
 
     See the :doc:`Method Card </method_cards/augmix>` for more details.
 
     Example:
         .. testcode::
```

### Comparing `mosaicml-0.8.2/composer/algorithms/blurpool/__init__.py` & `mosaicml-0.9.0/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/blurpool/blurpool.py` & `mosaicml-0.9.0/composer/algorithms/blurpool/blurpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     return model
 
 
 class BlurPool(Algorithm):
     """`BlurPool <http://proceedings.mlr.press/v97/zhang19a.html>`_ adds anti-aliasing filters to convolutional layers.
 
     This algorithm increases accuracy and invariance to small shifts in the input. It runs on
-    :attr:`~composer.core.event.Event.INIT`.
+    :attr:`.Event.INIT`.
 
     Args:
         replace_convs (bool): replace strided :class:`torch.nn.Conv2d` modules with
             :class:`.BlurConv2d` modules. Default: ``True``.
         replace_maxpools (bool): replace eligible :class:`torch.nn.MaxPool2d` modules
             with :class:`.BlurMaxPool2d` modules. Default: ``True``.
         blur_first (bool): when ``replace_convs`` is ``True``, blur input before the
```

### Comparing `mosaicml-0.8.2/composer/algorithms/blurpool/blurpool_layers.py` & `mosaicml-0.9.0/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     This function can be understood as decoupling the max from the pooling, and
     inserting a low-pass filtering step between the two. Concretely, this
     function computes the max within spatial neighborhoods of shape
     ``kernel_size``, then applies an anti-aliasing filter to smooth the maxes,
     and only then pools according to ``stride``.
 
-    See also: :func:`~blur_2d`.
+    See also: :func:`.blur_2d`.
 
     Args:
         input (torch.Tensor): A 4d tensor of shape NCHW
         kernel_size (int | tuple, optional): Size(s) of the spatial neighborhoods over which to pool.
             This is mostly commonly 2x2. If only a scalar ``s`` is provided, the
             neighborhood is of size ``(s, s)``. Default: ``(2, 2)``.
         stride (int | tuple, optional): Stride(s) along H and W axes. If a single value is passed, this
@@ -146,15 +146,15 @@
 
     The only API difference is that the parameter ``return_indices`` is not
     available, because it is ill-defined when using anti-aliasing.
 
     See the associated `paper <http://proceedings.mlr.press/v97/zhang19a.html>`_
     for more details, experimental results, etc.
 
-    See :func:`~blurmax_pool2d` for details.
+    See :func:`.blurmax_pool2d` for details.
     """
 
     # based on https://pytorch.org/docs/stable/_modules/torch/nn/modules/pooling.html#MaxPool2d # noqa
 
     def __init__(self,
                  kernel_size: _size_2_t,
                  stride: Optional[_size_2_t] = None,
@@ -183,15 +183,15 @@
                               stride=self.stride,
                               padding=self.padding,
                               dilation=self.dilation,
                               ceil_mode=self.ceil_mode,
                               filter=self.filt2d)
 
     @staticmethod
-    def from_maxpool2d(module: torch.nn.MaxPool2d, module_index: int):
+    def from_maxpool2d(module: torch.nn.MaxPool2d, module_index: int) -> 'BlurMaxPool2d':
         return BlurMaxPool2d(kernel_size=module.kernel_size,
                              stride=module.stride,
                              padding=module.padding,
                              dilation=module.dilation,
                              ceil_mode=module.ceil_mode)
 
 
@@ -211,15 +211,15 @@
     this approach most closely matches the behavior specified in the paper.
 
     This module should only be used to replace strided convolutions.
 
     See the associated `paper <http://proceedings.mlr.press/v97/zhang19a.html>`_
     for more details, experimental results, etc.
 
-    See also: :func:`~blur_2d`.
+    See also: :func:`.blur_2d`.
     """
 
     # based partially on https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv2d
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
@@ -291,15 +291,15 @@
             if has_bias:
                 blurconv.conv.bias.copy_(module.bias)
 
         return blurconv
 
 
 class BlurPool2d(nn.Module):
-    """This module just calls :func:`~blur_2d` in ``forward`` using the provided arguments."""
+    """This module just calls :func:`.blur_2d` in ``forward`` using the provided arguments."""
 
     def __init__(self, stride: _size_2_t = 2, padding: _size_2_t = 1) -> None:
         super(BlurPool2d, self).__init__()
         self.stride = stride
         self.padding = padding
         self.register_buffer('filt2d', _default_2d_filter())
```

### Comparing `mosaicml-0.8.2/composer/algorithms/channels_last/__init__.py` & `mosaicml-0.9.0/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/channels_last/channels_last.py` & `mosaicml-0.9.0/composer/algorithms/channels_last/channels_last.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     model.to(memory_format=torch.channels_last)  # type: ignore
 
 
 class ChannelsLast(Algorithm):
     """Changes the memory format of the model to `torch.channels_last <https://\\
     pytorch.org/tutorials/intermediate/memory_format_tutorial.html>`_. This usually improves GPU utilization.
 
-    Runs on :attr:`~composer.core.event.Event.INIT``, so it can set the memory format before the model is DDP wrapped.
+    Runs on :attr:`.Event.INIT``, so it can set the memory format before the model is DDP wrapped.
     Has no hyperparameters.
 
     Example:
         .. testcode::
 
             from composer.algorithms import ChannelsLast
             algorithm = ChannelsLast()
```

### Comparing `mosaicml-0.8.2/composer/algorithms/channels_last/metadata.json` & `mosaicml-0.9.0/composer/algorithms/channels_last/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/colout/__init__.py` & `mosaicml-0.9.0/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/colout/colout.py` & `mosaicml-0.9.0/composer/algorithms/colout/colout.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,18 +156,18 @@
 
 
 class ColOut(Algorithm):
     """Drops a fraction of the rows and columns of an input image and (optionally) a target image. If the fraction of
     rows/columns dropped isn't too large, this does not significantly alter the content of the image, but reduces its
     size and provides extra variability.
 
-    If ``batch`` is True (the default), then this algorithm runs on :attr:`~composer.core.event.Event.AFTER_DATALOADER`
+    If ``batch`` is True (the default), then this algorithm runs on :attr:`.Event.AFTER_DATALOADER`
     to modify the batch.
 
-    Otherwise, if ``batch=False`` (the default), this algorithm runs on :attr:`~composer.core.event.Event.INIT` to insert
+    Otherwise, if ``batch=False`` (the default), this algorithm runs on :attr:`.Event.INIT` to insert
     a dataset transformation. It is a no-op if this algorithm already applied itself on the :attr:`State.train_dataloader.dataset`.
 
     See the :doc:`Method Card </method_cards/colout>` for more details.
 
     Example:
          .. testcode::
```

### Comparing `mosaicml-0.8.2/composer/algorithms/cutmix/__init__.py` & `mosaicml-0.9.0/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/cutmix/cutmix.py` & `mosaicml-0.9.0/composer/algorithms/cutmix/cutmix.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,33 +7,31 @@
 
 import logging
 from typing import Any, Callable, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from torch import Tensor
-from torch.nn import functional as F
 
 from composer.core import Algorithm, Event, State
 from composer.loggers import Logger
-from composer.loss.utils import check_for_index_targets
+from composer.loss.utils import ensure_targets_one_hot
 
 log = logging.getLogger(__name__)
 
 __all__ = ['CutMix', 'cutmix_batch']
 
 
 def cutmix_batch(input: Tensor,
                  target: Tensor,
-                 num_classes: int,
                  length: Optional[float] = None,
                  alpha: float = 1.,
                  bbox: Optional[Tuple] = None,
                  indices: Optional[torch.Tensor] = None,
-                 uniform_sampling: bool = False) -> Tuple[torch.Tensor, torch.Tensor]:
+                 uniform_sampling: bool = False) -> Tuple[torch.Tensor, torch.Tensor, float, Tuple]:
     """Create new samples using combinations of pairs of samples.
 
     This is done by masking a region of each image in ``input`` and filling
     the masked region with the corresponding content from a random different
     image in``input``.
 
     The position of the masked region is determined by drawing a center point
@@ -60,15 +58,14 @@
         input (torch.Tensor): input tensor of shape ``(N, C, H, W)``.
         target (torch.Tensor): target tensor of either shape ``N`` or
             ``(N, num_classes)``. In the former case, elements of ``target``
             must be integer class ids in the range ``0..num_classes``. In the
             latter case, rows of ``target`` may be arbitrary vectors of targets,
             including, e.g., one-hot encoded class labels, smoothed class
             labels, or multi-output regression targets.
-        num_classes (int): total number of classes or output variables
         length (float, optional): Relative side length of the masked region.
             If specified, ``length`` is interpreted as a fraction of ``H`` and
             ``W``, and the resulting box is of size ``(length * H, length * W)``.
             Default: ``None``.
         alpha (float, optional): parameter for the Beta distribution over
             the fraction of the input to mask. Ignored if ``length`` is
             provided. Default: ``1``.
@@ -80,40 +77,33 @@
             such that each pixel has an equal probability of being mixed.
             If ``False``, defaults to the sampling used in the original paper
             implementation. Default: ``False``.
 
     Returns:
         input_mixed (torch.Tensor): batch of inputs after cutmix has been
             applied.
-        target_mixed (torch.Tensor): soft labels for mixed input samples.
-            These are a convex combination of the (possibly one-hot-encoded)
-            labels from the original samples and the samples chosen to fill
-            the masked regions, with the relative weighting equal to the
-            fraction of the spatial size that is cut.
-            E.g., if a sample was originally an image with label ``0`` and
-            40% of the image of was replaced with data from an image with label
-            ``2``, the resulting labels, assuming only three classes, would be
-            ``[1, 0, 0] * 0.6 + [0, 0, 1] * 0.4 = [0.6, 0, 0.4]``.
+        target_perm (torch.Tensor): The labels of the mixed-in examples
+        area (float): The fractional area of the unmixed region.
+        bounding_box (tuple): the ``(left, top, right, bottom)`` coordinates of
+            the bounding box that defines the mixed region.
 
     Raises:
         ValueError: If both ``length`` and ``bbox`` are provided.
 
     Example:
         .. testcode::
 
             import torch
             from composer.functional import cutmix_batch
 
             N, C, H, W = 2, 3, 4, 5
             num_classes = 10
             X = torch.randn(N, C, H, W)
             y = torch.randint(num_classes, size=(N,))
-            X_mixed, y_mixed = cutmix_batch(
-                X, y, num_classes=num_classes, alpha=0.2
-            )
+            X_mixed, target_perm, area, _ = cutmix_batch(X, y, alpha=0.2)
     """
     if bbox is not None and length is not None:
         raise ValueError(f'Cannot provide both length and bbox; got {length} and {bbox}')
 
     # Create shuffled indicies across the batch in preparation for cutting and mixing.
     # Use given indices if there are any.
     if indices is None:
@@ -142,48 +132,41 @@
         rx, ry, rw, rh = _rand_bbox(input.shape[2], input.shape[3], cutmix_lambda, uniform_sampling=uniform_sampling)
         bbox = (rx, ry, rw, rh)
 
     # Fill in the box with a part of a random image.
     X_cutmix[:, :, rx:rw, ry:rh] = X_cutmix[shuffled_idx, :, rx:rw, ry:rh]
     # adjust lambda to exactly match pixel ratio. This is an implementation detail taken from
     # the original implementation, and implies lambda is not actually beta distributed.
-    adjusted_lambda = _adjust_lambda(cutmix_lambda, input, bbox)
+    adjusted_lambda = _adjust_lambda(input, bbox)
 
     # Make a shuffled version of y for interpolation
     y_shuffled = target[shuffled_idx]
-    # Interpolate between labels using the adjusted lambda
-    # First check if labels are indices. If so, convert them to onehots.
-    # This is under the assumption that the loss expects torch.LongTensor, which is true for pytorch cross_entropy
-    if check_for_index_targets(target):
-        y_onehot = F.one_hot(target, num_classes=num_classes)
-        y_shuffled_onehot = F.one_hot(y_shuffled, num_classes=num_classes)
-        y_cutmix = adjusted_lambda * y_onehot + (1 - adjusted_lambda) * y_shuffled_onehot
-    else:
-        y_cutmix = adjusted_lambda * target + (1 - adjusted_lambda) * y_shuffled
 
-    return X_cutmix, y_cutmix
+    return X_cutmix, y_shuffled, adjusted_lambda, bbox
 
 
 class CutMix(Algorithm):
     """`CutMix <https://arxiv.org/abs/1905.04899>`_ trains the network on non-overlapping combinations
     of pairs of examples and interpolated targets rather than individual examples and targets.
 
     This is done by taking a non-overlapping combination of a given batch X with a
     randomly permuted copy of X. The area is drawn from a ``Beta(alpha, alpha)``
     distribution.
 
     Training in this fashion sometimes reduces generalization error.
 
     Args:
-        num_classes (int): the number of classes in the task labels.
         alpha (float, optional): the psuedocount for the Beta distribution
             used to sample area parameters. As ``alpha`` grows, the two samples
             in each pair tend to be weighted more equally. As ``alpha``
             approaches 0 from above, the combination approaches only using
             one element of the pair. Default: ``1``.
+        interpolate_loss (bool, optional): Interpolates the loss rather than the labels.
+            A useful trick when using a cross entropy loss. Will produce incorrect behavior
+            if the loss is not a linear function of the targets. Default: ``False``
         uniform_sampling (bool, optional): If ``True``, sample the bounding
             box such that each pixel has an equal probability of being mixed.
             If ``False``, defaults to the sampling used in the original
             paper implementation. Default: ``False``.
         input_key (str | int | Tuple[Callable, Callable] | Any, optional): A key that indexes to the input
             from the batch. Can also be a pair of get and set functions, where the getter
             is assumed to be first in the pair.  The default is 0, which corresponds to any sequence, where the first element
@@ -193,69 +176,124 @@
             is assumed to be first in the pair. The default is 1, which corresponds to any sequence, where the second element
             is the target. Default: ``1``.
 
     Example:
         .. testcode::
 
             from composer.algorithms import CutMix
-            algorithm = CutMix(num_classes=10, alpha=0.2)
+            algorithm = CutMix(alpha=0.2)
             trainer = Trainer(
                 model=model,
                 train_dataloader=train_dataloader,
                 eval_dataloader=eval_dataloader,
                 max_duration="1ep",
                 algorithms=[algorithm],
                 optimizers=[optimizer]
             )
     """
 
     def __init__(
         self,
-        num_classes: int,
         alpha: float = 1.,
+        interpolate_loss: bool = False,
         uniform_sampling: bool = False,
         input_key: Union[str, int, Tuple[Callable, Callable], Any] = 0,
         target_key: Union[str, int, Tuple[Callable, Callable], Any] = 1,
     ):
-        self.num_classes = num_classes
         self.alpha = alpha
+        self.interpolate_loss = interpolate_loss
         self._uniform_sampling = uniform_sampling
+
         self._indices = torch.Tensor()
         self._cutmix_lambda = 0.0
         self._bbox: Tuple[int, int, int, int] = (0, 0, 0, 0)
+        self._permuted_target = torch.Tensor()
+        self._adjusted_lambda = 0.0
         self.input_key, self.target_key = input_key, target_key
 
     def match(self, event: Event, state: State) -> bool:
-        return event == Event.AFTER_DATALOADER
+        if self.interpolate_loss:
+            return event in [Event.BEFORE_FORWARD, Event.BEFORE_BACKWARD]
+        else:
+            return event in [Event.BEFORE_FORWARD, Event.BEFORE_LOSS]
 
     def apply(self, event: Event, state: State, logger: Logger) -> None:
         input = state.batch_get_item(key=self.input_key)
         target = state.batch_get_item(key=self.target_key)
 
-        assert isinstance(input, Tensor) and isinstance(target, Tensor), \
-            'Multiple tensors for inputs or targets not supported yet.'
-        alpha = self.alpha
+        if not isinstance(input, torch.Tensor):
+            raise NotImplementedError('Multiple tensors for inputs not supported yet.')
+        if not isinstance(target, torch.Tensor):
+            raise NotImplementedError('Multiple tensors for targets not supported yet.')
 
-        # these are saved only for testing
-        self._indices = _gen_indices(input)
-        _cutmix_lambda = _gen_cutmix_coef(alpha)
-        self._bbox = _rand_bbox(input.shape[2], input.shape[3], _cutmix_lambda, uniform_sampling=self._uniform_sampling)
-        self._cutmix_lambda = _adjust_lambda(_cutmix_lambda, input, self._bbox)
-
-        new_input, new_target = cutmix_batch(
-            input=input,
-            target=target,
-            num_classes=self.num_classes,
-            alpha=alpha,
-            bbox=self._bbox,
-            indices=self._indices,
-        )
+        alpha = self.alpha
 
-        state.batch_set_item(key=self.input_key, value=new_input)
-        state.batch_set_item(key=self.target_key, value=new_target)
+        if event == Event.BEFORE_FORWARD:
+            # these are saved only for testing
+            self._indices = _gen_indices(input)
+
+            _cutmix_lambda = _gen_cutmix_coef(alpha)
+            self._bbox = _rand_bbox(input.shape[2],
+                                    input.shape[3],
+                                    _cutmix_lambda,
+                                    uniform_sampling=self._uniform_sampling)
+            self._adjusted_lambda = _adjust_lambda(input, self._bbox)
+
+            new_input, self._permuted_target, _, _ = cutmix_batch(input=input,
+                                                                  target=target,
+                                                                  alpha=self.alpha,
+                                                                  bbox=self._bbox,
+                                                                  indices=self._indices,
+                                                                  uniform_sampling=self._uniform_sampling)
+
+            state.batch_set_item(key=self.input_key, value=new_input)
+
+        if not self.interpolate_loss and event == Event.BEFORE_LOSS:
+            # Interpolate the targets
+            if not isinstance(state.outputs, torch.Tensor):
+                raise NotImplementedError('Multiple output tensors not supported yet')
+            if not isinstance(target, torch.Tensor):
+                raise NotImplementedError('Multiple target tensors not supported yet')
+            if self._permuted_target.ndim > 2 and self._permuted_target.shape[-2:] == input.shape[-2:]:
+                # Target has the same height and width as the input, no need to interpolate.
+                x1, y1, x2, y2 = self._bbox
+                target[..., x1:x2, y1:y2] = self._permuted_target[..., x1:x2, y1:y2]
+            else:
+                # Need to interpolate on dense/one-hot targets.
+                target = ensure_targets_one_hot(state.outputs, target)
+                permuted_target = ensure_targets_one_hot(state.outputs, self._permuted_target)
+                # Interpolate to get the new target
+                target = self._adjusted_lambda * target + (1 - self._adjusted_lambda) * permuted_target
+            # Create the new batch
+            state.batch_set_item(key=self.target_key, value=target)
+
+        if self.interpolate_loss and event == Event.BEFORE_BACKWARD:
+            if self._permuted_target.ndim > 2 and self._permuted_target.shape[-2:] == input.shape[-2:]:
+                raise ValueError("Can't interpolate loss when target has the same height and width as the input")
+
+            # Grab the loss function
+            if hasattr(state.model, 'loss'):
+                loss_fn = state.model.loss
+            elif hasattr(state.model, 'module') and hasattr(state.model.module, 'loss'):
+                if isinstance(state.model.module, torch.nn.Module):
+                    loss_fn = state.model.module.loss
+                else:
+                    raise TypeError('state.model.module must be a torch module')
+            else:
+                raise AttributeError('Loss must be accessible via model.loss or model.module.loss')
+            # Verify that the loss is callable
+            if not callable(loss_fn):
+                raise TypeError('Loss must be callable')
+            # Interpolate the loss
+            new_loss = loss_fn(state.outputs, (input, self._permuted_target))
+            if not isinstance(state.loss, torch.Tensor):
+                raise NotImplementedError('Multiple losses not supported yet')
+            if not isinstance(new_loss, torch.Tensor):
+                raise NotImplementedError('Multiple losses not supported yet')
+            state.loss = self._adjusted_lambda * state.loss + (1 - self._adjusted_lambda) * new_loss
 
 
 def _gen_indices(x: Tensor) -> Tensor:
     """Generates indices of a random permutation of elements of a batch.
 
     Args:
         x (torch.Tensor): input tensor of shape ``(B, d1, d2, ..., dn)``,
@@ -335,19 +373,18 @@
     bby1 = np.clip(cy - cut_h // 2, 0, H)
     bbx2 = np.clip(cx + cut_w // 2, 0, W)
     bby2 = np.clip(cy + cut_h // 2, 0, H)
 
     return bbx1, bby1, bbx2, bby2
 
 
-def _adjust_lambda(cutmix_lambda: float, x: Tensor, bbox: Tuple) -> float:
+def _adjust_lambda(x: Tensor, bbox: Tuple) -> float:
     """Rescale the cutmix lambda according to the size of the clipped bounding box.
 
     Args:
-        cutmix_lambda (float): Lambda param from cutmix, used to set the area of the box.
         x (torch.Tensor): input tensor of shape ``(B, d1, d2, ..., dn)``, B is batch size, d1-dn
             are feature dimensions.
         bbox (tuple): (x1, y1, x2, y2) coordinates of the boundind box, obeying x2 > x1, y2 > y1.
 
     Returns:
         adjusted_lambda: Rescaled cutmix_lambda to account for part of the bounding box
             being potentially out of bounds of the input.
```

### Comparing `mosaicml-0.8.2/composer/algorithms/cutmix/metadata.json` & `mosaicml-0.9.0/composer/algorithms/cutmix/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/cutout/cutout.py` & `mosaicml-0.9.0/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/ema/ema.py` & `mosaicml-0.9.0/composer/algorithms/ema/ema.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/factorize/__init__.py` & `mosaicml-0.9.0/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/factorize/factorize.py` & `mosaicml-0.9.0/composer/algorithms/factorize/factorize.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     allow larger intermediate ranks.
 
     See :func:`.factorize_matrix` and :func:`.factorize_conv2d` for more
     information about the factorization process. See :class:`.FactorizedConv2d`
     and :class:`.FactorizedLinear` for more information about the factorized modules
     used to replace the original modules.
 
-    Runs on :attr:`~composer.core.event.Event.INIT`.
+    Runs on :attr:`.Event.INIT`.
 
     Args:
         factorize_convs (bool): whether to try factorizing :class:`torch.nn.Conv2d` modules.
             Default: ``True``.
         factorize_linears (bool): whether to try factorizing :class:`torch.nn.Linear` modules.
             Default: ``True``.
         min_channels (int): if a :class:`torch.nn.Conv2d` module does not have at least
```

### Comparing `mosaicml-0.8.2/composer/algorithms/factorize/factorize_core.py` & `mosaicml-0.9.0/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/factorize/factorize_modules.py` & `mosaicml-0.9.0/composer/algorithms/factorize/factorize_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     def _create_child_modules(self) -> Tuple[torch.nn.Module, torch.nn.Module]:
         """This is used to populate the self.module0 and self.module1 attributes; it's not part of __init__ because the
         logic to initialize them is subclass-specific and might depend on the shared logic in __init__"""
         ...
 
     @abc.abstractmethod
     def solution_for_rank(self, input: torch.Tensor, rank: int) -> LowRankSolution:
-        """Returns a solution that :meth:`~apply_solution` can use to update the module's level of factorization.
+        """Returns a solution that :meth:`.apply_solution` can use to update the module's level of factorization.
 
         This is seperate from :meth:`set_rank` so that one can generate and assess
         many possible solutions for a given module before choosing one.
 
         Args:
             input (torch.Tensor): An input to the module used to optimize the solution's
                 weights. The optimization seeks to preserve the module's
@@ -205,15 +205,15 @@
         This *always* applies the solution and doesn't check whether
         using the solution is worthwhile.
 
         Args:
             solution (LowRankSolution): An object encapsulating the new
                 parameters to be used and their associated mean squared error on
                 the input for which they were optimized. Can be obtained using
-                :meth:`~solution_for_rank`.
+                :meth:`.solution_for_rank`.
         """
         ...
 
 
 class FactorizedConv2d(_FactorizedModule):
     """Factorized replacement for :class:`torch.nn.Conv2d`.
 
@@ -253,15 +253,15 @@
 
     Raises:
         ValueError:
             If ``latent_channels`` is not small enough for factorization
             to reduce the number of multiply-add operations. In this regime,
             factorization is both slower and less expressive than a
             non-factorized operation. Setting
-            ``latent_features`` to  :meth:`~max_allowed_latent_channels`
+            ``latent_features`` to  :meth:`.max_allowed_latent_channels`
             or a smaller value is sufficient to avoid this.
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: _size_2_t,
@@ -395,15 +395,15 @@
     Raises:
         ValueError:
             If ``latent_features`` is not small enough for factorization
             to reduce the number of multiply-add operations. In this regime,
             factorization is both slower and less expressive than a
             non-factorized operation. Setting
             ``latent_features < min(in_features, out_features) / 2`` or
-            using :meth:`~max_allowed_latent_features` is sufficient to avoid
+            using :meth:`.max_allowed_latent_features` is sufficient to avoid
             this.
     """
 
     def __init__(self,
                  in_features: int,
                  out_features: int,
                  bias: bool = True,
```

### Comparing `mosaicml-0.8.2/composer/algorithms/fused_layernorm/__init__.py` & `mosaicml-0.9.0/composer/algorithms/fused_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/fused_layernorm/fused_layernorm.py` & `mosaicml-0.9.0/composer/algorithms/fused_layernorm/fused_layernorm.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/fused_layernorm/metadata.json` & `mosaicml-0.9.0/composer/algorithms/fused_layernorm/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/gated_linear_units/__init__.py` & `mosaicml-0.9.0/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `mosaicml-0.9.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/gated_linear_units/gated_linear_units.py` & `mosaicml-0.9.0/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 import logging
 import warnings
 from typing import Callable, Dict, Optional, Sequence, Type, Union
 
 import torch
 
+from composer.models.huggingface import HuggingFaceModel
+
 try:
+    from transformers import BertForMaskedLM, BertForSequenceClassification
     from transformers.models.bert.modeling_bert import BertIntermediate, BertOutput
     IS_TRANSFORMERS_INSTALLED = True
 except ImportError as e:
     IS_TRANSFORMERS_INSTALLED = False
 
 from composer.algorithms.gated_linear_units.gated_linear_unit_layers import BERTGatedFFOutput
 from composer.algorithms.warnings import NoEffectWarning
 from composer.core import Algorithm, Event, State
 from composer.loggers import Logger
-from composer.models import BERTModel
 from composer.utils import MissingConditionalImportError, module_surgery
 
 log = logging.getLogger(__name__)
 
 
 def from_BertOutput(layer: torch.nn.Module,
                     module_index: int,
@@ -75,17 +77,18 @@
             use the existing activation function in the model.
         gated_layer_bias (bool, optional): Whether to use biases in the linear layers within the GLU. Default: ``False``.
         non_gated_layer_bias (bool, optional): Whether to use biases in the linear layers within the GLU. Default: ``False``.
     """
     if not IS_TRANSFORMERS_INSTALLED:
         raise MissingConditionalImportError(extra_deps_group='nlp', conda_package='transformers')
 
-    # ensure that the model is an instance of a BERTModel, since our replacement policy is only defined for BERTs
-    if not isinstance(model, BERTModel):
-        raise TypeError('Gated Linear Units only has a surgery policy defined for instances of BERTModel.')
+    # ensure that the model is an instance of a BERT model, since our replacement policy is only defined for BERTs
+    if not isinstance(model, HuggingFaceModel) and not (isinstance(model.model, BertForMaskedLM) or
+                                                        isinstance(model.model, BertForSequenceClassification)):
+        raise TypeError('Gated Linear Units only has a surgery policy defined for instances of BERT models.')
 
     if act_fn is None:
         # get the activation functions used
         act_fns = {module.intermediate_act_fn for module in model.modules() if isinstance(module, BertIntermediate)}
 
         if len(act_fns) != 1:
             raise ValueError('The model has non-uniform activation functions, which is currently unsupported.')
@@ -111,22 +114,23 @@
         BertOutput: from_bound_BertOutput
     }
     replaced_instances = module_surgery.replace_module_classes(module=model, optimizers=optimizers, policies=policy)
     if len(replaced_instances) == 0:
         warnings.warn(
             NoEffectWarning(
                 'No instances of `torch.nn.LayerNorm` were found, and therefore, there were no modules to replace.'))
-    log.info(f'Successfully replaced {len(replaced_instances)} of LayerNorm with a Fused LayerNorm.')
+    log.info(
+        f'Successfully replaced {len(replaced_instances)} of BertIntermediate and BertOutput with a GatedLinearUnit.')
 
 
 class GatedLinearUnits(Algorithm):
     """Replaces all instances of Linear layers in the feed-forward subnetwork with a `Gated Linear Unit <https://arxiv.org/abs/2002.05202>`_.
     The Gated Linear Units provide a more expressive form for the same number of parameters, and a slight degredation to throughput.
 
-    Runs on :attr:`~composer.core.event.Event.INIT`, so it can swap the Linear layers in the FFN for GLUs before the model is DDP wrapped.
+    Runs on :attr:`.Event.INIT`, so it can swap the Linear layers in the FFN for GLUs before the model is DDP wrapped.
 
     Args:
         act_fn (Callable[[torch.Tensor], torch.Tensor], optional): Optionally, the activation function to use. If ``None``, the algorithm will
             use the existing activation function in the model.
         gated_layer_bias (bool, optional): Whether to use biases in the linear layers within the GLU. Default: ``False``.
         non_gated_layer_bias (bool, optional): Whether to use biases in the linear layers within the GLU. Default: ``False``.
```

### Comparing `mosaicml-0.8.2/composer/algorithms/gated_linear_units/metadata.json` & `mosaicml-0.9.0/composer/algorithms/gated_linear_units/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/__init__.py` & `mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     `Ghost Batch Normalization <https://arxiv.org/abs/1705.08741>`_ modules
     that simulate the effect of using a smaller batch size.
 
     Works by spliting input into chunks of ``ghost_batch_size`` samples and
     running batch normalization on each chunk separately. ``dim=0`` is assumed to
     be the sample axis.
 
-    Runs on :attr:`~composer.core.event.Event.INIT`.
+    Runs on :attr:`.Event.INIT`.
 
     Args:
         ghost_batch_size (int, optional): size of sub-batches to normalize over. Default: ``32``.
     """
 
     def __init__(self, ghost_batch_size: int = 32):
         self.ghost_batch_size = ghost_batch_size
```

### Comparing `mosaicml-0.8.2/composer/algorithms/ghost_batchnorm/metadata.json` & `mosaicml-0.9.0/composer/algorithms/ghost_batchnorm/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/gradient_clipping/gradient_clipping.py` & `mosaicml-0.9.0/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/gradient_clipping/metadata.json` & `mosaicml-0.9.0/composer/algorithms/gradient_clipping/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/label_smoothing/__init__.py` & `mosaicml-0.9.0/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/label_smoothing/label_smoothing.py` & `mosaicml-0.9.0/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/label_smoothing/metadata.json` & `mosaicml-0.9.0/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/layer_freezing/layer_freezing.py` & `mosaicml-0.9.0/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     has elapsed. The fraction of layers frozen increases linearly until it
     reaches ``freeze_level`` at the end of training.
 
     This freezing schedule is most similar to
     `FreezeOut <https://arxiv.org/abs/1706.04983>`_ and
     `Freeze Training <https://arxiv.org/abs/1706.05806>`_.
 
-    Runs on :attr:`~composer.core.event.Event.EPOCH_END`.
+    Runs on :attr:`.Event.EPOCH_END`.
 
     Example:
          .. testcode::
 
             from composer.algorithms import LayerFreezing
             from composer.trainer import Trainer
             layer_freezing_algorithm = LayerFreezing(
```

### Comparing `mosaicml-0.8.2/composer/algorithms/layer_freezing/metadata.json` & `mosaicml-0.9.0/composer/algorithms/layer_freezing/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/mixup/metadata.json` & `mosaicml-0.9.0/composer/algorithms/mixup/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/mixup/mixup.py` & `mosaicml-0.9.0/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/no_op_model/__init__.py` & `mosaicml-0.9.0/composer/algorithms/no_op_model/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Replaces model with a dummy model of type :class:`NoOpModelClass`.
 
 The algorithm runs on :attr:`Event.INIT`. It replaces the model in the state with
-a :class:`~composer.algorithms.no_op_model.no_op_model.NoOpModelClass` and then updates the parameters in the optimizer
+a :class:`.NoOpModelClass` and then updates the parameters in the optimizer
 through module surgery.
 
 A dummy model can helpful for profiling the dataloader by eliminating the work
 necessary to compute model outputs.
 """
 
 from composer.algorithms.no_op_model.no_op_model import NoOpModel as NoOpModel
```

### Comparing `mosaicml-0.8.2/composer/algorithms/no_op_model/no_op_model.py` & `mosaicml-0.9.0/composer/algorithms/no_op_model/no_op_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
     Args:
         original_model (torch.nn.Module): Model to replace.
     """
 
     def __init__(self, original_model: torch.nn.Module):
         super().__init__()
-        self.weights = torch.nn.Parameter(torch.Tensor([1.5]))
+        original_device = next(original_model.parameters()).device
+        self.weights = torch.nn.Parameter(torch.Tensor([1.5]).to(original_device))
         try:
             # For classification
             self.num_classes = original_model.num_classes
         except AttributeError:
             pass
 
     def loss(self, outputs: torch.Tensor, batch: Batch):
```

### Comparing `mosaicml-0.8.2/composer/algorithms/progressive_resizing/__init__.py` & `mosaicml-0.9.0/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/progressive_resizing/metadata.json` & `mosaicml-0.9.0/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/progressive_resizing/progressive_resizing.py` & `mosaicml-0.9.0/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/randaugment/metadata.json` & `mosaicml-0.9.0/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/randaugment/randaugment.py` & `mosaicml-0.9.0/composer/algorithms/randaugment/randaugment.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                                  augmentation_set=self.augmentation_set)
 
 
 class RandAugment(Algorithm):
     """Randomly applies a sequence of image data augmentations to an image.
 
     This algorithm (`Cubuk et al, 2019 <https://arxiv.org/abs/1909.13719>`_) runs on
-    :attr:`~composer.core.event.Event.INIT` to insert a dataset
+    :attr:`.Event.INIT` to insert a dataset
     transformation. It is a no-op if this algorithm already applied itself on the
     :attr:`.State.train_dataloader.dataset`.
 
     See the :doc:`Method Card </method_cards/randaugment>` for more details.
 
     Example:
         .. testcode::
```

### Comparing `mosaicml-0.8.2/composer/algorithms/sam/__init__.py` & `mosaicml-0.9.0/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/sam/sam.py` & `mosaicml-0.9.0/composer/algorithms/sam/sam.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 
 class SAM(Algorithm):
     """Adds sharpness-aware minimization (`Foret et al, 2020 <https://arxiv.org/abs/2010.01412>`_)
     by wrapping an existing optimizer with a :class:`.SAMOptimizer`. SAM can improve model generalization
     and provide robustness to label noise.
 
-    Runs on :attr:`~composer.core.event.Event.INIT`.
+    Runs on :attr:`.Event.INIT`.
 
     Args:
         rho (float, optional): The neighborhood size parameter of SAM. Must be greater than 0.
             Default: ``0.05``.
         epsilon (float, optional): A small value added to the gradient norm for numerical stability.
             Default: ``1e-12``.
         interval (int, optional): SAM will run once per ``interval`` steps. A value of 1 will
```

### Comparing `mosaicml-0.8.2/composer/algorithms/selective_backprop/__init__.py` & `mosaicml-0.9.0/composer/algorithms/selective_backprop/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """`Selective Backprop <https://arxiv.org/abs/1910.00762>`_ prunes minibatches according to the difficulty of the
 individual training examples, and only computes weight gradients over the pruned subset, reducing iteration time and
 speeding up training.
 
-The algorithm runs on :attr:`~composer.core.event.Event.INIT` and :attr:`~composer.core.event.Event.AFTER_DATLOADER`.
+The algorithm runs on :attr:`.Event.INIT` and :attr:`.Event.AFTER_DATLOADER`.
 On Event.INIT, it gets the loss function before the model is wrapped. On Event.AFTER_DATALOADER, it applies selective
 backprop if the time is between ``self.start`` and ``self.end``.
 
 See the :doc:`Method Card </method_cards/selective_backprop>` for more details.
 """
 
 from composer.algorithms.selective_backprop.selective_backprop import SelectiveBackprop as SelectiveBackprop
```

### Comparing `mosaicml-0.8.2/composer/algorithms/selective_backprop/metadata.json` & `mosaicml-0.9.0/composer/algorithms/selective_backprop/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/selective_backprop/selective_backprop.py` & `mosaicml-0.9.0/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/seq_length_warmup/metadata.json` & `mosaicml-0.9.0/composer/algorithms/seq_length_warmup/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `mosaicml-0.9.0/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,280 +1,199 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""Core code for sequence length warmup."""
-
-import textwrap
-from math import ceil
-from typing import Dict, Mapping, Optional
+import inspect
+import logging
+import math
+from operator import attrgetter
+from typing import Callable, Dict, Optional, Type
 
 import torch
-import torch.utils.data
-
-from composer.core import Algorithm, Event, State
-from composer.core.precision import get_precision_context
-from composer.core.time import TimeUnit
-from composer.core.types import Batch
-from composer.loggers import Logger
-from composer.models import ComposerTransformer
-from composer.utils import ensure_tuple
-
-__all__ = ['SeqLengthWarmup', 'set_batch_sequence_length']
-
-
-def set_batch_sequence_length(batch: Dict[str, torch.Tensor], curr_seq_len: int, truncate: bool = True) -> Batch:
-    """Set the sequence length of a batch.
 
-    Changes the sequence length of all tensors in the provided dictionary
-    to ``curr_seq_len`` by either truncating the tensors (``truncate=True``)
-    or reshaping the tensors to create new examples from the extra tokens
-    (``truncate=False``).
+log = logging.getLogger(__name__)
 
-    .. note::
-
-        The schedule for ``curr_seq_len`` over training time should be managed
-        outside of this function.
-
-    .. note::
+# Alibi applies module surgery to registered modules using their associated alibi replacement function.
+# Such functions must have the following signature:
+AlibiReplacementFunction = Callable[[torch.nn.Module, int, int], Optional[torch.nn.Module]]
+
+
+class PolicyRegistry(Dict[Type[torch.nn.Module], AlibiReplacementFunction]):
+    """A registry mapping for ALiBi surgery."""
+
+    def register(self,
+                 *modules: Type[torch.nn.Module]) -> Callable[[AlibiReplacementFunction], AlibiReplacementFunction]:
+        """This decorator registers mappings from torch module types to their ALiBi surgery functions.
+
+        To accommodate the specifics of composer's module surgery, our ALiBi implementation uses a
+        registry to create a ``Mapping[torch.nn.Module, AlibiReplacementFunction]``, where
+        `AlibiReplacementFunction` is any function that has a :data:`~.module_surgery.ReplacementFunction`
+        signature but with an additional ``max_sequence_length`` argument.
+
+        Implementation files (e.g., :file:`_gpt2.py`) populate :data:`policy_registry` (an instance of
+        this class) by defining instances of `AlibiReplacementFunction` functions and decorating them
+        with :meth:`policy_registry.register` (this method). One or more ``Type[torch.nn.Module]`` source
+        classes must be supplied as inputs to the decorator, which tells :data:`policy_registry`
+        to map those classes to the decorated function.
+
+        Example:
+
+        .. code-block::
+
+           from composer.algorithms.alibi.attention_surgery_functions.utils import policy_registry
+           from transformers.models.gpt2.modeling_gpt2 import GPT2Attention
+
+           @policy_registry.register(GPT2Attention)
+           def convert_gpt2_attention(module: torch.nn.Module, index: int, max_sequence_length: int):
+               # Do surgery (change ``module`` or generate a new ``module`` instance to return)
+               # Note that this function should depend on ``max_sequence_length``
+
+               # YOUR CODE HERE
+
+               return module
+
+        In the above example, ``convert_gpt2_attention`` (an instance of a `AlibiReplacementFunction`
+        function) is decorated with ``@policy_registry.register(GPT2Attention)``. Using the decorator
+        this way instructs the ALiBi algorithms to apply surgery to any instance of `GPT2Attention`
+        within the model using ``convert_gpt2_attention`` (the decorated function).
+
+        Note that ``convert_gpt2_attention`` follows the specific signature of an `AlibiReplacementFunction`.
+        :meth:`policy_registry.register` will raise an exception if it is used to decorate a function that
+        does not follow this signature. The requirements are:
+        * The function takes 3 input arguments
+        * Argument 1 has type ``torch.nn.Module``
+        * Argument 2 has type ``int``
+        * Argument 3 is named ``max_sequence_length`` and has type ``int``
+
+        To better understand these requirements, it may be helpful to review composer's module
+        surgery (:file:`composer/utils/module_surgery.py`) and the way ALiBi's implementation uses
+        `policy_registry` in :func:`composer.algorithms.alibi.apply_alibi`.
+        """
+        if len(modules) == 0:
+            raise ValueError('Registry decoration without any module class inputs has no effect.')
+
+        def _validate_signature(func: Callable):
+            # Necessary to enforce that `func` has a valid signature (i.e. is a AlibiReplacementFunction)
+            signature = inspect.signature(func)
+            parameters = signature.parameters
+            if len(parameters) != 3:
+                raise ValueError(
+                    f'Each alibi surgery function must accept 3 arguments, {func} accepts {len(parameters)}')
+            ((_, module_param), (_, index_param), (max_seq_name, max_seq_param)) = parameters.items()
+            if module_param.annotation != torch.nn.Module:
+                raise TypeError(
+                    f'The first argument of alibi surgery function {func} must be of type "torch.nn.Module"')
+            if index_param.annotation != int:
+                raise TypeError(f'The second argument of alibi surgery function {func} must be of type "int"')
+            if max_seq_param.annotation != int:
+                raise TypeError(f'The third argument of alibi surgery function {func} must be of type "int"')
+            if max_seq_name != 'max_sequence_length':
+                raise NameError(f'The third argument of function {func} must be named "max_sequence_length"')
+
+        def _register_module(module: Type[torch.nn.Module], func: Callable) -> None:
+            if not issubclass(module, torch.nn.Module):
+                raise TypeError(f'Module {module.__name__} is not a subclass of `torch.nn.Module`.')
+            if module in self:
+                raise ValueError(
+                    f'An AlibiReplacementFunction has already been registered for module {module.__name__}.')
+            self[module] = func
+            return
 
-        Variable input lengths can create CUDA OOM errors. To avoid this,
-        we follow the `PyTorch notes <https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html#pre-allocate-memory-in-case-of-variable-input-length>`_
-        and pre-allocate the memory with a blank forward and backward pass.
+        def wrapper(func: AlibiReplacementFunction) -> AlibiReplacementFunction:
+            _validate_signature(func)
+            for module in modules:
+                _register_module(module, func)
+            return func
 
-    Args:
-        batch (Dict[str, Tensor]): The input batch to the model, must be a dictionary.
-        curr_seq_length (int): The desired sequence length to apply.
-        truncate (bool, optional): Truncate sequences early, or reshape tensors to create
-            new examples out of the extra tokens. Default: ``True``.
+        return wrapper
 
-    Returns:
-        Dict[str, Tensor]: a Mapping of input tensors to the model,
-            where all tensors have curr_seq_len in the second dimension.
 
-    Example:
+# Initialize the policy registry that Alibi will reference
+policy_registry = PolicyRegistry()
 
-    .. code-block::
 
-        import composer.functional as cf
+def zero_and_freeze_expand_position_embeddings(
+    module: torch.nn.Module,
+    max_sequence_length: int,
+    position_embedding_attribute: str,
+) -> None:
+    """Replaces weights with zero tensor and prevents them from being learned further.
 
-        for epoch in range(num_epochs):
-            for X, y in train_loader:
-                X = cf.set_batch_sequence_length(X, sequence_length)
-                y_hat = model(X)
-                loss = loss_fn(y_hat, y)
+    This is intended to be used specifically for "removing" positional embeddings.
     """
-
-    assert isinstance(batch, Mapping)
-
-    if truncate:
-        for k in batch.keys():
-            batch[k] = batch[k][:, :curr_seq_len]
+    try:
+        pos_embedding_module = attrgetter(position_embedding_attribute)(module)
+        old_weight = getattr(pos_embedding_module, 'weight')
+        if not isinstance(old_weight, torch.nn.Parameter):
+            raise TypeError(f'Module {module._get_name()}, position embedding {position_embedding_attribute}, '
+                            f"'weight' attribute must be of type torch.nn.Module")
+        new_weight = torch.nn.Parameter(
+            torch.zeros((max_sequence_length, old_weight.shape[1]),
+                        dtype=old_weight.dtype,
+                        layout=old_weight.layout,
+                        device=old_weight.device))
+        new_weight.requires_grad = False
+        setattr(pos_embedding_module, 'weight', new_weight)
+
+        log.info(f' Position embedding expanded to sequence length {max_sequence_length}, zeroed, and frozen')
+
+    except AttributeError:
+        log.error(f'Unable to zero and freeze position embeddings. Module '
+                  f'{module} may lack attribute {position_embedding_attribute}, or position '
+                  f"embeddings may lack attribute 'weight'.")
+        raise
+
+
+def register_alibi(module: torch.nn.Module, n_heads: int, max_token_length: int, causal: bool) -> torch.nn.Module:
+    """Adds ALiBi's linear attention biases as a buffer to the module."""
+    if causal:  # e.g., for GPT
+        # Modified from https://github.com/ofirpress/attention_with_linear_biases/blob/5b327adc6d131e28b40ba58906b30bb469483519/fairseq/models/transformer.py#L742
+        slopes = torch.Tensor(_get_alibi_head_slopes(n_heads))
+        # In the next line, the part after the * is what constructs the diagonal matrix
+        # (right matrix in Figure 3 in the paper).
+        # If you run it you'll see that it doesn't exactly print out the same matrix as we
+        # have in Figure 3, but one where all rows are identical.
+        # This works because the softmax operation is invariant to translation, and our bias
+        # functions are always linear.
+        alibi = slopes.unsqueeze(1).unsqueeze(1) * \
+            torch.arange(max_token_length). \
+            unsqueeze(0).unsqueeze(0).expand(n_heads, -1, -1)
+        assert alibi.shape == torch.Size([n_heads, 1, max_token_length])
+
+    else:  # e.g., for BERT
+        # Following https://github.com/ofirpress/attention_with_linear_biases/issues/5 (Implementation 1)
+        # In the causal case, you can exploit the fact that softmax is invariant to a uniform translation
+        # of the logits, which makes the math work out *after* applying causal masking. If no causal masking
+        # will be applied, it is necessary to construct the diagonal mask.
+        context_position = torch.arange(max_token_length)[:, None]
+        memory_position = torch.arange(max_token_length)[None, :]
+        relative_position = torch.abs(memory_position - context_position)
+        # [n_heads, max_token_length, max_token_length]
+        relative_position = relative_position.unsqueeze(0).expand(n_heads, -1, -1)
+
+        slopes = torch.Tensor(_get_alibi_head_slopes(n_heads))
+        alibi = slopes.unsqueeze(1).unsqueeze(1) * -relative_position
+        # [1, n_heads, max_token_length, max_token_length]
+        alibi = alibi.unsqueeze(0)
+        assert alibi.shape == torch.Size([1, n_heads, max_token_length, max_token_length])
+
+    module_device = next(module.parameters()).device
+    module.register_buffer('alibi', alibi.to(module_device))
+    return module
+
+
+def _get_alibi_head_slopes(n_heads: int):
+
+    def get_slopes_power_of_2(n_heads):
+        start = (2**(-2**-(math.log2(n_heads) - 3)))
+        ratio = start
+        return [start * ratio**i for i in range(n_heads)]
+
+    # In the paper, they only train models that have 2^a heads for some a. This function
+    # has some good properties that only occur when the input is a power of 2. To
+    # maintain that even when the number of heads is not a power of 2, we use a
+    # workaround.
+    if math.log2(n_heads).is_integer():
+        return get_slopes_power_of_2(n_heads)
     else:
-        # ensure new tensor shape is divisible by curr_seq_len
-        input_ids = batch['input_ids'].view(-1)
-        tensor_len = (input_ids.shape[0] // curr_seq_len) * curr_seq_len
-
-        input_ids = input_ids[:tensor_len]
-        input_ids = input_ids.view(-1, curr_seq_len)
-        batch['input_ids'] = input_ids
-
-        for k, v in batch.items():
-            if k == 'input_ids':
-                continue
-            v = v.view(-1)
-            v = v[:tensor_len]
-            batch[k] = v.view(-1, curr_seq_len)
-
-    return batch
-
-
-class SeqLengthWarmup(Algorithm):
-    """Progressively increases the sequence length during training.
-
-    Changes the sequence length of all tensors in the input batch. The
-    sequence length increases from ``min_seq_length`` to ``max_seq_length``
-    in steps of ``step_size`` during the first ``duration`` fraction of
-    training.
-
-    The sequence length is then kept at ``max_seq_length``
-    for the rest of training.
-
-    Tensors are either truncated (``truncate=True``) or reshaped to
-    create new examples from the extra tokens (``truncate=False``).
-
-    This algorithm runs on :attr:`~composer.core.event.Event.AFTER_DATALOADER` to modify
-    the sequence length of a batch of data after the model and data have been moved to
-    accelerators.
-
-    .. note::
-
-        ``step_size`` should be a `multiple of eight <https://developer.nvidia.com/blog/optimizing-gpu-performance-tensor-cores/>`_ for
-        optimal throughput on NVIDIA GPUs.
-
-    .. note::
-
-        Variable input lengths can create CUDA OOM errors. To avoid this,
-        we follow the `PyTorch notes <https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html#pre-allocate-memory-in-case-of-variable-input-length>`_
-        and pre-allocate the memory with a blank forward and backward pass.
-
-    See the :doc:`Method Card </method_cards/seq_length_warmup>` for more details.
-
-    Example:
-
-    .. code-block::
-
-        from composer.algorithms import SeqLengthWarmup
-        from composer import Trainer
-
-        seq_length_warmup = SeqLengthWarmup(duration=0.5,
-                                            min_seq_length=8,
-                                            max_seq_length=1024,
-                                            ste_size=8,
-                                            truncate=False)
-
-        trainer = Trainer(model=model,
-                          train_dataloader=train_dataloader,
-                          max_duration="1ep",
-                          algorithms=[seq_length_warmup])
-
-    Args:
-        duration (float, optional): Fraction of total training for sequential length
-            learning. Default = ``0.3``.
-        min_seq_length (int, optional): Minimum sequence length to start the warmup.
-            Default = ``8``.
-        max_seq_length (int, optional): Maximum sequence length to stop the warmup.
-            Default = ``1024``.
-        step_size (int, optional): Step size of sequence length. Default = ``8``.
-        truncate (bool, optional): Truncate tensors or reshape extra tokens to new
-            examples. Default = ``True``.
-    """
-
-    def __init__(
-        self,
-        duration: float = 0.3,
-        min_seq_length: int = 8,
-        max_seq_length: int = 1024,
-        step_size: int = 8,
-        truncate: bool = True,
-    ):
-        self.duration = duration
-        self.min_seq_length = min_seq_length
-        self.max_seq_length = max_seq_length
-        self.step_size = step_size
-        self.truncate = truncate
-
-        if self.duration < 0 or self.duration > 1:
-            raise ValueError(f'Duration must be getween 0 and 1, got: {self.duration}')
-
-        if self.max_seq_length < self.min_seq_length:
-            raise ValueError(f'max_seq_length={self.max_seq_length} must be '
-                             f'greater than min_seq_length={self.min_seq_length}')
-        self._activated = False
-        self._original_model = None
-
-    def match(self, event: Event, state: State) -> bool:
-        return (event == Event.INIT and self._original_model is None) or event == Event.AFTER_DATALOADER
-
-    def apply(self, event: Event, state: State, logger: Logger) -> Optional[int]:
-        if event == Event.INIT:
-            if not isinstance(state.model, ComposerTransformer):
-                raise RuntimeError(
-                    textwrap.dedent(f"""\
-                    {type(self).__name__} requires state.model to be of type {ComposerTransformer.__name__}, not of type {type(state.model)}"""
-                                   ))
-
-            self._original_model = state.model
-            return
-
-        assert state.dataloader is not None, 'dataloader should be set on AFTER_DATALOADER'
-        assert state.max_duration is not None, 'max_duration should be set on AFTER_DATALOADER'
-
-        # in order to avoid OOMs, we do a forward and a backward pass on a dummy input.
-        if not self._activated:
-            # ensure that input_ids is a valid model input. since we don't need the
-            # results, we don't use all inputs.
-            assert self._original_model is not None, 'original model should be set on Event.INIT'
-            model_inputs = self._original_model.get_model_inputs()
-            if 'input_ids' not in model_inputs:
-                raise RuntimeError("'input_ids' must be in model inputs")
-            if 'labels' not in model_inputs:
-                raise RuntimeError("'labels' must be in model inputs")
-
-            # create fake inputs
-            assert self._original_model.config is not None, 'model of type HuggingFaceModel should have .config'
-            vocab_size = self._original_model.config.vocab_size
-
-            # simplifying assumption: Composer doesn't support model-parallelism,
-            # so the first parameter's device is likely the same device for
-            # all of the parameters
-            device = next(state.model.parameters()).device
-
-            try:
-                # Both PyTorch and FFCV dataloaders define a `batch_size` attribute
-                # This exception would mainly be raised if the user is passing in a custom
-                # iterable
-                per_gpu_macrobatch = getattr(state.dataloader, 'batch_size')
-            except AttributeError as e:
-                raise AttributeError(
-                    'Sequence Length Warmup requires the `state.dataloader` to have a `batch_size` attribute.') from e
-            if per_gpu_macrobatch is None:
-                raise RuntimeError('Sequence Length Warmup algorithm requires constant batch size.')
-            per_gpu_batch = ceil(per_gpu_macrobatch / state.grad_accum)
-
-            input_ids = torch.randint(low=0,
-                                      high=vocab_size - 1,
-                                      size=(per_gpu_batch, self.max_seq_length),
-                                      device=device).long()
-            labels = input_ids.clone()
-            attn_mask = torch.ones_like(labels)
-            model_inputs = {
-                'input_ids': input_ids,
-                'labels': labels,
-                'attention_mask': attn_mask,
-            }
-
-            # start by running a forward and backward pass
-            # of the maximum sequence length to allocate cache.
-            with get_precision_context(state.precision):
-                outputs = state.model.forward(model_inputs)
-                loss = self._original_model.loss(outputs, model_inputs)
-
-            # since use_grad_scaling is in the Trainer, and we
-            # don't care about the loss values, skip scaling
-            for loss_item in ensure_tuple(loss):
-                loss_item.backward()
-
-            for optimizer in state.optimizers:
-                optimizer.zero_grad()
-
-            self._activated = True
-
-        if state.max_duration.unit == TimeUnit.EPOCH:
-            if state.dataloader_len is None:
-                raise RuntimeError('Sequential Length Warmup requires the dataloader to be sized.')
-            num_optimization_steps = int(state.dataloader_len) * state.max_duration.value
-        elif state.max_duration.unit == TimeUnit.BATCH:
-            num_optimization_steps = state.max_duration.value
-        else:
-            raise NotImplementedError(
-                textwrap.dedent("""\
-                    To use sequential length warmup, the max_duration must be in epochs or batches.
-                    Specifying the `max_duration` in tokens or samples for use with sequential
-                    length warmup will be supported in a future Composer release. See
-                    https://github.com/mosaicml/composer/issues/226."""))
-        num_warmup_steps = int(num_optimization_steps * self.duration)  # in batches
-
-        # assume the full sequence length is the unaltered sequence length
-        num_update_steps = (self.max_seq_length - self.min_seq_length) // self.step_size
-        update_every_n_steps = num_warmup_steps // num_update_steps
-
-        curr_seq_len = self.step_size * (int(state.timestamp.batch) // update_every_n_steps)
-        curr_seq_len = max(curr_seq_len, self.min_seq_length)
-        curr_seq_len = min(curr_seq_len, self.max_seq_length)
-
-        state.batch = set_batch_sequence_length(state.batch, curr_seq_len, self.truncate)
-
-        batch_size = state.batch['input_ids'].shape[0]
-        logger.data_batch({
-            'seq_length_warmup/curr_seq_len': curr_seq_len,
-            'seq_length_warmup/curr_bs': batch_size,
-        })
+        closest_power_of_2 = 2**math.floor(math.log2(n_heads))
+        return get_slopes_power_of_2(closest_power_of_2) + _get_alibi_head_slopes(
+            2 * closest_power_of_2)[0::2][:n_heads - closest_power_of_2]
```

### Comparing `mosaicml-0.8.2/composer/algorithms/squeeze_excite/__init__.py` & `mosaicml-0.9.0/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/squeeze_excite/squeeze_excite.py` & `mosaicml-0.9.0/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         return SqueezeExciteConv2d(conv=module, latent_channels=latent_channels)
 
 
 class SqueezeExcite(Algorithm):
     """Adds Squeeze-and-Excitation blocks (`Hu et al, 2019 <https://arxiv.org/abs/1709.01507>`_) after the
     :class:`torch.nn.Conv2d` modules in a neural network.
 
-    Runs on :attr:`~composer.core.event.Event.INIT`. See :class:`SqueezeExcite2d` for more information.
+    Runs on :attr:`.Event.INIT`. See :class:`SqueezeExcite2d` for more information.
 
     Args:
         latent_channels (float, optional): Dimensionality of the hidden layer within the added
             MLP. If less than 1, interpreted as a fraction of the number of
             output channels in the :class:`torch.nn.Conv2d` immediately
             preceding each Squeeze-and-Excitation block. Default: ``64``.
         min_channels (int, optional): An SE block is added after a :class:`torch.nn.Conv2d`
```

### Comparing `mosaicml-0.8.2/composer/algorithms/stochastic_depth/__init__.py` & `mosaicml-0.9.0/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/stochastic_depth/metadata.json` & `mosaicml-0.9.0/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/stochastic_depth/stochastic_depth.py` & `mosaicml-0.9.0/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
     The algorithm replaces the specified target layer with a stochastic version
     of the layer. The stochastic layer will randomly drop either samples or the
     layer itself depending on the stochastic method specified. The block-wise
     version follows the original paper. The sample-wise version follows the
     implementation used for EfficientNet in the
     `Tensorflow/TPU repo <https://github.com/tensorflow/tpu>`_.
 
-    Runs on :attr:`~composer.core.event.Event.INIT`, as well as
-    :attr:`~composer.core.event.Event.BATCH_START` if ``drop_warmup > 0``.
+    Runs on :attr:`.Event.INIT`, as well as
+    :attr:`.Event.BATCH_START` if ``drop_warmup > 0``.
 
     .. note::
 
         Stochastic Depth only works on instances of :class:`torchvision.models.resnet.ResNet` for now.
 
     Args:
         target_layer_name (str): Block to replace with a stochastic block
```

### Comparing `mosaicml-0.8.2/composer/algorithms/stochastic_depth/stochastic_layers.py` & `mosaicml-0.9.0/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/swa/swa.py` & `mosaicml-0.9.0/composer/algorithms/swa/swa.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/utils/augmentation_common.py` & `mosaicml-0.9.0/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/utils/augmentation_primitives.py` & `mosaicml-0.9.0/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/algorithms/warnings.py` & `mosaicml-0.9.0/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/callbacks/__init__.py` & `mosaicml-0.9.0/composer/callbacks/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """Callbacks that run at each training loop :class:`.Event`.
 
 Each callback inherits from the :class:`.Callback` base class. See detailed description and
 examples for writing your own callbacks at the :class:`.Callback` base class.
 """
 from composer.callbacks.checkpoint_saver import CheckpointSaver
 from composer.callbacks.early_stopper import EarlyStopper
+from composer.callbacks.export_for_inference import ExportForInferenceCallback
 from composer.callbacks.grad_monitor import GradMonitor
 from composer.callbacks.image_visualizer import ImageVisualizer
 from composer.callbacks.lr_monitor import LRMonitor
 from composer.callbacks.memory_monitor import MemoryMonitor
 from composer.callbacks.mlperf import MLPerfCallback
 from composer.callbacks.speed_monitor import SpeedMonitor
 from composer.callbacks.threshold_stopper import ThresholdStopper
@@ -20,10 +21,11 @@
     'GradMonitor',
     'LRMonitor',
     'MemoryMonitor',
     'SpeedMonitor',
     'CheckpointSaver',
     'MLPerfCallback',
     'EarlyStopper',
+    'ExportForInferenceCallback',
     'ThresholdStopper',
     'ImageVisualizer',
 ]
```

### Comparing `mosaicml-0.8.2/composer/callbacks/callback_hparams_registry.py` & `mosaicml-0.9.0/composer/callbacks/callback_hparams_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from typing import Dict, Type, Union
 
 import yahp as hp
 
 from composer.callbacks.checkpoint_saver import CheckpointSaver
 from composer.callbacks.early_stopper import EarlyStopper
+from composer.callbacks.export_for_inference import ExportForInferenceCallback
 from composer.callbacks.grad_monitor import GradMonitor
 from composer.callbacks.image_visualizer import ImageVisualizer
 from composer.callbacks.lr_monitor import LRMonitor
 from composer.callbacks.memory_monitor import MemoryMonitor
 from composer.callbacks.mlperf import MLPerfCallback
 from composer.callbacks.speed_monitor import SpeedMonitor
 from composer.callbacks.threshold_stopper import ThresholdStopper
@@ -22,10 +23,11 @@
     'checkpoint_saver': CheckpointSaver,
     'speed_monitor': SpeedMonitor,
     'lr_monitor': LRMonitor,
     'grad_monitor': GradMonitor,
     'memory_monitor': MemoryMonitor,
     'mlperf': MLPerfCallback,
     'early_stopper': EarlyStopper,
+    'export_for_inference': ExportForInferenceCallback,
     'threshold_stopper': ThresholdStopper,
     'image_visualizer': ImageVisualizer,
 }
```

### Comparing `mosaicml-0.8.2/composer/callbacks/checkpoint_saver.py` & `mosaicml-0.9.0/composer/callbacks/checkpoint_saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing import Callable, List, Optional, Tuple, Union
 
 from composer.core import Event, State
 from composer.core.callback import Callback
 from composer.core.time import Time, Timestamp, TimeUnit
 from composer.loggers import Logger
 from composer.loggers.logger import LogLevel
-from composer.utils import checkpoint, dist
+from composer.utils import checkpoint, dist, is_model_deepspeed
 from composer.utils.file_helpers import (FORMAT_NAME_WITH_DIST_AND_TIME_TABLE, FORMAT_NAME_WITH_DIST_TABLE,
                                          create_symlink_file, ensure_folder_has_no_conflicting_files,
                                          format_name_with_dist, format_name_with_dist_and_time, is_tar)
 
 log = logging.getLogger(__name__)
 
 __all__ = ['CheckpointSaver', 'checkpoint_periodically']
@@ -125,15 +125,15 @@
 
             .. note::
 
                 When training with multiple devices (i.e. GPUs), ensure that ``'{{rank}}'`` appears in the format.
                 Otherwise, multiple processes may attempt to write to the same file.
 
         filename (str, optional): A format string describing how to name checkpoints.
-            Default: ``'ep{{epoch}}-ba{{batch}}-rank{{rank}}'``.
+            Default: ``'ep{{epoch}}-ba{{batch}}-rank{{rank}}.pt'``.
 
             Checkpoints will be saved approximately to ``{{folder}}/{{filename.format(...)}}``.
 
             The following format variables are available:
 
             {textwrap.indent(FORMAT_NAME_WITH_DIST_AND_TIME_TABLE, prefix='            ')}
 
@@ -177,23 +177,23 @@
 
         artifact_name (str, optional): Format string for the checkpoint's artifact name.
             Default: ``"{{run_name}}/checkpoints/ep{{epoch}}-ba{{batch}}-rank{{rank}}"``.
 
             After the checkpoint is saved, it will be periodically logged as a file artifact.
             The artifact name will be determined by this format string.
 
-            .. seealso:: :meth:`.Logger.log_file_artifact` for file artifact logging.
+            .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
 
             The same format variables for ``filename`` are available.
 
             Leading slashes (``'/'``) will be stripped.
 
             To disable logging trace files as file artifacts, set this parameter to ``None``.
         latest_filename (str, optional): A format string for a symlink which points to the last saved checkpoint.
-            Default: ``'latest-rank{{rank}}'``.
+            Default: ``'latest-rank{{rank}}.pt'``.
 
             Symlinks will be created approximately at ``{{folder}}/{{latest_filename.format(...)}}``.
 
             The same format variables as for ``name`` are available.
 
             To disable symlinks, set this parameter to ``None``.
 
@@ -226,15 +226,15 @@
                 ...
         latest_artifact_name (str, optional): Format string for the checkpoint's latest symlink artifact name.
             Default: ``'{{run_name}}/checkpoints/latest-rank{{rank}}"``.
 
             Whenever a new checkpoint is saved, a symlink artifact is created or updated to point to the latest checkpoint's ``artifact_name``.
             The artifact name will be determined by this format string. This parameter has no effect if ``latest_filename`` or ``artifact_name`` is ``None``.
 
-            .. seealso:: :func:`.write_symlink` for symlink artifact logging.
+            .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
 
             The same format variables for ``filename`` are available.
 
             Leading slashes (``'/'``) will be stripped.
 
             To disable symlinks in logger, set this parameter to ``None``.
 
@@ -286,17 +286,17 @@
                 Otherwise, when not using DeepSpeed, each sub-list will contain only one filepath since only rank zero
                 saves checkpoints.
     """
 
     def __init__(
         self,
         folder: str = '{run_name}/checkpoints',
-        filename: str = 'ep{epoch}-ba{batch}-rank{rank}',
+        filename: str = 'ep{epoch}-ba{batch}-rank{rank}.pt',
         artifact_name: Optional[str] = '{run_name}/checkpoints/ep{epoch}-ba{batch}-rank{rank}',
-        latest_filename: Optional[str] = 'latest-rank{rank}',
+        latest_filename: Optional[str] = 'latest-rank{rank}.pt',
         latest_artifact_name: Optional[str] = '{run_name}/checkpoints/latest-rank{rank}',
         save_interval: Union[Time, str, int, Callable[[State, Event], bool]] = '1ep',
         *,
         overwrite: bool = False,
         num_checkpoints_to_keep: int = -1,
         weights_only: bool = False,
     ):
@@ -325,15 +325,15 @@
         # Verify safety with self.overwrite. Note that this has to be done at fit_start as opposed to init since it requires state.timestamp
         # from any checkpoints which are loaded, and checkpoint loading happens after Event.INIT.
         if not self.overwrite:
             folder = format_name_with_dist(self.folder, state.run_name)
             ensure_folder_has_no_conflicting_files(folder, self.filename, state.timestamp)
         # Ensure no rank proceeds (and potentially attempts to write to the folder), until all ranks have validated that the folder is safe.
         dist.barrier()
-        if state.is_model_deepspeed:
+        if is_model_deepspeed(state.model):
             if self.weights_only:
                 NotImplementedError(
                     ('Saving checkpoints with `weights_only=True` is not currently supported when using DeepSpeed. '
                      'See https://github.com/mosaicml/composer/issues/685.'))
 
     def batch_checkpoint(self, state: State, logger: Logger):
         if self.save_interval(state, Event.BATCH_CHECKPOINT):
@@ -356,15 +356,15 @@
 
         if dist.get_global_rank() < len(checkpoint_filepaths):
             # Log the checkpoint as an artifact
             checkpoint_filepath = checkpoint_filepaths[dist.get_global_rank()]
             if self.artifact_name is not None:
                 artifact_name = format_name_with_dist_and_time(self.artifact_name, state.run_name,
                                                                state.timestamp).lstrip('/')
-                if state.is_model_deepspeed and not is_tar(artifact_name):
+                if is_model_deepspeed(state.model) and not is_tar(artifact_name):
                     # Deepspeed requires tarballs; appending `.tar`
                     artifact_name += '.tar'
                 logger.file_artifact(log_level=log_level,
                                      artifact_name=artifact_name,
                                      file_path=checkpoint_filepath,
                                      overwrite=self.overwrite)
 
@@ -374,15 +374,15 @@
                     formatted_folder_path,
                     format_name_with_dist_and_time(
                         self.latest_filename,
                         state.run_name,
                         state.timestamp,
                     ).lstrip('/'),
                 )
-                if state.is_model_deepspeed and not is_tar(symlink_name):
+                if is_model_deepspeed(state.model) and not is_tar(symlink_name):
                     # Deepspeed requires tarballs; appending `.tar`
                     symlink_name += '.tar'
                 symlink_dirname = os.path.dirname(symlink_name)
                 if symlink_dirname:
                     os.makedirs(symlink_dirname, exist_ok=True)
                 try:
                     os.remove(symlink_name)
```

### Comparing `mosaicml-0.8.2/composer/callbacks/early_stopper.py` & `mosaicml-0.9.0/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/callbacks/grad_monitor.py` & `mosaicml-0.9.0/composer/callbacks/grad_monitor.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/callbacks/image_visualizer.py` & `mosaicml-0.9.0/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/callbacks/lr_monitor.py` & `mosaicml-0.9.0/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/callbacks/memory_monitor.py` & `mosaicml-0.9.0/composer/callbacks/memory_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             ...     train_dataloader=train_dataloader,
             ...     eval_dataloader=eval_dataloader,
             ...     optimizers=optimizer,
             ...     max_duration="1ep",
             ...     callbacks=[MemoryMonitor()],
             ... )
 
-    The memory statistics are logged by the :class:`~composer.loggers.logger.Logger` to the following keys as
+    The memory statistics are logged by the :class:`.Logger` to the following keys as
     described below.
 
     +--------------------------+-------------------------------------------------------------+
     | Key                      | Logged data                                                 |
     +==========================+=============================================================+
     |                          | Several memory usage statistics                             |
     | ``memory/{statistic}``   | are logged on                                               |
```

### Comparing `mosaicml-0.8.2/composer/callbacks/mlperf.py` & `mosaicml-0.9.0/composer/callbacks/mlperf.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/callbacks/speed_monitor.py` & `mosaicml-0.9.0/composer/callbacks/speed_monitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,87 +35,71 @@
             ...     train_dataloader=train_dataloader,
             ...     eval_dataloader=eval_dataloader,
             ...     optimizers=optimizer,
             ...     max_duration='1ep',
             ...     callbacks=[SpeedMonitor(window_size=100)],
             ... )
 
-    The training throughput is logged by the :class:`~composer.loggers.logger.Logger` to the following keys as
+    The training throughput is logged by the :class:`.Logger` to the following keys as
     described below.
 
-    +-----------------------+-------------------------------------------------------------+
-    | Key                   | Logged data                                                 |
-    +=======================+=============================================================+
-    |                       | Rolling average (over ``window_size`` most recent           |
-    | ``samples/step``      | batches) of the number of samples processed per second      |
-    |                       |                                                             |
-    +-----------------------+-------------------------------------------------------------+
-    |                       | Number of samples processed per second (averaged over       |
-    | ``samples/epoch``     | an entire epoch)                                            |
-    +-----------------------+-------------------------------------------------------------+
-    | ``wall_clock/train``  | Total elapsed training time                                 |
-    +-----------------------+-------------------------------------------------------------+
-    | ``wall_clock/val``    | Total elapsed validation time                               |
-    +-----------------------+-------------------------------------------------------------+
-    | ``wall_clock/total``  | Total elapsed time (wall_clock/train + wall_clock/val)      |
-    +-----------------------+-------------------------------------------------------------+
+    +----------------------------------+-------------------------------------------------------------+
+    | Key                              | Logged data                                                 |
+    +==================================+=============================================================+
+    |                                  | Rolling average (over ``window_size`` most recent           |
+    | ``throughput/samples_per_sec``   | batches) of the number of samples processed per second      |
+    |                                  |                                                             |
+    +----------------------------------+-------------------------------------------------------------+
+    | ``wall_clock/train``             | Total elapsed training time                                 |
+    +----------------------------------+-------------------------------------------------------------+
+    | ``wall_clock/val``               | Total elapsed validation time                               |
+    +----------------------------------+-------------------------------------------------------------+
+    | ``wall_clock/total``             | Total elapsed time (wall_clock/train + wall_clock/val)      |
+    +----------------------------------+-------------------------------------------------------------+
 
     Args:
         window_size (int, optional): Number of batches to use for a rolling average of throughput.
             Defaults to 100.
     """
 
     def __init__(self, window_size: int = 100):
-        # Track the epoch num samples and wct to compute throughput over the entire epoch
-        self.epoch_start_num_samples = 0
-        self.epoch_start_wct = 0.0
-
         # Track the batch num samples and wct to compute throughput over a window of batches
         self.batch_start_num_samples = 0
         self.batch_start_wct = 0.0
         self.batch_wct_buffer: Deque[float] = deque(maxlen=window_size)
         self.batch_num_samples_buffer: Deque[int] = deque(maxlen=window_size)
         self.window_size = window_size
 
         # Keep track of time spent evaluating
         self.total_eval_wct = 0.0
 
     def state_dict(self) -> Dict[str, Any]:
         return {
-            'epoch_start_num_samples': self.epoch_start_num_samples,
-            'epoch_start_wct': self.epoch_start_wct,
             'batch_start_num_samples': self.batch_start_num_samples,
             'batch_start_wct': self.batch_start_wct,
             'batch_wct_buffer': self.batch_wct_buffer,
             'batch_num_samples_buffer': self.batch_num_samples_buffer,
             # "window_wct": self.window_wct,
             # "window_num_samples": self.window_num_samples,
             'total_eval_wct': self.total_eval_wct,
         }
 
     def load_state_dict(self, state: Dict[str, Any]) -> None:
-        self.epoch_start_num_samples = state['epoch_start_num_samples']
-        self.epoch_start_wct = state['epoch_start_wct']
         self.batch_start_num_samples = state['batch_start_num_samples']
         self.batch_start_wct = state['batch_start_wct']
         self.batch_wct_buffer = deque(
             [x for x in state['batch_wct_buffer']],
             maxlen=self.window_size,
         )
         self.batch_num_samples_buffer = deque(
             [x for x in state['batch_num_samples_buffer']],
             maxlen=self.window_size,
         )
         self.total_eval_wct = state['total_eval_wct']
 
-    def epoch_start(self, state: State, logger: Logger):
-        del logger  # unused
-        self.epoch_start_wct = state.timestamp.total_wct.total_seconds()
-        self.epoch_start_num_samples = int(state.timestamp.sample)
-
     def batch_start(self, state: State, logger: Logger) -> None:
         del logger  # unused
         self.batch_start_wct = state.timestamp.total_wct.total_seconds()
         self.batch_start_num_samples = int(state.timestamp.sample)
 
     def batch_end(self, state: State, logger: Logger):
         batch_num_samples = int(state.timestamp.sample) - self.batch_start_num_samples
@@ -124,29 +108,20 @@
         # Add the new element
         self.batch_wct_buffer.append(batch_wct)
         self.batch_num_samples_buffer.append(batch_num_samples)
 
         # Log the throughput
         if len(self.batch_num_samples_buffer) == self.window_size:
             throughput = sum(self.batch_num_samples_buffer) / sum(self.batch_wct_buffer)
-            logger.data_batch({'samples/step': throughput})
+            logger.data_batch({'throughput/samples_per_sec': throughput})
 
         # Log the time
         # `state.timestamp` excludes any time spent in evaluation
         logger.data_batch({
             'wall_clock/train': state.timestamp.total_wct.total_seconds(),
             'wall_clock/val': self.total_eval_wct,
             'wall_clock/total': (state.timestamp.total_wct.total_seconds() + self.total_eval_wct),
         })
 
     def eval_end(self, state: State, logger: Logger):
         del logger  # unused
         self.total_eval_wct += state.eval_timestamp.total_wct.total_seconds()
-
-    def epoch_end(self, state: State, logger: Logger):
-        # `state.timestamp` excludes any time spent in evaluation
-        epoch_time_in_train = state.timestamp.total_wct.total_seconds() - self.epoch_start_wct
-        train_examples_per_epoch = int(state.timestamp.sample) - self.epoch_start_num_samples
-
-        logger.data_epoch({
-            'samples/epoch': train_examples_per_epoch / epoch_time_in_train,
-        })
```

### Comparing `mosaicml-0.8.2/composer/callbacks/threshold_stopper.py` & `mosaicml-0.9.0/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/cli/launcher.py` & `mosaicml-0.9.0/composer/cli/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 """The Composer CLI launcher for distributed training."""
 
 import contextlib
 import datetime
 import logging
 import os
 import signal
-import socket
 import subprocess
 import sys
 import tempfile
 import time
 import traceback
 import warnings
 from argparse import ArgumentParser
 from typing import Any, Dict, List
 
 import psutil
 import torch
 
 import composer
+from composer.utils.misc import get_free_tcp_port
 
 CLEANUP_TIMEOUT = datetime.timedelta(seconds=30)
 
 log = logging.getLogger(__name__)
 
 
 def _get_parser():
     parser = ArgumentParser(description='Utility for launching distributed machine learning jobs.')
 
-    parser.add_argument('--version', action='version', version=f'composer {composer.__version__}')
+    parser.add_argument('--version', action='version', version=f'MosaicML Composer {composer.__version__}')
 
     required_args = parser.add_argument_group('required arguments')
 
     parser.add_argument(
         '-n',
         '--nproc',
         type=int,
@@ -128,23 +128,14 @@
     required_args.add_argument('training_script_args',
                                nargs='...',
                                help='Any arguments for the training script, given in the expected order.')
 
     return parser
 
 
-def _get_free_tcp_port() -> int:
-    # from https://www.programcreek.com/python/?CodeExample=get+free+port
-    tcp = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    tcp.bind(('', 0))
-    _, port = tcp.getsockname()
-    tcp.close()
-    return port
-
-
 def _parse_args():
     parser = _get_parser()
 
     args = parser.parse_args()
 
     # Default values to env vars if they are not provided
     if args.nproc is None:
@@ -228,15 +219,15 @@
         if args.master_addr is None:
             args.master_addr = '127.0.0.1'
 
         if args.master_port is None:
             warnings.warn('AutoSelectPortWarning: The distributed key-value port was auto-selected. '
                           'This may lead to race conditions when launching multiple training processes simultaneously. '
                           'To eliminate this race condition, explicitly specify a port with --master_port PORT_NUMBER')
-            args.master_port = _get_free_tcp_port()
+            args.master_port = get_free_tcp_port()
 
     return args
 
 
 @contextlib.contextmanager
 def _patch_env(**environs: str):
     """Returns a context manager that patches ``os.environ`` with ``environs``.
```

### Comparing `mosaicml-0.8.2/composer/core/__init__.py` & `mosaicml-0.9.0/composer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/core/algorithm.py` & `mosaicml-0.9.0/composer/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/core/callback.py` & `mosaicml-0.9.0/composer/core/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
         Args:
             state (State): The training state.
             logger (Logger): The logger.
         """
         del state, logger  # unused
         pass
 
-    def batch_start(self, state: State, logger: Logger) -> None:
-        """Called on the :attr:`.Event.BATCH_START` event.
+    def before_dataloader(self, state: State, logger: Logger) -> None:
+        """Called on the :attr:`.Event.BEFORE_DATALOADER` event.
 
         Args:
             state (State): The training state.
             logger (Logger): The logger.
         """
         del state, logger  # unused
         pass
@@ -140,14 +140,24 @@
 
         Args:
             state (State): The training state.
             logger (Logger): The logger.
         """
         del state, logger  # unused
         pass
+
+    def batch_start(self, state: State, logger: Logger) -> None:
+        """Called on the :attr:`.Event.BATCH_START` event.
+
+        Args:
+            state (State): The training state.
+            logger (Logger): The logger.
+        """
+        del state, logger  # unused
+        pass
 
     def before_train_batch(self, state: State, logger: Logger) -> None:
         """Called on the :attr:`.Event.BEFORE_TRAIN_BATCH` event.
 
         Args:
             state (State): The training state.
             logger (Logger): The logger.
```

### Comparing `mosaicml-0.8.2/composer/core/data_spec.py` & `mosaicml-0.9.0/composer/core/data_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,19 @@
         if isinstance(batch, torch.Tensor):
             return batch.shape[0]
 
         dim0_sizes = []
         if isinstance(batch, (list, tuple)):
             for tensors in batch:
                 for t in ensure_tuple(tensors):
+                    if not hasattr(t, 'shape'):
+                        raise ValueError('Unable to determine the batch size, batch contains'
+                                         f'an element of type {type(t)}, which does not have a'
+                                         'shape. Please use a DataSpec and provide a'
+                                         '`get_num_samples_in_batch(your_batch) -> int` method.')
                     dim0_sizes.append(t.shape[0])
         elif isinstance(batch, dict):
             dim0_sizes = [t.shape[0] for t in batch.values()]
 
         if len(set(dim0_sizes)) == 1:
             return dim0_sizes[0]
         else:
```

### Comparing `mosaicml-0.8.2/composer/core/engine.py` & `mosaicml-0.9.0/composer/core/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,42 @@
 
 .. currentmodule:: composer
 
 The order in which algorithms are run matters significantly during composition. For example, the
 :class:`.SelectiveBackprop` algorithm runs on the :attr:`.Event.AFTER_DATALOADER` event and must run before
 any data augmentations. :class:`.Engine` runs re-ordering passes to resolve such ordering issues or conflicts.
 
-.. note::
+These orderings are enforced by algorithm passes. The default passes registered to the Engine are found in
+:mod:`composer.core.passes`. To register a new pass, use :meth:`.Engine.register_pass`, e.g.
 
-    * An instance of :class:`.Engine` is automatically constructed by the :class:`.Trainer`
-      constructor. A user need not instantiate the :class:`.Engine` class.
 
-    * The design of :class:`.Engine` is subject to change in future releases
-      to accommodate more complexity as we investigate composition of algorithms.
+.. testsetup::
 
+    # dummy algorithm
+    MyAlgorithm = None
 
-Currently, the following passes are registered:
+.. doctest::
 
-* **LIFO order for events**
+    from composer import Engine, Algorithm, Event
+    from typing import Sequence
 
-  For the events that follow the ``before_*`` (e.g., :attr:`.Event.BEFORE_LOSS`) and ``after_*`` (e.g.,
-  :attr:`.Event.AFTER_LOSS`) pattern, the ordering of algorithms is reversed for the ``after_*`` events. For example,
-  four given algorithms ``A``, ``B``, ``C``, and ``D`` will run in ``ABCD`` ordering on the ``before_*`` event while
-  ``DCBA`` ordering on the ``after_*`` event.
+    def run_last(algorithms: Sequence[Algorithm], event: Event) -> Sequence[Algorithm]:
+        algorithms = sorted(algorithms, key=lambda x: isinstance(x, MyAlgorithm))
 
-  This allows algorithms to "clean up" their changes. For example, :class:`.LabelSmoothing` will smooth the labels
-  upon the :attr:`.Event.BEFORE_LOSS` event and then restore the original unsmoothed labels on the
-  :attr:`.Event.AFTER_LOSS` event.
+    Engine.register_pass(run_last)
 
-* **Run Selective Backprop first**
+.. note::
+
+    * An instance of :class:`.Engine` is automatically constructed by the :class:`.Trainer`
+      constructor. A user need not instantiate the :class:`.Engine` class.
+
+.. note::
+    * The design of :class:`.Engine` is subject to change in future releases
+      to accommodate more complexity as we investigate composition of algorithms.
 
-  :class:`.SelectiveBackprop` runs after the dataloader returns the batch and executes an extra forward pass to rank
-  and prune the examples in the batch by loss. To ensure a clean estimate of loss, :class:`.SelectiveBackprop` should
-  run before any other data augmentations (e.g., :class:`.MixUp`) on the :attr:`.Event.AFTER_DATALOADER` event.
 
 Trace
 ~~~~~
 
 Traces record whether an algorithm ran at a particular step and event combination and also the order of such executions.
 These are logged with the key ``<algorithm_name>/<event>``.
 
@@ -63,56 +64,37 @@
 
 import atexit
 import contextlib
 import logging
 import weakref
 from collections import OrderedDict
 from dataclasses import dataclass
-from typing import ContextManager, Dict, Optional, Sequence, Union, cast
+from typing import ContextManager, Dict, List, Optional, Sequence, TypeVar, Union, cast
 
+from composer.core import passes
 from composer.core.algorithm import Algorithm
 from composer.core.callback import Callback
 from composer.core.event import Event
 from composer.core.state import State
 from composer.loggers import Logger, LogLevel
 from composer.profiler import ProfilerAction
 
 log = logging.getLogger(__name__)
 
 __all__ = ['Trace', 'Engine', 'Traces']
 
+T = TypeVar('T')
+
+_ALWAYS_RECORD_EVENTS = [Event.INIT, Event.FIT_START, Event.EPOCH_START, Event.EPOCH_END]
+
 #: The default traces of an entire run is an OrderedDict.
 #: The keys are of format ``<algorithm_name>/<event>`` (e.g.,  ``Blurpool/INIT``) and values are an instance of
 #: :class:`Trace`.
 Traces = Dict[str, 'Trace']
 
-_ALWAYS_RECORD_EVENTS = [Event.INIT, Event.FIT_START, Event.EPOCH_START, Event.EPOCH_END]
-_EVENTS_WHERE_DATALOADER_IS_SET = [e for e in Event if e != Event.INIT]
-_EVENTS_WHERE_MAX_DURATION_IS_SET = [
-    Event.FIT_START,
-    Event.EPOCH_START,
-    Event.BATCH_START,
-    Event.AFTER_DATALOADER,
-    Event.BEFORE_TRAIN_BATCH,
-    Event.BEFORE_FORWARD,
-    Event.AFTER_FORWARD,
-    Event.BEFORE_LOSS,
-    Event.AFTER_LOSS,
-    Event.BEFORE_BACKWARD,
-    Event.AFTER_BACKWARD,
-    Event.AFTER_TRAIN_BATCH,
-    Event.BATCH_END,
-    Event.BATCH_CHECKPOINT,
-    Event.EPOCH_END,
-    Event.EPOCH_CHECKPOINT,
-    Event.FIT_END,
-]
-_EVAL_EVENTS = [e for e in Event if e.name.startswith('EVAL_')]
-_PREDICT_EVENTS = [e for e in Event if e.name.startswith('PREDICT_')]
-
 # Track whether atexit triggered _close(), which indicates whether the python process is shutting down
 # If so, do not run close() again via __del__(), as Python machinery (e.g. the ability to do conditional
 # imports) are destroyed between close() and __del__().
 # Using a global variable instead of an instance variable as _close() is not bound to the instance
 _did_atexit_run = False
 
 
@@ -122,14 +104,23 @@
 
 
 # Since atexit calls hooks in LIFO order, this hook will always be invoked after all atexit-triggered
 # _close() calls are invoked
 atexit.register(_set_atexit_ran)
 
 
+def _get_default_passes():
+    return [
+        passes.sort_selective_backprop_first,
+        passes.sort_fused_layernorm_last,
+        passes.set_filo_order,
+        passes.warn_if_multiple_loss_interpolation,
+    ]
+
+
 @dataclass
 class Trace():
     """Record of an algorithm's execution.
 
     Attributes:
         name (str): The name of the algorithm.
         event (Event): The current event.
@@ -168,14 +159,17 @@
             specific metrics.
     """
 
     def __init__(self, state: State, logger: Logger):
         self.logger = logger
         self.state = state
         self._is_closed = False
+
+        self.algorithm_passes: List[passes.AlgorithmPass] = _get_default_passes()
+
         atexit.register(self._close, state, logger)
 
     def run_event(
         self,
         event: Union[Event, str],
     ) -> Traces:
         """Runs the sequence of algorithms and callbacks (see :class:`.Callback`).
@@ -218,29 +212,25 @@
         if self._is_closed:
             raise RuntimeError(('The engine was already closed and therefore cannot be used again. '
                                 'To fix, please create a new Engine (or Trainer)'))
 
         if self.state.profiler is not None:
             name = f'event/{event.canonical_name}'
             if (event.is_before_event or event.is_after_event):
-                # if not part of an event pair (e.g. init or after dataloader), then don't record an event here
+                # if not part of an event pair (e.g. init), then don't record an event here
                 if event in _ALWAYS_RECORD_EVENTS:
                     actions = [ProfilerAction.ACTIVE, ProfilerAction.WARMUP, ProfilerAction.SKIP]
                 else:
                     actions = [ProfilerAction.ACTIVE, ProfilerAction.WARMUP]
                 duration_marker = self.state.profiler.marker(name, actions=actions)
 
         if event.is_after_event and duration_marker is not None:
             duration_marker.finish()
 
-        if event in _EVENTS_WHERE_DATALOADER_IS_SET:
-            assert self.state.dataloader is not None, f'The trainer should have set state.dataloader for event {event}.'
-
-        if event in _EVENTS_WHERE_MAX_DURATION_IS_SET:
-            assert self.state.max_duration is not None, f'The trainer should have set state.max_duration for event {event}.'
+        self._assert_dataloader_and_duration_set(self.state, event)
 
         if event == Event.INIT:
             # For the INIT event, run the callbacks first to initialize the loggers
             # For other events, run the algorithms first, so the callbacks have the state
             # after algorithms modify it
             self._run_callbacks(event)
             traces = self._run_algorithms(event)
@@ -249,21 +239,81 @@
             self._run_callbacks(event)
 
         if event.is_before_event and duration_marker is not None:
             duration_marker.start()
 
         return traces
 
+    def run_marker_only_event(
+        self,
+        event: Union[Event, str],
+    ) -> None:
+        """Runs the marker for an event if the profiler is enabled.
+
+        This is primarily used to complete the dataloader marker at the end of the dataloader. In
+        this scenario, the dataloader marker has started from Event.BEFORE_DATALOADER, but
+        Event.AFTER_DATALOADER cannot be called as no batch was yielded from the dataloader.
+
+        Args:
+            event (Event | str): The current :class:`.Event`. It can be the enum member values or a
+                string with the event value.
+        """
+        duration_marker = None
+        event = Event(event)
+
+        if self._is_closed:
+            raise RuntimeError(('The engine was already closed and therefore cannot be used again. '
+                                'To fix, please create a new Engine (or Trainer)'))
+
+        if self.state.profiler is not None:
+            name = f'event/{event.canonical_name}'
+            if (event.is_before_event or event.is_after_event):
+                # if not part of an event pair (e.g. init), then don't record an event here
+                if event in _ALWAYS_RECORD_EVENTS:
+                    actions = [ProfilerAction.ACTIVE, ProfilerAction.WARMUP, ProfilerAction.SKIP]
+                else:
+                    actions = [ProfilerAction.ACTIVE, ProfilerAction.WARMUP]
+                duration_marker = self.state.profiler.marker(name, actions=actions)
+
+        if event.is_after_event and duration_marker is not None:
+            duration_marker.finish()
+        if event.is_before_event and duration_marker is not None:
+            duration_marker.start()
+
+    def register_pass(self, algorithm_pass: passes.AlgorithmPass, index: int = -1):
+        """Registers an algorithm pass with the Engine.
+
+        Args:
+            algorithm_pass (passes.AlgorithmPass): A method that maps a list of
+                algorithms to a list of algorithms.
+            index (int, optional): The index to insert into the list of passes.
+                If -1 (default), the pass will be insert to the end of the list.
+        """
+        if index == -1:
+            index = len(self.algorithm_passes)
+
+        self.algorithm_passes.insert(index, algorithm_pass)
+
+    @staticmethod
+    def _assert_dataloader_and_duration_set(state: State, event: Event):
+        # correctness checks that dataloader and max duration need to be set for certain events
+
+        if event != Event.INIT:  # datalaoder should be set on all events expect INIT
+            assert state.dataloader is not None, f'The trainer should have set state.dataloader for event {event}.'
+
+        if event != Event.INIT and not event.is_predict and not event.is_eval:
+            assert state.max_duration is not None, f'The trainer should have set state.max_duration for event {event}.'
+
     def _run_algorithms(
         self,
         event: Event,
     ) -> Traces:
         algorithms_to_run = [algo for algo in self.state.algorithms if algo.match(event, self.state)]
 
-        # future collision resolution
+        # apply algorithm passes
         algorithms_to_run = self._compile(algorithms_to_run, event)
 
         trace = _setup_trace(algorithms_to_run, event)
         for order, algorithm in enumerate(algorithms_to_run):
             marker = None
             if self.state.profiler is not None:
                 marker = self.state.profiler.marker(f'algorithm/{algorithm.__class__.__name__}/event/{event.value}',
@@ -316,29 +366,19 @@
         Args:
             algorithms_to_run(Sequence[Algorithm]): Sequence of algorithms.
             event (Event): The current event.
 
         Returns:
             Sequence[Algorithm]: Modified sequence of algorithms.
         """
-        from composer.algorithms import SelectiveBackprop, StochasticDepth
-
-        # Move selective backprop to the beginning while maintaining order of other algorithms
-        algorithms = sorted(algorithms_to_run,
-                            key=lambda x: not isinstance(x, SelectiveBackprop) and not isinstance(x, StochasticDepth))
-
-        if event.is_after_event:
-            """Establish a FILO queue of algorithms ``before_`` and ``after_`` an event.
-
-            before_loss: A, B, C, D
-            after_loss: D, C, B, A
-            """
-            algorithms = list(reversed(algorithms))
+        # run reordering passes on the algorithms
+        for passes in self.algorithm_passes:
+            algorithms_to_run = passes(algorithms_to_run, event)
 
-        return algorithms
+        return algorithms_to_run
 
     def _run_callbacks(
         self,
         event: Union[Event, str],
     ):
         """Runs a sequence of callbacks by calling the function for an event.
 
@@ -378,40 +418,25 @@
         if _did_atexit_run or self._is_closed:
             # Do not attempt to shutdown again, since close() already ran via __atexit__ or was already invoked
             return
         self.close()
 
     def _debug_log(self, event: Event, msg: str):
         """Helper to include timestamp and event info in log messages."""
-        if event in _EVAL_EVENTS:
-            log.debug(
-                '[ep=%i][ba=%i][eval_ba=%i][event=%s]: %s',
-                int(self.state.timestamp.epoch),
-                int(self.state.timestamp.batch),
-                int(self.state.eval_timestamp.batch),
-                event.name,
-                msg,
-            )
-        elif event in _PREDICT_EVENTS:
-            log.debug(
-                '[ep=%i][ba=%i][predict_ba=%i][event=%s]: %s',
-                int(self.state.timestamp.epoch),
-                int(self.state.timestamp.batch),
-                int(self.state.predict_timestamp.batch),
-                event.name,
-                msg,
-            )
-        else:
-            log.debug(
-                '[ep=%i][ba=%i][event=%s]: %s',
-                int(self.state.timestamp.epoch),
-                int(self.state.timestamp.batch),
-                event.name,
-                msg,
-            )
+        timestamp = f'[ep={int(self.state.timestamp.epoch)}][ba={int(self.state.timestamp.batch)}]'
+
+        # for eval or pr
+        if event.is_eval:
+            timestamp += f'[eval_ba={int(self.state.eval_timestamp.batch)}]'
+        if event.is_predict:
+            timestamp += f'[predict_ba={int(self.state.predict_timestamp.batch)}]'
+
+        timestamp += f'[event={event.name}]'
+
+        log.debug(f'{timestamp}: {msg}')
 
     def close(self) -> None:
         """Shutdown the engine.
 
         As part of the shutdown procedure, :meth:`.Callback.close` and :meth:`.Callback.post_close` are invoked
         for each callback. Note that :meth:`.Callback.post_close` is invoked only for callbacks that did not raise
         an exception during :meth:`.Callback.close`.
```

### Comparing `mosaicml-0.8.2/composer/core/evaluator.py` & `mosaicml-0.9.0/composer/core/evaluator.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/core/event.py` & `mosaicml-0.9.0/composer/core/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 
     .. code-block:: python
 
         # <INIT>
         # <FIT_START>
         for epoch in range(NUM_EPOCHS):
             # <EPOCH_START>
-            for batch in dataloader:
+            while True:
+                # <BEFORE_DATALOADER>
+                batch = next(dataloader)
+                if batch is None:
+                    break
                 # <AFTER_DATALOADER>
 
                 # <BATCH_START>
 
                 # <BEFORE_TRAIN_BATCH>
 
                 for microbatch in batch.split(grad_accum):
@@ -81,14 +85,15 @@
 
     Attributes:
         INIT: Invoked in the constructor of :class:`~.trainer.Trainer`. Model surgery (see
             :mod:`~composer.utils.module_surgery`) typically occurs here.
         FIT_START: Invoked at the beginning of each call to :meth:`.Trainer.fit`. Dataset transformations typically
             occur here.
         EPOCH_START: Start of an epoch.
+        BEFORE_DATALOADER: Immediately before the dataloader is called.
         AFTER_DATALOADER: Immediately after the dataloader is called.  Typically used for on-GPU dataloader transforms.
         BATCH_START: Start of a batch.
         BEFORE_TRAIN_BATCH: Before the forward-loss-backward computation for a training batch. When using gradient
             accumulation, this is still called only once.
         BEFORE_FORWARD: Before the call to ``model.forward()``.
             This is called multiple times per batch when using gradient accumulation.
         AFTER_FORWARD: After the call to ``model.forward()``.
@@ -124,14 +129,15 @@
     """
 
     INIT = 'init'
     FIT_START = 'fit_start'
 
     EPOCH_START = 'epoch_start'
 
+    BEFORE_DATALOADER = 'before_dataloader'
     AFTER_DATALOADER = 'after_dataloader'
 
     BATCH_START = 'batch_start'
 
     BEFORE_TRAIN_BATCH = 'before_train_batch'
 
     BEFORE_FORWARD = 'before_forward'
@@ -203,15 +209,25 @@
         name: str = self.value
         name = name.replace('before_', '')
         name = name.replace('after_', '')
         name = name.replace('_start', '')
         name = name.replace('_end', '')
         return name
 
+    @property
+    def is_predict(self) -> bool:
+        """Whether the event is during the predict loop."""
+        return self.value.startswith('predict')
+
+    @property
+    def is_eval(self) -> bool:
+        """Whether the event is during the eval loop."""
+        return self.value.startswith('eval')
+
 
-_BEFORE_EVENTS = (Event.FIT_START, Event.EPOCH_START, Event.BATCH_START, Event.BEFORE_TRAIN_BATCH, Event.BEFORE_FORWARD,
-                  Event.BEFORE_LOSS, Event.BEFORE_BACKWARD, Event.EVAL_START, Event.EVAL_BATCH_START,
-                  Event.EVAL_BEFORE_FORWARD, Event.PREDICT_START, Event.PREDICT_BATCH_START,
-                  Event.PREDICT_BEFORE_FORWARD)
-_AFTER_EVENTS = (Event.EPOCH_END, Event.BATCH_END, Event.AFTER_TRAIN_BATCH, Event.AFTER_FORWARD, Event.AFTER_LOSS,
-                 Event.AFTER_BACKWARD, Event.EVAL_END, Event.EVAL_BATCH_END, Event.EVAL_AFTER_FORWARD, Event.FIT_END,
-                 Event.PREDICT_END, Event.PREDICT_BATCH_END, Event.PREDICT_AFTER_FORWARD)
+_BEFORE_EVENTS = (Event.FIT_START, Event.EPOCH_START, Event.BEFORE_DATALOADER, Event.BATCH_START,
+                  Event.BEFORE_TRAIN_BATCH, Event.BEFORE_FORWARD, Event.BEFORE_LOSS, Event.BEFORE_BACKWARD,
+                  Event.EVAL_START, Event.EVAL_BATCH_START, Event.EVAL_BEFORE_FORWARD, Event.PREDICT_START,
+                  Event.PREDICT_BATCH_START, Event.PREDICT_BEFORE_FORWARD)
+_AFTER_EVENTS = (Event.EPOCH_END, Event.BATCH_END, Event.AFTER_DATALOADER, Event.AFTER_TRAIN_BATCH, Event.AFTER_FORWARD,
+                 Event.AFTER_LOSS, Event.AFTER_BACKWARD, Event.EVAL_END, Event.EVAL_BATCH_END, Event.EVAL_AFTER_FORWARD,
+                 Event.FIT_END, Event.PREDICT_END, Event.PREDICT_BATCH_END, Event.PREDICT_AFTER_FORWARD)
```

### Comparing `mosaicml-0.8.2/composer/core/precision.py` & `mosaicml-0.9.0/composer/core/precision.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """Enum class for the numerical precision to be used by the model."""
 
 import contextlib
 from typing import Generator, Union
 
 import torch
-from packaging import version
 
 from composer.utils.string_enum import StringEnum
 
 __all__ = ['Precision', 'get_precision_context']
 
 
 class Precision(StringEnum):
@@ -19,16 +18,15 @@
 
     Attributes:
         AMP: Use :mod:`torch.cuda.amp`. Only compatible with GPUs.
         FP16: Use 16-bit floating-point precision. Currently only
             compatible with GPUs on DeepSpeed.
         FP32: Use 32-bit floating-point precision.
             Compatible with CPUs and GPUs.
-        BF16: Use 16-bit BFloat mixed precision. Requires PyTorch
-            1.10. Compatible with CPUs and GPUs.
+        BF16: Use 16-bit BFloat mixed precision. Compatible with CPUs and GPUs.
     """
     AMP = 'amp'
     FP16 = 'fp16'
     FP32 = 'fp32'
     BF16 = 'bf16'
 
 
@@ -59,13 +57,16 @@
         # only when using DeepSpeed.
         yield
     elif precision == Precision.AMP:
         # Retain compatibility with PyTorch < 1.10
         with torch.cuda.amp.autocast(True):
             yield
     elif precision == Precision.BF16:
-        if version.parse(torch.__version__) < version.parse('1.10'):
-            raise ValueError(f'BF16 precision requires torch > 1.10, got version {torch.__version__}')
-        with torch.cuda.amp.autocast(enabled=True, dtype=torch.bfloat16):  # type: ignore (torch < 1.10 guard)
+        if torch.cuda.is_available():
+            with torch.cuda.amp.autocast(enabled=True, dtype=torch.bfloat16):
+                yield
+        else:
+            import os
+            os.environ['XLA_USE_BF16'] = '1'
             yield
     else:
         raise ValueError(f'Unsupported precision: {precision}')
```

### Comparing `mosaicml-0.8.2/composer/core/serializable.py` & `mosaicml-0.9.0/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/core/state.py` & `mosaicml-0.9.0/composer/core/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 import collections.abc
 import logging
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Sequence, Union, cast
 
 import torch
+import torch.nn
 import torch.nn.modules.utils
 from torch.nn.parallel import DistributedDataParallel
 from torch.optim import Optimizer
 
 from composer.core.precision import Precision
 from composer.core.serializable import Serializable
 from composer.core.time import Time, Timestamp, TimeUnit
-from composer.utils import batch_get, batch_set, dist, ensure_tuple
+from composer.utils import batch_get, batch_set, dist, ensure_tuple, is_model_deepspeed
 
 if TYPE_CHECKING:
     import deepspeed
 
     import composer.core.types as types
     from composer.core.algorithm import Algorithm
     from composer.core.callback import Callback
@@ -116,15 +117,15 @@
             ...     ...,
             ...     compute_training_metrics=True,
             ...     train_dataloader=train_dataloader,
             ...     eval_dataloader=eval_dataloader,
             ... )
             >>> trainer.fit()
             >>> trainer.state.current_metrics
-            {'train': {'Accuracy': tensor(...)}, 'eval': {'Accuracy': tensor(...)}}
+            {'train': {'Accuracy': tensor(...)}, 'eval': {'CrossEntropy': tensor(...), 'Accuracy': tensor(...)}}
 
             Or, when using an :class:`.Evaluator`:
 
             .. testsetup::
 
                 eval_1_dl = eval_dataloader
                 eval_2_dl = eval_dataloader
@@ -601,27 +602,17 @@
         return self._precision
 
     @precision.setter
     def precision(self, precision: Union[str, Precision]):
         self._precision = Precision(precision)
 
     @property
-    def is_model_deepspeed(self) -> bool:
-        """Whether :attr:`model` is an instance of a :class:`~deepspeed.DeepSpeedEngine`."""
-        try:
-            import deepspeed
-        except ImportError:
-            return False
-        else:
-            return isinstance(self.model, deepspeed.DeepSpeedEngine)
-
-    @property
     def is_model_ddp(self):
         """Whether :attr:`model` is an instance of a :class:`.DistributedDataParallel`."""
         return isinstance(self.model, DistributedDataParallel)
 
     @property
     def deepspeed_model(self) -> deepspeed.DeepSpeedEngine:
         """Cast :attr:`model` to :class:`~deepspeed.DeepSpeedEngine`."""
-        if self.is_model_deepspeed:
+        if is_model_deepspeed(self.model):
             return cast('deepspeed.DeepSpeedEngine', self.model)
         raise TypeError('state.model is not a DeepSpeed model')
```

### Comparing `mosaicml-0.8.2/composer/core/time.py` & `mosaicml-0.9.0/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/core/types.py` & `mosaicml-0.9.0/composer/core/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,32 +17,36 @@
 from typing import Any, Dict, List, Union
 
 import torch
 import torch.utils.data
 
 from composer.utils.string_enum import StringEnum
 
-__all__ = ['Batch', 'PyTorchScheduler', 'JSON', 'MemoryFormat', 'BreakEpochException']
+__all__ = ['Batch', 'PyTorchScheduler', 'JSON', 'MemoryFormat']
 
 Batch = Any
 
 Dataset = torch.utils.data.Dataset[Batch]
 
 PyTorchScheduler = torch.optim.lr_scheduler._LRScheduler
 
 JSON = Union[str, float, int, None, List['JSON'], Dict[str, 'JSON']]
 
 
-class BreakEpochException(Exception):
-    """Raising this exception will immediately end the current epoch.
+class TrainerMode(StringEnum):
+    """Enum to represent which mode the Trainer is in.
 
-    If you're wondering whether you should use this, the answer is no.
+    Attributes:
+        TRAIN: In training mode.
+        EVAL: In evaluation mode.
+        PREDICT: In predict mode.
     """
-
-    pass
+    TRAIN = 'train'
+    EVAL = 'eval'
+    PREDICT = 'predict'
 
 
 class MemoryFormat(StringEnum):
     """Enum class to represent different memory formats.
 
     See :class:`torch.torch.memory_format` for more details.
```

### Comparing `mosaicml-0.8.2/composer/datasets/__init__.py` & `mosaicml-0.9.0/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/ade20k.py` & `mosaicml-0.9.0/composer/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/ade20k_hparams.py` & `mosaicml-0.9.0/composer/datasets/ade20k_hparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
         if self.min_resize_scale <= 0:
             raise ValueError('min_resize_scale cannot be zero or negative')
 
         if self.max_resize_scale < self.min_resize_scale:
             raise ValueError('max_resize_scale cannot be less than min_resize_scale')
 
+        if self.final_size is not None and self.final_size <= 0:
+            raise ValueError('self.final_size cannot be zero or negative.')
+
     def initialize_object(self, batch_size, dataloader_hparams) -> DataSpec:
         self.validate()
 
         if self.use_synthetic:
             if self.split == 'train':
                 total_dataset_size = 20_206
             elif self.split == 'val':
```

### Comparing `mosaicml-0.8.2/composer/datasets/brats.py` & `mosaicml-0.9.0/composer/datasets/brats.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/brats_hparams.py` & `mosaicml-0.9.0/composer/datasets/brats_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/c4.py` & `mosaicml-0.9.0/composer/datasets/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/c4_hparams.py` & `mosaicml-0.9.0/composer/datasets/c4_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/cifar.py` & `mosaicml-0.9.0/composer/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/cifar_hparams.py` & `mosaicml-0.9.0/composer/datasets/cifar_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/coco.py` & `mosaicml-0.9.0/composer/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/coco_hparams.py` & `mosaicml-0.9.0/composer/datasets/coco_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/dataset_hparams.py` & `mosaicml-0.9.0/composer/datasets/dataset_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/dataset_hparams_registry.py` & `mosaicml-0.9.0/composer/datasets/dataset_hparams_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/evaluator_hparams.py` & `mosaicml-0.9.0/composer/datasets/evaluator_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/ffcv_utils.py` & `mosaicml-0.9.0/composer/datasets/ffcv_utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/glue_hparams.py` & `mosaicml-0.9.0/composer/datasets/glue_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/imagenet.py` & `mosaicml-0.9.0/composer/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/imagenet_hparams.py` & `mosaicml-0.9.0/composer/datasets/imagenet_hparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,30 +166,30 @@
             )
 
         else:
 
             if self.is_train:
                 # include fixed-size resize before RandomResizedCrop in training only
                 # if requested (by specifying a size > 0)
-                train_resize_size = self.resize_size
                 train_transforms: List[torch.nn.Module] = []
-                if train_resize_size > 0:
-                    train_transforms.append(transforms.Resize(train_resize_size))
+                if self.resize_size > 0:
+                    train_transforms.append(transforms.Resize(self.resize_size))
                 # always include RandomResizedCrop and RandomHorizontalFlip
                 train_transforms += [
                     transforms.RandomResizedCrop(self.crop_size, scale=(0.08, 1.0), ratio=(0.75, 4.0 / 3.0)),
                     transforms.RandomHorizontalFlip()
                 ]
                 transformation = transforms.Compose(train_transforms)
                 split = 'train'
             else:
-                transformation = transforms.Compose([
-                    transforms.Resize(self.resize_size),
-                    transforms.CenterCrop(self.crop_size),
-                ])
+                val_transforms: List[torch.nn.Module] = []
+                if self.resize_size > 0:
+                    val_transforms.append(transforms.Resize(self.resize_size))
+                val_transforms.append(transforms.CenterCrop(self.crop_size))
+                transformation = transforms.Compose(val_transforms)
                 split = 'val'
 
             device_transform_fn = NormalizationFn(mean=IMAGENET_CHANNEL_MEAN, std=IMAGENET_CHANNEL_STD)
             collate_fn = pil_image_collate
 
             if self.datadir is None:
                 raise ValueError('datadir must be specified if self.synthetic is False')
```

### Comparing `mosaicml-0.8.2/composer/datasets/lm_dataset_hparams.py` & `mosaicml-0.9.0/composer/datasets/lm_dataset_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/mnist_hparams.py` & `mosaicml-0.9.0/composer/datasets/mnist_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/streaming/__init__.py` & `mosaicml-0.9.0/composer/datasets/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/streaming/dataset.py` & `mosaicml-0.9.0/composer/datasets/streaming/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,27 @@
 from time import sleep
 from typing import Any, Callable, Dict, Iterator, Optional
 
 import numpy as np
 from torch.utils.data import IterableDataset
 
 from composer.datasets.streaming.download import download_or_wait
-from composer.datasets.streaming.format import (StreamingDatasetIndex, bytes_to_sample_dict, get_index_basename,
-                                                get_shard_basename)
+from composer.datasets.streaming.format import (StreamingDatasetIndex, bytes_to_sample_dict,
+                                                get_compression_scheme_basename, get_index_basename, get_shard_basename,
+                                                split_compression_suffix)
 from composer.datasets.streaming.world import get_world
 from composer.utils import dist
 
 __all__ = ['StreamingDataset']
 
 
+class DatasetCompressionException(Exception):
+    pass
+
+
 class _DownloadStatus(enum.IntEnum):
     NOT_STARTED = 1
     IN_PROGRESS = 2
     DONE = 3
     FAILED = 4
 
 
@@ -129,46 +134,66 @@
         self.local = local
         self.shuffle = shuffle
         self.decoders = decoders
         self.max_retries = max_retries
         self.timeout = timeout
         self.batch_size = batch_size
 
+        self.compression_scheme = None
+        if remote is not None:
+            try:
+                compression_local = self._download_file(get_compression_scheme_basename(),
+                                                        wait=(dist.get_local_rank() != 0),
+                                                        local_basename=get_compression_scheme_basename() + '.old')
+                with open(compression_local, 'r') as fp:
+                    compression_scheme = fp.read().rstrip()
+                    self.compression_scheme = compression_scheme if compression_scheme != '' else None
+                    if remote == local and self.compression_scheme is not None:
+                        raise DatasetCompressionException('cannot decompress when remote == local')
+
+            except FileNotFoundError:
+                compression_local = os.path.join(self.local, get_compression_scheme_basename() + '.old')
+                with open(compression_local, 'x') as fp:
+                    fp.write('')
+                pass
+
         # Load the index file containing the shard metadata
         # This file contains the shard and offset in bytes of each sample (for direct access).
         # Only local device 0 on each node downloads the index. All other devices wait.
-        index_basename = get_index_basename()
+        index_basename = get_index_basename(self.compression_scheme)
         index_local = self._download_file(index_basename, wait=(dist.get_local_rank() != 0))
         with open(index_local, 'rb') as fp:
             self.index = StreamingDatasetIndex.load(fp)
 
         # Fields, protected by the lock, relating to loading shards in the background.
         self._lock: Lock
         self._next_epoch = 0
         self._epoch_to_todo_ids = {}
         self._downloaded_ids = []
         self._download_status = _DownloadStatus.NOT_STARTED
         self._download_exception: Exception
 
-    def _download_file(self, basename: str, wait: bool = False) -> str:
+    def _download_file(self, basename: str, wait: bool = False, local_basename: Optional[str] = None) -> str:
         """Safely download a file from remote to local cache.
 
         Args:
             basename (str): Basename of file to download.
             wait (bool): Whether to wait for another worker to download the file.
 
         Returns:
             str: Local cache filename.
         """
+        local_basename = local_basename if local_basename is not None else basename
         if self.remote is None:
             remote = self.remote
         else:
             remote = os.path.join(self.remote, basename)
-        local = os.path.join(self.local, basename)
+        local = os.path.join(self.local, local_basename)
         download_or_wait(remote=remote, local=local, wait=wait, max_retries=self.max_retries, timeout=self.timeout)
+        local, _ = split_compression_suffix(local)
         return local
 
     def _insert_shard_samples(self, shard: int, part_min_id: int, part_max_id: int) -> None:
         """Load the given locally cached shard into the dataset.
 
         Every time you call __iter__ on this dataset, it registers the list of samples you have left, which will not be
         the full epoch if the dataset isn't finished loaded when you start training.
@@ -231,15 +256,15 @@
             part_shards = np.array(part_shards)
             np.random.shuffle(part_shards[1:])
 
         for shard in part_shards:
             # If this worker is in charge of downloading the shard, download it.
             # Otherwise, wait until shard gets downloaded by another worker on this node
             # This produces deterministic sample order.
-            basename = get_shard_basename(shard)
+            basename = get_shard_basename(shard, compression_name=self.compression_scheme)
             try:
                 self._download_file(basename, wait=(shard not in part_shards_to_download))
             except Exception as e:
                 self._download_status = _DownloadStatus.FAILED
                 self._download_exception = e
             self._insert_shard_samples(shard, part_min_id, part_max_id)
```

### Comparing `mosaicml-0.8.2/composer/datasets/streaming/download.py` & `mosaicml-0.9.0/composer/datasets/streaming/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,72 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Download handling for :class:`StreamingDataset`.
 """
 
+import gzip
 import os
 import shutil
 import time
 import urllib.parse
 from typing import Optional
 
-from composer.utils import MissingConditionalImportError, get_file
+from composer.datasets.streaming.format import split_compression_suffix
+from composer.utils import get_file
+from composer.utils.object_store.object_store import ObjectStore
+from composer.utils.object_store.s3_object_store import S3ObjectStore
+from composer.utils.object_store.sftp_object_store import SFTPObjectStore
 
-__all__ = ['download_or_wait']
+__all__ = ['download_or_wait', 'get_object_store']
 
 
 def download_from_http(remote: str, local: str) -> None:
     """Download a file from a http/https remote to local."""
     get_file(path=remote, destination=local, overwrite=True)
 
 
-def download_from_s3(remote: str, local: str, timeout: float) -> None:
-    """Download a file from remote to local.
+def get_object_store(remote: str) -> ObjectStore:
+    """Use the correct download handler to download the file
 
     Args:
-        remote (str): Remote path (S3).
-        local (str): Local path (local filesystem).
-        timeout (float): How long to wait for shard to download before raising an exception.
+        remote (Optional[str]): Remote path (local filesystem).
+        timeout (float): How long to wait for file to download before raising an exception.
     """
-    try:
-        import boto3
-        from botocore.config import Config
-    except ImportError as e:
-        raise MissingConditionalImportError(extra_deps_group='streaming', conda_package='boto3') from e
+    if remote.startswith('s3://'):
+        return _get_s3_object_store(remote)
+    elif remote.startswith('sftp://'):
+        return _get_sftp_object_store(remote)
+    else:
+        raise ValueError('unsupported upload scheme')
+
 
+def _get_s3_object_store(remote: str) -> S3ObjectStore:
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 's3':
         raise ValueError(f"Expected obj.scheme to be 's3', got {obj.scheme} for remote={remote}")
+    bucket = obj.netloc
+    object_store = S3ObjectStore(bucket=bucket)
+    return object_store
 
-    config = Config(read_timeout=timeout)
-    s3 = boto3.client('s3', config=config)
-    s3.download_file(obj.netloc, obj.path.lstrip('/'), local)
-
-
-def download_from_sftp(remote: str, local: str) -> None:
-    """Download a file from remote SFTP server to local filepath.
-
-    Authentication must be provided via username/password in the ``remote`` URI, or a valid SSH config, or a default key
-    discoverable in ``~/.ssh/``.
-
-    Args:
-        remote (str): Remote path (SFTP).
-        local (str): Local path (local filesystem).
-    """
-    try:
-        from paramiko import SSHClient
-    except ImportError as e:
-        raise MissingConditionalImportError(extra_deps_group='streaming', conda_package='paramiko') from e
-
-    # Parse URL
-    url = urllib.parse.urlsplit(remote)
-    if url.scheme.lower() != 'sftp':
-        raise ValueError('If specifying a URI, only the sftp scheme is supported.')
-    if not url.hostname:
-        raise ValueError('If specifying a URI, the URI must include the hostname.')
-    if url.query or url.fragment:
-        raise ValueError('Query and fragment parameters are not supported as part of a URI.')
-    hostname = url.hostname
-    port = url.port
-    username = url.username
-    password = url.password
-    remote_path = url.path
 
+def _get_sftp_object_store(remote: str) -> SFTPObjectStore:
     # Get SSH key file if specified
     key_filename = os.environ.get('COMPOSER_SFTP_KEY_FILE', None)
     known_hosts_filename = os.environ.get('COMPOSER_SFTP_KNOWN_HOSTS_FILE', None)
 
-    # Default port
-    port = port if port else 22
+    object_store = SFTPObjectStore(
+        host=remote,
+        known_hosts_filename=known_hosts_filename,
+        key_filename=key_filename,
+    )
+    return object_store
 
-    # Local tmp
-    local_tmp = local + '.tmp'
-    if os.path.exists(local_tmp):
-        os.remove(local_tmp)
 
-    with SSHClient() as ssh_client:
-        # Connect SSH Client
-        ssh_client.load_system_host_keys(known_hosts_filename)
-        ssh_client.connect(
-            hostname=hostname,
-            port=port,
-            username=username,
-            password=password,
-            key_filename=key_filename,
-        )
-
-        # SFTP Client
-        sftp_client = ssh_client.open_sftp()
-        sftp_client.get(remotepath=remote_path, localpath=local_tmp)
-    os.rename(local_tmp, local)
+__all__ = ['download_or_wait']
 
 
 def download_from_local(remote: str, local: str) -> None:
     """Download a file from remote to local.
 
     Args:
         remote (str): Remote path (local filesystem).
@@ -111,39 +75,53 @@
     local_tmp = local + '.tmp'
     if os.path.exists(local_tmp):
         os.remove(local_tmp)
     shutil.copy(remote, local_tmp)
     os.rename(local_tmp, local)
 
 
-def dispatch_download(remote: Optional[str], local: str, timeout: float):
+def dispatch_download(remote: Optional[str], local: str):
     """Use the correct download handler to download the file
 
     Args:
         remote (Optional[str]): Remote path (local filesystem).
         local (str): Local path (local filesystem).
         timeout (float): How long to wait for file to download before raising an exception.
     """
-    if os.path.exists(local):
+
+    local_decompressed, compression_scheme = split_compression_suffix(local)
+    if os.path.exists(local_decompressed):
         return
 
     local_dir = os.path.dirname(local)
     os.makedirs(local_dir, exist_ok=True)
 
     if not remote:
         raise ValueError('In the absence of local dataset, path to remote dataset must be provided')
-    elif remote.startswith('http://') or remote.startswith('https://'):
+    elif remote.startswith('s3://') or remote.startswith('sftp://'):
+        url = urllib.parse.urlsplit(remote)
+        remote_path = url.path.strip('/')
+        object_store = get_object_store(remote)
+        object_store.download_object(remote_path, local)
+    elif remote.startswith('http://'):
         download_from_http(remote, local)
-    elif remote.startswith('s3://'):
-        download_from_s3(remote, local, timeout)
-    elif remote.startswith('sftp://'):
-        download_from_sftp(remote, local)
     else:
         download_from_local(remote, local)
 
+    if compression_scheme is not None:
+        tempfile = local_decompressed + '.tmp'
+        if compression_scheme == 'gz':
+            with gzip.open(local, 'rb') as gzipfile:
+                with open(tempfile, 'xb') as dest_file:
+                    shutil.copyfileobj(gzipfile, dest_file)
+        else:
+            raise NotImplementedError
+        os.rename(tempfile, local_decompressed)
+        os.remove(local)
+
 
 def download_or_wait(remote: Optional[str],
                      local: str,
                      wait: bool = False,
                      max_retries: int = 2,
                      timeout: float = 60) -> None:
     """Downloads a file from remote to local, or waits for it to be downloaded.
@@ -154,26 +132,29 @@
         remote (Optional[str]): Remote path (S3, SFTP, or local filesystem).
         local (str): Local path (local filesystem).
         wait (bool, default False): If ``true``, then do not actively download the file, but instead wait (up to
             ``timeout`` seconds) for the file to arrive.
         max_retries (int, default 2): Number of download re-attempts before giving up.
         timeout (float, default 60): How long to wait for file to download before raising an exception.
     """
+    local_decompressed, _ = split_compression_suffix(local)
     last_error = None
     error_msgs = []
     for _ in range(1 + max_retries):
         try:
             if wait:
                 start = time.time()
-                while not os.path.exists(local):
+                while not os.path.exists(local_decompressed):
                     if time.time() - start > timeout:
                         raise TimeoutError(f'Waited longer than {timeout}s for other worker to download {local}.')
                     time.sleep(0.25)
             else:
-                dispatch_download(remote, local, timeout=timeout)
+                dispatch_download(remote, local)
             break
+        except FileNotFoundError:
+            raise  # bubble up file not found error
         except Exception as e:  # Retry for all causes of failure.
             error_msgs.append(e)
             last_error = e
             continue
     if len(error_msgs) > max_retries:
         raise RuntimeError(f'Failed to download {remote} -> {local}. Got errors:\n{error_msgs}') from last_error
```

### Comparing `mosaicml-0.8.2/composer/datasets/streaming/format.py` & `mosaicml-0.9.0/composer/datasets/streaming/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """The :class:`StreamingDatsetIndex` format that defines shard/sample metadata for :class:`StreamingDataset`."""
 
 import math
+from gzip import GzipFile
 from io import BufferedIOBase, BufferedReader, BufferedWriter, BytesIO
+from os.path import splitext
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from composer.datasets.streaming.world import World
 
@@ -17,33 +19,65 @@
     'get_shard_basename',
     'sample_dict_to_bytes',
     'bytes_to_sample_dict',
     'StreamingDatasetIndex',
 ]
 
 
-def get_index_basename() -> str:
+def split_compression_suffix(local_path: str) -> Tuple[str, Optional[str]]:
+    """Splits the compression suffix from a path
+
+    Args:
+        local_path (str): path to a (potentially) compressed file
+
+    Returns:
+        Tuple[str, str]: tuple containing decompressed filename and compression suffix, if one exists
+    """
+    decompressed_path, ext = splitext(local_path)
+    if ext in ['.mds', '.txt', '.old']:
+        return local_path, None
+
+    return decompressed_path, ext[1:]
+
+
+def get_compression_scheme_basename() -> str:
     """Get the basename for a streaming dataset index.
 
     Returns:
         str: Basename of file.
     """
-    return 'index.mds'
+    return 'compression.txt'
+
+
+def get_index_basename(compression_name: Optional[str] = None) -> str:
+    """Get the basename for a streaming dataset index.
+
+    Args:
+        compression_name (Optional[str]): compression extension of index file
+
+    Returns:
+        str: Basename of file.
+    """
+    compression_name = '.' + compression_name if compression_name is not None else ''
+    return f'index.mds{compression_name}'
 
 
-def get_shard_basename(shard: int) -> str:
+def get_shard_basename(shard: int, compression_name: Optional[str] = None) -> str:
     """Get the basename for a streaming dataset shard.
 
     Args:
         shard (int): Shard index.
+        compression_name (Optional[str]): compression extension of shard file
 
     Returns:
         str: Basename of file.
+        compression_name (Optional[str]): the compression scheme
     """
-    return f'{shard:06}.mds'
+    compression_name = '.' + compression_name if compression_name is not None else ''
+    return f'{shard:06}.mds{compression_name}'
 
 
 def sample_dict_to_bytes(obj: Dict[str, bytes], keys: List[str]) -> bytes:
     """Dump a sample dict to bytes, given field names.
 
     Args:
         obj (Dict[str, bytes]): The sample dict to encode.
@@ -79,15 +113,15 @@
     values = []
     for begin, end in zip(begins, ends):
         value = data[begin:end]
         values.append(value)
     return dict(zip(keys, values))
 
 
-def read_array(fp: BufferedIOBase, count: int, dtype: type) -> np.ndarray:
+def read_array(fp: Union[BufferedIOBase, GzipFile], count: int, dtype: type) -> np.ndarray:
     """Load the count items from the file handle, advancing its position.
 
     Args:
         fp (BufferedIOBase): File handle.
         count (int): Number of items to read.
         dtype (type): Item datatype.
 
@@ -145,15 +179,15 @@
         Returns:
             cls: The loaded object.
         """
         fp = BytesIO(data)
         return cls.load(fp)
 
     @classmethod
-    def load(cls, fp: Union[BufferedReader, BytesIO]):
+    def load(cls, fp: Union[BufferedReader, BytesIO, GzipFile]):
         """Load a StreamingDatasetIndex from a file handle.
 
         Args:
             fp (file): The file to read.
 
         Returns:
             cls: The loaded object.
@@ -220,15 +254,15 @@
         bytes_per_field = np.array([len(field.encode('utf-8')) for field in self.fields], np.int32)
         arrays = (header, totals, self.samples_per_shard, self.bytes_per_shard, bps_format, bps, num_fields,
                   bytes_per_field)
         array_bytes = b''.join([arr.tobytes() for arr in arrays])
         field_bytes = b''.join([field.encode('utf-8') for field in self.fields])
         return array_bytes + field_bytes
 
-    def dump(self, fp: BufferedWriter) -> None:
+    def dump(self, fp: Union[BufferedWriter, GzipFile]) -> None:
         """Dump a StreamingDatasetIndex to the file.
 
         Args:
             fp (file): The file to write.
         """
         data = self.dumps()
         fp.write(data)
```

### Comparing `mosaicml-0.8.2/composer/datasets/streaming/world.py` & `mosaicml-0.9.0/composer/datasets/streaming/world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/synthetic.py` & `mosaicml-0.9.0/composer/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/synthetic_hparams.py` & `mosaicml-0.9.0/composer/datasets/synthetic_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/synthetic_lm.py` & `mosaicml-0.9.0/composer/datasets/synthetic_lm.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/datasets/utils.py` & `mosaicml-0.9.0/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/functional/__init__.py` & `mosaicml-0.9.0/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/loggers/__init__.py` & `mosaicml-0.9.0/composer/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/loggers/file_logger.py` & `mosaicml-0.9.0/composer/loggers/file_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             Default: `'{{run_name}}/logs-rank{{rank}}.txt'`
 
         artifact_name (str, optional): Format string for the logfile's artifact name.
 
             The logfile will be periodically logged (according to the ``flush_interval``) as a file artifact.
             The artifact name will be determined by this format string.
 
-            .. seealso:: :meth:`~composer.loggers.logger.Logger.log_file_artifact` for file artifact logging.
+            .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
 
             The same format variables for ``filename`` are available. Setting this parameter to ``None``
             (the default) will use the same format string as ``filename``. It is sometimes helpful to deviate
             from this default. For example, when ``filename`` contains an absolute path, it is recommended to
             set this parameter explicitely, so the absolute path does not appear in any artifact stores.
 
             Leading slashes (``'/'``) will be stripped.
@@ -246,15 +246,15 @@
             self._flush_file(logger)
 
     def write(self, prefix: str, s: str):
         """Write to the logfile.
 
         .. note::
 
-            If the ``write`` occurs before the :attr:`~composer.core.event.Event.INIT` event,
+            If the ``write`` occurs before the :attr:`.Event.INIT` event,
             the write will be enqueued, as the file is not yet open.
 
         Args:
             prefix (str): A prefix for each line in the logfile.
             s (str): The string to write. Each line will be prefixed with ``prefix``.
         """
         formatted_lines = []
```

### Comparing `mosaicml-0.8.2/composer/loggers/in_memory_logger.py` & `mosaicml-0.9.0/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/loggers/logger.py` & `mosaicml-0.9.0/composer/loggers/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             return LogLevel[value.upper()]
         return super()._missing_(value)
 
 
 class Logger:
     """An interface to record training data.
 
-    The :class:`~composer.trainer.trainer.Trainer`, instances of :class:`~composer.core.callback.Callback`, and
+    The :class:`.Trainer`, instances of :class:`.Callback`, and
     instances of :class:`~composer.core.algorithm.Algorithm` invoke the logger to record data such as
     the epoch, training loss, and custom metrics as provided by individual callbacks and algorithms.
     This class does not store any data itself; instead, it routes all data to the ``destinations``.
     Each destination (e.g. the :class:`~composer.loggers.file_logger.FileLogger`,
     :class:`~composer.loggers.in_memory_logger.InMemoryLogger`) is responsible for storing the data itself
     (e.g. writing it to a file or storing it in memory).
 
@@ -101,14 +101,16 @@
         overwrite: bool = False,
     ):
         """Log ``file_path`` as an artifact named ``artifact_name``.
 
         Both ``file_path`` and ``artifact_name`` can be specified as format strings.
         See :func:`~.composer.utils.file_helpers.format_name_with_dist` for more information.
 
+        .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
+
         Args:
             log_level (str | int | LogLevel): The log level, which can be a name, value, or instance of
                 :class:`LogLevel`.
             artifact_name (str): A format string for the name of the artifact.
             file_path (str | pathlib.Path): A format string for the file path.
             overwrite (bool, optional): Whether to overwrite an existing artifact with the same ``artifact_name``.
                 (default: ``False``)
@@ -133,14 +135,27 @@
         """Helper function for ``self.data(LogLevel.EPOCH, data)``."""
         self.data(LogLevel.EPOCH, data)
 
     def data_batch(self, data: Dict[str, Any]) -> None:
         """Helper function for ``self.data(LogLevel.BATCH, data)``."""
         self.data(LogLevel.BATCH, data)
 
+    def has_file_artifact_destination(self) -> bool:
+        """Determines if the logger has a destination which supports logging file artifacts.
+
+            Needed for checking if a model can be exported via this logger.
+
+        Returns:
+            bool: Whether any of the destinations has supports file artifacts.
+        """
+        for destination in self.destinations:
+            if destination.can_log_file_artifacts():
+                return True
+        return False
+
 
 def format_log_data_value(data: Any) -> str:
     """Recursively formats a given log data value into a string.
 
     Args:
         data: Data to format.
```

### Comparing `mosaicml-0.8.2/composer/loggers/logger_destination.py` & `mosaicml-0.9.0/composer/loggers/logger_destination.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 __all__ = ['LoggerDestination']
 
 
 class LoggerDestination(Callback, ABC):
     """Base class for logger destination.
 
     As this class extends :class:`~.callback.Callback`, logger destinations can run on any training loop
-    :class:`~composer.core.event.Event`. For example, it may be helpful to run on
-    :attr:`~composer.core.event.Event.EPOCH_END` to perform any flushing at the end of every epoch.
+    :class:`.Event`. For example, it may be helpful to run on
+    :attr:`.Event.EPOCH_END` to perform any flushing at the end of every epoch.
 
     Example:
         .. doctest::
 
             >>> from composer.loggers import LoggerDestination
             >>> class MyLogger(LoggerDestination):
             ...     def log_data(self, state, log_level, data):
@@ -47,15 +47,15 @@
         .. note::
 
             This method will block the training loop. For optimal performance, it is recommended to deepcopy the
             ``data`` (e.g. ``copy.deepcopy(data)``), and store the copied data in queue. Then, either:
 
             *   Use background thread(s) or process(s) to read from this queue to perform any I/O.
             *   Batch the data together and flush periodically on events, such as
-                :attr:`~composer.core.event.Event.BATCH_END` or :attr:`~composer.core.event.Event.EPOCH_END`.
+                :attr:`.Event.BATCH_END` or :attr:`.Event.EPOCH_END`.
 
                 .. seealso:: :class:`~composer.loggers.file_logger.FileLogger` as an example.
 
         Args:
             state (State): The training state.
             log_level (LogLevel): The log level.
             data (Dict[str, Any]): The data to log.
@@ -72,28 +72,30 @@
         *,
         overwrite: bool,
     ):
         """Handle logging of a file artifact stored at ``file_path`` to an artifact named ``artifact_name``.
 
         Subclasses should implement this method to store logged files (e.g. copy it to another folder or upload it to
         an object store), then it should implement this method. However, not all loggers need to implement this method.
-        For example, the :class:`~composer.loggers.tqdm_logger.TQDMLogger` does not implement this method, as it cannot
+        For example, the :class:`.TQDMLogger` does not implement this method, as it cannot
         handle file artifacts.
 
         .. note::
 
             *   This method will block the training loop. For optimal performance, it is recommended that this
                 method copy the file to a temporary directory, enqueue the copied file for processing, and return.
                 Then, use a background thread(s) or process(s) to read from this queue to perform any I/O.
             *   After this method returns, training can resume, and the contents of ``file_path`` may change (or be may
                 deleted). Thus, if processing the file in the background (as is recommended), it is necessary to first
                 copy the file to a temporary directory. Otherwise, the original file may no longer exist, or the logged
                 artifact can be corrupted (e.g., if the logger destination is reading from file while the training loop
                 is writing to it).
 
+        .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
+
         Args:
             state (State): The training state.
             log_level (Union[str, LogLevel]): A :class:`LogLevel`.
             artifact_name (str): The name of the artifact.
             file_path (pathlib.Path): The file path.
             overwrite (bool, optional): Whether to overwrite an existing artifact with the same ``artifact_name``.
                 (default: ``False``)
@@ -115,7 +117,17 @@
             destination (str): The destination filepath.
             overwrite (bool): Whether to overwrite an existing file at ``destination``. Defaults to ``False``.
             progress_bar (bool, optional): Whether to show a progress bar. Ignored if ``path`` is a local file.
                 (default: ``True``)
         """
         del artifact_name, destination, overwrite, progress_bar  # unused
         raise NotImplementedError
+
+    def can_log_file_artifacts(self) -> bool:
+        """Indicates whether LoggerDestination can log file artifacts.
+
+        Defaults to false, should return True for derived logger classes that implement log_file_artifact().
+
+        Returns:
+            bool: Whether the class supports logging file artifacts.
+        """
+        return False
```

### Comparing `mosaicml-0.8.2/composer/loggers/logger_hparams_registry.py` & `mosaicml-0.9.0/composer/loggers/logger_hparams_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     """Hyperparameters for the :class:`~.ObjectStoreLogger`.
 
     Args:
         object_store_hparams (ObjectStoreHparams): The object store provider hparams.
         should_log_artifact (str, optional): The path to a filter function which returns whether an artifact should be
             logged. The path should be of the format ``path.to.module:filter_function_name``.
 
-            The function should take (:class:`~composer.core.state.State`, :class:`.LogLevel`, ``<artifact name>``).
+            The function should take (:class:`~composer.core.State`, :class:`.LogLevel`, ``<artifact name>``).
             The artifact name will be a string. The function should return a boolean indicating whether the artifact
             should be logged.
 
             .. seealso: :func:`composer.utils.import_helpers.import_object`
 
             Setting this parameter to ``None`` (the default) will log all artifacts.
-        object_name (str, optional): See :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`.
-        num_concurrent_uploads (int, optional): See :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`.
-        upload_staging_folder (str, optional): See :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`.
-        use_procs (bool, optional): See :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`.
+        object_name (str, optional): See :class:`.ObjectStoreLogger`.
+        num_concurrent_uploads (int, optional): See :class:`.ObjectStoreLogger`.
+        upload_staging_folder (str, optional): See :class:`.ObjectStoreLogger`.
+        use_procs (bool, optional): See :class:`.ObjectStoreLogger`.
     """
 
     hparams_registry = {
         'object_store_hparams': object_store_registry,
     }
 
     object_store_hparams: ObjectStoreHparams = hp.required('Object store provider hparams.')
```

### Comparing `mosaicml-0.8.2/composer/loggers/object_store_logger.py` & `mosaicml-0.9.0/composer/loggers/object_store_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pathlib
 import queue
 import shutil
 import tempfile
 import threading
 import time
 import uuid
+import warnings
 from multiprocessing.context import SpawnProcess
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 from composer.core.state import State
 from composer.loggers.logger import Logger, LogLevel
 from composer.loggers.logger_destination import LoggerDestination
 from composer.utils import ObjectStore, ObjectStoreTransientError, dist, format_name_with_dist, get_file, retry
@@ -38,15 +39,15 @@
     # error: Expected no arguments to "ObjectStore" constructor
     return object_store_cls(**object_store_kwargs)  # type: ignore
 
 
 class ObjectStoreLogger(LoggerDestination):
     r"""Logger destination that uploads artifacts to an object store.
 
-    This logger destination handles calls to :meth:`~composer.loggers.logger.Logger.file_artifact`
+    This logger destination handles calls to :meth:`.Logger.file_artifact`
     and uploads files to :class:`.ObjectStore`, such as AWS S3 or Google Cloud Storage. To minimize the training
     loop performance hit, it supports background uploads.
 
     .. testcode:: composer.loggers.object_store_logger.ObjectStoreLogger.__init__
 
         from composer.loggers import ObjectStoreLogger
         from composer.utils import LibcloudObjectStore
@@ -221,62 +222,65 @@
         self._logged_objects: Dict[str, Tuple[str, bool]] = {}
 
         # Set of enqueued objects. This should keep track of everything in self._file_upload_queue with O(1) lookup
         self._enqueued_objects: Set[str] = set()
 
         # Thread that runs `self._enqueue_uploads`
         self._enqueue_thread = None
+        # Event to signal the enqueue thread to shut down.
+        self._enqueue_thread_flag = None
 
         if use_procs:
             mp_ctx = multiprocessing.get_context('spawn')
             self._file_upload_queue: Union[queue.Queue[Tuple[str, str, bool]],
                                            multiprocessing.JoinableQueue[Tuple[str, str,
                                                                                bool]],] = mp_ctx.JoinableQueue()
             self._completed_queue: Union[queue.Queue[str], multiprocessing.JoinableQueue[str],] = mp_ctx.JoinableQueue()
             self._finished_cls: Union[Callable[[], multiprocessing._EventType], Type[threading.Event]] = mp_ctx.Event
             self._proc_class = mp_ctx.Process
         else:
             self._file_upload_queue = queue.Queue()
             self._completed_queue = queue.Queue()
             self._finished_cls = threading.Event
             self._proc_class = threading.Thread
-        self._finished: Optional[Union[multiprocessing._EventType, threading.Event]] = None
+        self._worker_flag: Optional[Union[multiprocessing._EventType, threading.Event]] = None
         self._workers: List[Union[SpawnProcess, threading.Thread]] = []
         # the object store instance for the main thread. Deferring the construction of the object_store to first use.
         self._object_store = None
 
     @property
     def object_store(self) -> ObjectStore:
         """The :class:`.ObjectStore` instance for the main thread."""
         if self._object_store is None:
             self._object_store = _build_object_store(self.object_store_cls, self.object_store_kwargs)
         return self._object_store
 
     def init(self, state: State, logger: Logger) -> None:
         del logger  # unused
-        if self._finished is not None:
+        if self._worker_flag is not None:
             raise RuntimeError('The ObjectStoreLogger is already initialized.')
-        self._finished = self._finished_cls()
+        self._worker_flag = self._finished_cls()
         self._run_name = state.run_name
         object_name_to_test = self._object_name('.credentials_validated_successfully')
 
         # Create the enqueue thread
+        self._enqueue_thread_flag = self._finished_cls()
         self._enqueue_thread = threading.Thread(target=self._enqueue_uploads, daemon=True)
         self._enqueue_thread.start()
 
         if dist.get_global_rank() == 0:
             retry(ObjectStoreTransientError,
                   self.num_attempts)(lambda: _validate_credentials(self.object_store, object_name_to_test))()
-        assert len(self._workers) == 0, 'workers should be empty if self._finished was None'
+        assert len(self._workers) == 0, 'workers should be empty if self._worker_flag was None'
         for _ in range(self._num_concurrent_uploads):
             worker = self._proc_class(
                 target=_upload_worker,
                 kwargs={
                     'file_queue': self._file_upload_queue,
-                    'is_finished': self._finished,
+                    'is_finished': self._worker_flag,
                     'object_store_cls': self.object_store_cls,
                     'object_store_kwargs': self.object_store_kwargs,
                     'num_attempts': self.num_attempts,
                     'completed_queue': self._completed_queue,
                 },
                 # The worker threads are joined in the shutdown procedure, so it is OK to set the daemon status
                 # Setting daemon status prevents the process from hanging if close was never called (e.g. in doctests)
@@ -322,23 +326,27 @@
         shutil.copy2(file_path, copied_path)
         object_name = self._object_name(artifact_name)
         with self._object_lock:
             if object_name in self._logged_objects and not overwrite:
                 raise FileExistsError(f'Object {object_name} was already enqueued to be uploaded, but overwrite=False.')
             self._logged_objects[object_name] = (copied_path, overwrite)
 
+    def can_log_file_artifacts(self) -> bool:
+        """Whether the logger supports logging file artifacts."""
+        return True
+
     def _enqueue_uploads(self):
         """Worker thread to enqueue uploads.
 
         This thread does two things:
 
         1.  It enqueues objects from ``self._logged_objects`` onto ``self._file_upload_queue``.
         2.  It keeps ``self._enqueued_objects`` in sync with ``self._file_upload_queue`` by listening to ``self._completed_uploads``.
         """
-        assert self._finished is not None
+        assert self._enqueue_thread_flag is not None
         while True:
             with self._object_lock:
                 # Remove all objects from self._enqueued_objects that have been successfully uploaded
                 while True:
                     try:
                         object_name = self._completed_queue.get_nowait()
                     except queue.Empty:
@@ -353,16 +361,17 @@
                         continue
                     self._file_upload_queue.put_nowait((copied_path, object_name, overwrite))
                     objects_to_delete.append(object_name)
                     self._enqueued_objects.add(object_name)
                 for object_name in objects_to_delete:
                     del self._logged_objects[object_name]
 
-                #
-                if self._finished.is_set():
+                # Shutdown if the enqueue thread flag is set, which means that no more objects will be added to
+                # self._logged_objects
+                if self._enqueue_thread_flag.is_set():
                     if self._all_workers_alive:
                         if len(self._logged_objects) == 0:
                             # If finished (i.e. no more objects to be added to self._logged_objects) and all logged objects are
                             # enqueued, then break
                             break
                     else:
                         # If any worker died, then it's impossible to recover since the file was already popped off of the queue,
@@ -382,47 +391,64 @@
         get_file(path=artifact_name,
                  destination=destination,
                  object_store=self.object_store,
                  overwrite=overwrite,
                  progress_bar=progress_bar)
 
     def post_close(self):
-        # Cleaning up on post_close to ensure that all artifacts are uploaded
-        if self._finished is not None:
-            self._finished.set()
+        # Shutdown logic:
+        # 1. Signal to the enqueue thread that all uploads are enqueued. Specifically.
+        #    set a flag indicating that that no more objects will be added to self._logged_objects.
+        # 2. Wait for the enqueue thread to shut down. It will only shut down once all objects are added to
+        #    self._file_upload_queue. This will mean that self._logged_objects is empty.
+        # 3. Send a flag to the workers that all uploads are enqueued in self._file_upload_queue.
+        # 4. Wait for the workers to shut down. This means that all files have been uploaded
+        if self._enqueue_thread_flag is not None:
+            self._enqueue_thread_flag.set()
 
-        # First, ensure that all uploads are enqueued
         if self._enqueue_thread is not None:
             self._enqueue_thread.join()
 
+        if self._worker_flag is not None:
+            self._worker_flag.set()
+
         # Then, ensure all workers have finished all uploads
         for worker in self._workers:
             worker.join()
 
         # Clean up the tempdir
         if self._tempdir is not None:
             self._tempdir.cleanup()
 
-        # Reset all variables
-        self._tempdir = None
-        self._finished = None
-        self._workers.clear()
-        self._enqueued_objects.clear()
-        self._logged_objects.clear()
-        assert self._file_upload_queue.empty()
-
         # Empty the completed queue
+        # This cleanup will not be done by the enqueue_thread anymore, as that thread has been shut down
         while True:
             try:
-                self._completed_queue.get_nowait()
+                object_name = self._completed_queue.get_nowait()
             except queue.Empty:
                 break
+            self._enqueued_objects.remove(object_name)
             self._completed_queue.task_done()
 
+        if len(self._enqueued_objects) > 0 or len(self._logged_objects) > 0:
+            # Warn on all objects that have not been uploaded
+            object_names = list(self._enqueued_objects)
+            object_names.extend(self._logged_objects.keys())
+            warnings.warn(
+                RuntimeWarning('The following objects may not have been uploaded, likely due to a worker crash: ' +
+                               ', '.join(self._enqueued_objects)))
+
+        # Reset all variables
+        self._logged_objects.clear()
+        self._enqueued_objects.clear()
         self._enqueue_thread = None
+        self._tempdir = None
+        self._worker_flag = None
+        self._enqueue_thread_flag = None
+        self._workers.clear()
 
     def get_uri_for_artifact(self, artifact_name: str) -> str:
         """Get the object store provider uri for an artfact.
 
         Args:
             artifact_name (str): The name of an artifact.
```

### Comparing `mosaicml-0.8.2/composer/loggers/progress_bar_logger.py` & `mosaicml-0.9.0/composer/loggers/progress_bar_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         else:
             if self.position != 0:
                 # Force a (potentially hidden) progress bar to re-render itself
                 # Don't render the dummy pbar (at position 0), since that will clear a real pbar (at position 1)
                 self.pbar.refresh()
             # Create a newline that will not be erased by leave=False. This allows for the finished pbar to be cached in the terminal
             # This emulates `leave=True` without progress bar jumping
-            print('', file=self.file, flush=True)
+            if not self.file.closed:
+                print('', file=self.file, flush=True)
             self.pbar.close()
 
     def state_dict(self) -> Dict[str, Any]:
         pbar_state = self.pbar.format_dict
 
         return {
             'total': pbar_state['total'],
```

### Comparing `mosaicml-0.8.2/composer/loggers/tensorboard_logger.py` & `mosaicml-0.9.0/composer/loggers/tensorboard_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         self._flush(logger)
 
     def _flush(self, logger: Logger):
         # To avoid empty log artifacts for each rank.
         if self.rank_zero_only and dist.get_global_rank() != 0:
             return
 
-        assert self.writer is not None
+        if self.writer is None:
+            return
         # Skip if no writes occurred since last flush.
         if not self.writer.file_writer:
             return
 
         self.writer.flush()
 
         file_path = self.writer.file_writer.event_writer._file_name
@@ -130,7 +131,12 @@
                              artifact_name=('tensorboard_logs/{run_name}/' +
                                             f'{event_file_name}-{dist.get_global_rank()}'),
                              file_path=file_path,
                              overwrite=True)
 
         # Close writer, which creates new log file.
         self.writer.close()
+
+    def close(self, state: State, logger: Logger) -> None:
+        del state  # unused
+        self._flush(logger)
+        self.writer = None
```

### Comparing `mosaicml-0.8.2/composer/loggers/wandb_logger.py` & `mosaicml-0.9.0/composer/loggers/wandb_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,14 +91,19 @@
             init_kwargs['tags'] = tags
 
         self._rank_zero_only = rank_zero_only
         self._log_artifacts = log_artifacts
         self._init_kwargs = init_kwargs
         self._is_in_atexit = False
 
+        # Set these variable directly to allow fetching an Artifact **without** initializing a WandB run
+        # When used as a LoggerDestination, these values are overriden from global rank 0 to all ranks on Event.INIT
+        self.entity = entity
+        self.project = project
+
     def _set_is_in_atexit(self):
         self._is_in_atexit = True
 
     def log_data(self, state: State, log_level: LogLevel, data: Dict[str, Any]):
         import wandb
         del log_level  # unused
         if self._enabled:
@@ -132,15 +137,24 @@
         # Adjust name and group based on `rank_zero_only`.
         if not self._rank_zero_only:
             name = self._init_kwargs['name']
             self._init_kwargs['name'] += f'-rank{dist.get_global_rank()}'
             self._init_kwargs['group'] = self._init_kwargs['group'] if 'group' in self._init_kwargs else name
         if self._enabled:
             wandb.init(**self._init_kwargs)
+            assert wandb.run is not None, 'The wandb run is set after init'
+            entity_and_project = [str(wandb.run.entity), str(wandb.run.project)]
             atexit.register(self._set_is_in_atexit)
+        else:
+            entity_and_project = [None, None]
+        # Share the entity and project across all ranks, so they are available on ranks that did not initialize wandb
+        dist.broadcast_object_list(entity_and_project)
+        self.entity, self.project = entity_and_project
+        assert self.entity is not None, 'entity should be defined'
+        assert self.project is not None, 'project should be defined'
 
     def log_file_artifact(self, state: State, log_level: LogLevel, artifact_name: str, file_path: pathlib.Path, *,
                           overwrite: bool):
         del log_level, overwrite  # unused
 
         if self._enabled and self._log_artifacts:
             import wandb
@@ -169,26 +183,52 @@
                 name=new_artifact_name,
                 type=extension,
                 metadata=metadata,
             )
             artifact.add_file(os.path.abspath(file_path))
             wandb.log_artifact(artifact, aliases=aliases)
 
+    def can_log_file_artifacts(self) -> bool:
+        """Whether the logger supports logging file artifacts."""
+        return True
+
     def get_file_artifact(
         self,
         artifact_name: str,
         destination: str,
         overwrite: bool = False,
         progress_bar: bool = True,
     ):
-        # Note: Wandb doesn't support progress bars for downloading
+        # Note: WandB doesn't support progress bars for downloading
         del progress_bar
         import wandb
+        import wandb.errors
 
-        artifact = wandb.use_artifact(artifact_name)
+        # using the wandb.Api() to support retrieving artifacts on ranks where
+        # artifacts are not initialized
+        api = wandb.Api()
+        if not self.entity or not self.project:
+            raise RuntimeError('get_file_artifact can only be called after running init()')
+
+        # replace all unsupported characters with periods
+        # Only alpha-numeric, periods, hyphens, and underscores are supported by wandb.
+        if ':' not in artifact_name:
+            artifact_name += ':latest'
+
+        new_artifact_name = re.sub(r'[^a-zA-Z0-9-_\.:]', '.', artifact_name)
+        if new_artifact_name != artifact_name:
+            warnings.warn(('WandB permits only alpha-numeric, periods, hyphens, and underscores in artifact names. '
+                           f"The artifact with name '{artifact_name}' will be stored as '{new_artifact_name}'."))
+
+        try:
+            artifact = api.artifact('/'.join([self.entity, self.project, new_artifact_name]))
+        except wandb.errors.CommError as e:
+            if 'does not contain artifact' in str(e):
+                raise FileNotFoundError(f'Artifact {new_artifact_name} not found') from e
+            raise e
         with tempfile.TemporaryDirectory() as tmpdir:
             artifact_folder = os.path.join(tmpdir, 'artifact_folder')
             artifact.download(root=artifact_folder)
             artifact_names = os.listdir(artifact_folder)
             # We only log one file per artifact
             if len(artifact_names) > 1:
                 raise RuntimeError(
```

### Comparing `mosaicml-0.8.2/composer/loss/loss.py` & `mosaicml-0.9.0/composer/loss/loss.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import warnings
 from typing import Optional
 
 import torch
 from torch import Tensor
 from torch.nn import functional as F
+from torch.nn.modules.loss import _Loss
 
 from composer.loss.utils import ensure_targets_one_hot, infer_target_type
 
 __all__ = ['binary_cross_entropy_with_logits', 'loss_registry', 'soft_cross_entropy']
 
 
 def binary_cross_entropy_with_logits(
@@ -153,11 +154,128 @@
             xentropy *= num_examples / total_prob
 
         return xentropy
     else:
         raise ValueError(f'Unrecognized target type {target_type}')
 
 
+class DiceLoss(_Loss):
+    """Criterion that computes the dice loss between input and target.
+
+    The implementation is derived from MONAI: `<https://docs.monai.io/en/stable/losses.html#diceloss>`_.
+    For more information about the dice loss see the original paper on dice loss:
+    `<https://arxiv.org/abs/1606.04797>`_.
+
+    Args:
+        sigmoid (bool): If true, apply a sigmoid function to the input. Default: ``False``
+        softmax (bool): If true, apply a softmax function to the input. Default: ``False``
+        squared_pred (bool): If true, square the inputs and targets when calculating the
+            class unions. Default: ``False``
+        jaccard (bool): If true, compute the jaccard index (soft IoU) instead of dice.
+            Default: ``False``
+        batch (bool): If true, sum the intersection and union areas over the batch
+            dimension before dividing the two quantities. If false, a dice loss value is
+            computed independently for each sample in the batch before the reduction.
+        ignore_absent_classes (bool): If true, remove classes that are not present in
+            the target from the loss calculation. Classes not present in the target do
+            not contribute to the gradient, but can decrease the weight of present classes,
+            slowing optimization. This should have no effect if all classes are present in
+            each sample. Default: ``'False'``
+        reduction (str): Specifies the reduction to apply to the output: ``'none'`` |
+            ``'mean'`` | ``'sum'``. ``'none'``: no reduction will be appied, ``'mean'``:
+            the weighted mean of the output is taken, ``'sum'``: the output will be summed.
+            Default: ``'mean'``
+
+    """
+
+    def __init__(self,
+                 sigmoid: bool = False,
+                 softmax: bool = False,
+                 squared_pred: bool = False,
+                 jaccard: bool = False,
+                 batch: bool = False,
+                 ignore_absent_classes: bool = False,
+                 reduction: str = 'mean'):
+        super().__init__(reduction=reduction)
+        if sigmoid and softmax:
+            raise ValueError('Both sigmoid and softmax should not be true.')
+        if not reduction in ['none', 'mean', 'sum']:
+            raise ValueError(f'reduction was {reduction}, but must be one of ["none", "mean", "sum"]')
+
+        self.sigmoid = sigmoid
+        self.softmax = softmax
+        self.squared_pred = squared_pred
+        self.jaccard = jaccard
+        self.reduction = reduction
+        self.batch = batch
+        self.ignore_absent_classes = ignore_absent_classes
+
+    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
+
+        # If target is not one-hot, convert to one-hot
+        target = ensure_targets_one_hot(input, target)
+
+        # Get mask of pixels with a target
+        target_mask = target.sum(dim=1, keepdim=True) != 0
+
+        if input.shape != target.shape:
+            raise AssertionError(f'ground truth has different shape ({target.shape}) from input ({input.shape})')
+
+        if self.sigmoid:
+            input = torch.sigmoid(input)
+
+        n_pred_ch = input.shape[1]
+        if self.softmax:
+            if n_pred_ch == 1:
+                warnings.warn('single channel prediction, `softmax=True` ignored.')
+            else:
+                input = torch.softmax(input, 1)
+
+        reduce_axis = torch.arange(2, len(input.shape)).tolist()
+        if self.batch:
+            # reducing spatial dimensions and batch
+            reduce_axis = [0] + reduce_axis
+
+        intersection = torch.sum(target * input, dim=reduce_axis)
+
+        if self.squared_pred:
+            target = torch.pow(target, 2)
+            input = torch.pow(input, 2)
+
+        # Zero out pixels which do not have a target
+        input = target_mask * input
+
+        ground_o = torch.sum(target, dim=reduce_axis)
+        pred_o = torch.sum(input, dim=reduce_axis)
+
+        union = ground_o + pred_o
+
+        if self.jaccard:
+            union = 2.0 * (union - intersection)
+
+        epsilon = 1e-5
+        ious = 1.0 - (2.0 * intersection + epsilon) / (union + epsilon)
+
+        if self.ignore_absent_classes:
+            if self.batch:
+                ious = ious[ground_o > 0]
+            else:
+                ious = ious[:, (ground_o.sum(dim=0) > 0)]
+
+        if self.reduction == 'mean':
+            iou = torch.mean(ious)  # the batch and channel average
+        elif self.reduction == 'sum':
+            iou = torch.sum(ious)  # sum over the batch and channel dims
+        elif self.reduction == 'none':
+            # If we are not computing voxelwise loss components at least
+            # make sure a none reduction maintains a broadcastable shape
+            iou = ious
+        else:
+            raise ValueError(f'Unsupported reduction: {self.reduction}, available options are ["mean", "sum", "none"].')
+
+        return iou
+
+
 loss_registry = {
     'binary_cross_entropy_with_logits': binary_cross_entropy_with_logits,
     'soft_cross_entropy': soft_cross_entropy
 }
```

### Comparing `mosaicml-0.8.2/composer/metrics/metrics.py` & `mosaicml-0.9.0/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/metrics/nlp.py` & `mosaicml-0.9.0/composer/metrics/nlp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/__init__.py` & `mosaicml-0.9.0/composer/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 See :doc:`Composer Model </composer_model>` for more details.
 """
 
 from composer.models.base import ComposerModel as ComposerModel
 from composer.models.bert import BERTForClassificationHparams as BERTForClassificationHparams
 from composer.models.bert import BERTHparams as BERTHparams
-from composer.models.bert import BERTModel as BERTModel
-from composer.models.classify_mnist import MNIST_Classifier as MNIST_Classifier
+from composer.models.bert import create_bert_classification as create_bert_classification
+from composer.models.bert import create_bert_mlm as create_bert_mlm
 from composer.models.classify_mnist import MnistClassifierHparams as MnistClassifierHparams
-from composer.models.deeplabv3 import ComposerDeepLabV3 as ComposerDeepLabV3
+from composer.models.classify_mnist import mnist_model as mnist_model
 from composer.models.deeplabv3 import DeepLabV3Hparams as DeepLabV3Hparams
-from composer.models.efficientnetb0 import EfficientNetB0 as EfficientNetB0
+from composer.models.deeplabv3 import composer_deeplabv3 as composer_deeplabv3
 from composer.models.efficientnetb0 import EfficientNetB0Hparams as EfficientNetB0Hparams
+from composer.models.efficientnetb0 import composer_efficientnetb0 as composer_efficientnetb0
 from composer.models.gpt2 import GPT2Hparams as GPT2Hparams
-from composer.models.gpt2 import GPT2Model as GPT2Model
+from composer.models.gpt2 import create_gpt2 as create_gpt2
 from composer.models.huggingface import HuggingFaceModel as HuggingFaceModel
 from composer.models.initializers import Initializer as Initializer
 from composer.models.model_hparams import ModelHparams as ModelHparams
-from composer.models.resnet import ComposerResNet as ComposerResNet
 from composer.models.resnet import ResNetHparams as ResNetHparams
-from composer.models.resnet_cifar import ComposerResNetCIFAR as ComposerResNetCIFAR
+from composer.models.resnet import composer_resnet as composer_resnet
 from composer.models.resnet_cifar import ResNetCIFARHparams as ResNetCIFARHparams
+from composer.models.resnet_cifar import composer_resnet_cifar as composer_resnet_cifar
 from composer.models.ssd import SSD as SSD
 from composer.models.ssd import SSDHparams as SSDHparams
 from composer.models.tasks import ComposerClassifier as ComposerClassifier
-from composer.models.timm import Timm as Timm
 from composer.models.timm import TimmHparams as TimmHparams
-from composer.models.transformer_hparams import TransformerHparams as TransformerHparams
-from composer.models.transformer_shared import ComposerTransformer as ComposerTransformer
+from composer.models.timm import composer_timm as composer_timm
 from composer.models.unet import UNet as UNet
 from composer.models.unet import UnetHparams as UnetHparams
-from composer.models.vit_small_patch16 import ViTSmallPatch16 as ViTSmallPatch16
 from composer.models.vit_small_patch16 import ViTSmallPatch16Hparams as ViTSmallPatch16Hparams
+from composer.models.vit_small_patch16 import vit_small_patch16 as vit_small_patch16
```

### Comparing `mosaicml-0.8.2/composer/models/base.py` & `mosaicml-0.9.0/composer/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             def loss(self, outputs, batch):
                 # pass batches and `forward` outputs to the loss
                 _, targets = batch
                 return F.cross_entropy(outputs, targets)
 
     Attributes:
         logger (Optional[Logger]): The training :class:`.Logger`.
-            The trainer sets the :class:`.Logger` on the:attr:`~composer.core.event.Event.INIT` event.
+            The trainer sets the :class:`.Logger` on the:attr:`.Event.INIT` event.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.logger: Optional[Logger] = None
 
     def __deepcopy__(self, memo: dict):
```

### Comparing `mosaicml-0.8.2/composer/models/bert/__init__.py` & `mosaicml-0.9.0/composer/models/bert/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,10 +2,11 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """The `BERT <https://huggingface.co/docs/transformers/master/en/model_doc/bert>`_ model family using `Hugging Face
 Transformers <https://huggingface.co/transformers/>`_."""
 
 from composer.models.bert.bert_hparams import BERTForClassificationHparams as BERTForClassificationHparams
 from composer.models.bert.bert_hparams import BERTHparams as BERTHparams
-from composer.models.bert.model import BERTModel as BERTModel
+from composer.models.bert.model import create_bert_classification as create_bert_classification
+from composer.models.bert.model import create_bert_mlm as create_bert_mlm
 
-__all__ = ['BERTModel', 'BERTHparams', 'BERTForClassificationHparams']
+__all__ = ['BERTHparams', 'BERTForClassificationHparams', 'create_bert_classification', 'create_bert_mlm']
```

### Comparing `mosaicml-0.8.2/composer/models/bert/model.py` & `mosaicml-0.9.0/composer/models/gpt2/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,115 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""Implements a BERT wrapper around a :class:`.ComposerTransformer`."""
+"""GPT-2 model based on `Hugging Face GPT-2 <https://huggingface.co/docs/transformers/master/en/model_doc/gpt2>`_.
+
+Implemented as a wrapper using :class:`.ComposerTrainer`.
+"""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Mapping, Optional, Sequence, Union
+from typing import Optional
 
-import torch
-from torchmetrics import MeanSquaredError, Metric, MetricCollection
-from torchmetrics.classification.accuracy import Accuracy
-from torchmetrics.classification.matthews_corrcoef import MatthewsCorrCoef
-from torchmetrics.regression.spearman import SpearmanCorrCoef
+from composer.metrics.nlp import HFCrossEntropy, Perplexity
+from composer.models.huggingface import HuggingFaceModel
+from composer.utils.import_helpers import MissingConditionalImportError
 
-from composer.metrics.nlp import BinaryF1Score, LanguageCrossEntropy, MaskedAccuracy
-from composer.models.transformer_shared import ComposerTransformer
+__all__ = ['create_gpt2']
 
-if TYPE_CHECKING:
-    import transformers
 
-    from composer.core.types import Batch
+def create_gpt2(use_pretrained: Optional[bool] = False,
+                pretrained_model_name: Optional[str] = None,
+                model_config: Optional[dict] = None,
+                tokenizer_name: Optional[str] = None,
+                gradient_checkpointing: Optional[bool] = False):
+    """Implements :class:`~composer.models.huggingface.HuggingFaceModel` to wrap `Hugging Face GPT-2 \
+    transformers <https://huggingface.co/docs/transformers/master/en/model_doc/gpt2#overview>`_. Logs training and
+    validation perplexity.
 
-__all__ = ['BERTModel']
+    From `Language Models are Unsupervised Multitask Learners <https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf>`_ (Radford et al, 2018).
 
+    Args:
 
-class BERTModel(ComposerTransformer):
-    """BERT model based on |:hugging_face:| Transformers.
+        gradient_checkpointing (bool, optional): Use gradient checkpointing. Default: ``False``.
+        use_pretrained (bool, optional): Whether to initialize the model with the pretrained weights. Default: ``False``.
+        model_config (dict): A dictionary providing a HuggingFace model configuration.
+        tokenizer_name (str, optional): Tokenizer name used to preprocess the dataset
+        and validate the models inputs.
+
+        .. code-block::
+
+            {
+              "_name_or_path": "gpt2",
+              "activation_function": "gelu_new",
+              "architectures": ["GPT2LMHeadModel"],
+              "attn_pdrop": 0.1,
+              "bos_token_id": 50256,
+              "embd_pdrop": 0.1,
+              "eos_token_id": 50256,
+              "initializer_range": 0.02,
+              "layer_norm_epsilon": 1e-05,
+              "model_type": "gpt2",
+              "n_ctx": 1024,
+              "n_embd": 768,
+              "n_head": 12,
+              "n_inner": null,
+              "n_layer": 12,
+              "n_positions": 1024,
+              "reorder_and_upcast_attn": false,
+              "resid_pdrop": 0.1,
+              "scale_attn_by_inverse_layer_idx": false,
+              "scale_attn_weights": true,
+              "summary_activation": null,
+              "summary_first_dropout": 0.1,
+              "summary_proj_to_labels": true,
+              "summary_type": "cls_index",
+              "summary_use_proj": true,
+              "task_specific_params": {
+              "text-generation": {
+              "do_sample": true,
+              "max_length": 50 }
+              },
+              "transformers_version": "4.16.0",
+              "use_cache": true,
+              "vocab_size": 50257
+            }
 
-    For more information, see `Transformers <https://huggingface.co/transformers/>`_.
+   To create a GPT-2 model for language modeling pretraining:
 
-    Args:
-        module (transformers.BertModel): An instance of BertModel that
-            contains the forward pass function.
-        config (transformers.BertConfig): The BertConfig object that
-            stores information about the model hyperparameters.
-        tokenizer (transformers.BertTokenizer): An instance of BertTokenizer. Necessary to process model inputs.
+    .. testcode::
 
-    To create a BERT model for Language Model pretraining:
+        from composer.models import create_gpt2
 
-    .. testcode::
+        composer_model = create_gpt2()
 
-        from composer.models import BERTModel
+    """
+    try:
         import transformers
+    except ImportError as e:
+        raise MissingConditionalImportError(extra_deps_group='nlp', conda_package='transformers') from e
 
-        config = transformers.BertConfig()
-        hf_model = transformers.BertLMHeadModel(config=config)
-        tokenizer = transformers.BertTokenizer.from_pretrained("bert-base-uncased")
-        model = BERTModel(module=hf_model, config=config, tokenizer=tokenizer)
-    """
+    if not model_config:
+        model_config = {}
 
-    def __init__(self,
-                 module: transformers.BertModel,
-                 config: transformers.BertConfig,
-                 tokenizer: Optional[transformers.BertTokenizer] = None) -> None:
-
-        if tokenizer is None:
-            model_inputs = {'input_ids', 'attention_mask', 'token_type_ids'}
-        else:
-            model_inputs = set(tokenizer.model_input_names)
-
-        super().__init__(
-            module=module,  #type: ignore (thirdparty)
-            config=config,
-            model_inputs=model_inputs)
-
-        # we're going to remove the label from the expected inputs
-        # since we will handle metric calculation with TorchMetrics instead of HuggingFace.
-        self.model_inputs.remove('labels')
-
-        # When using Evaluators, the validation metrics represent all possible
-        # validation metrics that can be used with the bert model
-        # The Evaluator class checks if it's metrics are in the models validation metrics
-
-        ignore_index = -100
-        self.val_metrics = [
-            Accuracy(),
-            MeanSquaredError(),
-            SpearmanCorrCoef(),
-            BinaryF1Score(),
-            MatthewsCorrCoef(num_classes=config.num_labels),
-            LanguageCrossEntropy(ignore_index=ignore_index, vocab_size=config.num_labels),
-            MaskedAccuracy(ignore_index=ignore_index),
-        ]
-        self.train_metrics = []
-
-    def loss(self, outputs: Mapping, batch: Batch) -> Union[torch.Tensor, Sequence[torch.Tensor]]:
-        if outputs.get('loss', None) is not None:
-            return outputs['loss']
-        else:
-            raise NotImplementedError('Calculating loss directly not supported yet.')
-
-    def validate(self, batch: Any) -> Any:
-        """Runs the validation step.
-
-        Args:
-            batch (Dict): a dictionary of Dict[str, Tensor] of inputs
-                that the model expects, as found in :meth:`.ComposerTransformer.get_model_inputs`.
-
-        Returns:
-            tuple (Tensor, Tensor): with the output from the forward pass and the correct labels.
-                This is fed into directly into the output of :meth:`.ComposerModel.metrics`.
-        """
-        assert self.training is False, 'For validation, model must be in eval mode'
-
-        # temporary hack until eval on multiple datasets is finished
-        labels = batch.pop('labels')
-        output = self.forward(batch)
-        output = output['logits']
-
-        # if we are in the single class case, then remove the classes dimension
-        if output.shape[1] == 1:
-            output = output.squeeze(dim=1)
+    if not pretrained_model_name:
+        pretrained_model_name = 'gpt2'
 
-        return output, labels
+    if use_pretrained:
+        assert transformers.AutoModelForCausalLM.from_pretrained is not None, 'AutoModelForCausalLM has from_pretrained method'
+        model = transformers.AutoModelForCausalLM.from_pretrained(pretrained_model_name_or_path=pretrained_model_name,
+                                                                  **model_config)
+    else:
+        config = transformers.AutoConfig.from_pretrained(pretrained_model_name, **model_config)
+        assert transformers.AutoModelForCausalLM.from_config is not None, 'AutoModelForCausalLM has from_config method'
+        model = transformers.AutoModelForCausalLM.from_config(config)
+
+    if gradient_checkpointing:
+        model.gradient_checkpointing_enable()  # type: ignore
+
+    # setup the tokenizer
+    if tokenizer_name:
+        tokenizer = transformers.AutoTokenizer.from_pretrained(tokenizer_name)
+    else:
+        tokenizer = None
 
-    def metrics(self, train: bool = False) -> Union[Metric, MetricCollection]:
-        return MetricCollection(self.train_metrics) if train else MetricCollection(self.val_metrics)
+    return HuggingFaceModel(model=model, tokenizer=tokenizer, metrics=[HFCrossEntropy(), Perplexity()])
```

### Comparing `mosaicml-0.8.2/composer/models/classify_mnist/__init__.py` & `mosaicml-0.9.0/composer/models/classify_mnist/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A simple example convolutional neural network which can be used to classify MNIST data."""
 from composer.models.classify_mnist.mnist_hparams import MnistClassifierHparams as MnistClassifierHparams
-from composer.models.classify_mnist.model import MNIST_Classifier as MNIST_Classifier
+from composer.models.classify_mnist.model import mnist_model as mnist_model
 
-__all__ = ['MNIST_Classifier', 'MnistClassifierHparams']
+__all__ = ['mnist_model', 'MnistClassifierHparams']
 
 _task = 'Image Classification'
 _dataset = 'MNIST'
 _name = 'SimpleConvNet'
 _quality = ''
 _metric = 'Accuracy'
 _ttt = '?'
```

### Comparing `mosaicml-0.8.2/composer/models/classify_mnist/mnist_hparams.py` & `mosaicml-0.9.0/composer/models/classify_mnist/mnist_hparams.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.MNIST_Classifier`."""
+"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.mnist_model`."""
 
 from dataclasses import asdict, dataclass
 
 from composer.models.model_hparams import ModelHparams
 
 __all__ = ['MnistClassifierHparams']
 
 
 @dataclass
 class MnistClassifierHparams(ModelHparams):
-    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.MNIST_Classifier`.
+    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.mnist_model`.
 
     Args:
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: 10.
         initializers (List[Initializer], optional): Initializers for the model. ``None`` for no initialization. Default: ``None``.
     """
 
     def initialize_object(self):
-        from composer.models import MNIST_Classifier
-        return MNIST_Classifier(**asdict(self))
+        from composer.models import mnist_model
+        return mnist_model(**asdict(self))
```

### Comparing `mosaicml-0.8.2/composer/models/classify_mnist/model.py` & `mosaicml-0.9.0/composer/models/classify_mnist/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
 
 from composer.models.initializers import Initializer
 from composer.models.tasks import ComposerClassifier
 
-__all__ = ['Model', 'MNIST_Classifier']
+__all__ = ['Model', 'mnist_model']
 
 
 class Model(nn.Module):
     """Toy convolutional neural network architecture in pytorch for MNIST."""
 
     def __init__(self, initializers: Sequence[Union[str, Initializer]], num_classes: int = 10):
         super().__init__()
@@ -42,35 +42,33 @@
         out = F.adaptive_avg_pool2d(out, (4, 4))
         out = torch.flatten(out, 1, -1)
         out = self.fc1(out)
         out = F.relu(out)
         return self.fc2(out)
 
 
-class MNIST_Classifier(ComposerClassifier):
-    """A simple convolutional neural network extending :class:`.ComposerClassifier`. This class makes :class:`.Model`
-    compatible with :class:`.Trainer`
+def mnist_model(num_classes: int = 10, initializers: Optional[List[Initializer]] = None):
+    """Helper function to create a :class:`.ComposerClassifier` with a simple convolutional neural network.
 
     Args:
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``10``
         initializers (List[Initializer], optional): list of Initializers
             for the model. ``None`` for no initialization. Default: ``None``
 
+    Returns:
+        ComposerModel: instance of :class:`.ComposerClassifier` with a simple MNIST model.
+
     Example:
 
     .. testcode::
 
-        from composer.models import MNIST_Classifier
+        from composer.models import mnist_model
 
-        model = MNIST_Classifier()
+        model = mnist_model()
     """
 
-    def __init__(
-        self,
-        num_classes: int = 10,
-        initializers: Optional[List[Initializer]] = None,
-    ) -> None:
-        if initializers is None:
-            initializers = []
+    if initializers is None:
+        initializers = []
 
-        model = Model(initializers, num_classes)
-        super().__init__(module=model)
+    model = Model(initializers, num_classes)
+    composer_model = ComposerClassifier(module=model)
+    return composer_model
```

### Comparing `mosaicml-0.8.2/composer/models/deeplabv3/deeplabv3.py` & `mosaicml-0.9.0/composer/models/deeplabv3/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """DeepLabV3 model extending :class:`.ComposerClassifier`."""
 
+import functools
 import textwrap
-from typing import Any, Sequence
+import warnings
+from typing import Optional, Sequence
 
 import torch
+import torch.distributed as torch_dist
 import torch.nn.functional as F
+import torchvision
+from packaging import version
 from torchmetrics import MetricCollection
 from torchvision.models import _utils, resnet
 
-from composer.loss import soft_cross_entropy
+from composer.loss import DiceLoss, soft_cross_entropy
 from composer.metrics import CrossEntropy, MIoU
-from composer.models.base import ComposerModel
 from composer.models.initializers import Initializer
+from composer.models.tasks import ComposerClassifier
+from composer.utils import dist
 
-__all__ = ['deeplabv3_builder', 'ComposerDeepLabV3']
+__all__ = ['deeplabv3', 'composer_deeplabv3']
 
 
 class SimpleSegmentationModel(torch.nn.Module):
 
     def __init__(self, backbone, classifier):
         super().__init__()
         self.backbone = backbone
@@ -34,70 +40,89 @@
                                size=input_shape,
                                mode='bilinear',
                                align_corners=False,
                                recompute_scale_factor=False)
         return logits
 
 
-def deeplabv3_builder(num_classes: int,
-                      backbone_arch: str = 'resnet101',
-                      is_backbone_pretrained: bool = True,
-                      backbone_url: str = '',
-                      sync_bn: bool = True,
-                      use_plus: bool = True,
-                      initializers: Sequence[Initializer] = ()):
-    """Helper function to build a torchvision DeepLabV3 model with a 3x3 convolution layer and dropout removed.
+def deeplabv3(num_classes: int,
+              backbone_arch: str = 'resnet101',
+              backbone_weights: Optional[str] = None,
+              sync_bn: bool = True,
+              use_plus: bool = True,
+              initializers: Sequence[Initializer] = ()):
+    """Helper function to build a mmsegmentation DeepLabV3 model.
 
     Args:
         num_classes (int): Number of classes in the segmentation task.
-        backbone_arch (str, optional): The architecture to use for the backbone. Must be either [``'resnet50'``, ``'resnet101'``].
-            Default: ``'resnet101'``.
-        is_backbone_pretrained (bool, optional): If ``True``, use pretrained weights for the backbone. Default: ``True``.
-        backbone_url (str, optional): Url used to download model weights. If empty, the PyTorch url will be used.
-            Default: ``''``.
-        sync_bn (bool, optional): If ``True``, replace all BatchNorm layers with SyncBatchNorm layers. Default: ``True``.
+        backbone_arch (str, optional): The architecture to use for the backbone. Must be either
+            [``'resnet50'``, ``'resnet101'``]. Default: ``'resnet101'``.
+        backbone_weights (str, optional): If specified, the PyTorch pre-trained weights to load for the backbone.
+            Currently, only ['IMAGENET1K_V1', 'IMAGENET1K_V2'] are supported. Default: ``None``.
+        sync_bn (bool, optional): If ``True``, replace all BatchNorm layers with SyncBatchNorm layers.
+            Default: ``True``.
         use_plus (bool, optional): If ``True``, use DeepLabv3+ head instead of DeepLabv3. Default: ``True``.
-        initializers (Sequence[Initializer], optional): Initializers for the model. ``[]`` for no initialization. Default: ``()``.
+        initializers (Sequence[Initializer], optional): Initializers for the model. ``()`` for no initialization.
+            Default: ``()``.
 
     Returns:
         deeplabv3: A DeepLabV3 :class:`torch.nn.Module`.
 
     Example:
 
     .. code-block:: python
 
-        from composer.models.deeplabv3.deeplabv3 import deeplabv3_builder
+        from composer.models.deeplabv3.deeplabv3 import deeplabv3
 
-        pytorch_model = deeplabv3_builder(num_classes=150, backbone_arch='resnet101', is_backbone_pretrained=False)
+        pytorch_model = deeplabv3(num_classes=150, backbone_arch='resnet101', backbone_weights=None)
     """
 
     # check that the specified architecture is in the resnet module
     if not hasattr(resnet, backbone_arch):
         raise ValueError(f'backbone_arch must be part of the torchvision resnet module, got value: {backbone_arch}')
 
     # change the model weight url if specified
-    if backbone_url:
-        resnet.model_urls[backbone_arch] = backbone_url
-    backbone = getattr(resnet, backbone_arch)(pretrained=is_backbone_pretrained,
-                                              replace_stride_with_dilation=[False, True, True])
+    if version.parse(torchvision.__version__) < version.parse('0.13.0'):
+        pretrained = False
+        if backbone_weights:
+            pretrained = True
+            if backbone_weights == 'IMAGENET1K_V1':
+                resnet.model_urls[backbone_arch] = 'https://download.pytorch.org/models/resnet101-63fe2227.pth'
+            elif backbone_weights == 'IMAGENET1K_V2':
+                resnet.model_urls[backbone_arch] = 'https://download.pytorch.org/models/resnet101-cd907fc2.pth'
+            else:
+                ValueError(
+                    textwrap.dedent(f"""\
+                        `backbone_weights` must be either "IMAGENET1K_V1" or "IMAGENET1K_V2"
+                        if torchvision.__version__ < 0.13.0. `backbone_weights` was {backbone_weights}."""))
+        backbone = getattr(resnet, backbone_arch)(pretrained=pretrained,
+                                                  replace_stride_with_dilation=[False, True, True])
+    else:
+        backbone = getattr(resnet, backbone_arch)(weights=backbone_weights,
+                                                  replace_stride_with_dilation=[False, True, True])
 
     # specify which layers to extract activations from
     return_layers = {'layer1': 'layer1', 'layer4': 'layer4'} if use_plus else {'layer4': 'layer4'}
     backbone = _utils.IntermediateLayerGetter(backbone, return_layers=return_layers)
 
     try:
         from mmseg.models import ASPPHead, DepthwiseSeparableASPPHead
     except ImportError as e:
         raise ImportError(
             textwrap.dedent("""\
             Either mmcv or mmsegmentation is not installed. To install mmcv, please run pip install mmcv-full==1.4.4 -f
              https://download.openmmlab.com/mmcv/dist/{cu_version}/{torch_version}/index.html where {cu_version} and
              {torch_version} refer to your CUDA and PyTorch versions, respectively. To install mmsegmentation, please
              run pip install mmsegmentation==0.22.0 on command-line.""")) from e
-    norm_type = 'SyncBN' if sync_bn else 'BN'
+
+    world_size = dist.get_world_size()
+    if sync_bn and world_size == 1:
+        warnings.warn('sync_bn was true, but only one process is present for training. sync_bn will be ignored.')
+
+    norm_type = 'SyncBN' if sync_bn and world_size > 1 else 'BN'
     norm_cfg = {'type': norm_type, 'requires_grad': True}
     if use_plus:
         # mmseg config:
         # https://github.com/open-mmlab/mmsegmentation/blob/master/configs/_base_/models/deeplabv3plus_r50-d8.py
         head = DepthwiseSeparableASPPHead(in_channels=2048,
                                           in_index=-1,
                                           channels=512,
@@ -123,89 +148,105 @@
     model = SimpleSegmentationModel(backbone, head)
 
     if initializers:
         for initializer in initializers:
             initializer_fn = Initializer(initializer).get_initializer()
 
             # Only apply initialization to classifier head if pre-trained weights are used
-            if is_backbone_pretrained:
-                model.classifier.apply(initializer_fn)
-            else:
+            if backbone_weights is None:
                 model.apply(initializer_fn)
+            else:
+                model.classifier.apply(initializer_fn)
 
-    if sync_bn:
-        model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(model)
+    if sync_bn and world_size > 1:
+        local_world_size = dist.get_local_world_size()
+
+        # List of ranks for each node, assumes that each node has the same number of ranks
+        num_nodes = world_size // local_world_size
+        process_group = None
+        if num_nodes > 1:
+            ranks_per_node = [
+                list(range(node * local_world_size, (node + 1) * local_world_size)) for node in range(num_nodes)
+            ]
+            process_groups = [torch_dist.new_group(ranks) for ranks in ranks_per_node]
+            process_group = process_groups[dist.get_node_rank()]
+
+        model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(model, process_group=process_group)
 
     return model
 
 
-class ComposerDeepLabV3(ComposerModel):
-    """DeepLabV3 model extending :class:`.ComposerClassifier`. Logs Mean Intersection over Union (MIoU) and Cross
-    Entropy during training and validation.
+def composer_deeplabv3(num_classes: int,
+                       backbone_arch: str = 'resnet101',
+                       backbone_weights: Optional[str] = None,
+                       sync_bn: bool = True,
+                       use_plus: bool = True,
+                       ignore_index: int = -1,
+                       cross_entropy_weight: float = 1.0,
+                       dice_weight: float = 0.0,
+                       initializers: Sequence[Initializer] = ()):
+    """Helper function to create a :class:`.ComposerClassifier` with a DeepLabv3(+) model. Logs
+        Mean Intersection over Union (MIoU) and Cross Entropy during training and validation.
 
-    From `Rethinking Atrous Convolution for Semantic Image Segmentation <https://arxiv.org/abs/1706.05587>`_ (Chen et al, 2017).
+    From `Rethinking Atrous Convolution for Semantic Image Segmentation <https://arxiv.org/abs/1706.05587>`_
+        (Chen et al, 2017).
 
     Args:
         num_classes (int): Number of classes in the segmentation task.
-        backbone_arch (str, optional): The architecture to use for the backbone. Must be either [``'resnet50'``, ``'resnet101'``].
-            Default: ``'resnet101'``.
-        is_backbone_pretrained (bool, optional): If ``True``, use pretrained weights for the backbone. Default: ``True``.
-        backbone_url (str, optional): Url used to download model weights. If empty, the PyTorch url will be used.
-            Default: ``''``.
-        sync_bn (bool, optional): If ``True``, replace all BatchNorm layers with SyncBatchNorm layers. Default: ``True``.
+        backbone_arch (str, optional): The architecture to use for the backbone. Must be either
+            [``'resnet50'``, ``'resnet101'``]. Default: ``'resnet101'``.
+        backbone_weights (str, optional): If specified, the PyTorch pre-trained weights to load for the backbone.
+            Currently, only ['IMAGENET1K_V1', 'IMAGENET1K_V2'] are supported. Default: ``None``.
+        sync_bn (bool, optional): If ``True``, replace all BatchNorm layers with SyncBatchNorm layers.
+            Default: ``True``.
         use_plus (bool, optional): If ``True``, use DeepLabv3+ head instead of DeepLabv3. Default: ``True``.
-        initializers (List[Initializer], optional): Initializers for the model. ``[]`` for no initialization. Default: ``[]``.
+        ignore_index (int): Class label to ignore when calculating the loss and other metrics. Default: ``-1``.
+        cross_entropy_weight (float): Weight to scale the cross entropy loss. Default: ``1.0``.
+        dice_weight (float): Weight to scale the dice loss. Default: ``0.0``.
+        initializers (List[Initializer], optional): Initializers for the model. ``[]`` for no initialization.
+            Default: ``[]``.
 
 
+    Returns:
+        ComposerModel: instance of :class:`.ComposerClassifier` with a DeepLabv3(+) model.
+
     Example:
 
     .. code-block:: python
 
-        from composer.models import ComposerDeepLabV3
+        from composer.models import composer_deeplabv3
 
-        model = ComposerDeepLabV3(num_classes=150, backbone_arch='resnet101', is_backbone_pretrained=False)
+        model = composer_deeplabv3(num_classes=150, backbone_arch='resnet101', backbone_weights=None)
     """
 
-    def __init__(self,
-                 num_classes: int,
-                 backbone_arch: str = 'resnet101',
-                 is_backbone_pretrained: bool = True,
-                 backbone_url: str = '',
-                 sync_bn: bool = True,
-                 use_plus: bool = True,
-                 initializers: Sequence[Initializer] = ()):
-
-        super().__init__()
-        self.num_classes = num_classes
-        self.model = deeplabv3_builder(backbone_arch=backbone_arch,
-                                       is_backbone_pretrained=is_backbone_pretrained,
-                                       backbone_url=backbone_url,
-                                       use_plus=use_plus,
-                                       num_classes=num_classes,
-                                       sync_bn=sync_bn,
-                                       initializers=initializers)
-
-        # Metrics
-        self.train_miou = MIoU(self.num_classes, ignore_index=-1)
-        self.train_ce = CrossEntropy(ignore_index=-1)
-        self.val_miou = MIoU(self.num_classes, ignore_index=-1)
-        self.val_ce = CrossEntropy(ignore_index=-1)
-
-    def forward(self, batch: Any):
-        x = batch[0]
-        logits = self.model(x)
-        return logits
-
-    def loss(self, outputs: Any, batch: Any):
-        target = batch[1]
-        loss = soft_cross_entropy(outputs, target, ignore_index=-1)  # type: ignore
+    model = deeplabv3(backbone_arch=backbone_arch,
+                      backbone_weights=backbone_weights,
+                      use_plus=use_plus,
+                      num_classes=num_classes,
+                      sync_bn=sync_bn,
+                      initializers=initializers)
+
+    train_metrics = MetricCollection(
+        [CrossEntropy(ignore_index=ignore_index),
+         MIoU(num_classes, ignore_index=ignore_index)])
+    val_metrics = MetricCollection(
+        [CrossEntropy(ignore_index=ignore_index),
+         MIoU(num_classes, ignore_index=ignore_index)])
+
+    ce_loss_fn = functools.partial(soft_cross_entropy, ignore_index=ignore_index)
+    dice_loss_fn = DiceLoss(softmax=True, batch=True, ignore_absent_classes=True)
+
+    def _combo_loss(output, target):
+        loss = {}
+        if cross_entropy_weight:
+            ce_loss = ce_loss_fn(output, target) * cross_entropy_weight
+            loss['cross_entropy_loss'] = ce_loss
+        if dice_weight:
+            dice_loss = dice_loss_fn(output, target) * dice_weight
+            loss['dice_loss'] = dice_loss
         return loss
 
-    def metrics(self, train: bool = False):
-        metric_list = [self.train_miou, self.train_ce] if train else [self.val_miou, self.val_ce]
-        return MetricCollection(metric_list)
-
-    def validate(self, batch: Any):
-        assert self.training is False, 'For validation, model must be in eval mode'
-        target = batch[1]
-        logits = self.forward(batch)
-        return logits, target
+    composer_model = ComposerClassifier(module=model,
+                                        train_metrics=train_metrics,
+                                        val_metrics=val_metrics,
+                                        loss_fn=_combo_loss)
+    return composer_model
```

### Comparing `mosaicml-0.8.2/composer/models/efficientnetb0/__init__.py` & `mosaicml-0.9.0/composer/models/efficientnetb0/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 of vision tasks, but were initially designed for image classification. The model family was designed to reach the
 highest accuracy for a given computation budget during inference by simultaneously scaling model depth, model width, and
 image resolution according to an empirically determined scaling law.
 
 See the :doc:`Model Card </model_cards/efficientnet>` for more details.
 """
 from composer.models.efficientnetb0.efficientnetb0_hparams import EfficientNetB0Hparams as EfficientNetB0Hparams
-from composer.models.efficientnetb0.model import EfficientNetB0 as EfficientNetB0
+from composer.models.efficientnetb0.model import composer_efficientnetb0 as composer_efficientnetb0
 
-__all__ = ['EfficientNetB0', 'EfficientNetB0Hparams']
+__all__ = ['composer_efficientnetb0', 'EfficientNetB0Hparams']
 
 _task = 'Image Classification'
 _dataset = 'ImageNet'
 _name = 'EfficientNet-B0'
 _quality = '76.63'
 _metric = 'Top-1 Accuracy'
 _ttt = '21h 48m'
```

### Comparing `mosaicml-0.8.2/composer/models/efficientnetb0/_layers.py` & `mosaicml-0.9.0/composer/models/efficientnetb0/_layers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/efficientnetb0/efficientnets.py` & `mosaicml-0.9.0/composer/models/efficientnetb0/efficientnets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/efficientnetb0/model.py` & `mosaicml-0.9.0/composer/models/efficientnetb0/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A :class:`.ComposerClassifier` wrapper around the EfficientNet-b0 architecture."""
 from composer.models.efficientnetb0.efficientnets import EfficientNet
 from composer.models.tasks import ComposerClassifier
 
-__all__ = ['EfficientNetB0']
+__all__ = ['composer_efficientnetb0']
 
 
-class EfficientNetB0(ComposerClassifier):
-    """A :class:`.ComposerClassifier` wrapper around the EfficientNet-b0 architecture. From `Rethinking Model Scaling
-    for Convolutional Neural Networks <https://arxiv.org/abs/1905.11946>`_ (Tan et al, 2019).
+def composer_efficientnetb0(num_classes: int = 1000, drop_connect_rate: float = 0.2) -> ComposerClassifier:
+    """Helper function to create a :class:`.ComposerClassifier` with an EfficientNet-b0 architecture.
+
+    See `Rethinking Model Scaling for Convolutional Neural Networks <https://arxiv.org/abs/1905.11946>`_
+        (Tan et al, 2019) for more details.
 
     Args:
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``1000``.
-        drop_connect_rate (float, optional): Probability of dropping a sample within a block before identity connection. Default: ``0.2``.
+        drop_connect_rate (float, optional): Probability of dropping a sample within a block before identity
+            connection. Default: ``0.2``.
+
+    Returns:
+        ComposerModel: instance of :class:`.ComposerClassifier` with a EfficientNet-B0 model.
+
 
     Example:
 
     .. testcode::
 
-        from composer.models import EfficientNetB0
+        from composer.models import composer_efficientnetb0
 
-        model = EfficientNetB0()  # creates EfficientNet-b0 for image classification
+        model = composer_efficientnetb0()  # creates EfficientNet-b0 for image classification
     """
+    model = EfficientNet.get_model_from_name(model_name='efficientnet-b0',
+                                             num_classes=num_classes,
+                                             drop_connect_rate=drop_connect_rate)
 
-    def __init__(self, num_classes: int = 1000, drop_connect_rate: float = 0.2) -> None:
-        model = EfficientNet.get_model_from_name(
-            'efficientnet-b0',
-            num_classes,
-            drop_connect_rate,
-        )
-        super().__init__(module=model)
+    composer_model = ComposerClassifier(module=model)
+    return composer_model
```

### Comparing `mosaicml-0.8.2/composer/models/gpt2/__init__.py` & `mosaicml-0.9.0/composer/models/gpt2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 This family was originally proposed by OpenAI, and is trained on the OpenWebText dataset. It is useful for downstream
 language generation tasks, such as summarization, translation, and dialog.
 
 See the :doc:`Model Card </model_cards/GPT2>` for more details.
 """
 
 from composer.models.gpt2.gpt2_hparams import GPT2Hparams as GPT2Hparams
-from composer.models.gpt2.model import GPT2Model as GPT2Model
+from composer.models.gpt2.model import create_gpt2 as create_gpt2
 
-__all__ = ['GPT2Model', 'GPT2Hparams']
+__all__ = ['create_gpt2', 'GPT2Hparams']
 
 _metadata = {
     'gpt2': {
         '_task': 'Language Modeling',
         '_dataset': 'OpenWebText',
         '_name': 'GPT-2 52M',
         '_quality': '30.88',
```

### Comparing `mosaicml-0.8.2/composer/models/initializers.py` & `mosaicml-0.9.0/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/model_hparams.py` & `mosaicml-0.9.0/composer/models/model_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/resnet/__init__.py` & `mosaicml-0.9.0/composer/models/resnet/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 """The ResNet model family is a set of convolutional neural networks described in `Deep Residual Learning for Image
 Recognition <https://arxiv.org/abs/1512.03385>`_ (He et al, 2015). ResNets can be used as the base for a variety of
 vision tasks. ImageNet ResNets are a subset of the ResNet family which were designed specifically for classification on
 the ImageNet dataset.
 
 See the :doc:`Model Card </model_cards/resnet>` for more details.
 """
-from composer.models.resnet.model import ComposerResNet as ComposerResNet
+from composer.models.resnet.model import composer_resnet
 from composer.models.resnet.resnet_hparams import ResNetHparams as ResNetHparams
 
-__all__ = ['ComposerResNet', 'ResNetHparams']
+__all__ = ['ResNetHparams', 'composer_resnet']
 
 _metadata = {
     'resnet18': {
         '_task': 'Image Classification',
         '_dataset': 'ImageNet',
         '_name': 'ResNet18',
         '_quality': 'TBD',
```

### Comparing `mosaicml-0.8.2/composer/models/resnet/model.py` & `mosaicml-0.9.0/composer/models/resnet_cifar/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,51 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""A :class:`.ComposerClassifier` wrapper around the torchvision implementations of the ResNet model family."""
+"""ResNet models for CIFAR extending :class:`.ComposerClassifier`."""
 
 from typing import List, Optional
 
-from torchvision.models import resnet
-
 from composer.models.initializers import Initializer
+from composer.models.resnet_cifar.resnets import ResNet9, ResNetCIFAR
 from composer.models.tasks import ComposerClassifier
 
-__all__ = ['ComposerResNet']
+__all__ = ['composer_resnet_cifar']
 
 
-class ComposerResNet(ComposerClassifier):
-    """A :class:`.ComposerClassifier` wrapper around the torchvision implementations of the ResNet model family.
+def composer_resnet_cifar(model_name: str,
+                          num_classes: int = 10,
+                          initializers: Optional[List[Initializer]] = None) -> ComposerClassifier:
+    """Helper function to create a :class:`.ComposerClassifier` with a CIFAR ResNet models.
 
     From `Deep Residual Learning for Image Recognition <https://arxiv.org/abs/1512.03385>`_ (He et al, 2015).
+    ResNet9 is based on the  model from myrtle.ai `blog`_.
 
     Args:
-        model_name (str): Name of the ResNet model instance. Either [``"resnet18"``, ``"resnet34"``, ``"resnet50"``, ``"resnet101"``,
-            ``"resnet152"``].
-        num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``1000``.
-        pretrained (bool, optional): If True, use ImageNet pretrained weights. Default: ``False``.
-        groups (int, optional): Number of filter groups for the 3x3 convolution layer in bottleneck blocks. Default: ``1``.
-        width_per_group (int, optional): Initial width for each convolution group. Width doubles after each stage.
-            Default: ``64``.
+        model_name (str): ``"resnet_9"``, ``"resnet_20"``, or ``"resnet_56"``.
+        num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``10``.
         initializers (List[Initializer], optional): Initializers for the model. ``None`` for no initialization.
             Default: ``None``.
-        loss_name (str, optional): Loss function to use. E.g. 'soft_cross_entropy' or
-            'binary_cross_entropy_with_logits'. Loss function must be in
-            :mod:`~composer.loss.loss`. Default: ``'soft_cross_entropy'``".
+
+    Returns:
+        ComposerModel: instance of :class:`.ComposerClassifier` with a CIFAR ResNet model.
 
     Example:
 
     .. testcode::
 
-        from composer.models import ComposerResNet
+        from composer.models import composer_resnet_cifar
 
-        model = ComposerResNet(model_name='resnet18')  # creates a torchvision resnet18 for image classification
-    """
+        model = composer_resnet_cifar(model_name="resnet_56")  # creates a resnet56 for cifar image classification
 
-    valid_model_names = ['resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152']
+    .. _blog: https://myrtle.ai/learn/how-to-train-your-resnet-4-architecture/
+    """
+    if initializers is None:
+        initializers = []
 
-    def __init__(
-        self,
-        model_name: str,
-        num_classes: int = 1000,
-        pretrained: bool = False,
-        groups: int = 1,
-        width_per_group: int = 64,
-        initializers: Optional[List[Initializer]] = None,
-        loss_name: str = 'soft_cross_entropy',
-    ) -> None:
-
-        if model_name not in self.valid_model_names:
-            raise ValueError(f'model_name must be one of {self.valid_model_names} instead of {model_name}.')
-
-        if initializers is None:
-            initializers = []
-
-        model_func = getattr(resnet, model_name)
-        model = model_func(pretrained=pretrained,
-                           num_classes=num_classes,
-                           groups=groups,
-                           width_per_group=width_per_group)
-
-        for initializer in initializers:
-            initializer = Initializer(initializer)
-            model.apply(initializer.get_initializer())
+    if model_name == 'resnet_9':
+        model = ResNet9(num_classes)  # current initializers don't work with this architecture.
+    else:
+        model = ResNetCIFAR.get_model_from_name(model_name, initializers, num_classes)
 
-        super().__init__(module=model, loss_name=loss_name)
+    composer_model = ComposerClassifier(module=model)
+    return composer_model
```

### Comparing `mosaicml-0.8.2/composer/models/resnet/resnet_hparams.py` & `mosaicml-0.9.0/composer/models/resnet/resnet_hparams.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.ComposerResNet`."""
+"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.composer_resnet`."""
 
 from dataclasses import dataclass
+from typing import Optional
 
 import yahp as hp
 
 from composer.models.model_hparams import ModelHparams
-from composer.models.resnet.model import ComposerResNet
+from composer.models.resnet.model import composer_resnet, valid_model_names
 
 __all__ = ['ResNetHparams']
 
 
 @dataclass
 class ResNetHparams(ModelHparams):
-    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.ComposerResNet`.
+    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.composer_resnet`.
 
     Args:
         model_name (str): Name of the ResNet model instance. Either [``"resnet18"``, ``"resnet34"``, ``"resnet50"``, ``"resnet101"``,
             ``"resnet152"``].
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``1000``.
-        pretrained (bool, optional): If True, use ImageNet pretrained weights. Default: ``False``.
+        weights (str, optional): If provided, pretrained weights can be specified, such as with ``IMAGENET1K_V2``. Default: ``None``.
+        pretrained (bool, optional): If True, use ImageNet pretrained weights. Default: ``False``. This parameter is deprecated and
+            will soon be removed.
         groups (int, optional): Number of filter groups for the 3x3 convolution layer in bottleneck blocks. Default: ``1``.
         width_per_group (int, optional): Initial width for each convolution group. Width doubles after each stage.
             Default: ``64``.
         initializers (List[Initializer], optional): Initializers for the model. ``None`` for no initialization.
             Default: ``None``.
     """
 
     model_name: str = hp.optional(
-        f"ResNet architecture to instantiate, must be one of {ComposerResNet.valid_model_names}. (default: '')",
-        default='')
-    pretrained: bool = hp.optional('If true, use ImageNet pretrained weights. (default: ``False``)', default=False)
+        f"ResNet architecture to instantiate, must be one of {valid_model_names}. (default: '')", default='')
+    weights: Optional[str] = hp.optional(
+        'If provided, pretrained weights can be specified, such as with ``IMAGENET1K_V2``. (default: ``None``)',
+        default=None)
+    pretrained: bool = hp.optional(
+        'If True, use ImageNet pretrained weights. Default: ``False``. This parameter is deprecated and will soon be removed.',
+        default=False)
     groups: int = hp.optional(
         'Number of filter groups for the 3x3 convolution layer in bottleneck block. (default: ``1``)', default=1)
     width_per_group: int = hp.optional(
         'Initial width for each convolution group. Width doubles after each stage. (default: ``64``)', default=64)
     loss_name: str = hp.optional(
         "Name of loss function. E.g. 'soft_cross_entropy' or 'binary_cross_entropy_with_logits'. (default: ``soft_cross_entropy``)",
         default='soft_cross_entropy')
 
     def validate(self):
-        if self.model_name not in ComposerResNet.valid_model_names:
-            raise ValueError(f'model_name must be one of {ComposerResNet.valid_model_names}, but got {self.model_name}')
-
         if self.num_classes is None:
             raise ValueError('num_classes must be specified')
 
     def initialize_object(self):
         if self.num_classes is None:
             raise ValueError('num_classes must be specified')
-        return ComposerResNet(model_name=self.model_name,
-                              num_classes=self.num_classes,
-                              pretrained=self.pretrained,
-                              groups=self.groups,
-                              width_per_group=self.width_per_group,
-                              initializers=self.initializers,
-                              loss_name=self.loss_name)
+        return composer_resnet(model_name=self.model_name,
+                               num_classes=self.num_classes,
+                               weights=self.weights,
+                               pretrained=self.pretrained,
+                               groups=self.groups,
+                               width_per_group=self.width_per_group,
+                               initializers=self.initializers,
+                               loss_name=self.loss_name)
```

### Comparing `mosaicml-0.8.2/composer/models/resnet_cifar/__init__.py` & `mosaicml-0.9.0/composer/models/resnet_cifar/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """A ResNet model family adapted for CIFAR10 image sizes.
 
 See the :doc:`Model Card </model_cards/cifar_resnet>` for more details.
 """
 
-from composer.models.resnet_cifar.model import ComposerResNetCIFAR as ComposerResNetCIFAR
+from composer.models.resnet_cifar.model import composer_resnet_cifar as composer_resnet_cifar
 from composer.models.resnet_cifar.resnet_cifar_hparams import ResNetCIFARHparams as ResNetCIFARHparams
 
-__all__ = ['ComposerResNetCIFAR', 'ResNetCIFARHparams']
+__all__ = ['composer_resnet_cifar', 'ResNetCIFARHparams']
 
 _metadata = {
     'resnet9': {
         '_task': 'Image Classification',
         '_dataset': 'CIFAR10',
         '_name': 'ResNet9',
         '_quality': 'tbd',
```

### Comparing `mosaicml-0.8.2/composer/models/resnet_cifar/model.py` & `mosaicml-0.9.0/composer/models/resnet_cifar/resnet_cifar_hparams.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,38 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""ResNet models for CIFAR extending :class:`.ComposerClassifier`."""
+"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for
+:func:`.composer_resnet_cifar`."""
+from dataclasses import dataclass
+from typing import Optional
 
-from typing import List, Optional
+import yahp as hp
 
-from composer.models.initializers import Initializer
-from composer.models.resnet_cifar.resnets import ResNet9, ResNetCIFAR
-from composer.models.tasks import ComposerClassifier
+from composer.models.model_hparams import ModelHparams
+from composer.models.resnet_cifar import composer_resnet_cifar
 
-__all__ = ['ComposerResNetCIFAR']
+__all__ = ['ResNetCIFARHparams']
 
 
-class ComposerResNetCIFAR(ComposerClassifier):
-    """ResNet models for CIFAR10 extending :class:`.ComposerClassifier`.
-
-    From `Deep Residual Learning for Image Recognition <https://arxiv.org/abs/1512.03385>`_ (He et al, 2015).
-    ResNet9 is based on the  model from myrtle.ai `blog`_.
+@dataclass
+class ResNetCIFARHparams(ModelHparams):
+    """:class:`~.hp.Hparams` interface for :func:`.composer_resnet_cifar`.
 
     Args:
         model_name (str): ``"resnet_9"``, ``"resnet_20"``, or ``"resnet_56"``.
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``10``.
         initializers (List[Initializer], optional): Initializers for the model. ``None`` for no initialization. Default: ``None``.
-
-    Example:
-
-    .. testcode::
-
-        from composer.models import ComposerResNetCIFAR
-
-        model = ComposerResNetCIFAR(model_name="resnet_56")  # creates a resnet56 for cifar image classification
-
-    .. _blog: https://myrtle.ai/learn/how-to-train-your-resnet-4-architecture/
     """
+    model_name: Optional[str] = hp.optional('"cifar_resnet_9", "cifar_resnet_20" or "cifar_resnet_56"', default=None)
+    num_classes: int = hp.optional('The number of classes.  Needed for classification tasks', default=10)
 
-    def __init__(
-        self,
-        model_name: str,
-        num_classes: int = 10,
-        initializers: Optional[List[Initializer]] = None,
-    ) -> None:
-        if initializers is None:
-            initializers = []
-
-        if model_name == 'resnet_9':
-            model = ResNet9(num_classes)  # current initializers don't work with this architecture.
-        else:
-            model = ResNetCIFAR.get_model_from_name(
-                model_name,
-                initializers,
-                num_classes,
-            )
-        super().__init__(module=model)
+    def validate(self):
+        if self.model_name is None:
+            raise ValueError('model name must be one of "cifar_resnet_9", "cifar_resnet_20" or "cifar_resnet_56".')
+
+    def initialize_object(self):
+        if self.model_name is None:
+            raise ValueError('model name must be one of "cifar_resnet_9", "cifar_resnet_20" or "cifar_resnet_56".')
+        return composer_resnet_cifar(model_name=self.model_name,
+                                     num_classes=self.num_classes,
+                                     initializers=self.initializers)
```

### Comparing `mosaicml-0.8.2/composer/models/resnet_cifar/resnets.py` & `mosaicml-0.9.0/composer/models/resnet_cifar/resnets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/ssd/base_model.py` & `mosaicml-0.9.0/composer/models/ssd/base_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/ssd/ssd.py` & `mosaicml-0.9.0/composer/models/ssd/ssd.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/ssd/ssd300.py` & `mosaicml-0.9.0/composer/models/ssd/ssd300.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/ssd/ssd_hparams.py` & `mosaicml-0.9.0/composer/models/ssd/ssd_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/ssd/utils.py` & `mosaicml-0.9.0/composer/models/ssd/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/timm/model.py` & `mosaicml-0.9.0/composer/models/timm/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,26 @@
 used to create :class:`.ComposerClassifier`."""
 
 from typing import Optional
 
 from composer.models.tasks import ComposerClassifier
 from composer.utils.import_helpers import MissingConditionalImportError
 
-__all__ = ['Timm']
+__all__ = ['composer_timm']
 
 
-class Timm(ComposerClassifier):
+def composer_timm(model_name: str,
+                  pretrained: bool = False,
+                  num_classes: int = 1000,
+                  drop_rate: float = 0.0,
+                  drop_path_rate: Optional[float] = None,
+                  drop_block_rate: Optional[float] = None,
+                  global_pool: Optional[str] = None,
+                  bn_momentum: Optional[float] = None,
+                  bn_eps: Optional[float] = None) -> ComposerClassifier:
     """A wrapper around `timm.create_model() <https://rwightman.github.io/pytorch-image-models/#load-a-pretrained-
     model>`_ used to create :class:`.ComposerClassifier`.
 
     Args:
         model_name (str): timm model name e.g: ``"resnet50"``. List of models can be found at
             `PyTorch Image Models <https://github.com/rwightman/pytorch-image-models>`_.
         pretrained (bool, optional): Imagenet pretrained. Default: ``False``.
@@ -24,47 +32,35 @@
         drop_rate (float, optional): Dropout rate. Default: ``0.0``.
         drop_path_rate (float, optional): Drop path rate (model default if ``None``). Default: ``None``.
         drop_block_rate (float, optional): Drop block rate (model default if ``None``). Default: ``None``.
         global_pool (str, optional): Global pool type, one of (``"fast"``, ``"avg"``, ``"max"``, ``"avgmax"``, ``"avgmaxc"``). Model default if ``None``. Default: ``None``.
         bn_momentum (float, optional): BatchNorm momentum override (model default if ``None``). Default: ``None``.
         bn_eps (float, optional): BatchNorm epsilon override (model default if ``None``). Default: ``None``.
 
+    Returns:
+        ComposerModel: instance of :class:`.ComposerClassifier` with the specified TIMM model.
+
     Resnet18 Example:
 
     .. testcode::
 
-        from composer.models import Timm
+        from composer.models import composer_timm
 
-        model = Timm(model_name='resnet18')  # creates a timm resnet18
+        model = composer_timm(model_name='resnet18')  # creates a timm resnet18
     """
+    try:
+        import timm
+    except ImportError as e:
+        raise MissingConditionalImportError(extra_deps_group='timm', conda_package='timm>=0.5.4',
+                                            conda_channel=None) from e
+    model = timm.create_model(model_name=model_name,
+                              pretrained=pretrained,
+                              num_classes=num_classes,
+                              drop_rate=drop_rate,
+                              drop_path_rate=drop_path_rate,
+                              drop_block_rate=drop_block_rate,
+                              global_pool=global_pool,
+                              bn_momentum=bn_momentum,
+                              bn_eps=bn_eps)
 
-    def __init__(
-        self,
-        model_name: str,
-        pretrained: bool = False,
-        num_classes: int = 1000,
-        drop_rate: float = 0.0,
-        drop_path_rate: Optional[float] = None,
-        drop_block_rate: Optional[float] = None,
-        global_pool: Optional[str] = None,
-        bn_momentum: Optional[float] = None,
-        bn_eps: Optional[float] = None,
-    ) -> None:
-        try:
-            import timm
-        except ImportError as e:
-            raise MissingConditionalImportError(extra_deps_group='timm',
-                                                conda_package='timm>=0.5.4',
-                                                conda_channel=None) from e
-
-        model = timm.create_model(
-            model_name=model_name,
-            pretrained=pretrained,
-            num_classes=num_classes,
-            drop_rate=drop_rate,
-            drop_path_rate=drop_path_rate,
-            drop_block_rate=drop_block_rate,
-            global_pool=global_pool,
-            bn_momentum=bn_momentum,
-            bn_eps=bn_eps,
-        )
-        super().__init__(module=model)
+    composer_model = ComposerClassifier(module=model)
+    return composer_model
```

### Comparing `mosaicml-0.8.2/composer/models/timm/timm_hparams.py` & `mosaicml-0.9.0/composer/models/timm/timm_hparams.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.Timm`."""
+"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.composer_timm`."""
 
 import textwrap
 from dataclasses import dataclass
 from typing import Optional
 
 import yahp as hp
 
 from composer.models.model_hparams import ModelHparams
-from composer.models.timm.model import Timm
+from composer.models.timm.model import composer_timm
 from composer.utils.import_helpers import MissingConditionalImportError
 
 __all__ = ['TimmHparams']
 
 
 @dataclass
 class TimmHparams(ModelHparams):
-    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.Timm`.
+    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.composer_timm`.
 
     Args:
         model_name (str): timm model name e.g: ``"resnet50"``. List of models can be found at
             `PyTorch Image Models <https://github.com/rwightman/pytorch-image-models>`_.
         pretrained (bool, optional): Imagenet pretrained. Default: ``False``.
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``1000``.
         drop_rate (float, optional): Dropout rate. Default: ``0.0``.
@@ -58,16 +58,16 @@
                                                     conda_package='timm >=0.5.4',
                                                     conda_channel=None) from e
             raise ValueError(f'model must be one of {timm.models.list_models()}')
 
     def initialize_object(self):
         if self.model_name is None:
             raise ValueError('model_name must be specified')
-        return Timm(model_name=self.model_name,
-                    pretrained=self.pretrained,
-                    num_classes=self.num_classes,
-                    drop_rate=self.drop_rate,
-                    drop_path_rate=self.drop_path_rate,
-                    drop_block_rate=self.drop_block_rate,
-                    global_pool=self.global_pool,
-                    bn_momentum=self.bn_momentum,
-                    bn_eps=self.bn_eps)
+        return composer_timm(model_name=self.model_name,
+                             pretrained=self.pretrained,
+                             num_classes=self.num_classes,
+                             drop_rate=self.drop_rate,
+                             drop_path_rate=self.drop_path_rate,
+                             drop_block_rate=self.drop_block_rate,
+                             global_pool=self.global_pool,
+                             bn_momentum=self.bn_momentum,
+                             bn_eps=self.bn_eps)
```

### Comparing `mosaicml-0.8.2/composer/models/transformer_hparams.py` & `mosaicml-0.9.0/composer/models/gpt2/gpt2_hparams.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""YAHP :class:`.hp.Hparams` hyperparameters for ComposerTransformers."""
+"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.GPT2Model`."""
 
-from abc import ABC
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 import yahp as hp
 
 from composer.core.types import JSON
 from composer.models.model_hparams import ModelHparams
 
-__all__ = ['TransformerHparams']
+__all__ = ['GPT2Hparams']
 
 
 @dataclass
-class TransformerHparams(ModelHparams, ABC):
-    """Defines the necessary hyperparameters for a Transformer base module.
+class GPT2Hparams(ModelHparams):
+    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.GPT2Model`.
 
     Args:
-        pretrained_model_name (Optional[str]): "Pretrained model name to pull from Huggingface Model Hub."
-        model_config (Dict[str, JSON]): A dictionary providing a HuggingFace model configuration.
-        tokenizer_name (str): The tokenizer used for this model,
-            necessary to assert required model inputs.
-        use_pretrained (bool, optional): Whether to initialize the model with the pretrained weights. Default: ``False``
+        model_config (Dict[str, JSON], optional ): A dictionary providing a HuggingFace model configuration.
+        pretrained_model_name (str, optional): Pretrained model name to pull from Hugging Face Model Hub.
+        use_pretrained (bool, optional): Whether to initialize the model with the pretrained weights. Default: ``False``.
+        tokenizer_name (str, optional): The tokenizer used for this model,
+            necessary to assert required model inputs. Default ``None``.
         gradient_checkpointing (bool, optional): Use gradient checkpointing. Default: ``False``.
     """
+    model_config: Optional[Dict[str,
+                                JSON]] = hp.optional(doc='A dictionary providing a HuggingFace model configuration.',
+                                                     default_factory=dict)
+    pretrained_model_name: Optional[str] = hp.optional(doc='Pretrained model name to pull from Hugging Face Model Hub.',
+                                                       default=None)
+    use_pretrained: Optional[bool] = hp.optional('Whether to initialize the model with the pretrained weights.',
+                                                 default=False)
+    tokenizer_name: Optional[str] = hp.optional(
+        'The tokenizer used for this model, necessary to assert required model inputs.', default=None)
+    gradient_checkpointing: Optional[bool] = hp.optional('Whether to enable gradient checkpointing.', default=False)
 
-    tokenizer_name: Optional[str] = hp.optional('Tokenizer name to pull from Huggingface Model Hub.', default=None)
-    pretrained_model_name: Optional[str] = hp.optional(
-        doc='Pretrained model name to pull from Huggingface Model Hub.',
-        default=None,
-    )
-    model_config: Dict[str, JSON] = hp.optional(doc='A dictionary providing a HuggingFace model configuration.',
-                                                default_factory=dict)
-    use_pretrained: bool = hp.optional('Whether to initialize the model with the pretrained weights.', default=False)
-    gradient_checkpointing: bool = hp.optional('Whether to enable gradient checkpointing.', default=False)
+    def initialize_object(self):
+        from composer.models.gpt2.model import create_gpt2
 
-    def validate(self):
-        if self.pretrained_model_name is None and self.model_config == {}:
+        # user must specify one of either config or the pretrained model
+        if not self.pretrained_model_name and self.model_config == {}:
             raise Exception('One of pretrained_model_name or model_config needed.')
 
-        if self.pretrained_model_name is not None and self.model_config != {}:
-            raise Exception('Only one of pretrained_model_name or model_config can be provided.')
-
         if self.use_pretrained and self.model_config:
             raise Exception('A model cannot load pretrained weights from configuration.')
+
+        return create_gpt2(
+            model_config=self.model_config,  #type: ignore (thirdparty)
+            pretrained_model_name=self.pretrained_model_name,
+            use_pretrained=self.use_pretrained,
+            tokenizer_name=self.tokenizer_name,
+            gradient_checkpointing=self.gradient_checkpointing,
+        )
```

### Comparing `mosaicml-0.8.2/composer/models/unet/__init__.py` & `mosaicml-0.9.0/composer/models/unet/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/unet/_layers.py` & `mosaicml-0.9.0/composer/models/unet/_layers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/unet/model.py` & `mosaicml-0.9.0/composer/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/unet/unet.py` & `mosaicml-0.9.0/composer/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/unet/unet_hparams.py` & `mosaicml-0.9.0/composer/models/unet/unet_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/models/vit_small_patch16/hparams.py` & `mosaicml-0.9.0/composer/models/vit_small_patch16/hparams.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.ViTSmallPatch16`."""
+"""`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :func:`.vit_small_patch16`."""
 
 from dataclasses import dataclass
 
 import yahp as hp
 
 from composer.models.model_hparams import ModelHparams
 from composer.utils.import_helpers import MissingConditionalImportError
 
 __all__ = ['ViTSmallPatch16Hparams']
 
 
 @dataclass
 class ViTSmallPatch16Hparams(ModelHparams):
-    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.ViTSmallPatch16`.
+    """`YAHP <https://docs.mosaicml.com/projects/yahp/en/stable/README.html>`_ interface for :class:`.vit_small_batch16`.
 
     Args:
         num_classes (int, optional): number of classes for the model. Default: ``1000``.
         image_size (int, optional): input image size. If you have rectangular images, make sure your image
          size is the maximum of the width and height. Default: ``224``.
         channels (int, optional): number of  image channels. Default: ``3``.
         dropout (float, optional): 0.0 - 1.0 dropout rate. Default: ``0``.
@@ -37,13 +37,13 @@
         try:
             import vit_pytorch
         except ImportError as e:
             raise MissingConditionalImportError(extra_deps_group='vit', conda_package='vit_pytorch>=0.27') from e
         del vit_pytorch  # unused
 
     def initialize_object(self):
-        from composer.models import ViTSmallPatch16
-        return ViTSmallPatch16(num_classes=self.num_classes,
-                               image_size=self.image_size,
-                               channels=self.channels,
-                               dropout=self.dropout,
-                               embedding_dropout=self.embedding_dropout)
+        from composer.models import vit_small_patch16
+        return vit_small_patch16(num_classes=self.num_classes,
+                                 image_size=self.image_size,
+                                 channels=self.channels,
+                                 dropout=self.dropout,
+                                 embedding_dropout=self.embedding_dropout)
```

### Comparing `mosaicml-0.8.2/composer/models/vit_small_patch16/model.py` & `mosaicml-0.9.0/composer/models/vit_small_patch16/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Implements ViT-S/16 as a :class:`.ComposerClassifier`."""
 
 from composer.models.tasks import ComposerClassifier
 
-__all__ = ['ViTSmallPatch16']
+__all__ = ['vit_small_patch16']
 
 
-class ViTSmallPatch16(ComposerClassifier):
-    """Implements ViT-S/16 as a :class:`.ComposerClassifier`.
+def vit_small_patch16(num_classes: int = 1000,
+                      image_size: int = 224,
+                      channels: int = 3,
+                      dropout: float = 0.0,
+                      embedding_dropout: float = 0.0):
+    """Helper function to create a :class:`.ComposerClassifier` using a ViT-S/16 model.
 
-    See `Training data-efficient image transformers & distillation through attention <https://arxiv.org/pdf/2012.12877.pdf>`_ (Touvron et al, 2021) for details on ViT-S/16.
+    See `Training data-efficient image transformers & distillation through attention <https://arxiv.org/pdf/2012.12877.pdf>`_
+        (Touvron et al, 2021) for details on ViT-S/16.
 
     Args:
         num_classes (int, optional): number of classes for the model. Default: ``1000``.
         image_size (int, optional): input image size. If you have rectangular images, make sure your image
          size is the maximum of the width and height. Default: ``224``.
         channels (int, optional): number of  image channels. Default: ``3``.
         dropout (float, optional): 0.0 - 1.0 dropout rate. Default: ``0``.
         embedding_dropout (float, optional): 0.0 - 1.0 embedding dropout rate. Default: ``0``.
+
+    Returns:
+        ComposerModel: instance of :class:`.ComposerClassifier` with a ViT-S/16 model.
     """
 
-    def __init__(self,
-                 num_classes: int = 1000,
-                 image_size: int = 224,
-                 channels: int = 3,
-                 dropout: float = 0.0,
-                 embedding_dropout: float = 0.0) -> None:
-        from vit_pytorch import ViT
-        model = ViT(
-            image_size=image_size,
-            channels=channels,
-            num_classes=num_classes,
-            dim=384,  # embed dim/width
-            patch_size=16,
-            depth=12,  # layers
-            heads=6,
-            mlp_dim=1536,
-            dropout=dropout,
-            emb_dropout=embedding_dropout)
-        super().__init__(module=model)
+    from vit_pytorch import ViT
+    model = ViT(
+        image_size=image_size,
+        channels=channels,
+        num_classes=num_classes,
+        dim=384,  # embed dim/width
+        patch_size=16,
+        depth=12,  # layers
+        heads=6,
+        mlp_dim=1536,
+        dropout=dropout,
+        emb_dropout=embedding_dropout)
+
+    composer_model = ComposerClassifier(module=model)
+    return composer_model
```

### Comparing `mosaicml-0.8.2/composer/optim/__init__.py` & `mosaicml-0.9.0/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/optim/decoupled_weight_decay.py` & `mosaicml-0.9.0/composer/optim/decoupled_weight_decay.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,72 @@
 proposes this decoupling. In general, it is recommended to use these optimizers over their native PyTorch equivalents.
 """
 
 from __future__ import annotations
 
 import logging
 import math
-from typing import Iterable, List, Tuple
+from typing import Iterable, List, Tuple, Union
 
 import torch
 from torch.optim import SGD, AdamW
 from torch.optim.optimizer import required  # type: ignore
 
 log = logging.getLogger(__name__)
 
 __all__ = ['DecoupledSGDW', 'DecoupledAdamW']
 
 
 class DecoupledSGDW(SGD):
     """SGD optimizer with the weight decay term decoupled from the learning rate.
 
+    NOTE: Since `weight_decay` is no longer scaled by `lr`, you will likely want to use much smaller values
+    for `weight_decay` than you would if using `torch.optim.SGD`. In this optimizer, the value `weight_decay` translates exactly to:
+    'On every optimizer update, every weight element will be multiplied by `(1.0 - weight_decay_t)`'.
+    The term `weight_decay_t` will follow the same schedule as `lr_t` but crucially will not be scaled by `lr`.
+
     Argument defaults are copied from :class:`torch.optim.SGD`.
 
-    The standard `SGD <https://pytorch.org/docs/stable/generated/torch.optim.SGD.html?highlight=sgd#torch.optim.SGD>`_
+    Why use this optimizer? The standard `SGD <https://pytorch.org/docs/stable/generated/torch.optim.SGD.html?highlight=sgd#torch.optim.SGD>`_
     optimizer couples the weight decay term with the gradient calculation. This ties the optimal value
     of :attr:`weight_decay` to :attr:`lr` and can also hurt generalization in practice. For more details
     on why decoupling might be desirable, see `Decoupled Weight Decay Regularization <https://arxiv.org/abs/1711.05101>`_.
 
     Args:
-        params (list): List of parameters to optimize or dicts defining parameter groups.
-        lr (float, optional): Learning rate.
+        params (iterable): Iterable of parameters to optimize or dicts defining parameter groups.
+        lr (float): Learning rate.
         momentum (int, optional): Momentum factor. Default: ``0``.
         dampening (int, optional): Dampening factor applied to the momentum. Default: ``0``.
         weight_decay (int, optional): Decoupled weight decay factor. Default: ``0``.
         nesterov (bool, optional): Enables Nesterov momentum updates. Default: ``False``.
     """
 
+    def __init__(self,
+                 params: Union[Iterable[torch.Tensor], Iterable[dict]],
+                 lr: float = required,
+                 momentum: float = 0,
+                 dampening: float = 0,
+                 weight_decay: float = 0,
+                 nesterov: bool = False):
+        if weight_decay >= 1e-3:
+            log.warning(
+                f'You are using a high value of `weight_decay={weight_decay}` for the `DecoupledSGDW` optimizer. Are you sure you want to do this? '
+                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!')
+        super().__init__(params=params,
+                         lr=lr,
+                         momentum=momentum,
+                         dampening=dampening,
+                         weight_decay=weight_decay,
+                         nesterov=nesterov)
+        for group in self.param_groups:
+            group['initial_lr'] = group['lr']
+
     @staticmethod
-    def sgdw(params: Iterable[torch.nn.parameter.Parameter], d_p_list: List[torch.Tensor],
-             momentum_buffer_list: List[torch.Tensor], *, weight_decay: float, momentum: float, lr: float,
-             initial_lr: float, dampening: float, nesterov: bool):
+    def sgdw(params: List[torch.Tensor], d_p_list: List[torch.Tensor], momentum_buffer_list: List[torch.Tensor], *,
+             weight_decay: float, momentum: float, lr: float, initial_lr: float, dampening: float, nesterov: bool):
         r"""Functional API that performs SGDW algorithm computation.
 
         Args:
             params (list): List of parameters to update
             d_p_list (list): List of parameter gradients
             momentum_buffer_list (list): List of momentum buffers
             weight_decay (float): Decoupled weight decay factor
@@ -73,30 +97,19 @@
 
                 if nesterov:
                     d_p = d_p.add(buf, alpha=momentum)
                 else:
                     d_p = buf
 
             if weight_decay != 0:
-                decay_factor = lr / initial_lr
+                decay_factor = (lr / initial_lr) if initial_lr else 1.0
                 param.mul_(1 - decay_factor * weight_decay)
 
             param.add_(d_p, alpha=-lr)
 
-    def __init__(self,
-                 params: List[torch.Tensor],
-                 lr: float = required,
-                 momentum: float = 0,
-                 dampening: float = 0,
-                 weight_decay: float = 0,
-                 nesterov: bool = False):
-        super().__init__(params, lr, momentum, dampening, weight_decay, nesterov)
-        for group in self.param_groups:
-            group['initial_lr'] = group['lr']
-
     @torch.no_grad()
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
@@ -145,45 +158,67 @@
 
         return loss
 
 
 class DecoupledAdamW(AdamW):
     """Adam optimizer with the weight decay term decoupled from the learning rate.
 
-    Argument defaults are copied from :class:`torch.optim.AdamW`.
+    NOTE: Since `weight_decay` is no longer scaled by `lr`, you will likely want to use much smaller values
+    for `weight_decay` than you would if using `torch.optim.Adam` or `torch.optim.AdamW`. In this optimizer, the value `weight_decay` translates exactly to:
+    'On every optimizer update, every weight element will be multiplied by `(1.0 - weight_decay_t)`'.
+    The term `weight_decay_t` will follow the same schedule as `lr_t` but crucially will not be scaled by `lr`.
+
+    Argument defaults are similar to :class:`torch.optim.AdamW` but we make two changes:
+    * The default for ``weight_decay`` is changed from ``1e-2`` -> ``1e-5`` because in `DecoupledAdamW`, the weight decay is decoupled and no longer scaled by the `lr=1e-3`.
+    * The default for ``betas`` is changed from ``(0.9, 0.999)`` to ``(0.9, 0.95)`` to reflect community best-practices for the beta2 hyperparameter.
 
-    The standard `AdamW <https://pytorch.org/docs/stable/generated/torch.optim.AdamW.html#torch.optim.AdamW>`_
+    Why use this optimizer? The standard `AdamW <https://pytorch.org/docs/stable/generated/torch.optim.AdamW.html#torch.optim.AdamW>`_
     optimizer explicitly couples the weight decay term with the learning rate. This ties the
     optimal value of :attr:`weight_decay` to :attr:`lr` and can also hurt generalization in practice. For more details on
     why decoupling might be desirable, see `Decoupled Weight Decay Regularization <https://arxiv.org/abs/1711.05101>`_.
 
     Args:
-        params (list): List of parameters to update.
+        params (iterable): Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float, optional): Learning rate. Default: ``1e-3``.
         betas (tuple, optional): Coefficients used for computing running averages of gradient and its square
-                                 Default: ``(0.9, 0.999)``.
+                                 Default: ``(0.9, 0.95)``.
         eps (float, optional): Term added to the denominator to improve numerical stability. Default: ``1e-8``.
-        weight_decay (float, optional): Decoupled weight decay factor. Default: ``1e-2``.
+        weight_decay (float, optional): Decoupled weight decay factor. Default: ``1e-5``.
         amsgrad (bool, optional): Enables the amsgrad variant of Adam. Default: ``False``.
     """
 
+    def __init__(self,
+                 params: Union[Iterable[torch.Tensor], Iterable[dict]],
+                 lr: float = 1e-3,
+                 betas: Tuple[float, float] = (0.9, 0.95),
+                 eps: float = 1e-8,
+                 weight_decay: float = 1e-5,
+                 amsgrad: bool = False):
+        if weight_decay >= 1e-3:
+            log.warning(
+                f'You are using a high value of `weight_decay={weight_decay}` for the `DecoupledAdamW` optimizer. Are you sure you want to do this? '
+                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!')
+        super().__init__(params=params, lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, amsgrad=amsgrad)
+        for group in self.param_groups:
+            group['initial_lr'] = group['lr']
+
     @staticmethod
     def adamw(params: List[torch.Tensor], grads: List[torch.Tensor], exp_avgs: List[torch.Tensor],
               exp_avg_sqs: List[torch.Tensor], max_exp_avg_sqs: List[torch.Tensor], state_steps: List[int], *,
               amsgrad: bool, beta1: float, beta2: float, lr: float, initial_lr: float, weight_decay: float,
               eps: float) -> None:
         r"""Functional API that performs AdamW algorithm computation with decoupled weight decay.
 
         Args:
-            params (List[torch.Tensor]): List of parameters to update.
-            grads (List[torch.Tensor]): List of parameter gradients.
-            exp_avgs (List[torch.Tensor]): List of average gradients.
-            exp_avg_sqs (List[torch.Tensor]): List of average squared gradients.
-            max_exp_avg_sqs (List[torch.Tensor]): List of max average squared gradients for amsgrad updates.
-            state_steps (Iterable[int]): List of steps taken for all parameters.
+            params (list): List of parameters to update.
+            grads (list): List of parameter gradients.
+            exp_avgs (list): List of average gradients.
+            exp_avg_sqs (list): List of average squared gradients.
+            max_exp_avg_sqs (list): List of max average squared gradients for amsgrad updates.
+            state_steps (list): List of steps taken for all parameters.
             amsgrad (bool): Enables amsgrad variant of Adam.
             beta1 (float): Coefficient for computing the moving average of gradient values.
             beta2 (float): Coefficient for computing the moving average of squared gradient values.
             lr (float): Learning rate.
             initial_lr (float): Initial learning rate.
             weight_decay (float): Factor for decoupled weight decay
             eps (float): Term added to the denominator to improve numerical stability.
@@ -192,15 +227,15 @@
             grad = grads[i]
             exp_avg = exp_avgs[i]
             exp_avg_sq = exp_avg_sqs[i]
             step = state_steps[i]
 
             # Perform stepweight decay
             if weight_decay != 0:
-                decay_factor = lr / initial_lr
+                decay_factor = (lr / initial_lr) if initial_lr else 1.0
                 param.mul_(1 - decay_factor * weight_decay)
 
             bias_correction1 = 1 - beta1**step
             bias_correction2 = 1 - beta2**step
 
             # Decay the first and second moment running average coefficient
             exp_avg.mul_(beta1).add_(grad, alpha=1 - beta1)
@@ -213,25 +248,14 @@
             else:
                 denom = (exp_avg_sq.sqrt() / math.sqrt(bias_correction2)).add_(eps)
 
             step_size = lr / bias_correction1
 
             param.addcdiv_(exp_avg, denom, value=-step_size)
 
-    def __init__(self,
-                 params: List[torch.Tensor],
-                 lr: float = 1e-3,
-                 betas: Tuple[float, float] = (0.9, 0.999),
-                 eps: float = 1e-8,
-                 weight_decay: float = 1e-2,
-                 amsgrad: bool = False):
-        super().__init__(params, lr, betas, eps, weight_decay, amsgrad)
-        for group in self.param_groups:
-            group['initial_lr'] = group['lr']
-
     @torch.no_grad()
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
```

### Comparing `mosaicml-0.8.2/composer/optim/optimizer_hparams_registry.py` & `mosaicml-0.9.0/composer/optim/optimizer_hparams_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/optim/scheduler.py` & `mosaicml-0.9.0/composer/optim/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         trainer = Trainer(
             schedulers=[ten_epoch_decay_scheduler],
             ...
         )
 
     The constructions of ``ten_epoch_decay_scheduler`` in each of the examples above are equivalent. Note that neither
     scheduler uses the ``scale_schedule_ratio`` parameter. As long as this parameter is not used when initializing
-    :class:`~composer.trainer.trainer.Trainer`, it is not required that any schedulers implement that parameter.
+    :class:`.Trainer`, it is not required that any schedulers implement that parameter.
 
     .. automethod:: __call__
     """
 
     def __call__(self, state: State, ssr: float = 1.0) -> float:
         r"""Calculate the current learning rate multiplier :math:`\alpha`.
 
@@ -128,21 +128,20 @@
 def _convert_time(time: Union[str, Time[int], Time[float]], state: State, ssr: float = 1.0) -> Time[int]:
     if isinstance(time, str):
         time = Time.from_timestring(time)
 
     assert state.max_duration is not None, 'max_duration should be set whenever schedulers are invoked'
 
     if time.unit == TimeUnit.DURATION:
-        if state.dataloader_len is None:
-            raise RuntimeError('Cannot convert time, as state.dataloader_len is None.')
         if state.max_duration.unit == TimeUnit.EPOCH:
+            if state.dataloader_len is None:
+                raise RuntimeError('Cannot convert time, as state.dataloader_len is None.')
             return Time(int(time.value * int(state.dataloader_len) * state.max_duration.value), TimeUnit.BATCH)
         return Time(int(time.value * state.max_duration.value), state.max_duration.unit)
-
-    if time.unit == TimeUnit.EPOCH:
+    elif time.unit == TimeUnit.EPOCH:
         # Epochs do not provide sufficient granularity for SSR scaling
         # e.g. if max_duration = 1ep, then any SSR would result in a new duration of 0.
         # so, convert the time into batches
         if state.dataloader_len is None:
             raise RuntimeError('Cannot convert time, as state.dataloader_len is None.')
         time = Time(value=time.value * int(state.dataloader_len), unit=TimeUnit.BATCH)
 
@@ -689,15 +688,16 @@
         if state.timestamp < t_warmup:
             if self.scale_warmup:
                 return self.warmup_scheduler(state, ssr)
             return self.warmup_scheduler(state)
 
         t_max = _convert_time(self.t_max, state, ssr=ssr)
         current_time = state.timestamp.get(t_warmup.unit)
-        frac_of_total = min(1.0, ((current_time - t_warmup) / (t_max - t_warmup)).value)
+        frac_of_total = ((current_time - t_warmup) / (t_max - t_warmup)).value if (t_max > t_warmup) else 0.0
+        frac_of_total = min(1.0, frac_of_total)
 
         current_factor = self.alpha_i + frac_of_total * (self.alpha_f - self.alpha_i)
 
         return current_factor
 
 
 class CosineAnnealingWithWarmupScheduler(ComposerScheduler):
@@ -756,15 +756,16 @@
         if state.timestamp < t_warmup:
             if self.scale_warmup:
                 return self.warmup_scheduler(state, ssr)
             return self.warmup_scheduler(state)
 
         t_max = _convert_time(self.t_max, state, ssr=ssr)
         current_time = state.timestamp.get(t_warmup.unit)
-        frac_of_total = ((current_time - t_warmup) / (t_max - t_warmup)).value
+        frac_of_total = ((current_time - t_warmup) / (t_max - t_warmup)).value if (t_max > t_warmup) else 0.0
+        frac_of_total = min(1.0, frac_of_total)
 
         return _cosine_anneal(x=frac_of_total, min_y=self.alpha_f)
 
 
 class PolynomialWithWarmupScheduler(ComposerScheduler):
     r"""Decays the learning rate according to a power of the fraction of training time left, with an initial warmup.
 
@@ -825,12 +826,13 @@
         if state.timestamp < t_warmup:
             if self.scale_warmup:
                 return self.warmup_scheduler(state, ssr)
             return self.warmup_scheduler(state)
 
         t_max = _convert_time(self.t_max, state, ssr=ssr)
         current_time = state.timestamp.get(t_warmup.unit)
-        frac_of_total = ((current_time - t_warmup) / (t_max - t_warmup)).value
+        frac_of_total = ((current_time - t_warmup) / (t_max - t_warmup)).value if (t_max > t_warmup) else 0.0
+        frac_of_total = min(1.0, frac_of_total)
 
         coeff = (1 - frac_of_total)**self.power
         current_factor = self.alpha_f + coeff * (1.0 - self.alpha_f)
         return current_factor
```

### Comparing `mosaicml-0.8.2/composer/optim/scheduler_hparams_registry.py` & `mosaicml-0.9.0/composer/optim/scheduler_hparams_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/profiler/__init__.py` & `mosaicml-0.9.0/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/profiler/json_trace_handler.py` & `mosaicml-0.9.0/composer/profiler/json_trace_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         artifact_name (str, optional): Format string for the trace file's artifact name.
             (default: ``'{{run_name}}/traces/ep{{epoch}}-ba{{batch}}-rank{{rank}}.json'``)
 
             Whenever a trace file is saved, it is also logged as a file artifact according to this format string.
             The same format variables as for ``filename`` are available.
 
-            .. seealso:: :meth:`~composer.loggers.logger.Logger.file_artifact` for file artifact logging.
+            .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
 
             Leading slashes (``'/'``) will be stripped.
 
             To disable logging trace files as file artifacts, set this parameter to ``None``.
 
         merged_trace_filename (str, optional): Format string for the merged trace filename.
             (default: ``'node{{node_rank}}.json'``)
@@ -121,15 +121,15 @@
             If ``False``, the :meth:`trace_folder` (as determined by the ``trace_folder`` argument)
             must be empty when training starts.
 
         num_traces_to_keep (int, optional): The number of traces to keep locally. The oldest traces
             are removed first. Set to ``-1`` to keep all traces locally. (default: ``-1``)
 
             Traces will be removed after they have been logged as a file artifact. For example, when this handler
-            is used in conjunction with the :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`, set this
+            is used in conjunction with the :class:`.ObjectStoreLogger`, set this
             parameter to ``0`` to immediately delete traces from the local disk after they have been uploaded to
             the object store.
 
             This parameter only controls how many traces are kept locally; traces are not deleted from
             artifact stores.
 
     Attributes:
```

### Comparing `mosaicml-0.8.2/composer/profiler/json_trace_merger.py` & `mosaicml-0.9.0/composer/profiler/json_trace_merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,32 @@
 
 def merge_traces(output_file: Union[str, pathlib.Path], *trace_files: Union[str, pathlib.Path]):
     """Merge profiler output JSON trace files together.
 
     This function will update the trace events such that:
 
     - The ``pid`` will be set to the global rank.
-    - The ``ts`` is syncronized with that of the rank 0 process.
+    - The ``ts`` is synchronized with that of the rank 0 process.
     - The backward pass process appears below the forward process.
 
     Args:
         output_file (str | pathlib.Path): The file to write the merged trace to
         trace_files (str | pathlib.Path): Variable number of trace files to merge together
     """
     ranks_to_clock_sync = _get_rank_to_clock_syncs(trace_files)
     rank_to_backwards_thread = {}
     rank_to_seen_threads = {rank: set() for rank in ranks_to_clock_sync.keys()}
 
-    rank_zero_clock_sync = ranks_to_clock_sync[0]
+    # Local rank zero will be the lowest global rank
+    # Use that as the base timestamp for clock syncing
+    lowest_rank = float('inf')
+    for k in ranks_to_clock_sync:
+        lowest_rank = min(k, lowest_rank)
+    assert isinstance(lowest_rank, int), 'there should be at least one rank'
+    rank_zero_clock_sync = ranks_to_clock_sync[lowest_rank]
 
     with open(output_file, 'w+') as output_f:
         is_first_line = True
         output_f.write('[')
         for trace_filename in trace_files:
             rank = _get_global_rank_from_file(trace_filename)
             clock_sync_diff = rank_zero_clock_sync - ranks_to_clock_sync[rank]
```

### Comparing `mosaicml-0.8.2/composer/profiler/marker.py` & `mosaicml-0.9.0/composer/profiler/marker.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __all__ = ['Marker']
 
 
 class Marker:
     """Profiler Marker.
 
-    Used by the :class:`~composer.core.engine.Engine` to measure the duration of :class:`~composer.core.event.Event` during training.
+    Used by the :class:`.Engine` to measure the duration of :class:`.Event` during training.
 
     .. note::
 
         :class:`.Marker` should not be instantiated directly; instead use :meth:`.Profiler.marker`.
 
     Markers can record the following types of events:
```

### Comparing `mosaicml-0.8.2/composer/profiler/profiler.py` & `mosaicml-0.9.0/composer/profiler/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         self,
         state: State,
     ):
         """Bind the profiler to the ``state``.
 
         .. note::
 
-            The :class:`~composer.trainer.trainer.Trainer` automatically invokes this method.
+            The :class:`.Trainer` automatically invokes this method.
 
         Args:
             state (State): The training state.
         """
         self.state = state
         self.state.callbacks.extend(self._callbacks)
         self.state.callbacks.extend(self._trace_handlers)
```

### Comparing `mosaicml-0.8.2/composer/profiler/profiler_action.py` & `mosaicml-0.9.0/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/profiler/profiler_hparams.py` & `mosaicml-0.9.0/composer/profiler/profiler_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/profiler/profiler_schedule.py` & `mosaicml-0.9.0/composer/profiler/profiler_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     warmup: int = 1,
     active: int = 4,
     repeat: int = 1,
 ) -> Callable[[State], ProfilerAction]:
     """Profiler schedule function for a cyclic profiling window.
 
     This function returns a schedule function that uses a cyclic profiling window. The resulting function can be
-    passed as the ``prof_schedule`` argument to the :class:`~composer.trainer.trainer.Trainer`.
+    passed as the ``prof_schedule`` argument to the :class:`.Trainer`.
 
     The cyclic window skips the first ``skip_first`` batches in every epoch. Then, it performs a cycle of
     skipping ``wait`` batches, warming up for ``warmup`` batches, and recording ``active`` batches.
     It repeats this cycle up to ``repeat`` times per epoch (or for the entire epoch, if ``repeat`` is 0).
     This logic repeats every epoch.
 
     Args:
@@ -35,15 +35,15 @@
         warmup (int, optional): For each profiling cycle, number of batches to be in the warmup state after skipping
             ``wait`` batches. Defaults to ``1``.
         active (int, optional): For each profiling cycle, number of batches to record after warming up.  Defaults to ``4``.
         repeat (int, optional): Number of profiling cycles to perform per epoch. Set to ``0`` to record the entire epoch.
             Defaults to ``1``.
 
     Returns:
-        (State -> ProfilerAction): A ``prof_schedule`` for the :class:`~composer.trainer.trainer.Trainer`.
+        (State -> ProfilerAction): A ``prof_schedule`` for the :class:`.Trainer`.
     """
 
     def schedule(state: State):
         # do wait, then warump, then active, up to repeat times per cycle
         cycle_len = wait + warmup + active
         batch_idx = int(state.timestamp.batch_in_epoch)
         if batch_idx < skip_first:
```

### Comparing `mosaicml-0.8.2/composer/profiler/system_profiler.py` & `mosaicml-0.9.0/composer/profiler/system_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 
 class SystemProfiler(Callback):
     """The SystemProfiler records system level metrics.
 
     .. note::
 
-        The Composer :class:`~composer.trainer.trainer.Trainer` automatically creates an instance of this
+        The Composer :class:`.Trainer` automatically creates an instance of this
         :class:`.SystemProfiler` callback whenever any of the System Profiler arguments (``sys_prof_cpu``,
         ``sys_prof_memory``, ``sys_prof_disk``, or ``sys_prof_net``) are enabled.
 
-        When using the Composer :class:`~composer.trainer.trainer.Trainer`, one does not need to directly create an
+        When using the Composer :class:`.Trainer`, one does not need to directly create an
         instance of this :class:`.SystemProfiler` callback.
 
     Args:
         profile_cpu (bool): Whether to record cpu statistics (Default: ``True``)
         profile_memory (bool): Whether to record memory statistics (Default: ``False``)
         profile_disk (bool): Whether to record disk I/O statistics (Default: ``False``)
         profile_net (bool): Whether to record network I/O statistics (Default: ``False``)
```

### Comparing `mosaicml-0.8.2/composer/profiler/torch_profiler.py` & `mosaicml-0.9.0/composer/profiler/torch_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 class TorchProfiler(Callback):  # noqa: D101
     __doc__ = f"""Profile the execution using the :class:`PyTorch Profiler <torch.profiler.profile>`.
 
     Profiling results are stored in TensorBoard format in the directory specified by ``folder``.
 
     .. note::
 
-        The Composer :class:`~composer.trainer.trainer.Trainer` automatically creates an instance of this
+        The Composer :class:`.Trainer` automatically creates an instance of this
         :class:`.TorchProfiler` callback whenever any of the PyTorch Profiler arguments
         (``torch_prof_record_shapes``, ``torch_prof_profile_memory``, ``torch_prof_with_stack``, or
         ``torch_prof_with_flops``) are enabled.
 
-        When using the Composer :class:`~composer.trainer.trainer.Trainer`, one does not need to directly create an
+        When using the Composer :class:`.Trainer`, one does not need to directly create an
         instance of this :class:`.TorchProfiler` callback.
 
 
     To view profiling results, run::
 
         pip install tensorbaord torch_tb_profiler
         tensorboard --logdir path/to/torch/trace_folder
@@ -96,15 +96,15 @@
 
         artifact_name (str, optional): Format string for a Torch Profiler trace file's artifact name.
             Defaults to ``'{{run_name}}/torch_traces/rank{{rank}}.{{batch}}.pt.trace.json'``.
 
             Whenever a trace file is saved, it is also logged as a file artifact according to this format string.
             The same format variables as for ``filename`` are available.
 
-            .. seealso:: :meth:`~composer.loggers.logger.Logger.file_artifact` for file artifact logging.
+            .. seealso:: :doc:`Artifact Logging</trainer/artifact_logging>` for notes for file artifact logging.
 
             Leading slashes (``'/'``) will be stripped.
 
             To disable logging trace files as file artifacts, set this parameter to ``None``.
         overwrite (bool, optional): Whether to override existing Torch Profiler traces. Defaults to False.
 
             If False, then the trace folder as determined by ``folder`` must be empty.
@@ -120,15 +120,15 @@
             If set to -1, then all traces files are kept locally.
 
             After a trace has been saved and logged as a file artifact, the oldest traces are removed until
             ``num_traces_to_keep`` traces remain. This parameter only controls how many traces are kept locally;
             traces are not deleted from artifact stores.
 
             It can be useful to set this parameter to ``0`` when using an artifact logger such as the
-            :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`. This combination will minimize local
+            :class:`.ObjectStoreLogger`. This combination will minimize local
             disk usage by deleting trace files immediately after they have been uploaded to the object store.
 
     Attributes:
         saved_traces (List[Tuple[Timestamp, List[pathlib.Path]]]): The trace timestamps and filepaths.
 
             This list contains tuples of the save timestamp and the trace filepaths.
             This list will have at most ``num_traces_to_keep`` entries. The latest trace
```

### Comparing `mosaicml-0.8.2/composer/profiler/trace_handler.py` & `mosaicml-0.9.0/composer/profiler/trace_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class TraceHandler(Callback, abc.ABC):
     """Base class for Composer Profiler trace handlers.
 
     Subclasses should implement :meth:`process_duration_event`, :meth:`process_instant_event`,
     :meth:`process_counter_event`, and :meth:`process_chrome_json_trace_file` to record trace events.
 
-    Since :class:`TraceHandler` subclasses :class:`~composer.core.callback.Callback`, a trace handler can run on any
+    Since :class:`TraceHandler` subclasses :class:`.Callback`, a trace handler can run on any
     :class:`.Event` (such as on :attr:`.Event.INIT` to open files or on :attr:`.Event.BATCH_END` to periodically dump
     data to files) and use :meth:`.Callback.close` to perform any cleanup.
     """
 
     def process_duration_event(
         self,
         name: str,
```

### Comparing `mosaicml-0.8.2/composer/trainer/_deepspeed.py` & `mosaicml-0.9.0/composer/trainer/_deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     Args:
         config (Dict[str, Any]): The DeepSpeed config to use. Must follow the format specified
             in `DeepSpeed's documentation <https://www.deepspeed.ai/docs/config-json/>`_.
         state (State): The state of the trainer.
 
     Returns:
         Dict[str, Any]: The DeepSpeed config updated with values from the arguments passed to the
-            :class:`~composer.trainer.trainer.Trainer`.
+            :class:`.Trainer`.
 
     Raises:
         ValueError: If any of the values in the DeepSpeed config conflict with arguments passed
             to the trainer.
         RuntimeError: If the batch size of the train dataloader in the provided state is not set.
     """
     new_config = copy.deepcopy(config)
```

### Comparing `mosaicml-0.8.2/composer/trainer/_scale_schedule.py` & `mosaicml-0.9.0/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/trainer/_scaler.py` & `mosaicml-0.9.0/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/trainer/ddp.py` & `mosaicml-0.9.0/composer/trainer/ddp.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 @contextmanager
 def ddp_sync_context(state: State, is_final_microbatch: bool, sync_strategy: Union[str, DDPSyncStrategy]):
     """A context manager for handling the :class:`DDPSyncStrategy`.
 
     Args:
-        state (State): The state of the :class:`~composer.trainer.trainer.Trainer`.
+        state (State): The state of the :class:`.Trainer`.
         is_final_microbatch (bool): Whether or not the context is being used during the final
             microbatch of the gradient accumulation steps.
         sync_strategy (str | DDPSyncStrategy): The ddp sync strategy to use. If a string
             is provided, the string must be one of the values in :class:`DDPSyncStrategy`.
     """
     if not isinstance(state.model, DistributedDataParallel):
         yield
```

### Comparing `mosaicml-0.8.2/composer/trainer/devices/device.py` & `mosaicml-0.9.0/composer/trainer/devices/device.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/trainer/devices/device_cpu.py` & `mosaicml-0.9.0/composer/trainer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/trainer/devices/device_gpu.py` & `mosaicml-0.9.0/composer/trainer/devices/device_gpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional, TypeVar
 
 import torch
 import torch.backends.cuda
 import torch.backends.cudnn
+import torch.cuda
 import torch.cuda.amp
 import torch.utils.data
 
 from composer.trainer.devices.device import Device
 from composer.utils import dist
 
 __all__ = ['DeviceGPU']
```

### Comparing `mosaicml-0.8.2/composer/trainer/devices/device_hparams_registry.py` & `mosaicml-0.9.0/composer/trainer/devices/device_hparams_registry.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from typing import Dict, Type, Union
 
 import yahp as hp
 
 from composer.trainer.devices.device import Device
 from composer.trainer.devices.device_cpu import DeviceCPU
 from composer.trainer.devices.device_gpu import DeviceGPU
+from composer.trainer.devices.device_mps import DeviceMPS
+from composer.trainer.devices.device_tpu import DeviceTPU
 
 __all__ = ['device_registry']
 
 device_registry: Dict[str, Union[Type[Device], Type[hp.Hparams]]] = {
     'gpu': DeviceGPU,
     'cpu': DeviceCPU,
+    'mps': DeviceMPS,
+    'tpu': DeviceTPU,
 }
```

### Comparing `mosaicml-0.8.2/composer/trainer/trainer.py` & `mosaicml-0.9.0/composer/trainer/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,44 @@
 import time
 import warnings
 from typing import Any, Callable, ContextManager, Dict, Iterable, List, Optional, Sequence, TextIO, Tuple, Union, cast
 
 import coolname
 import torch
 import torch.distributed
+import torch.nn as nn
 import torch.utils.data
 from torch.cuda.amp.grad_scaler import GradScaler
 from torch.nn.parallel import DistributedDataParallel
 from torch.utils.data import DataLoader, DistributedSampler
 from torchmetrics import Metric, MetricCollection
 
 from composer.algorithms import GradientClipping
 from composer.callbacks import CheckpointSaver
 from composer.core import (Algorithm, Callback, DataSpec, Engine, Evaluator, Event, Precision, State, Time, Timestamp,
                            ensure_data_spec, ensure_evaluator, ensure_time)
 from composer.core.precision import get_precision_context
 from composer.core.time import TimeUnit
-from composer.core.types import Batch, BreakEpochException, PyTorchScheduler
+from composer.core.types import Batch, PyTorchScheduler, TrainerMode
 from composer.loggers import Logger, LoggerDestination, LogLevel, ProgressBarLogger
 from composer.models.base import ComposerModel
 from composer.optim.decoupled_weight_decay import DecoupledSGDW
 from composer.optim.scheduler import ComposerScheduler, compile_composer_scheduler
 from composer.profiler import Profiler
 from composer.trainer._deepspeed import _fix_batch_precision_for_deepspeed, _parse_deepspeed_config
 from composer.trainer._scale_schedule import scale_pytorch_scheduler
 from composer.trainer._scaler import ClosureGradScaler
 from composer.trainer.ddp import DDPSyncStrategy, ddp_sync_context, prepare_ddp_module
-from composer.trainer.devices import Device, DeviceCPU, DeviceGPU
-from composer.utils import (ObjectStore, dist, ensure_tuple, format_name_with_dist, map_collection, module_surgery,
+from composer.trainer.devices import Device, DeviceCPU, DeviceGPU, DeviceMPS, DeviceTPU
+from composer.utils import (ObjectStore, dist, ensure_tuple, format_name_with_dist, is_model_deepspeed, map_collection,
                             reproducibility)
 from composer.utils.checkpoint import load_checkpoint, save_checkpoint
 from composer.utils.file_helpers import get_file
 from composer.utils.import_helpers import MissingConditionalImportError
+from composer.utils.inference import ExportFormat, Transform, export_with_logger
 
 log = logging.getLogger(__name__)
 
 __all__ = ['Trainer']
 
 # syntax to shorten the Scheduler type annoations
 Scheduler = Union[ComposerScheduler, PyTorchScheduler]
@@ -166,16 +168,24 @@
     if not device:
         device = DeviceGPU() if torch.cuda.is_available() else DeviceCPU()
     elif isinstance(device, str):
         if device.lower() == 'cpu':
             device = DeviceCPU()
         elif device.lower() == 'gpu':
             device = DeviceGPU()
+        elif device.lower() == 'mps':
+            device = DeviceMPS()
+        elif device.lower() == 'tpu':
+            if not _is_tpu_installed():
+                raise ImportError(
+                    'Unable to import torch_xla. Please follow installation instructions at https://github.com/pytorch/xla'
+                )
+            device = DeviceTPU()
         else:
-            raise ValueError(f'device ({device}) must be one of (cpu, gpu).')
+            raise ValueError(f'device ({device}) must be one of (cpu, gpu, mps, tpu).')
     return device
 
 
 def _distribute_and_get_random_seed(seed: Optional[int], device: Device):
     if not seed:
         seed = reproducibility.get_random_seed()
 
@@ -212,14 +222,29 @@
     run_name_list = [generated_run_name]
     # ensure all ranks have the same experiment name
     dist.broadcast_object_list(run_name_list)
     generated_run_name = run_name_list[0]
     return generated_run_name
 
 
+def _is_tpu_installed() -> bool:
+    try:
+        import torch_xla.core.xla_model as xm
+        del xm
+    except ImportError:
+        return False
+    else:
+        return True
+
+
+if _is_tpu_installed():
+    import torch_xla.core.xla_model as xm
+    import torch_xla.distributed.parallel_loader as pl
+
+
 class Trainer:
     """Train models with Composer algorithms.
 
     The trainer supports models with :class:`~composer.models.base.ComposerModel` instances.
     The :class:`.Trainer` is highly customizable and can support a wide variety of workloads.
     See the :doc:`training guide</trainer/using_the_trainer>` for more information.
 
@@ -532,33 +557,33 @@
             .. note::
 
                 For fine-grained control on checkpoint saving (e.g. to save different types of checkpoints
                 at different intervals), leave this parameter as ``None``, and instead pass
                 instance(s) of :class:`~.CheckpointSaver` directly as ``callbacks``.
         save_filename (str, optional): A format string describing how to name checkpoints.
             This parameter has no effect if ``save_folder`` is ``None``.
-            (default: ``"ep{epoch}-ba{batch}-rank{rank}"``)
+            (default: ``"ep{epoch}-ba{batch}-rank{rank}.pt"``)
 
             .. seealso:: :class:`~.CheckpointSaver`
         save_artifact_name (str, optional): A format string describing how to name checkpoints in loggers.
             This parameter has no effect if ``save_folder`` is ``None``.
             (default: ``"{run_name}/checkpoints/ep{epoch}-ba{batch}-rank{rank}"``)
 
-            .. seealso:: :class:`~.CheckpointSaver`
+            .. seealso:: :class:`~.CheckpointSaver` and :doc:`Artifact Logging</trainer/artifact_logging>` notes.
         save_latest_filename (str, optional): A format string for the name of a symlink
             (relative to ``save_folder``) that points to the last saved checkpoint.
             This parameter has no effect if ``save_folder`` is ``None``.
-            To disable symlinking, set this to ``None``. (default: ``"latest-rank{rank}"``)
+            To disable symlinking, set this to ``None``. (default: ``"latest-rank{rank}.pt"``)
 
             .. seealso:: :class:`~.CheckpointSaver`
         save_latest_artifact_name (str, optional): A format string describing how to name symlinks in loggers.
             This parameter has no effect if ``save_folder``, ``save_latest_filename``, or ``save_artifact_name`` are ``None``.
             To disable symlinking in logger, set this or ``save_latest_filename`` to ``None``. (default: ``"{run_name}/checkpoints/latest-rank{rank}"``)
 
-            .. seealso:: :class:`~.CheckpointSaver`
+            .. seealso:: :class:`~.CheckpointSaver` and :doc:`Artifact Logging</trainer/artifact_logging>` notes.
         save_overwrite (bool, optional): Whether existing checkpoints should be overridden.
             This parameter has no effect if ``save_folder`` is None. (default: ``False``)
 
             .. seealso:: :class:`~.CheckpointSaver`
         save_interval (Time | str | int | (State, Event) -> bool): A :class:`Time`, time-string, integer (in epochs),
             or a function that takes (state, event) and returns a boolean whether a checkpoint should be saved.
             This parameter has no effect if ``save_folder`` is ``None``. (default: ``'1ep'``)
@@ -568,15 +593,15 @@
             state. This parameter has no effect if ``save_folder`` is ``None``. (default: ``False``)
 
             .. seealso:: :class:`~.CheckpointSaver`
         save_num_checkpoints_to_keep (int, optional): The number of checkpoints to keep locally. The oldest checkpoints
             are removed first. Set to ``-1`` to keep all checkpoints locally. (default: ``-1``)
 
             Checkpoints will be removed after they have been logged as a file artifact. For example, when this callback
-            is used in conjunction with the :class:`~composer.loggers.object_store_logger.ObjectStoreLogger`, set this
+            is used in conjunction with the :class:`.ObjectStoreLogger`, set this
             parameter to ``0`` to immediately delete checkpoints from the local disk after they have been uploaded to
             the object store.
 
             This parameter only controls how many checkpoints are kept locally; checkpoints are not deleted from
             artifact stores.
         autoresume (bool, optional): Whether or not to enable autoresume, which allows for stopping and resuming
         training. This allows use of spot instances, as the training run is now fault tolerant.  This parameter requires
@@ -592,19 +617,18 @@
             checkpoint. For any future restarts, such as due to the spot instance being killed, the loggers would be queried for the latest checkpoint
             the object store logger would be downloaded and used to resume training.
         deepspeed_config (Dict[str, Any], optional): Configuration for DeepSpeed, formatted as a JSON
             according to `DeepSpeed's documentation <https://www.deepspeed.ai/docs/config-json/>`_. (default: ``None``)
 
             To use DeepSpeed with default values, set to the empty dictionary ``{}``.
             To disable DeepSpeed (the default), set to ``None``.
-        device (Device | str, optional): The device to use for training, which can be ``'cpu'`` or ``'gpu'``.
-            (default: ``None``)
+        device (Device | str, optional): The device to use for training, which can be ``'cpu'``, ``'gpu'``,
+            ``'tpu'``, or ``'mps'``. (default: ``None``)
 
-            The default behavior sets the device to ``'gpu'`` if CUDA is available; otherwise, it sets the device to
-            ``'cpu'``.
+            The default behavior sets the device to ``'gpu'`` if CUDA is available, and otherwise ``'cpu'``.
         precision (Precision | str, optional): Numerical precision to use for training. One of ``fp32``, ``fp16``
             or ``amp`` (recommended). (default: ``Precision.FP32`` if training on CPU; ``Precision.AMP`` if training
             on GPU)
 
             .. note::
                 ``fp16`` only works if ``deepspeed_config`` is also provided.
         grad_accum (Union[int, str], optional): The number of microbatches to split a per-device batch into. Gradients
@@ -704,17 +728,17 @@
         load_weights_only: bool = False,
         load_strict_model_weights: bool = False,
         load_progress_bar: bool = True,
         load_ignore_keys: Optional[Union[List[str], Callable[[Dict], None]]] = None,
 
         # Save Checkpoint
         save_folder: Optional[str] = None,
-        save_filename: str = 'ep{epoch}-ba{batch}-rank{rank}',
+        save_filename: str = 'ep{epoch}-ba{batch}-rank{rank}.pt',
         save_artifact_name: str = '{run_name}/checkpoints/ep{epoch}-ba{batch}-rank{rank}',
-        save_latest_filename: Optional[str] = 'latest-rank{rank}',
+        save_latest_filename: Optional[str] = 'latest-rank{rank}.pt',
         save_latest_artifact_name: Optional[str] = '{run_name}/checkpoints/latest-rank{rank}',
         save_overwrite: bool = False,
         save_interval: Union[str, int, Time, Callable[[State, Event], bool]] = '1ep',
         save_weights_only: bool = False,
         save_num_checkpoints_to_keep: int = -1,
 
         # Graceful Resumption
@@ -750,46 +774,64 @@
         # Device
         self._device = _get_device(device)
 
         # Distributed
         if deepspeed_enabled or dist.get_world_size() > 1:
             # deepspeed requires torch.distributed to be initialized, even if the world size is 1
             # distributed is always required with multi-rank training
-            dist.initialize_dist(self._device.dist_backend, datetime.timedelta(seconds=dist_timeout))
+            dist.initialize_dist(self._device, datetime.timedelta(seconds=dist_timeout))
 
         # Reproducibility
         rank_zero_seed, seed = _distribute_and_get_random_seed(seed, self._device)
         # If hparams is used to create the Trainer this function is called twice
         # which is okay because all runs with the hparams codepath will do this
         reproducibility.seed_all(seed)
         if deterministic_mode:
             reproducibility.configure_deterministic_mode()
 
         # Precision
         if precision is None:
-            precision = Precision.AMP if isinstance(device, DeviceGPU) else Precision.FP32
+            precision = Precision.AMP if isinstance(self._device, DeviceGPU) else Precision.FP32
         if isinstance(precision, str):
             precision = Precision(precision)
 
         _validate_precision(precision, self._device, deepspeed_enabled)
 
-        # optimizers and schedulers
+        # Optimizers and Schedulers
         if not optimizers:
             optimizers = DecoupledSGDW(list(model.parameters()), lr=0.1)
             # hard-coding the optimizer in the warning, as repr(optimizers) would print an annoying, multi-line warning
             warnings.warn(('No optimizer was specified. Defaulting to '
                            f"{type(optimizers).__name__}(lr={optimizers.defaults['lr']})"))
 
         num_optimizers = len(ensure_tuple(optimizers))
         if num_optimizers != 1:
             raise NotImplementedError(f'Only one optimizer is supported; found {num_optimizers} optimizers')
 
+        # Move the model and optimizers to the device
+
+        if not deepspeed_enabled:
+            # check if model is already on tpu
+            if isinstance(self._device, DeviceTPU) and 'xla' not in str(next(model.parameters()).device):
+                raise ValueError(
+                    'Use model.to(xm.xla_device()) to set the model to the TPU before providing to the trainer.')
+            else:
+                model = self._device.module_to_device(model)
+                # Move any remaining optimizer parameters onto the device
+                # It is possible that optimizer initialize created some internal tensors on CPU
+                # that need to be moved onto GPU.
+            optimizers = map_collection(optimizers, self._device.optimizer_to_device)
+
         # Grad Accum
         self.adaptive_gradient_accumulation = _is_adaptive_grad_accum(grad_accum, device=self._device)
         grad_accum = _get_initial_grad_accum(grad_accum)
+        if self.adaptive_gradient_accumulation and isinstance(self._device, DeviceTPU):
+            raise NotImplementedError(f'grad_accum=auto not supported on TPUs.')
+        # Dynamic time estimate for forward and backward pass. Used for monitored_barrier to avoid deadlocks
+        self.batch_compute_time = 300
 
         # Grad Clip Norm
         if grad_clip_norm > 0:
 
             warnings.warn(
                 DeprecationWarning((f"Using the 'grad_clip_norm' field in Trainer is deprecated. Please use"
                                     'the GradientClipping Algorithm in composer.algorithms.gradient_clipping.')))
@@ -879,15 +921,18 @@
         # Setting these attributes here ensures that algorithms do not depend on unavailable attributes during Event.INIT
 
         # Train Dataloader
         self._train_data_spec = None if train_dataloader is None else ensure_data_spec(train_dataloader)
         if self._train_data_spec is not None:
             self.state.set_dataloader(self._train_data_spec.dataloader, train_dataloader_label,
                                       train_subset_num_batches)
-            self.state.train_dataloader = self.state.dataloader
+            if isinstance(self._device, DeviceTPU):
+                self.state.train_dataloader = pl.MpDeviceLoader(self.state.dataloader, xm.xla_device())
+            else:
+                self.state.train_dataloader = self.state.dataloader
         self.train_metrics = _get_training_metrics(model) if compute_training_metrics else None
 
         # Max Duration
         if max_duration is not None:
             self.state.max_duration = ensure_time(max_duration, TimeUnit.EPOCH)
 
         self.logger.data_fit({'rank_zero_seed': rank_zero_seed})
@@ -920,21 +965,21 @@
                 subset_num_batches=eval_subset_num_batches,
             )
         if len(evaluators) == 0:
             if eval_subset_num_batches != -1:
                 raise ValueError('Specifying `eval_subset_num_batches` without an `eval_dataloader` has no effect.')
             if eval_interval != 1:
                 raise ValueError('Specifying `eval_interval` without an `eval_dataloader` has no effect.')
+
         self.state.evaluators = evaluators
 
         # Some algorithms require specific settings
         self._backwards_create_graph = any(map(lambda x: x.backwards_create_graph, ensure_tuple(algorithms)))
         self._find_unused_parameters = any(map(lambda x: x.find_unused_parameters, ensure_tuple(algorithms)))
         self._ddp_sync_strategy = _get_ddp_sync_strategy(ddp_sync_strategy, self._find_unused_parameters)
-
         # Configure Deepspeed
         if self.state.deepspeed_config is not None:
             try:
                 import deepspeed
             except ImportError as e:
                 raise MissingConditionalImportError(
                     extra_deps_group='deepspeed',
@@ -960,14 +1005,19 @@
             if 'optimizers' in self.state.serialized_attributes:
                 self.state.serialized_attributes.remove('optimizers')
 
         # If using DeepSpeed, the model must be loaded from checkpoint after the engine has been
         # initialized, but if using PyTorch DDP, the model must be loaded before it is wrapped with
         # DDP.
 
+        # surpressing GradScaler warnings as they are always created
+        # self._use_grad_scaling() will raise a RuntimeError if grad scaling is not available when it is required
+        warnings.filterwarnings(action='ignore', message='torch.cuda.amp.GradScaler')
+        self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
+
         # Load Checkpoint
         self._rng_state = None
         # If autoresume is enabled, first check for existing checkpoints to load
         if autoresume:
             log.info('Searching for a previous checkpoint to autoresume')
             if save_folder is None:
                 raise ValueError('The `save_folder` must be specified when autoresume is enabled.')
@@ -1020,39 +1070,25 @@
         # parameters are initialized randomly, rng state will change. This reseeding nullifies such effects.
         # 2. While resuming from a checkpoint, we want to spin dataloader and bring it back to the same state as at the time
         # of the checkpoint. Therefore, spinning needs to start from the same rng state as in the original run.
         log.info(f'Setting seed to {self.state.seed}')
         reproducibility.seed_all(self.state.seed)
 
         # Move the model and optimizers to the specified device
-        if not self.deepspeed_enabled:
-            host_model_params = self.state.model.parameters()
-            self.state.model = self._device.module_to_device(self.state.model)
-            device_model_params = self.state.model.parameters()
-
-            # use surgery to update the parameters of the optimizers, now that the model is on the device
-            # see https://pytorch.org/docs/stable/optim.html#constructing-it
-            module_surgery.replace_params_in_optimizer(old_params=host_model_params,
-                                                       new_params=device_model_params,
-                                                       optimizers=self.state.optimizers)
-
-            # Move any remaining optimizer parameters onto the device
-            self.state.optimizers = map_collection(self.state.optimizers, self._device.optimizer_to_device)
-
-            if dist.get_world_size() > 1:
-                # Only wrap the module if required
-                self.state.model = prepare_ddp_module(self.state.model, self._find_unused_parameters)
+        if not self.deepspeed_enabled and dist.get_world_size() > 1:
+            # Only wrap the module if required
+            self.state.model = prepare_ddp_module(self.state.model, self._find_unused_parameters)
 
     @property
     def deepspeed_enabled(self):
         """Whether DeepSpeed is enabled.
 
         .. seealso:: `DeepSpeed's documentation <https://www.deepspeed.ai/docs/config-json/>`_
         """
-        return self.state.is_model_deepspeed
+        return is_model_deepspeed(self.state.model)
 
     @property
     def saved_checkpoints(self) -> List[Tuple[Timestamp, List[pathlib.Path]]]:
         """The checkpoint timestamps and filepaths.
 
         This list contains tuples of the save timestamp and the checkpoint filepaths.
         This list will have at most ``save_num_checkpoints_to_keep`` entries. The latest checkpoint
@@ -1334,21 +1370,23 @@
 
         # Grad Accum
         if grad_accum is not None:
             self.adaptive_gradient_accumulation = _is_adaptive_grad_accum(grad_accum, device=self._device)
             self.state.grad_accum = _get_initial_grad_accum(grad_accum)
 
         # Precision
-        if precision is not None:
+        if precision is not None and Precision(precision) != self.state.precision:
             if self.deepspeed_enabled:
                 raise ValueError('Changing the precision when using DeepSpeed is not supported')
             precision = Precision(precision)
             _validate_precision(precision, self._device, self.deepspeed_enabled)
             self.state.precision = precision
 
+            # update scaler since precision was provided
+            self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
         self._train_loop()
 
     def close(self):
         """Shutdown the trainer.
 
         .. seealso:: :meth:`.Engine.close` for additional information.
         """
@@ -1417,37 +1455,33 @@
 
         Returns a (num_samples, num_tokens, batch_time) tuple.
         """
         # Samples and tokens should be summed
         # Batch time should be the value from rank 0
         sample_token_tensor = self._device.tensor_to_device(torch.tensor([num_samples, num_tokens], dtype=torch.int))
         dist.all_reduce(sample_token_tensor, reduce_operation='SUM')
-
         batch_time_tensor = self._device.tensor_to_device(
-            torch.tensor([batch_time.total_seconds()], dtype=torch.float64))
+            torch.tensor([batch_time.total_seconds()], dtype=torch.float32))
         dist.broadcast(batch_time_tensor, src=0)
         batch_time = datetime.timedelta(seconds=batch_time_tensor[0].cpu().item())
 
         return int(sample_token_tensor[0].cpu().item()), int(sample_token_tensor[1].cpu().item()), batch_time
 
     def _train_loop(self) -> None:
         """Run training for the specified number of epochs and log results."""
         # print training start
         log.info('Using precision %s', self.state.precision)
         self.logger.data_fit({algo.__class__.__name__: 1 for algo in self.state.algorithms})
 
         assert self.state.dataloader is not None, 'dataloader is set in __init__() or fit()'
         assert self._train_data_spec is not None, 'The train data spec is set in __init__() or fit()'
+        assert self.state.scaler is not None, 'scaler should have been set in __init__()'
 
         self.engine.run_event(Event.FIT_START)
 
-        # surpressing GradScaler warnings as they are always created
-        # self._use_grad_scaling() will raise a RuntimeError if grad scaling is not available when it is required
-        warnings.filterwarnings(action='ignore', message='torch.cuda.amp.GradScaler')
-        self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
         use_grad_scaling = self._use_grad_scaling(self.state.precision, self.state.scaler)
 
         self._spin_dataloaders()
 
         if self.state.timestamp.batch_in_epoch == 0 and self._rng_state is not None:
             # only restore the rng state here if the step in the current epoch is zero.
             reproducibility.load_rng_state(self._rng_state)
@@ -1458,132 +1492,131 @@
 
         # Flag if the epoch finished early, so it can be tracked whether to run the epoch end events
         finished_epoch_early = False
 
         last_wct = datetime.datetime.now()
 
         while self.state.timestamp < self.state.max_duration:
-            try:
+            self.state.model.train()
+
+            if int(self.state.timestamp.batch_in_epoch) == 0:
+                self.engine.run_event(Event.EPOCH_START)
+                self.logger.data_epoch({'epoch': int(self.state.timestamp.epoch)})
+                if self.train_metrics is not None:
+                    # reset the metrics before every epoch
+                    self.train_metrics.reset()
+
+            dataloader = self.state.dataloader
+            if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
+                dataloader.sampler.set_epoch(int(self.state.timestamp.epoch))
+
+            for batch_idx, self.state.batch in enumerate(self._iter_dataloader(TrainerMode.TRAIN)):
+
+                # if resuming, skip dataloader forward to the minibatch index
+                if batch_idx < int(self.state.timestamp.batch_in_epoch):
+                    # Restore the RNG state immediately before the next batch is yielded from the dataloader
+                    if batch_idx + 1 == int(self.state.timestamp.batch_in_epoch) and self._rng_state is not None:
+                        reproducibility.load_rng_state(self._rng_state)
+                        self._rng_state = None
+                    continue
+
+                self.state.batch = self._device.batch_to_device(self.state.batch)
+                self.state.batch = self._train_data_spec.device_transforms(self.state.batch)
+                rank_num_samples = self._train_data_spec.get_num_samples_in_batch(self.state.batch)
+                rank_num_tokens = self._train_data_spec.get_num_tokens_in_batch(self.state.batch)
+
+                if self.deepspeed_enabled:
+                    self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
+
+                if self.train_metrics is not None:
+                    self.state.model.eval()
+                    with torch.no_grad():
+                        for eval_microbatch in self._train_data_spec.split_batch(self.state.batch,
+                                                                                 self.state.grad_accum):
+                            # TODO: Detect if self.run_event(Event.AFTER_DATALOADER) changes the training
+                            # data and if so print a warning that metrics may return unexpected results
+                            with get_precision_context(self.state.precision):
+                                outputs, targets = self._original_model.validate(eval_microbatch)
+                                # Run in same precision context to avoid NaNs
+                                self.train_metrics.update(outputs, targets)
+
                 self.state.model.train()
 
-                if int(self.state.timestamp.batch_in_epoch) == 0:
-                    self.engine.run_event(Event.EPOCH_START)
-                    self.logger.data_epoch({'epoch': int(self.state.timestamp.epoch)})
-                    if self.train_metrics is not None:
-                        # reset the metrics before every epoch
-                        self.train_metrics.reset()
-
-                dataloader = self.state.dataloader
-                if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
-                    dataloader.sampler.set_epoch(int(self.state.timestamp.epoch))
-
-                for batch_idx, self.state.batch in enumerate(self._iter_dataloader()):
-
-                    # if resuming, skip dataloader forward to the minibatch index
-                    if batch_idx < int(self.state.timestamp.batch_in_epoch):
-                        # Restore the RNG state immediately before the next batch is yielded from the dataloader
-                        if batch_idx + 1 == int(self.state.timestamp.batch_in_epoch) and self._rng_state is not None:
-                            reproducibility.load_rng_state(self._rng_state)
-                            self._rng_state = None
-                        continue
-
-                    self.state.batch = self._device.batch_to_device(self.state.batch)
-                    self.state.batch = self._train_data_spec.device_transforms(self.state.batch)
-                    rank_num_samples = self._train_data_spec.get_num_samples_in_batch(self.state.batch)
-                    rank_num_tokens = self._train_data_spec.get_num_tokens_in_batch(self.state.batch)
-
-                    if self.deepspeed_enabled:
-                        self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
-
-                    if self.train_metrics is not None:
-                        self.state.model.eval()
-                        with torch.no_grad():
-                            for eval_microbatch in self._train_data_spec.split_batch(
-                                    self.state.batch, self.state.grad_accum):
-                                # TODO: Detect if self.run_event(Event.AFTER_DATALOADER) changes the training
-                                # data and if so print a warning that metrics may return unexpected results
-                                self.train_metrics.update(*self._original_model.validate(eval_microbatch))
-
-                    self.state.model.train()
-
-                    self.engine.run_event(Event.AFTER_DATALOADER)
-
-                    self.engine.run_event(Event.BATCH_START)
-                    self.logger.data_batch({
-                        'trainer/global_step': int(self.state.timestamp.batch),
-                        'trainer/batch_idx': self.state.timestamp.batch_in_epoch.value,
-                    })
-
-                    total_loss = self._train_batch(use_grad_scaling)
-
-                    if use_grad_scaling:
-                        self.state.scaler.update()
-
-                    if total_loss is not None:
-                        if not isinstance(total_loss, torch.Tensor):
-                            total_loss = self._device.tensor_to_device(torch.tensor([total_loss]))
-
-                        # total_loss can be None if gradient scaling failed
-                        dist.all_reduce(total_loss, reduce_operation='SUM')
-                        full_loss = total_loss.cpu().item()
-                        self.logger.data_batch({'loss/train': full_loss / dist.get_world_size()})
-
-                    # The scheduler step.step() and compute_and_log_metrics() are going to be included in the
-                    # next batch's wall clock time. The time accumulation must be done here so schedulers
-                    # have the latest timing information
-
-                    now = datetime.datetime.now()
-
-                    batch_time = now - last_wct
-
-                    total_num_samples, total_num_tokens, batch_time = self._accumulate_time_across_ranks(
-                        rank_num_samples,
-                        rank_num_tokens,
-                        batch_time,
-                    )
+                self.engine.run_event(Event.AFTER_DATALOADER)
+
+                self.engine.run_event(Event.BATCH_START)
+                self.logger.data_batch({
+                    'trainer/global_step': int(self.state.timestamp.batch),
+                    'trainer/batch_idx': self.state.timestamp.batch_in_epoch.value,
+                })
+
+                total_loss = self._train_batch(use_grad_scaling)
+
+                if use_grad_scaling:
+                    self.state.scaler.update()
+
+                if total_loss is not None:
+                    if not isinstance(total_loss, torch.Tensor):
+                        total_loss = self._device.tensor_to_device(torch.tensor([total_loss]))
+
+                    # total_loss can be None if gradient scaling failed
+                    dist.all_reduce(total_loss, reduce_operation='SUM')
+                    full_loss = total_loss.cpu().item()
+                    self.logger.data_batch({'loss/train': full_loss / dist.get_world_size()})
+
+                # The scheduler step.step() and compute_and_log_metrics() are going to be included in the
+                # next batch's wall clock time. The time accumulation must be done here so schedulers
+                # have the latest timing information
 
-                    # `now` is actually in the past, but want to include the time it takes to perform this reduction
-                    last_wct = now
+                now = datetime.datetime.now()
+
+                batch_time = now - last_wct
+
+                total_num_samples, total_num_tokens, batch_time = self._accumulate_time_across_ranks(
+                    rank_num_samples,
+                    rank_num_tokens,
+                    batch_time,
+                )
+
+                # `now` is actually in the past, but want to include the time it takes to perform this reduction
+                last_wct = now
+
+                self.state.timestamp = self.state.timestamp.to_next_batch(
+                    samples=total_num_samples,
+                    tokens=total_num_tokens,
+                    duration=batch_time,
+                )
+
+                if self._scheduler_step_frequency == TimeUnit.BATCH:
+                    for scheduler in self.state.schedulers:
+                        scheduler.step()
 
-                    self.state.timestamp = self.state.timestamp.to_next_batch(
-                        samples=total_num_samples,
-                        tokens=total_num_tokens,
-                        duration=batch_time,
+                if self.train_metrics is not None:
+                    self._compute_and_log_metrics(
+                        dataloader_label='train',
+                        log_level=LogLevel.BATCH,
+                        metrics=self.train_metrics,
                     )
 
-                    if self._scheduler_step_frequency == TimeUnit.BATCH:
-                        for scheduler in self.state.schedulers:
-                            scheduler.step()
-
-                    if self.train_metrics is not None:
-                        self._compute_and_log_metrics(
-                            dataloader_label='train',
-                            log_level=LogLevel.BATCH,
-                            metrics=self.train_metrics,
-                        )
-
-                    self.engine.run_event(Event.BATCH_END)
-
-                    # Pause the timing during evaluation
-                    # Evaluation time is tracked separately in state.eval_timestamp
-                    duration = datetime.datetime.now() - last_wct
-                    self._run_evaluators(Event.BATCH_END, log_level=LogLevel.BATCH)
-                    last_wct = datetime.datetime.now() - duration
-
-                    self.engine.run_event(Event.BATCH_CHECKPOINT)
-
-                    if self.state.timestamp >= self.state.max_duration:
-                        # If max_duration is specified in batches, samples, or tokens, and
-                        # and the max_duration is reached mid-epoch, then break out of the dataloader
-                        # to finish the epoch early and finish training.
-                        finished_epoch_early = True
-                        break
+                self.engine.run_event(Event.BATCH_END)
+
+                # Pause the timing during evaluation
+                # Evaluation time is tracked separately in state.eval_timestamp
+                duration = datetime.datetime.now() - last_wct
+                self._run_evaluators(Event.BATCH_END, log_level=LogLevel.BATCH)
+                last_wct = datetime.datetime.now() - duration
+
+                self.engine.run_event(Event.BATCH_CHECKPOINT)
 
-            except BreakEpochException:
-                log.info(f'Skipping the rest of Epoch {int(self.state.timestamp.epoch)}')
+                if self.state.timestamp >= self.state.max_duration:
+                    # If max_duration is specified in batches, samples, or tokens, and
+                    # and the max_duration is reached mid-epoch, then break out of the dataloader
+                    # to finish the epoch early and finish training.
+                    finished_epoch_early = True
+                    break
 
             if not finished_epoch_early or self.state.dataloader_len == self.state.timestamp.batch_in_epoch:
                 # Trigger the epoch end events if the dataloader was exhausted.
                 # This happens if the "break" did not trigger above, or if it
                 # did (e.g. duration specified in samples/batches/tokens), but it is still
                 # the end of the dataloader (i.e. next(dataloader) would raise StopIteration)
                 self.state.timestamp = self.state.timestamp.to_next_epoch()
@@ -1637,18 +1670,18 @@
 
         # Cache the device batch, because `self.state.batch` gets overridden in microbatching loop
         # TODO: fix this name collision!
         device_batch = self.state.batch
 
         # Retry until we successfully complete training and return loss
         while True:
+            start_time = time.time()
             total_loss = None
             # Note: We use uint8 instead of bool as BOR is not supported on all torch.distributed backends
             should_handle_cuda_oom = 0
-            caught_timeout_error = None
             try:
                 assert self.state.scaler is not None
                 microbatches = self._train_data_spec.split_batch(device_batch, self.state.grad_accum)
                 if self.deepspeed_enabled:
                     total_loss = self._train_microbatches(microbatches)
                 elif self._use_closures():
                     for optimizer in self.state.optimizers:
@@ -1660,52 +1693,73 @@
                                 closure=lambda **kwargs: self._train_microbatches(microbatches, **kwargs).item())
                 else:
                     total_loss = self._train_microbatches(microbatches)
                     for optimizer in self.state.optimizers:
                         if use_grad_scaling:
                             self.state.scaler.step(optimizer)
                         else:
-                            optimizer.step()
+                            if isinstance(self._device, DeviceTPU):
+                                xm.optimizer_step(optimizer, barrier=True)
+                            else:
+                                optimizer.step()
             except RuntimeError as e:
                 if self.adaptive_gradient_accumulation and _is_cuda_oom(e):
                     log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                     should_handle_cuda_oom = 1
-                elif 'Timed out' in str(e):
-                    # Catch timeout errors and only reraise if we did not encounter OOM on other ranks. Error
-                    # is likely transient if one rank OOMed, it likely did not reach a barrier. Note that if we
-                    # catch non-transient timeout errors they will be later reraised if no rank OOMed.
-                    caught_timeout_error = e
                 else:
                     raise
+            end_time = time.time()
+
+            # Use monitored barrier to error on deadlock. If one rank OOMs and another doesn't and gets stuck
+            # on a dist reduction in gradient syncronization, the monitored barrier will fail after the timeout.
+            # If `adaptive_gradient_accumulation=False`, the OOMing rank will instead crash, avoiding deadlock risk.
+            if self.adaptive_gradient_accumulation:
+                try:
+                    dist.monitored_barrier(timeout=datetime.timedelta(seconds=max(10, 0.5 * self.batch_compute_time)))
+                except RuntimeError as e:
+                    raise RuntimeError(
+                        'A deadlock was encountered in the train loop, likely because a strict subset of '
+                        'ranks encountered CUDA OOM when `grad_accum=auto`. Try manually setting `grad_accum` '
+                        'instead.') from e
 
             # Propagate across all ranks if any rank hit CUDA OOM
             should_handle_cuda_oom = self._device.tensor_to_device(
                 torch.tensor([should_handle_cuda_oom], dtype=torch.uint8))
-            dist.all_reduce(should_handle_cuda_oom, reduce_operation='MAX')
+
+            if not isinstance(self._device, DeviceTPU):
+                dist.all_reduce(should_handle_cuda_oom, reduce_operation='MAX')
             if int(should_handle_cuda_oom.item()) == 1:
                 # If any rank hit CUDA OOM, update grad_accum and retry. Ignore any caught_timeout_error since
                 # it is likely transient, e.g. timeout because certain ranks OOMed and didn't reach barrier.
                 # Raise runtime error if training 1 sample at a time still resulted in CUDA out of memory
                 device_batch_size = self._train_data_spec.get_num_samples_in_batch(device_batch)
                 if self.state.grad_accum == device_batch_size:
                     raise RuntimeError(
                         ('CUDA out of memory. The train loop failed with an internal microbatch of size 1.'
                          'The GPU does not have enough memory to process even 1 sample.'))
                 else:
                     original_grad_accum = self.state.grad_accum
                     self.state.grad_accum = min(2 * self.state.grad_accum, device_batch_size)
-                    log.info(('CUDA out of memory detected. Gradient Accumulation '
-                              f'increased from {original_grad_accum} -> {self.state.grad_accum}, '
-                              'and the batch will be retrained.'))
-            elif caught_timeout_error:
-                # If not CUDA out of memory, raise exception to user. Note that this truncates the call stack
-                # back only to this newly raised error.
-                raise caught_timeout_error
+                    warnings.warn(
+                        RuntimeWarning('CUDA out of memory detected. Gradient Accumulation '
+                                       f'increased from {original_grad_accum} -> {self.state.grad_accum}, '
+                                       'and the batch will be retrained with a '
+                                       f'micro-batchsize of {device_batch_size // self.state.grad_accum}'))
+                    # Empty cache if on GPU, which will help reduce fragmentation
+                    if isinstance(self._device, DeviceGPU):
+                        torch.cuda.empty_cache()
+            # Otherwise, log grad_accum and return calculated loss
             else:
-                # Otherwise, log grad_accum and return calculated loss
+                # Synchronize new batch compute time
+                batch_compute_time = end_time - start_time
+                batch_compute_time = self._device.tensor_to_device(torch.tensor([batch_compute_time],
+                                                                                dtype=torch.float))
+                dist.all_reduce(batch_compute_time, reduce_operation='MAX')
+                self.batch_compute_time = batch_compute_time.item()
+
                 self.logger.data_batch({'trainer/grad_accum': self.state.grad_accum})
                 return total_loss
 
     def _train_microbatches(self, microbatches: Sequence[Batch], ddp_sync: bool = True):
         """Iterate over microbatches and compute the loss that will be used to step the optimizer.
 
         Args:
@@ -1782,62 +1836,114 @@
 
             # loss
             self.engine.run_event(Event.BEFORE_LOSS)
 
             with get_precision_context(self.state.precision):
                 self.state.loss = self._original_model.loss(self.state.outputs, self.state.batch)
 
-            # We always want to scale loss by the grad_accum before the backwards pass and
-            # also for sake of metrics. Complicating matters, the DeepSpeed engine does its
-            # own scaling when we call `.backward`, but this isn't in place so we still need
-            # to scale for sake of metrics after the `.backward` call.
-
-            # Loss is added to losses with clone to not scale the loss for the step printout
-            # Likely need to look into the performance impact
-            if not self.deepspeed_enabled:
-                for loss in ensure_tuple(self.state.loss):
-                    loss.mul_(microbatch_num_samples / current_batch_size)
-                    total_loss += loss.detach().clone()
-
             assert self.state.loss is not None
             self.engine.run_event(Event.AFTER_LOSS)
 
             # backward
             self.engine.run_event(Event.BEFORE_BACKWARD)
 
+            # Sum individual losses
+            microbatch_loss = self._device.tensor_to_device(torch.zeros(size=(1,)))
+            for loss in ensure_tuple(self.state.loss):
+                microbatch_loss.add_(loss.mean())
+
+            # Loss used for logging, scaled by grad_accum for correctly calculating metrics
+            total_loss += microbatch_loss.detach().clone() * (microbatch_num_samples / current_batch_size)
+
             if use_grad_scaling:
-                self.state.loss = cast(torch.Tensor, self.state.scaler.scale(self.state.loss))
+                microbatch_loss = cast(torch.Tensor, self.state.scaler.scale(microbatch_loss))
 
             if self.deepspeed_enabled:
-                self.state.deepspeed_model.backward(self.state.loss)
+                self.state.deepspeed_model.backward(microbatch_loss)
 
-                # This is the same loss scaling and reporting we skipped earlier.
-                for loss in ensure_tuple(self.state.loss):
-                    loss.mul_(microbatch_num_samples / current_batch_size)
-                    total_loss += loss.detach().clone()
             else:
-                final_loss = self._device.tensor_to_device(torch.zeros(size=(1,)))
-                for loss in ensure_tuple(self.state.loss):
-                    final_loss += loss
-                final_loss.backward(create_graph=self._backwards_create_graph)
+                # Scale loss based on the number of samples in the microbatch to maintain gradient numerics
+                microbatch_loss.mul_(microbatch_num_samples / current_batch_size)
+                microbatch_loss.backward(create_graph=self._backwards_create_graph)
 
             self.engine.run_event(Event.AFTER_BACKWARD)
 
         if self.deepspeed_enabled:
             self.state.deepspeed_model.step()
 
-    def predict(self, dataloader: Union[DataLoader, DataSpec], subset_num_batches: int = -1):
+    def predict(
+        self,
+        dataloader: Union[DataLoader, DataSpec],
+        subset_num_batches: int = -1,
+        *,
+        return_outputs: bool = True,
+    ):
         """Output model prediction on the provided data.
 
+        There are two ways to access the prediction outputs.
+
+        1.  With ``return_outputs`` set to True, the batch predictions will be collected into a list and returned.
+        2.  Via a custom callback, which can be used with ``return_outputs`` set to False.
+
+            This technique can be useful if collecting all the outputs from the dataloader would exceed available memory,
+            and you want to write outputs directly to files. For example:
+
+            .. testsetup::
+
+                predict_dl = train_dataloader
+
+            .. testcode::
+
+                import os
+                import torch
+
+                from torch.utils.data import DataLoader
+
+                from composer import Trainer, Callback
+                from composer.loggers import Logger, LogLevel
+
+                class PredictionSaver(Callback):
+                    def __init__(self, folder: str):
+                        self.folder = folder
+                        os.makedirs(self.folder, exist_ok=True)
+
+                    def predict_batch_end(self, state: State, logger: Logger) -> None:
+                        name = f'batch_{int(state.predict_timestamp.batch)}.pt'
+                        filepath = os.path.join(self.folder, name)
+                        torch.save(state.outputs, filepath)
+
+                        # Also log the outputs as an artifact
+                        logger.file_artifact(LogLevel.BATCH, artifact_name=name, file_path=filepath)
+
+                trainer = Trainer(
+                    ...,
+                    callbacks=PredictionSaver('./predict_outputs'),
+                )
+
+                trainer.predict(predict_dl, return_outputs=False)
+
+                print(sorted(os.listdir('./predict_outputs')))
+
+            .. testoutput::
+
+                ['batch_1.pt', ...]
+
         Args:
             dataloader (DataLoader | DataSpec): The :class:`.DataLoader` or
                 :class:`.DataSpec` for the prediction data.
             subset_num_batches (int, optional): If specified, only perform model prediction
                 on this many batches. This parameter has no effect if it is greater than ``len(dataloader)``.
                 If ``-1``, then the entire loader will be iterated over. (default: ``-1``)
+            return_outputs (bool, optional): If True (the default), then prediction outputs will be (recursively)
+                moved to cpu and accumulated into a list. Otherwise, prediction outputs are discarded after each
+                batch.
+
+        Returns:
+            List: A list of batch outputs, if ``return_outputs`` is True. Otherwise, an empty list.
+
         """
         if isinstance(dataloader, DataSpec):
             data_spec = dataloader
         else:
             data_spec = DataSpec(dataloader)
 
         # Put the model into evaluation mode, but be able to restore it to training mode afterwards
@@ -1852,19 +1958,22 @@
         assert self.state.dataloader is not None, 'Already set the dataloader'
 
         # Reset the predict timestamp
         self.state.predict_timestamp = Timestamp()
 
         last_wct = datetime.datetime.now()
 
+        outputs = []
+        cpu_device = DeviceCPU()
+
         with torch.no_grad():
 
             self.engine.run_event(Event.PREDICT_START)
 
-            for self.state.batch in self._iter_dataloader():
+            for self.state.batch in self._iter_dataloader(TrainerMode.PREDICT):
                 # Move the batch onto the device
                 self.state.batch = self._device.batch_to_device(self.state.batch)
 
                 # Perform any device transforms
                 if data_spec.device_transforms is not None:
                     self.state.batch = data_spec.device_transforms(self.state.batch)
 
@@ -1875,17 +1984,21 @@
                 # Fix the batch if using DeepSpeed
                 if self.deepspeed_enabled:
                     self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
 
                 self.engine.run_event(Event.PREDICT_BATCH_START)
 
                 self.engine.run_event(Event.PREDICT_BEFORE_FORWARD)
-                self.state.outputs = self.state.model(self.state.batch)
+                with get_precision_context(self.state.precision):
+                    self.state.outputs = self.state.model(self.state.batch)
                 self.engine.run_event(Event.PREDICT_AFTER_FORWARD)
 
+                if return_outputs:
+                    outputs.append(cpu_device.batch_to_device(self.state.outputs))
+
                 now = datetime.datetime.now()
                 batch_time = now - last_wct
 
                 total_num_samples, total_num_tokens, batch_time = self._accumulate_time_across_ranks(
                     num_samples=rank_num_samples,
                     num_tokens=rank_num_tokens,
                     batch_time=batch_time,
@@ -1906,14 +2019,16 @@
             self.state.model.train()
 
         # Restore the dataloader
         self.state.set_dataloader(original_dataloader, original_dataloader_label)
         if original_dataloader_len is not None:
             self.state.dataloader_len = original_dataloader_len
 
+        return outputs
+
     def eval(
         self,
         dataloader: Union[Iterable, DataSpec, dict],
         dataloader_label: str = 'eval',
         *,
         metrics: Union[Metric, MetricCollection],
         subset_num_batches: int = -1,
@@ -1972,33 +2087,41 @@
             if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
                 # The distributed sampler uses `set_epoch` to set the random seed
                 # Because evaluation can run on each batch, we use the batch to seed the sampler
                 # so each evaluation will get a proper shuffle.
                 # The epoch provided to `set_epoch` need not be sequential, so this is fine.
                 dataloader.sampler.set_epoch(int(self.state.timestamp.batch))
 
-            for self.state.batch in self._iter_dataloader():
+            for self.state.batch in self._iter_dataloader(TrainerMode.EVAL):
                 self.state.batch = self._device.batch_to_device(self.state.batch)
                 if data_spec.device_transforms is not None:
                     self.state.batch = data_spec.device_transforms(self.state.batch)
 
                 # Count the batch size and num tokens before any events run
                 rank_num_samples = data_spec.get_num_samples_in_batch(self.state.batch)
                 rank_num_tokens = data_spec.get_num_tokens_in_batch(self.state.batch)
 
                 if self.deepspeed_enabled:
                     self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
 
                 self.engine.run_event(Event.EVAL_BATCH_START)
 
                 self.engine.run_event(Event.EVAL_BEFORE_FORWARD)
-                self.state.outputs, targets = self._original_model.validate(self.state.batch)
+                with get_precision_context(self.state.precision):
+                    self.state.outputs, targets = self._original_model.validate(self.state.batch)
                 self.engine.run_event(Event.EVAL_AFTER_FORWARD)
 
-                metrics.update(self.state.outputs, targets)
+                # Run in same precision context to avoid NaNs
+                with get_precision_context(self.state.precision):
+                    if isinstance(self._device, DeviceMPS):
+                        # torchmetrics math has numerical errors on M1 devices
+                        # running the compute on CPU instead
+                        metrics.update(self.state.outputs.cpu(), targets.cpu())
+                    else:
+                        metrics.update(self.state.outputs, targets)
 
                 now = datetime.datetime.now()
                 batch_time = now - last_wct
 
                 total_num_samples, total_num_tokens, batch_time = self._accumulate_time_across_ranks(
                     num_samples=rank_num_samples,
                     num_tokens=rank_num_tokens,
@@ -2052,50 +2175,60 @@
         use_grad_scaling = precision == Precision.AMP
 
         if use_grad_scaling and (scaler is None or not scaler.is_enabled()):
             raise RuntimeError(f'Attempting to use grad scaling with {precision}, but scaler is not enabled.'
                                f'Potentially your hardware does not support Precision {precision}.')
         return use_grad_scaling
 
-    def _iter_dataloader(self):
+    def _iter_dataloader(self, trainer_mode: TrainerMode):
         """Helper method to iterate over the dataloader.
 
         This method yields up to :attr:`.State.dataloader_len`` batches from the dataloader. In addition, if the
         profiler is enabled, the dataloader latency recorded via the :class:`.Marker` API.
+
+        Args:
+            trainer_mode (TrainerMode): Specifies which mode the trainer is in.
         """
-        marker = None
-        if self.state.profiler is not None:
-            marker = self.state.profiler.marker(f'dataloader/{self.state.dataloader_label}', categories=['dataloader'])
         assert self.state.dataloader is not None, 'the dataloader should be set before calling this method'
 
         if self.state.dataloader_len is None:
             dataloader_iter = iter(self.state.dataloader)
         else:
             dataloader_iter = itertools.islice(self.state.dataloader, int(self.state.dataloader_len))
 
         while True:
-            if marker is not None:
-                marker.start()
             try:
-                yield next(dataloader_iter)
+                # [BEFORE/AFTER]_DATALOADER only runs while training
+                if trainer_mode == TrainerMode.TRAIN:
+                    self.engine.run_event(Event.BEFORE_DATALOADER)
+                batch = next(dataloader_iter)
             except StopIteration:
+                # [BEFORE/AFTER]_DATALOADER only runs while training
+                if trainer_mode == TrainerMode.TRAIN:
+                    # Event.AFTER_DATALOADER is normally called in the train loop. However, if we
+                    # encounter StopIteration, the train loop will not run. Accordingly, we need to
+                    # explicitly call the engine to run marker.finish() for the dataloader marker.
+                    # Otherwise, we will encounter an error at the start of the next epoch when
+                    # Event.BEFORE_DATALOADER tries to start an unfinished marker.
+                    self.engine.run_marker_only_event(Event.AFTER_DATALOADER)
                 break
-            finally:
-                if marker is not None:
-                    marker.finish()
+            yield batch
 
     def _use_closures(self) -> bool:
         """Determines based on precision and optimizers whether to use closures.
 
         We default to using closures unless AMP is enabled, in which case we only allow closures when using optimizers
         with the _step_supports_amp_closure flag.
         """
         if self.deepspeed_enabled:
             return False
 
+        if isinstance(self._device, DeviceTPU):
+            return False
+
         if self.state.precision != Precision.AMP:
             return True
 
         if self.state.optimizers is None:
             raise RuntimeError('state.optimizers must be set before `_use_closures` can be determined')
 
         return all(
@@ -2109,7 +2242,49 @@
             name (str, optional): See :func:`.save_checkpoint`.
             weights_only (bool, optional): See :func:`.save_checkpoint`.
 
         Returns:
             List[pathlib.Path]: See :func:`.save_checkpoint`.
         """
         return save_checkpoint(state=self.state, filename=name, weights_only=weights_only)
+
+    def export_for_inference(
+        self,
+        save_format: Union[str, ExportFormat],
+        save_path: str,
+        save_object_store: Optional[ObjectStore] = None,
+        sample_input: Optional[Any] = None,
+        transforms: Optional[Sequence[Transform]] = None,
+    ):
+        """Export a model for inference.
+
+        Args:
+            save_format (Union[str, ExportFormat]):  Format to export to. Either ``"torchscript"`` or ``"onnx"``.
+            save_path: (str): The path for storing the exported model. It can be a path to a file on the local disk,
+            a URL, or if ``save_object_store`` is set, the object name
+                in a cloud bucket. For example, ``my_run/exported_model``.
+            save_object_store (ObjectStore, optional): If the ``save_path`` is in an object name in a cloud bucket
+                (i.e. AWS S3 or Google Cloud Storage), an instance of
+                :class:`~.ObjectStore` which will be used
+                to store the exported model. If this is set to ``None``,  will save to ``save_path`` using the trainer's
+                logger. (default: ``None``)
+            sample_input (Any, optional): Example model inputs used for tracing. This is needed for "onnx" export.
+                The ``sample_input`` need not match the batch size you intend to use for inference. However, the model
+                should accept the ``sample_input`` as is. (default: ``None``)
+            transforms (Sequence[Transform], optional): transformations (usually optimizations) that should
+                be applied to the model. Each Transform should be a callable that takes a model and returns a modified model.
+
+        Returns:
+            None
+        """
+        export_model = self.state.model.module if self.state.is_model_ddp else self.state.model
+        if not isinstance(export_model, nn.Module):
+            raise ValueError(f'Exporting Model requires type torch.nn.Module, got {type(export_model)}')
+        if sample_input == None and save_format == 'onnx':
+            sample_input = self.state.batch
+        export_with_logger(model=export_model,
+                           save_format=save_format,
+                           save_path=save_path,
+                           logger=self.logger,
+                           save_object_store=save_object_store,
+                           sample_input=(sample_input,),
+                           transforms=transforms)
```

### Comparing `mosaicml-0.8.2/composer/trainer/trainer_hparams.py` & `mosaicml-0.9.0/composer/trainer/trainer_hparams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""The :class:`~yahp.hparams.Hparams` used to construct the :class:`~composer.trainer.trainer.Trainer`."""
+"""The :class:`~yahp.hparams.Hparams` used to construct the :class:`.Trainer`."""
 
 from __future__ import annotations
 
 import copy
 import dataclasses
 import datetime
 import logging
@@ -32,17 +32,17 @@
                              SSDHparams, TimmHparams, UnetHparams, ViTSmallPatch16Hparams)
 from composer.models.base import ComposerModel
 from composer.optim import ComposerScheduler
 from composer.optim.optimizer_hparams_registry import OptimizerHparams, optimizer_registry
 from composer.optim.scheduler_hparams_registry import scheduler_registry
 from composer.profiler import Profiler
 from composer.trainer.ddp import DDPSyncStrategy
-from composer.trainer.devices import Device, DeviceCPU, DeviceGPU
+from composer.trainer.devices import Device, DeviceCPU, DeviceGPU, DeviceTPU
 from composer.trainer.devices.device_hparams_registry import device_registry
-from composer.trainer.trainer import Trainer
+from composer.trainer.trainer import Trainer, _is_tpu_installed
 from composer.utils import dist, reproducibility
 from composer.utils.object_store.object_store_hparams import ObjectStoreHparams, object_store_registry
 
 if TYPE_CHECKING:
     from typing import TypedDict
 else:
     TypedDict = object  # TypedDict is not available on python 3.7
@@ -81,19 +81,18 @@
     if dataset_hparams is not None:
         if batch_size is None:
             raise ValueError(
                 f'The batch size for {dataloader_label} must be specified if the {dataloader_label} dataset is specified'
             )
 
         train_device_batch_size = batch_size // dist.get_world_size()
-        if dataset_hparams.shuffle and subset_num_batches is not None:
-            warnings.warn(
-                (f'SubsetNumBatchesWarning: When specifying `subset_num_batches` for the {dataloader_label} dataset, '
-                 f'dataset_hparams.shuffle should be set to False. '
-                 'Otherwise, each epoch may load a different subset of samples.'))
+        if dataset_hparams.shuffle and subset_num_batches is not None and subset_num_batches != -1:
+            warnings.warn((f'SubsetNumBatchesWarning: When specifying `[train|eval]_subset_num_batches` for '
+                           f'the {dataloader_label} dataset, dataset_hparams.shuffle should be set to False. '
+                           'Otherwise, each epoch may load a different subset of samples.'))
         dataloader = dataset_hparams.initialize_object(train_device_batch_size, dataloader_hparams)
     return dataloader
 
 
 def _parse_grad_accum(grad_accum: Union[int, str]) -> Union[int, str]:
     if grad_accum == 'auto':
         return grad_accum
@@ -227,25 +226,25 @@
             ``load_logger_destination`` and ``load_object_store`` should not be provided since there can only be one location
             to load from.
         load_weights_only (bool, optional): See :class:`.Trainer`.
         load_strict_model_weights (bool, optional): See :class:`.Trainer`.
         load_progress_bar (bool, optional): See :class:`.Trainer`.
         load_ignore_keys (List[str] | (Dict) -> None, optional): See :class:`.Trainer`.
 
-        save_folder (str, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
-        save_filename (str, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
-        save_artifact_name (str, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
+        save_folder (str, optional): See :class:`.CheckpointSaver`.
+        save_filename (str, optional): See :class:`.CheckpointSaver`.
+        save_artifact_name (str, optional): See :class:`.CheckpointSaver`.
         save_latest_filename (str, optional): See
-            :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
-        save_latest_artifact_name (str, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
-        save_overwrite (str, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
-        save_weights_only (bool, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
+            :class:`.CheckpointSaver`.
+        save_latest_artifact_name (str, optional): See :class:`.CheckpointSaver`.
+        save_overwrite (str, optional): See :class:`.CheckpointSaver`.
+        save_weights_only (bool, optional): See :class:`.CheckpointSaver`.
         save_interval (str, optional): See
             :class:`~composer.callbacks.callback_hparams.CheckpointSaverHparams`.
-        save_num_checkpoints_to_keep (int, optional): See :class:`~composer.callbacks.checkpoint_saver.CheckpointSaver`.
+        save_num_checkpoints_to_keep (int, optional): See :class:`.CheckpointSaver`.
         autoresume (bool, optional): See :class:`.Trainer`.
 
         deepspeed_config (Dict[str, JSON], optional): If set to a dict will be used for as the DeepSpeed
             config for training  (see :class:`.Trainer` for more details). If ``None`` (the default), DeepSpeed will not
             be used.
 
         device (Device, optional): Hparams for constructing the device used for training.
@@ -430,26 +429,36 @@
         device = self.device
         if device is None:
             device = DeviceGPU() if torch.cuda.is_available() else DeviceCPU()
 
         # Distributed
         # Initialized here so it is available within dataloaders
         if dist.get_world_size() > 1:
-            dist.initialize_dist(device.dist_backend, datetime.timedelta(seconds=self.dist_timeout))
+            dist.initialize_dist(device, datetime.timedelta(seconds=self.dist_timeout))
 
         # Reproducibility
         seed = self.seed if self.seed else reproducibility.get_random_seed()
         # need to set seed before model initialization for determinism
         # don't need to set different seeds per process since only the rank 0 initialization is used
         # Algorithms should not use the `seed` on `__init__` but rather on `Event.INIT`, which occurs
         # after the seed was properly distributed across ranks to ensure checkpoint compatibility
         reproducibility.seed_all(seed)
 
         # The model
         model = self.model.initialize_object()
+        # on TPUs, model must be moved to device before optimizer creation
+        if isinstance(device, DeviceTPU):
+            if not _is_tpu_installed():
+                raise ImportError(
+                    'Unable to import torch_xla. Please follow installation instructions at https://github.com/pytorch/xla'
+                )
+            import torch_xla.core.xla_model as xm
+            import torch_xla.distributed.xla_multiprocessing as xmp
+
+            model = xmp.MpModelWrapper(model).to(xm.xla_device())
 
         # Train dataloader
         train_dataloader = _initialize_dataloader(self.train_dataset, self.train_dataloader_label,
                                                   self.train_batch_size, self.train_subset_num_batches, self.dataloader)
 
         # Evaluation
         eval_dataloader = _initialize_eval_dataloader(
@@ -522,14 +531,15 @@
 
             # Checkpoint Saving
             save_folder=self.save_folder,
             save_overwrite=self.save_overwrite,
             save_filename=self.save_filename,
             save_latest_filename=self.save_latest_filename,
             save_artifact_name=self.save_artifact_name,
+            save_latest_artifact_name=self.save_latest_artifact_name,
             save_interval=self.save_interval,
             save_weights_only=self.save_weights_only,
             save_num_checkpoints_to_keep=self.save_num_checkpoints_to_keep,
 
             # Graceful Resumption
             autoresume=self.autoresume,
```

### Comparing `mosaicml-0.8.2/composer/utils/__init__.py` & `mosaicml-0.9.0/composer/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from composer.utils.batch_helpers import batch_get, batch_set
 from composer.utils.checkpoint import load_checkpoint, save_checkpoint
 from composer.utils.collect_env import configure_excepthook, disable_env_report, enable_env_report, print_env
 from composer.utils.file_helpers import (create_symlink_file, ensure_folder_has_no_conflicting_files,
                                          ensure_folder_is_empty, format_name_with_dist, format_name_with_dist_and_time,
                                          get_file, is_tar)
 from composer.utils.import_helpers import MissingConditionalImportError, import_object
+from composer.utils.inference import export_for_inference, export_with_logger
 from composer.utils.iter_helpers import IteratorFileStream, ensure_tuple, map_collection
-from composer.utils.misc import is_notebook
+from composer.utils.misc import is_model_deepspeed, is_notebook
 from composer.utils.object_store import (LibcloudObjectStore, ObjectStore, ObjectStoreTransientError, S3ObjectStore,
                                          SFTPObjectStore)
 from composer.utils.retrying import retry
 from composer.utils.string_enum import StringEnum
 
 __all__ = [
     'ensure_tuple',
@@ -25,20 +26,23 @@
     'ObjectStore',
     'ObjectStoreTransientError',
     'LibcloudObjectStore',
     'S3ObjectStore',
     'SFTPObjectStore',
     'MissingConditionalImportError',
     'import_object',
+    'is_model_deepspeed',
     'is_notebook',
     'StringEnum',
     'load_checkpoint',
     'save_checkpoint',
     'ensure_folder_is_empty',
     'ensure_folder_has_no_conflicting_files',
+    'export_for_inference',
+    'export_with_logger',
     'format_name_with_dist',
     'format_name_with_dist_and_time',
     'is_tar',
     'batch_get',
     'batch_set',
     'configure_excepthook',
     'disable_env_report',
```

### Comparing `mosaicml-0.8.2/composer/utils/batch_helpers.py` & `mosaicml-0.9.0/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/checkpoint.py` & `mosaicml-0.9.0/composer/utils/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 
 from composer.utils import dist, reproducibility
 from composer.utils.file_helpers import (FORMAT_NAME_WITH_DIST_AND_TIME_TABLE, format_name_with_dist_and_time, get_file,
                                          is_tar)
+from composer.utils.misc import is_model_deepspeed
 from composer.utils.object_store import ObjectStore
 
 if TYPE_CHECKING:
     from composer.core.state import State
     from composer.loggers import LoggerDestination
 
 log = logging.getLogger(__name__)
 
-__all__ = ['load_checkpoint', 'save_checkpoint']
+__all__ = ['load_checkpoint', 'save_checkpoint', 'download_checkpoint']
 
 _COMPOSER_STATES_FILENAME = 'composer_states.pt'
 _DEEPSPEED_TAG = 'deepspeed'  # always tag with the same, deterministic name. We'll rename the tarball to the appropriate name.
 
 
 def _format_path_with_rank_zero(path: str) -> str:
     """Formats ``path`` with the rank zero values."""
@@ -108,15 +109,15 @@
                 my_model/ep1-rank1.tar
                 my_model/ep1-rank2.tar
                 ...
 
             Then, ``path`` should be set to ``my_model/ep1-rank{rank}.tar``, and all ranks will load the
             correct state.
 
-        state (State): The :class:`~composer.core.state.State` to load the checkpoint into.
+        state (State): The :class:`~composer.core.State` to load the checkpoint into.
         object_store (Union[ObjectStore, LoggerDestination], optional): If the ``path`` is in an object store
             (i.e. AWS S3 or Google Cloud Storage), an instance of
             :class:`~.ObjectStore` or :class:`~.LoggerDestination` which will be used
             to retreive the checkpoint. Otherwise, if the checkpoint is a local filepath, set to ``None``.
             (default: ``None``)
         load_weights_only (bool, optional): Whether or not to only restore the model weights from the checkpoint without
             restoring the associated state. (default: ``False``)
@@ -152,15 +153,15 @@
     """
     # download the checkpoint to the node-local folder
     log.debug('Loading checkpoint at %s', path)
     tempdir_ctx = tempfile.TemporaryDirectory() if dist.get_local_rank() == 0 else contextlib.nullcontext(None)
     with tempdir_ctx as tempdir:
         try:
             node_checkpoint_folder = _get_node_checkpoint_download_folder(tempdir)
-            composer_states_filepath, extracted_checkpoint_folder, extracted_rank_n = _download_checkpoint(
+            composer_states_filepath, extracted_checkpoint_folder, extracted_rank_n = download_checkpoint(
                 path=path,
                 node_checkpoint_folder=node_checkpoint_folder,
                 object_store=object_store,
                 progress_bar=progress_bar,
             )
             rng_state_dicts = _restore_checkpoint(
                 state,
@@ -185,15 +186,15 @@
     local_rank_zero = dist.get_local_world_size() * dist.get_node_rank()
     paths = dist.all_gather_object(path)
     local_rank_zero_path = paths[local_rank_zero]
     assert local_rank_zero_path is not None, 'local rank zero provides the path'
     return local_rank_zero_path
 
 
-def _download_checkpoint(
+def download_checkpoint(
     path: str,
     node_checkpoint_folder: str,
     object_store: Optional[Union[ObjectStore, LoggerDestination]],
     progress_bar: bool,
 ) -> Tuple[str, Optional[str], bool]:
     """Download the checkpoint stored at ``path``, potentially in ``object_store``, to ``node_checkpoint_folder``.
 
@@ -359,15 +360,15 @@
         # Filter provided list of key paths
         if not callable(ignore_keys):
             ignore_keys = glob_filter(ignore_keys)
         # Call function to modify state_dict
         ignore_keys(state_dict)
     log.debug(f"Loaded checkpoint with keys {state_dict.keys()} and state keys {state_dict['state'].keys()}")
 
-    if state.is_model_deepspeed:
+    if is_model_deepspeed(state.model):
         if extracted_checkpoint_folder is None:
             raise RuntimeError('Deepspeed checkpoints require a tarball, not a weights file.')
 
         global_rank = dist.get_global_rank()
         if global_rank > 0 and not extracted_rank_n:
             raise RuntimeError(f'Deepspeed checkpoint missing for rank {global_rank}')
 
@@ -394,37 +395,37 @@
     weights_only: bool = False,
 ) -> List[pathlib.Path]:  # noqa: D103
     log.debug('Saving checkpoint to %s', filename)
     state_dict = {
         'state': state.state_dict(),
         'rng': reproducibility.get_rng_state(),
     }
-    if weights_only and not state.is_model_deepspeed:
+    if weights_only and not is_model_deepspeed(state.model):
         state_dict['state'] = {'model': state_dict['state']['model']}
 
     checkpoint_filepath = format_name_with_dist_and_time(filename, state.run_name, state.timestamp)
-    if state.is_model_deepspeed and not is_tar(checkpoint_filepath):
+    if is_model_deepspeed(state.model) and not is_tar(checkpoint_filepath):
         # Deepspeed requires tarballs; appending `.tar`
         checkpoint_filepath += '.tar'
 
     with tempfile.TemporaryDirectory() as tmpdir:
         composer_states_filepath = os.path.join(tmpdir, _COMPOSER_STATES_FILENAME)
         if dist.get_global_rank() == 0:
             # Only rank zero saves the composer state dict
             with open(composer_states_filepath, 'xb') as f:
                 torch.save(state_dict, f)
 
-        if state.is_model_deepspeed:
+        if is_model_deepspeed(state.model):
             state.deepspeed_model.save_checkpoint(tmpdir, _DEEPSPEED_TAG)
 
         # Move the checkpoint to the correct location
 
         checkpoint_dirname = os.path.dirname(checkpoint_filepath)
 
-        if is_tar(checkpoint_filepath) and (state.is_model_deepspeed or dist.get_global_rank() == 0):
+        if is_tar(checkpoint_filepath) and (is_model_deepspeed(state.model) or dist.get_global_rank() == 0):
             # Either deepspeed (and every rank needs to call this),
             # or not deepspeed (but using an archive), in which case only rank zero should call this.
             if checkpoint_dirname:
                 os.makedirs(checkpoint_dirname, exist_ok=True)
             write_mode = _get_write_mode(checkpoint_filepath)
             with tarfile.open(checkpoint_filepath, write_mode) as tarball:
                 # add files flat to the tarball with the specified compression
```

### Comparing `mosaicml-0.8.2/composer/utils/collect_env.py` & `mosaicml-0.9.0/composer/utils/collect_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 To override the original :func:`sys.excepthook` see :func:`configure_excepthook`.
 
 By default, the Composer custom ``excepthook`` automatically generates the environment report.
 To disable automatic environment report generation, use the :func:`disable_env_report` helper
 function.  Report generation can be re-enabled by using the :func:`enable_env_report` function.
 """
 
+import json
 import sys
 import time
 from typing import NamedTuple, Optional, TextIO
 
 import cpuinfo
+import importlib_metadata
 import psutil
 
 from composer.utils.misc import is_notebook
 
 __all__ = ['configure_excepthook', 'disable_env_report', 'enable_env_report', 'print_env']
 
 # Check if PyTorch is installed
@@ -85,22 +87,39 @@
 # Track if environment report generation on exception is enabled, enabled by default
 _ENV_EXCEPTION_REPORT = True
 
 
 # Same convention as Torch collect_env, create a namedtuple to track collected fields
 class ComposerEnv(NamedTuple):
     composer_version: str
+    composer_commit_hash: Optional[str]
     node_world_size: int
     host_processor_model_name: str
     host_processor_core_count: int
     local_world_size: int
     accelerator_model_name: str
     cuda_device_count: int
 
 
+def get_composer_commit_hash() -> Optional[str]:
+    # Use PEP-610 to get the commit hash
+    # See https://packaging.python.org/en/latest/specifications/direct-url/
+    files = importlib_metadata.files('mosaicml')
+    if files is None:
+        return
+    files = [f for f in files if str(f).endswith('direct_url.json')]
+    if len(files) == 0:
+        return
+    f = files[0]
+    direct_url = json.loads(f.read_text())
+    vcs_info = direct_url.get('vcs_info', {})
+    commit_id = vcs_info.get('commit_id')
+    return commit_id
+
+
 # Helper functions to get Composer environment information
 def get_composer_version() -> str:
     """Query the Composer version."""
     return str(composer.__version__)
 
 
 def get_host_processor_name() -> str:
@@ -250,28 +269,30 @@
     """Query Torch system environment via :mod:`torch.utils.collect_env`."""
     return torchenv.get_pretty_env_info()
 
 
 # Composer environment information string output format
 _COMPOSER_ENV_INFO_FORMAT = """
 Composer version: {composer_version}
+Composer commit hash: {composer_commit_hash}
 Host processor model name: {host_processor_model_name}
 Host processor core count: {host_processor_core_count}
 Number of nodes: {node_world_size}
 Accelerator model name: {accelerator_model_name}
 Accelerators per node: {local_world_size}
 CUDA Device Count: {cuda_device_count}
 """.strip()
 
 
 # Get Composer environment info
 def get_composer_env() -> str:
     """Query Composer pertinent system information."""
     mutable_dict = ComposerEnv(
         composer_version=get_composer_version(),
+        composer_commit_hash=get_composer_commit_hash(),
         host_processor_model_name=get_host_processor_name(),
         host_processor_core_count=get_host_processor_cores(),
         node_world_size=get_node_world_size(),
         accelerator_model_name=get_accel_model_name(),
         local_world_size=get_local_world_size(),
         cuda_device_count=get_cuda_device_count(),
     )._asdict()
@@ -344,14 +365,15 @@
         [pip3] vit-pytorch==0.27.0
         [conda] Could not collect
 
 
         Composer information
         --------------------
         Composer version: 0.8.2
+        Composer commit hash: 9e14a47562def0baa414242c36954eb3083dcd46
         Host processor model name: AMD EPYC 7502 32-Core Processor
         Host processor core count: 64
         Number of nodes: 1
         Accelerator model name: NVIDIA GeForce RTX 3080
         Accelerators per node: 1
         CUDA Device Count: 4
```

### Comparing `mosaicml-0.8.2/composer/utils/dist.py` & `mosaicml-0.9.0/composer/utils/dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,23 @@
 """
 from __future__ import annotations
 
 import datetime
 import logging
 import os
 from contextlib import contextmanager
-from typing import Any, List, Optional, Sequence, TypeVar, cast
+from typing import TYPE_CHECKING, Any, List, Optional, Sequence, TypeVar, cast
 
 import torch
 import torch.distributed as dist
 import torch.utils.data
 
+if TYPE_CHECKING:
+    from composer.trainer.devices import Device
+
 TObj = TypeVar('TObj')
 
 __all__ = [
     'all_gather',
     'all_gather_object',
     'all_reduce',
     'barrier',
@@ -56,18 +59,22 @@
     'get_local_world_size',
     'get_node_rank',
     'get_sampler',
     'get_world_size',
     'initialize_dist',
     'is_available',
     'is_initialized',
+    'monitored_barrier',
 ]
 
 log = logging.getLogger(__name__)
 
+# monitored_barrier requires gloo backend, which is initialized as a global variable
+group_gloo = None
+
 
 def _get_distributed_config_var(
     env_var: str,
     human_name: str,
     default: int,
     fetch_fn_name: Optional[str] = None,
 ) -> int:
@@ -160,14 +167,37 @@
         return
     raise RuntimeError(f'The world_size({world_size}) > 1, but the distributed package is not '
                        'available or has not been initialized. Please check you have initialized '
                        'the distributed runtime and that PyTorch has been built with distributed '
                        'support.')
 
 
+def monitored_barrier(timeout: Optional[datetime.timedelta] = None) -> None:
+    """Synchronizes all processes.
+
+    This function blocks until all processes reach this function. Unlike `barrier`, `monitored_barrier`
+    times out and raises an error if not all ranks reach this function by `timeout`.
+
+    .. seealso:: :func:`torch.distributed.barrier`
+    """
+    if dist.is_available() and dist.is_initialized():
+        # monitored_barrier requires gloo backend, which is initialized as a global variable
+        global group_gloo
+        if group_gloo:
+            dist.monitored_barrier(group=group_gloo, timeout=timeout)
+        return
+    world_size = get_world_size()
+    if world_size == 1:
+        return
+    raise RuntimeError(f'The world_size({world_size}) > 1, but the distributed package is not '
+                       'available or has not been initialized. Please check you have initialized '
+                       'the distributed runtime and that PyTorch has been built with distributed '
+                       'support.')
+
+
 def all_reduce(
     tensor: torch.Tensor,
     reduce_operation: str = 'SUM',
 ) -> None:
     """Reduce a ``tensor`` by applying the ``reduce_operation``.
 
     All ranks get the same, bitwise-identical result.
@@ -331,15 +361,15 @@
 
     Returns:
         bool: Whether PyTorch distributed is initialized.
     """
     return dist.is_initialized()
 
 
-def initialize_dist(backend: str, timeout: datetime.timedelta):
+def initialize_dist(device: Device, timeout: datetime.timedelta):
     """Initialize the default PyTorch distributed process group.
 
     This function assumes that the following environment variables are set:
 
     * ``RANK``: The global rank of the process, which should be on ``[0; WORLD_SIZE - 1]``.
     * ``LOCAL_RANK``: The local rank for the process, which should be on ``[0; LOCAL_WORLD_SIZE - 1]``.
     * ``NODE_RANK``: The rank of the node.
@@ -350,27 +380,25 @@
 
     If none of the environment variables are set, this function will assume a single-rank
     configuration and initialize the default process group using a :class:`torch.distributed.HashStore` store.
 
     .. seealso:: :func:`torch.distributed.init_process_group`
 
     Args:
-        backend (str): The distributed backend to use. Should be ``gloo`` for CPU training,
-            or ``nccl`` for GPU training.
+        device (str): The device from which the distributed backend is interpreted.
         timeout (datetime.timedelta): The timeout for operations executed against the process group.
     """
     if get_world_size() > 1 and not dist.is_available():
         raise RuntimeError('When the world size is > 1, ``torch.distributed`` must be used. However, it is '
                            'not available in your installation of PyTorch. Please install or build PyTorch '
                            'with distributed support.')
-        return
 
     if dist.is_initialized():
-        if dist.get_backend() != backend.lower():
-            raise RuntimeError(f'The requested backend ({backend}) differs from the backend '
+        if dist.get_backend() != device.dist_backend.lower():
+            raise RuntimeError(f'The requested backend ({device.dist_backend}) differs from the backend '
                                f'of the current process group ({dist.get_backend()}). If you '
                                'wish to change backends, please restart the python process.')
         return
 
     # If any of these variables are set, and they do not match the single rank defaults,
     # then do not automatically configure distributed. There are no reasonable defaults to infer
     # for the other variables. Instead, let torch.dist error on an incomplete configuration.
@@ -396,18 +424,17 @@
     )
 
     dist_env_vars_match_defaults = all(os.environ.get(k, v) == v for (k, v) in dist_env_var_defaults.items())
 
     if dist_env_vars_match_defaults:
         # Fill in the remaining single-rank variables
         os.environ.update(dist_env_var_defaults)
-        dist.init_process_group(backend, store=dist.HashStore(), world_size=1, rank=0)
-        return
-
-    dist.init_process_group(backend, timeout=timeout)
+        dist.init_process_group(device.dist_backend, store=dist.HashStore(), world_size=1, rank=0)
+    else:
+        dist.init_process_group(device.dist_backend, timeout=timeout)
 
 
 def get_sampler(dataset: torch.utils.data.Dataset, *, drop_last: bool, shuffle: bool):
     """Constructs a :class:`~torch.utils.data.distributed.DistributedSampler` for a dataset.
 
     The :class:`~torch.utils.data.distributed.DistributedSampler` assumes that each rank has a complete copy of the
     dataset. It ensures that each rank sees a unique shard for each epoch containing
```

### Comparing `mosaicml-0.8.2/composer/utils/file_helpers.py` & `mosaicml-0.9.0/composer/utils/file_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 
 FORMAT_NAME_WITH_DIST_TABLE = """
 +------------------------+-------------------------------------------------------+
 | Variable               | Description                                           |
 +========================+=======================================================+
 | ``{run_name}``         | The name of the training run. See                     |
-|                        | :attr:`~composer.loggers.logger.Logger.run_name`.     |
+|                        | :attr:`.Logger.run_name`.                             |
 +------------------------+-------------------------------------------------------+
 | ``{rank}``             | The global rank, as returned by                       |
 |                        | :func:`~composer.utils.dist.get_global_rank`.         |
 +------------------------+-------------------------------------------------------+
 | ``{local_rank}``       | The local rank of the process, as returned by         |
 |                        | :func:`~composer.utils.dist.get_local_rank`.          |
 +------------------------+-------------------------------------------------------+
@@ -191,15 +191,15 @@
 """
 
 FORMAT_NAME_WITH_DIST_AND_TIME_TABLE = """
 +----------------------------+------------------------------------------------------------+
 | Variable                   | Description                                                |
 +============================+============================================================+
 | ``{run_name}``             | The name of the training run. See                          |
-|                            | :attr:`~composer.loggers.logger.Logger.run_name`.          |
+|                            | :attr:`.Logger.run_name`.                                  |
 +----------------------------+------------------------------------------------------------+
 | ``{rank}``                 | The global rank, as returned by                            |
 |                            | :func:`~composer.utils.dist.get_global_rank`.              |
 +----------------------------+------------------------------------------------------------+
 | ``{local_rank}``           | The local rank of the process, as returned by              |
 |                            | :func:`~composer.utils.dist.get_local_rank`.               |
 +----------------------------+------------------------------------------------------------+
```

### Comparing `mosaicml-0.8.2/composer/utils/fx_utils.py` & `mosaicml-0.9.0/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/import_helpers.py` & `mosaicml-0.9.0/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/iter_helpers.py` & `mosaicml-0.9.0/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/module_surgery.py` & `mosaicml-0.9.0/composer/utils/module_surgery.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 from torch.optim import Optimizer
 
 from composer.utils.iter_helpers import ensure_tuple
 
 log = logging.getLogger(__name__)
 
 __all__ = [
-    'ReplacementFunction', 'replace_module_classes', 'count_module_instances', 'update_params_in_optimizer',
-    'replace_params_in_optimizer'
+    'ReplacementFunction',
+    'replace_module_classes',
+    'count_module_instances',
+    'update_params_in_optimizer',
 ]
 
 ReplacementFunction = Callable[[torch.nn.Module, int], Optional[torch.nn.Module]]
 
 
 def _add_children_recursive(
     module: torch.nn.Module,
@@ -160,32 +162,45 @@
                     `deepspeed.DeepSpeedEngine` Instead, please perform surgery on the underlying module`,
                     and re-wrap it with `deepspeed.DeepSpeedEngine`"""))
     replaced_pairs = {}
     children_to_parents_and_names: OrderedDict[torch.nn.Module, List[Tuple[torch.nn.Module,
                                                                            str]]] = collections.OrderedDict()
     _add_children_recursive(module, children_to_parents_and_names)
     indices = indices if indices is not None else {c: 0 for c in policies}
+
+    default_device = _infer_device(module)
+
     while len(children_to_parents_and_names) > 0:
         child, parents = children_to_parents_and_names.popitem(last=False)
         for policy_class, replacement_fn in policies.items():
             if not isinstance(child, policy_class):
                 continue
             module_index = indices[policy_class]
             replacement = replacement_fn(
                 child,
                 module_index,
             )
             indices[policy_class] += 1
             if replacement is not None:
                 assert child not in replaced_pairs
-                replaced_pairs[child] = replacement
 
+                # if no device inferred (child has no parameters, e.g. Pool2d),
+                # use the default device inferred from the entire module.
+                device = _infer_device(child)
+                if device is None:
+                    device = default_device
+
+                if device:
+                    replacement = replacement.to(device)
+
+                replaced_pairs[child] = replacement
                 for parent, name in parents:
                     # update each parent with the replaced child
                     setattr(parent, name, replacement)
+
                 # recurse on new child object
                 if recurse_on_replacements:
                     children_to_parents_and_names[replacement] = list(parents)  # copy the parents list
                     _add_children_recursive(replacement, children_to_parents_and_names)
     if optimizers:
         for old_module, new_module in replaced_pairs.items():
             update_params_in_optimizer(old_params=old_module.parameters(),
@@ -196,14 +211,24 @@
             textwrap.dedent("""\
             optimizers was not provided. Be sure to either create the optimizer after
             invoking this method, or manually add new parameters to the existing optimizer."""))
 
     return replaced_pairs
 
 
+def _infer_device(module: torch.nn.Module) -> Optional[torch.device]:
+    """Attempt to infer a module's device by inspecting its parameters and buffers."""
+    try:
+        p = next(itertools.chain(module.parameters(), module.buffers()))
+    except StopIteration:
+        return None
+    else:
+        return p.device
+
+
 def count_module_instances(module: torch.nn.Module, module_class: Union[Type[torch.nn.Module],
                                                                         Tuple[Type[torch.nn.Module], ...]]) -> int:
     """Counts the number of instances of ``module_class`` in ``module``, recursively.
 
     .. rubric:: Example
 
     .. testsetup::
@@ -359,51 +384,7 @@
         group_idx = old_group_idxs[0]
 
     param_group = opt.param_groups[group_idx]
     new_param_list = [p for p in param_group['params'] if not _tensor_in(p, removed_params)]
     new_param_list += list(added_params)
     log.info(f'adding {len(added_params)} new parameters to parameter group #{group_idx}')
     param_group['params'] = new_param_list
-
-
-def replace_params_in_optimizer(old_params: Iterable[torch.nn.parameter.Parameter],
-                                new_params: Iterable[torch.nn.parameter.Parameter],
-                                optimizers: Union[Optimizer, Sequence[Optimizer]]) -> None:
-    """Fully replaces an optimizer's parameters.
-
-    This differs from :meth:`update_params_in_optimizer` in that this method is capable
-    of replacing parameters spanning multiple param groups. To accomplish this,
-    this function assumes that parameters in ``new_params`` should inherit the
-    param group of the corresponding parameter from ``old_params``. Thus, this
-    function also assumes that ``old_params`` and ``new_params`` have the same length.
-
-    Args:
-        old_params (Iterator[torch.nn.parameter.Parameter]): Current parameters of the optimizer.
-        new_params (Iterator[torch.nn.parameter.Parameter]): New parameters of the optimizer, given in the same order as
-            ``old_params``. Must be the same length as ``old_params``.
-        optimizers (torch.optim.Optimizer | Sequence[torch.optim.Optimizer]): One or more :class:`torch.optim.Optimizer` objects.
-
-    Raises:
-        NotImplementedError: If ``optimizers`` contains more than one optimizer.
-        RuntimeError: If ``old_params`` and ``new_params`` have different lengths, or
-            if a param from ``old_params`` cannot be found.
-    """
-    if len(ensure_tuple(optimizers)) > 1:
-        raise NotImplementedError('Surgery with multiple optimizers is not yet supported.')
-
-    opt = ensure_tuple(optimizers)[0]
-
-    param_to_idxs_map = {}
-    for group_idx, param_group in enumerate(opt.param_groups):
-        param_list = param_group['params']
-        for param_idx, param in enumerate(param_list):
-            param_to_idxs_map[param] = (group_idx, param_idx)
-
-    for old_param, new_param in itertools.zip_longest(old_params, new_params):
-        if old_params is None or new_params is None:
-            raise RuntimeError('old_params and new_params have different lengths.')
-
-        if not old_param in param_to_idxs_map:
-            raise RuntimeError(f'Parameter {old_param} is missing from the optimizer.')
-
-        group_idx, param_idx = param_to_idxs_map[old_param]
-        opt.param_groups[group_idx]['params'][param_idx] = new_param
```

### Comparing `mosaicml-0.8.2/composer/utils/object_store/__init__.py` & `mosaicml-0.9.0/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/object_store/libcloud_object_store.py` & `mosaicml-0.9.0/composer/utils/object_store/libcloud_object_store.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/object_store/object_store.py` & `mosaicml-0.9.0/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/object_store/object_store_hparams.py` & `mosaicml-0.9.0/composer/utils/object_store/object_store_hparams.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/object_store/s3_object_store.py` & `mosaicml-0.9.0/composer/utils/object_store/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/object_store/sftp_object_store.py` & `mosaicml-0.9.0/composer/utils/object_store/sftp_object_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             Defaults to None.
         password (str, optional): The password (if required) needed to authenticate. Defaults to None.
         key_filename (pathlib.Path | str, optional): The filepath to the a private key (if required) needed to
             authenticate. Defaults to None. Any keys specified here will be tried *in addition* to any keys
             specified in ``~/.ssh/`` or via a SSH agent.
         known_hosts_filename (pathlib.Path | str, optional): The filename of the known hosts file. If not specified,
             the default SSH known hosts will be used.
-        missing_host_key_policy (str | paramiko.client.MissingHostKeyPolicy): The class name or instance of
+        missing_host_key_policy (str | paramiko.client.MissingHostKeyPolicy, optional): The class name or instance of
             :class:`paramiko.client.MissingHostKeyPolicy` to use for a missing host key. Defaults to ``'RejectPolicy'``.
 
             Built-in options:
             *   ``'RejectPolicy'`` (the default), which will reject any host key not authorized in the ``known_hosts_filename``.
             *   ``'AutoAddPolicy'``, which will add any unknown host key.
             *   ``'WarningPolicy'``, which will warn on an unknown host key.
 
@@ -197,20 +197,28 @@
 
     def upload_object(
         self,
         object_name: str,
         filename: Union[str, pathlib.Path],
         callback: Optional[Callable[[int, int], None]] = None,
     ) -> None:
-        object_name = os.path.join(self.cwd, object_name)
-        dirname = os.path.dirname(object_name)
+        remote_object_name = os.path.join(self.cwd, object_name)
+        dirname = os.path.dirname(remote_object_name)
         with self._handle_transient_errors():
             if dirname:
                 self.ssh_client.exec_command(f'mkdir -p {dirname}')
-            self.sftp_client.put(str(filename), object_name, callback=callback, confirm=True)
+            self.sftp_client.put(str(filename), remote_object_name, callback=callback, confirm=False)
+            # Validating manually to raise ObjectStoreTransientErrors if the size mismatches
+            # This logic was adapted from the original source -- see
+            # https://github.com/paramiko/paramiko/blob/1824a27c644132e5d46f2294c1e2fa131c523559/paramiko/sftp_client.py#L719-L724
+            local_file_size = os.stat(filename).st_size
+            remote_file_size = self.get_object_size(object_name)
+            if local_file_size != remote_file_size:
+                raise ObjectStoreTransientError(
+                    f'Size mismatch in put: local size ({local_file_size}) != remote size ({remote_file_size})')
 
     def download_object(
         self,
         object_name: str,
         filename: Union[str, pathlib.Path],
         overwrite: bool = False,
         callback: Optional[Callable[[int, int], None]] = None,
```

### Comparing `mosaicml-0.8.2/composer/utils/reproducibility.py` & `mosaicml-0.9.0/composer/utils/reproducibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 def configure_deterministic_mode():
     """Configure PyTorch deterministic mode.
 
     .. note::
 
-        When using the :class:`~composer.trainer.trainer.Trainer`, you can use the ``deterministic_mode`` flag
+        When using the :class:`.Trainer`, you can use the ``deterministic_mode`` flag
         instead of invoking this function directly.
         For example:
 
         .. testsetup::
 
             import warnings
 
@@ -136,15 +136,15 @@
 
 
 def seed_all(seed: int):
     """Seed all rng objects.
 
     .. note::
 
-        When using the :class:`~composer.trainer.trainer.Trainer`, you can use the ``seed`` parameter
+        When using the :class:`.Trainer`, you can use the ``seed`` parameter
         instead of invoking this function directly.
         For example:
 
         .. doctest::
 
             >>> trainer = Trainer(seed=42)
```

### Comparing `mosaicml-0.8.2/composer/utils/retrying.py` & `mosaicml-0.9.0/composer/utils/retrying.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/utils/string_enum.py` & `mosaicml-0.9.0/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/bert-base.yaml` & `mosaicml-0.9.0/composer/yamls/models/bert-base.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     use_pretrained: false
     tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 
 # Train the model on the English C4 corpus
 train_dataset:
   streaming_c4:
-    remote: s3://allenai-c4/mds/1/
+    remote: s3://allenai-c4/mds/1-gz/
     local: /tmp/mds-cache/mds-c4/
     split: train
     shuffle: true
     tokenizer_name: bert-base-uncased
     max_seq_len: 128
     group_method: truncate
     mlm: true
@@ -24,19 +24,18 @@
   prefetch_factor: 2
   persistent_workers: true
   num_workers: 8
 
 # Periodically evaluate the LanguageCrossEntropy and Masked Accuracy
 # on the validation split of the dataset.
 evaluators:
-  evaluator:
-    label: bert_pre_training
+  - label: bert_pre_training
     eval_dataset:
       streaming_c4:
-        remote: s3://allenai-c4/mds/1/
+        remote: s3://allenai-c4/mds/1-gz/
         local: /tmp/mds-cache/mds-c4/
         split: val
         shuffle: false
         tokenizer_name: bert-base-uncased
         max_seq_len: 128
         group_method: truncate
         mlm: true
@@ -77,8 +76,8 @@
 
 loggers:
   progress_bar: {} # Add a TQDM progress bar
   # Optional, some nice default parameters for object store checkpointing. Uncomment this if you want to checkpoint to cloud.
   # object_store:
   #  object_store_hparams:
   #    s3:
-  #      bucket: mosaicml-internal-checkpoints-bert
+  #      bucket:
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/classify_mnist.yaml` & `mosaicml-0.9.0/composer/yamls/models/classify_mnist.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/classify_mnist_cpu.yaml` & `mosaicml-0.9.0/composer/yamls/models/classify_mnist_cpu.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/deeplabv3_ade20k_optimized.yaml` & `mosaicml-0.9.0/composer/yamls/models/deeplabv3_ade20k_optimized.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 model:
   deeplabv3:
     initializers:
       - kaiming_normal
       - bn_ones
     num_classes: 150
     backbone_arch: resnet101
-    is_backbone_pretrained: true
-    backbone_url: https://download.pytorch.org/models/resnet101-cd907fc2.pth
+    backbone_weights: IMAGENET1K_V2
     use_plus: true
     sync_bn: false
 max_duration: 128ep
 train_batch_size: 128
 eval_batch_size: 128
 seed: 17
 dataloader:
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/deeplabv3_ade20k_unoptimized.yaml` & `mosaicml-0.9.0/composer/yamls/models/deeplabv3_ade20k_unoptimized.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 model:
   deeplabv3:
     initializers:
       - kaiming_normal
       - bn_ones
     num_classes: 150
     backbone_arch: resnet101
-    is_backbone_pretrained: true
-    backbone_url: https://download.pytorch.org/models/resnet101-cd907fc2.pth
+    backbone_weights: IMAGENET1K_V1
     use_plus: true
     sync_bn: true
 max_duration: 127ep
 train_batch_size: 16
 eval_batch_size: 16
 seed: 17
 dataloader:
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/deeplabv3_streaming_ade20k_optimized.yaml` & `mosaicml-0.9.0/composer/yamls/models/deeplabv3_streaming_ade20k_optimized.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 train_dataset:
   streaming_ade20k:
-    remote: s3://mosaicml-internal-dataset-ade20k/mds/1/
+    remote: your-bucket-here
     local: /tmp/mds-cache/mds-ade20k/
     split: train
     base_size: 512
     min_resize_scale: 0.5
     max_resize_scale: 2.0
     final_size: 512
     ignore_background: true
     drop_last: true
     shuffle: true
 val_dataset:
   streaming_ade20k:
-    remote: s3://mosaicml-internal-dataset-ade20k/mds/1/
+    remote: your-bucket-here
     local: /tmp/mds-cache/mds-ade20k/
     split: val
     base_size: 512
     final_size: 512
     ignore_background: true
     drop_last: false
     shuffle: false
@@ -33,16 +33,15 @@
 model:
   deeplabv3:
     initializers:
       - kaiming_normal
       - bn_ones
     num_classes: 150
     backbone_arch: resnet101
-    is_backbone_pretrained: true
-    backbone_url: https://download.pytorch.org/models/resnet101-cd907fc2.pth
+    backbone_weights: IMAGENET1K_V2
     use_plus: true
     sync_bn: false
 max_duration: 128ep
 train_batch_size: 128
 eval_batch_size: 128
 seed: 17
 dataloader:
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/efficientnetb0.yaml` & `mosaicml-0.9.0/composer/yamls/models/efficientnetb0.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/cola.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/cola.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,31 +3,29 @@
     task: cola
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_cola
-      eval_dataset:
-        glue:
-          task: cola
-          tokenizer_name: bert-base-uncased
-          split: validation
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - MatthewsCorrCoef
+  - label: glue_cola
+    eval_dataset:
+      glue:
+        task: cola
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - MatthewsCorrCoef
 model:
   bert_classification:
     num_labels: 2
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
     lr: 5.0e-5
     betas:
       - 0.9
       - 0.98
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/mnli.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/qqp.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,54 @@
 train_dataset:
   glue:
-    task: mnli
+    task: qqp
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_mnli
-      eval_dataset:
-        glue:
-          task: mnli
-          tokenizer_name: bert-base-uncased
-          split: validation_matched
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
-  - evaluator:
-      label: glue_mnli_mismatched
-      eval_dataset:
-        glue:
-          task: mnli
-          tokenizer_name: bert-base-uncased
-          split: validation_mismatched
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
+  - label: glue_qqp
+    eval_dataset:
+      glue:
+        task: qqp
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - Accuracy
+      - BinaryF1Score
 model:
   bert_classification:
-    num_labels: 3
+    num_labels: 2
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
-    lr: 5.0e-5
+    lr: 3.0e-5
     betas:
       - 0.9
       - 0.98
     eps: 1.0e-06
-    weight_decay: 5.0e-6
+    weight_decay: 3.0e-6
 schedulers:
   - linear_decay_with_warmup:
       t_warmup: 0.06dur
-max_duration: 3ep
-train_batch_size: 48
-eval_batch_size: 48
+max_duration: 5ep
+train_batch_size: 16
+eval_batch_size: 16
 seed: 19
 dataloader:
   pin_memory: true
   persistent_workers: true
   num_workers: 8
   timeout: 0
   prefetch_factor: 2
 grad_accum: 1
-eval_interval: 2300ba
+eval_interval: 2000ba
 callbacks:
   - lr_monitor: {}
 load_path: https://storage.googleapis.com/llm_checkpoints/bert_checkpoint/bert_checkpoints/ep7.pt
 load_weights_only: true
 load_strict_model_weights: false
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/mrpc.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/mrpc.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,30 @@
     task: mrpc
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_mrpc
-      eval_dataset:
-        glue:
-          task: mrpc
-          tokenizer_name: bert-base-uncased
-          split: validation
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
-        - BinaryF1Score
+  - label: glue_mrpc
+    eval_dataset:
+      glue:
+        task: mrpc
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - Accuracy
+      - BinaryF1Score
 model:
   bert_classification:
     num_labels: 2
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
     lr: 8.0e-5
     betas:
       - 0.9
       - 0.98
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/qnli.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/qnli.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,29 @@
     task: qnli
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_qnli
-      eval_dataset:
-        glue:
-          task: qnli
-          tokenizer_name: bert-base-uncased
-          split: validation
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
+  - label: glue_qnli
+    eval_dataset:
+      glue:
+        task: qnli
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - Accuracy
 model:
   bert_classification:
     num_labels: 2
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
     lr: 1.0e-5
     betas:
       - 0.9
       - 0.98
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/qqp.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/rte.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 train_dataset:
   glue:
-    task: qqp
+    task: rte
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_qqp
-      eval_dataset:
-        glue:
-          task: qqp
-          tokenizer_name: bert-base-uncased
-          split: validation
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
-        - BinaryF1Score
+  - label: glue_rte
+    eval_dataset:
+      glue:
+        task: rte
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - Accuracy
 model:
   bert_classification:
     num_labels: 2
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
-    lr: 3.0e-5
+    lr: 1.0e-5
     betas:
       - 0.9
       - 0.98
     eps: 1.0e-06
-    weight_decay: 3.0e-6
+    weight_decay: 1.0e-5
 schedulers:
   - linear_decay_with_warmup:
       t_warmup: 0.06dur
-max_duration: 5ep
+max_duration: 3ep
 train_batch_size: 16
 eval_batch_size: 16
 seed: 19
 dataloader:
   pin_memory: true
   persistent_workers: true
   num_workers: 8
   timeout: 0
   prefetch_factor: 2
 grad_accum: 1
-eval_interval: 2000ba
+eval_interval: 1000ba
 callbacks:
   - lr_monitor: {}
 load_path: https://storage.googleapis.com/llm_checkpoints/bert_checkpoint/bert_checkpoints/ep7.pt
 load_weights_only: true
 load_strict_model_weights: false
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/rte.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/sst-2.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 train_dataset:
   glue:
-    task: rte
+    task: sst2
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_rte
-      eval_dataset:
-        glue:
-          task: rte
-          tokenizer_name: bert-base-uncased
-          split: validation
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
+  - label: glue_sst2
+    eval_dataset:
+      glue:
+        task: sst2
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - Accuracy
 model:
   bert_classification:
     num_labels: 2
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
-    lr: 1.0e-5
+    lr: 3.0e-5
     betas:
       - 0.9
       - 0.98
     eps: 1.0e-06
-    weight_decay: 1.0e-5
+    weight_decay: 3.0e-6
 schedulers:
   - linear_decay_with_warmup:
       t_warmup: 0.06dur
 max_duration: 3ep
 train_batch_size: 16
 eval_batch_size: 16
 seed: 19
 dataloader:
   pin_memory: true
   persistent_workers: true
   num_workers: 8
   timeout: 0
   prefetch_factor: 2
 grad_accum: 1
-eval_interval: 1000ba
+eval_interval: 500ba
 callbacks:
   - lr_monitor: {}
 load_path: https://storage.googleapis.com/llm_checkpoints/bert_checkpoint/bert_checkpoints/ep7.pt
 load_weights_only: true
 load_strict_model_weights: false
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/glue/sst-2.yaml` & `mosaicml-0.9.0/composer/yamls/models/glue/stsb.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 train_dataset:
   glue:
-    task: sst2
+    task: stsb
     tokenizer_name: bert-base-uncased
     split: train
     max_seq_length: 256
     shuffle: false
     drop_last: false
 evaluators:
-  - evaluator:
-      label: glue_sst2
-      eval_dataset:
-        glue:
-          task: sst2
-          tokenizer_name: bert-base-uncased
-          split: validation
-          max_seq_length: 256
-          shuffle: false
-          drop_last: false
-      metric_names:
-        - Accuracy
+  - label: glue_stsb
+    eval_dataset:
+      glue:
+        task: stsb
+        tokenizer_name: bert-base-uncased
+        split: validation
+        max_seq_length: 256
+        shuffle: false
+        drop_last: false
+    metric_names:
+      - SpearmanCorrCoef
 model:
   bert_classification:
-    num_labels: 2
+    num_labels: 1
     use_pretrained: true
-    tokenizer_name: bert-base-uncased
     pretrained_model_name: bert-base-uncased
 optimizers:
   decoupled_adamw:
     lr: 3.0e-5
     betas:
       - 0.9
       - 0.98
     eps: 1.0e-06
     weight_decay: 3.0e-6
 schedulers:
   - linear_decay_with_warmup:
       t_warmup: 0.06dur
-max_duration: 3ep
-train_batch_size: 16
-eval_batch_size: 16
+max_duration: 10ep
+train_batch_size: 32
+eval_batch_size: 32
 seed: 19
 dataloader:
   pin_memory: true
   persistent_workers: true
   num_workers: 8
   timeout: 0
   prefetch_factor: 2
 grad_accum: 1
-eval_interval: 500ba
+eval_interval: 200ba
 callbacks:
   - lr_monitor: {}
 load_path: https://storage.googleapis.com/llm_checkpoints/bert_checkpoint/bert_checkpoints/ep7.pt
 load_weights_only: true
 load_strict_model_weights: false
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_1,3b.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_1,3b.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_125m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_125m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_13b.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_13b.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_2,7b.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_2,7b.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_350m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_350m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_52m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_52m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_6,7b.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_6,7b.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_760m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_760m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt2_83m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt2_83m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt3_125m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt3_125m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt3_350m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt3_350m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/gpt3_760m.yaml` & `mosaicml-0.9.0/composer/yamls/models/gpt3_760m.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet101.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet101.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet101_synthetic.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet101_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet152.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet152.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet152_synthetic.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet152_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet18.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet18.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet18_synthetic.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet18_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet20_cifar10.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet20_cifar10.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet34.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet34.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet34_synthetic.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet34_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet50.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet50.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet50_streaming.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet50_streaming.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 train_dataset:
   streaming_imagenet1k:
-    remote: s3://mosaicml-internal-dataset-imagenet1k/mds/1/
+    remote: your-bucket-here
     local: /tmp/mds-cache/mds-imagenet1k/
     split: train
     resize_size: -1
     crop_size: 224
     shuffle: true
     drop_last: true
 val_dataset:
   streaming_imagenet1k:
-    remote: s3://mosaicml-internal-dataset-imagenet1k/mds/1/
+    remote: your-bucket-here
     local: /tmp/mds-cache/mds-imagenet1k/
     split: val
     resize_size: 256
     crop_size: 224
     shuffle: false
     drop_last: false
 optimizers:
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet50_synthetic.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet50_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet56_cifar10.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet56_cifar10.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet56_cifar10_synthetic.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet56_cifar10_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/resnet9_cifar10.yaml` & `mosaicml-0.9.0/composer/yamls/models/resnet9_cifar10.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/timm_resnet50_imagenet.yaml` & `mosaicml-0.9.0/composer/yamls/models/timm_resnet50_imagenet.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/timm_vit_small_patch16.yaml` & `mosaicml-0.9.0/composer/yamls/models/timm_vit_small_patch16.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     crop_size: 224
     is_train: false
     datadir: /datasets/ImageNet
     shuffle: false
     drop_last: false
 optimizers:
   adamw:
-    lr: 3e-3
+    lr: 3.0e-3
     betas:
       - 0.9
       - 0.999
     eps: 1.0e-08
     weight_decay: 0.3
 schedulers:
   - cosine_decay_with_warmup:
```

### Comparing `mosaicml-0.8.2/composer/yamls/models/unet.yaml` & `mosaicml-0.9.0/composer/yamls/models/unet.yaml`

 * *Files identical despite different names*

### Comparing `mosaicml-0.8.2/composer/yamls/models/vit_small_patch16.yaml` & `mosaicml-0.9.0/composer/yamls/models/vit_small_patch16.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     crop_size: 224
     is_train: false
     datadir: /datasets/ImageNet
     shuffle: false
     drop_last: false
 optimizers:
   adamw:
-    lr: 3e-3
+    lr: 3.0e-3
     betas:
       - 0.9
       - 0.999
     eps: 1.0e-08
     weight_decay: 0.3
 schedulers:
   - cosine_decay_with_warmup:
```

### Comparing `mosaicml-0.8.2/composer/yamls/recipes/resnet50_medium.yaml` & `mosaicml-0.9.0/composer/yamls/recipes/resnet50_medium.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 algorithms:
-  blurpool:
-    blur_first: true
-    min_channels: 16
-    replace_convs: true
-    replace_maxpools: true
-  channels_last: {}
-  ema:
-    half_life: 100ba
-    train_with_ema_weights: false
-    update_interval: 20ba
-  label_smoothing:
-    smoothing: 0.1
-  mixup:
-    alpha: 0.2
-    interpolate_loss: false
-  progressive_resizing:
-    delay_fraction: 0.4
-    finetune_fraction: 0.2
-    initial_scale: 0.5
-    mode: resize
-    resize_targets: false
-    size_increment: 4
-  sam:
-    epsilon: 1.0e-12
-    interval: 10
-    rho: 0.5
+  - blurpool:
+      blur_first: true
+      min_channels: 16
+      replace_convs: true
+      replace_maxpools: true
+  - channels_last: {}
+  - ema:
+      half_life: 100ba
+      train_with_ema_weights: false
+      update_interval: 20ba
+  - label_smoothing:
+      smoothing: 0.1
+  - mixup:
+      alpha: 0.2
+      interpolate_loss: false
+  - progressive_resizing:
+      delay_fraction: 0.4
+      finetune_fraction: 0.2
+      initial_scale: 0.5
+      mode: resize
+      resize_targets: false
+      size_increment: 4
+  - sam:
+      epsilon: 1.0e-12
+      interval: 10
+      rho: 0.5
 callbacks:
-  lr_monitor: {}
-  speed_monitor:
-    window_size: 100
+  - lr_monitor: {}
+  - speed_monitor:
+      window_size: 100
 dataloader:
   num_workers: 8
   persistent_workers: true
   pin_memory: true
   prefetch_factor: 2
   timeout: 0.0
 device:
   gpu: {}
 eval_batch_size: 2048
 eval_interval: 1
 loggers:
-  progress_bar:
-    console_log_level: EPOCH
-    stream: stderr
+  - progress_bar:
+      console_log_level: EPOCH
+      stream: stderr
 model:
   resnet:
     initializers:
       - KAIMING_NORMAL
       - BN_UNIFORM
       - LINEAR_LOG_CONSTANT_BIAS
     loss_name: binary_cross_entropy_with_logits
```

### Comparing `mosaicml-0.8.2/composer/yamls/recipes/resnet50_mild.yaml` & `mosaicml-0.9.0/composer/yamls/recipes/resnet50_mild.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 algorithms:
-  blurpool:
-    blur_first: true
-    min_channels: 16
-    replace_convs: true
-    replace_maxpools: true
-  channels_last: {}
-  ema:
-    half_life: 100ba
-    train_with_ema_weights: false
-    update_interval: 20ba
-  label_smoothing:
-    smoothing: 0.08
-  progressive_resizing:
-    delay_fraction: 0.4
-    finetune_fraction: 0.2
-    initial_scale: 0.5
-    mode: resize
-    resize_targets: false
-    size_increment: 4
+  - blurpool:
+      blur_first: true
+      min_channels: 16
+      replace_convs: true
+      replace_maxpools: true
+  - channels_last: {}
+  - ema:
+      half_life: 100ba
+      train_with_ema_weights: false
+      update_interval: 20ba
+  - label_smoothing:
+      smoothing: 0.08
+  - progressive_resizing:
+      delay_fraction: 0.4
+      finetune_fraction: 0.2
+      initial_scale: 0.5
+      mode: resize
+      resize_targets: false
+      size_increment: 4
 callbacks:
-  lr_monitor: {}
-  speed_monitor:
-    window_size: 100
+  - lr_monitor: {}
+  - speed_monitor:
+      window_size: 100
 dataloader:
   num_workers: 8
   persistent_workers: true
   pin_memory: true
   prefetch_factor: 2
   timeout: 0.0
 device:
   gpu: {}
 eval_batch_size: 2048
 eval_interval: 1
 loggers:
-  progress_bar:
-    console_log_level: EPOCH
-    stream: stderr
+  - progress_bar:
+      console_log_level: EPOCH
+      stream: stderr
 model:
   resnet:
     initializers:
       - KAIMING_NORMAL
       - BN_UNIFORM
       - LINEAR_LOG_CONSTANT_BIAS
     loss_name: binary_cross_entropy_with_logits
```

### Comparing `mosaicml-0.8.2/composer/yamls/recipes/resnet50_spicy.yaml` & `mosaicml-0.9.0/composer/yamls/recipes/resnet50_spicy.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 algorithms:
-  blurpool:
-    blur_first: true
-    min_channels: 16
-    replace_convs: true
-    replace_maxpools: true
-  channels_last: {}
-  colout:
-    batch: true
-    p_col: 0.05
-    p_row: 0.05
-    resize_target: auto
-  ema:
-    half_life: 100ba
-    train_with_ema_weights: false
-    update_interval: 20ba
-  label_smoothing:
-    smoothing: 0.13
-  mixup:
-    alpha: 0.25
-    interpolate_loss: false
-  progressive_resizing:
-    delay_fraction: 0.2
-    finetune_fraction: 0.2
-    initial_scale: 0.6
-    mode: resize
-    resize_targets: false
-    size_increment: 4
-  randaugment:
-    augmentation_set: all
-    depth: 1
-    severity: 10
-  sam:
-    epsilon: 1.0e-12
-    interval: 5
-    rho: 0.5
-  stochastic_depth:
-    drop_distribution: linear
-    drop_rate: 0.1
-    drop_warmup: 0.0dur
-    stochastic_method: sample
-    target_layer_name: ResNetBottleneck
+  - blurpool:
+      blur_first: true
+      min_channels: 16
+      replace_convs: true
+      replace_maxpools: true
+  - channels_last: {}
+  - colout:
+      batch: true
+      p_col: 0.05
+      p_row: 0.05
+      resize_target: auto
+  - ema:
+      half_life: 100ba
+      train_with_ema_weights: false
+      update_interval: 20ba
+  - label_smoothing:
+      smoothing: 0.13
+  - mixup:
+      alpha: 0.25
+      interpolate_loss: false
+  - progressive_resizing:
+      delay_fraction: 0.2
+      finetune_fraction: 0.2
+      initial_scale: 0.6
+      mode: resize
+      resize_targets: false
+      size_increment: 4
+  - randaugment:
+      augmentation_set: all
+      depth: 1
+      severity: 10
+  - sam:
+      epsilon: 1.0e-12
+      interval: 5
+      rho: 0.5
+  - stochastic_depth:
+      drop_distribution: linear
+      drop_rate: 0.1
+      drop_warmup: 0.0dur
+      stochastic_method: sample
+      target_layer_name: ResNetBottleneck
 callbacks:
-  lr_monitor: {}
-  speed_monitor:
-    window_size: 100
+  - lr_monitor: {}
+  - speed_monitor:
+      window_size: 100
 dataloader:
   num_workers: 8
   persistent_workers: true
   pin_memory: true
   prefetch_factor: 2
   timeout: 0.0
 device:
   gpu: {}
 eval_batch_size: 2048
 loggers:
-  progress_bar:
-    console_log_level: EPOCH
-    stream: stderr
+  - progress_bar:
+      console_log_level: EPOCH
+      stream: stderr
 model:
   resnet:
     groups: 1
     initializers:
       - KAIMING_NORMAL
       - BN_UNIFORM
       - LINEAR_LOG_CONSTANT_BIAS
```

### Comparing `mosaicml-0.8.2/mosaicml.egg-info/PKG-INFO` & `mosaicml-0.9.0/mosaicml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml
-Version: 0.8.2
+Version: 0.9.0
 Summary: Composer provides well-engineered implementations of efficient training methods to give the tools that help you train a better model for cheaper.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -97,21 +97,21 @@
 <!-- end numbers -->
 
 # 🚀 Quickstart
 
 ## 💾 Installation
 Composer is available with Pip:
 
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.skip-->
 ```bash
 pip install mosaicml
 ```
 Alternatively, install Composer with Conda:
 
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.skip-->
 ```bash
 conda install -c mosaicml mosaicml
 ```
 ---
 
 ## 🚌 Usage
 
@@ -142,39 +142,48 @@
 For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/latest/functional_api.html).
 
 ### Example: Trainer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/getting_started.ipynb)
 
 For the best experience and the most efficient possible training, we recommend using Composer's built-in trainer, which automatically takes care of the low-level details of using speedup methods and provides useful abstractions that facilitate rapid experimentation.
 
 <!-- begin_example_2 --->
-<!-- TODO: Address timeouts -->
-<!--pytest-codeblocks:skip-->
+<!--pytest.mark.gpu-->
+<!--pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')-->
+<!--
+```python
+import torch
+
+# adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
+torch.use_deterministic_algorithms(False)
+
+```
+-->
+<!--pytest-codeblocks:cont-->
 ```python
 from torch.utils.data import DataLoader
 from torchvision import datasets, transforms
 
 from composer import Trainer
-from composer.algorithms import BlurPool, ChannelsLast, CutMix, LabelSmoothing
-from composer.models import MNIST_Classifier
+from composer.algorithms import ChannelsLast, CutMix, LabelSmoothing
+from composer.models import mnist_model
 
 transform = transforms.Compose([transforms.ToTensor()])
 train_dataset = datasets.MNIST("data", download=True, train=True, transform=transform)
 eval_dataset = datasets.MNIST("data", download=True, train=False, transform=transform)
 train_dataloader = DataLoader(train_dataset, batch_size=128)
 eval_dataloader = DataLoader(eval_dataset, batch_size=128)
 
 trainer = Trainer(
-    model=MNIST_Classifier(num_classes=10),
+    model=mnist_model(),
     train_dataloader=train_dataloader,
     eval_dataloader=eval_dataloader,
     max_duration="2ep",
     algorithms=[
-        BlurPool(replace_convs=True, replace_maxpools=True, blur_first=True),
         ChannelsLast(),
-        CutMix(num_classes=10),
+        CutMix(alpha=1.0),
         LabelSmoothing(smoothing=0.1),
     ]
 )
 trainer.fit()
 ```
 <!-- end_example_2 -->
 
@@ -368,15 +377,15 @@
   <tr>
     <td><a href="https://mosaicml.com/jobs" target="_blank" rel="noopener noreferrer">We're Hiring!</a></td>
     <td>Join us! 🤩</td>
   </tr>
 </tbody>
 </table>
 
-If you have any questions, please feel free to reach out to us on [Twitter](https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg)!
+If you have any questions, please feel free to reach out to us on [Twitter](https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-1dc6mo5wg-arlv6Oo9JjEn_g4d5s7PXQ)!
 
 # 💫 Contributors
 Composer is part of the broader Machine Learning community, and we welcome any contributions, pull requests, or issues!
 
 To start contributing, see our [Contributing](https://github.com/mosaicml/composer/blob/dev/CONTRIBUTING.md) page.
 
 # ✍️ Citation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml Version: 0.8.2 Summary: Composer provides
+Metadata-Version: 2.1 Name: mosaicml Version: 0.9.0 Summary: Composer provides
 well-engineered implementations of efficient training methods to give the tools
 that help you train a better model for cheaper. Home-page: https://github.com/
 mosaicml/composer Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: base Provides-Extra: dev Provides-
@@ -61,35 +61,33 @@
 functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/
 latest/functional_api.html). ### Example: Trainer [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 getting_started.ipynb) For the best experience and the most efficient possible
 training, we recommend using Composer's built-in trainer, which automatically
 takes care of the low-level details of using speedup methods and provides
-useful abstractions that facilitate rapid experimentation.    ```python from
+useful abstractions that facilitate rapid experimentation.      ```python from
 torch.utils.data import DataLoader from torchvision import datasets, transforms
-from composer import Trainer from composer.algorithms import BlurPool,
-ChannelsLast, CutMix, LabelSmoothing from composer.models import
-MNIST_Classifier transform = transforms.Compose([transforms.ToTensor()])
-train_dataset = datasets.MNIST("data", download=True, train=True,
-transform=transform) eval_dataset = datasets.MNIST("data", download=True,
-train=False, transform=transform) train_dataloader = DataLoader(train_dataset,
-batch_size=128) eval_dataloader = DataLoader(eval_dataset, batch_size=128)
-trainer = Trainer( model=MNIST_Classifier(num_classes=10),
-train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
-max_duration="2ep", algorithms=[ BlurPool(replace_convs=True,
-replace_maxpools=True, blur_first=True), ChannelsLast(), CutMix
-(num_classes=10), LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```
-Composer's built-in [trainer](https://docs.mosaicml.com/en/stable/trainer/
-using_the_trainer.html) makes it easy to **add multiple speedup methods in a
-single line of code!** Trying out new methods or combinations of methods is as
-easy as changing a single list. As we continually implement more methods, they
-will be easy for you to add to your code. For concrete examples of methods in
-Composer, here are some ([_see here for all_](https://docs.mosaicml.com/en/
-latest/trainer/algorithms.html)) speedup methods currently in Composer:
+from composer import Trainer from composer.algorithms import ChannelsLast,
+CutMix, LabelSmoothing from composer.models import mnist_model transform =
+transforms.Compose([transforms.ToTensor()]) train_dataset = datasets.MNIST
+("data", download=True, train=True, transform=transform) eval_dataset =
+datasets.MNIST("data", download=True, train=False, transform=transform)
+train_dataloader = DataLoader(train_dataset, batch_size=128) eval_dataloader =
+DataLoader(eval_dataset, batch_size=128) trainer = Trainer( model=mnist_model
+(), train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
+max_duration="2ep", algorithms=[ ChannelsLast(), CutMix(alpha=1.0),
+LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```  Composer's built-in
+[trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html)
+makes it easy to **add multiple speedup methods in a single line of code!**
+Trying out new methods or combinations of methods is as easy as changing a
+single list. As we continually implement more methods, they will be easy for
+you to add to your code. For concrete examples of methods in Composer, here are
+some ([_see here for all_](https://docs.mosaicml.com/en/latest/trainer/
+algorithms.html)) speedup methods currently in Composer:
 Name|Attribution|tl;dr|Example Benchmark|Speed Up*| ----|-----------|-----|----
 -----|---------| [Alibi](https://github.com/mosaicml/composer/tree/dev/
 composer/algorithms/alibi)|[Press et al, 2021](https://arxiv.org/abs/
 2108.12409)|Replace attention with AliBi.|GPT-2|1.5x [BlurPool](https://
 github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|[Zhang,
 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter before
 every downsampling operation.|ResNet-101|1.2x [ChannelsLast](https://
@@ -238,14 +236,14 @@
                                         An interactive Colab Notebook aimed at
 Training_BERTs_with_Composer            helping users learn how to train BERT
                                         models with Composer!
 We're_Hiring!                           Join us! ð¤©
 If you have any questions, please feel free to reach out to us on [Twitter]
 (https://twitter.com/mosaicml), [email](mailto:community@mosaicml.com), or our
 [Community Slack](https://join.slack.com/t/mosaicml-community/shared_invite/zt-
-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg)! # ð« Contributors Composer is part of the
+1dc6mo5wg-arlv6Oo9JjEn_g4d5s7PXQ)! # ð« Contributors Composer is part of the
 broader Machine Learning community, and we welcome any contributions, pull
 requests, or issues! To start contributing, see our [Contributing](https://
 github.com/mosaicml/composer/blob/dev/CONTRIBUTING.md) page. # âï¸ Citation
 ``` @misc{mosaicml2022composer, author = {The Mosaic ML Team}, title =
 {composer}, year = {2021}, howpublished = {\url{https://github.com/mosaicml/
 composer/}}, } ```
```

### Comparing `mosaicml-0.8.2/mosaicml.egg-info/SOURCES.txt` & `mosaicml-0.9.0/mosaicml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 composer/__init__.py
 composer/__main__.py
+composer/_version.py
 composer/py.typed
 composer/algorithms/__init__.py
 composer/algorithms/algorithm_hparams_registry.py
 composer/algorithms/warnings.py
 composer/algorithms/alibi/__init__.py
-composer/algorithms/alibi/_gpt2_alibi.py
 composer/algorithms/alibi/alibi.py
 composer/algorithms/alibi/metadata.json
+composer/algorithms/alibi/attention_surgery_functions/__init__.py
+composer/algorithms/alibi/attention_surgery_functions/_bert.py
+composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+composer/algorithms/alibi/attention_surgery_functions/utils.py
 composer/algorithms/augmix/__init__.py
 composer/algorithms/augmix/augmix.py
 composer/algorithms/augmix/metadata.json
 composer/algorithms/blurpool/__init__.py
 composer/algorithms/blurpool/blurpool.py
 composer/algorithms/blurpool/blurpool_layers.py
 composer/algorithms/blurpool/metadata.json
@@ -93,14 +97,15 @@
 composer/algorithms/utils/__init__.py
 composer/algorithms/utils/augmentation_common.py
 composer/algorithms/utils/augmentation_primitives.py
 composer/callbacks/__init__.py
 composer/callbacks/callback_hparams_registry.py
 composer/callbacks/checkpoint_saver.py
 composer/callbacks/early_stopper.py
+composer/callbacks/export_for_inference.py
 composer/callbacks/grad_monitor.py
 composer/callbacks/image_visualizer.py
 composer/callbacks/lr_monitor.py
 composer/callbacks/memory_monitor.py
 composer/callbacks/mlperf.py
 composer/callbacks/speed_monitor.py
 composer/callbacks/threshold_stopper.py
@@ -110,14 +115,15 @@
 composer/core/__init__.py
 composer/core/algorithm.py
 composer/core/callback.py
 composer/core/data_spec.py
 composer/core/engine.py
 composer/core/evaluator.py
 composer/core/event.py
+composer/core/passes.py
 composer/core/precision.py
 composer/core/serializable.py
 composer/core/state.py
 composer/core/time.py
 composer/core/types.py
 composer/datasets/__init__.py
 composer/datasets/ade20k.py
@@ -167,25 +173,23 @@
 composer/metrics/metrics.py
 composer/metrics/nlp.py
 composer/models/__init__.py
 composer/models/base.py
 composer/models/huggingface.py
 composer/models/initializers.py
 composer/models/model_hparams.py
-composer/models/transformer_hparams.py
-composer/models/transformer_shared.py
 composer/models/bert/__init__.py
 composer/models/bert/bert_hparams.py
 composer/models/bert/model.py
 composer/models/classify_mnist/__init__.py
 composer/models/classify_mnist/mnist_hparams.py
 composer/models/classify_mnist/model.py
 composer/models/deeplabv3/__init__.py
-composer/models/deeplabv3/deeplabv3.py
 composer/models/deeplabv3/deeplabv3_hparams.py
+composer/models/deeplabv3/model.py
 composer/models/efficientnetb0/__init__.py
 composer/models/efficientnetb0/_layers.py
 composer/models/efficientnetb0/efficientnetb0_hparams.py
 composer/models/efficientnetb0/efficientnets.py
 composer/models/efficientnetb0/model.py
 composer/models/gpt2/__init__.py
 composer/models/gpt2/gpt2_hparams.py
@@ -240,22 +244,25 @@
 composer/trainer/trainer.py
 composer/trainer/trainer_hparams.py
 composer/trainer/devices/__init__.py
 composer/trainer/devices/device.py
 composer/trainer/devices/device_cpu.py
 composer/trainer/devices/device_gpu.py
 composer/trainer/devices/device_hparams_registry.py
+composer/trainer/devices/device_mps.py
+composer/trainer/devices/device_tpu.py
 composer/utils/__init__.py
 composer/utils/batch_helpers.py
 composer/utils/checkpoint.py
 composer/utils/collect_env.py
 composer/utils/dist.py
 composer/utils/file_helpers.py
 composer/utils/fx_utils.py
 composer/utils/import_helpers.py
+composer/utils/inference.py
 composer/utils/iter_helpers.py
 composer/utils/misc.py
 composer/utils/module_surgery.py
 composer/utils/reproducibility.py
 composer/utils/retrying.py
 composer/utils/string_enum.py
 composer/utils/object_store/__init__.py
```

### Comparing `mosaicml-0.8.2/mosaicml.egg-info/requires.txt` & `mosaicml-0.9.0/mosaicml.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 pyyaml<7,>=6.0
 tqdm<5,>=4.62.3
 torchmetrics<0.8,>=0.7.0
 torch_optimizer<0.2,>=0.1.0
 torchvision>=0.10.0
-torch<2,>=1.9
-yahp<0.2,>=0.1.1
+torch<2,>=1.10
+yahp<0.2,>=0.1.3
 requests<3,>=2.26.0
-numpy<2,>=1.21.5
+numpy<1.23.0,>=1.21.5
 psutil<6,>=5.8.0
 coolname<2,>=1.1.0
-py-cpuinfo>=8.0.0
+tabulate==0.8.9
+py-cpuinfo<9,>=8.0.0
+packaging<22,>=21.3.0
+importlib-metadata<5,>=4.11.0
 
 [all]
-fasteners==0.17.3
-sphinxext.opengraph==0.6.1
+pycocotools<3,>=2.0.4
+sphinxcontrib-images==0.9.4
+onnxruntime<2,>=1.11.0
+pytest_codeblocks==0.16.1
+jupyter==1.0.0
+pytest-httpserver<1.1,>=1.0.4
+scikit-learn<2,>=1.0.1
+recommonmark==0.7.1
+yamllint==1.26.3
+timm<0.6,>=0.5.4
 testbook==0.4.2
+datasets<2,>=1.14
+onnx<2,>=1.11.0
+myst-parser==0.16.1
+traitlets==5.1.1
 sphinx-argparse==0.3.1
-toml==0.10.2
-sphinxcontrib-images==0.9.4
+custom_inherit==2.3.2
 pytest==7.1.0
-jupyter==1.0.0
+sphinx-copybutton==0.5.0
+pypandoc==1.8.1
+deepspeed==0.5.10
 vit_pytorch==0.27
-datasets<2,>=1.14
-pre-commit<3,>=2.18.1
-apache-libcloud<4,>=3.3.1
+sphinxemoji==0.2.0
 sphinx_markdown_tables==0.0.15
-ipython==7.32.0
-transformers<5,>=4.11
-junitparser==2.4.3
-pytest_codeblocks==0.15.0
-nbsphinx==0.8.8
-timm<0.6,>=0.5.4
-deepspeed==0.5.10
-coverage[toml]==6.3.2
-cryptography==37.0.2
-sphinx==4.4.0
 wandb<0.13,>=0.12.17
+tensorflow-io<0.27,>=0.26.0
+ipykernel==6.9.2
+cryptography==37.0.2
 boto3<2,>=1.21.45
-myst-parser==0.16.1
-tensorboard<3.0.0,>=2.9.1
-py-cpuinfo<9,>=8.0.0
-furo==2022.3.4
-recommonmark==0.7.1
-sphinx-copybutton==0.5.0
-tabulate==0.8.9
 sphinxcontrib.katex==0.8.6
-monai<0.9,>=0.8.0
 pandoc==2.2
+ipython==7.32.0
+nbsphinx==0.8.8
+transformers<5,>=4.11
 sphinx_panels==0.6.0
-pycocotools<3,>=2.0.4
-paramiko<3,>=2.11.0
-onnxruntime<2,>=1.11.0
-pypandoc==1.8.1
-yamllint==1.26.3
+toml==0.10.2
+monai<0.9,>=0.8.0
+tensorboard<3.0.0,>=2.9.1
+junitparser==2.4.3
+furo==2022.3.4
+sphinxext.opengraph==0.6.1
+coverage[toml]==6.3.2
 moto[s3]<3.2,>=3.1.12
-custom_inherit==2.3.2
-scikit-learn<2,>=1.0.1
+fasteners==0.17.3
+sphinx==4.4.0
+pre-commit<3,>=2.18.1
+docutils==0.17.1
 GitPython==3.1.27
-pytest-httpserver<1.1,>=1.0.4
-ipykernel==6.9.2
-sphinxemoji==0.2.0
-pytest-timeout==2.1.0
 mock-ssh-server==0.9.1
-docutils==0.17.1
-onnx<2,>=1.11.0
-traitlets==5.1.1
+py-cpuinfo<9,>=8.0.0
+paramiko<3,>=2.11.0
+apache-libcloud<4,>=3.3.1
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [deepspeed]
@@ -81,32 +83,30 @@
 fasteners==0.17.3
 pytest==7.1.0
 toml==0.10.2
 ipython==7.32.0
 ipykernel==6.9.2
 jupyter==1.0.0
 yamllint==1.26.3
-pytest-timeout==2.1.0
 recommonmark==0.7.1
 sphinx==4.4.0
 pre-commit<3,>=2.18.1
 docutils==0.17.1
 sphinx_markdown_tables==0.0.15
 sphinx-argparse==0.3.1
 sphinxcontrib.katex==0.8.6
 sphinxext.opengraph==0.6.1
 sphinxemoji==0.2.0
 furo==2022.3.4
 sphinx-copybutton==0.5.0
-tabulate==0.8.9
 testbook==0.4.2
 myst-parser==0.16.1
 sphinx_panels==0.6.0
 sphinxcontrib-images==0.9.4
-pytest_codeblocks==0.15.0
+pytest_codeblocks==0.16.1
 traitlets==5.1.1
 nbsphinx==0.8.8
 pandoc==2.2
 pypandoc==1.8.1
 GitPython==3.1.27
 moto[s3]<3.2,>=3.1.12
 mock-ssh-server==0.9.1
@@ -129,14 +129,15 @@
 
 [streaming]
 boto3<2,>=1.21.45
 paramiko<3,>=2.11.0
 
 [tensorboard]
 tensorboard<3.0.0,>=2.9.1
+tensorflow-io<0.27,>=0.26.0
 
 [timm]
 timm<0.6,>=0.5.4
 
 [unet]
 monai<0.9,>=0.8.0
 scikit-learn<2,>=1.0.1
```

### Comparing `mosaicml-0.8.2/pyproject.toml` & `mosaicml-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,14 @@
 reportUnusedCoroutine = "error"
 
 # Pytest
 [tool.pytest.ini_options]
 # By default, do not run gpu, vision, notebook, or daily tests
 addopts = "--codeblocks --strict-markers -m 'not gpu and not vision and not daily and not remote'"
 
-# by default, tests should be fast.
-# for slower tests, use @pytest.mark.timeout with a higher timeout (specified in seconds)
-timeout = 2
 markers = [
     # !!!!!!!!!!!IMPORTANT!!!!!!!!!: when updating the markers, also make sure to update .ci/Jenkinsfile and meta.yaml
     # Tests that require a world_size of two should be annotated with `@pytest.mark.world_size(2)`.
     # If not specified, the test will be assumed to have a world-size of one, which is
     # equivalent to `@pytest.mark.world_size(1)`
     "world_size(val)",
     # Tests that require a gpu should be annotated with `@pytest.mark.gpu`
@@ -94,33 +91,33 @@
     'ignore:No optimizer was specified.:UserWarning',  # OK to not specify an optimizer in the tests
     # Ignore deprecation warnings in pillow. TODO: remove this ignore for when we upgrade pillow-simd +
     # use torchvision 0.13  -- it appears to be fixed in main -- see
     # https://github.com/pytorch/vision/blob/main/torchvision/transforms/functional_pil.py
     'ignore:.*is deprecated and will be removed in Pillow 10.*:DeprecationWarning',
     # Ignore deprecation warnings in deepspeed. TODO: remove this when we upgrade to v0.6.1+ -- it has been fixed
     'ignore::DeprecationWarning:deepspeed.*:',
-    # Ignore malformed yaml warnings coming from yahp
-    'ignore:MalformedYAMLWarning:UserWarning',
     # Ingore validate is deprecated warnings. TODO(ravi) Need to manually remove on hparams.validate functionality
     'ignore:.*Instead, perform any validation directly in initialize_object\(\):DeprecationWarning',
     # Ignore a bug in the pytorch dataloader
     '''ignore:Exception ignored in. <function _MultiProcessingDataLoaderIter.__del__:pytest.PytestUnraisableExceptionWarning''',
     # Ignore torchvision complaining about no c libraries (happens in the conda build)
     'ignore:Failed to load image Python extension:UserWarning',
     # Ignore a deprecation warning in the conda build
     'ignore:distutils Version classes are deprecated:DeprecationWarning',
     # Ignore a UserWarning from TorchMetrics about potentially large memory usage when batch sizes are extremely large
     'ignore:Metric `SpearmanCorrcoef` will save all targets and predictions in the buffer:UserWarning:torchmetrics',
+    # Ignore a UserWarning from torch 1.12 due to DeepSpeed's use of positional args
+    'ignore:Positional args are being deprecated, use kwargs instead.*:UserWarning',
 ]
-timeout_func_only = true  # exclude fixtures from the timeout
 
 # Coverage
 [tool.coverage.run]
 parallel = true
 branch = true
+relative_files = true
 concurrency = ["thread"]
 include = [
     "composer/*"
 ]
 
 # Yapf
 [tool.yapf]
```

### Comparing `mosaicml-0.8.2/setup.py` & `mosaicml-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 import sys
 import textwrap
 
 import setuptools
 from setuptools import setup
 from setuptools.command.develop import develop as develop_orig
 
+# Read the composer version
+# Cannot import from `composer.__version__` since that will not be available when building or installing the package
+with open(os.path.join(os.path.dirname(__file__), 'composer', '_version.py')) as f:
+    version_globals = {}
+    version_locals = {}
+    exec(f.read(), version_globals, version_locals)
+    composer_version = version_locals['__version__']
+
 _IS_ROOT = os.getuid() == 0
 _IS_USER = '--user' in sys.argv[1:]
 _IS_VIRTUALENV = 'VIRTUAL_ENV' in os.environ
 
 
 # From https://stackoverflow.com/questions/51292333/how-to-tell-from-setup-py-if-the-module-is-being-installed-in-editable-mode
 class develop(develop_orig):
@@ -66,21 +74,24 @@
 
 install_requires = [
     'pyyaml>=6.0,<7',
     'tqdm>=4.62.3,<5',
     'torchmetrics>=0.7.0,<0.8',
     'torch_optimizer>=0.1.0,<0.2',
     'torchvision>=0.10.0',  # torchvision has strict pytorch requirements
-    'torch>=1.9,<2',
-    'yahp>=0.1.1,<0.2',
+    'torch>=1.10,<2',
+    'yahp>=0.1.3,<0.2',
     'requests>=2.26.0,<3',
-    'numpy>=1.21.5,<2',
+    'numpy>=1.21.5,<1.23.0',
     'psutil>=5.8.0,<6',
     'coolname>=1.1.0,<2',
-    'py-cpuinfo>=8.0.0',
+    'tabulate==0.8.9',  # for auto-generating tables
+    'py-cpuinfo>=8.0.0,<9',
+    'packaging>=21.3.0,<22',
+    'importlib-metadata>=4.11.0,<5',
 ]
 extra_deps = {}
 
 extra_deps['base'] = []
 
 extra_deps['dev'] = [
     # Imports for docs builds and running tests
@@ -92,34 +103,32 @@
     'fasteners==0.17.3',  # object store tests require fasteners
     'pytest==7.1.0',
     'toml==0.10.2',
     'ipython==7.32.0',
     'ipykernel==6.9.2',
     'jupyter==1.0.0',
     'yamllint==1.26.3',
-    'pytest-timeout==2.1.0',
     'recommonmark==0.7.1',
     'sphinx==4.4.0',
     'pre-commit>=2.18.1,<3',
     # embedding md in rst require docutils>=0.17. See
     # https://myst-parser.readthedocs.io/en/latest/sphinx/use.html?highlight=parser#include-markdown-files-into-an-rst-file
     'docutils==0.17.1',
     'sphinx_markdown_tables==0.0.15',
     'sphinx-argparse==0.3.1',
     'sphinxcontrib.katex==0.8.6',
     'sphinxext.opengraph==0.6.1',
     'sphinxemoji==0.2.0',
     'furo==2022.3.4',
     'sphinx-copybutton==0.5.0',
-    'tabulate==0.8.9',  # for auto-generating tables
     'testbook==0.4.2',
     'myst-parser==0.16.1',
     'sphinx_panels==0.6.0',
     'sphinxcontrib-images==0.9.4',
-    'pytest_codeblocks==0.15.0',
+    'pytest_codeblocks==0.16.1',
     'traitlets==5.1.1',  # required by testbook. Version 5.2.2 has an import bug, so pinning to 5.1.1, which worked previously.
     'nbsphinx==0.8.8',
     'pandoc==2.2',
     'pypandoc==1.8.1',
     'GitPython==3.1.27',
     'moto[s3]>=3.1.12,<3.2',
     'mock-ssh-server==0.9.1',
@@ -131,15 +140,18 @@
     'deepspeed==0.5.10',  # TODO should this be >=0.5.10,<0.6
 ]
 
 extra_deps['wandb'] = [
     'wandb>=0.12.17,<0.13',
 ]
 
-extra_deps['tensorboard'] = ['tensorboard>=2.9.1,<3.0.0']
+extra_deps['tensorboard'] = [
+    'tensorboard>=2.9.1,<3.0.0',
+    'tensorflow-io>=0.26.0,<0.27',
+]
 
 extra_deps['unet'] = [
     'monai>=0.8.0,<0.9',
     'scikit-learn>=1.0.1,<2',
 ]
 
 extra_deps['vit'] = [
@@ -187,15 +199,15 @@
 
 package_name = os.environ.get('COMPOSER_PACKAGE_NAME', 'mosaicml')
 
 if package_name != 'mosaicml':
     print(f'`Building composer as `{package_name}`)', file=sys.stderr)
 
 setup(name=package_name,
-      version='0.8.2',
+      version=composer_version,
       author='MosaicML',
       author_email='team@mosaicml.com',
       description='Composer provides well-engineered implementations of efficient training methods to give '
       'the tools that help you train a better model for cheaper.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/mosaicml/composer',
```

