# Comparing `tmp/composer-0.13.5.tar.gz` & `tmp/composer-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer-0.13.5.tar", last modified: Mon Apr 24 20:59:01 2023, max compression
+gzip compressed data, was "composer-0.14.0.tar", last modified: Wed May  3 15:48:36 2023, max compression
```

## Comparing `composer-0.13.5.tar` & `composer-0.14.0.tar`

### file list

```diff
@@ -1,338 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.473396 composer-0.13.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-04-24 20:58:47.000000 composer-0.13.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 20:58:47.000000 composer-0.13.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-24 20:59:01.473396 composer-0.13.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-24 20:58:47.000000 composer-0.13.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-24 20:58:47.000000 composer-0.13.5/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 20:58:47.000000 composer-0.13.5/composer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 20:58:47.000000 composer-0.13.5/composer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/algorithms/alibi/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/alibi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/augmix/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/blurpool/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/channels_last/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/colout/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/colout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/colout/colout.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/cutout/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/ema/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21563 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ema/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/factorize/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/fused_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/fused_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/fused_layernorm/fused_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/fused_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/gated_linear_units/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/gradient_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/gyro_dropout/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gyro_dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gyro_dropout/gyro_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gyro_dropout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/label_smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/layer_freezing/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/low_precision_groupnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_groupnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_groupnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/low_precision_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/mixup/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/no_op_model/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/progressive_resizing/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/randaugment/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/sam/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/selective_backprop/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/squeeze_excite/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/stochastic_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/swa/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/swa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/swa/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/weight_standardization/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/weight_standardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/weight_standardization/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/weight_standardization/weight_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/export_for_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/mlperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/optimizer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/runtime_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.457396 composer-0.13.5/composer/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 20:58:47.000000 composer-0.13.5/composer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-24 20:58:47.000000 composer-0.13.5/composer/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-04-24 20:58:47.000000 composer-0.13.5/composer/cli/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.457396 composer-0.13.5/composer/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)    60941 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.457396 composer-0.13.5/composer/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/c4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/ffcv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/lm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-24 20:58:47.000000 composer-0.13.5/composer/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/cometml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/file_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/in_memory_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/logger_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/remote_uploader_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/bert/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/models/classify_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/classify_mnist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/classify_mnist/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/deeplabv3/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/efficientnetb0/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/efficientnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/gpt2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/mmdetection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/resnet_cifar/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet_cifar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet_cifar/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet_cifar/resnets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/tasks/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/timm/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/unet/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/vit_small_patch16/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/vit_small_patch16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/vit_small_patch16/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-24 20:58:48.000000 composer-0.13.5/composer/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-04-24 20:58:48.000000 composer-0.13.5/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-04-24 20:58:48.000000 composer-0.13.5/composer/optim/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.469396 composer-0.13.5/composer/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/json_trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/json_trace_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/profiler_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/profiler_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/system_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/torch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:58:48.000000 composer-0.13.5/composer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.469396 composer-0.13.5/composer/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/_scale_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/dist_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/meta_safe_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/mosaic_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)   152656 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.469396 composer-0.13.5/composer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/auto_log_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/batch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28956 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/fx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/iter_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/module_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.473396 composer-0.13.5/composer/utils/object_store/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/oci_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/retrying.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/string_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34926 2023-04-24 20:58:48.000000 composer-0.13.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:59:01.473396 composer-0.13.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-24 20:58:48.000000 composer-0.13.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.473396 composer-0.13.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_full_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_simple_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_split_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.853834 composer-0.14.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-03 15:48:18.000000 composer-0.14.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 15:48:18.000000 composer-0.14.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-05-03 15:48:36.853834 composer-0.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-05-03 15:48:18.000000 composer-0.14.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.745833 composer-0.14.0/composer/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-03 15:48:18.000000 composer-0.14.0/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 15:48:18.000000 composer-0.14.0/composer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 15:48:18.000000 composer-0.14.0/composer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.749833 composer-0.14.0/composer/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.749833 composer-0.14.0/composer/algorithms/alibi/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.749833 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.753833 composer-0.14.0/composer/algorithms/augmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.753833 composer-0.14.0/composer/algorithms/blurpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.753833 composer-0.14.0/composer/algorithms/channels_last/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/colout/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/colout/colout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/cutout/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/ema/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ema/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.761833 composer-0.14.0/composer/algorithms/factorize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.761833 composer-0.14.0/composer/algorithms/fused_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/fused_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/fused_layernorm/fused_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/fused_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.765833 composer-0.14.0/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.765833 composer-0.14.0/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/gyro_dropout/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gyro_dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gyro_dropout/gyro_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gyro_dropout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/label_smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/layer_freezing/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.773833 composer-0.14.0/composer/algorithms/low_precision_groupnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_groupnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_groupnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.773833 composer-0.14.0/composer/algorithms/low_precision_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.773833 composer-0.14.0/composer/algorithms/mixup/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/no_op_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/randaugment/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.781833 composer-0.14.0/composer/algorithms/selective_backprop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.781833 composer-0.14.0/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18808 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.781833 composer-0.14.0/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.785833 composer-0.14.0/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.785833 composer-0.14.0/composer/algorithms/swa/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.785833 composer-0.14.0/composer/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.789833 composer-0.14.0/composer/algorithms/weight_standardization/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/weight_standardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/weight_standardization/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/weight_standardization/weight_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.793833 composer-0.14.0/composer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/activation_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/mlperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/optimizer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/runtime_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.793833 composer-0.14.0/composer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 15:48:18.000000 composer-0.14.0/composer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-03 15:48:18.000000 composer-0.14.0/composer/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-05-03 15:48:18.000000 composer-0.14.0/composer/cli/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.801833 composer-0.14.0/composer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.805833 composer-0.14.0/composer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/c4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/ffcv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51747 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/lm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.805833 composer-0.14.0/composer/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.805833 composer-0.14.0/composer/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-03 15:48:18.000000 composer-0.14.0/composer/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.813834 composer-0.14.0/composer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/cometml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/file_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/logger_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/mosaicml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/remote_uploader_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/slack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.813834 composer-0.14.0/composer/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25727 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/bert/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/models/classify_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/classify_mnist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/classify_mnist/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/deeplabv3/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/efficientnetb0/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/efficientnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/gpt2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34533 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/mmdetection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/resnet_cifar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet_cifar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet_cifar/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet_cifar/resnets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/tasks/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.829834 composer-0.14.0/composer/models/vit_small_patch16/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/vit_small_patch16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/vit_small_patch16/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.829834 composer-0.14.0/composer/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-03 15:48:18.000000 composer-0.14.0/composer/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-05-03 15:48:18.000000 composer-0.14.0/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-05-03 15:48:18.000000 composer-0.14.0/composer/optim/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.833834 composer-0.14.0/composer/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/profiler_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/system_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/torch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:18.000000 composer-0.14.0/composer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.837834 composer-0.14.0/composer/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/dist_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/meta_safe_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/mosaic_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153175 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.845834 composer-0.14.0/composer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/auto_log_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/batch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30139 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/fx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/iter_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/module_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.845834 composer-0.14.0/composer/utils/object_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/oci_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/string_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.745833 composer-0.14.0/composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-05-03 15:48:18.000000 composer-0.14.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:48:36.853834 composer-0.14.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-03 15:48:18.000000 composer-0.14.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.853834 composer-0.14.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_full_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_simple_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_split_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_time.py
```

### Comparing `composer-0.13.5/LICENSE` & `composer-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/PKG-INFO` & `composer-0.14.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.13.5
+Version: 0.14.0
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: dev
 Provides-Extra: health_checker
+Provides-Extra: slack
 Provides-Extra: deepspeed
 Provides-Extra: wandb
 Provides-Extra: comet_ml
 Provides-Extra: tensorboard
 Provides-Extra: unet
 Provides-Extra: vit
 Provides-Extra: timm
@@ -26,14 +27,15 @@
 Provides-Extra: sentencepiece
 Provides-Extra: mlperf
 Provides-Extra: streaming
 Provides-Extra: libcloud
 Provides-Extra: oci
 Provides-Extra: onnx
 Provides-Extra: mlflow
+Provides-Extra: mcli
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/composer#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg" width="50%"/>
@@ -42,31 +44,31 @@
 </p>
 
 <h2><p align="center">A PyTorch Library for Efficient Neural Network Training</p></h2>
 <h3><p align="center">Train Faster, Reduce Cost, Get Better Models</p></h3>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
-- <a href="https://docs.mosaicml.com/en/stable/getting_started/installation.html">[Getting Started]</a>
-- <a href="https://docs.mosaicml.com/">[Docs]</a>
-- <a href="https://docs.mosaicml.com/en/stable/method_cards/methods_overview.html">[Methods]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/en/stable/getting_started/installation.html">[Getting Started]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/">[Docs]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/en/stable/method_cards/methods_overview.html">[Methods]</a>
 - <a href="https://www.mosaicml.com/team">[We're Hiring!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/mosaicml/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mosaicml">
     </a>
     <a href="https://pypi.org/project/mosaicml/">
         <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/mosaicml">
     </a>
     <a href="https://pepy.tech/project/mosaicml/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
-    <a href="https://docs.mosaicml.com/en/stable/">
+    <a href="https://docs.mosaicml.com/projects/composer/en/stable/">
         <img alt="Documentation" src="https://readthedocs.org/projects/composer/badge/?version=stable">
     </a>
     <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/composer/blob/dev/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
@@ -125,15 +127,15 @@
 You can use Composer's speedup methods in two ways:
 
 * Through a standalone **Functional API** (similar to `torch.nn.functional`) that allows you to integrate them into your existing training code.
 * Using Composer's built-in **Trainer**, which is designed to be performant and automatically takes care of the details of using speedup methods.
 
 ### Example: Functional API [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb)
 
-Integrate our speedup methods into your training loop with just a few lines of code, and see the results. Here we easily apply [BlurPool](https://docs.mosaicml.com/en/stable/method_cards/blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/en/stable/method_cards/squeeze_excite.html):
+Integrate our speedup methods into your training loop with just a few lines of code, and see the results. Here we easily apply [BlurPool](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/squeeze_excite.html):
 
 <!-- begin_example_1 --->
 ```python
 import composer.functional as cf
 from torchvision import models
 
 my_model = models.resnet18()
@@ -142,24 +144,24 @@
 cf.apply_blurpool(my_model)
 cf.apply_squeeze_excite(my_model)
 
 # your own training code starts here
 ```
 <!-- end_example_1 --->
 
-For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/latest/functional_api.html).
+For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/projects/composer/en/latest/functional_api.html).
 
 ### Example: Trainer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/getting_started.ipynb)
 
 For the best experience and the most efficient possible training, we recommend using Composer's built-in trainer, which automatically takes care of the details of using speedup methods and provides useful abstractions that facilitate rapid experimentation.
 
 <!-- begin_example_2 --->
 <!--pytest.mark.gpu-->
 <!--pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')-->
-<!--
+<!--pytest.mark.filterwarnings('ignore:Cannot split tensor of length .* into batches of size 128.*:UserWarning')-->
 ```python
 import torch
 
 # adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
 torch.use_deterministic_algorithms(False)
 
 ```
@@ -190,31 +192,31 @@
         LabelSmoothing(smoothing=0.1),
     ]
 )
 trainer.fit()
 ```
 <!-- end_example_2 -->
 
-Composer's built-in [trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html) makes it easy to **add multiple speedup methods in a single line of code!**
+Composer's built-in [trainer](https://docs.mosaicml.com/projects/composer/en/stable/trainer/using_the_trainer.html) makes it easy to **add multiple speedup methods in a single line of code!**
 Trying out new methods or combinations of methods is as easy as changing a single list.
 
-Here are some examples of methods available in Composer ([_see here for the full list_](https://docs.mosaicml.com/en/latest/trainer/algorithms.html)):
+Here are some examples of methods available in Composer ([_see here for the full list_](https://docs.mosaicml.com/projects/composer/en/latest/trainer/algorithms.html)):
 
 Name|Attribution|tl;dr|Example Benchmark|Speed Up*|
 ----|-----------|-----|---------|---------|
 [Alibi](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/alibi)|[Press et al, 2021](https://arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-2|1.5x
 [BlurPool](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter before every downsampling operation.|ResNet-101|1.2x
 [ChannelsLast](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/channels_last)|[PyTorch](https://pytorch.org/tutorials/intermediate/memory_format_tutorial.html)|Uses channels last memory format (NHWC).|ResNet-101|1.5x
-[CutOut](https://docs.mosaicml.com/en/latest/method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
+[CutOut](https://docs.mosaicml.com/projects/composer/en/latest/method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
 [LabelSmoothing](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/1512.00567)|Smooths the labels with a uniform prior|ResNet-101|1.5x
 [MixUp](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/mixup)|[Zhang et al, 2017](https://arxiv.org/abs/1710.09412)|Blends pairs of examples and labels.|ResNet-101|1.5x
 [RandAugment](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/randaugment)|[Cubuk et al, 2020](https://openaccess.thecvf.com/content_CVPRW_2020/html/w40/Cubuk_Randaugment_Practical_Automated_Data_Augmentation_With_a_Reduced_Search_Space_CVPRW_2020_paper.html)|Applies a series of random augmentations to each image.|ResNet-101|1.3x
 [SAM](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/sam)|[Foret et al, 2021](https://arxiv.org/abs/2010.01412)|An optimization strategy that seeks flatter minima.|ResNet-101|1.4x
 [SeqLengthWarmup](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/seq_length_warmup)|[Li et al, 2021](https://arxiv.org/abs/2108.06084)|Progressively increase sequence length.|GPT-2|1.2x
-[Stochastic Depth](https://docs.mosaicml.com/en/latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version that randomly drops the layer or samples during training|ResNet-101|1.1x
+[Stochastic Depth](https://docs.mosaicml.com/projects/composer/en/latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version that randomly drops the layer or samples during training|ResNet-101|1.1x
 <p align="right">* = time-to-train to the same quality as the baseline.</p>
 
 ## 🛠 Building Speedup Recipes
 
 Given two methods that speed up training by 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not necessarily.
 They may optimize the [same part of the training process](https://en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they may even interact in ways that prove detrimental.
 Determining which methods to compose together isn't as simple as assembling a set of methods that perform best individually.
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: composer Version: 0.13.5 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.14.0 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
-health_checker Provides-Extra: deepspeed Provides-Extra: wandb Provides-Extra:
-comet_ml Provides-Extra: tensorboard Provides-Extra: unet Provides-Extra: vit
-Provides-Extra: timm Provides-Extra: coco Provides-Extra: nlp Provides-Extra:
-sentencepiece Provides-Extra: mlperf Provides-Extra: streaming Provides-Extra:
-libcloud Provides-Extra: oci Provides-Extra: onnx Provides-Extra: mlflow
-Provides-Extra: all License-File: LICENSE
+health_checker Provides-Extra: slack Provides-Extra: deepspeed Provides-Extra:
+wandb Provides-Extra: comet_ml Provides-Extra: tensorboard Provides-Extra: unet
+Provides-Extra: vit Provides-Extra: timm Provides-Extra: coco Provides-Extra:
+nlp Provides-Extra: sentencepiece Provides-Extra: mlperf Provides-Extra:
+streaming Provides-Extra: libcloud Provides-Extra: oci Provides-Extra: onnx
+Provides-Extra: mlflow Provides-Extra: mcli Provides-Extra: all License-File:
+LICENSE
   [https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg]
 ***** A PyTorch Library for Efficient Neural Network Training *****
 **** Train Faster, Reduce Cost, Get Better Models ****
 *** [Website] - [Getting_Started] - [Docs] - [Methods] - [We're_Hiring!] ***
 [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads] [Documentation] [Chat_@
                                Slack] [License]
 
@@ -49,78 +50,80 @@
 your existing training code. * Using Composer's built-in **Trainer**, which is
 designed to be performant and automatically takes care of the details of using
 speedup methods. ### Example: Functional API [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 functional_api.ipynb) Integrate our speedup methods into your training loop
 with just a few lines of code, and see the results. Here we easily apply
-[BlurPool](https://docs.mosaicml.com/en/stable/method_cards/blurpool.html) and
-[SqueezeExcite](https://docs.mosaicml.com/en/stable/method_cards/
-squeeze_excite.html):  ```python import composer.functional as cf from
-torchvision import models my_model = models.resnet18() # add blurpool and
-squeeze excite layers cf.apply_blurpool(my_model) cf.apply_squeeze_excite
-(my_model) # your own training code starts here ```  For more examples, see the
-[Composer Functional API Colab notebook](https://colab.research.google.com/
-github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and
-[Functional API guide](https://docs.mosaicml.com/en/latest/
-functional_api.html). ### Example: Trainer [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+[BlurPool](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/
+blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/projects/composer/
+en/stable/method_cards/squeeze_excite.html):  ```python import
+composer.functional as cf from torchvision import models my_model =
+models.resnet18() # add blurpool and squeeze excite layers cf.apply_blurpool
+(my_model) cf.apply_squeeze_excite(my_model) # your own training code starts
+here ```  For more examples, see the [Composer Functional API Colab notebook]
+(https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
+functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/
+projects/composer/en/latest/functional_api.html). ### Example: Trainer [![Open
+In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 getting_started.ipynb) For the best experience and the most efficient possible
 training, we recommend using Composer's built-in trainer, which automatically
 takes care of the details of using speedup methods and provides useful
-abstractions that facilitate rapid experimentation.      ```python from
+abstractions that facilitate rapid experimentation.     ```python import torch
+# adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
+torch.use_deterministic_algorithms(False) ``` -->  ```python from
 torch.utils.data import DataLoader from torchvision import datasets, transforms
 from composer import Trainer from composer.algorithms import ChannelsLast,
 CutMix, LabelSmoothing from composer.models import mnist_model transform =
 transforms.Compose([transforms.ToTensor()]) train_dataset = datasets.MNIST
 ("data", download=True, train=True, transform=transform) eval_dataset =
 datasets.MNIST("data", download=True, train=False, transform=transform)
 train_dataloader = DataLoader(train_dataset, batch_size=128) eval_dataloader =
 DataLoader(eval_dataset, batch_size=128) trainer = Trainer( model=mnist_model
 (), train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
 max_duration="1ep", algorithms=[ ChannelsLast(), CutMix(alpha=1.0),
 LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```  Composer's built-in
-[trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html)
-makes it easy to **add multiple speedup methods in a single line of code!**
-Trying out new methods or combinations of methods is as easy as changing a
-single list. Here are some examples of methods available in Composer ([_see
-here for the full list_](https://docs.mosaicml.com/en/latest/trainer/
-algorithms.html)): Name|Attribution|tl;dr|Example Benchmark|Speed Up*| ----|---
---------|-----|---------|---------| [Alibi](https://github.com/mosaicml/
-composer/tree/dev/composer/algorithms/alibi)|[Press et al, 2021](https://
-arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-2|1.5x [BlurPool]
-(https://github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|
-[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter
-before every downsampling operation.|ResNet-101|1.2x [ChannelsLast](https://
-github.com/mosaicml/composer/tree/dev/composer/algorithms/channels_last)|
-[PyTorch](https://pytorch.org/tutorials/intermediate/
+[trainer](https://docs.mosaicml.com/projects/composer/en/stable/trainer/
+using_the_trainer.html) makes it easy to **add multiple speedup methods in a
+single line of code!** Trying out new methods or combinations of methods is as
+easy as changing a single list. Here are some examples of methods available in
+Composer ([_see here for the full list_](https://docs.mosaicml.com/projects/
+composer/en/latest/trainer/algorithms.html)): Name|Attribution|tl;dr|Example
+Benchmark|Speed Up*| ----|-----------|-----|---------|---------| [Alibi](https:
+//github.com/mosaicml/composer/tree/dev/composer/algorithms/alibi)|[Press et
+al, 2021](https://arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-
+2|1.5x [BlurPool](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/blurpool)|[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an
+anti-aliasing filter before every downsampling operation.|ResNet-101|1.2x
+[ChannelsLast](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/channels_last)|[PyTorch](https://pytorch.org/tutorials/intermediate/
 memory_format_tutorial.html)|Uses channels last memory format (NHWC).|ResNet-
-101|1.5x [CutOut](https://docs.mosaicml.com/en/latest/method_cards/
-cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly
-erases rectangular blocks from the image.|ResNet-101|1.2x [LabelSmoothing]
-(https://github.com/mosaicml/composer/tree/dev/composer/algorithms/
-label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/
+101|1.5x [CutOut](https://docs.mosaicml.com/projects/composer/en/latest/
+method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/
+1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
+[LabelSmoothing](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/
 1512.00567)|Smooths the labels with a uniform prior|ResNet-101|1.5x [MixUp]
 (https://github.com/mosaicml/composer/tree/dev/composer/algorithms/mixup)|
 [Zhang et al, 2017](https://arxiv.org/abs/1710.09412)|Blends pairs of examples
 and labels.|ResNet-101|1.5x [RandAugment](https://github.com/mosaicml/composer/
 tree/dev/composer/algorithms/randaugment)|[Cubuk et al, 2020](https://
 openaccess.thecvf.com/content_CVPRW_2020/html/w40/
 Cubuk_Randaugment_Practical_Automated_Data_Augmentation_With_a_Reduced_Search_Space_CVPRW_2020_paper.html)|Applies
 a series of random augmentations to each image.|ResNet-101|1.3x [SAM](https://
 github.com/mosaicml/composer/tree/dev/composer/algorithms/sam)|[Foret et al,
 2021](https://arxiv.org/abs/2010.01412)|An optimization strategy that seeks
 flatter minima.|ResNet-101|1.4x [SeqLengthWarmup](https://github.com/mosaicml/
 composer/tree/dev/composer/algorithms/seq_length_warmup)|[Li et al, 2021]
 (https://arxiv.org/abs/2108.06084)|Progressively increase sequence length.|GPT-
-2|1.2x [Stochastic Depth](https://docs.mosaicml.com/en/latest/method_cards/
-stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/
-1603.09382)|Replaces a specified layer with a stochastic version that randomly
-drops the layer or samples during training|ResNet-101|1.1x
+2|1.2x [Stochastic Depth](https://docs.mosaicml.com/projects/composer/en/
+latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://
+arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version
+that randomly drops the layer or samples during training|ResNet-101|1.1x
                          * = time-to-train to the same quality as the baseline.
 ## ð  Building Speedup Recipes Given two methods that speed up training by
 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not
 necessarily. They may optimize the [same part of the training process](https://
 en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they
 may even interact in ways that prove detrimental. Determining which methods to
 compose together isn't as simple as assembling a set of methods that perform
```

### Comparing `composer-0.13.5/README.md` & `composer-0.14.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 </p>
 
 <h2><p align="center">A PyTorch Library for Efficient Neural Network Training</p></h2>
 <h3><p align="center">Train Faster, Reduce Cost, Get Better Models</p></h3>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
-- <a href="https://docs.mosaicml.com/en/stable/getting_started/installation.html">[Getting Started]</a>
-- <a href="https://docs.mosaicml.com/">[Docs]</a>
-- <a href="https://docs.mosaicml.com/en/stable/method_cards/methods_overview.html">[Methods]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/en/stable/getting_started/installation.html">[Getting Started]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/">[Docs]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/en/stable/method_cards/methods_overview.html">[Methods]</a>
 - <a href="https://www.mosaicml.com/team">[We're Hiring!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/mosaicml/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mosaicml">
     </a>
     <a href="https://pypi.org/project/mosaicml/">
         <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/mosaicml">
     </a>
     <a href="https://pepy.tech/project/mosaicml/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
-    <a href="https://docs.mosaicml.com/en/stable/">
+    <a href="https://docs.mosaicml.com/projects/composer/en/stable/">
         <img alt="Documentation" src="https://readthedocs.org/projects/composer/badge/?version=stable">
     </a>
     <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/composer/blob/dev/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
@@ -98,15 +98,15 @@
 You can use Composer's speedup methods in two ways:
 
 * Through a standalone **Functional API** (similar to `torch.nn.functional`) that allows you to integrate them into your existing training code.
 * Using Composer's built-in **Trainer**, which is designed to be performant and automatically takes care of the details of using speedup methods.
 
 ### Example: Functional API [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb)
 
-Integrate our speedup methods into your training loop with just a few lines of code, and see the results. Here we easily apply [BlurPool](https://docs.mosaicml.com/en/stable/method_cards/blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/en/stable/method_cards/squeeze_excite.html):
+Integrate our speedup methods into your training loop with just a few lines of code, and see the results. Here we easily apply [BlurPool](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/squeeze_excite.html):
 
 <!-- begin_example_1 --->
 ```python
 import composer.functional as cf
 from torchvision import models
 
 my_model = models.resnet18()
@@ -115,24 +115,24 @@
 cf.apply_blurpool(my_model)
 cf.apply_squeeze_excite(my_model)
 
 # your own training code starts here
 ```
 <!-- end_example_1 --->
 
-For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/latest/functional_api.html).
+For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/projects/composer/en/latest/functional_api.html).
 
 ### Example: Trainer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/getting_started.ipynb)
 
 For the best experience and the most efficient possible training, we recommend using Composer's built-in trainer, which automatically takes care of the details of using speedup methods and provides useful abstractions that facilitate rapid experimentation.
 
 <!-- begin_example_2 --->
 <!--pytest.mark.gpu-->
 <!--pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')-->
-<!--
+<!--pytest.mark.filterwarnings('ignore:Cannot split tensor of length .* into batches of size 128.*:UserWarning')-->
 ```python
 import torch
 
 # adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
 torch.use_deterministic_algorithms(False)
 
 ```
@@ -163,31 +163,31 @@
         LabelSmoothing(smoothing=0.1),
     ]
 )
 trainer.fit()
 ```
 <!-- end_example_2 -->
 
-Composer's built-in [trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html) makes it easy to **add multiple speedup methods in a single line of code!**
+Composer's built-in [trainer](https://docs.mosaicml.com/projects/composer/en/stable/trainer/using_the_trainer.html) makes it easy to **add multiple speedup methods in a single line of code!**
 Trying out new methods or combinations of methods is as easy as changing a single list.
 
-Here are some examples of methods available in Composer ([_see here for the full list_](https://docs.mosaicml.com/en/latest/trainer/algorithms.html)):
+Here are some examples of methods available in Composer ([_see here for the full list_](https://docs.mosaicml.com/projects/composer/en/latest/trainer/algorithms.html)):
 
 Name|Attribution|tl;dr|Example Benchmark|Speed Up*|
 ----|-----------|-----|---------|---------|
 [Alibi](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/alibi)|[Press et al, 2021](https://arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-2|1.5x
 [BlurPool](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter before every downsampling operation.|ResNet-101|1.2x
 [ChannelsLast](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/channels_last)|[PyTorch](https://pytorch.org/tutorials/intermediate/memory_format_tutorial.html)|Uses channels last memory format (NHWC).|ResNet-101|1.5x
-[CutOut](https://docs.mosaicml.com/en/latest/method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
+[CutOut](https://docs.mosaicml.com/projects/composer/en/latest/method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
 [LabelSmoothing](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/1512.00567)|Smooths the labels with a uniform prior|ResNet-101|1.5x
 [MixUp](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/mixup)|[Zhang et al, 2017](https://arxiv.org/abs/1710.09412)|Blends pairs of examples and labels.|ResNet-101|1.5x
 [RandAugment](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/randaugment)|[Cubuk et al, 2020](https://openaccess.thecvf.com/content_CVPRW_2020/html/w40/Cubuk_Randaugment_Practical_Automated_Data_Augmentation_With_a_Reduced_Search_Space_CVPRW_2020_paper.html)|Applies a series of random augmentations to each image.|ResNet-101|1.3x
 [SAM](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/sam)|[Foret et al, 2021](https://arxiv.org/abs/2010.01412)|An optimization strategy that seeks flatter minima.|ResNet-101|1.4x
 [SeqLengthWarmup](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/seq_length_warmup)|[Li et al, 2021](https://arxiv.org/abs/2108.06084)|Progressively increase sequence length.|GPT-2|1.2x
-[Stochastic Depth](https://docs.mosaicml.com/en/latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version that randomly drops the layer or samples during training|ResNet-101|1.1x
+[Stochastic Depth](https://docs.mosaicml.com/projects/composer/en/latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version that randomly drops the layer or samples during training|ResNet-101|1.1x
 <p align="right">* = time-to-train to the same quality as the baseline.</p>
 
 ## 🛠 Building Speedup Recipes
 
 Given two methods that speed up training by 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not necessarily.
 They may optimize the [same part of the training process](https://en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they may even interact in ways that prove detrimental.
 Determining which methods to compose together isn't as simple as assembling a set of methods that perform best individually.
```

#### html2text {}

```diff
@@ -39,78 +39,80 @@
 your existing training code. * Using Composer's built-in **Trainer**, which is
 designed to be performant and automatically takes care of the details of using
 speedup methods. ### Example: Functional API [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 functional_api.ipynb) Integrate our speedup methods into your training loop
 with just a few lines of code, and see the results. Here we easily apply
-[BlurPool](https://docs.mosaicml.com/en/stable/method_cards/blurpool.html) and
-[SqueezeExcite](https://docs.mosaicml.com/en/stable/method_cards/
-squeeze_excite.html):  ```python import composer.functional as cf from
-torchvision import models my_model = models.resnet18() # add blurpool and
-squeeze excite layers cf.apply_blurpool(my_model) cf.apply_squeeze_excite
-(my_model) # your own training code starts here ```  For more examples, see the
-[Composer Functional API Colab notebook](https://colab.research.google.com/
-github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and
-[Functional API guide](https://docs.mosaicml.com/en/latest/
-functional_api.html). ### Example: Trainer [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+[BlurPool](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/
+blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/projects/composer/
+en/stable/method_cards/squeeze_excite.html):  ```python import
+composer.functional as cf from torchvision import models my_model =
+models.resnet18() # add blurpool and squeeze excite layers cf.apply_blurpool
+(my_model) cf.apply_squeeze_excite(my_model) # your own training code starts
+here ```  For more examples, see the [Composer Functional API Colab notebook]
+(https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
+functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/
+projects/composer/en/latest/functional_api.html). ### Example: Trainer [![Open
+In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 getting_started.ipynb) For the best experience and the most efficient possible
 training, we recommend using Composer's built-in trainer, which automatically
 takes care of the details of using speedup methods and provides useful
