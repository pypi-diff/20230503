# Comparing `tmp/cryptotoolbox-0.6.8.tar.gz` & `tmp/cryptotoolbox-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptotoolbox-0.6.8.tar", last modified: Tue Dec  6 16:52:02 2022, max compression
+gzip compressed data, was "cryptotoolbox-0.6.9.tar", last modified: Tue Dec  6 17:06:34 2022, max compression
```

## Comparing `cryptotoolbox-0.6.8.tar` & `cryptotoolbox-0.6.9.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.835765 cryptotoolbox-0.6.8/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      705 2022-12-06 16:52:02.835491 cryptotoolbox-0.6.8/PKG-INFO
--rw-r--r--   0 stefanduprey   (501) staff       (20)       18 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/README.md
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.783680 cryptotoolbox-0.6.8/cryptotoolbox/
--rw-r--r--   0 stefanduprey   (501) staff       (20)       23 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/__init__.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.785172 cryptotoolbox-0.6.8/cryptotoolbox/analyzer/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/analyzer/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11057 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/analyzer/hourly_market.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13650 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/analyzer/market.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11173 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/analyzer/minutely_market.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.786512 cryptotoolbox-0.6.8/cryptotoolbox/backtest/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      593 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/backtest/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3049 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/backtest/dynamic_plot_backtest.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     4619 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/backtest/plot_backtest.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6976 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/backtest/plot_tools.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5148 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/backtest/print_stats.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.786801 cryptotoolbox-0.6.8/cryptotoolbox/binanceutils/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-08-27 18:13:58.000000 cryptotoolbox-0.6.8/cryptotoolbox/binanceutils/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    16653 2022-09-19 09:32:05.000000 cryptotoolbox-0.6.8/cryptotoolbox/binanceutils/binanceutils.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.787224 cryptotoolbox-0.6.8/cryptotoolbox/boosted_trees/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/boosted_trees/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     7565 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/boosted_trees/roll_lightgbm.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.787952 cryptotoolbox-0.6.8/cryptotoolbox/bot/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/bot/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    21250 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/bot/binance_bot.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    29549 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/bot/binance_spot_bot.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.788285 cryptotoolbox-0.6.8/cryptotoolbox/callback/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/callback/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     8590 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/callback/ts_callback.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.788644 cryptotoolbox-0.6.8/cryptotoolbox/colab/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/colab/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1553 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/colab/colab_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.788900 cryptotoolbox-0.6.8/cryptotoolbox/comparison_kpis/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/comparison_kpis/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      781 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/comparison_kpis/comparison_plot_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.789133 cryptotoolbox-0.6.8/cryptotoolbox/config/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      153 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/__init__.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.789804 cryptotoolbox-0.6.8/cryptotoolbox/config/loader/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      127 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/loader/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      260 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/loader/abstractreader.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1522 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/loader/reader.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.790758 cryptotoolbox-0.6.8/cryptotoolbox/config/object/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      208 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/object/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2115 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/object/config.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      129 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/object/environment.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      444 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/object/model_param_cointegration.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1161 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/object/modelparamtemplate.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      773 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/object/profile.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.791264 cryptotoolbox-0.6.8/cryptotoolbox/config/parser/
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3278 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/parser/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1261 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/parser/abstractparser.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     4420 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/config/parser/parsertemplate.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.793136 cryptotoolbox-0.6.8/cryptotoolbox/connector/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     9023 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/augmento_connector.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    34620 2022-08-29 07:21:31.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/crypto_connector.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     7213 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/crypto_dlws_connector.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5962 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/crypto_s3_connector.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      930 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/pickle_utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1040 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/connector/shifting_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.793475 cryptotoolbox-0.6.8/cryptotoolbox/dash/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/dash/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      489 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/dash/dash_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.793917 cryptotoolbox-0.6.8/cryptotoolbox/dataloader/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      345 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/dataloader/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5284 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/dataloader/models.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.794674 cryptotoolbox-0.6.8/cryptotoolbox/derebit/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-10-13 11:31:55.000000 cryptotoolbox-0.6.8/cryptotoolbox/derebit/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     8168 2022-10-17 10:41:58.000000 cryptotoolbox-0.6.8/cryptotoolbox/derebit/hedging.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     4536 2022-10-17 09:10:34.000000 cryptotoolbox-0.6.8/cryptotoolbox/derebit/retrieve_instruments.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.795287 cryptotoolbox-0.6.8/cryptotoolbox/display/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/display/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      671 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/display/graph.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1779 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/display/table.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.795617 cryptotoolbox-0.6.8/cryptotoolbox/erk/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-06-08 11:43:31.000000 cryptotoolbox-0.6.8/cryptotoolbox/erk/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    74299 2022-06-08 13:54:49.000000 cryptotoolbox-0.6.8/cryptotoolbox/erk/erk_utilities.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.797018 cryptotoolbox-0.6.8/cryptotoolbox/features/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/features/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6330 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/features/easy_feature.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    32664 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/features/features_assembler.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      121 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/features/features_type.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11324 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/features/utility_supervision.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.797279 cryptotoolbox-0.6.8/cryptotoolbox/file_saver/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/file_saver/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13200 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/file_saver/dropbox_file_saver.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.799222 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      349 2022-02-07 17:37:09.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/BestAccuracySelecter.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1483 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/anova_like_model.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2402 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/arima_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1448 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/forecasting_utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1674 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/lgbm_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     4504 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/preprocessing_features.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     4662 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/simple_baseline.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6767 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/simple_threshold_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3062 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/forecasting/sma_model_wrapper.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.799549 cryptotoolbox-0.6.8/cryptotoolbox/ftx/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-05-02 07:08:31.000000 cryptotoolbox-0.6.8/cryptotoolbox/ftx/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    14136 2022-05-02 07:09:10.000000 cryptotoolbox-0.6.8/cryptotoolbox/ftx/clientftx.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.799888 cryptotoolbox-0.6.8/cryptotoolbox/hedge/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-11-02 12:35:17.000000 cryptotoolbox-0.6.8/cryptotoolbox/hedge/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    10715 2022-11-02 12:48:54.000000 cryptotoolbox-0.6.8/cryptotoolbox/hedge/hedge.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.803335 cryptotoolbox-0.6.8/cryptotoolbox/indice/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    72624 2022-11-11 23:54:19.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/alpha.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    60676 2022-11-14 07:44:54.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/alpha_neutral.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)   132016 2022-11-28 13:26:43.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/alpha_neutral_stoploss.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3618 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/indice_plot_utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    36972 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/numba_rebalancing.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    23437 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/rebalancing.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    65807 2022-10-06 08:20:16.000000 cryptotoolbox-0.6.8/cryptotoolbox/indice/smart_liquidity.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.804028 cryptotoolbox-0.6.8/cryptotoolbox/metbots/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/metbots/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    28205 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/metbots/metrics.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.806893 cryptotoolbox-0.6.8/cryptotoolbox/mixing/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1069 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/deterministic_sharpe_optim_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2933 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/erc_allocation_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2933 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/hrp_allocation_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2933 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/ivp_allocation_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1789 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/lasso_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1613 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/lgbm_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      666 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/linear_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      645 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/max_occurence_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3245 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/mixing_utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2934 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/mvp_allocation_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2940 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/mvp_uc_allocation_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      625 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/standard_mean_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      961 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/to_weighted_mean_model_wrapper.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2203 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/mixing/xgb_model_wrapper.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.807138 cryptotoolbox-0.6.8/cryptotoolbox/model_state/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/model_state/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      681 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/model_state/resuming_state.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.807392 cryptotoolbox-0.6.8/cryptotoolbox/movie/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/movie/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2497 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/movie/movie_maker.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.810991 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      867 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      706 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/activations.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    18325 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/expanding_roll_multi_layer_perceptron.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)       71 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/lrs_type.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     9417 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_aggregated_multi_neural_networks.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    21934 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_cnn.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13969 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_lstm.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    20671 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_perceptron.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    14501 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_shortcut_lstm.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    21354 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_shortcut_perceptron.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     7048 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_neural_networks.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6864 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_roll_neural_networks.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11850 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_neural_network.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.811319 cryptotoolbox-0.6.8/cryptotoolbox/onchain_data/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-12-06 07:35:49.000000 cryptotoolbox-0.6.8/cryptotoolbox/onchain_data/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    15459 2022-12-06 16:51:36.000000 cryptotoolbox-0.6.8/cryptotoolbox/onchain_data/onchain_data.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.811698 cryptotoolbox-0.6.8/cryptotoolbox/orderbook/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-16 12:48:20.000000 cryptotoolbox-0.6.8/cryptotoolbox/orderbook/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6472 2022-03-02 09:17:30.000000 cryptotoolbox-0.6.8/cryptotoolbox/orderbook/orderbook.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.821701 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    15673 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/augmento_forecaster.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    17165 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/big_ensembling_runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11785 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/crypto_parallel_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    16732 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/ensembling_runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13512 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/features_explainer.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3607 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/features_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    12361 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/forecaster_runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11208 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/hourlyzation_mixer_runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      906 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/launcher_utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    15455 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/mixer_runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    16919 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_augmento_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    12876 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_big_ensembling_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    14120 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_cointegration_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     8520 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_ensembling_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    16665 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_forecaster_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13801 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    16923 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_mixer_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    14205 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_signal_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5465 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_signal_realtime_backtest_ensembling_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     9127 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/result_analyzer.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    16304 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6955 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_aggregating_analyzer.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    11194 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_aggregating_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    18930 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_aggregating_runner.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     7979 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_mixer.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13447 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_result_analyzer.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5335 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_runner.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.824509 cryptotoolbox-0.6.8/cryptotoolbox/realtime/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/realtime/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    75038 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/realtime/parallel_signal_realtime_ensembling_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    97234 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_bot_degenerate_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    78956 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_bot_multilo_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    78813 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_bot_quantile_launcher.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    22080 2022-11-18 12:57:57.000000 cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_plotting_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.826132 cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    43595 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/allocation.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    21831 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/crypto_signal_mixer.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     6926 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/rolling.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    13413 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/time_series.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.826559 cryptotoolbox-0.6.8/cryptotoolbox/requester/
--rw-r--r--   0 stefanduprey   (501) staff       (20)       29 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/requester/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      730 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/requester/requests.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.826911 cryptotoolbox-0.6.8/cryptotoolbox/risk_metrics/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-05-24 14:34:32.000000 cryptotoolbox-0.6.8/cryptotoolbox/risk_metrics/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    32306 2022-09-28 14:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/risk_metrics/riskmetrics.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.827431 cryptotoolbox-0.6.8/cryptotoolbox/roller/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/roller/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     8733 2022-03-22 14:45:31.000000 cryptotoolbox-0.6.8/cryptotoolbox/roller/roller.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.828901 cryptotoolbox-0.6.8/cryptotoolbox/signal/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/signal/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    36033 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/signal/parameters_generator.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    74901 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/signal/signal_generator.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    50732 2022-09-07 09:01:00.000000 cryptotoolbox-0.6.8/cryptotoolbox/signal/signal_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.830760 cryptotoolbox-0.6.8/cryptotoolbox/slippage/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/slippage/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    70663 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/slippage/binance_slippage_utils.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    84108 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/slippage/bitmex_slippage_utils.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     3764 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/slippage/slippage_plot_utility.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.831104 cryptotoolbox-0.6.8/cryptotoolbox/statistics/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/statistics/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      838 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/statistics/tester.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.832045 cryptotoolbox-0.6.8/cryptotoolbox/tools/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/tools/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1830 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/tools/analyze_tools.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5768 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/tools/display.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2862 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/tools/time_tools.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)      945 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/tools/utils.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.833462 cryptotoolbox-0.6.8/cryptotoolbox/utility/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/utility/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2780 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/utility/date_utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    21564 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/utility/metrics.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1917 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/utility/money_management.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1050 2022-03-22 14:45:31.000000 cryptotoolbox-0.6.8/cryptotoolbox/utility/utility.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5627 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/utility/weights.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.834378 cryptotoolbox-0.6.8/cryptotoolbox/wavelets_fft/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/wavelets_fft/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     2918 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/wavelets_fft/fft_features.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)    12315 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/wavelets_fft/wavelet_features.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.834981 cryptotoolbox-0.6.8/cryptotoolbox/widget/
--rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/widget/__init__.py
--rw-r--r--   0 stefanduprey   (501) staff       (20)     5264 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.8/cryptotoolbox/widget/figure.py
-drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 16:52:02.784437 cryptotoolbox-0.6.8/cryptotoolbox.egg-info/
--rw-r--r--   0 stefanduprey   (501) staff       (20)      705 2022-12-06 16:52:02.000000 cryptotoolbox-0.6.8/cryptotoolbox.egg-info/PKG-INFO
--rw-r--r--   0 stefanduprey   (501) staff       (20)     8529 2022-12-06 16:52:02.000000 cryptotoolbox-0.6.8/cryptotoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 stefanduprey   (501) staff       (20)        1 2022-12-06 16:52:02.000000 cryptotoolbox-0.6.8/cryptotoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 stefanduprey   (501) staff       (20)       14 2022-12-06 16:52:02.000000 cryptotoolbox-0.6.8/cryptotoolbox.egg-info/top_level.txt
--rw-r--r--   0 stefanduprey   (501) staff       (20)       38 2022-12-06 16:52:02.835854 cryptotoolbox-0.6.8/setup.cfg
--rw-r--r--   0 stefanduprey   (501) staff       (20)     1811 2022-12-06 16:51:58.000000 cryptotoolbox-0.6.8/setup.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.447007 cryptotoolbox-0.6.9/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      705 2022-12-06 17:06:34.446795 cryptotoolbox-0.6.9/PKG-INFO
+-rw-r--r--   0 stefanduprey   (501) staff       (20)       18 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/README.md
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.397101 cryptotoolbox-0.6.9/cryptotoolbox/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)       23 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/__init__.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.398630 cryptotoolbox-0.6.9/cryptotoolbox/analyzer/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/analyzer/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11057 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/analyzer/hourly_market.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13650 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/analyzer/market.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11173 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/analyzer/minutely_market.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.399780 cryptotoolbox-0.6.9/cryptotoolbox/backtest/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      593 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/backtest/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3049 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/backtest/dynamic_plot_backtest.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     4619 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/backtest/plot_backtest.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6976 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/backtest/plot_tools.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5148 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/backtest/print_stats.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.400339 cryptotoolbox-0.6.9/cryptotoolbox/binanceutils/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-08-27 18:13:58.000000 cryptotoolbox-0.6.9/cryptotoolbox/binanceutils/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    16653 2022-09-19 09:32:05.000000 cryptotoolbox-0.6.9/cryptotoolbox/binanceutils/binanceutils.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.400988 cryptotoolbox-0.6.9/cryptotoolbox/boosted_trees/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/boosted_trees/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     7565 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/boosted_trees/roll_lightgbm.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.401813 cryptotoolbox-0.6.9/cryptotoolbox/bot/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/bot/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    21250 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/bot/binance_bot.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    29549 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/bot/binance_spot_bot.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.402165 cryptotoolbox-0.6.9/cryptotoolbox/callback/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/callback/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     8590 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/callback/ts_callback.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.402531 cryptotoolbox-0.6.9/cryptotoolbox/colab/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/colab/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1553 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/colab/colab_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.402802 cryptotoolbox-0.6.9/cryptotoolbox/comparison_kpis/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/comparison_kpis/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      781 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/comparison_kpis/comparison_plot_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.403062 cryptotoolbox-0.6.9/cryptotoolbox/config/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      153 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/__init__.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.403769 cryptotoolbox-0.6.9/cryptotoolbox/config/loader/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      127 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/loader/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      260 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/loader/abstractreader.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1522 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/loader/reader.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.404765 cryptotoolbox-0.6.9/cryptotoolbox/config/object/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      208 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/object/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2115 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/object/config.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      129 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/object/environment.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      444 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/object/model_param_cointegration.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1161 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/object/modelparamtemplate.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      773 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/object/profile.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.405264 cryptotoolbox-0.6.9/cryptotoolbox/config/parser/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3278 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/parser/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1261 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/parser/abstractparser.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     4420 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/config/parser/parsertemplate.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.408233 cryptotoolbox-0.6.9/cryptotoolbox/connector/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     9023 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/augmento_connector.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    34620 2022-08-29 07:21:31.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/crypto_connector.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     7213 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/crypto_dlws_connector.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5962 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/crypto_s3_connector.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      930 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/pickle_utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1040 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/connector/shifting_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.408609 cryptotoolbox-0.6.9/cryptotoolbox/dash/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/dash/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      489 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/dash/dash_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.409023 cryptotoolbox-0.6.9/cryptotoolbox/dataloader/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      345 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/dataloader/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5284 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/dataloader/models.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.409745 cryptotoolbox-0.6.9/cryptotoolbox/derebit/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-10-13 11:31:55.000000 cryptotoolbox-0.6.9/cryptotoolbox/derebit/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     8168 2022-10-17 10:41:58.000000 cryptotoolbox-0.6.9/cryptotoolbox/derebit/hedging.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     4536 2022-10-17 09:10:34.000000 cryptotoolbox-0.6.9/cryptotoolbox/derebit/retrieve_instruments.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.410351 cryptotoolbox-0.6.9/cryptotoolbox/display/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/display/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      671 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/display/graph.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1779 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/display/table.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.410736 cryptotoolbox-0.6.9/cryptotoolbox/erk/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-06-08 11:43:31.000000 cryptotoolbox-0.6.9/cryptotoolbox/erk/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    74299 2022-06-08 13:54:49.000000 cryptotoolbox-0.6.9/cryptotoolbox/erk/erk_utilities.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.412343 cryptotoolbox-0.6.9/cryptotoolbox/features/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/features/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6330 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/features/easy_feature.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    32664 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/features/features_assembler.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      121 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/features/features_type.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11324 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/features/utility_supervision.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.412608 cryptotoolbox-0.6.9/cryptotoolbox/file_saver/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/file_saver/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13200 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/file_saver/dropbox_file_saver.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.414651 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      349 2022-02-07 17:37:09.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/BestAccuracySelecter.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1483 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/anova_like_model.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2402 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/arima_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1448 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/forecasting_utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1674 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/lgbm_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     4504 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/preprocessing_features.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     4662 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/simple_baseline.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6767 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/simple_threshold_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3062 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/forecasting/sma_model_wrapper.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.415014 cryptotoolbox-0.6.9/cryptotoolbox/ftx/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-05-02 07:08:31.000000 cryptotoolbox-0.6.9/cryptotoolbox/ftx/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    14136 2022-05-02 07:09:10.000000 cryptotoolbox-0.6.9/cryptotoolbox/ftx/clientftx.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.416160 cryptotoolbox-0.6.9/cryptotoolbox/hedge/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-11-02 12:35:17.000000 cryptotoolbox-0.6.9/cryptotoolbox/hedge/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    10715 2022-11-02 12:48:54.000000 cryptotoolbox-0.6.9/cryptotoolbox/hedge/hedge.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.420479 cryptotoolbox-0.6.9/cryptotoolbox/indice/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    72624 2022-11-11 23:54:19.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/alpha.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    60676 2022-11-14 07:44:54.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/alpha_neutral.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)   132016 2022-11-28 13:26:43.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/alpha_neutral_stoploss.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3618 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/indice_plot_utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    36972 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/numba_rebalancing.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    23437 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/rebalancing.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    65807 2022-10-06 08:20:16.000000 cryptotoolbox-0.6.9/cryptotoolbox/indice/smart_liquidity.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.421469 cryptotoolbox-0.6.9/cryptotoolbox/metbots/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/metbots/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    28205 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/metbots/metrics.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.424275 cryptotoolbox-0.6.9/cryptotoolbox/mixing/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1069 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/deterministic_sharpe_optim_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2933 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/erc_allocation_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2933 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/hrp_allocation_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2933 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/ivp_allocation_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1789 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/lasso_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1613 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/lgbm_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      666 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/linear_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      645 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/max_occurence_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3245 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/mixing_utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2934 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/mvp_allocation_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2940 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/mvp_uc_allocation_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      625 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/standard_mean_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      961 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/to_weighted_mean_model_wrapper.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2203 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/mixing/xgb_model_wrapper.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.424532 cryptotoolbox-0.6.9/cryptotoolbox/model_state/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/model_state/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      681 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/model_state/resuming_state.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.424785 cryptotoolbox-0.6.9/cryptotoolbox/movie/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/movie/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2497 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/movie/movie_maker.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.427662 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      867 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      706 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/activations.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    18325 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/expanding_roll_multi_layer_perceptron.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)       71 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/lrs_type.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     9417 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_aggregated_multi_neural_networks.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    21934 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_cnn.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13969 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_lstm.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    20671 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_perceptron.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    14501 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_shortcut_lstm.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    21354 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_shortcut_perceptron.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     7048 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_neural_networks.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6864 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_roll_neural_networks.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11850 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_neural_network.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.427948 cryptotoolbox-0.6.9/cryptotoolbox/onchain_data/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-12-06 07:35:49.000000 cryptotoolbox-0.6.9/cryptotoolbox/onchain_data/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    15456 2022-12-06 17:06:14.000000 cryptotoolbox-0.6.9/cryptotoolbox/onchain_data/onchain_data.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.428281 cryptotoolbox-0.6.9/cryptotoolbox/orderbook/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-16 12:48:20.000000 cryptotoolbox-0.6.9/cryptotoolbox/orderbook/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6472 2022-03-02 09:17:30.000000 cryptotoolbox-0.6.9/cryptotoolbox/orderbook/orderbook.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.434720 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    15673 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/augmento_forecaster.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    17165 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/big_ensembling_runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11785 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/crypto_parallel_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    16732 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/ensembling_runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13512 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/features_explainer.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3607 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/features_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    12361 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/forecaster_runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11208 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/hourlyzation_mixer_runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      906 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/launcher_utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    15455 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/mixer_runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    16919 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_augmento_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    12876 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_big_ensembling_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    14120 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_cointegration_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     8520 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_ensembling_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    16665 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_forecaster_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13801 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    16923 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_mixer_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    14205 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_signal_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5465 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_signal_realtime_backtest_ensembling_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     9127 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/result_analyzer.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    16304 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6955 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_aggregating_analyzer.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    11194 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_aggregating_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    18930 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_aggregating_runner.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     7979 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_mixer.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13447 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_result_analyzer.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5335 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_runner.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.436900 cryptotoolbox-0.6.9/cryptotoolbox/realtime/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/realtime/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    75038 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/realtime/parallel_signal_realtime_ensembling_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    97234 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_bot_degenerate_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    78956 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_bot_multilo_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    78813 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_bot_quantile_launcher.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    22080 2022-11-18 12:57:57.000000 cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_plotting_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.438459 cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    43595 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/allocation.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    21831 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/crypto_signal_mixer.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     6926 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/rolling.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    13413 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/time_series.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.438866 cryptotoolbox-0.6.9/cryptotoolbox/requester/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)       29 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/requester/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      730 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/requester/requests.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.439223 cryptotoolbox-0.6.9/cryptotoolbox/risk_metrics/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-05-24 14:34:32.000000 cryptotoolbox-0.6.9/cryptotoolbox/risk_metrics/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    32306 2022-09-28 14:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/risk_metrics/riskmetrics.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.439726 cryptotoolbox-0.6.9/cryptotoolbox/roller/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/roller/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     8733 2022-03-22 14:45:31.000000 cryptotoolbox-0.6.9/cryptotoolbox/roller/roller.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.440858 cryptotoolbox-0.6.9/cryptotoolbox/signal/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/signal/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    36033 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/signal/parameters_generator.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    74901 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/signal/signal_generator.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    50732 2022-09-07 09:01:00.000000 cryptotoolbox-0.6.9/cryptotoolbox/signal/signal_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.442618 cryptotoolbox-0.6.9/cryptotoolbox/slippage/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/slippage/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    70663 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/slippage/binance_slippage_utils.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    84108 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/slippage/bitmex_slippage_utils.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     3764 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/slippage/slippage_plot_utility.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.443124 cryptotoolbox-0.6.9/cryptotoolbox/statistics/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/statistics/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      838 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/statistics/tester.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.444106 cryptotoolbox-0.6.9/cryptotoolbox/tools/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/tools/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1830 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/tools/analyze_tools.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5768 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/tools/display.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2862 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/tools/time_tools.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      945 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/tools/utils.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.445404 cryptotoolbox-0.6.9/cryptotoolbox/utility/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/utility/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2780 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/utility/date_utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    21564 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/utility/metrics.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1917 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/utility/money_management.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1050 2022-03-22 14:45:31.000000 cryptotoolbox-0.6.9/cryptotoolbox/utility/utility.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5627 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/utility/weights.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.446045 cryptotoolbox-0.6.9/cryptotoolbox/wavelets_fft/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/wavelets_fft/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     2918 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/wavelets_fft/fft_features.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)    12315 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/wavelets_fft/wavelet_features.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.446425 cryptotoolbox-0.6.9/cryptotoolbox/widget/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        0 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/widget/__init__.py
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     5264 2022-02-07 12:49:26.000000 cryptotoolbox-0.6.9/cryptotoolbox/widget/figure.py
+drwxr-xr-x   0 stefanduprey   (501) staff       (20)        0 2022-12-06 17:06:34.397815 cryptotoolbox-0.6.9/cryptotoolbox.egg-info/
+-rw-r--r--   0 stefanduprey   (501) staff       (20)      705 2022-12-06 17:06:34.000000 cryptotoolbox-0.6.9/cryptotoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     8529 2022-12-06 17:06:34.000000 cryptotoolbox-0.6.9/cryptotoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanduprey   (501) staff       (20)        1 2022-12-06 17:06:34.000000 cryptotoolbox-0.6.9/cryptotoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanduprey   (501) staff       (20)       14 2022-12-06 17:06:34.000000 cryptotoolbox-0.6.9/cryptotoolbox.egg-info/top_level.txt
+-rw-r--r--   0 stefanduprey   (501) staff       (20)       38 2022-12-06 17:06:34.447064 cryptotoolbox-0.6.9/setup.cfg
+-rw-r--r--   0 stefanduprey   (501) staff       (20)     1811 2022-12-06 17:06:29.000000 cryptotoolbox-0.6.9/setup.py
```

### Comparing `cryptotoolbox-0.6.8/PKG-INFO` & `cryptotoolbox-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptotoolbox
-Version: 0.6.8
+Version: 0.6.9
 Summary: Dashboard for financial market data
 Download-URL: https://github.com/sduprey/cryptotoolbox/archive/0.0.tar.gz
 Author: stefan duprey
 Author-email: stefan.duprey@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/analyzer/hourly_market.py` & `cryptotoolbox-0.6.9/cryptotoolbox/analyzer/hourly_market.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/analyzer/market.py` & `cryptotoolbox-0.6.9/cryptotoolbox/analyzer/market.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/analyzer/minutely_market.py` & `cryptotoolbox-0.6.9/cryptotoolbox/analyzer/minutely_market.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/backtest/__init__.py` & `cryptotoolbox-0.6.9/cryptotoolbox/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/backtest/dynamic_plot_backtest.py` & `cryptotoolbox-0.6.9/cryptotoolbox/backtest/dynamic_plot_backtest.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/backtest/plot_backtest.py` & `cryptotoolbox-0.6.9/cryptotoolbox/backtest/plot_backtest.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/backtest/plot_tools.py` & `cryptotoolbox-0.6.9/cryptotoolbox/backtest/plot_tools.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/backtest/print_stats.py` & `cryptotoolbox-0.6.9/cryptotoolbox/backtest/print_stats.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/binanceutils/binanceutils.py` & `cryptotoolbox-0.6.9/cryptotoolbox/binanceutils/binanceutils.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/boosted_trees/roll_lightgbm.py` & `cryptotoolbox-0.6.9/cryptotoolbox/boosted_trees/roll_lightgbm.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/bot/binance_bot.py` & `cryptotoolbox-0.6.9/cryptotoolbox/bot/binance_bot.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/bot/binance_spot_bot.py` & `cryptotoolbox-0.6.9/cryptotoolbox/bot/binance_spot_bot.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/callback/ts_callback.py` & `cryptotoolbox-0.6.9/cryptotoolbox/callback/ts_callback.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/colab/colab_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/colab/colab_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/comparison_kpis/comparison_plot_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/comparison_kpis/comparison_plot_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/loader/reader.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/loader/reader.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/object/config.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/object/config.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/object/modelparamtemplate.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/object/modelparamtemplate.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/object/profile.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/object/profile.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/parser/__init__.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/parser/abstractparser.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/parser/abstractparser.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/config/parser/parsertemplate.py` & `cryptotoolbox-0.6.9/cryptotoolbox/config/parser/parsertemplate.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/connector/augmento_connector.py` & `cryptotoolbox-0.6.9/cryptotoolbox/connector/augmento_connector.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/connector/crypto_connector.py` & `cryptotoolbox-0.6.9/cryptotoolbox/connector/crypto_connector.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/connector/crypto_dlws_connector.py` & `cryptotoolbox-0.6.9/cryptotoolbox/connector/crypto_dlws_connector.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/connector/crypto_s3_connector.py` & `cryptotoolbox-0.6.9/cryptotoolbox/connector/crypto_s3_connector.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/connector/pickle_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/connector/pickle_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/connector/shifting_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/connector/shifting_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/dataloader/models.py` & `cryptotoolbox-0.6.9/cryptotoolbox/dataloader/models.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/derebit/hedging.py` & `cryptotoolbox-0.6.9/cryptotoolbox/derebit/hedging.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/derebit/retrieve_instruments.py` & `cryptotoolbox-0.6.9/cryptotoolbox/derebit/retrieve_instruments.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/display/graph.py` & `cryptotoolbox-0.6.9/cryptotoolbox/display/graph.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/display/table.py` & `cryptotoolbox-0.6.9/cryptotoolbox/display/table.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/erk/erk_utilities.py` & `cryptotoolbox-0.6.9/cryptotoolbox/erk/erk_utilities.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/features/easy_feature.py` & `cryptotoolbox-0.6.9/cryptotoolbox/features/easy_feature.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/features/features_assembler.py` & `cryptotoolbox-0.6.9/cryptotoolbox/features/features_assembler.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/features/utility_supervision.py` & `cryptotoolbox-0.6.9/cryptotoolbox/features/utility_supervision.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/file_saver/dropbox_file_saver.py` & `cryptotoolbox-0.6.9/cryptotoolbox/file_saver/dropbox_file_saver.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/anova_like_model.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/anova_like_model.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/arima_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/arima_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/forecasting_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/forecasting_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/lgbm_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/lgbm_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/preprocessing_features.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/preprocessing_features.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/simple_baseline.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/simple_baseline.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/simple_threshold_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/simple_threshold_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/forecasting/sma_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/forecasting/sma_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/ftx/clientftx.py` & `cryptotoolbox-0.6.9/cryptotoolbox/ftx/clientftx.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/hedge/hedge.py` & `cryptotoolbox-0.6.9/cryptotoolbox/hedge/hedge.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/alpha.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/alpha.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/alpha_neutral.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/alpha_neutral.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/alpha_neutral_stoploss.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/alpha_neutral_stoploss.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/indice_plot_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/indice_plot_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/numba_rebalancing.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/numba_rebalancing.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/rebalancing.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/rebalancing.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/indice/smart_liquidity.py` & `cryptotoolbox-0.6.9/cryptotoolbox/indice/smart_liquidity.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/metbots/metrics.py` & `cryptotoolbox-0.6.9/cryptotoolbox/metbots/metrics.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/deterministic_sharpe_optim_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/deterministic_sharpe_optim_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/erc_allocation_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/erc_allocation_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/hrp_allocation_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/hrp_allocation_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/ivp_allocation_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/ivp_allocation_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/lasso_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/lasso_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/lgbm_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/lgbm_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/linear_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/linear_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/max_occurence_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/max_occurence_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/mixing_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/mixing_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/mvp_allocation_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/mvp_allocation_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/mvp_uc_allocation_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/mvp_uc_allocation_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/standard_mean_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/standard_mean_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/to_weighted_mean_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/to_weighted_mean_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/mixing/xgb_model_wrapper.py` & `cryptotoolbox-0.6.9/cryptotoolbox/mixing/xgb_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/model_state/resuming_state.py` & `cryptotoolbox-0.6.9/cryptotoolbox/model_state/resuming_state.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/movie/movie_maker.py` & `cryptotoolbox-0.6.9/cryptotoolbox/movie/movie_maker.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/__init__.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/activations.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/activations.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/expanding_roll_multi_layer_perceptron.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/expanding_roll_multi_layer_perceptron.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_aggregated_multi_neural_networks.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_aggregated_multi_neural_networks.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_cnn.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_cnn.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_lstm.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_lstm.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_perceptron.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_perceptron.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_shortcut_lstm.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_shortcut_lstm.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_layer_shortcut_perceptron.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_layer_shortcut_perceptron.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_neural_networks.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_neural_networks.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_multi_roll_neural_networks.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_multi_roll_neural_networks.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/neural_net/roll_neural_network.py` & `cryptotoolbox-0.6.9/cryptotoolbox/neural_net/roll_neural_network.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/onchain_data/onchain_data.py` & `cryptotoolbox-0.6.9/cryptotoolbox/onchain_data/onchain_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,17 +182,17 @@
     final_df = pd.merge(UR.copy(), supply_df.copy(), left_index=True, right_index=True)
     traderjoe_usdc_df = final_df[['USDC_liquidity', 'USDC_apy']].copy()
     traderjoe_usdt_df = final_df[['USDT_liquidity', 'USDT_apy']].copy()
     traderjoe_btcb_df = final_df[['BTC.B_liquidity', 'BTCB_apy']].copy()
     #    final_df[['USDC.E_liquidity', 'USDC.E', 'USDCE_apy']].copy()
     #    final_df[['USDT.E_liquidity','USDT.E', 'USDTE_apy']].copy()
 