-abstractions that facilitate rapid experimentation.      ```python from
+abstractions that facilitate rapid experimentation.     ```python import torch
+# adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
+torch.use_deterministic_algorithms(False) ``` -->  ```python from
 torch.utils.data import DataLoader from torchvision import datasets, transforms
 from composer import Trainer from composer.algorithms import ChannelsLast,
 CutMix, LabelSmoothing from composer.models import mnist_model transform =
 transforms.Compose([transforms.ToTensor()]) train_dataset = datasets.MNIST
 ("data", download=True, train=True, transform=transform) eval_dataset =
 datasets.MNIST("data", download=True, train=False, transform=transform)
 train_dataloader = DataLoader(train_dataset, batch_size=128) eval_dataloader =
 DataLoader(eval_dataset, batch_size=128) trainer = Trainer( model=mnist_model
 (), train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
 max_duration="1ep", algorithms=[ ChannelsLast(), CutMix(alpha=1.0),
 LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```  Composer's built-in
-[trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html)
-makes it easy to **add multiple speedup methods in a single line of code!**
-Trying out new methods or combinations of methods is as easy as changing a
-single list. Here are some examples of methods available in Composer ([_see
-here for the full list_](https://docs.mosaicml.com/en/latest/trainer/
-algorithms.html)): Name|Attribution|tl;dr|Example Benchmark|Speed Up*| ----|---
---------|-----|---------|---------| [Alibi](https://github.com/mosaicml/
-composer/tree/dev/composer/algorithms/alibi)|[Press et al, 2021](https://
-arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-2|1.5x [BlurPool]
-(https://github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|
-[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter
-before every downsampling operation.|ResNet-101|1.2x [ChannelsLast](https://
-github.com/mosaicml/composer/tree/dev/composer/algorithms/channels_last)|
-[PyTorch](https://pytorch.org/tutorials/intermediate/
+[trainer](https://docs.mosaicml.com/projects/composer/en/stable/trainer/
+using_the_trainer.html) makes it easy to **add multiple speedup methods in a
+single line of code!** Trying out new methods or combinations of methods is as
+easy as changing a single list. Here are some examples of methods available in
+Composer ([_see here for the full list_](https://docs.mosaicml.com/projects/
+composer/en/latest/trainer/algorithms.html)): Name|Attribution|tl;dr|Example
+Benchmark|Speed Up*| ----|-----------|-----|---------|---------| [Alibi](https:
+//github.com/mosaicml/composer/tree/dev/composer/algorithms/alibi)|[Press et
+al, 2021](https://arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-
+2|1.5x [BlurPool](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/blurpool)|[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an
+anti-aliasing filter before every downsampling operation.|ResNet-101|1.2x
+[ChannelsLast](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/channels_last)|[PyTorch](https://pytorch.org/tutorials/intermediate/
 memory_format_tutorial.html)|Uses channels last memory format (NHWC).|ResNet-
-101|1.5x [CutOut](https://docs.mosaicml.com/en/latest/method_cards/
-cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly
-erases rectangular blocks from the image.|ResNet-101|1.2x [LabelSmoothing]
-(https://github.com/mosaicml/composer/tree/dev/composer/algorithms/
-label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/
+101|1.5x [CutOut](https://docs.mosaicml.com/projects/composer/en/latest/
+method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/
+1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
+[LabelSmoothing](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/
 1512.00567)|Smooths the labels with a uniform prior|ResNet-101|1.5x [MixUp]
 (https://github.com/mosaicml/composer/tree/dev/composer/algorithms/mixup)|
 [Zhang et al, 2017](https://arxiv.org/abs/1710.09412)|Blends pairs of examples
 and labels.|ResNet-101|1.5x [RandAugment](https://github.com/mosaicml/composer/
 tree/dev/composer/algorithms/randaugment)|[Cubuk et al, 2020](https://
 openaccess.thecvf.com/content_CVPRW_2020/html/w40/
 Cubuk_Randaugment_Practical_Automated_Data_Augmentation_With_a_Reduced_Search_Space_CVPRW_2020_paper.html)|Applies
 a series of random augmentations to each image.|ResNet-101|1.3x [SAM](https://
 github.com/mosaicml/composer/tree/dev/composer/algorithms/sam)|[Foret et al,
 2021](https://arxiv.org/abs/2010.01412)|An optimization strategy that seeks
 flatter minima.|ResNet-101|1.4x [SeqLengthWarmup](https://github.com/mosaicml/
 composer/tree/dev/composer/algorithms/seq_length_warmup)|[Li et al, 2021]
 (https://arxiv.org/abs/2108.06084)|Progressively increase sequence length.|GPT-
-2|1.2x [Stochastic Depth](https://docs.mosaicml.com/en/latest/method_cards/
-stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/
-1603.09382)|Replaces a specified layer with a stochastic version that randomly
-drops the layer or samples during training|ResNet-101|1.1x
+2|1.2x [Stochastic Depth](https://docs.mosaicml.com/projects/composer/en/
+latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://
+arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version
+that randomly drops the layer or samples during training|ResNet-101|1.1x
                          * = time-to-train to the same quality as the baseline.
 ## ð  Building Speedup Recipes Given two methods that speed up training by
 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not
 necessarily. They may optimize the [same part of the training process](https://
 en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they
 may even interact in ways that prove detrimental. Determining which methods to
 compose together isn't as simple as assembling a set of methods that perform
```

### Comparing `composer-0.13.5/composer/__init__.py` & `composer-0.14.0/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/__init__.py` & `composer-0.14.0/composer/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/alibi/__init__.py` & `composer-0.14.0/composer/algorithms/alibi/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/alibi/alibi.py` & `composer-0.14.0/composer/algorithms/alibi/alibi.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/__init__.py` & `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_bert.py` & `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py` & `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/utils.py` & `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/augmix/__init__.py` & `composer-0.14.0/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/augmix/augmix.py` & `composer-0.14.0/composer/algorithms/augmix/augmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/blurpool/__init__.py` & `composer-0.14.0/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/blurpool/blurpool.py` & `composer-0.14.0/composer/algorithms/blurpool/blurpool.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/blurpool/blurpool_layers.py` & `composer-0.14.0/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/channels_last/__init__.py` & `composer-0.14.0/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/channels_last/channels_last.py` & `composer-0.14.0/composer/algorithms/channels_last/channels_last.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/channels_last/metadata.json` & `composer-0.14.0/composer/algorithms/channels_last/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/colout/__init__.py` & `composer-0.14.0/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/colout/colout.py` & `composer-0.14.0/composer/algorithms/colout/colout.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/cutmix/__init__.py` & `composer-0.14.0/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/cutmix/cutmix.py` & `composer-0.14.0/composer/algorithms/cutmix/cutmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/cutmix/metadata.json` & `composer-0.14.0/composer/algorithms/cutmix/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/cutout/cutout.py` & `composer-0.14.0/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/ema/ema.py` & `composer-0.14.0/composer/algorithms/ema/ema.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,16 @@
         # Calculate the appropriate weighting for the moving average
         if smoothing is None and self.half_life:
             self.smoothing = 2**(-(self.update_interval.value / self.half_life.value))
         else:
             self.smoothing = smoothing
 
         # Construct the appropriate matching events
-        self.match_events = [Event.FIT_START, Event.BATCH_START, Event.EVAL_START, Event.EVAL_END]
+        self.move_device_events = [Event.EVAL_START, Event.FIT_START, Event.PREDICT_START]
+        self.move_param_events = [Event.BATCH_START, Event.EVAL_START, Event.EVAL_END]
         self.checkpoint_events = [Event.BATCH_CHECKPOINT, Event.EPOCH_CHECKPOINT]
         if self.update_interval.unit == TimeUnit.BATCH:
             self.update_event = Event.BATCH_END
         elif self.update_interval.unit == TimeUnit.EPOCH:
             self.update_event = Event.EPOCH_END
 
     def _should_start(self, state: State) -> bool:
@@ -238,19 +239,24 @@
             self.ema_model = EMAParameters(state.model)
             self.ema_started = True
 
         # Match on checkpointing events if a checkpoint is to be saved
         if event in [Event.BATCH_CHECKPOINT, Event.EPOCH_CHECKPOINT] and self.ema_started:
             checkpoint_savers = [cb for cb in state.callbacks if isinstance(cb, CheckpointSaver)]
             for checkpoint_saver in checkpoint_savers:
+                assert callable(checkpoint_saver.save_interval)
                 if checkpoint_saver.save_interval(state, event) is True:
                     return True
 
-        # Otherwise, always run on some events after ema has started
-        if event in self.match_events and self.ema_started:
+        # Otherwise, always run on events where ema params must be moved after ema has started
+        if event in self.move_param_events and self.ema_started:
+            return True
+
+        # Run on events where ema params must be moved to the correct device
+        if event in self.move_device_events and self.ema_started:
             return True
 
         # Conditionally run on the update event if ema has started
         if event == self.update_event and self.ema_started:
             return (state.timestamp.get(self.update_interval.unit).value % self.update_interval.value == 0)
 
         return False
@@ -261,27 +267,30 @@
 
         if event == Event.INIT:
             # Create the models so that the checkpoints can be loaded
             self.ema_model = EMAParameters(state.model)
 
         assert self.ema_model is not None
 
-        if event == Event.FIT_START:
+        if event == Event.FIT_START or event == Event.PREDICT_START:
             # Ensure that params are on the right device if a checkpoint has been loaded
             self.ema_model.move_params_to_device(destination_model=state.model)
 
         if event == Event.BATCH_START and self.ema_weights_active:
             # Ensure the model being trained has the correct weights
             self._ensure_training_weights_active(state)
 
         if event in [Event.BATCH_END, Event.EPOCH_END]:
             # Update the ema model
             compute_ema(state.model, self.ema_model, smoothing=self.smoothing)
 
-        if event == Event.EVAL_START and self.ema_weights_active is False:
+        if event == Event.EVAL_START:
+            # Verify that the ema params are on the correct device.
+            # Needed to ensure doing eval before training can resume correctly.
+            self.ema_model.move_params_to_device(destination_model=state.model)
             # Swap out the training model for the ema model in state
             self._ensure_ema_weights_active(state)
 
         if event == Event.EVAL_END:
             # Swap out the ema model for the training model in state
             self._ensure_training_weights_active(state)
```

### Comparing `composer-0.13.5/composer/algorithms/factorize/__init__.py` & `composer-0.14.0/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/factorize/factorize.py` & `composer-0.14.0/composer/algorithms/factorize/factorize.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/factorize/factorize_core.py` & `composer-0.14.0/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/factorize/factorize_modules.py` & `composer-0.14.0/composer/algorithms/factorize/factorize_modules.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/fused_layernorm/__init__.py` & `composer-0.14.0/composer/algorithms/fused_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/fused_layernorm/fused_layernorm.py` & `composer-0.14.0/composer/algorithms/fused_layernorm/fused_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/fused_layernorm/metadata.json` & `composer-0.14.0/composer/algorithms/fused_layernorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/gated_linear_units/__init__.py` & `composer-0.14.0/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_units.py` & `composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/gated_linear_units/metadata.json` & `composer-0.14.0/composer/algorithms/gated_linear_units/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/ghost_batchnorm/__init__.py` & `composer-0.14.0/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `composer-0.14.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/ghost_batchnorm/metadata.json` & `composer-0.14.0/composer/algorithms/ghost_batchnorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/gradient_clipping/gradient_clipping.py` & `composer-0.14.0/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import torch
 from packaging import version
 
 from composer.core import Algorithm, Event, State
 from composer.loggers import Logger
 from composer.models import ComposerModel
+from composer.utils import using_torch_2
 
 log = logging.getLogger(__name__)
 
 __all__ = ['GradientClipping', 'apply_gradient_clipping']
 
 
 def apply_gradient_clipping(model: Union[ComposerModel, torch.nn.Module], clipping_type: str, clipping_threshold: float,
@@ -38,29 +39,34 @@
             scale gradients by this threshold * (weight_norm / grad_norm) (for 'adaptive').
         fsdp_enabled (bool): Bool of if the model is a FSDP model or not.
     """
     if fsdp_enabled:
         if version.parse(torch.__version__) < version.parse('1.13.0'):
             raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
         from torch.distributed.fsdp import FullyShardedDataParallel
+
+        is_torch_2_0 = using_torch_2()
+
         for module in model.modules():
             if isinstance(module, FullyShardedDataParallel):
                 # We can only call grad clip on the parent instance, so we iterate through all
                 # modules and try grad clipping and FSDP will throw an exception if we
                 # clip any gradients that aren't a parent module
                 try:
                     if clipping_type == 'norm':
                         module.clip_grad_norm_(max_norm=clipping_threshold)
                     elif clipping_type == 'value':
                         module.clip_grad_norm_(max_norm=clipping_threshold, norm_type=float('inf'))
                     else:
                         raise ValueError(f"clipping type must be 'norm' or 'value' with FSDP not {clipping_type}")
-                except AssertionError as e:
-                    # Catches the error message from PyTorch
-                    if 'clip_grad_norm should only be called on the root (parent) instance' == str(e):
+                except (AssertionError, RuntimeError) as e:
+                    if (('clip_grad_norm should only be called on the root (parent) instance' == str(e) and
+                         not is_torch_2_0) or
+                        ('`clip_grad_norm_()` should only be called on the root FSDP instance' == str(e) and
+                         is_torch_2_0)):
                         continue
                     else:
                         raise
         return
     parameters = model.parameters()
     if clipping_type == 'adaptive':
         _apply_agc(parameters, clipping_threshold=clipping_threshold)
```

### Comparing `composer-0.13.5/composer/algorithms/gradient_clipping/metadata.json` & `composer-0.14.0/composer/algorithms/gradient_clipping/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/gyro_dropout/gyro_dropout.py` & `composer-0.14.0/composer/algorithms/gyro_dropout/gyro_dropout.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     """
 
     def __init__(self, p: float = 0.5, sigma: int = 256, tau: int = 16):
         self.p = p
         self.sigma = sigma
         self.tau = tau
 
-        log.warning(
+        warnings.warn(
             'GyroDropout is not implemented in a way that allows correct resumption from checkpoint, which may lead to incorrect behavior.'
         )
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}()'
 
     @staticmethod
```

### Comparing `composer-0.13.5/composer/algorithms/label_smoothing/__init__.py` & `composer-0.14.0/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/label_smoothing/label_smoothing.py` & `composer-0.14.0/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/label_smoothing/metadata.json` & `composer-0.14.0/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/layer_freezing/layer_freezing.py` & `composer-0.14.0/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/layer_freezing/metadata.json` & `composer-0.14.0/composer/algorithms/layer_freezing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/low_precision_groupnorm/__init__.py` & `composer-0.14.0/composer/algorithms/low_precision_groupnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py` & `composer-0.14.0/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/low_precision_layernorm/__init__.py` & `composer-0.14.0/composer/algorithms/low_precision_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py` & `composer-0.14.0/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/mixup/metadata.json` & `composer-0.14.0/composer/algorithms/mixup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/mixup/mixup.py` & `composer-0.14.0/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/no_op_model/__init__.py` & `composer-0.14.0/composer/algorithms/no_op_model/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/no_op_model/no_op_model.py` & `composer-0.14.0/composer/algorithms/no_op_model/no_op_model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/progressive_resizing/__init__.py` & `composer-0.14.0/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/progressive_resizing/metadata.json` & `composer-0.14.0/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/progressive_resizing/progressive_resizing.py` & `composer-0.14.0/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/randaugment/metadata.json` & `composer-0.14.0/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/randaugment/randaugment.py` & `composer-0.14.0/composer/algorithms/randaugment/randaugment.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/sam/__init__.py` & `composer-0.14.0/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/sam/sam.py` & `composer-0.14.0/composer/algorithms/sam/sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """SAM algorithm and optimizer class."""
 
 from __future__ import annotations
 
 import logging
+import warnings
 from typing import Optional
 
 import torch
 
 from composer.core import Algorithm, Event, State
 from composer.loggers import Logger
 from composer.utils import ensure_tuple
@@ -143,18 +144,17 @@
 
     def __init__(
         self,
         rho: float = 0.05,
         epsilon: float = 1.0e-12,
         interval: int = 1,
     ):
-        log.warning(
+        warnings.warn(
             'SAM has known issues of weight mismatch when loading from a checkpoint, which will cause an error when resuming without `load_weights_only=True`.'
         )
-        """__init__ is constructed from the same fields as in hparams."""
         self.rho = rho
         self.epsilon = epsilon
         self.interval = interval
 
     def match(self, event: Event, state: State) -> bool:
         return event == Event.INIT
```

### Comparing `composer-0.13.5/composer/algorithms/selective_backprop/__init__.py` & `composer-0.14.0/composer/algorithms/selective_backprop/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/selective_backprop/metadata.json` & `composer-0.14.0/composer/algorithms/selective_backprop/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/selective_backprop/selective_backprop.py` & `composer-0.14.0/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/seq_length_warmup/metadata.json` & `composer-0.14.0/composer/algorithms/seq_length_warmup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `composer-0.14.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Core code for sequence length warmup."""
 
 import logging
 import textwrap
-from math import ceil
 from typing import Dict, Mapping, Optional
 
 import torch
 import torch.utils.data
 
 from composer.core import Algorithm, Batch, Event, State, TimeUnit, get_precision_context
 from composer.loggers import Logger
@@ -246,16 +245,16 @@
 
         The purpose of activating the model is to prevent OOMs. This happens two ways.
 
         First, this prevents GPU memory from being reallocated when the sequence
         length increases.
 
         Second, it detects if the batch*max_sequence_length size will cause an OOM and
-        increases state.grad_accum accordingly. This logic mirrors the ``grad_accum="auto"``
-        logic in :class:`.Trainer`.
+        decreases state.device_train_microbatch_size accordingly. This logic mirrors the
+        ``device_train_microbatch_size='auto'`` logic in :class:`.Trainer`.
         """
 
         assert self._original_model is not None, 'original model should be set on Event.INIT'
 
         try:
             # Both PyTorch and FFCV dataloaders define a `batch_size` attribute
             # This exception would mainly be raised if the user is passing in a custom
@@ -265,66 +264,83 @@
             raise AttributeError(
                 'Sequence Length Warmup requires the `state.dataloader` to have a `batch_size` attribute.') from e
         if per_gpu_macrobatch is None:
             raise RuntimeError('Sequence Length Warmup algorithm requires constant batch size.')
 
         # truncate all sequence-shaped tensors to the max sequence length
         batch_clone = {k: torch.clone(v) for k, v in state.batch.items()}
-        device_batch_size = 0
         for k, v in batch_clone.items():
             if v.ndim < 2:
                 raise ValueError(f'Sequence Length Warmup requires that all tensors are sequence-shaped. '
                                  f'Tensor "{k}" has shape {v.shape}.')
             batch_clone[k] = v[:, :self.max_seq_length].contiguous()
-            device_batch_size = v.shape[0]
 
         # In-line to avoid circular dependency
-        from composer.trainer.trainer import _adjust_device_train_microbatch_size, _adjust_grad_accum, _is_cuda_oom
+        from composer.trainer.trainer import _adjust_device_train_microbatch_size, _is_cuda_oom
 
         # This loop tries to do a forward/backward pass using the current microbatch size.
-        # If it hits an OOM error, it doubles `state.grad_accum` and tries again until
-        # it succeeds.
+        # If it hits an OOM error, it halves `state.device_train_microbatch_size` and tries again
+        # until it succeeds.
         while True:
-            per_gpu_batch = ceil(per_gpu_macrobatch / state.grad_accum)
-            model_inputs = {k: v[:per_gpu_batch] for k, v in batch_clone.items()}
+            model_inputs = {k: v[:state.device_train_microbatch_size] for k, v in batch_clone.items()}
 
             found_cuda_oom = 0  # int since bool BOR not supported on all torch.distributed backends
             try:
-                # start by running a forward and backward pass
+                # Start by running a forward and backward pass
                 # of the maximum sequence length to allocate cache.
                 with get_precision_context(state.precision):
                     outputs = state.model.forward(model_inputs)
                     loss = self._original_model.loss(outputs, model_inputs)
 
-                # since use_grad_scaling is in the Trainer, and we
+                # Check if other ranks OOMed after forward pass when using auto microbatching. This may
+                # happen when close to memory limit or with uneven memory usage across ranks
+                if state.auto_microbatching:
+                    # Check if any other rank hit an OOM
+                    found_cuda_oom_tensor = state.device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
+                    dist.all_reduce(found_cuda_oom_tensor, reduce_operation='MAX')
+                    found_cuda_oom = found_cuda_oom_tensor.item()
+                    # Signal current rank is still in batch
+                    all_ranks_finished_tensor = state.device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
+                    dist.all_reduce(all_ranks_finished_tensor, reduce_operation='MIN')
+
+                    if found_cuda_oom == 1:
+                        raise RuntimeError('CUDA out of memory encountered on a different rank')
+
+                # Since use_grad_scaling is in the Trainer, and we
                 # don't care about the loss values, skip scaling
                 for loss_item in ensure_tuple(loss):
                     loss_item.backward()
 
                 # Zero any gradients created by the backward pass
                 for optimizer in state.optimizers:
                     optimizer.zero_grad()
 
-            # This error/state.grad_accum handling mimics the logic in trainer._train_batch().
+            # This error/state.device_train_microbatch_size handling mimics the logic in trainer._train_batch().
             except RuntimeError as e:
                 if state.auto_microbatching and _is_cuda_oom(e):
                     log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                     found_cuda_oom = 1
                 else:
                     raise
 
             if state.auto_microbatching:
-                # Propagate across all ranks if any rank hit CUDA OOM
-                found_cuda_oom = state.device.tensor_to_device(torch.tensor([found_cuda_oom], dtype=torch.uint8))
-                dist.all_reduce(found_cuda_oom, reduce_operation='MAX')
-                if found_cuda_oom.item() == 1:
-                    if state.using_device_microbatch_size:
-                        _adjust_device_train_microbatch_size(state)
-                    else:
-                        _adjust_grad_accum(state, device_batch_size)
+                all_ranks_finished = False
+                while not all_ranks_finished:
+                    # Propagate across all ranks if any rank hit CUDA OOM
+                    found_cuda_oom_tensor = state.device.tensor_to_device(
+                        torch.tensor([found_cuda_oom], dtype=torch.uint8))
+                    dist.all_reduce(found_cuda_oom_tensor, reduce_operation='MAX')
+                    found_cuda_oom = found_cuda_oom_tensor.item()
+                    # Check if any rank is still not done with the batch. This may happen if only a
+                    # subset of ranks OOM, leaving some batches still in the forward pass
+                    all_ranks_finished_tensor = state.device.tensor_to_device(torch.tensor([1], dtype=torch.uint8))
+                    dist.all_reduce(all_ranks_finished_tensor, reduce_operation='MIN')
+                    all_ranks_finished = all_ranks_finished_tensor.item() == 1
+                if found_cuda_oom == 1:
+                    _adjust_device_train_microbatch_size(state)
                     # Skip return and rerun after handling oom
                     continue
             # Activate and return if we've completed without OOMing.
             self._activated = True
             return
 
     def match(self, event: Event, state: State) -> bool:
```

### Comparing `composer-0.13.5/composer/algorithms/squeeze_excite/__init__.py` & `composer-0.14.0/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/squeeze_excite/squeeze_excite.py` & `composer-0.14.0/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/stochastic_depth/__init__.py` & `composer-0.14.0/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/stochastic_depth/metadata.json` & `composer-0.14.0/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_depth.py` & `composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_layers.py` & `composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/swa/swa.py` & `composer-0.14.0/composer/algorithms/swa/swa.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Core code for Stochastic Weight Averaging."""
 
 from __future__ import annotations
 
 import logging
+import warnings
 from typing import Any, Dict, List, Optional
 
 import torch
 from torch.optim.swa_utils import SWALR, AveragedModel
 
 from composer.core import Algorithm, Event, PyTorchScheduler, State, Time, TimeUnit
 from composer.loggers import Logger
@@ -111,15 +112,15 @@
                  swa_end: str = '0.97dur',
                  update_interval: str = '1ep',
                  schedule_swa_lr: bool = False,
                  anneal_strategy: str = 'linear',
                  anneal_steps: int = 10,
                  swa_lr: Optional[float] = None):
 
-        log.warning(
+        warnings.warn(
             'SWA has known issues when resuming from a checkpoint on multiple GPUs, which will cause an error when resuming without `load_weights_only=True`.'
         )
         self.schedule_swa_lr = schedule_swa_lr
         self.anneal_strategy = anneal_strategy
         self.anneal_steps = anneal_steps
         self.swa_lr = swa_lr
         self.swa_model: Optional[torch.nn.Module] = None
```

### Comparing `composer-0.13.5/composer/algorithms/utils/augmentation_common.py` & `composer-0.14.0/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/utils/augmentation_primitives.py` & `composer-0.14.0/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/warnings.py` & `composer-0.14.0/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/weight_standardization/metadata.json` & `composer-0.14.0/composer/algorithms/weight_standardization/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/algorithms/weight_standardization/weight_standardization.py` & `composer-0.14.0/composer/algorithms/weight_standardization/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/__init__.py` & `composer-0.14.0/composer/callbacks/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Callbacks that run at each training loop :class:`.Event`.
 
 Each callback inherits from the :class:`.Callback` base class. See detailed description and
 examples for writing your own callbacks at the :class:`.Callback` base class.
 """
+from composer.callbacks.activation_monitor import ActivationMonitor
 from composer.callbacks.checkpoint_saver import CheckpointSaver
 from composer.callbacks.early_stopper import EarlyStopper
 from composer.callbacks.export_for_inference import ExportForInferenceCallback
 from composer.callbacks.health_checker import HealthChecker
 from composer.callbacks.image_visualizer import ImageVisualizer
 from composer.callbacks.lr_monitor import LRMonitor
 from composer.callbacks.memory_monitor import MemoryMonitor
 from composer.callbacks.mlperf import MLPerfCallback
 from composer.callbacks.optimizer_monitor import OptimizerMonitor
 from composer.callbacks.runtime_estimator import RuntimeEstimator
 from composer.callbacks.speed_monitor import SpeedMonitor
 from composer.callbacks.threshold_stopper import ThresholdStopper
 
 __all__ = [
+    'ActivationMonitor',
     'OptimizerMonitor',
     'LRMonitor',
     'MemoryMonitor',
     'SpeedMonitor',
     'CheckpointSaver',
     'MLPerfCallback',
     'EarlyStopper',
```

### Comparing `composer-0.13.5/composer/callbacks/checkpoint_saver.py` & `composer-0.14.0/composer/callbacks/checkpoint_saver.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Callback to save checkpoints during training."""
 
 from __future__ import annotations
 
 import logging
+import math
 import os
 import pathlib
 import tempfile
 import textwrap
 from typing import Callable, List, Optional, Union
 
 from composer.core import Callback, Event, State, Time, TimeUnit
@@ -25,15 +26,16 @@
 
 def checkpoint_periodically(interval: Union[str, int, Time]) -> Callable[[State, Event], bool]:
     r"""Helper function to create a checkpoint scheduler according to a specified interval.
 
     Args:
         interval (Union[str, int, :class:`.Time`]): The interval describing how often checkpoints should be
             saved. If an integer, it will be assumed to be in :attr:`.TimeUnit.EPOCH`\s.
-            Otherwise, the unit must be either :attr:`.TimeUnit.EPOCH` or :attr:`.TimeUnit.BATCH`.
+            Otherwise, the unit must be either :attr:`.TimeUnit.EPOCH`, :attr:`.TimeUnit.BATCH`,
+            :attr:`.TimeUnit.TOKEN`, or :attr:`.TimeUnit.SAMPLE`.
 
             Checkpoints will be saved every ``n`` batches or epochs (depending on the unit),
             and at the end of training.
 
     Returns:
         Callable[[State, Event], bool]: A function that can be passed as the ``save_interval``
             argument into the :class:`.CheckpointSaver`.
@@ -41,39 +43,44 @@
     if isinstance(interval, str):
         interval = Time.from_timestring(interval)
     if isinstance(interval, int):
         interval = Time(interval, TimeUnit.EPOCH)
 
     if interval.unit == TimeUnit.EPOCH:
         save_event = Event.EPOCH_CHECKPOINT
-    elif interval.unit == TimeUnit.BATCH:
+    elif interval.unit in {TimeUnit.BATCH, TimeUnit.TOKEN, TimeUnit.SAMPLE}:
         save_event = Event.BATCH_CHECKPOINT
     else:
         raise NotImplementedError(
-            f'Unknown checkpointing interval: {interval.unit}. Must be TimeUnit.EPOCH or TimeUnit.BATCH.')
+            f'Unknown checkpointing interval: {interval.unit}. Must be TimeUnit.EPOCH, TimeUnit.BATCH, TimeUnit.TOKEN, or TimeUnit.SAMPLE.'
+        )
 
     def save_interval(state: State, event: Event):
         elapsed_duration = state.get_elapsed_duration()
         assert elapsed_duration is not None, 'elapsed_duration is set on the BATCH_CHECKPOINT and EPOCH_CHECKPOINT'
 
         # Always checkpoint at end of training
         if elapsed_duration >= 1.0:
             return True
 
-        if save_event == Event.EPOCH_CHECKPOINT:
-            count = state.timestamp.epoch
-        elif save_event == Event.BATCH_CHECKPOINT:
-            count = state.timestamp.batch
+        # previous timestamp will only be None if training has not started, but we are returning False
+        # in this case, just to be safe
+        if state.previous_timestamp is None:
+            return False
+
+        if interval.unit in {TimeUnit.EPOCH, TimeUnit.BATCH, TimeUnit.TOKEN, TimeUnit.SAMPLE}:
+            previous_count = state.previous_timestamp.get(interval.unit)
+            count = state.timestamp.get(interval.unit)
         else:
-            raise RuntimeError(f'Invalid save_event: {save_event}')
-
-        if event == save_event and int(count) % int(interval) == 0:
-            return True
+            raise NotImplementedError(
+                f'Unknown checkpointing interval: {interval.unit}. Must be TimeUnit.EPOCH, TimeUnit.BATCH, TimeUnit.TOKEN, or TimeUnit.SAMPLE.'
+            )
 
-        return False
+        threshold_passed = math.floor(previous_count / interval.value) != math.floor(count / interval.value)
+        return event == save_event and threshold_passed
 
     return save_interval
 
 
 class CheckpointSaver(Callback):  # noqa: D101
     __doc__ = f"""Callback to save checkpoints.
 
@@ -309,14 +316,16 @@
         self.latest_remote_file_name = PartialFilePath(latest_remote_file_name) if latest_remote_file_name else None
 
         self.overwrite = overwrite
         self.saved_checkpoints: List[str] = []
         self.num_checkpoints_to_keep = num_checkpoints_to_keep
         self.weights_only = weights_only
 
+        self.start_batch = None
+
     def init(self, state: State, logger: Logger) -> None:
         folder = format_name_with_dist(self.folder, state.run_name)
         os.makedirs(folder, exist_ok=True)
 
     def fit_start(self, state: State, logger: Logger) -> None:
         if not self.overwrite:
             # checks that save_folder contains no files with a timestamp after the current timestamp,
@@ -325,28 +334,40 @@
             ensure_folder_has_no_conflicting_files(folder, self.filename.filename, state.timestamp)
 
         dist.barrier()  # holds all ranks until folder check is done
 
         if is_model_deepspeed(state.model) and self.weights_only:
             raise NotImplementedError('weights_only=True is not supported when using DeepSpeed.')
 
+        self.start_batch = state.timestamp.batch
+
     def batch_checkpoint(self, state: State, logger: Logger):
+        assert callable(self.save_interval)
         if self.save_interval(state, Event.BATCH_CHECKPOINT) and self.last_checkpoint_batch != state.timestamp.batch:
             self._save_checkpoint(
                 state,
                 logger,
             )
 
     def epoch_checkpoint(self, state: State, logger: Logger):
+        assert callable(self.save_interval)
         if self.save_interval(state, Event.EPOCH_CHECKPOINT) and self.last_checkpoint_batch != state.timestamp.batch:
             self._save_checkpoint(
                 state,
                 logger,
             )
 
+    def close(self, state: State, logger: Logger):
+        trained_at_least_one_batch = self.start_batch is not None and self.start_batch != state.timestamp.batch
+        if self.last_checkpoint_batch != state.timestamp.batch and trained_at_least_one_batch:
+            self._save_checkpoint(
+                state,
+                logger,
+            )
+
     def get_state_dict(self, state):
         return {
             'state': state.state_dict(),
             'rng': reproducibility.get_rng_state(),
         }
 
     def _save_checkpoint(self, state: State, logger: Logger):
```

### Comparing `composer-0.13.5/composer/callbacks/early_stopper.py` & `composer-0.14.0/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/export_for_inference.py` & `composer-0.14.0/composer/callbacks/export_for_inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/health_checker.py` & `composer-0.14.0/composer/callbacks/health_checker.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/image_visualizer.py` & `composer-0.14.0/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/lr_monitor.py` & `composer-0.14.0/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/memory_monitor.py` & `composer-0.14.0/composer/callbacks/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/callbacks/mlperf.py` & `composer-0.14.0/composer/callbacks/mlperf.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 
             if batch_size is None:
                 raise ValueError('Batch size is required to be set for dataloader.')
 
             self._log_dict({
                 constants.SEED: state.seed,
                 constants.GLOBAL_BATCH_SIZE: batch_size * dist.get_world_size(),
-                constants.GRADIENT_ACCUMULATION_STEPS: state.grad_accum,
+                constants.DEVICE_TRAIN_MICROBATCH_SIZE: state.device_train_microbatch_size,
                 constants.TRAIN_SAMPLES: num_samples,
                 constants.EVAL_SAMPLES: eval_num_samples,
             })
 
         if _local_rank_zero():
             self.mllogger.event(key=constants.INIT_STOP)
```

### Comparing `composer-0.13.5/composer/callbacks/optimizer_monitor.py` & `composer-0.14.0/composer/callbacks/optimizer_monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,27 +79,31 @@
     +-----------------------------------------------+-----------------------------------------------------+
     |                                               | Layer-wise ratio between step size and parameter    |
     | ``l2_norm_ratio/update_param/LAYER_NAME``     | norm                                                |
     |                                               |                                                     |
     +-----------------------------------------------+-----------------------------------------------------+
     """
 
-    def __init__(self, log_optimizer_metrics: bool = True):
+    def __init__(self, log_optimizer_metrics: bool = True, batch_log_interval: int = 1):
         self.log_optimizer_metrics = log_optimizer_metrics
+        self.batch_log_interval = batch_log_interval
 
     def batch_end(self, state: State, logger: Logger):
+        if state.timestamp.batch.value % self.batch_log_interval != 0:
+            return
+
         norm = 0.0
         optimizer_metrics = {}
 
         for name, p in state.model.named_parameters():
             if p.grad is not None and p.requires_grad:
 
                 metric_reporter = getattr(state.optimizers[0], 'report_per_parameter_metrics', None)
                 if callable(metric_reporter) and self.log_optimizer_metrics:
-                    optimizer_metrics = metric_reporter(p, name, optimizer_metrics)
+                    optimizer_metrics.update(metric_reporter(p, name, optimizer_metrics))
 
                 # Always log grad norm as a default metric if it's not specified
                 if f'l2_norm/grad/{name}' not in optimizer_metrics:
                     param_grad_norm = torch.linalg.vector_norm(p.grad)
                     optimizer_metrics[f'l2_norm/grad/{name}'] = param_grad_norm
 
         if state.fsdp_enabled and dist.get_world_size() > 0 and self.log_optimizer_metrics:
```

### Comparing `composer-0.13.5/composer/callbacks/runtime_estimator.py` & `composer-0.14.0/composer/callbacks/runtime_estimator.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,22 @@
             ... )
 
     The runtime estimate is logged by the :class:`.Logger` to the following key as described below.
 
     +-----------------------------------+---------------------------------------------------------+
     | Key                               | Logged data                                             |
     +===================================+=========================================================+
-    | `wall_clock/remaining_estimate`   | Estimated time to completion                            |
+    | `time/remaining_estimate`         | Estimated time to completion                            |
     +-----------------------------------+---------------------------------------------------------+
 
     Args:
         skip_batches (int, optional): Number of batches to skip before starting clock to estimate
             remaining time. Typically, the first few batches are slower due to dataloader, cache
             warming, and other reasons. Defaults to 1.
-        time_unit (str, optional): Time unit to use for `wall_clock` logging. Can be one of
+        time_unit (str, optional): Time unit to use for `time` logging. Can be one of
             'seconds', 'minutes', 'hours', or 'days'. Defaults to 'hours'.
     """
 
     def __init__(self, skip_batches: int = 1, time_unit: str = 'hours') -> None:
         self._enabled = True
         self.batches_left_to_skip = skip_batches
         self.start_time = None
@@ -133,19 +133,19 @@
                 eval_wct_avg = None
                 num_evals_finished = len(eval_wcts)
                 if num_evals_finished > 1:
                     eval_wct_avg = sum(eval_wcts[1:]) / (num_evals_finished - 1)
                 else:
                     eval_wct_avg = sum(eval_wcts) / num_evals_finished
                 eval_rate = self.eval_frequency_per_label[dataloader_label]
-                num_total_evals = 1 / eval_rate
+                num_total_evals = 1 / eval_rate * (1 - self.start_dur)
                 remaining_calls = num_total_evals - num_evals_finished
                 remaining_time += eval_wct_avg * remaining_calls
 
-            logger.log_metrics({'wall_clock/remaining_estimate': remaining_time / self.divider})
+            logger.log_metrics({'time/remaining_estimate': remaining_time / self.divider})
 
     def eval_end(self, state: State, logger: Logger) -> None:
         # If eval is called before training starts, ignore it
         if not self._enabled or self.start_time is None:
             return
         self.total_eval_wct += state.eval_timestamp.total_wct.total_seconds()
         # state.dataloader_label should always be non-None unless user explicitly sets evaluator
```

### Comparing `composer-0.13.5/composer/callbacks/speed_monitor.py` & `composer-0.14.0/composer/callbacks/speed_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,27 +194,27 @@
     |                                     |                                                           |
     +-------------------------------------+-----------------------------------------------------------+
     |                                     | `throughput/device/flops_per_sec` divided by world size.  |
     | `throughput/device/mfu`             | Only logged when model has attribute `flops_per_batch`    |
     |                                     | and `gpu_flops_available`, which can be passed as an      |
     |                                     | argument if not automatically determined by SpeedMonitor  |
     +-------------------------------------+-----------------------------------------------------------+
-    | `wall_clock/train`                  | Total elapsed training time                               |
+    | `time/train`                        | Total elapsed training time                               |
     +-------------------------------------+-----------------------------------------------------------+
-    | `wall_clock/val`                    | Total elapsed validation time                             |
+    | `time/val`                          | Total elapsed validation time                             |
     +-------------------------------------+-----------------------------------------------------------+
-    | `wall_clock/total`                  | Total elapsed time (wall_clock/train + wall_clock/val)    |
+    | `time/total`                        | Total elapsed time (time/train + time/val)                |
     +-------------------------------------+-----------------------------------------------------------+
 
     Args:
         window_size (int, optional): Number of batches to use for a rolling average of throughput.
             Defaults to 100.
         gpu_flops_available (float, optional): Number of flops available on the GPU. If not set,
             SpeedMonitor will attempt to determine this automatically. Defaults to None.
-        time_unit (str, optional): Time unit to use for `wall_clock` logging. Can be one of
+        time_unit (str, optional): Time unit to use for `time` logging. Can be one of
             'seconds', 'minutes', 'hours', or 'days'. Defaults to 'hours'.
     """
 
     def __init__(
         self,
         window_size: int = 100,
         gpu_flops_available: Optional[Union[float, int]] = None,
@@ -317,15 +317,15 @@
                 mfu = device_flops_per_sec / self.gpu_flops_available
                 logger.log_metrics({'throughput/device/mfu': mfu})
 
         # Log the time
         # `state.timestamp` excludes any time spent in evaluation
         train_wct = state.timestamp.total_wct.total_seconds()
         logger.log_metrics({
-            'wall_clock/train': train_wct / self.divider,
-            'wall_clock/val': self.total_eval_wct / self.divider,
-            'wall_clock/total': (train_wct + self.total_eval_wct) / self.divider,
+            'time/train': train_wct / self.divider,
+            'time/val': self.total_eval_wct / self.divider,
+            'time/total': (train_wct + self.total_eval_wct) / self.divider,
         })
 
     def eval_end(self, state: State, logger: Logger):
         del logger  # unused
         self.total_eval_wct += state.eval_timestamp.total_wct.total_seconds()
```

### Comparing `composer-0.13.5/composer/callbacks/threshold_stopper.py` & `composer-0.14.0/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/cli/launcher.py` & `composer-0.14.0/composer/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/__init__.py` & `composer-0.14.0/composer/core/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 :class:`~.time.Timestamp` are implemented under core.
 """
 
 from composer.core.algorithm import Algorithm
 from composer.core.callback import Callback
 from composer.core.data_spec import DataSpec, ensure_data_spec
 from composer.core.engine import Engine, Trace
-from composer.core.evaluator import Evaluator, ensure_evaluator
+from composer.core.evaluator import Evaluator, ensure_evaluator, validate_eval_automicrobatching
 from composer.core.event import Event
 from composer.core.passes import AlgorithmPass
 from composer.core.precision import Precision, get_precision_context
 from composer.core.serializable import Serializable
 from composer.core.state import State
 from composer.core.time import Time, Timestamp, TimeUnit, ensure_time
 from composer.core.types import JSON, Batch, BreakEpochException, Dataset, MemoryFormat, PyTorchScheduler, TrainerMode
@@ -43,8 +43,9 @@
     'ensure_evaluator',
     'Batch',
     'PyTorchScheduler',
     'JSON',
     'MemoryFormat',
     'TrainerMode',
     'BreakEpochException',
+    'validate_eval_automicrobatching',
 ]
```

### Comparing `composer-0.13.5/composer/core/algorithm.py` & `composer-0.14.0/composer/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/callback.py` & `composer-0.14.0/composer/core/callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/data_spec.py` & `composer-0.14.0/composer/core/data_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,119 +18,45 @@
 
 if TYPE_CHECKING:
     from composer.core.types import Batch
 
 __all__ = ['DataSpec', 'ensure_data_spec']
 
 
-def _num_microbatches_split_list(l, num_microbatches: int):
-    if len(l) < num_microbatches:
-        raise ValueError(
-            textwrap.dedent(f"""\
-        Cannot split list of length {len(l)} into {num_microbatches} batches.
-         make sure `grad_accum` is less than or equal to `train_batch_size // world_size`."""))
-
-    # Note: this is to match the behavior of tensor.chunk, which is used in _split_tensor
-    chunked_microbatch_size = math.ceil(len(l) / num_microbatches)
-    return [l[start:start + chunked_microbatch_size] for start in range(0, len(l), chunked_microbatch_size)]
-
-
-def _num_microbatches_split_tensor(t, num_microbatches: int):
-    if len(t) < num_microbatches:
-        raise ValueError(
-            textwrap.dedent(f"""\
-        Cannot split tensor of length {len(t)} into {num_microbatches} batches.
-         make sure `grad_accum` is less than or equal to `train_batch_size // world_size`."""))
-    return t.chunk(num_microbatches)
-
-
-def _num_microbatches_split_mapping(m, num_microbatches: int):
-    chunked = {}
-    for k, v in m.items():
-        if isinstance(v, torch.Tensor):
-            chunked[k] = _num_microbatches_split_tensor(v, num_microbatches)
-        elif isinstance(v, (List, Tuple)):
-            chunked[k] = _num_microbatches_split_list(v, num_microbatches)
-        elif isinstance(v, (int, float, str, bool)):
-            # Broadcast primitives to all chunks
-            chunked[k] = [v] * num_microbatches
-        else:
-            raise ValueError(f'Unsupported batch type: {type(v)}.')
-    num_chunks = len(list(chunked.values())[0])
-    return [{k: v[idx] for k, v in chunked.items()} for idx in range(num_chunks)]
-
-
-def _num_microbatches_split_batch(batch: Any, num_microbatches: int) -> Sequence:
-    """Splits batch into `num_microbatches` chunks for gradient accumulation.
-
-    Works with tensors, dictionaries of tensors, (x, y) tuples, and lists where ``batch`` is the 2nd dimension.
-
-    Args:
-        batch (Any): output from the dataloader.
-        num_microbatches (int): number of microbatches to batch into. Will be set by `grad_accum`.
-    """
-    if num_microbatches < 1:
-        raise ValueError('num_microbatches must be at least 1')
-    if num_microbatches == 1:
-        return [batch]
-
-    if isinstance(batch, torch.Tensor):  # check for a single stack of tensors
-        return _num_microbatches_split_tensor(batch, num_microbatches)
-
-    if isinstance(batch, Mapping):  # check for dictionary (hf style)
-        return _num_microbatches_split_mapping(batch, num_microbatches)
-
-    if isinstance(batch, (Tuple, list)) and _check_list_is_primitives(batch):  # check for list of primitives
-        return _num_microbatches_split_list(batch, num_microbatches)
-
-    if isinstance(batch, (Tuple, List)):  # check for batch on 2nd dimension
-        result = []
-        for item in batch:
-            if isinstance(item, torch.Tensor):
-                result.append(_num_microbatches_split_tensor(item, num_microbatches))
-            elif isinstance(item, (List, Tuple)):
-                result.append(_num_microbatches_split_list(item, num_microbatches))
-            else:
-                raise ValueError(f'Unsupported batch type: {type(item)}.')
-        return list(zip(*result))
-
-    raise NotImplementedError(
-        textwrap.dedent("""\
-            The default `split_fn` is unable to split the output of this dataloader. To enable microbatching,
-             please and specify a `DataSpec` with `split_batch` for your dataset and use `device_train_microbatch_size`."""
-                       ))
-
-
 def _split_list(l, microbatch_size: int):
     if len(l) < microbatch_size:
         warnings.warn(f'Cannot split list of length {len(l)} into batches of size {microbatch_size}. '
-                      'As it is smaller, no splitting will be done.')
+                      'As it is smaller, no splitting will be done. This may happen on the last batch '
+                      'of a dataset if it is a smaller size than the microbatch size.')
         microbatch_size = len(l)
     num_microbatches = math.ceil(len(l) / microbatch_size)
     # Note: this is to match the behavior of tensor.chunk, which is used in _split_tensor
     chunked_microbatch_size = math.ceil(len(l) / num_microbatches)
     return [l[start:start + chunked_microbatch_size] for start in range(0, len(l), chunked_microbatch_size)]
 
 
 def _split_tensor(t, microbatch_size: int):
     if len(t) < microbatch_size:
         warnings.warn(f'Cannot split tensor of length {len(t)} into batches of size {microbatch_size}. '
-                      'As it is smaller, no splitting will be done.')
+                      'As it is smaller, no splitting will be done. This may happen on the last batch '
+                      'of a dataset if it is a smaller size than the microbatch size.')
         microbatch_size = len(t)
     num_microbatches = math.ceil(len(t) / microbatch_size)
     return t.chunk(num_microbatches)
 
 
 def _split_mapping(m, microbatch_size: int):
     chunked = {}
     for k, v in m.items():
         if isinstance(v, torch.Tensor):
             chunked[k] = _split_tensor(v, microbatch_size)
         elif isinstance(v, (List, Tuple)):
             chunked[k] = _split_list(v, microbatch_size)
+        elif isinstance(v, Mapping):
+            chunked[k] = _split_mapping(v, microbatch_size)
         elif isinstance(v, (int, float, str, bool)):
             # Defer broadcasting primitives until we know num_chunks
             pass
         else:
             raise ValueError(f'Unsupported batch type: {type(v)}.')
     num_chunks = 1  # Default to 1 chunks if there are no tensors or everything is primitive
     if len(chunked.keys()) != 0:
@@ -237,17 +163,18 @@
 
             By default, if the batch contains tensors that all have the same 0th dim, then the value of the 0th dim will
             be returned. If the batch contains tensors where the 0th dim differ, then this function must be specified.
 
         get_num_tokens_in_batch ((Batch) -> int, optional): Function that is called by the :class:`.Trainer` to
             get the number of tokens in the provided batch.
 
-            By default, it returns 0, meaning that number of tokens processed will not be tracked as a part of the
-            training progress tracking. This function must be specified to track the number of tokens processed during
-            training.
+            By default, it checks for HuggingFace-style dictionary batches with ``input_ids``, and then checks ``dataset.max_seq_len``, and returns 0
+            if both of those fail, meaning that number of tokens processed will not be tracked as a part of the training progress tracking.
+            Note that the defaults do NOT take padding into account, so if you want the token calculation to exclude padding, you should specify this function.
+            This function must be specified to track the number of tokens processed during training in a non-default way.
     """
 
     def __init__(
         self,
         dataloader: Union[Iterable, torch.utils.data.DataLoader],
         num_samples: Optional[int] = None,
         num_tokens: Optional[int] = None,
@@ -256,15 +183,14 @@
         get_num_samples_in_batch: Optional[Callable[[Batch], int]] = None,
         get_num_tokens_in_batch: Optional[Callable[[Batch], int]] = None,
     ) -> None:
         self.dataloader: Union[Iterable, torch.utils.data.DataLoader] = dataloader
         self.num_tokens = num_tokens
         self.device_transforms = self._default_device_transforms if device_transforms is None else device_transforms
         self.split_batch = _default_split_batch if split_batch is None else split_batch
-        self._num_microbatches_split_batch = _num_microbatches_split_batch  # For fallback using `grad_accum`
         self.get_num_samples_in_batch = self._default_get_num_samples_in_batch if get_num_samples_in_batch is None else get_num_samples_in_batch
         self.get_num_tokens_in_batch = self._default_get_num_tokens_in_batch if get_num_tokens_in_batch is None else get_num_tokens_in_batch
 
         if num_samples is not None:
             self.num_samples = num_samples
         else:
             if isinstance(dataloader, torch.utils.data.DataLoader) and isinstance(dataloader.dataset,
@@ -331,15 +257,22 @@
             raise NotImplementedError(
                 textwrap.dedent(f"""\
                     Cannot determine the batch size, as multiple Tensors of
                     different lengths were found in the batch: sizes in batch: {dim0_sizes}.
                     Please use a DataSpec and specify `get_num_samples_in_batch`."""))
 
     def _default_get_num_tokens_in_batch(self, batch: Batch) -> int:
-        del batch  # unused
+        # First try HuggingFace-style input dicts
+        if isinstance(batch, Mapping) and 'input_ids' in batch:
+            samples_per_batch = batch['input_ids'].shape[0]
+            return batch['input_ids'].shape[1] * samples_per_batch
+        # Then try dataset.max_seq_len
+        elif hasattr(self.dataloader, 'dataset') and hasattr(self.dataloader.dataset, 'max_seq_len'):  # type: ignore
+            samples_per_batch = self.get_num_samples_in_batch(batch)
+            return self.dataloader.dataset.max_seq_len * samples_per_batch  # type: ignore
         return 0
 
 
 def ensure_data_spec(dataloader: Union[DataSpec, Iterable, dict]) -> DataSpec:
     """Ensures that the ``dataloader`` is a :class:`.DataSpec`.
 
     Args:
```

### Comparing `composer-0.13.5/composer/core/engine.py` & `composer-0.14.0/composer/core/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 from __future__ import annotations
 
 import atexit
 import contextlib
 import logging
 import os
+import signal
+import sys
 import textwrap
 import weakref
 from collections import OrderedDict
 from dataclasses import dataclass
 from typing import Callable, ContextManager, Dict, List, Optional, Sequence, Tuple, TypeVar, Union, cast
 
 from composer.core import passes
@@ -110,14 +112,25 @@
 
 
 # Since atexit calls hooks in LIFO order, this hook will always be invoked after all atexit-triggered
 # _close() calls are invoked
 atexit.register(_set_atexit_ran)
 
 