-    traderjoe_usdc_df = traderjoe_usdc_df.rename(columns={'USDC_liquidity': 'supply_liquidity', 'USDC_apy': 'dapr'})
-    traderjoe_usdt_df = traderjoe_usdt_df.rename(columns={'USDT_liquidity': 'supply_liquidity', 'USDT_apy': 'dapr'})
-    traderjoe_btcb_df = traderjoe_btcb_df.rename(columns={'BTC.B_liquidity': 'supply_liquidity', 'BTCB_apy': 'dapr'})
+    traderjoe_usdc_df = traderjoe_usdc_df.rename(columns={'USDC_liquidity': 'supply_liquidity', 'USDC_apy': 'apy'})
+    traderjoe_usdt_df = traderjoe_usdt_df.rename(columns={'USDT_liquidity': 'supply_liquidity', 'USDT_apy': 'apy'})
+    traderjoe_btcb_df = traderjoe_btcb_df.rename(columns={'BTC.B_liquidity': 'supply_liquidity', 'BTCB_apy': 'apy'})
     return traderjoe_usdc_df, traderjoe_usdt_df, traderjoe_btcb_df
 
 
 def request_samurai_aave_v3_usdc():
     # https://yieldsamurai.com/pool/avalanche/0x625e7708f30ca75bfd92586e17077590c60eb4cd
     samurai_url = 'https://yieldsamurai.com/api/pool-historical-data'
     aave_usdc_payload = {
```

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/orderbook/orderbook.py` & `cryptotoolbox-0.6.9/cryptotoolbox/orderbook/orderbook.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/augmento_forecaster.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/augmento_forecaster.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/big_ensembling_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/big_ensembling_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/crypto_parallel_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/crypto_parallel_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/ensembling_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/ensembling_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/features_explainer.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/features_explainer.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/features_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/features_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/forecaster_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/forecaster_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/hourlyzation_mixer_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/hourlyzation_mixer_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/launcher_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/launcher_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/mixer_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/mixer_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_augmento_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_augmento_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_big_ensembling_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_big_ensembling_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_cointegration_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_cointegration_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_ensembling_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_ensembling_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_forecaster_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_forecaster_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_mixer_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_mixer_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_signal_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_signal_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/parallel_signal_realtime_backtest_ensembling_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/parallel_signal_realtime_backtest_ensembling_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/result_analyzer.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/result_analyzer.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_aggregating_analyzer.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_aggregating_analyzer.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_aggregating_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_aggregating_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_aggregating_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_aggregating_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_mixer.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_mixer.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_result_analyzer.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_result_analyzer.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/parallel_run/signal_runner.py` & `cryptotoolbox-0.6.9/cryptotoolbox/parallel_run/signal_runner.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/realtime/parallel_signal_realtime_ensembling_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/realtime/parallel_signal_realtime_ensembling_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_bot_degenerate_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_bot_degenerate_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_bot_multilo_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_bot_multilo_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_bot_quantile_launcher.py` & `cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_bot_quantile_launcher.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/realtime/realtime_plotting_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/realtime/realtime_plotting_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/allocation.py` & `cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/allocation.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/crypto_signal_mixer.py` & `cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/crypto_signal_mixer.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/rolling.py` & `cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/rolling.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/rebalancing/time_series.py` & `cryptotoolbox-0.6.9/cryptotoolbox/rebalancing/time_series.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/requester/requests.py` & `cryptotoolbox-0.6.9/cryptotoolbox/requester/requests.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/risk_metrics/riskmetrics.py` & `cryptotoolbox-0.6.9/cryptotoolbox/risk_metrics/riskmetrics.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/roller/roller.py` & `cryptotoolbox-0.6.9/cryptotoolbox/roller/roller.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/signal/parameters_generator.py` & `cryptotoolbox-0.6.9/cryptotoolbox/signal/parameters_generator.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/signal/signal_generator.py` & `cryptotoolbox-0.6.9/cryptotoolbox/signal/signal_generator.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/signal/signal_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/signal/signal_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/slippage/binance_slippage_utils.py` & `cryptotoolbox-0.6.9/cryptotoolbox/slippage/binance_slippage_utils.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/slippage/bitmex_slippage_utils.py` & `cryptotoolbox-0.6.9/cryptotoolbox/slippage/bitmex_slippage_utils.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/slippage/slippage_plot_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/slippage/slippage_plot_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/statistics/tester.py` & `cryptotoolbox-0.6.9/cryptotoolbox/statistics/tester.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/tools/analyze_tools.py` & `cryptotoolbox-0.6.9/cryptotoolbox/tools/analyze_tools.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/tools/display.py` & `cryptotoolbox-0.6.9/cryptotoolbox/tools/display.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/tools/time_tools.py` & `cryptotoolbox-0.6.9/cryptotoolbox/tools/time_tools.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/tools/utils.py` & `cryptotoolbox-0.6.9/cryptotoolbox/tools/utils.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/utility/date_utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/utility/date_utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/utility/metrics.py` & `cryptotoolbox-0.6.9/cryptotoolbox/utility/metrics.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/utility/money_management.py` & `cryptotoolbox-0.6.9/cryptotoolbox/utility/money_management.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/utility/utility.py` & `cryptotoolbox-0.6.9/cryptotoolbox/utility/utility.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/utility/weights.py` & `cryptotoolbox-0.6.9/cryptotoolbox/utility/weights.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/wavelets_fft/fft_features.py` & `cryptotoolbox-0.6.9/cryptotoolbox/wavelets_fft/fft_features.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/wavelets_fft/wavelet_features.py` & `cryptotoolbox-0.6.9/cryptotoolbox/wavelets_fft/wavelet_features.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox/widget/figure.py` & `cryptotoolbox-0.6.9/cryptotoolbox/widget/figure.py`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox.egg-info/PKG-INFO` & `cryptotoolbox-0.6.9/cryptotoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptotoolbox
-Version: 0.6.8
+Version: 0.6.9
 Summary: Dashboard for financial market data
 Download-URL: https://github.com/sduprey/cryptotoolbox/archive/0.0.tar.gz
 Author: stefan duprey
 Author-email: stefan.duprey@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cryptotoolbox-0.6.8/cryptotoolbox.egg-info/SOURCES.txt` & `cryptotoolbox-0.6.9/cryptotoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptotoolbox-0.6.8/setup.py` & `cryptotoolbox-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     'python-binance',
     'llvmlite'
 #    'llvmlite==0.33.0'
 ]
 build_requires=[]
 setup(
     name='cryptotoolbox',
-    version='0.6.8',
+    version='0.6.9',
     packages=find_packages(),
     download_url='https://github.com/sduprey/cryptotoolbox/archive/0.0.tar.gz',
     author='stefan duprey',
     author_email='stefan.duprey@gmail.com',
     description='Dashboard for financial market data',
     license='MIT',
     install_requires=build_requires,
```