+# Catch SIGTERM/SIGINT and instead exit via `sys.exit` using same error code, ensuring atexit
+# functions still run. Composer CLI launcher will give a 30 second grace period before sending
+# SIGKILL.
+def sigterm_handler(signal, frame):
+    sys.exit(128 + signal)
+
+
+signal.signal(signal.SIGTERM, sigterm_handler)
+signal.signal(signal.SIGINT, sigterm_handler)
+
+
 def _get_default_passes():
     return [
         passes.sort_selective_backprop_first,
         passes.sort_fused_layernorm_last,
         passes.sort_low_precision_layernorm_last,
         passes.set_filo_order,
         passes.warn_if_multiple_loss_interpolation,
```

### Comparing `composer-0.13.5/composer/core/evaluator.py` & `composer-0.14.0/composer/loggers/console_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,209 +1,205 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
-"""A wrapper for a dataloader to include metrics that apply to a specific dataset."""
+"""Logs metrics to the console and without a progress bar."""
 
 from __future__ import annotations
 
-import math
-import warnings
-from typing import Any, Callable, Dict, Iterable, List, Optional, Union
-
-from torchmetrics import Metric, MetricCollection
-
-from composer.core.data_spec import DataSpec, ensure_data_spec
-from composer.core.event import Event
-from composer.core.state import State
+import sys
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, TextIO, Union
+
+import numpy as np
+import yaml
+
 from composer.core.time import Time, TimeUnit
+from composer.loggers.logger import Logger, format_log_data_value
+from composer.loggers.logger_destination import LoggerDestination
+from composer.utils import dist
 
-__all__ = ['Evaluator', 'evaluate_periodically', 'ensure_evaluator']
+if TYPE_CHECKING:
+    from composer.core import State
 
+# We use deciles here, so 11 events because deciles including 0.
+NUM_EVAL_LOGGING_EVENTS = 11
 
-def evaluate_periodically(eval_interval: Union[str, Time, int], eval_at_fit_end: bool = True):
-    """Helper function to generate an evaluation interval callable.
 
-    Args:
-        eval_interval (str | Time | int): A :class:`.Time` instance or time string, or integer in epochs,
-            representing how often to evaluate. Set to ``0`` to disable evaluation.
-        eval_at_fit_end (bool): Whether to evaluate at the end of training, regardless of `eval_interval`.
-            Default: True
-    Returns:
-        (State, Event) -> bool: A callable for the ``eval_interval`` argument of an
-            :class:`.Evaluator`.
-    """
-    if isinstance(eval_interval, int):
-        eval_interval = Time(eval_interval, TimeUnit.EPOCH)
-    if isinstance(eval_interval, str):
-        eval_interval = Time.from_timestring(eval_interval)
-
-    if eval_interval.unit not in (TimeUnit.EPOCH, TimeUnit.BATCH, TimeUnit.DURATION):
-        raise ValueError('The `eval_interval` must have units of EPOCH, BATCH, DURATION or be a function.')
-
-    last_batch_seen = -1
-
-    def should_eval(state: State, event: Event):
-        # `TimeUnit.Duration` value is a float from `[0.0, 1.0)`
-        if not eval_interval.unit == TimeUnit.DURATION and int(eval_interval) <= 0:
-            return False
-        nonlocal last_batch_seen  # required to use the last_batch_seen from the outer function scope
-
-        # if requested, evaluate at the end of training, as long as the length of training is specified.
-        if eval_at_fit_end and event == Event.FIT_END and state.timestamp.batch != last_batch_seen:
-            return True
-
-        if eval_interval.unit == TimeUnit.EPOCH and int(
-                state.timestamp.epoch) % int(eval_interval) == 0 and event == Event.EPOCH_END:
-            last_batch_seen = state.timestamp.batch
-            return True
-
-        if eval_interval.unit == TimeUnit.BATCH and int(
-                state.timestamp.batch) % int(eval_interval) == 0 and event == Event.BATCH_END:
-            last_batch_seen = state.timestamp.batch
-            return True
+class ConsoleLogger(LoggerDestination):
+    """Log metrics to the console.
 
-        if eval_interval.unit == TimeUnit.DURATION:
-            assert state.max_duration is not None, 'max_duration should not be None'
-            if state.dataloader_len is None:
-                raise RuntimeError(
-                    f'Evaluation interval of type `dur` or {TimeUnit.DURATION} requires the dataloader to be sized.')
-            if state.max_duration.unit == TimeUnit.EPOCH and int(
-                    state.timestamp.batch) % math.ceil(state.max_duration.value * float(eval_interval) *
-                                                       state.dataloader_len) == 0 and event == Event.BATCH_END:
-                last_batch_seen = state.timestamp.batch
-                return True
-            elif state.max_duration.unit == TimeUnit.BATCH and int(state.timestamp.batch) % math.ceil(
-                    state.max_duration.value * eval_interval.value) == 0 and event == Event.BATCH_END:
-                last_batch_seen = state.timestamp.batch
-                return True
-            elif state.max_duration.unit == TimeUnit.SAMPLE and event == Event.BATCH_END:
-                # If last sample in batch is not evenly divisible by eval_interval, perform evaluation in next batch
-                if int(state.timestamp.batch) > 0:
-                    samples_in_a_batch = int(state.timestamp.sample) // int(state.timestamp.batch)
-                    if int(state.timestamp.sample) // math.ceil(state.max_duration.value * eval_interval) != int(
-                            state.timestamp.sample - samples_in_a_batch) // math.ceil(
-                                state.max_duration.value * eval_interval):
-                        last_batch_seen = state.timestamp.batch
-                        return True
-            elif state.max_duration.unit == TimeUnit.TOKEN and event == Event.BATCH_END:
-                raise ValueError(f'Evaluation interval of type `dur` is not supported yet for max_duration as `tok`')
-        return False
-
-    return should_eval
-
-
-class Evaluator:
-    """A wrapper for a dataloader to include metrics that apply to a specific dataset.
-
-    For example, :class:`.CrossEntropyLoss` metric for NLP models.
-
-    .. doctest::
-
-       >>> eval_evaluator = Evaluator(
-       ...     label='myEvaluator',
-       ...     dataloader=eval_dataloader,
-       ...     metric_names=['MulticlassAccuracy']
-       ... )
-       >>> trainer = Trainer(
-       ...     model=model,
-       ...     train_dataloader=train_dataloader,
-       ...     eval_dataloader=eval_evaluator,
-       ...     optimizers=optimizer,
-       ...     max_duration='1ep',
-       ... )
+    .. note::
 
-    Args:
-        label (str): Name of the Evaluator.
-        dataloader (DataSpec | Iterable | Dict[str, Any]): Iterable that yields batches, a :class:`.DataSpec`
-            for evaluation, or a Dict of :class:`.DataSpec` kwargs.
-        metric_names: The list of metric names to compute.
-            Each value in this list can be a regex string (e.g. "MulticlassAccuracy", "f1" for "BinaryF1Score",
-            "Top-." for "Top-1", "Top-2", etc). Each regex string will be matched against the keys of the dictionary returned
-            by ``model.get_metrics()``. All matching metrics will be evaluated.
-
-            By default, if left blank, then all metrics returned by ``model.get_metrics()`` will be used.
-        subset_num_batches (int, optional): The maximum number of batches to use for each evaluation. Defaults to ``None``,
-            which means that the ``eval_subset_num_batches`` parameter from the :class:`.Trainer` will be used.
-            Set to ``-1`` to evaluate the entire ``dataloader``.
-        eval_interval (Time | int | str | (State, Event) -> bool, optional): An integer,
-            which will be interpreted to be epochs, a str (e.g. ``1ep``, or ``10ba``), a :class:`.Time` object, or a callable.
-            Defaults to ``None``, which means that the ``eval_interval`` parameter from the :class:`.Trainer` will be used.
-
-            If an integer (in epochs), :class:`.Time` string, or :class:`.Time` instance, the evaluator will be run
-            with this frequency. :class:`.Time` strings or :class:`.Time` instances must have units of
-            :attr:`.TimeUnit.BATCH` or :attr:`.TimeUnit.EPOCH`.
-
-            Set to ``0`` to disable evaluation.
-
-            If a callable, it should take two arguments (:class:`.State`, :class:`.Event`) and return a bool
-            representing whether the evaluator should be invoked. The event will be either :attr:`.Event.BATCH_END`
-            or :attr:`.Event.EPOCH_END`.
+        This logger is automatically instantiated by the trainer via the ``log_to_console``,
+        and ``console_stream`` options. This logger does not need to be created manually.
 
-            When specifying ``eval_interval``, the evaluator(s) are also run at the ``Event.FIT_END`` if it doesn't
-            evenly divide the training duration.
+    Args:
+        log_interval (int | str | Time): How frequently to log to console. (default: ``'1ep'``)
+        stream (str | TextIO, optional): The console stream to use. If a string, it can either be ``'stdout'`` or
+            ``'stderr'``. (default: :attr:`sys.stderr`)
+        log_traces (bool): Whether to log traces or not. (default: ``False``)
     """
 
-    def __init__(
-        self,
-        *,
-        label: str,
-        dataloader: Union[DataSpec, Iterable, Dict[str, Any]],
-        metric_names: Optional[List[str]] = None,
-        metrics: Optional[Union[Metric, MetricCollection]] = None,
-        subset_num_batches: Optional[int] = None,
-        eval_interval: Optional[Union[int, str, Time, Callable[[State, Event], bool]]] = None,
-    ):
-        self.label = label
-        self.dataloader = ensure_data_spec(dataloader)
-
-        self.metric_names = []
-        if metric_names is not None and metrics is not None:
-            raise ValueError('only one of ``metrics`` or ``metric_names`` should be specified.')
-        elif metric_names is not None:
-            if not isinstance(metric_names, list):
-                raise ValueError(f'``metric_names`` should be a list of strings, not a {type(metric_names)}')
-            self.metric_names = metric_names
-        elif metrics is not None:
-            warnings.warn(DeprecationWarning('``metrics`` is deprecated and will be removed in 0.13.0.'))
-            if isinstance(metrics, Metric):
-                self.metric_names = [metrics.__class__.__name__]
+    def __init__(self,
+                 log_interval: Union[int, str, Time] = '1ba',
+                 stream: Union[str, TextIO] = sys.stderr,
+                 log_traces: bool = False) -> None:
+
+        if isinstance(log_interval, int):
+            log_interval = Time(log_interval, TimeUnit.EPOCH)
+        if isinstance(log_interval, str):
+            log_interval = Time.from_timestring(log_interval)
+
+        if log_interval.unit not in (TimeUnit.EPOCH, TimeUnit.BATCH):
+            raise ValueError('The `console_log_interval` argument must have units of EPOCH or BATCH.')
+
+        self.log_interval = log_interval
+        # set the stream
+        if isinstance(stream, str):
+            if stream.lower() == 'stdout':
+                stream = sys.stdout
+            elif stream.lower() == 'stderr':
+                stream = sys.stderr
             else:
-                self.metric_names = [str(k) for k, _ in metrics.items()]
-
-        self.subset_num_batches = subset_num_batches
-        self._eval_interval = None
-        self.eval_interval = eval_interval
-
-    @property
-    def eval_interval(self):
-        return self._eval_interval
-
-    @eval_interval.setter
-    def eval_interval(self, eval_interval: Optional[Union[int, str, Time, Callable[[State, Event], bool]]]):
-        if eval_interval is None:
-            self._eval_interval = None
-        elif not callable(eval_interval):
-            self._eval_interval = evaluate_periodically(eval_interval)
+                raise ValueError(f'stream must be one of ("stdout", "stderr", TextIO-like), got {stream}')
+        self.should_log_traces = log_traces
+        self.stream = stream
+        self.hparams: Dict[str, Any] = {}
+        self.hparams_already_logged_to_console: bool = False
+        self.logged_metrics: Dict[str, float] = {}
+        self.eval_batch_idxs_to_log: Sequence[int] = []
+
+    def log_traces(self, traces: Dict[str, Any]):
+        if self.should_log_traces:
+            for trace_name, trace in traces.items():
+                trace_str = format_log_data_value(trace)
+                self._log_to_console(f'[trace]: {trace_name}:' + trace_str + '\n')
+
+    def log_hyperparameters(self, hyperparameters: Dict[str, Any]):
+        # Lazy logging of hyperparameters.
+        self.hparams.update(hyperparameters)
+
+    def log_metrics(self, metrics: Dict[str, float], step: Optional[int] = None) -> None:
+        del step
+        # Lazy logging of metrics.
+        # Stores all metrics logged until they are cleared with a log_to_console call
+        self.logged_metrics.update(metrics)
+
+    def _log_hparams_to_console(self):
+        if dist.get_local_rank() == 0:
+            self._log_to_console('*' * 30)
+            self._log_to_console('Config:')
+            self._log_to_console(yaml.dump(self.hparams))
+            self._log_to_console('*' * 30)
+
+    def epoch_end(self, state: State, logger: Logger) -> None:
+        cur_epoch = int(state.timestamp.epoch)  # epoch gets incremented right before EPOCH_END
+        unit = self.log_interval.unit
+
+        if unit == TimeUnit.EPOCH and (cur_epoch % int(self.log_interval) == 0 or cur_epoch == 1):
+            self.log_to_console(self.logged_metrics, prefix='Train ', state=state)
+        # Always clear logged metrics so they don't get logged in a subsequent eval call. The
+        # metrics will be recomputed and overridden in future batches so they can be safely
+        # discarded.
+        self.logged_metrics = {}
+
+    def batch_end(self, state: State, logger: Logger) -> None:
+        cur_batch = int(state.timestamp.batch)
+        unit = self.log_interval.unit
+        if unit == TimeUnit.BATCH and (cur_batch % int(self.log_interval) == 0 or cur_batch == 1):
+            self.log_to_console(self.logged_metrics, prefix='Train ', state=state)
+            # Clear logged metrics.
+            self.logged_metrics = {}
+
+    def fit_end(self, state: State, logger: Logger) -> None:
+        # Always clear logged metrics so they don't get logged in a subsequent eval call.
+        self.logged_metrics = {}
+
+    def eval_batch_end(self, state: State, logger: Logger) -> None:
+        cur_batch = int(state.eval_timestamp.batch)
+        if cur_batch in self.eval_batch_idxs_to_log:
+            self.log_to_console({}, prefix='Eval ', state=state, is_train=False)
+
+    def eval_end(self, state: State, logger: Logger) -> None:
+        # Log to the console at the end of eval no matter what log interval is selected.
+        self.log_to_console(self.logged_metrics, prefix='Eval ', state=state, is_train=False)
+        self.logged_metrics = {}
+
+    def fit_start(self, state: State, logger: Logger) -> None:
+        if not self.hparams_already_logged_to_console:
+            self.hparams_already_logged_to_console = True
+            self._log_hparams_to_console()
+
+    def predict_start(self, state: State, logger: Logger) -> None:
+        if not self.hparams_already_logged_to_console:
+            self.hparams_already_logged_to_console = True
+            self._log_hparams_to_console()
+
+    def eval_start(self, state: State, logger: Logger) -> None:
+        total_eval_batches = self._get_total_eval_batches(state)
+        deciles = np.linspace(0, 1, NUM_EVAL_LOGGING_EVENTS)
+        batch_idxs = np.arange(1, total_eval_batches + 1)
+        if total_eval_batches < NUM_EVAL_LOGGING_EVENTS:
+            self.eval_batch_idxs_to_log = list(batch_idxs)
         else:
-            self._eval_interval = eval_interval
-
-
-def ensure_evaluator(evaluator: Union[Evaluator, DataSpec, Iterable, Dict[str, Any]], default_metric_names: List[str]):
-    """Ensure that ``evaluator`` is an :class:`.Evaluator`.
-
-    Args:
-        evaluator (Evaluator | DataSpec | Iterable | Dict[str, Any]): A dataloader,
-            :class:`.DataSpec` instance, dictionary of :class:`.DataSpec` kwargs, or existing evaluator.
-        default_metric_names (List[str]): The names of the metrics for the ``evaluator``,
-            if a dataloader was specified.
+            self.eval_batch_idxs_to_log = list(np.quantile(batch_idxs, deciles).round().astype(dtype=int))
+        # Remove index of last batch, so that we don't print progress at end of last batch and then
+        # at eval end.
+        last_batch_idx = total_eval_batches
+        self.eval_batch_idxs_to_log.remove(last_batch_idx)
+        if not self.hparams_already_logged_to_console:
+            self.hparams_already_logged_to_console = True
+            self._log_hparams_to_console()
+
+    def _get_eval_progress_string(self, state: State):
+        eval_batch = state.eval_timestamp.batch.value
+        eval_dataloader_label = state.dataloader_label
+        total_eval_batches = self._get_total_eval_batches(state)
+        curr_progress = f'[Eval batch={eval_batch}/{total_eval_batches}] Eval on {eval_dataloader_label} data'
+        return curr_progress
+
+    def _get_total_eval_batches(self, state: State) -> int:
+        cur_evaluator = [evaluator for evaluator in state.evaluators if evaluator.label == state.dataloader_label][0]
+        total_eval_batches = int(
+            state.dataloader_len) if state.dataloader_len is not None else cur_evaluator.subset_num_batches
+        # To please pyright. Based on _set_evaluator_interval_and_subset_num_batches, total_eval_batches can't be None
+        assert total_eval_batches is not None
+        return total_eval_batches
+
+    def _get_progress_string(self, state: State):
+        if state.max_duration is None:
+            training_progress = ''
+        elif state.max_duration.unit == TimeUnit.EPOCH:
+            cur_batch = int(state.timestamp.batch_in_epoch)
+            cur_epoch = int(state.timestamp.epoch)
+            if cur_batch == 0 and cur_epoch != 0:
+                cur_epoch -= 1
+                cur_batch = int(state.dataloader_len) if state.dataloader_len is not None else cur_batch
+            if state.dataloader_len is None:
+                curr_progress = f'[batch={cur_batch}]'
+            else:
+                total = int(state.dataloader_len)
+                curr_progress = f'[batch={cur_batch}/{total}]'
 
-    Returns:
-        Evaluator: An evaluator.
-    """
-    if isinstance(evaluator, Evaluator):
-        return evaluator
-    else:
-        return Evaluator(
-            label='eval',
-            dataloader=evaluator,
-            metric_names=default_metric_names,
-        )
+            training_progress = f'[epoch={cur_epoch + 1}]{curr_progress}'
+        else:
+            unit = state.max_duration.unit
+            curr_duration = int(state.timestamp.get(unit))
+            total = state.max_duration.value
+            training_progress = f'[{unit.name.lower()}={curr_duration}/{total}]'
+        return training_progress
+
+    def log_to_console(self, data: Dict[str, Any], state: State, prefix: str = '', is_train=True) -> None:
+        # log to console
+        if is_train:
+            progress = self._get_progress_string(state)
+        else:
+            progress = self._get_eval_progress_string(state)
+        log_str = f'{progress}' + (':' if len(data) > 0 else '')
+        for data_name, data in data.items():
+            data_str = format_log_data_value(data)
+            log_str += f'\n\t {prefix}{data_name}: {data_str}'
+        self._log_to_console(log_str)
+
+    def _log_to_console(self, log_str: str):
+        """Logs to the console, avoiding interleaving with a progress bar."""
+        # write directly to self.stream; no active progress bar
+        print(log_str, file=self.stream, flush=True)
```

### Comparing `composer-0.13.5/composer/core/event.py` & `composer-0.14.0/composer/core/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                     break
                 # <AFTER_DATALOADER>
 
                 # <BATCH_START>
 
                 # <BEFORE_TRAIN_BATCH>
 
-                for microbatch in batch.split(grad_accum):
+                for microbatch in batch.split(device_train_microbatch_size):
 
                     # <BEFORE_FORWARD>
                     outputs = model(batch)
                     # <AFTER_FORWARD>
 
                     # <BEFORE_LOSS>
                     loss = model.loss(outputs, batch)
```

### Comparing `composer-0.13.5/composer/core/passes.py` & `composer-0.14.0/composer/core/passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/precision.py` & `composer-0.14.0/composer/core/precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/serializable.py` & `composer-0.14.0/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/state.py` & `composer-0.14.0/composer/core/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 """The state of the trainer."""
 from __future__ import annotations
 
 import collections.abc
 import logging
 import textwrap
 import warnings
+from collections import OrderedDict
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Optional, Sequence, Union, cast
 
 import torch
 import torch.nn.modules.utils
 from packaging import version
 from torch.nn.parallel import DistributedDataParallel
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader, Dataset
 from torchmetrics import Metric
-from torchmetrics.metric import jit_distributed_available
 
 from composer.core.data_spec import DataSpec
 from composer.core.event import Event
 from composer.core.precision import Precision
 from composer.core.serializable import Serializable
 from composer.core.time import Time, Timestamp, TimeUnit
 from composer.devices import Device
 from composer.utils import batch_get, batch_set, dist, ensure_tuple, get_composer_env_dict, is_model_deepspeed
+from composer.utils.misc import using_torch_2
 
 if TYPE_CHECKING:
     import deepspeed
 
     import composer.core.types as types
     from composer.core.algorithm import Algorithm
     from composer.core.callback import Callback
@@ -115,27 +116,69 @@
 
     Returns:
         Dict[str, Any]: The state_dict for the given optimizer.
     """
     if version.parse(torch.__version__) < version.parse('1.13.0'):
         raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
     from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+    if not using_torch_2():
+        optim_state_dict = _legacy_fsdp_get_optim_state_dict(model, optim, state_dict_type)
+    else:
+        with fsdp_state_dict_type_context(module=model, state_dict_type=state_dict_type):
+            optim_state_dict = FSDP.optim_state_dict(model, optim)  # type: ignore
+    return optim_state_dict
+
+
+def _legacy_fsdp_get_optim_state_dict(model: torch.nn.Module,
+                                      optim: torch.optim.Optimizer,
+                                      state_dict_type: str = 'full') -> Dict[str, Any]:
+    if version.parse(torch.__version__) < version.parse('1.13.0'):
+        raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
+    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
     if state_dict_type == 'full':
         # Converts local state dict to full.
         return FSDP.full_optim_state_dict(model=model, optim=optim)
     elif state_dict_type == 'sharded':
         # Converts local state dict to sharded.
         return FSDP.sharded_optim_state_dict(model=model, optim=optim)
     elif state_dict_type == 'local':
         # State dict is already local, so just return state dict.
         return optim.state_dict()
     else:
         raise NotImplementedError(f'No valid FSDP state_dict_type for {state_dict_type}')
 
 
+def _legacy_optim_state_dict_to_load(
+    optim_state_dict: Dict[str, Any],
+    model: torch.nn.Module,
+    optim: torch.optim.Optimizer,
+    state_dict_type: str = 'full',
+):
+    if version.parse(torch.__version__) < version.parse('1.13.0'):
+        raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
+    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+    if state_dict_type == 'sharded':
+        # Optimizer and optimizer state dict are already sharded, but not
+        # flattened, so we flatten the state dict then load it.
+        flattened_optim_state_dict = FSDP.flatten_sharded_optim_state_dict(sharded_optim_state_dict=optim_state_dict,
+                                                                           model=model,
+                                                                           optim=optim)
+        return flattened_optim_state_dict
+    elif state_dict_type == 'local':
+        # Optimizer and optimizer state dict are already sharded and flattened,
+        # so just load the state_dict.
+        return optim_state_dict
+    else:  # fsdp_state_dict_type == 'full'
+        # FSDP enabled, but fsdp_state_dict is set to 'full', so the state dict
+        # is a full state dict and we must shard and flatten it first before loading it.
+        sharded_optim_state_dict = FSDP.scatter_full_optim_state_dict(full_optim_state_dict=optim_state_dict,
+                                                                      model=model)
+        return sharded_optim_state_dict
+
+
 def get_fsdp_sharded_optim_state_dict(full_optim_state_dict: Dict[str, Any], model: torch.nn.Module):
     if version.parse(torch.__version__) < version.parse('1.13.0'):
         raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
     from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
     log.debug(
         f'Scattering optimizer state dict with keys {full_optim_state_dict.keys()} and model of type {type(model)}')
     return FSDP.scatter_full_optim_state_dict(full_optim_state_dict=full_optim_state_dict, model=model)
@@ -153,28 +196,14 @@
     # It also renamed _is_model_ddp_wrapped to is_model_ddp
     state = {}
     for attribute_name, serialized_value in state_dict.items():
         if attribute_name == '_is_model_ddp_wrapped':
             attribute_name = 'is_model_ddp'
         if attribute_name.startswith('_'):
             attribute_name = attribute_name[1:]
-        # Torchmetrics adds a new attribute as of 0.11 which must be added to deserialized metrics
-        if attribute_name == 'train_metrics':
-            for metric_name in serialized_value.keys():
-                metric = serialized_value[metric_name]
-                if not hasattr(metric, 'distributed_available_fn'):
-                    metric.distributed_available_fn = jit_distributed_available
-                    serialized_value[metric_name] = metric
-        elif attribute_name == 'eval_metrics':
-            for evaluator_name, eval_metrics in serialized_value.items():
-                for metric_name in eval_metrics.keys():
-                    metric = eval_metrics[metric_name]
-                    if not hasattr(metric, 'distributed_available_fn'):
-                        metric.distributed_available_fn = jit_distributed_available
-                        serialized_value[evaluator_name][metric_name] = metric
         state[attribute_name] = serialized_value
     return state
 
 
 _STATE_DICT_SERIALIZED_ATTRIBUTES = [
     # List of attributes that are serialized with state_dict
     # Only the attributes listed in state.serialized_attributes will actually be saved.
@@ -203,21 +232,16 @@
 
     Args:
         model (torch.nn.Module): The model, typically as a subclass of :class:`~.ComposerModel`.
         rank_zero_seed (int): The seed used on the rank zero process. It is assumed that each rank's seed is
             ``rank_zero_seed + dist.get_global_rank()``.
         run_name (str): The name for this training run.
         device (Device): The device used by this process. The trainer moves the model and loaded data to this device.
-        grad_accum (int, optional): The number of gradient accumulation steps to use. With this argument, micro batch
-            size for each device becomes ``microbatch_size = train_batch_size / (num_devices * grad_accum)``.
-        eval_batch_split (int, optional): The mirror of grad_accum for eval. With this argument, micro batch
-            size for each device becomes ``microbatch_size = eval_batch_size / (num_devices * eval_batch_split)``.
         device_train_microbatch_size (int, optional): The microbatch size for each device during training.
         auto_microbatching (bool, optional): Whether automatic microbatching is enabled.
-        using_device_microbatch_size (bool, optional): Whether device_train_microbatch_size is set by the user.
         train_dataloader (Iterable, optional): Dataloader used for training
         evaluators (Evaluator | Evaluators, optional): :class:`.Evaluator` used for evaluation.
         dataloader (Iterable, optional): The active DataLoader.
         dataloader_len (int | Time[int], optional): The number of batches per dataloader iteration (e.g. epoch).
             The trainer will yield the first ``dataloader_len`` batches per iteration. If ``-1`` (the default),
             the entire dataloader will be iterated over.
         dataloader_label (str, optional): The name for the dataloader. Required if ``dataloader`` is specified.
@@ -258,15 +282,15 @@
             >>> trainer.fit()
             >>> trainer.state.train_metrics
             {'MulticlassAccuracy': MulticlassAccuracy()}
 
         eval_metrics (Dict[str, Dict[str, Metric]]): The current evaluation metrics, organized
             by dataloader label and then by metric name. If not using an :class:`.Evaluator`,
             the eval dataloader is labeled ``'eval'``. Otherwise, in the case of having multiple evaluation datasets,
-            the evaluator label is used. See the `Multiple Datasets Documentation <https://docs.mosaicml.com/en/stable/trainer/evaluation.html#multiple-datasets>`_
+            the evaluator label is used. See the `Multiple Datasets Documentation <https://docs.mosaicml.com/projects/composer/en/stable/trainer/evaluation.html#multiple-datasets>`_
             for more information. ``eval_metrics`` will be deep-copied to ensure that each evaluator updates only its ``eval_metrics``.
 
             For example:
             >>> from composer.metrics import CrossEntropy
             >>> trainer = Trainer(
             ...     ...,
             ...     train_dataloader=train_dataloader,
@@ -294,15 +318,14 @@
             ... )
             >>> trainer.fit()
             >>> trainer.state.eval_metrics
             {'eval1': {'MulticlassAccuracy': MulticlassAccuracy()}, 'eval2': {'MulticlassAccuracy': MulticlassAccuracy()}}
         eval_timestamp (Timestamp): The timestamp for the current evaluation dataloader. This timestamp is reset
             before the dataloader is evaluated. The :attr:`~Timestamp.epoch` attribute for this timestamp is always
             ``0``.
-        grad_accum (int): The number of gradient accumulation steps per batch.
         device_train_microbatch_size (int): The size of each train microbatch per device.
         loss (torch.Tensor | Sequence[torch.Tensor]): The most recently computed loss.
         model (torch.nn.Module): The training model.
 
             .. note::
 
                 When using DeepSpeed or multi-rank training, the model will be wrapped with
@@ -368,19 +391,16 @@
         # device
         device: Device,
 
         # stopping conditions
         max_duration: Optional[Union[str, Time[int]]] = None,
 
         # data configurations
-        grad_accum: Optional[int] = 1,
-        eval_batch_split: int = 1,
         device_train_microbatch_size: Optional[int] = None,
         auto_microbatching: bool = False,
-        using_device_microbatch_size: bool = True,
 
         # dataloaders
         train_dataloader: Optional[Iterable] = None,
         evaluators: Optional[Union[Evaluator, Sequence[Evaluator]]] = None,
 
         # these track the current 'active' dataloader
         # depending on train, eval, or others
@@ -407,31 +427,29 @@
         deepspeed_config: Optional[Dict[str, Any]] = None,
         fsdp_config: Optional[Dict[str, Any]] = None,
     ):
         self.rank_zero_seed = rank_zero_seed
         self.model = model
         self.run_name = run_name
         self.device = device
-        self.grad_accum = grad_accum
-        self.eval_batch_split = eval_batch_split
         self.device_train_microbatch_size = device_train_microbatch_size
         self.auto_microbatching = auto_microbatching
-        self.using_device_microbatch_size = using_device_microbatch_size
         self._dataloader_len = None
         self._dataloader = None
         self._dataloader_label = None
         self.set_dataloader(dataloader, dataloader_label, dataloader_len)
         self.dataset_state = dataset_state
         self.dataset_resumption = dataset_resumption or {}
         self._max_duration = None
         self.max_duration = max_duration
 
         self._train_dataloader = train_dataloader
         self._evaluators = list(ensure_tuple(evaluators))
 
+        self.previous_timestamp: Optional[Timestamp] = None
         self.timestamp = Timestamp()
         self.eval_timestamp = Timestamp()
         self.predict_timestamp = Timestamp()
         self._precision = Precision(precision)
 
         if optimizers is None:
             self._optimizers = []
@@ -539,21 +557,14 @@
             dataset = self._dataset_of(self._train_dataloader)
             if hasattr(dataset, 'load_state_dict'):
                 dataset.load_state_dict(self.dataset_state['train'])  # pyright: ignore
                 self.dataset_resumption['train'] = True
             self.dataset_state['train'] = None
 
     @property
-    def current_metrics(self):
-        warnings.warn(
-            'The ``current_metrics`` argument for a :class:`Trainer`. state is deprecated and will be removed in the future. Please use ``train_metrics`` and'
-            '``eval_metrics`` instead.')
-        return {'train': self.train_metrics, **self.eval_metrics}
-
-    @property
     def seed(self):
         """The seed for the current rank."""
         return self.rank_zero_seed + dist.get_global_rank()
 
     @property
     def max_duration(self):
         """The maximum training duration."""
@@ -794,14 +805,35 @@
                     optim_state_dict = {type(optimizer).__qualname__: optimizer.state_dict()}
                 serialized_value = optim_state_dict
             elif attribute_name == 'algorithms':
                 # Store as list to preserve order in which algorithms were applied
                 serialized_value = [(type(obj).__qualname__, obj.state_dict()) for obj in ensure_tuple(attribute_value)]
             elif attribute_name in _STATE_DICT_SERIALIZED_ATTRIBUTES:
                 serialized_value = {type(obj).__qualname__: obj.state_dict() for obj in ensure_tuple(attribute_value)}
+            elif attribute_name == 'train_metrics':
+                serialized_value = {}
+                for k, v in attribute_value.items():
+                    # No need to use __qualname__, we already know this corresponds to
+                    # a metric object when we deserialize.
+                    # Along with the rest of a Composer checkpoint, the state_dict() and _computed attributes of
+                    # a Torchmetrics object are enough information to recreate it upon serialization. We only serialize
+                    # the minimum metric information to maximize backwards compatibility --- old checkpoints
+                    # will continue to be compatible even if other Torchmetrics attributes have changed.
+                    # metric._computed stores the cached value of the previous metric computation
+                    # We need to serialize this because it cannot always be recomputed from the state dict.
+                    # See https://torchmetrics.readthedocs.io/en/stable/pages/implement.html#torchmetrics.Metric for more details
+                    v.persistent(mode=True)
+                    serialized_value[k] = {'state_dict': v.state_dict(), '_computed': v._computed}
+            elif attribute_name == 'eval_metrics':
+                serialized_value = {}
+                for eval_key, eval_metrics in attribute_value.items():
+                    serialized_value[eval_key] = {}
+                    for k, v in eval_metrics.items():
+                        v.persistent(mode=True)
+                        serialized_value[eval_key][k] = {'state_dict': v.state_dict(), '_computed': v._computed}
             else:
                 serialized_value = attribute_value
 
             state_dict[attribute_name] = serialized_value
 
         state_dict['integrations'] = self._get_integrations_state_dict()
         state_dict['metadata'] = self._get_state_metadata()
@@ -947,14 +979,21 @@
             with fsdp_state_dict_type_context(self.model, state_dict_type=self.fsdp_state_dict_type):
                 missing_keys, unexpected_keys = self.model.load_state_dict(state_dict['model'], strict=strict)
         else:
             missing_keys, unexpected_keys = self.model.load_state_dict(state_dict['model'], strict=strict)
         if len(missing_keys) > 0:
             log.warning(f"Found these missing keys in the checkpoint: {', '.join(missing_keys)}")
         if len(unexpected_keys) > 0:
+            if self.fsdp_config is not None and self.fsdp_config.get(
+                    'use_orig_params') and self.fsdp_state_dict_type == 'local':
+                log.warning(
+                    'You are using use_orig_params=True and fsdp_state_dict_type=local. '
+                    'This results in both the original parameters and the flat parameters being '
+                    'in the state dict. If you see a warning with unexpected keys ending in ._flat_param, the model'
+                    'was still loaded correctly.')
             log.warning(f"Found these unexpected keys in the checkpoint: {', '.join(unexpected_keys)}")
 
     def load_optim_state(self, state_dict: Dict[str, Any]):
         """Load the optimizer state.
 
         Args:
             state_dict (Dict[str, Any]): The state to load.
@@ -964,37 +1003,29 @@
             if type(optimizer).__qualname__ not in serialized_value:
                 warnings.warn(
                     f'{type(optimizer).__qualname__} is not in the state_dict. Its state will not be restored.',
                     category=UserWarning)
                 continue
             optim_state_dict = serialized_value[type(optimizer).__qualname__]
             if self.fsdp_enabled:
+                assert self.fsdp_state_dict_type is not None  # pyright
+                if version.parse(torch.__version__) < version.parse('1.13.0'):
+                    raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
+                from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
                 log.debug(f'Loading FSDP optimizer with fsdp_state_dict_type={self.fsdp_state_dict_type}')
-                if self.fsdp_state_dict_type == 'sharded':
-                    if version.parse(torch.__version__) < version.parse('1.13.0'):
-                        raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
-                    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-
-                    # Optimizer and optimizer state dict are already sharded, but not
-                    # flattened, so we flatten the state dict then load it.
-                    flattened_optim_state_dict = FSDP.flatten_sharded_optim_state_dict(
-                        sharded_optim_state_dict=optim_state_dict, model=self.model, optim=optimizer)
-                    optimizer.load_state_dict(flattened_optim_state_dict)
-                elif self.fsdp_state_dict_type == 'local':
-                    # Optimizer and optimizer state dict are already sharded and flattened,
-                    # so just load the state_dict.
-                    optimizer.load_state_dict(optim_state_dict)
-                else:  # fsdp_state_dict_type == 'full'
-                    # FSDP enabled, but fsdp_state_dict is set to 'full', so the state dict
-                    # is a full state dict and we must shard and flatten it first before loading it.
-                    sharded_optim_state_dict = get_fsdp_sharded_optim_state_dict(full_optim_state_dict=optim_state_dict,
-                                                                                 model=self.model)
-                    log.debug(f'optimizer.load_state_dict call with fsdp_state_dict_type=full')
-                    optimizer.load_state_dict(sharded_optim_state_dict)
-            # No FSDP, so just load the optim state dict.
+                if not using_torch_2():
+                    optim_state_dict = _legacy_optim_state_dict_to_load(optim_state_dict=optim_state_dict,
+                                                                        model=self.model,
+                                                                        optim=optimizer,
+                                                                        state_dict_type=self.fsdp_state_dict_type)
+                else:
+                    with fsdp_state_dict_type_context(module=self.model, state_dict_type=self.fsdp_state_dict_type):
+                        optim_state_dict = FSDP.optim_state_dict_to_load(  #  type: ignore
+                            optim_state_dict=optim_state_dict, model=self.model, optim=optimizer)
+                optimizer.load_state_dict(optim_state_dict)
             else:
                 log.debug(f'Loading optimizer state dict')
                 optimizer.load_state_dict(optim_state_dict)
 
     def _load_dataset_state(self, obj: Dict[str, Any]) -> None:
         """Load the dataset state.
 
@@ -1072,24 +1103,91 @@
                 serialized_value = {algo_name: algo_serialized for algo_name, algo_serialized in serialized_value}
 
             if attribute_name == 'dataset_state':
                 self._load_dataset_state(serialized_value)
             elif attribute_name == 'optimizers':
                 self.load_optim_state(state)
             elif attribute_name == 'train_metrics':
+                # Get current metrics object and populate each metric present
+                # in serialization with serialized data via load_state_dict()
                 state_field_value = getattr(self, attribute_name)
-                for metric_name, metric in serialized_value.items():
-                    metric._device = self.device._device
-                    state_field_value[metric_name] = metric
+                for metric_name in state_field_value.keys():
+                    if metric_name not in serialized_value:
+                        continue
+                    # Increment _update_count so it is non-zero, preventing Torchmetrics from warning us when we call metric.compute()
+                    state_field_value[metric_name]._update_count += 1
+                    if isinstance(serialized_value[metric_name], Metric):
+                        # For checkpoints saved using Composer <= 0.13.5
+                        serialized_value[metric_name].persistent(mode=True)
+                        # Add new attr in torch2
+                        serialized_value[metric_name]._state_dict_pre_hooks = OrderedDict()
+                        metric_state_dict = serialized_value[metric_name].state_dict()
+                        metric_computed_field = serialized_value[metric_name]._computed
+                    elif isinstance(serialized_value[metric_name], dict):
+                        # For checkpoints saved using Composer >= 0.14
+                        metric_state_dict = serialized_value[metric_name]['state_dict']
+                        metric_computed_field = serialized_value[metric_name]['_computed']
+                    else:
+                        raise ValueError(
+                            'Error while loading train metric. Train metric from serialization is neither a Torchmetrics Metric object nor a dictionary.'
+                        )
+                    missing_keys, unexpected_keys = state_field_value[metric_name].load_state_dict(metric_state_dict,
+                                                                                                   strict=False)
+                    state_field_value[metric_name]._computed = metric_computed_field
+                    state_field_value[metric_name].persistent(mode=True)
+                    self.device.module_to_device(state_field_value[metric_name])
+                    if len(missing_keys) > 0:
+                        warnings.warn(
+                            f"While loading train metric: {metric_name}, missing these keys:  {', '.join(missing_keys)}"
+                        )
+                    if len(unexpected_keys) > 0:
+                        warnings.warn(
+                            f"While loading train metric: {metric_name}, found these unexpected keys:  {', '.join(unexpected_keys)}"
+                        )
             elif attribute_name == 'eval_metrics':
+                # Get current metrics object and populate each metric present
+                # in serialization with serialized data via load_state_dict()
                 state_field_value = getattr(self, attribute_name)
-                for eval_key, eval_metrics in serialized_value.items():
-                    for metric_name, metric in eval_metrics.items():
-                        metric._device = self.device._device
-                        state_field_value[eval_key][metric_name] = metric
+                for eval_key in state_field_value.keys():
+                    if eval_key not in serialized_value:
+                        continue
+                    for metric_name in state_field_value[eval_key].keys():
+                        if metric_name not in serialized_value[eval_key]:
+                            continue
+                        # Increment _update_count so it is non-zero, preventing Torchmetrics from warning us when we call metric.compute()
+                        state_field_value[eval_key][metric_name]._update_count += 1
+                        if isinstance(serialized_value[eval_key][metric_name], Metric):
+                            # For checkpoints saved using Composer <= 0.13.5
+                            serialized_value[eval_key][metric_name].persistent(mode=True)
+                            # Add new attr in torch2
+                            serialized_value[eval_key][metric_name]._state_dict_pre_hooks = OrderedDict()
+                            eval_metric_state_dict = serialized_value[eval_key][metric_name].state_dict()
+                            eval_metric_computed_field = serialized_value[eval_key][metric_name]._computed
+                        elif isinstance(serialized_value[eval_key][metric_name], dict):
+                            # For checkpoints saved using Composer >= 0.14
+                            eval_metric_state_dict = serialized_value[eval_key][metric_name]['state_dict']
+                            eval_metric_computed_field = serialized_value[eval_key][metric_name]['_computed']
+                        else:
+                            raise ValueError(
+                                'Error while loading evaluation metric. Evaluation metric from serialization is neither a Torchmetrics Metric object nor a dictionary.'
+                            )
+                        missing_keys, unexpected_keys = state_field_value[eval_key][metric_name].load_state_dict(
+                            eval_metric_state_dict, strict=False)
+                        state_field_value[eval_key][metric_name]._computed = eval_metric_computed_field
+                        state_field_value[eval_key][metric_name].persistent(mode=True)
+                        self.device.module_to_device(state_field_value[eval_key][metric_name])
+                        if len(missing_keys) > 0:
+                            warnings.warn(
+                                f"While loading evaluation metric: {metric_name} for eval dataloader {eval_key}, missing these keys: {', '.join(missing_keys)}"
+                            )
+                        if len(unexpected_keys) > 0:
+                            warnings.warn(
+                                f"While loading evaluation metric: {metric_name} for eval dataloader {eval_key}, found these unexpected keys: {', '.join(unexpected_keys)}"
+                            )
+
             elif attribute_name in _STATE_DICT_SERIALIZED_ATTRIBUTES:
                 state_field_value = getattr(self, attribute_name)
                 for target in ensure_tuple(state_field_value):
                     if type(target).__qualname__ not in serialized_value:
                         warnings.warn(
                             f'{type(target).__qualname__} is not in the state_dict. Its state will not be restored.',
                             category=UserWarning)
```

### Comparing `composer-0.13.5/composer/core/time.py` & `composer-0.14.0/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/core/types.py` & `composer-0.14.0/composer/core/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,20 @@
 
 __all__ = ['Batch', 'PyTorchScheduler', 'JSON', 'MemoryFormat', 'TrainerMode', 'BreakEpochException']
 
 Batch = Any
 
 Dataset = torch.utils.data.Dataset[Batch]
 
-PyTorchScheduler = torch.optim.lr_scheduler._LRScheduler
+try:
+    # This is correct for PyTorch >= 2.0
+    PyTorchScheduler = torch.optim.lr_scheduler.LRScheduler  # type: ignore
+except:
+    # This is correct for PyTorch < 2.0
+    PyTorchScheduler = torch.optim.lr_scheduler._LRScheduler
 
 JSON = Union[str, float, int, None, List['JSON'], Dict[str, 'JSON']]
 
 
 class BreakEpochException(Exception):
     """Raising this exception will immediately end the current epoch.
```

### Comparing `composer-0.13.5/composer/datasets/__init__.py` & `composer-0.14.0/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/ade20k.py` & `composer-0.14.0/composer/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/brats.py` & `composer-0.14.0/composer/datasets/brats.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/c4.py` & `composer-0.14.0/composer/datasets/c4.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/cifar.py` & `composer-0.14.0/composer/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/ffcv_utils.py` & `composer-0.14.0/composer/datasets/ffcv_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/imagenet.py` & `composer-0.14.0/composer/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/lm_dataset.py` & `composer-0.14.0/composer/datasets/lm_dataset.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/mnist.py` & `composer-0.14.0/composer/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/synthetic.py` & `composer-0.14.0/composer/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/datasets/utils.py` & `composer-0.14.0/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/devices/device.py` & `composer-0.14.0/composer/devices/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/devices/device_cpu.py` & `composer-0.14.0/composer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/devices/device_gpu.py` & `composer-0.14.0/composer/devices/device_gpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/devices/device_mps.py` & `composer-0.14.0/composer/devices/device_mps.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/devices/device_tpu.py` & `composer-0.14.0/composer/devices/device_tpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/functional/__init__.py` & `composer-0.14.0/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/__init__.py` & `composer-0.14.0/composer/loggers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 from composer.loggers.cometml_logger import CometMLLogger
 from composer.loggers.console_logger import ConsoleLogger
 from composer.loggers.file_logger import FileLogger
 from composer.loggers.in_memory_logger import InMemoryLogger
 from composer.loggers.logger import Logger
 from composer.loggers.logger_destination import LoggerDestination
 from composer.loggers.mlflow_logger import MLFlowLogger
+from composer.loggers.mosaicml_logger import MosaicMLLogger
 from composer.loggers.progress_bar_logger import ProgressBarLogger
 from composer.loggers.remote_uploader_downloader import RemoteUploaderDownloader
+from composer.loggers.slack_logger import SlackLogger
 from composer.loggers.tensorboard_logger import TensorboardLogger
 from composer.loggers.wandb_logger import WandBLogger
 
 # All needs to be defined properly for sphinx autosummary
 __all__ = [
     'Logger',
     'LoggerDestination',
@@ -33,8 +35,10 @@
     'ProgressBarLogger',
     'WandBLogger',
     'RemoteUploaderDownloader',
     'TensorboardLogger',
     'CometMLLogger',
     'ConsoleLogger',
     'MLFlowLogger',
+    'MosaicMLLogger',
+    'SlackLogger',
 ]
```

### Comparing `composer-0.13.5/composer/loggers/cometml_logger.py` & `composer-0.14.0/composer/loggers/cometml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/file_logger.py` & `composer-0.14.0/composer/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/in_memory_logger.py` & `composer-0.14.0/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/logger.py` & `composer-0.14.0/composer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/logger_destination.py` & `composer-0.14.0/composer/loggers/logger_destination.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/mlflow_logger.py` & `composer-0.14.0/composer/loggers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/progress_bar_logger.py` & `composer-0.14.0/composer/loggers/progress_bar_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/remote_uploader_downloader.py` & `composer-0.14.0/composer/loggers/remote_uploader_downloader.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/tensorboard_logger.py` & `composer-0.14.0/composer/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/loggers/wandb_logger.py` & `composer-0.14.0/composer/loggers/wandb_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         log_artifacts (bool, optional): Whether to log
             `artifacts <https://docs.wandb.ai/ref/python/artifact>`_ (Default: ``False``).
         rank_zero_only (bool, optional): Whether to log only on the rank-zero process.
             When logging `artifacts <https://docs.wandb.ai/ref/python/artifact>`_, it is
             highly recommended to log on all ranks.  Artifacts from ranks ≥1 will not be
             stored, which may discard pertinent information. For example, when using
             Deepspeed ZeRO, it would be impossible to restore from checkpoints without
-            artifacts from all ranks (default: ``False``).
+            artifacts from all ranks (default: ``True``).
         init_kwargs (Dict[str, Any], optional): Any additional init kwargs
             ``wandb.init`` (see
             `WandB documentation <https://docs.wandb.ai/ref/python/init>`_).
     """
 
     def __init__(
         self,
```

### Comparing `composer-0.13.5/composer/loss/loss.py` & `composer-0.14.0/composer/loss/loss.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 __all__ = ['binary_cross_entropy_with_logits', 'loss_registry', 'soft_cross_entropy']
 
 
 def binary_cross_entropy_with_logits(
     input: Tensor,
     target: Tensor,
     weight: Optional[Tensor] = None,
-    size_average: Optional[bool] = None,
-    reduce: Optional[bool] = None,
     reduction: str = 'sum',
     pos_weight: Optional[Tensor] = None,
     scale_by_batch_size: Optional[bool] = True,
 ) -> torch.Tensor:
     r"""Replacement for :class:`~F.binary_cross_entropy_with_logits` that handles class indices or one-hot labels.
 
     :class:`~torch.nn.functional.binary_cross_entropy_with_logits` with ``reduction =
@@ -43,48 +41,39 @@
             (often referred to as logits).
         target (torch.Tensor) : If containing class indices, shape :math:`(N)` where each value is
             :math:`0 \leq \text{targets}[i] \leq C-1`, or :math:`(N, d_1, d_2, ..., d_K)` with
             :math:`K \geq 1` in the case of K-dimensional loss. If containing class probabilities,
             same shape as the input.
         weight (torch.Tensor, optional): a manual rescaling weight given to each
             class. If given, has to be a Tensor of size `C`. Default: ``None``.
-        size_average (bool, optional): Deprecated (see `reduction`). By default,
-            the losses are averaged over each loss element in the batch. Note that for
-            some losses, there multiple elements per sample. If the field ``size_average``
-            is set to ``False``, the losses are instead summed for each minibatch. Ignored
-            when reduce is ``False``. Default: ``True``
-        reduce (bool, optional): Deprecated (see ``reduction``). By default, the
-            losses are averaged or summed over observations for each minibatch depending
-            on `size_average`. When ``reduce`` is ``False``, returns a loss per
-            batch element instead and ignores `size_average`. Default: ``True``
         reduction (str, optional): Specifies the reduction to apply to the output:
             ``'none'`` | ``'mean'`` | ``'sum'``. ``'none'``: no reduction will be applied,
             ``'mean'``: the sum of the output will be divided by the number of
-            elements in the output, ``'sum'``: the output will be summed. Note: ``size_average``
-            and ``reduce`` are in the process of being deprecated, and in the meantime,
-            specifying either of those two args will override ``reduction``. Default:
+            elements in the output, ``'sum'``: the output will be summed. Default:
             ``'sum'``
         pos_weight (Tensor, optional): a weight of positive examples.
                 Must be a vector with length equal to the number of classes.
         scale_by_batch_size (bool, optional): Whether to scale the loss by the batch size
             (i.e. input.shape[0]). Default: ``True``.
     """
     target = ensure_targets_one_hot(input, target)
-    bce = F.binary_cross_entropy_with_logits(input, target, weight, size_average, reduce, reduction, pos_weight)
+    bce = F.binary_cross_entropy_with_logits(input=input,
+                                             target=target,
+                                             weight=weight,
+                                             reduction=reduction,
+                                             pos_weight=pos_weight)
     if scale_by_batch_size:
         bce /= torch.tensor(input.shape[0])
     return bce
 
 
 def soft_cross_entropy(input: Tensor,
                        target: Tensor,
                        weight: Optional[Tensor] = None,
-                       size_average: Optional[bool] = None,
                        ignore_index: int = -100,
-                       reduce: Optional[bool] = None,
                        reduction: str = 'mean'):
     r"""Drop-in replacement for :class:`~.F.cross_entropy` that handles class indices or one-hot labels.
 
     .. note::
 
         This function will be obsolete with `this update <https://github.com/pytorch/pytorch/pull/61044>`_.
 
@@ -95,43 +84,35 @@
             (often referred to as logits).
         target (torch.Tensor) : If containing class indices, shape :math:`(N)` where each value is
             :math:`0 \leq \text{targets}[i] \leq C-1`, or :math:`(N, d_1, d_2, ..., d_K)` with
             :math:`K \geq 1` in the case of K-dimensional loss. If containing class probabilities,
             same shape as the input.
         weight (torch.Tensor, optional): a manual rescaling weight given to each
             class. If given, has to be a Tensor of size `C`. Default: ``None``.
-        size_average (bool, optional): Deprecated (see `reduction`). By default,
-            the losses are averaged over each loss element in the batch. Note that for
-            some losses, there multiple elements per sample. If the field ``size_average``
-            is set to ``False``, the losses are instead summed for each minibatch. Ignored
-            when reduce is ``False``. Default: ``True``
         ignore_index (int, optional): Specifies a target value that is ignored
             and does not contribute to the input gradient. When ``size_average`` is
             ``True``, the loss is averaged over non-ignored targets. Note that
             ``ignore_index`` is only applicable when the target contains class indices.
             Default: ``-100``
-        reduce (bool, optional): Deprecated (see ``reduction``). By default, the
-            losses are averaged or summed over observations for each minibatch depending
-            on `size_average`. When ``reduce`` is ``False``, returns a loss per
-            batch element instead and ignores `size_average`. Default: ``True``
         reduction (str, optional): Specifies the reduction to apply to the output:
             ``'none'`` | ``'mean'`` | ``'sum'``. ``'none'``: no reduction will be applied,
             ``'mean'``: the sum of the output will be divided by the number of
-            elements in the output, ``'sum'``: the output will be summed. Note: ``size_average``
-            and ``reduce`` are in the process of being deprecated, and in the meantime,
-            specifying either of those two args will override ``reduction``. Default: ``'mean'``
+            elements in the output, ``'sum'``: the output will be summed. Default: ``'mean'``
     """
     target_type = infer_target_type(input, target)
 
     if target_type == 'indices':
-        return F.cross_entropy(input, target, weight, size_average, ignore_index, reduce, reduction)
+        return F.cross_entropy(input=input,
+                               target=target,
+                               weight=weight,
+                               ignore_index=ignore_index,
+                               reduction=reduction)
     elif target_type == 'one_hot':
-        assert reduction in ['sum', 'mean', 'none'], f'{reduction} reduction not supported.'
-        assert size_average is None, 'size_average is deprecated'
-        assert reduce is None, 'reduce is deprecated'
+        if reduction not in ['sum', 'mean', 'none']:
+            raise ValueError(f'{reduction} reduction not supported.')
         if ignore_index != -100:
             warnings.warn('ignore_index not supported when using dense labels. Ignoring targets with 0 probability.')
         xentropy = -(target * F.log_softmax(input, dim=1))
 
         if weight is not None:
             # Ugly dimension shuffle to make multiplication work.
             xentropy = torch.movedim(xentropy, 1, -1)
```

### Comparing `composer-0.13.5/composer/loss/utils.py` & `composer-0.14.0/composer/loss/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/metrics/__init__.py` & `composer-0.14.0/composer/metrics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A collection of common torchmetrics."""
 
 from composer.metrics.map import MAP
 from composer.metrics.metrics import CrossEntropy, Dice, LossMetric, MIoU
-from composer.metrics.nlp import (BinaryF1Score, HFCrossEntropy, InContextLearningLMAccuracy, InContextLearningMetric,
-                                  InContextLearningMultipleChoiceAccuracy, LanguageCrossEntropy, LanguagePerplexity,
-                                  MaskedAccuracy, Perplexity)
+from composer.metrics.nlp import (BinaryF1Score, HFCrossEntropy, InContextLearningLMAccuracy,
+                                  InContextLearningLMExpectedCalibrationError,
+                                  InContextLearningMCExpectedCalibrationError, InContextLearningMetric,
+                                  InContextLearningMultipleChoiceAccuracy, InContextLearningQAAccuracy,
+                                  LanguageCrossEntropy, LanguagePerplexity, MaskedAccuracy, Perplexity)
 
 __all__ = [
     'MAP',
     'MIoU',
     'Dice',
     'CrossEntropy',
     'LossMetric',
@@ -19,14 +21,18 @@
     'BinaryF1Score',
     'HFCrossEntropy',
     'LanguageCrossEntropy',
     'MaskedAccuracy',
     'LanguagePerplexity',
     'InContextLearningLMAccuracy',
     'InContextLearningMultipleChoiceAccuracy',
+    'InContextLearningQAAccuracy',
+    'InContextLearningMCExpectedCalibrationError',
+    'InContextLearningLMExpectedCalibrationError',
     'InContextLearningMetric',
 ]
 
 METRIC_DEFAULT_CTORS = {
     'InContextLearningLMAccuracy': InContextLearningLMAccuracy,
-    'InContextLearningMultipleChoiceAccuracy': InContextLearningMultipleChoiceAccuracy
+    'InContextLearningMultipleChoiceAccuracy': InContextLearningMultipleChoiceAccuracy,
+    'InContextLearningQAAccuracy': InContextLearningQAAccuracy
 }
```

### Comparing `composer-0.13.5/composer/metrics/map.py` & `composer-0.14.0/composer/metrics/map.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/metrics/metrics.py` & `composer-0.14.0/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/__init__.py` & `composer-0.14.0/composer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/base.py` & `composer-0.14.0/composer/models/base.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/bert/model.py` & `composer-0.14.0/composer/models/bert/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/classify_mnist/model.py` & `composer-0.14.0/composer/models/classify_mnist/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/deeplabv3/model.py` & `composer-0.14.0/composer/models/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/efficientnetb0/__init__.py` & `composer-0.14.0/composer/models/efficientnetb0/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/efficientnetb0/_layers.py` & `composer-0.14.0/composer/models/efficientnetb0/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/efficientnetb0/efficientnets.py` & `composer-0.14.0/composer/models/efficientnetb0/efficientnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/efficientnetb0/model.py` & `composer-0.14.0/composer/models/efficientnetb0/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/gpt2/__init__.py` & `composer-0.14.0/composer/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/gpt2/model.py` & `composer-0.14.0/composer/models/gpt2/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/huggingface.py` & `composer-0.14.0/composer/models/huggingface.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 from __future__ import annotations
 
 import inspect
 import json
 import logging
 import tempfile
 import textwrap
-import warnings
-from collections import UserDict
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple, Type, Union
 
 import torch
 from torchmetrics import Metric
 
-from composer.metrics import METRIC_DEFAULT_CTORS, InContextLearningMetric
+from composer.metrics import InContextLearningMetric
 from composer.models.base import ComposerModel
-from composer.utils import MissingConditionalImportError, get_file, import_object, safe_torch_load
+from composer.utils import MissingConditionalImportError, dist, get_file, import_object, is_model_fsdp, safe_torch_load
 
 if TYPE_CHECKING:
     import transformers
     from transformers import PretrainedConfig
     from transformers.models.auto.auto_factory import _BaseAutoModelClass
 
 log = logging.getLogger(__name__)
@@ -106,41 +104,45 @@
                     f' You can resize the model embeddings to {len(tokenizer)} from {self.config.vocab_size}'
                     f' by calling `model.resize_token_embeddings(len(tokenizer))` before calling the `HuggingFaceModel`'
                     f' constructor, or pass `allow_embedding_resizing=True` to have it done automatically.')
         elif tokenizer is not None and self.config.vocab_size > len(tokenizer):
             # when the embedding size is greater than the tokenizer vocab size,
             # the embeddings do not _need_ to be resized to match the tokenizer vocab size,
             # and should be done by the user if desired
-            log.warning(
+            log.info(
                 f'The number of tokens in the tokenizer is less than the number of tokens in the model.'
                 f' You may want to resize the model embeddings to {len(tokenizer)} from {self.config.vocab_size}'
                 f' by calling `model.resize_token_embeddings(len(tokenizer))` before calling the `HuggingFaceModel`'
-                f' constructor.')
+                f' constructor. The vocab size is sometimes intentionally set to a multiple of 32 or 64 to improve'
+                f' performance.')
 
         self.use_logits = use_logits
 
         self.train_metrics: Optional[Dict] = None
         self.val_metrics: Optional[Dict] = None
 
+        if eval_metrics is not None:
+            self.val_metrics = {metric.__class__.__name__: metric for metric in eval_metrics}
         if metrics is not None:
             self.train_metrics = {metric.__class__.__name__: metric for metric in metrics}
+            # if eval_metrics is None, use the same metrics as train_metrics
             if eval_metrics is None:
                 self.val_metrics = {metric.__class__.__name__: metric for metric in metrics}
-            else:
-                self.val_metrics = {metric.__class__.__name__: metric for metric in eval_metrics}
 
         self.labels: Optional[torch.Tensor] = None  # set in eval_forward() if exists
 
         is_causal_lm = _is_registered_causal_lm(model)
         self.shift_labels = is_causal_lm if shift_labels is None else shift_labels
         if is_causal_lm and not self.shift_labels:
             log.warning('The shift_labels argument was set to False but the model is an instance of a'
                         ' HuggingFace Causal LM. This may lead to incorrect behavior.')
             # Note: No warning if shift_labels and not is_causal_lm, since the model may simply be a custom class.
 
+        self.dummy_forward_called = False
+
     @staticmethod
     def hf_from_composer_checkpoint(
         checkpoint_path: str,
         model_instantiation_class: Optional[Union[Type[transformers.PreTrainedModel], Type['_BaseAutoModelClass'],
                                                   str]] = None,
         model_config_kwargs: Optional[dict] = None,
         local_checkpoint_save_location: Optional[Union[Path, str]] = None
@@ -292,26 +294,25 @@
                         s = spm.SentencePieceProcessor()
                         s.load_from_serialized_proto(saved_content['content'])
                         with open(tokenizer_file_path, 'wb') as _tmp_file:
                             _tmp_file.write(s.serialized_model_proto())
                 hf_tokenizer = transformers.AutoTokenizer.from_pretrained(_tmp_dir)
 
                 # we need to set the name_or_path back because otherwise it is the tmp dir we are loading from here
-                hf_tokenizer.name_or_path = hf_tokenizer_state['tokenizer_config']['content']['name_or_path']
-                hf_tokenizer.init_kwargs['name_or_path'] = hf_tokenizer_state['tokenizer_config']['content'][
-                    'name_or_path']
+                hf_tokenizer.name_or_path = hf_tokenizer_state['tokenizer_config']['content'].get('name_or_path', '')
+                hf_tokenizer.init_kwargs['name_or_path'] = hf_tokenizer.name_or_path
 
                 # for an unknown reason this key is missing when loading the saved tokenizer, but present with a value of None
                 # for the original tokenizer, so we default it to None
                 hf_tokenizer.init_kwargs['tokenizer_file'] = hf_tokenizer.init_kwargs.get('tokenizer_file', None)
 
         return hf_model, hf_tokenizer
 
     def forward(self, batch):
-        if isinstance(batch, dict) or isinstance(batch, UserDict):
+        if isinstance(batch, Mapping):
             # Further input validation is left to the huggingface forward call
             batch = {k: v for k, v in batch.items() if k in self.model_forward_args}
             output = self.model(**batch)  # type: ignore (thirdparty)
         else:
             raise ValueError(
                 'Unexpected batch type. Expected a dictionary with keys corresponding to the inputs to the forward function of the Huggingface model'
             )
@@ -321,14 +322,30 @@
         if self.config.use_return_dict:
             return outputs['loss']
         else:
             # loss is at index 0 in the output tuple
             return outputs[0]
 
     def eval_forward(self, batch, outputs: Optional[Any] = None):
+        # If the batch mode is generate, we will generate a requested number of tokens using the underlying
+        # model's generate function. Extra generation kwargs can be passed in via the batch. Strings will
+        # be returned from eval_forward
+        if batch.get('mode', None) == 'generate':
+            if self.tokenizer is None:
+                raise ValueError(
+                    'Generation eval cannot be used without providing a tokenizer to the model constructor.')
+
+            self.labels = batch.pop('labels')
+            generation = self.generate(batch['input_ids'],
+                                       attention_mask=batch['attention_mask'],
+                                       max_new_tokens=batch['generation_length'],
+                                       synced_gpus=dist.get_world_size() > 1,
+                                       **batch.get('generation_kwargs', {}))
+            return self.tokenizer.batch_decode(generation[:, batch['input_ids'].shape[1]:], skip_special_tokens=True)
+
         if self.use_logits or batch.get('mode', None) == 'icl_task':
             # pop labels first to avoid computing loss
             self.labels = batch.pop('labels')
 
             # HF encoder decoder models like T5 expect either decoder_input_ids or labels,
             # so we add decoder_input_ids to the batch if it is missing
             if self.model.config.is_encoder_decoder and 'decoder_input_ids' not in batch:
@@ -420,23 +437,57 @@
                             f'Unexpected file ending {tokenizer_file_name} in output of tokenizer.save_pretrained.')
                     tokenizer_output[tokenizer_file_path.stem] = {
                         'file_extension': tokenizer_file_extension,
                         'content': tokenizer_file_content
                     }
         return {'model': model_output, 'tokenizer': tokenizer_output}
 
-    def add_eval_metrics(self, evaluator):
-        warnings.warn(
-            DeprecationWarning('The add_eval_metrics method is deprecated and will be removed in a future release. '
-                               'Please pass in `eval_metrics` directly to the constructor.'))
-        evaluator_metrics = {m: METRIC_DEFAULT_CTORS[m]() for m in evaluator.metric_names}
-        if self.val_metrics is not None:
-            self.val_metrics.update(evaluator_metrics)
+    def generate(self, input_ids: torch.Tensor, **kwargs):
+        """Generate from the underlying HuggingFace model.
+
+        Except for ``pad_token_id``, which is optionally read from ``self.tokenizer``, all args are passed along
+        to :meth:`transformers.GenerationMixin.generate` function.
+
+        Args:
+            input_ids (torch.Tensor): Input ids to generate from.
+            **kwargs: Additional arguments passed to :meth:`transformers.GenerationMixin.generate` function.
+                See :class:`transformers.GenerationConfig` for all available arguments.
+        """
+        pad_token_id = kwargs.pop('pad_token_id', self.tokenizer.pad_token_id if self.tokenizer is not None else None)
+
+        from composer.utils.misc import using_torch_2
+
+        # We need to call forward once in order for FSDP + generate to work
+        # This solution works because parameters in the root FSDP module are not freed after forward
+        # See https://github.com/huggingface/accelerate/issues/570, https://github.com/huggingface/accelerate/issues/947,
+        # and https://github.com/pytorch/pytorch/issues/82461, https://github.com/pytorch/pytorch/issues/100069 for more info
+        # Note: This is a solution for Torch 1.13.x, and there is a different solution below for Torch 2.0
+        if not using_torch_2() and not self.dummy_forward_called and is_model_fsdp(self.model):
+            with torch.no_grad():
+                maybe_decoder_input_ids = {}
+                if self.model.config.is_encoder_decoder:
+                    maybe_decoder_input_ids['decoder_input_ids'] = torch.tensor([[0]],
+                                                                                dtype=torch.long,
+                                                                                device=input_ids.device)
+                self.model(input_ids=torch.tensor([[0]], dtype=torch.long, device=input_ids.device),
+                           **maybe_decoder_input_ids)
+            self.dummy_forward_called = True
+
+        if is_model_fsdp(self.model) and using_torch_2():
+            from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+
+            # Note: We need to use the FSDP.summon_full_params context manager here because the generate function
+            # does not seem to gather the weights for the LM head. This solution works because the tied weights of the LM head
+            # are in the root FSDP module, and are summoned by the below context manager. See https://github.com/pytorch/pytorch/issues/100069
+            # for more info.
+            # Note: We use recurse=False here so that we only summon full params for the LM head, not the entire model.
+            with FSDP.summon_full_params(self.model, writeback=False, recurse=False):
+                return self.model.generate(input_ids, pad_token_id=pad_token_id, **kwargs)
         else:
-            self.val_metrics = evaluator_metrics
+            return self.model.generate(input_ids, pad_token_id=pad_token_id, **kwargs)
 
 
 def _is_registered_causal_lm(model: transformers.PreTrainedModel) -> bool:
     """Return True if model class is either a registered 🤗 Causal LM or a subclass of one"""
     try:
         from transformers.models.auto.modeling_auto import MODEL_FOR_CAUSAL_LM_MAPPING
     except ImportError as e:
@@ -471,15 +522,24 @@
     hf_config_dict = state_dict['state']['integrations']['huggingface']['model']['config']['content']
     # Update the config with any extra args needed
     hf_config_dict.update(config_overrides)
     # JSON keys need to be converted back to ints, huggingface does not auto convert them along this code path
     if 'id2label' in hf_config_dict:
         hf_config_dict['id2label'] = {int(k): v for k, v in hf_config_dict['id2label'].items()}
 
-    return transformers.AutoConfig.from_pretrained(hf_config_dict['_name_or_path'], **hf_config_dict)
+    try:
+        return transformers.AutoConfig.for_model(**hf_config_dict)
+    except ValueError:
+        try:
+            return transformers.AutoConfig.from_pretrained(hf_config_dict['_name_or_path'], **hf_config_dict)
+        except KeyError:
+            raise Exception(
+                f'Could not load config from state dict using either `for_model` or `from_pretrained`.'
+                f'Please make sure that the model_type={hf_config_dict.get("model_type")} is valid, or that the'
+                f'config has a valid `_name_or_path`.')
 
 
 def write_huggingface_pretrained_from_composer_checkpoint(
         checkpoint_path: Union[Path, str],
         output_folder: Union[Path, str],
         local_checkpoint_save_location: Optional[Union[Path, str]] = None) -> None:
     """Write a ``config.json`` and ``pytorch_model.bin``, like :meth:`transformers.PreTrainedModel.from_pretrained` expects, from a composer checkpoint
```

### Comparing `composer-0.13.5/composer/models/initializers.py` & `composer-0.14.0/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/mmdetection.py` & `composer-0.14.0/composer/models/mmdetection.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/resnet/__init__.py` & `composer-0.14.0/composer/models/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/resnet/model.py` & `composer-0.14.0/composer/models/resnet/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A :class:`.ComposerClassifier` wrapper around the torchvision implementations of the ResNet model family."""
 
 import logging
+import textwrap
 import warnings
 from typing import List, Optional
 
 import torchvision
 from packaging import version
 from torchmetrics import MetricCollection
 from torchmetrics.classification import MulticlassAccuracy
@@ -88,26 +89,27 @@
         raise ValueError(
             'composer_resnet expects only one of ``pretrained`` or ``weights`` to be specified, but both were specified.'
         )
     if pretrained:
         weights = 'IMAGENET1K_V2'
         warnings.warn(
             DeprecationWarning(
-                'The ``pretrained`` argument for composer_resnet is deprecated and will be removed in the future. Please use ``weights`` instead.'
+                'The ``pretrained`` argument for composer_resnet is deprecated and will be removed in the future when torch 1.11 is no longer supported. Please use ``weights`` instead.'
             ))
 
     # Instantiate model
     model_fn = getattr(resnet, model_name)
     model = None
     if version.parse(torchvision.__version__) < version.parse('0.13.0'):
         if weights:
             pretrained = True
             warnings.warn(
-                f'The current torchvision version {torchvision.__version__} does not support the ``weights`` argument, so ``pretrained=True`` will be used instead. To enable ``weights``, please ugprade to the latest version of torchvision.'
-            )
+                textwrap.dedent(f'The current torchvision version {torchvision.__version__} does not support the '
+                                '``weights`` argument, so ``pretrained=True`` will be used instead. To enable '
+                                '``weights``, please upgrade to the latest version of torchvision.'))
         model = model_fn(pretrained=pretrained, num_classes=num_classes, groups=groups, width_per_group=width_per_group)
     else:
         model = model_fn(weights=weights, num_classes=num_classes, groups=groups, width_per_group=width_per_group)
 
     # Grab loss function from loss registry
     loss_fn = loss_registry[loss_name]
```

### Comparing `composer-0.13.5/composer/models/resnet_cifar/__init__.py` & `composer-0.14.0/composer/models/resnet_cifar/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/resnet_cifar/model.py` & `composer-0.14.0/composer/models/resnet_cifar/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/resnet_cifar/resnets.py` & `composer-0.14.0/composer/models/resnet_cifar/resnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/tasks/classification.py` & `composer-0.14.0/composer/models/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/timm/model.py` & `composer-0.14.0/composer/models/timm/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/unet/_layers.py` & `composer-0.14.0/composer/models/unet/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/unet/model.py` & `composer-0.14.0/composer/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/unet/unet.py` & `composer-0.14.0/composer/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/models/vit_small_patch16/model.py` & `composer-0.14.0/composer/models/vit_small_patch16/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/optim/__init__.py` & `composer-0.14.0/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/optim/decoupled_weight_decay.py` & `composer-0.14.0/composer/optim/decoupled_weight_decay.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,35 +347,42 @@
                        initial_lr=initial_lr,
                        weight_decay=weight_decay,
                        eps=eps)
 
         return loss
 
     def dist_reduce_metrics(self, optimizer_metrics):
-        for metric in optimizer_metrics:
+        local_keys = list(optimizer_metrics.keys())
+        all_gathered_keys = dist.all_gather_object(local_keys)
+        all_keys = set()
+        for keys in all_gathered_keys:
+            all_keys.update(keys)
+
+        all_keys = sorted(all_keys, key=lambda metric: 0 if 'l2_norm' in metric else 1)
+        for metric in all_keys:
             if metric.startswith('l2_norm'):
-                reduced = optimizer_metrics[metric]
+                reduced = optimizer_metrics.get(metric, torch.tensor(0.0, device=torch.cuda.current_device()))
                 if dist.get_world_size() > 1:
                     dist.all_reduce(reduced, reduce_operation='SUM')
 
                 optimizer_metrics[metric] = math.sqrt(reduced)
             elif metric.startswith('cosine'):
-                reduced = optimizer_metrics[metric]
+                reduced = optimizer_metrics.get(metric, torch.tensor(0.0, device=torch.cuda.current_device()))
                 if dist.get_world_size() > 1:
                     dist.all_reduce(reduced, reduce_operation='SUM')
 
                 _, vectors, layer = tuple(metric.split('/'))
 
                 A, B = tuple(vectors.split('_'))
 
                 A_reduced_norm = optimizer_metrics[f'l2_norm/{A}/{layer}']
                 B_reduced_norm = optimizer_metrics[f'l2_norm/{B}/{layer}']
                 optimizer_metrics[metric] = reduced / (A_reduced_norm * B_reduced_norm)
             else:
-                reduced = optimizer_metrics[metric]
+                reduced = optimizer_metrics.get(metric, torch.tensor(0.0, device=torch.cuda.current_device()))
                 if dist.get_world_size() > 1:
                     dist.all_reduce(reduced, reduce_operation='SUM')
                 optimizer_metrics[metric] = reduced / dist.get_world_size()
 
         return optimizer_metrics
 
     def pre_reduce_metrics(self, optimizer_metrics):
```

### Comparing `composer-0.13.5/composer/optim/scheduler.py` & `composer-0.14.0/composer/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/__init__.py` & `composer-0.14.0/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/json_trace_handler.py` & `composer-0.14.0/composer/profiler/json_trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/json_trace_merger.py` & `composer-0.14.0/composer/profiler/json_trace_merger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/marker.py` & `composer-0.14.0/composer/profiler/marker.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/profiler.py` & `composer-0.14.0/composer/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/profiler_action.py` & `composer-0.14.0/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/profiler_schedule.py` & `composer-0.14.0/composer/profiler/profiler_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/system_profiler.py` & `composer-0.14.0/composer/profiler/system_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/torch_profiler.py` & `composer-0.14.0/composer/profiler/torch_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/profiler/trace_handler.py` & `composer-0.14.0/composer/profiler/trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/trainer/_deepspeed.py` & `composer-0.14.0/composer/trainer/_deepspeed.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,87 +22,45 @@
             'When using DeepSpeed, the `train_dataloader` must be specified when constructing the Trainer.')
 
     try:
         batch_size = state.dataloader.batch_size  # type: ignore as we catch the exception
     except AttributeError as e:
         raise RuntimeError('DeepSpeed requires the `state.dataloader` to have a `batch_size` attribute.') from e
 
-    if state.using_device_microbatch_size:
-        assert state.device_train_microbatch_size is not None
-        if batch_size % state.device_train_microbatch_size != 0:
-            # DeepSpeed will throw an error in this configuration.
-            raise ValueError('The Mosaic trainer has been configured to use batch size='
-                             f'{batch_size}, but this is not divisible by the '
-                             f'train device microbatch size={state.device_train_microbatch_size}. '
-                             'This is unsupported when using DeepSpeed.')
-
-        train_batch_size = batch_size * dist.get_world_size()
-        # Per the check at the start of this function, the following division is always clean.
-        grad_accum = batch_size // state.device_train_microbatch_size
-
-        if 'train_batch_size' in config:
-            ds_train_batch_size = config['train_batch_size']
-            if ds_train_batch_size != train_batch_size:
-                raise ValueError(f'Provided DeepSpeed configuration specifies batch size={ds_train_batch_size}, '
-                                 f'but the Mosaic trainer has been configured with batch size={train_batch_size}.')
-        else:
-            config['train_batch_size'] = train_batch_size
-
-        if 'gradient_accumulation_steps' in config:
-            ds_grad_accum = config['gradient_accumulation_steps']
-            if ds_grad_accum != state.grad_accum:
-                raise ValueError((f'Provided DeepSpeed configuration specifies grad accum={ds_grad_accum}, '
-                                  f'but the Mosaic trainer has been configured with grad accum={grad_accum}.'))
-        else:
-            config['gradient_accumulation_steps'] = state.grad_accum
-
-        if 'train_micro_batch_size_per_gpu' in config:
-            ds_per_gpu_microbatch_size = config['train_micro_batch_size_per_gpu']
-            if ds_per_gpu_microbatch_size != state.device_train_microbatch_size:
-                raise ValueError('Provided DeepSpeed configuration specifies per-GPU microbatch size='
-                                 f'{ds_per_gpu_microbatch_size}, but the Mosaic trainer has been '
-                                 f'configured with per-GPU microbatch size={state.device_train_microbatch_size}.')
-        else:
-            config['train_micro_batch_size_per_gpu'] = state.device_train_microbatch_size
+    assert state.device_train_microbatch_size is not None
+    if batch_size % state.device_train_microbatch_size != 0:
+        # DeepSpeed will throw an error in this configuration.
+        raise ValueError('The Mosaic trainer has been configured to use batch size='
+                         f'{batch_size}, but this is not divisible by the '
+                         f'train device microbatch size={state.device_train_microbatch_size}. '
+                         'This is unsupported when using DeepSpeed.')
+
+    train_batch_size = batch_size * dist.get_world_size()
+    # Per the check at the start of this function, the following division is always clean.
+    grad_accum = batch_size // state.device_train_microbatch_size
+
+    if 'train_batch_size' in config:
+        ds_train_batch_size = config['train_batch_size']
+        if ds_train_batch_size != train_batch_size:
+            raise ValueError(f'Provided DeepSpeed configuration specifies batch size={ds_train_batch_size}, '
+                             f'but the Mosaic trainer has been configured with batch size={train_batch_size}.')
     else:
-        assert state.grad_accum is not None
-        if batch_size % state.grad_accum != 0:
-            # DeepSpeed will throw an error in this configuration.
-            raise ValueError('The Mosaic trainer has been configured to use batch size='
-                             f'{batch_size}, but this is not divisible by the '
-                             f'grad accum={state.grad_accum}. This is unsupported when using DeepSpeed.')
-
-        train_batch_size = batch_size * dist.get_world_size()
-        # Per the check at the start of this function, the following division is always clean.
-        per_gpu_microbatch_size = batch_size // state.grad_accum
-
-        if 'train_batch_size' in config:
-            ds_train_batch_size = config['train_batch_size']
-            if ds_train_batch_size != train_batch_size:
-                raise ValueError(f'Provided DeepSpeed configuration specifies batch size={ds_train_batch_size}, '
-                                 f'but the Mosaic trainer has been configured with batch size={train_batch_size}.')
-        else:
-            config['train_batch_size'] = train_batch_size
-
-        if 'train_micro_batch_size_per_gpu' in config:
-            ds_per_gpu_microbatch_size = config['train_micro_batch_size_per_gpu']
-            if ds_per_gpu_microbatch_size != per_gpu_microbatch_size:
-                raise ValueError('Provided DeepSpeed configuration specifies per-GPU microbatch size='
-                                 f'{ds_per_gpu_microbatch_size}, but the Mosaic trainer has been '
-                                 f'configured with per-GPU microbatch size={per_gpu_microbatch_size}.')
-        else:
-            config['train_micro_batch_size_per_gpu'] = per_gpu_microbatch_size
-
-        if 'gradient_accumulation_steps' in config:
-            ds_grad_accum = config['gradient_accumulation_steps']
-            if ds_grad_accum != state.grad_accum:
-                raise ValueError((f'Provided DeepSpeed configuration specifies grad accum={ds_grad_accum}, '
-                                  f'but the Mosaic trainer has been configured with grad accum={state.grad_accum}.'))
-        else:
-            config['gradient_accumulation_steps'] = state.grad_accum
+        config['train_batch_size'] = train_batch_size
+
+    if 'gradient_accumulation_steps' not in config:
+        config['gradient_accumulation_steps'] = grad_accum
+
+    if 'train_micro_batch_size_per_gpu' in config:
+        ds_per_gpu_microbatch_size = config['train_micro_batch_size_per_gpu']
+        if ds_per_gpu_microbatch_size != state.device_train_microbatch_size:
+            raise ValueError('Provided DeepSpeed configuration specifies per-GPU microbatch size='
+                             f'{ds_per_gpu_microbatch_size}, but the Mosaic trainer has been '
+                             f'configured with per-GPU microbatch size={state.device_train_microbatch_size}.')
+    else:
+        config['train_micro_batch_size_per_gpu'] = state.device_train_microbatch_size
 
 
 def _ensure_no_optim_in_config(config: Dict[str, Any]):
     if 'optimizer' in config:
         raise ValueError(('The DeepSpeed configuration specifies an optimizer, but the Mosaic '
                           'trainer will override this setting.'))
```

### Comparing `composer-0.13.5/composer/trainer/_scale_schedule.py` & `composer-0.14.0/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/trainer/_scaler.py` & `composer-0.14.0/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/trainer/dist_strategy.py` & `composer-0.14.0/composer/trainer/dist_strategy.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from typing import Any, Callable, ContextManager, Dict, Optional, Sequence, Union, cast
 
 import torch
 from packaging import version
 from torch.nn.parallel import DistributedDataParallel
 from torchmetrics import Metric, MetricCollection
 
-from composer.core import Precision
-from composer.core.state import State
+from composer.core import Precision, State
+from composer.devices import Device
 from composer.trainer.meta_safe_apply import meta_safe_apply
-from composer.utils import StringEnum, dist, ensure_tuple
+from composer.utils import StringEnum, dist, ensure_tuple, using_torch_2
 
 __all__ = ['DDPSyncStrategy', 'ddp_sync_context', 'prepare_ddp_module', 'prepare_fsdp_module']
 
 log = logging.getLogger(__name__)
 
 
 class DDPSyncStrategy(StringEnum):
@@ -119,36 +119,61 @@
         raise RuntimeError('Please call dist.initialize_dist() before calling ddp.prepare_module()')
 
     raise RuntimeError('When the world size is > 1, ``torch.distributed`` must be used. However, it is '
                        'not available in your installation of PyTorch. Please install or build PyTorch '
                        'with distributed support.')
 
 
-def prepare_fsdp_module(model: torch.nn.Module, optimizers: Optional[Union[torch.optim.Optimizer,
-                                                                           Sequence[torch.optim.Optimizer]]],
-                        fsdp_config: Dict[str, Any], precision: Precision) -> None:
+def prepare_fsdp_module(
+    model: torch.nn.Module,
+    optimizers: Optional[Union[torch.optim.Optimizer, Sequence[torch.optim.Optimizer]]],
+    fsdp_config: Dict[str, Any],
+    precision: Precision,
+    device: Device,
+    auto_microbatching: bool,
+) -> None:
     """Prepare a module (assumed ComposerModel) and optimizer for use with :class:`torch.distributed.fsdp.FullyShardedDataParallel`.
 
     Args:
         model (torch.nn.Module): The model to wrap.
         optimizers (torch.optim.Optimizer | Sequence[torch.optim.Optimizer], optional): The optimizer for `model`, assumed to have a single param group := model.parameters().
         fsdp_config (Dict[str, Any]): The FSDP config.
         precision: (Precision): The precision being used by the Trainer, used to fill in defaults for FSDP `mixed_precision` settings.
+        device (Device): The device being used by the Trainer.
+        auto_microbatching (bool, optional): Whether or not auto microbatching is enabled.
     """
     if version.parse(torch.__version__) < version.parse('1.13.0'):
         raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
+    is_torch_2_0 = using_torch_2()
     from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (CheckpointImpl,
                                                                              apply_activation_checkpointing,
                                                                              checkpoint_wrapper)
     from torch.distributed.fsdp import FullyShardedDataParallel
-    from torch.distributed.fsdp.flatten_params_wrapper import FlattenParamsWrapper
+    if not is_torch_2_0:
+        from torch.distributed.fsdp.flatten_params_wrapper import FlattenParamsWrapper
 
     from composer.trainer.mosaic_fsdp import (MosaicFullyShardedDataParallel, backward_prefetch_map, get_cpu_offload,
                                               get_mixed_precision, sharding_map)
 
+    # Check if other ranks OOMed after forward/backward pass when using auto microbatching. This
+    # may happen when close to memory limit or with uneven memory usage across ranks. Since we
+    # need to do this before the model weights are gathered for the next FSDP block, we wrap every
+    # FSPD block with a hook that checks if any other rank OOMed.
+    def sync_hook(*args):
+        # Check if any other rank hit an OOM
+        found_cuda_oom_tensor = device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
+        dist.all_reduce(found_cuda_oom_tensor, reduce_operation='MAX')
+        found_cuda_oom = found_cuda_oom_tensor.item()
+        # Signal current rank is still in batch
+        all_ranks_finished_tensor = device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
+        dist.all_reduce(all_ranks_finished_tensor, reduce_operation='MIN')
+
+        if found_cuda_oom == 1:
+            raise RuntimeError('CUDA out of memory encountered on a different rank')
+
     if optimizers:
         optimizers_tuple = ensure_tuple(optimizers)
         if len(optimizers_tuple) != 1:
             raise NotImplementedError(f'Only one optimizer is supported; found {len(optimizers_tuple)} optimizers')
 
         # clearing optimizer param groups and state
         # that will be recreated at the end of prepare_fsdp_module
@@ -183,41 +208,61 @@
 
         if param_dtype == torch.float32:
             raise ValueError(
                 f'FSDP in PyTorch 1.13 does not support param_dtype `{param_dtype}` with sharding_strategy `{sharding_map_key}` '
                 f'Consider using `amp` or `bf16` for precision or setting param_dtype in mixed_precision to `None` '
                 f'with sharding strategy `{sharding_map_key}.`')
 
+    if fsdp_config.get('min_params') is not None:
+        warnings.warn(DeprecationWarning('`min_params` in FSDP config will be depricated in composer version 0.16.0.'))
+
     backward_prefetch = backward_prefetch_map[fsdp_config.get('backward_prefetch', 'BACKWARD_POST').upper()]
     min_params = int(float(fsdp_config.get('min_params', 1e9)))
     activation_checkpointing = fsdp_config.get('activation_checkpointing', False)
     activation_cpu_offload = fsdp_config.get('activation_cpu_offload', False)
     sync_module_states = fsdp_config.get('sync_module_states', False)
     forward_prefetch = fsdp_config.get('forward_prefetch', False)
     limit_all_gathers = fsdp_config.get('limit_all_gathers', False)
     ignored_modules = fsdp_config.get('ignored_modules', None)
     state_dict_type = fsdp_config.get('state_dict_type', 'full')
     activation_checkpointing_reentrant = fsdp_config.get('activation_checkpointing_reentrant', True)
 
+    kwargs = {}
+    if is_torch_2_0:
+        # Support of new parameter `use_orig_params` in PyTorch 2.0 or higher.
+        # Setting this to `True` has FSDP use `module`'s original parameters via method
+        # `nn.Module.named_parameters` instead of FSDP's internal class `FlatParameter`. However,
+        # setting it to `False` exposes FSDP's internal class `FlatParameter` via method
+        # `nn.Module.named_parameters`.
+        # Setting it to `True` is mandatory when using `torch.compile()`.
+        kwargs['use_orig_params'] = fsdp_config.get('use_orig_params', True)
+
     # We choose to not wrap the ComposerModel directly, but instead wrap any submodules like `ComposerModel.model`
     # This makes it safer to call ComposerModel-specific functions like 'eval_forward' that
     # may make calls to sharded submodules. If we only wrap the submodules, then any call that ComposerModel makes
     # to a FSDP-wrapped submodule's `forward()` function will be safe and all-gather the necessary weights before `forward()`.
     for obj_name, obj in model.named_children():
         if not isinstance(obj, (Metric, MetricCollection)):
 
+            # Skip wrapping submodules which are explicitly marked with no wrap
+            if hasattr(obj, '_fsdp_wrap') and not bool(obj._fsdp_wrap):
+                continue
+
             def _param_init_fn(module: torch.nn.Module) -> None:
                 # A dictionary of all tied parameter pointers to module names
                 tied_pointers = {}
 
                 # Goes through all modules finding which weights have the same pointers
                 for name, mod in module.named_modules():
                     for attr in ['weight', 'bias']:
                         if hasattr(mod, attr):
-                            ptr = id(getattr(mod, attr))
+                            mod_attr = getattr(mod, attr)
+                            if mod_attr is None:
+                                continue
+                            ptr = id(mod_attr)
                             ptr_attr = (ptr, attr)
                             name_list = tied_pointers.get(ptr_attr, [])
                             name_list.append(name)
                             tied_pointers[ptr_attr] = name_list
 
                 # Creates a dictionary of module names that should be tied together
                 tied_mod_names = collections.defaultdict(list)
@@ -271,40 +316,60 @@
                         'This leaves parameters without initialization. Please add a ``param_init_fn`` or ``reset_parameters`` '
                         f'to module `{obj_name}`.')
 
             # Choose which modules to FSDP wrap according to the following priority:
             # If module has attribute `module._fsdp_wrap = ...`, always respect it
             # Otherwise wrap if root object `obj.fsdp_wrap_fn(module)` is true
             # Or if unwrapped params in module in greater than or equal to fsdp_config.min_params
-            def _auto_wrap_policy(module: torch.nn.Module, recurse: bool, unwrapped_params: int) -> bool:
+            def __auto_wrap_policy(module: torch.nn.Module, recurse: bool, nonwrapped_numel: int) -> bool:
                 if recurse:
                     return True
+                should_be_wrapped = False
+                if hasattr(module, '_fsdp_wrap'):
+                    should_be_wrapped = bool(module._fsdp_wrap)
                 else:
-                    if hasattr(module, '_fsdp_wrap'):
-                        return bool(module._fsdp_wrap)
-
-                    is_large = unwrapped_params >= min_params
+                    is_large = nonwrapped_numel >= min_params
                     if hasattr(obj, 'fsdp_wrap_fn') and isinstance(obj.fsdp_wrap_fn, Callable):
-                        return obj.fsdp_wrap_fn(module) or is_large
+                        should_be_wrapped = obj.fsdp_wrap_fn(module) or is_large
                     else:
-                        return is_large
+                        should_be_wrapped = is_large
+
+                if should_be_wrapped and auto_microbatching:
+                    module.register_forward_hook(sync_hook)
+                    module.register_full_backward_hook(sync_hook)
+                return should_be_wrapped
+
+            if is_torch_2_0:
+
+                def _auto_wrap_policy_new(module: torch.nn.Module, recurse: bool, nonwrapped_numel: int) -> bool:
+                    return __auto_wrap_policy(module, recurse, nonwrapped_numel)
+
+                _auto_wrap_policy = _auto_wrap_policy_new
+
+            else:
+
+                def _auto_wrap_policy_old(module: torch.nn.Module, recurse: bool, unwrapped_params: int) -> bool:
+                    return __auto_wrap_policy(module, recurse, unwrapped_params)
+
+                _auto_wrap_policy = _auto_wrap_policy_old
 
             fsdp_obj = MosaicFullyShardedDataParallel(
                 obj,
                 sharding_strategy=sharding_strategy,
                 auto_wrap_policy=_auto_wrap_policy,
                 cpu_offload=cpu_offload,
                 mixed_precision=mixed_precision,
                 backward_prefetch=backward_prefetch,
                 ignored_modules=ignored_modules,
                 param_init_fn=_param_init_fn,
                 device_id=torch.cuda.current_device(),
                 sync_module_states=sync_module_states,
                 forward_prefetch=forward_prefetch,
                 limit_all_gathers=limit_all_gathers,
+                **kwargs,
             )
 
             # Activation Checkpointing
             if activation_checkpointing or activation_cpu_offload:
                 if not activation_checkpointing_reentrant:
                     first_wrap_fn = lambda m: checkpoint_wrapper(m, checkpoint_impl=CheckpointImpl.NO_REENTRANT
                                                                 ) if activation_checkpointing else (lambda module:
@@ -321,15 +386,17 @@
                             first_wrap_fn(module),  # type: ignore reportGeneralTypeIssues
                             offload_to_cpu=True)) if activation_cpu_offload else first_wrap_fn
 
                 # Choose which modules to activation checkpoint according to the following priority:
                 # If module has attribute `module._activation_checkpointing = ...`, always respect it
                 # Otherwise checkpoint if root object `obj.activation_checkpointing_fn(module)` is true
                 def _check_fn(module: torch.nn.Module) -> bool:
-                    if isinstance(module, (FullyShardedDataParallel, FlattenParamsWrapper)):
+                    if not is_torch_2_0 and isinstance(module, FlattenParamsWrapper):
+                        return False
+                    if isinstance(module, FullyShardedDataParallel):
                         return False
                     if hasattr(module, '_activation_checkpointing'):
                         return bool(module._activation_checkpointing)
                     if hasattr(obj, 'activation_checkpointing_fn') and isinstance(obj.activation_checkpointing_fn,
                                                                                   Callable):
                         return obj.activation_checkpointing_fn(module)
                     return False
```

### Comparing `composer-0.13.5/composer/trainer/meta_safe_apply.py` & `composer-0.14.0/composer/trainer/meta_safe_apply.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/trainer/mosaic_fsdp.py` & `composer-0.14.0/composer/trainer/mosaic_fsdp.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/trainer/trainer.py` & `composer-0.14.0/composer/trainer/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,38 +21,41 @@
 from typing import Any, Callable, ContextManager, Dict, Iterable, List, Optional, Sequence, TextIO, Tuple, Union, cast
 
 import coolname
 import torch
 import torch.distributed
 import torch.nn as nn
 import torch.utils.data
+from packaging import version
 from torch.cuda.amp.grad_scaler import GradScaler, _refresh_per_optimizer_state
 from torch.nn.parallel import DistributedDataParallel
 from torch.utils.data import DataLoader, DistributedSampler
 from torchmetrics import Metric
 
 from composer.callbacks import CheckpointSaver, OptimizerMonitor
 from composer.core import (Algorithm, AlgorithmPass, Batch, BreakEpochException, Callback, DataSpec, Engine, Evaluator,
                            Event, Precision, PyTorchScheduler, State, Time, Timestamp, TimeUnit, TrainerMode,
-                           ensure_data_spec, ensure_evaluator, ensure_time, get_precision_context)
+                           ensure_data_spec, ensure_evaluator, ensure_time, get_precision_context,
+                           validate_eval_automicrobatching)
 from composer.devices import Device, DeviceCPU, DeviceGPU, DeviceMPS, DeviceTPU
 from composer.loggers import (ConsoleLogger, Logger, LoggerDestination, ProgressBarLogger, RemoteUploaderDownloader,
                               WandBLogger)
 from composer.models import ComposerModel
 from composer.optim import ComposerScheduler, DecoupledSGDW, compile_composer_scheduler
 from composer.profiler import Profiler
 from composer.trainer._deepspeed import _fix_batch_precision_for_deepspeed, _parse_deepspeed_config
 from composer.trainer._scale_schedule import scale_pytorch_scheduler
 from composer.trainer._scaler import ClosureGradScaler
 from composer.trainer.dist_strategy import DDPSyncStrategy, ddp_sync_context, prepare_ddp_module, prepare_fsdp_module
 from composer.utils import (ExportFormat, MissingConditionalImportError, ObjectStore, Transform, checkpoint, dist,
                             ensure_tuple, export_with_logger, extract_hparams, format_name_with_dist, get_device,
                             get_file, is_tpu_installed, map_collection, maybe_create_object_store_from_uri,
                             maybe_create_remote_uploader_downloader_from_uri, model_eval_mode, parse_uri,
-                            reproducibility)
+                            reproducibility, using_torch_2)
+from composer.utils.misc import is_model_deepspeed
 
 if is_tpu_installed():
     import torch_xla.core.xla_model as xm
     import torch_xla.distributed.parallel_loader as pl
 
 log = logging.getLogger(__name__)
 
@@ -150,67 +153,56 @@
                 dataloader_len = None
             if dataloader_len == None:
                 raise ValueError('eval_subset_num_batches must be set when using an infinite sized '
                                  'eval_dataloader where length is `None`. Otherwise, evaluation will '
                                  'run forever and never terminate.')
 
 
-def _is_auto_grad_accum(grad_accum: Union[int, str], device: Device):
-    if grad_accum == 'auto':
-        warnings.warn(("Setting `grad_accum='auto'` is an experimental feature which may cause "
-                       'uncaught Cuda Out of Memory errors. In this case, please manually '
-                       'set grad_accum explicitly to an integer instead.'))
-        if not isinstance(device, DeviceGPU):
-            raise ValueError('Can only use adaptive grad_accum on GPU. Please set grad_accum >= 1')
-        return True
-    else:
-        return False
-
-
-def _is_auto_microbatching(device_train_microbatch_size: Union[int, str], device: Device):
+def _is_auto_microbatching(device_train_microbatch_size: Optional[Union[int, str]], device: Device):
     if device_train_microbatch_size == 'auto':
-        warnings.warn(("Setting `device_train_microbatch_size='auto'` is an experimental feature which may cause "
-                       'uncaught Cuda Out of Memory errors. In this case, please manually '
-                       'set device_train_microbatch_size explicitly to an integer instead.'))
+        warnings.warn(("`device_train_microbatch_size='auto'` may potentially fail with unexpected "
+                       'CUDA errors. Auto microbatching attempts to catch CUDA Out of Memory errors '
+                       'and adjust the batch size, but it is possible CUDA will be put into an '
+                       'irrecoverable state due to PyTorch bugs, e.g. integer overflow. In this case, '
+                       'please manually set device_train_microbatch_size explicitly to an integer '
+                       'instead.'))
         if not isinstance(device, DeviceGPU):
             raise ValueError(
                 'Can only use adaptive device_train_microbatch_size on GPU. Please set device_train_microbatch_size >= 1.'
             )
         return True
     else:
         return False
 
 
-def _get_initial_grad_accum(grad_accum: Union[int, str]):
-    if grad_accum == 'auto':
-        return 1
-    elif isinstance(grad_accum, int):
-        return grad_accum
-    else:
-        raise ValueError("grad_accum must be an int or ``'auto'``")
-
-
 def _get_initial_device_train_microbatch_size(device_train_microbatch_size: Optional[Union[int, str]],
                                               auto_microbatching: bool,
                                               train_dataloader: Optional[Iterable]) -> Optional[int]:
     """Sets initial value of device_train_microbatch_size.
 
     If auto_microbatching, sets initial `device_train_microbatch_size` to per rank batch size. If
     `train_dataloader` is not set yet, returns None and this function will be called again when
     `train_dataloader` is set, such as when `fit()` is called.
     """
-    if auto_microbatching:
+    if device_train_microbatch_size is None or auto_microbatching:
         # Return None, this function will be called again when `train_dataloader` is set
         if train_dataloader is None:
             return None
         try:
             batch_size = getattr(train_dataloader, 'batch_size')
         except AttributeError as e:
+            # Error message when `device_train_microbatch_size` is None
+            # Note: This code path will be removed after `auto` is made default
+            if device_train_microbatch_size is None:
+                raise ValueError(
+                    '`device_train_microbatch_size` must be set when `state.train_dataloader` does not have a `batch_size` attribute.'
+                ) from e
+            # Error message when `device_train_microbatch_size` is 'auto'
             raise AttributeError(
-                'device_train_microbatch_size requires the `state.train_dataloader` to have a `batch_size` attribute.'
+                "`device_train_microbatch_size='auto'` requires the `state.train_dataloader` to have a `batch_size` attribute."
             ) from e
         return batch_size
     elif isinstance(device_train_microbatch_size, int):
         return device_train_microbatch_size
     else:
         raise ValueError("device_train_microbatch_size must be an int or ``'auto'``")
 
@@ -226,47 +218,14 @@
                       'a non-contiguous input." This can happen when the batch_size is too large for the GPU so auto '
                       'auto_microbatching will rerun with a smaller microbatch size value, but there may be a user '
                       'error with non-contiguous inputs.')
         return True
     return False
 
 
-def _adjust_grad_accum(state: State, device_batch_size: int):
-    """Adjust grad_accum if we encounter OOM.
-
-    Args:
-        state (State): State of trainer.
-        device_batch_size (int): Batch size.
-    """
-    # If any rank hit CUDA OOM, update grad_accum and retry. Raise runtime error if training 1 sample
-    # at a time still resulted in CUDA out of memory.
-    assert state.grad_accum is not None
-    if state.grad_accum == device_batch_size:
-        raise RuntimeError(('CUDA out of memory. The train loop failed with an internal microbatch of size 1.'
-                            'The GPU does not have enough memory to process even 1 sample during train.'))
-    else:
-        original_grad_accum = state.grad_accum
-        state.grad_accum = min(2 * state.grad_accum, device_batch_size)
-        warnings.warn(
-            RuntimeWarning('CUDA out of memory detected. Gradient Accumulation, the number of train microbatches, '
-                           f'increased from {original_grad_accum} -> {state.grad_accum}, '
-                           'and the batch will be retrained with a '
-                           f'micro-batchsize of {device_batch_size // state.grad_accum}'))
-    # Clear gradients in case failure happened during backwards pass
-    if hasattr(state, 'outputs'):
-        del state.outputs
-    if hasattr(state, 'loss'):
-        del state.loss
-    for optimizer in state.optimizers:
-        optimizer.zero_grad(set_to_none=True)
-    if state.scaler is not None:
-        state.scaler._per_optimizer_states = defaultdict(_refresh_per_optimizer_state)
-    torch.cuda.empty_cache()
-
-
 def _adjust_device_train_microbatch_size(state: State):
     """Adjust device_train_microbatch_size if we encounter OOM.
 
     Args:
         state (State): State of trainer.
     """
     # If any rank hit CUDA OOM, update device_train_microbatch_size and retry. Raise runtime error
@@ -289,34 +248,32 @@
     for optimizer in state.optimizers:
         optimizer.zero_grad(set_to_none=True)
     if state.scaler is not None:
         state.scaler._per_optimizer_states = defaultdict(_refresh_per_optimizer_state)
     torch.cuda.empty_cache()
 
 
-def _adjust_eval_batch_split(state: State, device_batch_size: int):
-    """Adjust eval_batch_split if we encounter OOM.
+def _adjust_device_eval_microbatch_size(evaluator: Evaluator):
+    """Adjust device_eval_microbatch_size if we encounter OOM.
 
     Args:
-        state (State): State of trainer.
-        device_batch_size (int): Batch size.
+        evaluator (State): Current evaluator
     """
-    # If any rank hit CUDA OOM, update grad_accum and retry. Raise runtime error if training 1 sample
-    # at a time still resulted in CUDA out of memory.
-    if state.eval_batch_split == device_batch_size:
-        raise RuntimeError(('CUDA out of memory. The train loop failed with an internal microbatch of size 1.'
-                            'The GPU does not have enough memory to process even 1 sample in eval. '))
+    # If any rank hit CUDA OOM, update device_eval_microbatch_size and retry. Raise runtime error
+    # if evaluating 1 sample at a time still resulted in CUDA out of memory.
+    assert evaluator.device_eval_microbatch_size is not None
+    if evaluator.device_eval_microbatch_size == 1:
+        raise RuntimeError(('CUDA out of memory. The eval loop failed with an internal microbatch of size 1.'
+                            'The GPU does not have enough memory to process even 1 sample during eval.'))
     else:
-        original_eval_batch_split = state.eval_batch_split
-        state.eval_batch_split = min(2 * state.eval_batch_split, device_batch_size)
+        original_microbatch_size = evaluator.device_eval_microbatch_size
+        evaluator.device_eval_microbatch_size = max(int(original_microbatch_size / 2), 1)
         warnings.warn(
-            RuntimeWarning('CUDA out of memory detected. Number of eval microbatches '
-                           f'increased from {original_eval_batch_split} -> {state.eval_batch_split}, '
-                           'and the batch will be retrained with a '
-                           f'micro-batchsize of {device_batch_size // state.eval_batch_split}'))
+            RuntimeWarning('CUDA out of memory detected. Train microbatch size will be decreased from '
+                           f'{original_microbatch_size} -> {evaluator.device_eval_microbatch_size}.'))
     torch.cuda.empty_cache()
 
 
 def _distribute_and_get_random_seed(seed: Optional[int], device: Device):
     if not seed:
         seed = reproducibility.get_random_seed()
 
@@ -350,33 +307,14 @@
 
 def _get_precision_context(precision: Precision, deepspeed_enabled: bool):
     if deepspeed_enabled:
         return contextlib.nullcontext()
     return get_precision_context(precision)
 
 
-def _get_backwards_compatible_precision(precision: str):
-    if precision == 'fp16':
-        warnings.warn(
-            DeprecationWarning(
-                "'fp16' is deprecated as the naming is unclear and will be removed in 0.13. Use 'amp_fp16' instead."))
-        return Precision.AMP_FP16
-    if precision == 'amp':
-        warnings.warn(
-            DeprecationWarning(
-                "'amp' is deprecated as the naming is unclear and will be removed in 0.13. Use 'amp_fp16' instead."))
-        return Precision.AMP_FP16
-    if precision == 'bf16':
-        warnings.warn(
-            DeprecationWarning(
-                "'bf16' is deprecated as the naming is unclear and will be removed in 0.13. Use 'amp_bf16' instead."))
-        return Precision.AMP_BF16
-    return precision
-
-
 def _generate_run_name() -> str:
     # change coolname randomness for different names with same seed
     coolname.replace_random(random.Random(os.urandom(128)))
     # prefixing with the time so experiments sorted alphabetically will have the latest experiment last
     generated_run_name = str(int(time.time())) + '-' + coolname.generate_slug(2)
     run_name_list = [generated_run_name]
     # ensure all ranks have the same experiment name
@@ -773,32 +711,24 @@
 
             To use DeepSpeed with default values, set to the empty dictionary ``{}``.
             To disable DeepSpeed (the default), set to ``None``.
         fsdp_config (Dict[str, Any], optional): Configuration for FSDP.
             See :doc:`FSDP Documentation </notes/distributed_training>` for more details.
             To use FSDP with default values, set to the empty dictionary ``{}``. To
             disable FSDP, set to ``None``. (default: ``None``)
+        fsdp_auto_wrap (bool, optional): option to let trainer wrap the module, or if
+            the module is already wrapped outside, allow the user to disable auto-wrapping.
+
         device (Device | str, optional): The device to use for training, which can be ``'cpu'``, ``'gpu'``,
             ``'tpu'``, or ``'mps'``. (default: ``None``)
 
             The default behavior sets the device to ``'gpu'`` if CUDA is available, and otherwise ``'cpu'``.
         precision (Precision | str, optional): Numerical precision to use for training. One of ``fp32``, ``amp_bf16``
             or ``amp_fp16`` (recommended). (default: ``Precision.FP32`` if training on CPU; ``Precision.AMP_FP16`` if
             training on GPU)
-        grad_accum (Union[int, str], optional): The number of microbatches to split a per-device batch into. Gradients
-            are summed over the microbatches per device. If set to ``auto``, dynamically increases grad_accum
-            if microbatch is too large for GPU. (default: ``1``)
-
-            .. note:: This is implemented by taking the batch yielded by the ``train_dataloader`` and splitting
-                it into ``grad_accum`` sections. Each section is of size ``train_dataloader // grad_accum``.
-                If the batch size of the dataloader is not divisible by ``grad_accum``,
-                then the last section will be of size ``batch_size mod grad_accum``.
-
-            .. deprecated:: 0.12
-               Please use device_train_microbatch_size.
         device_train_microbatch_size (Union[int, str), optional): The number of samples to process on each device per
             microbatch during training. Gradients are summed over the microbatches per device. If set to ``auto``,
             dynamically decreases device_train_microbatch_size if microbatch is too large for GPU. (default: ``None``)
 
             .. note:: This is implemented by taking the batch yielded by the ``train_dataloader`` and splitting
                 it into sections of size ``device_train_microbatch_size``. If the batch size of the dataloader
                 is not divisible by ``device_train_microbatch_size``, the last section will be potentially smaller.
@@ -818,29 +748,34 @@
 
             .. note:: In order to get reproducible results, call the
                 :func:`.configure_deterministic_mode` function at the start of your script.
                 This will ensure any initialization done before the trainer init also runs deterministically.
 
             .. seealso:: :mod:`composer.utils.reproducibility` for more details on reproducibility.
         dist_timeout (float, optional): Timeout, in seconds, for initializing the distributed process group.
-            (default: ``1800.0``)
+            (default: ``300.0``)
         ddp_sync_strategy (str | DDPSyncStrategy, optional): The strategy to use for synchronizing gradients.
             Leave unset to let the trainer auto-configure this. See :class:`.DDPSyncStrategy`
             for more details.
         profiler (Profiler, optional): The profiler, if profiling should be enabled. (default: ``None``)
 
             .. seealso::
 
                 See the :doc:`Profiling Guide </trainer/performance_tutorials/profiling>` for
                 additional information.
         python_log_level (str, optional): The Python log level to use for log statements in the :mod:`composer`
             module. (default: ``None``). If it is ``None``, python logging will not be configured (i.e.
             ``logging.basicConfig`` won't be called).
 
             .. seealso:: The :mod:`logging` module in Python.
+        compile_config (Dict[str, Any], optional): Configuration for torch compile. Only supported with PyTorch 2.0 or higher.
+            Checkout [`torch.compile`](https://pytorch.org/get-started/pytorch-2.0/) for more details.
+            To use torch compile with default values, set it to empty dictionary ``{}``.
+            To use torch compile with custom config, set to a dictionary such as ``{'mode': 'max-autotune'}``.
+            To disable torch compile, set to ``None``. (default: ``None``)
 
     Attributes:
         state (State): The :class:`.State` object used to store training state.
         evaluators (List[Evaluator]): The :class:`.Evaluator` objects to use for validation
             during training.
         logger (Logger): The :class:`.Logger` used for logging.
         engine (Engine): The :class:`.Engine` used for running callbacks and algorithms.
@@ -910,34 +845,37 @@
 
         # Graceful Resumption
         autoresume: bool = False,
 
         # DeepSpeed
         deepspeed_config: Optional[Dict[str, Any]] = None,
         fsdp_config: Optional[Dict[str, Any]] = None,
+        fsdp_auto_wrap: Optional[bool] = True,
 
         # System/Numerics
         device: Optional[Union[str, Device]] = None,
         precision: Optional[Union[str, Precision]] = None,
-        grad_accum: Optional[Union[int, str]] = 1,
         device_train_microbatch_size: Optional[Union[int, str]] = None,
 
         # Reproducibility
         seed: Optional[int] = None,
         deterministic_mode: bool = False,
 
         # Distributed Training
-        dist_timeout: float = 1800.0,
+        dist_timeout: float = 300.0,
         ddp_sync_strategy: Optional[Union[str, DDPSyncStrategy]] = None,
 
         # Profiling
         profiler: Optional[Profiler] = None,
 
         # Python logging
         python_log_level: Optional[str] = None,
+
+        # compile config for PyTorch 2.0 or higher
+        compile_config: Optional[Dict[str, Any]] = None,
     ):
 
         self.auto_log_hparams = auto_log_hparams
         self.python_log_level = python_log_level
         if self.python_log_level is not None:
             logging.basicConfig(
                 # Example of format string
@@ -950,37 +888,74 @@
             logging.getLogger('composer').setLevel(self.python_log_level.upper())
 
         algorithms = list(ensure_tuple(algorithms))
 
         # Device
         device = get_device(device)
 
-        # Determine whether DeepSpeed and FSDP are enabled
-        self.deepspeed_config = deepspeed_config
-        self.fsdp_config = fsdp_config
-        self.deepspeed_enabled = self.deepspeed_config is not None
-        self.fsdp_enabled = self.fsdp_config is not None
-
         # Precision
         if precision is None:
             precision = Precision.AMP_FP16 if isinstance(device, DeviceGPU) else Precision.FP32
-        if isinstance(precision, str):
-            precision = _get_backwards_compatible_precision(precision)
+        elif isinstance(precision, str):
             precision = Precision(precision)
         _validate_precision(precision, device)
 
+        # check if provided model is compiled or not
+        is_torch_2_0 = using_torch_2()
+        is_model_compiled = False
+        if is_torch_2_0:
+            from torch._dynamo import OptimizedModule
+            if isinstance(model, OptimizedModule):
+                log.warning(f'Provided `model` is already compiled with `torch.compile`. Ignoring ' +
+                            f'parameter `compile_config` if provided. If you would like `Trainer` ' +
+                            f'to takes care of model compilation, provide a not-compiled model and ' +
+                            f'`compile_config` parameter.')
+                # The `torch.compile` function returns an object of type `torch._dynamo.OptimizedModule`
+                # which wraps the original `nn.Module` object and later patches its forward method to
+                # optimized `self.forward` method.
+                is_model_compiled = True
+                compiled_model = model._orig_mod
+                if not isinstance(compiled_model, ComposerModel):
+                    raise ValueError(f'Provided `model` must be a subclass of ComposerModel. ' +
+                                     f'Instead found as type `{type(compiled_model)}`')
+                compiled_model.forward = model.dynamo_ctx(
+                    compiled_model.forward)  # pyright: ignore [reportGeneralTypeIssues]
+                model = compiled_model
+
+        # Microbatching
+        auto_microbatching = _is_auto_microbatching(device_train_microbatch_size, device=device)
+        if auto_microbatching and profiler:
+            raise ValueError("`device_train_microbatch_size='auto'` is not compatible with the profiler. It is "
+                             "recommended to run a mini-run with `device_train_microbatch_size='auto'` to identify "
+                             'the optimal device_train_microbatch_size value and then manually specify that in a '
+                             'second run with profiler.')
+        self.first_batch_complete = False
+        # If auto_microbatching is True or `device_train_microbatch_size` is not specified, the microbatch size
+        # will be determined when dataloader is specified. train_dataloader is parsed after `Event.INIT` or in
+        # fit()
+        device_train_microbatch_size = _get_initial_device_train_microbatch_size(device_train_microbatch_size,
+                                                                                 auto_microbatching, None)
+
+        assert not isinstance(device_train_microbatch_size, str)
+
+        # Determine whether DeepSpeed and FSDP are enabled
+        self.deepspeed_config = deepspeed_config
+        self.fsdp_config = fsdp_config
+        self.deepspeed_enabled = self.deepspeed_config is not None
+        self.fsdp_enabled = self.fsdp_config is not None
+
         # Distributed
         if self.deepspeed_enabled or self.fsdp_enabled or dist.get_world_size() > 1:
             # Deepspeed and FSDP both require torch.distributed to be initialized, even if the world size is 1
             # And torch.distributed is always required for multi-rank training
             dist.initialize_dist(device, dist_timeout)
 
-        # Handle FSDP sharding
-        if self.fsdp_config is not None:
-            prepare_fsdp_module(model, optimizers, self.fsdp_config, precision)
+        # Handle FSDP wrapping
+        if self.fsdp_config is not None and fsdp_auto_wrap:
+            prepare_fsdp_module(model, optimizers, self.fsdp_config, precision, device, auto_microbatching)
 
         # Reproducibility
         rank_zero_seed, seed = _distribute_and_get_random_seed(seed, device)
         # If hparams is used to create the Trainer this function is called twice
         # which is okay because all runs with the hparams codepath will do this
         reproducibility.seed_all(seed)
         if deterministic_mode:
@@ -994,86 +969,42 @@
                            f"{type(optimizers).__name__}(lr={optimizers.defaults['lr']})"))
 
         num_optimizers = len(ensure_tuple(optimizers))
         if num_optimizers != 1:
             raise NotImplementedError(f'Only one optimizer is supported; found {num_optimizers} optimizers')
 
         # Move the model and optimizers to the device
-
         if not (self.deepspeed_enabled or self.fsdp_enabled):
             # check if model is already on tpu
             if isinstance(device, DeviceTPU) and 'xla' not in str(next(model.parameters()).device):
                 raise ValueError(
                     'Use model.to(xm.xla_device()) to set the model to the TPU before providing to the trainer.')
             else:
                 model = device.module_to_device(model)
                 # Move any remaining optimizer parameters onto the device
                 # It is possible that optimizer initialize created some internal tensors on CPU
                 # that need to be moved onto GPU.
             optimizers = map_collection(optimizers, device.optimizer_to_device)
 
-        # Microbatching
-        # To support backwards compatibility, we currently support both device_train_microbatch_size
-        # and grad_accum. If both are specified with grad_accum=1, we will use device_train_microbatch_size.
-        if device_train_microbatch_size is not None:
-            using_device_microbatch_size = True
-            if grad_accum != 1:
-                raise ValueError(
-                    'Cannot use both device_train_microbatch_size and grad_accum. grad_accum is deprecated '
-                    'so it is recommended to use device_train_microbatch_size.')
-            grad_accum = None
-            auto_microbatching = _is_auto_microbatching(device_train_microbatch_size, device=device)
-            if auto_microbatching and profiler:
-                raise ValueError("`device_train_microbatch_size='auto'` is not compatible with the profiler. It is "
-                                 "recommended to run a mini-run with `device_train_microbatch_size='auto'` to identify "
-                                 'the optimal device_train_microbatch_size value and then manually specify that in a '
-                                 'second run with profiler.')
-            # If auto_microbatching is True, the microbatch size will be determined when dataloader
-            # is specified. train_dataloader is parsed after `Event.INIT` or in fit()
-            device_train_microbatch_size = _get_initial_device_train_microbatch_size(
-                device_train_microbatch_size, auto_microbatching, None)
-        elif grad_accum is not None:
-            using_device_microbatch_size = False
-            if grad_accum != 1:
-                warnings.warn(
-                    DeprecationWarning(
-                        f'grad_accum set to {grad_accum} but is deprecated and will be removed in 0.13. Please use device_train_microbatch_size instead.'
-                    ))
-            auto_microbatching = _is_auto_grad_accum(grad_accum, device=device)
-            if auto_microbatching and profiler:
-                raise ValueError("`grad_accum='auto'` is not compatible with the profiler. It is recommended to run "
-                                 "a mini-run with `grad_accum='auto'` to identify the optimal grad_accum value and "
-                                 'then manually specify that in a second run with profiler.')
-            grad_accum = _get_initial_grad_accum(grad_accum)
-        else:
-            raise ValueError('Either grad_accum or device_train_microbatch_size must be specified. As grad-accum '
-                             'is deprecated, we recommend using device_train_microbatch_size.')
-        eval_batch_split = 1
-        assert not isinstance(grad_accum, str)
-        assert not isinstance(device_train_microbatch_size, str)
-
         # Run Name
         if run_name is None:
             if autoresume:
                 raise ValueError('When autoresume=True, the `run_name` must be specified.')
             run_name = _generate_run_name()
         log.info('Run name: %s', run_name)
 
         # Create the State
         self.state = State(
             rank_zero_seed=rank_zero_seed,
             algorithms=algorithms,
             model=model,
             device=device,
             callbacks=callbacks,
-            grad_accum=grad_accum,
-            eval_batch_split=eval_batch_split,
             device_train_microbatch_size=device_train_microbatch_size,
             auto_microbatching=auto_microbatching,
-            using_device_microbatch_size=using_device_microbatch_size,
             precision=precision,
             optimizers=optimizers,
             run_name=run_name,
             deepspeed_config=deepspeed_config,
             fsdp_config=fsdp_config,
         )
 
@@ -1194,15 +1125,15 @@
         self.logger.log_hyperparameters({
             'num_nodes': int(dist.get_world_size() / dist.get_local_world_size()),
             f'num_{device_name}s_per_node': dist.get_local_world_size(),
             'node_name': os.environ.get('NODENAME', 'unknown because NODENAME environment variable not set')
         })
 
         if not isinstance(self.state.model, ComposerModel):
-            raise ValueError('Provided model should be a subclass of ComposerModel.')
+            raise ValueError('Provided model must be a subclass of ComposerModel.')
 
         # After running Event.INIT, then set the "optional" elements of state that could be passed in on FIT instead of INIT
         # Setting these attributes here ensures that algorithms do not depend on unavailable attributes during Event.INIT
 
         # Metrics and Evaluators
         # Set state.train_metrics and state.eval_metrics here to allow callbacks / algs to potentially
         # change the model, which could change what metrics are computed
@@ -1224,14 +1155,17 @@
             }
 
             _set_evaluator_interval_and_subset_num_batches(
                 evaluators=evaluators,
                 eval_interval=eval_interval,
                 subset_num_batches=eval_subset_num_batches,
             )
+
+            for evaluator in evaluators:
+                validate_eval_automicrobatching(evaluator.auto_microbatching, self.state.device)
         if len(evaluators) == 0:
             if eval_subset_num_batches != -1:
                 raise ValueError(
                     f'Specifying `eval_subset_num_batches={eval_subset_num_batches}` without an `eval_dataloader` '
                     'has no effect. If trying to run an evaluator, make sure `eval_dataloader` is specified. '
                     'Otherwise, set `eval_subset_num_batches` to default value -1.')
             if eval_interval != 1:
@@ -1247,17 +1181,16 @@
         if self._train_data_spec is not None:
             self.state.set_dataloader(self._train_data_spec.dataloader, train_dataloader_label,
                                       train_subset_num_batches)
             if isinstance(self.state.device, DeviceTPU):
                 self.state.train_dataloader = pl.MpDeviceLoader(self.state.dataloader, xm.xla_device())
             else:
                 self.state.train_dataloader = self.state.dataloader
-            if self.state.using_device_microbatch_size:
-                self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
-                    self.state.device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
+            self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
+                self.state.device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
 
         # Max Duration
         if max_duration is not None:
             self.state.max_duration = ensure_time(max_duration, TimeUnit.EPOCH)
 
         self.logger.log_hyperparameters({'rank_zero_seed': rank_zero_seed})
 
@@ -1277,16 +1210,14 @@
         self._backwards_create_graph = any(map(lambda x: x.backwards_create_graph, self.state.algorithms))
         self._find_unused_parameters = any(map(lambda x: x.find_unused_parameters, self.state.algorithms))
         self._ddp_sync_strategy = _get_ddp_sync_strategy(ddp_sync_strategy, self._find_unused_parameters)
 
         # If using DDP or DeepSpeed, we need to wrap the ComposerModel
         # But store a reference to the original model for functions like `eval_forward`, `get_metrics`, etc.
         self._original_model = self.state.model
-        if not isinstance(self._original_model, ComposerModel):
-            raise ValueError('self.state.model must be a subclass of ComposerModel.')
 
         # Configure Deepspeed
         if self.state.deepspeed_config is not None:
             for callback in self.state.callbacks:
                 if isinstance(callback, OptimizerMonitor):
                     raise ValueError('OptimizerMonitor is not supported with DeepSpeed because DeepSpeed clears '
                                      'the gradients before in the last call to .backward see: '
@@ -1324,14 +1255,25 @@
         # DDP.
 
         # suppressing GradScaler warnings as they are always created
         # self._use_grad_scaling() will raise a RuntimeError if grad scaling is not available when it is required
         warnings.filterwarnings(action='ignore', message='torch.cuda.amp.GradScaler')
         self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
 
+        if self.fsdp_config is not None:
+            if version.parse(torch.__version__) < version.parse('1.13.0'):
+                raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
+            from torch.distributed.fsdp.sharded_grad_scaler import ShardedGradScaler
+
+            # This state should never be reached, but we raise a ValueError just in case
+            if self._use_closures() and self.state.precision == Precision.AMP_FP16:
+                raise ValueError(f'Using closures and precision {self.state.precision} is not supported'
+                                 f' with FSDP. Please use another optimizer or precision type.')
+            self.state.scaler = ShardedGradScaler()
+
         # suppressing FSDP warning when auto grad accum exits the forward pass before completing
         warnings.filterwarnings(action='ignore', message='Forward order differs from that of the first iteration')
 
         # Load Checkpoint
         self._rng_state = None
         # If autoresume is enabled, first check for existing checkpoints to load
         if autoresume:
@@ -1411,14 +1353,31 @@
         log.info(f'Setting seed to {self.state.seed}')
         reproducibility.seed_all(self.state.seed)
 
         if not (self.deepspeed_enabled or self.fsdp_enabled) and dist.get_world_size() > 1:
             # Only wrap the module if required
             self.state.model = prepare_ddp_module(self.state.model, self._find_unused_parameters)
 
+        # The model would need to be torch.compile()'d after being wrapped in a distributed strategy
+        # to take advantage of any graph breaks.
+        if is_torch_2_0 and not is_model_compiled and compile_config is not None:
+            compiled_model = torch.compile(  # pyright: ignore [reportGeneralTypeIssues]
+                self.state.model, **compile_config)
+            self.state.model = compiled_model._orig_mod
+            self.state.model.forward = compiled_model.dynamo_ctx(self.state.model.forward)
+            is_model_compiled = True
+            # update local_hparams to ensure the `is_model_compiled` is set correctly for
+            # debugging purpose and for unit test.
+            if self.auto_log_hparams:
+                self.local_hparams['is_model_compiled'] = is_model_compiled
+        elif not is_torch_2_0 and compile_config is not None:
+            raise ValueError(f'`torch.compile` is supported for PyTorch 2.0 or higher.' +
+                             f'Either update your PyTorch version or disable parameter by providing ' +
+                             f'`compile_config` to `None`.')
+
     @property
     def saved_checkpoints(self) -> List[str]:
         """Returns list of saved checkpoints.
 
         .. note::
 
             For DeepSpeed, which saves file on every rank, only the files corresponding to the process's rank
@@ -1517,19 +1476,24 @@
 
             signal_file_path = os.path.join(os.path.dirname(latest_checkpoint_path),
                                             '.local_rank0_completed_autoresume')
             if dist.get_local_rank() == 0:
                 with open(signal_file_path, 'wb') as f:
                     f.write(b'local_rank0_completed_autoresume')
 
-            # avoid the collective call until the local rank zero has finished trying to download the checkpoint
-            # so that we don't timeout for large downloads
+            # Avoid the collective call until the local rank zero has finished trying to download the checkpoint
+            # so that we don't timeout for large downloads. This syncs all processes on the node
             with dist.local_rank_zero_download_and_wait(signal_file_path):
+                # Then, wait to ensure every node has finished downloading the checkpoint
                 dist.barrier()
 
+            if dist.get_local_rank() == 0:
+                os.remove(signal_file_path)
+            dist.barrier()
+
             # At this point the rank 0 filepath should exist on all ranks if the download succeeded
             # list of whether the checkpoint exists on each rank
             latest_checkpoint_exists = dist.all_gather_object(os.path.exists(latest_checkpoint_path))
 
             log.debug(
                 f'Checkpoint {latest_checkpoint_path} exists on rank {dist.get_global_rank()}? {os.path.exists(latest_checkpoint_path)}'
             )
@@ -1562,15 +1526,14 @@
 
         # Evaluation
         eval_dataloader: Optional[Union[Iterable, DataSpec, Evaluator, Sequence[Evaluator]]] = None,
         eval_subset_num_batches: int = -1,
         eval_interval: Union[int, str, Time, Callable[[State, Event], bool]] = 1,
 
         # Numerics
-        grad_accum: Optional[Union[int, str]] = None,
         device_train_microbatch_size: Optional[Union[int, str]] = None,
         precision: Optional[Union[str, Precision]] = None,
     ):
         """Train the model.
 
         The Composer :class:`.Trainer` supports multiple calls to :meth:`.fit`. Any arguments specified during
         the call to :meth:`.fit` will override the values specified when constructing the :class:`.Trainer`.
@@ -1671,26 +1634,24 @@
             optimizers (torch.optim.Optimizer | Sequence[torch.optim.Optimizer], optional): See :class:`.Trainer`.
             schedulers (PyTorchScheduler | ComposerScheduler | Sequence[PyTorchScheduler | ComposerScheduler], optional): See :class:`.Trainer`.
             scale_schedule_ratio (float, optional): See :class:`.Trainer`.
             step_schedulers_every_batch (bool, optional): See :class:`.Trainer`.
             eval_dataloader (Iterable | DataSpec | Evaluator | Sequence[Evaluator], optional): See :class:`.Trainer`.
             eval_subset_num_batches (int, optional): See :class:`.Trainer`.
             eval_interval (int | str | Time | (State, Event) -> bool, optional): See :class:`.Trainer`.
-            grad_accum (int | str, optional): See :class:`.Trainer`.
             device_train_microbatch_size (int | str, optional): See :class:`.Trainer`.
             precision (Precision | str, optional): See :class:`.Trainer`.
         """
         # Train Dataloader
         if train_dataloader is not None:
             self._train_data_spec = ensure_data_spec(train_dataloader)
             self.state.set_dataloader(self._train_data_spec.dataloader, train_dataloader_label)
             self.state.train_dataloader = self.state.dataloader
-            if self.state.using_device_microbatch_size:
-                self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
-                    self.state.device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
+            self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
+                self.state.device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
         if self._train_data_spec is None:
             _raise_missing_argument_exception('train_dataloader')
         if train_subset_num_batches is not None:
             self.state.dataloader_len = train_subset_num_batches
 
         # Reset Time
         if reset_time:
@@ -1761,78 +1722,75 @@
             }
 
             _set_evaluator_interval_and_subset_num_batches(
                 evaluators=evaluators,
                 eval_interval=eval_interval,
                 subset_num_batches=eval_subset_num_batches,
             )
+
+            for evaluator in evaluators:
+                validate_eval_automicrobatching(evaluator.auto_microbatching, self.state.device)
+
             if len(evaluators) == 0:
                 if eval_subset_num_batches != -1:
                     raise ValueError('Specifying `eval_subset_num_batches` without an `eval_dataloader` has no effect.')
                 if eval_interval != 1:
                     raise ValueError('Specifying `eval_interval` without an `eval_dataloader` has no effect.')
 
             self.state.evaluators = evaluators
 
         # Microbatching
-        if grad_accum is not None and device_train_microbatch_size is not None:
-            raise ValueError('Cannot specify both `grad_accum` and `device_train_microbatch_size`.')
-        elif device_train_microbatch_size is not None:
+        if device_train_microbatch_size is not None:
             self.state.auto_microbatching = _is_auto_microbatching(device_train_microbatch_size,
                                                                    device=self.state.device)
             if self.state.auto_microbatching and self.state.profiler:
                 raise ValueError("`device_train_microbatch_size='auto'` is not compatible with the profiler. It is "
                                  "recommended to run a mini-run with `device_train_microbatch_size='auto'` to identify "
                                  'the optimal device_train_microbatch_size value and then manually specify that in a '
                                  'second run with profiler.')
             self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
                 device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
-            self.state.using_device_microbatch_size = True
-        elif grad_accum is not None:
-            self.state.auto_microbatching = _is_auto_grad_accum(grad_accum, device=self.state.device)
-            if self.state.auto_microbatching and self.state.profiler:
-                raise ValueError("`grad_accum='auto'` is not compatible with the profiler. It is recommended to run "
-                                 "a mini-run with `grad_accum='auto'` to identify the optimal grad_accum value and "
-                                 'then manually specify that in a second run with profiler.')
-            self.state.grad_accum = _get_initial_grad_accum(grad_accum)
-            self.state.using_device_microbatch_size = False
 
         # Precision
         if precision is not None:
-            if isinstance(precision, str):
-                precision = _get_backwards_compatible_precision(precision)
             if Precision(precision) != self.state.precision:
                 if self.deepspeed_enabled:
                     raise ValueError('Changing the precision when using DeepSpeed is not supported')
                 precision = Precision(precision)
                 _validate_precision(precision, self.state.device)
                 self.state.precision = precision
 
             # update scaler since precision was provided
             self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
+
+        self.first_batch_complete = False
         self._train_loop()
 
     def close(self):
         """Shutdown the trainer.
 
         .. seealso:: :meth:`.Engine.close` for additional information.
         """
         self.engine.close()
         dist.barrier()
 
     def _ensure_metrics_device_and_dtype(self, metrics: Dict[str, Metric]):
-        # HACK: DeepSpeed somehow manages to convert metric internal states to its own dtype. When
-        # running with FP16, this tends to result in overflows. Let's assume FP32 is good enough.
         for name, metric in metrics.items():
             # Safety check to ensure the metric and data are on the same device. Normally not
             # needed because the metric is automatically on the same device as the model.
             # See https://torchmetrics.readthedocs.io/en/latest/pages/overview.html for details.
             metrics[name] = self.state.device.module_to_device(metric)
-            metric.set_dtype(torch.float32)  # type: ignore
-
+            if is_model_deepspeed(self.state.model):
+                # HACK: DeepSpeed somehow manages to convert metric internal states to its own dtype. When
+                # running with FP16, this tends to result in overflows. Let's assume FP32 is good enough.
+                for key in metric._defaults:
+                    metric_data = getattr(metric, key)
+                    if isinstance(metric_data, torch.Tensor) and metric_data.dtype == torch.float16:
+                        metric_data = metric_data.to(torch.float32)  # type: ignore
+                        setattr(metric, key, metric_data)
         return metrics
 
     def _compute_and_log_metrics(self, dataloader_label: str, metrics: Dict[str, Metric]):
         """Computes metrics, logs the results, and updates the state with the deep-copied metrics.
 
         Args:
             dataloader_label (str): The dataloader label.
@@ -1936,15 +1894,15 @@
         finished_epoch_early = False
         last_wct = datetime.datetime.now()
 
         while self.state.timestamp < self.state.max_duration:
             try:
                 if int(self.state.timestamp.batch_in_epoch) == 0:
                     self.engine.run_event(Event.EPOCH_START)
-                    self.logger.log_metrics({'trainer/epoch': int(self.state.timestamp.epoch)})
+                    self.logger.log_metrics({'time/epoch': self.state.timestamp.epoch.value})
 
                 dataloader = self.state.dataloader
                 if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
                     dataloader.sampler.set_epoch(int(self.state.timestamp.epoch))
 
                 for batch_idx, self.state.batch in enumerate(self._iter_dataloader(TrainerMode.TRAIN)):
                     # Don't spin if dataloader handles it internally. Otherwise, if resuming, skip dataloader forward
@@ -1963,18 +1921,25 @@
 
                     if self.deepspeed_enabled:
                         self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
 
                     self.engine.run_event(Event.AFTER_DATALOADER)
 
                     self.engine.run_event(Event.BATCH_START)
+
+                    # Log time values
                     self.logger.log_metrics({
-                        'trainer/global_step': int(self.state.timestamp.batch),
-                        'trainer/batch_idx': self.state.timestamp.batch_in_epoch.value,
+                        'time/batch': self.state.timestamp.batch.value,
+                        'time/sample': self.state.timestamp.sample.value,
+                        'time/batch_in_epoch': self.state.timestamp.batch_in_epoch.value,
+                        'time/sample_in_epoch': self.state.timestamp.sample_in_epoch.value,
                     })
+                    if rank_num_tokens > 0:
+                        self.logger.log_metrics({'time/token': self.state.timestamp.token.value})
+                        self.logger.log_metrics({'time/token_in_epoch': self.state.timestamp.token_in_epoch.value})
 
                     total_loss_dict = self._train_batch(use_grad_scaling)
 
                     if use_grad_scaling:
                         self.state.scaler.update()
 
                     # total_loss_dict can be None if gradient scaling failed
@@ -2009,14 +1974,15 @@
 
                     if self.state.train_metrics is not None:
                         self._compute_and_log_metrics(
                             dataloader_label='train',
                             metrics=self.state.train_metrics,
                         )
 
+                    self.state.previous_timestamp = self.state.timestamp
                     self.state.timestamp = self.state.timestamp.to_next_batch(
                         samples=total_num_samples,
                         tokens=total_num_tokens,
                         duration=batch_time,
                     )
 
                     self.engine.run_event(Event.BATCH_END)
@@ -2047,67 +2013,70 @@
                             metrics=self.state.train_metrics,
                         )
 
                     if self._scheduler_step_frequency == TimeUnit.EPOCH:
                         for scheduler in self.state.schedulers:
                             scheduler.step()
 
+                    self.state.previous_timestamp = self.state.timestamp
                     self.state.timestamp = self.state.timestamp.to_next_epoch()
 
                     self.engine.run_event(Event.EPOCH_END)
 
                     # Pause the timing during evaluation
                     # Evaluation time is tracked separately in state.eval_timestamp
                     duration = datetime.datetime.now() - last_wct
                     self._run_evaluators(Event.EPOCH_END)
                     last_wct = datetime.datetime.now() - duration
 
                     self.engine.run_event(Event.EPOCH_CHECKPOINT)
             except BreakEpochException:
                 log.info(f'Skipping the rest of Epoch {int(self.state.timestamp.epoch)}')
 
+        # Log final time values
+        self.logger.log_metrics({
+            'time/epoch': self.state.timestamp.epoch.value,
+            'time/batch': self.state.timestamp.batch.value,
+            'time/sample': self.state.timestamp.sample.value,
+            'time/batch_in_epoch': self.state.timestamp.batch_in_epoch.value,
+            'time/sample_in_epoch': self.state.timestamp.sample_in_epoch.value,
+        })
+        if self.state.previous_timestamp is not None and self.state.timestamp.token.value - self.state.previous_timestamp.token.value > 0:
+            self.logger.log_metrics({'time/token': self.state.timestamp.token.value})
+            self.logger.log_metrics({'time/token_in_epoch': self.state.timestamp.token_in_epoch.value})
+
         self.engine.run_event(Event.FIT_END)
         self._run_evaluators(Event.FIT_END)
 
     def _eval_train_metrics(self, device_batch):
         assert self._train_data_spec is not None, 'The train data spec should be set on __init__ or fit()'
         assert self.state.train_metrics is not None, 'The train metrics should be set on __init__ or fit()'
 
         with torch.no_grad(),\
                 model_eval_mode(self.state.model),\
                 _get_precision_context(self.state.precision, self.deepspeed_enabled):
-            if hasattr(self._original_model, 'validate'):  # backwards compatibility check
-                warnings.warn(
-                    DeprecationWarning(
-                        'Using validate() is deprecated and will be removed in 0.13. Please use eval_forward() instead.'
-                    ))
-                assert isinstance(self._original_model.validate, Callable)
-                eval_outputs, target = self._original_model.validate(device_batch)
-
-                for _, metric in self.state.train_metrics.items():
-                    metric.update(eval_outputs, target)
-            else:
-                eval_outputs = self._original_model.eval_forward(device_batch, self.state.outputs)
-                for _, metric in self.state.train_metrics.items():
-                    self._original_model.update_metric(
-                        device_batch,
-                        eval_outputs,
-                        metric,
-                    )
+            eval_outputs = self._original_model.eval_forward(device_batch, self.state.outputs)
+            for _, metric in self.state.train_metrics.items():
+                self._original_model.update_metric(
+                    device_batch,
+                    eval_outputs,
+                    metric,
+                )
 
     def _run_evaluators(self, event: Event):
         """Runs evaluators periodically during training."""
         for evaluator in self.state.evaluators:
             assert evaluator.eval_interval is not None, 'eval_interval should have been set on __init__() or fit()'
             assert evaluator.subset_num_batches is not None, 'subset_num_batches should have been set on __init__() or fit()'
             if evaluator.eval_interval(self.state, event):
-                self._eval_loop(dataloader=evaluator.dataloader,
-                                dataloader_label=evaluator.label,
-                                subset_num_batches=evaluator.subset_num_batches,
-                                metrics=self.state.eval_metrics[evaluator.label])
+                self._eval_loop(
+                    evaluator=evaluator,
+                    subset_num_batches=evaluator.subset_num_batches,
+                    metrics=self.state.eval_metrics[evaluator.label],
+                )
 
     def _train_batch(self, use_grad_scaling: bool) -> Dict[str, torch.Tensor]:
         """Compute loss by training on a full batch of data.
 
         Adaptively change microbatch size if enabled to maximize GPU usage.
 
         Args:
@@ -2130,22 +2099,16 @@
                 for _, metric in self.state.train_metrics.items():
                     metric.reset()
 
             total_loss_dict = {'loss/train/total': self.state.device.tensor_to_device(torch.zeros(size=(1,)))}
             found_cuda_oom = 0  # int since bool BOR not supported on all torch.distributed backends
             try:
                 assert self.state.scaler is not None
-                if self.state.using_device_microbatch_size:
-                    assert self.state.device_train_microbatch_size is not None
-                    microbatches = self._train_data_spec.split_batch(device_batch,
-                                                                     self.state.device_train_microbatch_size)
-                else:
-                    assert self.state.grad_accum is not None
-                    microbatches = self._train_data_spec._num_microbatches_split_batch(
-                        device_batch, self.state.grad_accum)
+                assert self.state.device_train_microbatch_size is not None
+                microbatches = self._train_data_spec.split_batch(device_batch, self.state.device_train_microbatch_size)
                 if self._use_closures():
                     for optimizer in self.state.optimizers:
                         if use_grad_scaling:
                             self.state.scaler.step(optimizer,
                                                    closure=lambda loss_dict=total_loss_dict, **kwargs: self.
                                                    _train_microbatches(microbatches, loss_dict, **kwargs))
                         else:
@@ -2166,33 +2129,34 @@
                 if self.state.auto_microbatching and _is_cuda_oom(e):
                     log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                     found_cuda_oom = 1
                 else:
                     raise
 
             if self.state.auto_microbatching:
-                # Propagate across all ranks if any rank hit CUDA OOM
-                found_cuda_oom = self.state.device.tensor_to_device(torch.tensor([found_cuda_oom], dtype=torch.uint8))
-                dist.all_reduce(found_cuda_oom, reduce_operation='MAX')
-                if found_cuda_oom.item() == 1:
-                    device_batch_size = self._train_data_spec.get_num_samples_in_batch(device_batch)
-                    if self.state.using_device_microbatch_size:
-                        _adjust_device_train_microbatch_size(self.state)
-                    else:
-                        _adjust_grad_accum(self.state, device_batch_size)
+                all_ranks_finished = False
+                while not all_ranks_finished:
+                    # Propagate across all ranks if any rank hit CUDA OOM
+                    found_cuda_oom_tensor = self.state.device.tensor_to_device(
+                        torch.tensor([found_cuda_oom], dtype=torch.uint8))
+                    dist.all_reduce(found_cuda_oom_tensor, reduce_operation='MAX')
+                    found_cuda_oom = found_cuda_oom_tensor.item()
+                    # Check if any rank is still not done with the batch. This may happen if only a
+                    # subset of ranks OOM, leaving some batches still in the forward pass
+                    all_ranks_finished_tensor = self.state.device.tensor_to_device(torch.tensor([1], dtype=torch.uint8))
+                    dist.all_reduce(all_ranks_finished_tensor, reduce_operation='MIN')
+                    all_ranks_finished = all_ranks_finished_tensor.item() == 1
+                if found_cuda_oom == 1:
+                    _adjust_device_train_microbatch_size(self.state)
                     # Skip return and rerun after handling oom
                     continue
             # Log microbatch and return loss if we've completed without OOMing.
-            if self.state.using_device_microbatch_size:
-                assert self.state.device_train_microbatch_size is not None
-                self.logger.log_metrics(
-                    {'trainer/device_train_microbatch_size': self.state.device_train_microbatch_size})
-            else:
-                assert self.state.grad_accum is not None
-                self.logger.log_metrics({'trainer/grad_accum': self.state.grad_accum})
+            assert self.state.device_train_microbatch_size is not None
+            self.logger.log_metrics({'trainer/device_train_microbatch_size': self.state.device_train_microbatch_size})
+            self.first_batch_complete = True
             return total_loss_dict
 
     def _train_microbatches(self,
                             microbatches: Sequence[Batch],
                             total_loss_dict: Dict[str, torch.Tensor],
                             ddp_sync: bool = True) -> torch.Tensor:
         """Iterate over microbatches and compute the loss that will be used to step the optimizer.
@@ -2204,15 +2168,27 @@
             ddp_sync (bool): True to sync gradients between devices on every backwards
                 pass and False to only sync gradients after each device has finished
                 computing a gradient on it's entire set of microbatches. (default: ``True``)
         """
         if ddp_sync or not isinstance(self.state.model, DistributedDataParallel):
             context = contextlib.nullcontext
         else:
-            context = cast(Callable[[], ContextManager], self.state.model.no_sync)
+            if self.state.auto_microbatching and not self.first_batch_complete:
+                # PyTorch DDP rebuilds gradient reduction buckets after 1) a forward pass where the
+                # no_sync context was not set 2) a backward pass 3) a forward pass. If only a
+                # subset of ranks OOM on the first batch, this will cause a deadlock since a rank
+                # that did not OOM will complete steps (1), (2), and (3) on the first succesful
+                # microbatch after the OOMs but an OOMing rank will have never completed (1) if
+                # using `SINGLE_AUTO_SYNC`. To avoid this, we force a sync on every microbatch for
+                # the first batch.
+                log.info('Auto microbatching requires syncing every microbatch (`MULTI_AUTO_SYNC`)'
+                         ' to avoid deadlock on first batch, so ddp_sync_strategy will be ignored.')
+                context = contextlib.nullcontext
+            else:
+                context = cast(Callable[[], ContextManager], self.state.model.no_sync)
 
         assert self._train_data_spec is not None
 
         with context():
             self.engine.run_event(Event.BEFORE_TRAIN_BATCH)
 
             assert self.state.optimizers is not None
@@ -2268,39 +2244,67 @@
         assert self.state.scaler is not None
         assert self._train_data_spec is not None
 
         # Cache the device batch, because `self.state.batch` gets overridden in microbatching loop
         device_batch = deepcopy(self.state.batch)
 
         microbatch_num_samples = self._train_data_spec.get_num_samples_in_batch(self.state.batch)
-        sync_context = contextlib.nullcontext() if self.deepspeed_enabled else ddp_sync_context(
-            self.state,
-            is_final_microbatch,
-            self._ddp_sync_strategy,
-        )
+        if self.deepspeed_enabled or not isinstance(self.state.model, DistributedDataParallel):
+            sync_context = contextlib.nullcontext()
+        elif self.state.auto_microbatching and not self.first_batch_complete:
+            # PyTorch DDP rebuilds gradient reduction buckets after 1) a forward pass where the
+            # no_sync context was not set 2) a backward pass 3) a forward pass. If only a
+            # subset of ranks OOM on the first batch, this will cause a deadlock since a rank
+            # that did not OOM will complete steps (1), (2), and (3) on the first succesful
+            # microbatch after the OOMs but an OOMing rank will have never completed (1) if
+            # using `SINGLE_AUTO_SYNC`. To avoid this, we force a sync on every microbatch for
+            # the first batch.
+            log.info('Auto microbatching requires syncing every microbatch (`MULTI_AUTO_SYNC`)'
+                     ' to avoid deadlock on first batch, so ddp_sync_strategy will be ignored.')
+            sync_context = contextlib.nullcontext()
+        else:
+            sync_context = ddp_sync_context(
+                self.state,
+                is_final_microbatch,
+                self._ddp_sync_strategy,
+            )
 
         with sync_context:
-            # forward pass
+            # Forward pass
             self.engine.run_event(Event.BEFORE_FORWARD)
 
             with _get_precision_context(self.state.precision, self.deepspeed_enabled):
                 self.state.outputs = self.state.model(self.state.batch)
 
             self.engine.run_event(Event.AFTER_FORWARD)
 
-            # loss
+            # Check if other ranks OOMed after forward pass when using auto microbatching. This may
+            # happen when close to memory limit or with uneven memory usage across ranks
+            if self.state.auto_microbatching:
+                # Check if any other rank hit an OOM
+                found_cuda_oom_tensor = self.state.device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
+                dist.all_reduce(found_cuda_oom_tensor, reduce_operation='MAX')
+                found_cuda_oom = found_cuda_oom_tensor.item()
+                # Signal current rank is still in batch
+                all_ranks_finished_tensor = self.state.device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
+                dist.all_reduce(all_ranks_finished_tensor, reduce_operation='MIN')
+
+                if found_cuda_oom == 1:
+                    raise RuntimeError('CUDA out of memory encountered on a different rank')
+
+            # Loss
             self.engine.run_event(Event.BEFORE_LOSS)
 
             with _get_precision_context(self.state.precision, self.deepspeed_enabled):
                 self.state.loss = self._original_model.loss(self.state.outputs, self.state.batch)
 
             assert self.state.loss is not None
             self.engine.run_event(Event.AFTER_LOSS)
 
-            # backward
+            # Backward Pass
             self.engine.run_event(Event.BEFORE_BACKWARD)
 
             microbatch_loss_dict = {}
             # If total loss key is present, copy loss
             if isinstance(self.state.loss, dict) and ('total' in self.state.loss):
                 microbatch_loss = self.state.loss['total']  # type: ignore
                 microbatch_loss_dict = self.state.loss.copy()
@@ -2563,21 +2567,14 @@
                 eval_dataloader=[glue_mrpc_task, glue_mnli_task],
                 ...
             )
 
         The metrics used are defined in your model's ``get_metrics()`` method. For more information,
         see :doc:`/trainer/evaluation`.
 
-        .. note::
-
-            This eval API was recently changed to better much the trainer fit API. Please migrate your
-            code to using the new design here. For backwards compatibility, the old API can still be
-            invoked by calling ``_eval_loop()``, however this is not recommended as this may be
-            removed in the future.
-
         Args:
             eval_dataloader (DataLoader | DataSpec | Evaluator | Sequence[Evaluator], optional): Dataloaders
                 for evaluation.  If not provided, defaults to using the
                 ``eval_dataloader`` provided to the trainer init().
             subset_num_batches (int, optional): Evaluate on this many batches. Default to ``-1`` (the entire
                 dataloader. Can also be provided in the trainer.__init__() as ``eval_subset_num_batches``.
 
@@ -2606,77 +2603,67 @@
             self.state.eval_metrics.update({e.label: _filter_metrics(eval_metrics, e.metric_names) for e in evaluators})
 
             _set_evaluator_interval_and_subset_num_batches(
                 evaluators=evaluators,
                 eval_interval='1ep',  # ignored
                 subset_num_batches=subset_num_batches,
             )
+
+            for evaluator in evaluators:
+                validate_eval_automicrobatching(evaluator.auto_microbatching, self.state.device)
+
             self.state.evaluators.extend(evaluators)  # Add evaluators to state.evaluators
         else:
             eval_passed_in = False
             if not self.state.evaluators:
                 raise ValueError('eval_dataloader must be provided to either Trainer init() or eval().')
             evaluators = self.state.evaluators
 
         for evaluator in evaluators:
             eval_subset_num_batches = evaluator.subset_num_batches if subset_num_batches == -1 else subset_num_batches
             self._eval_loop(
-                dataloader=evaluator.dataloader,
-                dataloader_label=evaluator.label,
-                subset_num_batches=eval_subset_num_batches,
+                evaluator=evaluator,
                 metrics=self.state.eval_metrics[evaluator.label],
+                subset_num_batches=eval_subset_num_batches,
             )
             if eval_passed_in:
                 self.state.evaluators.remove(evaluator)  # Remove them from state once eval is finished.
 
     def _eval_loop(
         self,
-        dataloader: Union[Iterable, DataSpec, dict],
-        dataloader_label: str = 'eval',
-        *,
+        evaluator: Evaluator,
         metrics: Dict[str, Metric],
         subset_num_batches: Optional[int] = None,
     ):
         """Evaluate the model and log appropriate metrics.
 
         Args:
-            dataloader (DataLoader | DataSpec | dict): The class:`.DataLoader`, :class:`.DataSpec`, or
-                dict of :class:`.DataSpec` kwargs to use for evaluation
-            dataloader_label (str, optional): The dataloader label to use for logging metrics. Defaults to ``'eval'``.
+            evaluator (Evaluator): The evaluator to use for evaluation.
             metrics (Dict[str, Metric]): Dictionary mapping metric names to metrics to evaluate against.
             subset_num_batches (int, optional): If specified, evaluate on this many batches. Defaults to ``-1``,
                 which means to iterate over the entire dataloader.
-
-                This parameter has no effect if ``eval_dataloader`` is not specified, it is greater than
-                ``len(eval_dataloader)``, or ``eval_dataloader`` is an :class:`.Evaluator` (which is via
-                ``Evaluator(subset_num_batches=...)``.)
         """
         if subset_num_batches is None:
             subset_num_batches = -1
 
         # back up the original dataloader on the state, so we can restore it after evaluation is finished
         original_dataloader = self.state.dataloader
         original_dataloader_label = self.state.dataloader_label
         original_num_batches = self.state.dataloader_len
 
-        # Unpack the dataloader
-        if isinstance(dataloader, dict):
-            # treat as DataSpec kwargs
-            dataloader = DataSpec(**dataloader)
-        if not isinstance(dataloader, DataSpec):
-            dataloader = DataSpec(dataloader)
-        data_spec = dataloader
+        # Unpack data_spec
+        data_spec = evaluator.dataloader
 
         # Reset the eval timestamp
         self.state.eval_timestamp = Timestamp()
 
         last_wct = datetime.datetime.now()
 
         with torch.no_grad(), model_eval_mode(self.state.model):
-            self.state.set_dataloader(data_spec.dataloader, dataloader_label, subset_num_batches)
+            self.state.set_dataloader(data_spec.dataloader, evaluator.label, subset_num_batches)
             assert self.state.dataloader is not None, 'dataloader is set'
 
             self.engine.run_event(Event.EVAL_START)
 
             metrics = self._ensure_metrics_device_and_dtype(metrics)
 
             for _, metric in metrics.items():
@@ -2707,28 +2694,20 @@
                 # Cache the device batch, because `self.state.batch` gets overridden in microbatching loop
                 device_batch = self.state.batch
                 # Retry until we successfully complete evaluation
                 while True:
                     # Note: We use uint8 instead of bool as BOR is not supported on all torch.distributed backends
                     found_cuda_oom = 0
                     try:
-                        for self.state.batch in data_spec._num_microbatches_split_batch(
-                                self.state.batch, self.state.eval_batch_split):
+                        for self.state.batch in data_spec.split_batch(device_batch,
+                                                                      evaluator.device_eval_microbatch_size):
                             self.engine.run_event(Event.EVAL_BEFORE_FORWARD)
                             with _get_precision_context(self.state.precision, self.deepspeed_enabled):
-                                if hasattr(self._original_model, 'validate'):  # backwards compatibility check
-                                    warnings.warn(
-                                        DeprecationWarning(
-                                            'Using validate() is deprecated and will be removed in 0.13. Please use eval_forward() instead.'
-                                        ))
-                                    assert isinstance(self._original_model.validate, Callable)
-                                    self.state.outputs, target = self._original_model.validate(self.state.batch)
-                                else:
-                                    self.state.outputs = self._original_model.eval_forward(self.state.batch)
-                                    target = None
+                                self.state.outputs = self._original_model.eval_forward(self.state.batch)
+                                target = None
 
                             self.engine.run_event(Event.EVAL_AFTER_FORWARD)
 
                             # Run in same precision context to avoid NaNs
                             with _get_precision_context(self.state.precision, self.deepspeed_enabled):
                                 if isinstance(self.state.device, DeviceMPS):
                                     # torchmetrics math has numerical errors on M1 devices
@@ -2745,29 +2724,33 @@
                                         self._original_model.update_metric(
                                             self.state.batch,
                                             outputs,
                                             metric,
                                         )
 
                     except RuntimeError as e:
-                        if self.state.auto_microbatching and _is_cuda_oom(e):
+                        if evaluator.auto_microbatching and _is_cuda_oom(e):
                             log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                             found_cuda_oom = 1
                         else:
                             raise
-                    if self.state.auto_microbatching:
+                    if evaluator.auto_microbatching:
                         # Propagate across all ranks if any rank hit CUDA OOM
                         found_cuda_oom = self.state.device.tensor_to_device(
                             torch.tensor([found_cuda_oom], dtype=torch.uint8))
                         dist.all_reduce(found_cuda_oom, reduce_operation='MAX')
                         if found_cuda_oom.item() == 1:
-                            device_batch_size = data_spec.get_num_samples_in_batch(device_batch)
-                            _adjust_eval_batch_split(self.state, device_batch_size)
+                            _adjust_device_eval_microbatch_size(evaluator)
                             # Skip return and rerun after handling oom
                             continue
+                        # Log device_eval_microbatch_size if auto_microbatching is enabled
+                        self.logger.log_metrics({
+                            f'trainer/{evaluator.label}/device_eval_microbatch_size':
+                                evaluator.device_eval_microbatch_size
+                        })
                     # Break if we've successfully completed eval without OOMing.
                     break
 
                 now = datetime.datetime.now()
                 batch_time = now - last_wct
 
                 total_num_samples, total_num_tokens, batch_time = self._accumulate_time_across_ranks(
@@ -2782,15 +2765,15 @@
                     duration=batch_time,
                 )
 
                 last_wct = now
 
                 self.engine.run_event(Event.EVAL_BATCH_END)
 
-            self._compute_and_log_metrics(dataloader_label=dataloader_label, metrics=metrics)
+            self._compute_and_log_metrics(dataloader_label=evaluator.label, metrics=metrics)
 
             self.engine.run_event(Event.EVAL_END)
 
         self.state.set_dataloader(original_dataloader, original_dataloader_label)
         if original_num_batches is not None:
             self.state.dataloader_len = original_num_batches
```

### Comparing `composer-0.13.5/composer/utils/__init__.py` & `composer-0.14.0/composer/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Helper utilities."""
-import warnings
 
 from composer.utils.auto_log_hparams import (convert_flat_dict_to_nested_dict, convert_nested_dict_to_flat_dict,
                                              extract_hparams)
 from composer.utils.batch_helpers import batch_get, batch_set
 from composer.utils.checkpoint import PartialFilePath, load_checkpoint, safe_torch_load, save_checkpoint
 from composer.utils.collect_env import (configure_excepthook, disable_env_report, enable_env_report,
                                         get_composer_env_dict, print_env)
@@ -15,30 +14,21 @@
                                          create_symlink_file, ensure_folder_has_no_conflicting_files,
                                          ensure_folder_is_empty, format_name_with_dist, format_name_with_dist_and_time,
                                          get_file, is_tar, maybe_create_object_store_from_uri,
                                          maybe_create_remote_uploader_downloader_from_uri, parse_uri)
 from composer.utils.import_helpers import MissingConditionalImportError, import_object
 from composer.utils.inference import ExportFormat, Transform, export_for_inference, export_with_logger, quantize_dynamic
 from composer.utils.iter_helpers import IteratorFileStream, ensure_tuple, map_collection
-from composer.utils.misc import get_free_tcp_port, is_model_deepspeed, is_model_fsdp, is_notebook, model_eval_mode
+from composer.utils.misc import (get_free_tcp_port, is_model_deepspeed, is_model_fsdp, is_notebook, model_eval_mode,
+                                 using_torch_2)
 from composer.utils.object_store import (LibcloudObjectStore, ObjectStore, ObjectStoreTransientError, OCIObjectStore,
                                          S3ObjectStore, SFTPObjectStore)
 from composer.utils.retrying import retry
 from composer.utils.string_enum import StringEnum
 
-
-def warn_yahp_deprecation() -> None:
-    warnings.warn(
-        'yahp-based workflows are deprecated and will be removed in a future release. Please'
-        'migrate to using other configuration managers and create the Trainer objects directly.'
-        'v0.10 will be the last release to support yahp.',
-        DeprecationWarning,
-        stacklevel=2)
-
-
 __all__ = [
     'ensure_tuple',
     'get_free_tcp_port',
     'map_collection',
     'IteratorFileStream',
     'FORMAT_NAME_WITH_DIST_AND_TIME_TABLE',
     'FORMAT_NAME_WITH_DIST_TABLE',
@@ -84,8 +74,9 @@
     'is_tpu_installed',
     'ExportFormat',
     'Transform',
     'export_with_logger',
     'extract_hparams',
     'convert_nested_dict_to_flat_dict',
     'convert_flat_dict_to_nested_dict',
+    'using_torch_2',
 ]
```

### Comparing `composer-0.13.5/composer/utils/auto_log_hparams.py` & `composer-0.14.0/composer/utils/auto_log_hparams.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Returns:
         Dict[str, Any]: A nested dictionary with every element of locals_dict mapped to its
             value or to another sub_dict.
     """
     hparams = {}
     for k, v in locals_dict.items():
-        if k.startswith('_') or k == 'self':
+        if k.startswith('_') or k == 'self' or type(v) is type:
             continue
         hparams_to_add = _grab_hparams(v)
         hparams[k] = hparams_to_add
     return hparams
 
 
 def _grab_hparams(obj) -> Any:
```

### Comparing `composer-0.13.5/composer/utils/batch_helpers.py` & `composer-0.14.0/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/checkpoint.py` & `composer-0.14.0/composer/utils/checkpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,26 +187,26 @@
         algorithm_passes (List[AlgorithmPass], optional): A list of algorithm passes to apply to autoloaded algorithms
             to sort them into the correct order. (default: ``None``)
 
     Returns:
         Optional[List[Dict[str, Any]]]: The RNG state dicts, indexed by global rank, if
             :attr:`load_weights_only` is not None. Otherwise, None.
     """
-    # download the checkpoint to the node-local folder
+    # Download the checkpoint to the node-local folder
     log.debug('Loading checkpoint at %s', path)
     # Each node gets one unique folder to store checkpoints that is shared amongst all local ranks in that node.
     # If fsdp sharded state_dicts is enabled then EVERY rank gets a unique checkpoint folder.
-    tempdir_ctx = (tempfile.TemporaryDirectory() if (state.fsdp_sharded_state_dict_enabled or
-                                                     dist.get_local_rank() == 0) else contextlib.nullcontext(None))
+    needs_unique_checkpoint_folder = state.fsdp_sharded_state_dict_enabled or dist.get_local_rank() == 0
+    tempdir_ctx = tempfile.TemporaryDirectory() if needs_unique_checkpoint_folder else contextlib.nullcontext(None)
     with tempdir_ctx as tempdir:
         try:
             # Get the path to the proper checkpoint folder corresponding to the current rank's node.
             # If fsdp_sharded_state_dict_enabled then just use that rank's unique tempdir.
-            node_checkpoint_folder = (tempdir if state.fsdp_sharded_state_dict_enabled else
-                                      _get_node_checkpoint_download_folder(tempdir))
+            node_checkpoint_folder = (tempdir
+                                      if state.fsdp_sharded_state_dict_enabled else _get_local_rank_zero_path(tempdir))
             assert node_checkpoint_folder is not None
 
             composer_states_filepath, extracted_checkpoint_folder, extracted_rank_n = download_checkpoint(
                 path=path,
                 node_checkpoint_folder=node_checkpoint_folder,
                 object_store=object_store,
                 progress_bar=progress_bar,
@@ -230,15 +230,15 @@
             # be a shared resource between nodes.
             dist.barrier()
 
     log.info('%s loaded from %s', 'Model weights' if load_weights_only else 'Trainer checkpoint', path)
     return rng_state_dicts
 
 
-def _get_node_checkpoint_download_folder(path: Optional[str]) -> str:
+def _get_local_rank_zero_path(path: Optional[str]) -> str:
     """Broadcasts the ``path`` from the LOCAL rank zero to all LOCAL ranks."""
     local_rank_zero = dist.get_local_world_size() * dist.get_node_rank()
     paths = dist.all_gather_object(path)
     local_rank_zero_path = paths[local_rank_zero]
     assert local_rank_zero_path is not None, 'local rank zero provides the path'
     return local_rank_zero_path
 
@@ -317,31 +317,30 @@
                         extracted_rank_n = True
                 except FileNotFoundError:
                     # this will happen most of the time (i.e. whenever deepspeed
                     # is not being used) so not logging anything
                     pass
 
     finally:
-        # Wait for all checkpoints on the node to finish downloading
-        # First we wait for the local rank 0 to finish its download. This prevents timeouts
-        # in cases where the local rank 0 is downloading a monolithic checkpoint, and so takes
-        # much longer than the other ranks, which have nothing to download
-        # Putting the barrier in a finally so the rank will always block on the barrier,
-        # even if it has an exception.
-        # Any exception will be re-raised after the barrier passes. The launcher script
-        # will detect the process crash and terminate the other ranks
-
-        signal_file_path = os.path.join(node_checkpoint_folder, '.local_rank0_completed')
-        if dist.get_local_rank() == 0:
-            with open(signal_file_path, 'wb') as f:
-                f.write(b'local_rank0_completed')
-        dist.local_rank_zero_download_and_wait(signal_file_path)
-        if dist.get_local_rank() == 0:
-            os.remove(signal_file_path)
+        # Use busy wait to avoid timeouts on large downloads for non-sharded checkpoints
+        if not checkpoint_is_sharded:
+            signal_file_path = os.path.join(node_checkpoint_folder, '.local_rank0_completed')
+            if dist.get_local_rank() == 0:
+                with open(signal_file_path, 'wb') as f:
+                    f.write(b'local_rank0_completed')
+
+            # Avoid the collective call until the local rank zero has finished trying to download the
+            # checkpoint so that we don't timeout for large downloads. This syncs all processes on the
+            # node
+            with dist.local_rank_zero_download_and_wait(signal_file_path):
+                # Then, wait to ensure every node has finished downloading the checkpoint
+                dist.barrier()
 
+            if dist.get_local_rank() == 0:
+                os.remove(signal_file_path)
         dist.barrier()
 
     return composer_states_filepath, extracted_checkpoint_folder, extracted_rank_n
 
 
 def _flatten_keys(obj: Any, paths: List[str], existing_path: str):
     """Recursively flatten the keys of a dictionary or list into a set of paths."""
@@ -480,14 +479,31 @@
     if not load_weights_only:
         state.load_state_dict(
             state_dict['state'],
             logger,
             exclude_algorithms=exclude_algorithms,
             algorithm_passes=algorithm_passes,
         )
+        step_to_resume_from = state.timestamp.batch.value
+        max_step_to_resume_from = state.device.tensor_to_device(
+            torch.tensor(state.timestamp.batch.value, dtype=torch.int64))
+        min_step_to_resume_from = state.device.tensor_to_device(
+            torch.tensor(state.timestamp.batch.value, dtype=torch.int64))
+        dist.all_reduce(max_step_to_resume_from, reduce_operation='MAX')
+        dist.all_reduce(min_step_to_resume_from, reduce_operation='MIN')
+        if max_step_to_resume_from.data != min_step_to_resume_from.data:
+            raise RuntimeError(
+                textwrap.dedent(
+                    f'Timestamp mismatch error: batch to resume from {step_to_resume_from} is not the same on all ranks. '
+                    'This usually occurs when at least one rank fails to save the last checkpoint '
+                    'while using sharded checkpointing + autoresume. '
+                    'Please manually resume by disabling autoresume and explicitly setting load_path '
+                    'to the most recent checkpoints that all ranks have saved. '
+                    'E.g. for the 10th batch: trainer = Trainer(autoresume=False, load_path="/path/to/checkpoint/ba10-rank{rank}.pt", ...). '
+                    'Remember to keep the {rank} placeholder!'))
         return state_dict['rng']
 
 
 def save_checkpoint(
     state: State,
     filename: str = 'ep{epoch}-ba{batch}-rank{rank}',
     *,
```

### Comparing `composer-0.13.5/composer/utils/collect_env.py` & `composer-0.14.0/composer/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/device.py` & `composer-0.14.0/composer/utils/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/dist.py` & `composer-0.14.0/composer/utils/dist.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/file_helpers.py` & `composer-0.14.0/composer/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/fx_utils.py` & `composer-0.14.0/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/import_helpers.py` & `composer-0.14.0/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/inference.py` & `composer-0.14.0/composer/utils/inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     save_format: Union[str, ExportFormat],
     save_path: str,
     save_object_store: Optional[ObjectStore] = None,
     sample_input: Optional[Any] = None,
     dynamic_axes: Optional[Any] = None,
     surgery_algs: Optional[Union[Callable[[nn.Module], nn.Module], Sequence[Callable[[nn.Module], nn.Module]]]] = None,
     transforms: Optional[Sequence[Transform]] = None,
+    onnx_opset_version: Optional[int] = None,
     load_path: Optional[str] = None,
     load_object_store: Optional[ObjectStore] = None,
     load_strict: bool = False,
 ) -> None:
     """Export a model for inference.
 
     Args:
@@ -116,14 +117,16 @@
             for exporting models using older versions of PyTorch when types cannot be inferred.
         surgery_algs (Union[Callable, Sequence[Callable]], optional): Algorithms that should be applied to the model
             before loading a checkpoint. Each should be callable that takes a model and returns None.
             ``surgery_algs`` are applied before ``transforms``. (default: ``None``)
         transforms (Sequence[Transform], optional): transformations (usually optimizations) that should
             be applied to the model. Each Transform should be a callable that takes a model and returns a modified model.
             ``transforms`` are applied after ``surgery_algs``. (default: ``None``)
+        onnx_opset_version (int, optional): The opset version ONNX should use for exporting. Only used if save_format is ``"onnx"``.
+            Defaults to Pytorch's default torch.onnx.export opset version, which changes by PyTorch version. (default: ``None``)
         load_path (str): The path to an existing checkpoint file.
             It can be a path to a file on the local disk, a URL, or if ``load_object_store`` is set, the object name
             for a checkpoint in a cloud bucket. For example, run_name/checkpoints/ep0-ba4-rank0. (default: ``None``)
         load_object_store (ObjectStore, optional): If the ``load_path`` is in an object name  in a cloud bucket
             (i.e. AWS S3 or Google Cloud Storage), an instance of
             :class:`~.ObjectStore` which will be used to retreive the checkpoint.
             Otherwise, if the checkpoint is a local filepath, set to ``None``. (default: ``None``)
@@ -237,15 +240,15 @@
                 torch.onnx.export(
                     model,
                     sample_input,
                     local_save_path,
                     input_names=input_names,
                     output_names=['output'],
                     dynamic_axes=dynamic_axes,
-                    opset_version=13,
+                    opset_version=onnx_opset_version,
                 )
 
             # upload if required.
             if is_remote_store:
                 save_object_store.upload_object(save_path, local_save_path)
```

### Comparing `composer-0.13.5/composer/utils/iter_helpers.py` & `composer-0.14.0/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/misc.py` & `composer-0.14.0/composer/utils/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """Miscellaneous Helpers."""
 
 import socket
 from contextlib import contextmanager
 from typing import Type
 
 import torch
+from packaging import version
 from torch.nn.parallel import DistributedDataParallel
 
 __all__ = [
     'is_model_deepspeed', 'is_model_fsdp', 'is_notebook', 'warning_on_one_line', 'get_free_tcp_port', 'model_eval_mode'
 ]
 
 
@@ -30,20 +31,23 @@
     return isinstance(model, DistributedDataParallel)
 
 
 def is_model_fsdp(model: torch.nn.Module) -> bool:
     """Whether ``model`` is an instance of a :class:`.FullyShardedDataParallel`."""
     try:
         from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-        is_fsdp = False
+
+        if isinstance(model, FSDP):
+            return True
+
         # Check if model is wrapped with FSDP
         for _, obj in model.named_children():
             if isinstance(obj, FSDP):
-                is_fsdp = True
-        return is_fsdp
+                return True
+        return False
     except ImportError:
         return False
 
 
 def is_notebook():
     """Whether Composer is running in a IPython/Jupyter Notebook."""
     try:
@@ -74,7 +78,16 @@
     """Set model.eval() for context duration, restoring model status at end."""
     is_training = model.training
     try:
         model.eval()
         yield
     finally:
         model.train(mode=is_training)
+
+
+def using_torch_2() -> bool:
+    """Check the PyTorch version and compared it with version 2.0.0.
+
+    Returns:
+        bool: Return True if current version is greater than or equal to 2.0.0 else False
+    """
+    return version.parse(torch.__version__) >= version.parse('2.0.0')
```

### Comparing `composer-0.13.5/composer/utils/module_surgery.py` & `composer-0.14.0/composer/utils/module_surgery.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,15 +367,17 @@
     added_params = _ordered_diff(new_values, old_values)
 
     if len(removed_params) == 0 and len(added_params) == 0:
         return  # nothing to do
 
     # rip out the removed_params' states from the optimizer
     for p in removed_params:
-        if _tensor_in(p, opt.state):  # only true after training starts
+        # Only true after training starts
+        # Note: it appears that opt.state is a dict whose keys _might_ be tensors
+        if _tensor_in(p, opt.state):  # type: ignore
             opt.state.pop(p)
 
     if len(opt.param_groups) == 1:
         group_idx = 0
     else:
         # if there is more than one group, use the ripped out parameters to infer the group
         # to add the new parameters into
```

### Comparing `composer-0.13.5/composer/utils/object_store/__init__.py` & `composer-0.14.0/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/object_store/libcloud_object_store.py` & `composer-0.14.0/composer/utils/object_store/libcloud_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/object_store/object_store.py` & `composer-0.14.0/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/object_store/oci_object_store.py` & `composer-0.14.0/composer/utils/object_store/oci_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/object_store/s3_object_store.py` & `composer-0.14.0/composer/utils/object_store/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/object_store/sftp_object_store.py` & `composer-0.14.0/composer/utils/object_store/sftp_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/reproducibility.py` & `composer-0.14.0/composer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/retrying.py` & `composer-0.14.0/composer/utils/retrying.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer/utils/string_enum.py` & `composer-0.14.0/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/composer.egg-info/PKG-INFO` & `composer-0.14.0/composer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.13.5
+Version: 0.14.0
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: dev
 Provides-Extra: health_checker
+Provides-Extra: slack
 Provides-Extra: deepspeed
 Provides-Extra: wandb
 Provides-Extra: comet_ml
 Provides-Extra: tensorboard
 Provides-Extra: unet
 Provides-Extra: vit
 Provides-Extra: timm
@@ -26,14 +27,15 @@
 Provides-Extra: sentencepiece
 Provides-Extra: mlperf
 Provides-Extra: streaming
 Provides-Extra: libcloud
 Provides-Extra: oci
 Provides-Extra: onnx
 Provides-Extra: mlflow
+Provides-Extra: mcli
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/composer#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg" width="50%"/>
@@ -42,31 +44,31 @@
 </p>
 
 <h2><p align="center">A PyTorch Library for Efficient Neural Network Training</p></h2>
 <h3><p align="center">Train Faster, Reduce Cost, Get Better Models</p></h3>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
-- <a href="https://docs.mosaicml.com/en/stable/getting_started/installation.html">[Getting Started]</a>
-- <a href="https://docs.mosaicml.com/">[Docs]</a>
-- <a href="https://docs.mosaicml.com/en/stable/method_cards/methods_overview.html">[Methods]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/en/stable/getting_started/installation.html">[Getting Started]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/">[Docs]</a>
+- <a href="https://docs.mosaicml.com/projects/composer/en/stable/method_cards/methods_overview.html">[Methods]</a>
 - <a href="https://www.mosaicml.com/team">[We're Hiring!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/mosaicml/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mosaicml">
     </a>
     <a href="https://pypi.org/project/mosaicml/">
         <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/mosaicml">
     </a>
     <a href="https://pepy.tech/project/mosaicml/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
-    <a href="https://docs.mosaicml.com/en/stable/">
+    <a href="https://docs.mosaicml.com/projects/composer/en/stable/">
         <img alt="Documentation" src="https://readthedocs.org/projects/composer/badge/?version=stable">
     </a>
     <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/composer/blob/dev/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
@@ -125,15 +127,15 @@
 You can use Composer's speedup methods in two ways:
 
 * Through a standalone **Functional API** (similar to `torch.nn.functional`) that allows you to integrate them into your existing training code.
 * Using Composer's built-in **Trainer**, which is designed to be performant and automatically takes care of the details of using speedup methods.
 
 ### Example: Functional API [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb)
 
-Integrate our speedup methods into your training loop with just a few lines of code, and see the results. Here we easily apply [BlurPool](https://docs.mosaicml.com/en/stable/method_cards/blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/en/stable/method_cards/squeeze_excite.html):
+Integrate our speedup methods into your training loop with just a few lines of code, and see the results. Here we easily apply [BlurPool](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/squeeze_excite.html):
 
 <!-- begin_example_1 --->
 ```python
 import composer.functional as cf
 from torchvision import models
 
 my_model = models.resnet18()
@@ -142,24 +144,24 @@
 cf.apply_blurpool(my_model)
 cf.apply_squeeze_excite(my_model)
 
 # your own training code starts here
 ```
 <!-- end_example_1 --->
 
-For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/en/latest/functional_api.html).
+For more examples, see the [Composer Functional API Colab notebook](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/projects/composer/en/latest/functional_api.html).
 
 ### Example: Trainer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/getting_started.ipynb)
 
 For the best experience and the most efficient possible training, we recommend using Composer's built-in trainer, which automatically takes care of the details of using speedup methods and provides useful abstractions that facilitate rapid experimentation.
 
 <!-- begin_example_2 --->
 <!--pytest.mark.gpu-->
 <!--pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')-->
-<!--
+<!--pytest.mark.filterwarnings('ignore:Cannot split tensor of length .* into batches of size 128.*:UserWarning')-->
 ```python
 import torch
 
 # adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
 torch.use_deterministic_algorithms(False)
 
 ```
@@ -190,31 +192,31 @@
         LabelSmoothing(smoothing=0.1),
     ]
 )
 trainer.fit()
 ```
 <!-- end_example_2 -->
 
-Composer's built-in [trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html) makes it easy to **add multiple speedup methods in a single line of code!**
+Composer's built-in [trainer](https://docs.mosaicml.com/projects/composer/en/stable/trainer/using_the_trainer.html) makes it easy to **add multiple speedup methods in a single line of code!**
 Trying out new methods or combinations of methods is as easy as changing a single list.
 
-Here are some examples of methods available in Composer ([_see here for the full list_](https://docs.mosaicml.com/en/latest/trainer/algorithms.html)):
+Here are some examples of methods available in Composer ([_see here for the full list_](https://docs.mosaicml.com/projects/composer/en/latest/trainer/algorithms.html)):
 
 Name|Attribution|tl;dr|Example Benchmark|Speed Up*|
 ----|-----------|-----|---------|---------|
 [Alibi](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/alibi)|[Press et al, 2021](https://arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-2|1.5x
 [BlurPool](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter before every downsampling operation.|ResNet-101|1.2x
 [ChannelsLast](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/channels_last)|[PyTorch](https://pytorch.org/tutorials/intermediate/memory_format_tutorial.html)|Uses channels last memory format (NHWC).|ResNet-101|1.5x
-[CutOut](https://docs.mosaicml.com/en/latest/method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
+[CutOut](https://docs.mosaicml.com/projects/composer/en/latest/method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
 [LabelSmoothing](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/1512.00567)|Smooths the labels with a uniform prior|ResNet-101|1.5x
 [MixUp](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/mixup)|[Zhang et al, 2017](https://arxiv.org/abs/1710.09412)|Blends pairs of examples and labels.|ResNet-101|1.5x
 [RandAugment](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/randaugment)|[Cubuk et al, 2020](https://openaccess.thecvf.com/content_CVPRW_2020/html/w40/Cubuk_Randaugment_Practical_Automated_Data_Augmentation_With_a_Reduced_Search_Space_CVPRW_2020_paper.html)|Applies a series of random augmentations to each image.|ResNet-101|1.3x
 [SAM](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/sam)|[Foret et al, 2021](https://arxiv.org/abs/2010.01412)|An optimization strategy that seeks flatter minima.|ResNet-101|1.4x
 [SeqLengthWarmup](https://github.com/mosaicml/composer/tree/dev/composer/algorithms/seq_length_warmup)|[Li et al, 2021](https://arxiv.org/abs/2108.06084)|Progressively increase sequence length.|GPT-2|1.2x
-[Stochastic Depth](https://docs.mosaicml.com/en/latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version that randomly drops the layer or samples during training|ResNet-101|1.1x
+[Stochastic Depth](https://docs.mosaicml.com/projects/composer/en/latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version that randomly drops the layer or samples during training|ResNet-101|1.1x
 <p align="right">* = time-to-train to the same quality as the baseline.</p>
 
 ## 🛠 Building Speedup Recipes
 
 Given two methods that speed up training by 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not necessarily.
 They may optimize the [same part of the training process](https://en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they may even interact in ways that prove detrimental.
 Determining which methods to compose together isn't as simple as assembling a set of methods that perform best individually.
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: composer Version: 0.13.5 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.14.0 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
-health_checker Provides-Extra: deepspeed Provides-Extra: wandb Provides-Extra:
-comet_ml Provides-Extra: tensorboard Provides-Extra: unet Provides-Extra: vit
-Provides-Extra: timm Provides-Extra: coco Provides-Extra: nlp Provides-Extra:
-sentencepiece Provides-Extra: mlperf Provides-Extra: streaming Provides-Extra:
-libcloud Provides-Extra: oci Provides-Extra: onnx Provides-Extra: mlflow
-Provides-Extra: all License-File: LICENSE
+health_checker Provides-Extra: slack Provides-Extra: deepspeed Provides-Extra:
+wandb Provides-Extra: comet_ml Provides-Extra: tensorboard Provides-Extra: unet
+Provides-Extra: vit Provides-Extra: timm Provides-Extra: coco Provides-Extra:
+nlp Provides-Extra: sentencepiece Provides-Extra: mlperf Provides-Extra:
+streaming Provides-Extra: libcloud Provides-Extra: oci Provides-Extra: onnx
+Provides-Extra: mlflow Provides-Extra: mcli Provides-Extra: all License-File:
+LICENSE
   [https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg]
 ***** A PyTorch Library for Efficient Neural Network Training *****
 **** Train Faster, Reduce Cost, Get Better Models ****
 *** [Website] - [Getting_Started] - [Docs] - [Methods] - [We're_Hiring!] ***
 [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads] [Documentation] [Chat_@
                                Slack] [License]
 
@@ -49,78 +50,80 @@
 your existing training code. * Using Composer's built-in **Trainer**, which is
 designed to be performant and automatically takes care of the details of using
 speedup methods. ### Example: Functional API [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 functional_api.ipynb) Integrate our speedup methods into your training loop
 with just a few lines of code, and see the results. Here we easily apply
-[BlurPool](https://docs.mosaicml.com/en/stable/method_cards/blurpool.html) and
-[SqueezeExcite](https://docs.mosaicml.com/en/stable/method_cards/
-squeeze_excite.html):  ```python import composer.functional as cf from
-torchvision import models my_model = models.resnet18() # add blurpool and
-squeeze excite layers cf.apply_blurpool(my_model) cf.apply_squeeze_excite
-(my_model) # your own training code starts here ```  For more examples, see the
-[Composer Functional API Colab notebook](https://colab.research.google.com/
-github/mosaicml/composer/blob/dev/examples/functional_api.ipynb) and
-[Functional API guide](https://docs.mosaicml.com/en/latest/
-functional_api.html). ### Example: Trainer [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+[BlurPool](https://docs.mosaicml.com/projects/composer/en/stable/method_cards/
+blurpool.html) and [SqueezeExcite](https://docs.mosaicml.com/projects/composer/
+en/stable/method_cards/squeeze_excite.html):  ```python import
+composer.functional as cf from torchvision import models my_model =
+models.resnet18() # add blurpool and squeeze excite layers cf.apply_blurpool
+(my_model) cf.apply_squeeze_excite(my_model) # your own training code starts
+here ```  For more examples, see the [Composer Functional API Colab notebook]
+(https://colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
+functional_api.ipynb) and [Functional API guide](https://docs.mosaicml.com/
+projects/composer/en/latest/functional_api.html). ### Example: Trainer [![Open
+In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/mosaicml/composer/blob/dev/examples/
 getting_started.ipynb) For the best experience and the most efficient possible
 training, we recommend using Composer's built-in trainer, which automatically
 takes care of the details of using speedup methods and provides useful
-abstractions that facilitate rapid experimentation.      ```python from
+abstractions that facilitate rapid experimentation.     ```python import torch
+# adaptive_avg_pool2d_backward_cuda in mnist_classifier is not deterministic
+torch.use_deterministic_algorithms(False) ``` -->  ```python from
 torch.utils.data import DataLoader from torchvision import datasets, transforms
 from composer import Trainer from composer.algorithms import ChannelsLast,
 CutMix, LabelSmoothing from composer.models import mnist_model transform =
 transforms.Compose([transforms.ToTensor()]) train_dataset = datasets.MNIST
 ("data", download=True, train=True, transform=transform) eval_dataset =
 datasets.MNIST("data", download=True, train=False, transform=transform)
 train_dataloader = DataLoader(train_dataset, batch_size=128) eval_dataloader =
 DataLoader(eval_dataset, batch_size=128) trainer = Trainer( model=mnist_model
 (), train_dataloader=train_dataloader, eval_dataloader=eval_dataloader,
 max_duration="1ep", algorithms=[ ChannelsLast(), CutMix(alpha=1.0),
 LabelSmoothing(smoothing=0.1), ] ) trainer.fit() ```  Composer's built-in
-[trainer](https://docs.mosaicml.com/en/stable/trainer/using_the_trainer.html)
-makes it easy to **add multiple speedup methods in a single line of code!**
-Trying out new methods or combinations of methods is as easy as changing a
-single list. Here are some examples of methods available in Composer ([_see
-here for the full list_](https://docs.mosaicml.com/en/latest/trainer/
-algorithms.html)): Name|Attribution|tl;dr|Example Benchmark|Speed Up*| ----|---
---------|-----|---------|---------| [Alibi](https://github.com/mosaicml/
-composer/tree/dev/composer/algorithms/alibi)|[Press et al, 2021](https://
-arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-2|1.5x [BlurPool]
-(https://github.com/mosaicml/composer/tree/dev/composer/algorithms/blurpool)|
-[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an anti-aliasing filter
-before every downsampling operation.|ResNet-101|1.2x [ChannelsLast](https://
-github.com/mosaicml/composer/tree/dev/composer/algorithms/channels_last)|
-[PyTorch](https://pytorch.org/tutorials/intermediate/
+[trainer](https://docs.mosaicml.com/projects/composer/en/stable/trainer/
+using_the_trainer.html) makes it easy to **add multiple speedup methods in a
+single line of code!** Trying out new methods or combinations of methods is as
+easy as changing a single list. Here are some examples of methods available in
+Composer ([_see here for the full list_](https://docs.mosaicml.com/projects/
+composer/en/latest/trainer/algorithms.html)): Name|Attribution|tl;dr|Example
+Benchmark|Speed Up*| ----|-----------|-----|---------|---------| [Alibi](https:
+//github.com/mosaicml/composer/tree/dev/composer/algorithms/alibi)|[Press et
+al, 2021](https://arxiv.org/abs/2108.12409)|Replace attention with AliBi.|GPT-
+2|1.5x [BlurPool](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/blurpool)|[Zhang, 2019](https://arxiv.org/abs/1904.11486)|Applies an
+anti-aliasing filter before every downsampling operation.|ResNet-101|1.2x
+[ChannelsLast](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/channels_last)|[PyTorch](https://pytorch.org/tutorials/intermediate/
 memory_format_tutorial.html)|Uses channels last memory format (NHWC).|ResNet-
-101|1.5x [CutOut](https://docs.mosaicml.com/en/latest/method_cards/
-cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/1708.04552)|Randomly
-erases rectangular blocks from the image.|ResNet-101|1.2x [LabelSmoothing]
-(https://github.com/mosaicml/composer/tree/dev/composer/algorithms/
-label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/
+101|1.5x [CutOut](https://docs.mosaicml.com/projects/composer/en/latest/
+method_cards/cutout.html)|[DeVries et al, 2017](https://arxiv.org/abs/
+1708.04552)|Randomly erases rectangular blocks from the image.|ResNet-101|1.2x
+[LabelSmoothing](https://github.com/mosaicml/composer/tree/dev/composer/
+algorithms/label_smoothing)|[Szegedy et al, 2015](https://arxiv.org/abs/
 1512.00567)|Smooths the labels with a uniform prior|ResNet-101|1.5x [MixUp]
 (https://github.com/mosaicml/composer/tree/dev/composer/algorithms/mixup)|
 [Zhang et al, 2017](https://arxiv.org/abs/1710.09412)|Blends pairs of examples
 and labels.|ResNet-101|1.5x [RandAugment](https://github.com/mosaicml/composer/
 tree/dev/composer/algorithms/randaugment)|[Cubuk et al, 2020](https://
 openaccess.thecvf.com/content_CVPRW_2020/html/w40/
 Cubuk_Randaugment_Practical_Automated_Data_Augmentation_With_a_Reduced_Search_Space_CVPRW_2020_paper.html)|Applies
 a series of random augmentations to each image.|ResNet-101|1.3x [SAM](https://
 github.com/mosaicml/composer/tree/dev/composer/algorithms/sam)|[Foret et al,
 2021](https://arxiv.org/abs/2010.01412)|An optimization strategy that seeks
 flatter minima.|ResNet-101|1.4x [SeqLengthWarmup](https://github.com/mosaicml/
 composer/tree/dev/composer/algorithms/seq_length_warmup)|[Li et al, 2021]
 (https://arxiv.org/abs/2108.06084)|Progressively increase sequence length.|GPT-
-2|1.2x [Stochastic Depth](https://docs.mosaicml.com/en/latest/method_cards/
-stochastic_depth.html)|[Huang et al, 2016](https://arxiv.org/abs/
-1603.09382)|Replaces a specified layer with a stochastic version that randomly
-drops the layer or samples during training|ResNet-101|1.1x
+2|1.2x [Stochastic Depth](https://docs.mosaicml.com/projects/composer/en/
+latest/method_cards/stochastic_depth.html)|[Huang et al, 2016](https://
+arxiv.org/abs/1603.09382)|Replaces a specified layer with a stochastic version
+that randomly drops the layer or samples during training|ResNet-101|1.1x
                          * = time-to-train to the same quality as the baseline.
 ## ð  Building Speedup Recipes Given two methods that speed up training by
 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not
 necessarily. They may optimize the [same part of the training process](https://
 en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they
 may even interact in ways that prove detrimental. Determining which methods to
 compose together isn't as simple as assembling a set of methods that perform
```

### Comparing `composer-0.13.5/composer.egg-info/SOURCES.txt` & `composer-0.14.0/composer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 composer/algorithms/utils/__init__.py
 composer/algorithms/utils/augmentation_common.py
 composer/algorithms/utils/augmentation_primitives.py
 composer/algorithms/weight_standardization/__init__.py
 composer/algorithms/weight_standardization/metadata.json
 composer/algorithms/weight_standardization/weight_standardization.py
 composer/callbacks/__init__.py
+composer/callbacks/activation_monitor.py
 composer/callbacks/checkpoint_saver.py
 composer/callbacks/early_stopper.py
 composer/callbacks/export_for_inference.py
 composer/callbacks/health_checker.py
 composer/callbacks/image_visualizer.py
 composer/callbacks/lr_monitor.py
 composer/callbacks/memory_monitor.py
@@ -166,16 +167,18 @@
 composer/loggers/cometml_logger.py
 composer/loggers/console_logger.py
 composer/loggers/file_logger.py
 composer/loggers/in_memory_logger.py
 composer/loggers/logger.py
 composer/loggers/logger_destination.py
 composer/loggers/mlflow_logger.py
+composer/loggers/mosaicml_logger.py
 composer/loggers/progress_bar_logger.py
 composer/loggers/remote_uploader_downloader.py
+composer/loggers/slack_logger.py
 composer/loggers/tensorboard_logger.py
 composer/loggers/wandb_logger.py
 composer/loss/__init__.py
 composer/loss/loss.py
 composer/loss/utils.py
 composer/metrics/__init__.py
 composer/metrics/map.py
```

### Comparing `composer-0.13.5/composer.egg-info/requires.txt` & `composer-0.14.0/composer.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,158 +1,164 @@
 pyyaml<7,>=6.0
 tqdm<5,>=4.62.3
 torchmetrics<0.11.4,>=0.10.0
 torch_optimizer<0.4,>=0.3.0
-torchvision<0.15,>=0.11.0
-torch<1.14,>=1.10.0
+torchvision<0.16,>=0.11.0
+torch<2.1,>=1.10.0
 requests<3,>=2.26.0
-numpy<1.23.0,>=1.21.5
+numpy<1.25.0,>=1.21.5
 psutil<6,>=5.8.0
 coolname<3,>=1.1.0
 tabulate==0.9.0
 py-cpuinfo<10,>=8.0.0
 packaging<23,>=21.3.0
 importlib-metadata<7,>=5.0.0
 
 [all]
-GitPython==3.1.31
-tensorboard<3.0.0,>=2.9.1
-pycocotools<3,>=2.0.4
-setuptools<=59.5.0
-jupyter==1.0.0
-moto[s3]<5,>=4.0.1
 fasteners==0.18
-coverage[toml]==7.2.1
-timm<0.6,>=0.5.4
-pytest_codeblocks==0.16.1
-apache-libcloud<4,>=3.3.1
-oci<3.0.0,>=2.88.2
-custom_inherit==2.4.1
-recommonmark==0.7.1
-junitparser==2.8.0
-docutils==0.17.1
+jupyter==1.0.0
 myst-parser==0.16.1
-ipykernel==6.20.1
-pypandoc==1.11
-sphinxcontrib.katex==0.9.4
+timm<0.6,>=0.5.4
+sphinxext.opengraph==0.8.2
+mosaicml-streaming<1.0
+pycocotools<3,>=2.0.4
+mlflow<3.0,>=2.0.1
 sphinx==4.4.0
-testbook==0.4.2
-sphinxemoji==0.2.0
-onnx<2,>=1.12.0
-pytest-httpserver<1.1,>=1.0.4
-vit_pytorch==0.35.8
-paramiko<3,>=2.11.0
-nbsphinx==0.8.12
-sphinx-copybutton==0.5.0
-scikit-learn<2,>=1.0.1
-py-cpuinfo<10,>=8.0.0
-onnxruntime<2,>=1.12.1
-furo==2022.9.29
-sphinx_markdown_tables==0.0.17
+yamllint==1.31.0
 mock-ssh-server==0.9.1
-monai<1.2,>=0.9.1
-mosaicml-streaming<1.0
-traitlets==5.9.0
-wandb<0.14,>=0.13.2
-yamllint==1.28.0
-sphinxcontrib-images==0.9.4
-sphinxext.opengraph==0.7.4
-pynvml<12,>=11.5.0
-deepspeed==0.7.7
+sphinx_markdown_tables==0.0.17
+deepspeed==0.8.3
+junitparser==3.0.0
 sphinx-argparse==0.4.0
+paramiko<3,>=2.11.0
+recommonmark==0.7.1
 comet_ml<4.0.0,>=3.31.12
-mlflow<3.0,>=2.0.1
-sentencepiece==0.1.97
-pandoc==2.3
+monai<1.2,>=0.9.1
+slack_sdk<4,>=3.19.5
 toml==0.10.2
-sphinx_panels==0.6.0
-ipython==8.11.0
+vit_pytorch==0.35.8
+onnxruntime<2,>=1.12.1
+sphinx-copybutton==0.5.2
+sentencepiece==0.1.98
+oci<3.0.0,>=2.88.2
+traitlets==5.9.0
+pytest-httpserver<1.1,>=1.0.4
+datasets<3,>=2.4
+mosaicml-cli<0.4,>=0.3.6
+tensorboard<3.0.0,>=2.9.1
+pynvml<12,>=11.5.0
+transformers<4.29,>=4.11
+pypandoc==1.11
 boto3<2,>=1.21.45
-pytest==7.2.2
+ipykernel==6.22.0
+onnx<2,>=1.12.0
 pre-commit<3,>=2.18.1
-transformers<4.27,>=4.11
-slack_sdk<4,>=3.19.5
-datasets<3,>=2.4
+sphinx_panels==0.6.0
+sphinxemoji==0.2.0
+furo==2022.9.29
+pytest==7.3.1
+apache-libcloud<4,>=3.3.1
 cryptography==38.0.4
+custom_inherit==2.4.1
+setuptools<=59.5.0
+wandb<0.16,>=0.13.2
+sphinxcontrib.katex==0.9.4
+docutils==0.17.1
+GitPython==3.1.31
+sphinxcontrib-images==0.9.4
+coverage[toml]==7.2.5
+testbook==0.4.2
+pytest_codeblocks==0.16.1
+nbsphinx==0.9.1
+pandoc==2.3
+scikit-learn<2,>=1.0.1
+py-cpuinfo<10,>=8.0.0
+moto[s3]<5,>=4.0.1
+ipython==8.11.0
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [comet_ml]
 comet_ml<4.0.0,>=3.31.12
 
 [deepspeed]
-deepspeed==0.7.7
+deepspeed==0.8.3
 
 [dev]
 custom_inherit==2.4.1
-junitparser==2.8.0
-coverage[toml]==7.2.1
+junitparser==3.0.0
+coverage[toml]==7.2.5
 fasteners==0.18
-pytest==7.2.2
+pytest==7.3.1
 toml==0.10.2
 ipython==8.11.0
-ipykernel==6.20.1
+ipykernel==6.22.0
 jupyter==1.0.0
-yamllint==1.28.0
+yamllint==1.31.0
 recommonmark==0.7.1
 sphinx==4.4.0
 pre-commit<3,>=2.18.1
 docutils==0.17.1
 sphinx_markdown_tables==0.0.17
 sphinx-argparse==0.4.0
 sphinxcontrib.katex==0.9.4
-sphinxext.opengraph==0.7.4
+sphinxext.opengraph==0.8.2
 sphinxemoji==0.2.0
 furo==2022.9.29
-sphinx-copybutton==0.5.0
+sphinx-copybutton==0.5.2
 testbook==0.4.2
 myst-parser==0.16.1
 sphinx_panels==0.6.0
 sphinxcontrib-images==0.9.4
 pytest_codeblocks==0.16.1
 traitlets==5.9.0
-nbsphinx==0.8.12
+nbsphinx==0.9.1
 pandoc==2.3
 pypandoc==1.11
 GitPython==3.1.31
 moto[s3]<5,>=4.0.1
 mock-ssh-server==0.9.1
 cryptography==38.0.4
 pytest-httpserver<1.1,>=1.0.4
 setuptools<=59.5.0
 
 [health_checker]
 pynvml<12,>=11.5.0
-slack_sdk<4,>=3.19.5
 
 [libcloud]
 apache-libcloud<4,>=3.3.1
 
+[mcli]
+mosaicml-cli<0.4,>=0.3.6
+
 [mlflow]
 mlflow<3.0,>=2.0.1
 
 [mlperf]
 py-cpuinfo<10,>=8.0.0
 
 [nlp]
-transformers<4.27,>=4.11
+transformers<4.29,>=4.11
 datasets<3,>=2.4
 
 [oci]
 oci<3.0.0,>=2.88.2
 
 [onnx]
 onnx<2,>=1.12.0
 onnxruntime<2,>=1.12.1
 
 [sentencepiece]
-sentencepiece==0.1.97
+sentencepiece==0.1.98
+
+[slack]
+slack_sdk<4,>=3.19.5
 
 [streaming]
 mosaicml-streaming<1.0
 boto3<2,>=1.21.45
 paramiko<3,>=2.11.0
 
 [tensorboard]
@@ -165,8 +171,8 @@
 monai<1.2,>=0.9.1
 scikit-learn<2,>=1.0.1
 
 [vit]
 vit_pytorch==0.35.8
 
 [wandb]
-wandb<0.14,>=0.13.2
+wandb<0.16,>=0.13.2
```

### Comparing `composer-0.13.5/pyproject.toml` & `composer-0.14.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -110,24 +110,25 @@
     'ignore:Failed to load image Python extension:UserWarning',
     # Ignore a deprecation warning in the conda build
     'ignore:distutils Version classes are deprecated:DeprecationWarning',
     # Ignore a UserWarning from TorchMetrics about potentially large memory usage when batch sizes are extremely large
     'ignore:Metric `SpearmanCorrcoef` will save all targets and predictions in the buffer:UserWarning:torchmetrics',
     # Ignore a UserWarning from torch 1.12 due to DeepSpeed's use of positional args
     'ignore:Positional args are being deprecated, use kwargs instead.*:UserWarning',
-    'ignore:yahp-based workflows are deprecated and will be removed:DeprecationWarning',
     'ignore:Torchmetrics v0.9 introduced a new argument class property:UserWarning',
     'ignore:torch.distributed._all_gather_base is a private function and will be deprecated.*:UserWarning',
     'ignore:torch.distributed._reduce_scatter_base is a private function and will be deprecated.*:UserWarning',
     # Ignore tensorboard deprecation warnings
     'ignore:Call to deprecated create function Descriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function EnumDescriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function EnumValueDescriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function FieldDescriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function FileDescriptor().*:DeprecationWarning:tensorboard',
+    # Ignore TracerWarnings for operations potentially unsupported by model tracing
+    'ignore:.*might cause the trace to be incorrect.*:Warning',
 ]
 
 # Coverage
 [tool.coverage.run]
 parallel = true
 branch = true
 relative_files = true
```

### Comparing `composer-0.13.5/setup.py` & `composer-0.14.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,18 @@
         long_description = long_description[:start] + long_description[end + len(end_tag):]
 
 install_requires = [
     'pyyaml>=6.0,<7',
     'tqdm>=4.62.3,<5',
     'torchmetrics>=0.10.0,<0.11.4',
     'torch_optimizer>=0.3.0,<0.4',
-    'torchvision>=0.11.0,<0.15',
-    'torch>=1.10.0,<1.14',
+    'torchvision>=0.11.0,<0.16',
+    'torch>=1.10.0,<2.1',
     'requests>=2.26.0,<3',
-    'numpy>=1.21.5,<1.23.0',
+    'numpy>=1.21.5,<1.25.0',
     'psutil>=5.8.0,<6',
     'coolname>=1.1.0,<3',
     'tabulate==0.9.0',  # for auto-generating tables
     'py-cpuinfo>=8.0.0,<10',
     'packaging>=21.3.0,<23',
     'importlib-metadata>=5.0.0,<7',
 ]
@@ -93,64 +93,67 @@
 extra_deps['base'] = []
 
 extra_deps['dev'] = [
     # Imports for docs builds and running tests
     # Pinning versions strictly to avoid random test failures.
     # Should manually update dependency versions occassionally.
     'custom_inherit==2.4.1',
-    'junitparser==2.8.0',
-    'coverage[toml]==7.2.1',
+    'junitparser==3.0.0',
+    'coverage[toml]==7.2.5',
     'fasteners==0.18',  # object store tests require fasteners
-    'pytest==7.2.2',
+    'pytest==7.3.1',
     'toml==0.10.2',
     'ipython==8.11.0',
-    'ipykernel==6.20.1',
+    'ipykernel==6.22.0',
     'jupyter==1.0.0',
-    'yamllint==1.28.0',
+    'yamllint==1.31.0',
     'recommonmark==0.7.1',
     'sphinx==4.4.0',
     'pre-commit>=2.18.1,<3',
     # embedding md in rst require docutils>=0.17. See
     # https://myst-parser.readthedocs.io/en/latest/sphinx/use.html?highlight=parser#include-markdown-files-into-an-rst-file
     'docutils==0.17.1',
     'sphinx_markdown_tables==0.0.17',
     'sphinx-argparse==0.4.0',
     'sphinxcontrib.katex==0.9.4',
-    'sphinxext.opengraph==0.7.4',
+    'sphinxext.opengraph==0.8.2',
     'sphinxemoji==0.2.0',
     'furo==2022.9.29',
-    'sphinx-copybutton==0.5.0',
+    'sphinx-copybutton==0.5.2',
     'testbook==0.4.2',
     'myst-parser==0.16.1',
     'sphinx_panels==0.6.0',
     'sphinxcontrib-images==0.9.4',
     'pytest_codeblocks==0.16.1',
     'traitlets==5.9.0',
-    'nbsphinx==0.8.12',
+    'nbsphinx==0.9.1',
     'pandoc==2.3',
     'pypandoc==1.11',
     'GitPython==3.1.31',
     'moto[s3]>=4.0.1,<5',
     'mock-ssh-server==0.9.1',
     'cryptography==38.0.4',
     'pytest-httpserver>=1.0.4,<1.1',
     'setuptools<=59.5.0',
 ]
 
 extra_deps['health_checker'] = {
     'pynvml>=11.5.0,<12',
+}
+
+extra_deps['slack'] = {
     'slack_sdk>=3.19.5,<4',
 }
 
 extra_deps['deepspeed'] = [
-    'deepspeed==0.7.7',
+    'deepspeed==0.8.3',
 ]
 
 extra_deps['wandb'] = [
-    'wandb>=0.13.2,<0.14',
+    'wandb>=0.13.2,<0.16',
 ]
 
 extra_deps['comet_ml'] = [
     'comet_ml>=3.31.12,<4.0.0',
 ]
 
 extra_deps['tensorboard'] = [
@@ -171,19 +174,19 @@
 ]
 
 extra_deps['coco'] = [
     'pycocotools>=2.0.4,<3',
 ]
 
 extra_deps['nlp'] = [
-    'transformers>=4.11,<4.27',
+    'transformers>=4.11,<4.29',
     'datasets>=2.4,<3',
 ]
 
-extra_deps['sentencepiece'] = ['sentencepiece==0.1.97']
+extra_deps['sentencepiece'] = ['sentencepiece==0.1.98']
 
 extra_deps['mlperf'] = [
     # TODO: use pip when available: https://github.com/mlcommons/logging/issues/218
     # "mlperf_logging @ git+https://github.com/mlperf/logging.git",
     'py-cpuinfo>=8.0.0,<10',
 ]
 
@@ -202,15 +205,21 @@
 ]
 
 extra_deps['onnx'] = [
     'onnx>=1.12.0,<2',
     'onnxruntime>=1.12.1,<2',
 ]
 
-extra_deps['mlflow'] = ['mlflow>=2.0.1,<3.0']
+extra_deps['mlflow'] = [
+    'mlflow>=2.0.1,<3.0',
+]
+
+extra_deps['mcli'] = [
+    'mosaicml-cli>=0.3.6,<0.4',
+]
 
 extra_deps['all'] = set(dep for deps in extra_deps.values() for dep in deps)
 
 composer_data_files = ['py.typed']
 composer_data_files += package_files('composer', 'yamls', '.yaml')
 composer_data_files += package_files('composer', 'algorithms', '.json')
```

### Comparing `composer-0.13.5/tests/test_device.py` & `composer-0.14.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_docker.py` & `composer-0.14.0/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_docs.py` & `composer-0.14.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_engine.py` & `composer-0.14.0/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_events.py` & `composer-0.14.0/tests/test_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,21 +112,18 @@
         self._assert_expected_event_calls(trainer, save_interval, num_epochs=2)
 
     def _assert_expected_event_calls(self, trainer: Trainer, eval_interval: Time, num_epochs: int):
         state = trainer.state
 
         assert state.dataloader_len is not None
         total_steps = num_epochs * int(state.dataloader_len)
-        if state.using_device_microbatch_size:
-            batch_size = state.train_dataloader.batch_size  # type: ignore
-            total_microbatches = total_steps * math.ceil(
-                batch_size / state.device_train_microbatch_size)  # type: ignore
-        else:
-            assert state.grad_accum is not None
-            total_microbatches = total_steps * state.grad_accum
+        batch_size = state.train_dataloader.batch_size  # type: ignore
+        assert batch_size is not None
+        assert state.device_train_microbatch_size is not None
+        total_microbatches = total_steps * math.ceil(batch_size / state.device_train_microbatch_size)
 
         if eval_interval.unit == TimeUnit.BATCH:
             total_evals = total_steps // int(eval_interval)
         elif eval_interval.unit == TimeUnit.EPOCH:
             total_evals = num_epochs // int(eval_interval)
         else:
             total_evals = 0
```

### Comparing `composer-0.13.5/tests/test_full_nlp.py` & `composer-0.14.0/tests/test_full_nlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import copy
 import os
 
 import pytest
 import torch
+from packaging import version
 from torch.utils.data import DataLoader
 from torchmetrics.classification import MulticlassAccuracy
 
 from composer.algorithms import GatedLinearUnits
 from composer.loggers import RemoteUploaderDownloader
 from composer.metrics.nlp import LanguageCrossEntropy, MaskedAccuracy
 from composer.models import HuggingFaceModel
@@ -141,30 +142,31 @@
     assert original_acc.compute() > 0.0
     assert original_acc.compute() == loaded_acc.compute()
 
     return loaded_finetuning_trainer, finetuning_eval_dataloader, rud, 'finetuning_checkpoints/latest-rank0.pt'
 
 
 def inference_test_helper(finetuning_output_path, rud, finetuning_model, algorithms, original_input, original_output,
-                          tmp_path, save_format, device):
+                          onnx_opset_version, tmp_path, save_format, device):
     inference_trainer = Trainer(model=finetuning_model,
                                 load_path=finetuning_output_path,
                                 load_weights_only=True,
                                 loggers=[rud],
                                 seed=17,
                                 algorithms=algorithms,
                                 device=device)
 
     os.mkdir(tmp_path / 'inference_checkpoints')
     sample_input = (original_input, {})
 
     inference.export_for_inference(model=inference_trainer.state.model,
                                    save_format=save_format,
                                    save_path=str(tmp_path / 'inference_checkpoints' / f'exported_model.{save_format}'),
-                                   sample_input=sample_input)
+                                   sample_input=sample_input,
+                                   onnx_opset_version=onnx_opset_version)
 
     copied_batch = copy.deepcopy(original_input)
 
     if save_format == 'onnx':
         onnx = pytest.importorskip('onnx')
         ort = pytest.importorskip('onnxruntime')
         loaded_inference_model = onnx.load(str(tmp_path / 'inference_checkpoints' / 'exported_model.onnx'))
@@ -187,23 +189,28 @@
         if isinstance(original_output, torch.Tensor) else original_output.logits.detach().numpy())
 
 
 @device('cpu', 'gpu')
 # Note: the specificity of these settings are due to incompatibilities (e.g. the simpletransformer model is not traceable)
 @pytest.mark.parametrize('model_type,algorithms,save_format', [('tinybert_hf', [GatedLinearUnits], 'onnx'),
                                                                ('simpletransformer', [], 'torchscript')])
-def test_full_nlp_pipeline(model_type, algorithms, save_format, tiny_bert_tokenizer, tmp_path, request, device):
+@pytest.mark.parametrize('onnx_opset_version', [13, None])
+def test_full_nlp_pipeline(model_type, algorithms, save_format, tiny_bert_tokenizer, onnx_opset_version, tmp_path,
+                           request, device):
     """This test is intended to exercise our full pipeline for NLP.
 
     To this end, it performs pretraining, loads the pretrained model with a classification head for finetuning
     and finetunes it, exports the model for inference, and loads it back in to make predictions.
     """
     pytest.importorskip('libcloud')
     pytest.importorskip('transformers')
 
+    if onnx_opset_version == None and version.parse(torch.__version__) < version.parse('1.13'):
+        pytest.skip("Don't test prior PyTorch version's default Opset version.")
+
     algorithms = [algorithm() for algorithm in algorithms]
 
     device = get_device(device)
 
     tiny_bert_model = None
     if model_type == 'tinybert_hf':
         tiny_bert_model = request.getfixturevalue('tiny_bert_model')
@@ -245,8 +252,8 @@
 
     # inference
     batch = next(iter(finetuning_dataloader))
     finetuning_trainer.state.model.to('cpu')
     finetuning_trainer.state.model.eval()
     original_output = finetuning_trainer.state.model(batch)
     inference_test_helper(finetuning_output_path, rud, finetuning_model_copy, algorithms, batch, original_output,
-                          tmp_path, save_format, device)
+                          onnx_opset_version, tmp_path, save_format, device)
```

### Comparing `composer-0.13.5/tests/test_loss.py` & `composer-0.14.0/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_notebooks.py` & `composer-0.14.0/tests/test_notebooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,19 +95,26 @@
     trainer_monkeypatch_code = inspect.getsource(patch_notebooks)
     notebook_name = os.path.split(notebook)[-1][:-len('.ipynb')]
     if notebook_name == 'medical_image_segmentation':
         pytest.skip('Dataset is only available via kaggle; need to authenticate on ci/cd')
     if notebook_name == 'training_with_submitit':
         pytest.skip('The CI does not support SLURM and submitit')
     if notebook_name == 'auto_microbatching' and device == 'cpu':
-        pytest.skip('auto_grad_accum notebook only runs with a gpu')
+        pytest.skip('auto_microbatching notebook only runs with a gpu')
     if notebook_name == 'TPU_Training_in_composer':
         pytest.skip('The CI does not support tpus')
     if notebook_name == 'ffcv_dataloaders' and device == 'cpu':
         pytest.skip('The FFCV notebook requires CUDA')
+    if notebook_name == 'finetune_huggingface':
+        pytest.skip(
+            "Error that is unreproducible locally: ModuleNotFoundError: No module named 'transformers.models.ernie_m.configuration_ernie_m'"
+        )
+    if notebook_name == 'pretrain_finetune_huggingface':
+        pytest.skip(
+            "Error that is unreproducible locally: No module named 'transformers.models.mega.configuration_mega'")
     with testbook.testbook(notebook) as tb:
         tb.inject(trainer_monkeypatch_code)
         tb.inject('patch_notebooks()')
         for i, cell in enumerate(tb.cells):
             if cell['cell_type'] != 'code':
                 continue
             cell['source'] = modify_cell_source(tb,
```

### Comparing `composer-0.13.5/tests/test_passes.py` & `composer-0.14.0/tests/test_passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_precision.py` & `composer-0.14.0/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_simple_nlp.py` & `composer-0.14.0/tests/test_simple_nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from tests.common.models import SimpleTransformerClassifier, SimpleTransformerMaskedLM
 
 
 def test_simple_nlp_classification():
     vocab_size = 100
     sequence_length = 32
     num_classes = 2
-    size = 100
+    size = 96
     batch_size = 8
 
     train_dataset = RandomTextClassificationDataset(size=size,
                                                     vocab_size=vocab_size,
                                                     sequence_length=sequence_length,
                                                     num_classes=num_classes)
     eval_dataset = RandomTextClassificationDataset(size=size,
@@ -59,15 +59,15 @@
 
 
 def test_simple_nlp_mlm(tiny_bert_tokenizer, tiny_bert_model):
     transformers = pytest.importorskip('transformers')
 
     vocab_size = tiny_bert_tokenizer.vocab_size
     sequence_length = 32
-    size = 100
+    size = 96
     batch_size = 8
 
     train_dataset = RandomTextLMDataset(size=size,
                                         vocab_size=vocab_size,
                                         sequence_length=sequence_length,
                                         use_keys=True)
     eval_dataset = RandomTextLMDataset(size=size, vocab_size=vocab_size, sequence_length=sequence_length, use_keys=True)
```

### Comparing `composer-0.13.5/tests/test_smoketest.py` & `composer-0.14.0/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.5/tests/test_state.py` & `composer-0.14.0/tests/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         device = DeviceCPU() if item.get_closest_marker('gpu') is None else DeviceGPU()
         break
     assert device != None
     state = State(model=model,
                   device=device,
                   train_dataloader=dataloader,
                   run_name=f'{random.randint(0, 100)}',
-                  grad_accum=random.randint(0, 100),
                   rank_zero_seed=random.randint(0, 100),
                   precision=Precision.AMP_FP16,
                   max_duration=f'{random.randint(0, 100)}ep',
                   optimizers=optimizers,
                   device_train_microbatch_size=2)
     state.schedulers = torch.optim.lr_scheduler.StepLR(optimizers, step_size=3)
     state.loss = random_tensor()
```

### Comparing `composer-0.13.5/tests/test_time.py` & `composer-0.14.0/tests/test_time.py`

 * *Files identical despite different names*

