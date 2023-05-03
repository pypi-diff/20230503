# Comparing `tmp/qis-1.0.8.tar.gz` & `tmp/qis-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qis-1.0.8.tar", max compression
+gzip compressed data, was "qis-1.0.9.tar", max compression
```

## Comparing `qis-1.0.8.tar` & `qis-1.0.9.tar`

### file list

```diff
@@ -1,101 +1,108 @@
--rw-r--r--   0        0        0    35802 2022-12-30 16:28:55.000000 qis-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1792 2023-01-23 15:09:31.473164 qis-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1000 2023-01-23 05:33:44.000000 qis-1.0.8/qis/__init__.py
--rw-r--r--   0        0        0     5275 2023-01-23 14:33:26.250571 qis-1.0.8/qis/examples/asset_perf_report.py
--rw-r--r--   0        0        0     2088 2023-01-22 21:54:41.000000 qis-1.0.8/qis/examples/gaussian_mixure_scatter.py
--rw-r--r--   0        0        0    14511 2023-01-23 06:27:37.000000 qis-1.0.8/qis/examples/move_index.py
--rw-r--r--   0        0        0     3450 2023-01-23 14:03:45.862167 qis-1.0.8/qis/examples/performance_visuals.py
--rw-r--r--   0        0        0     1270 2023-01-22 21:54:41.000000 qis-1.0.8/qis/examples/plot_ust_rates.py
--rw-r--r--   0        0        0     2311 2023-01-22 21:54:41.000000 qis-1.0.8/qis/examples/portfolio_opt_backtest.py
--rw-r--r--   0        0        0    11025 2023-01-23 14:47:37.965644 qis-1.0.8/qis/examples/simulate_quant_strats.py
--rw-r--r--   0        0        0     8042 2023-01-08 15:37:28.000000 qis-1.0.8/qis/examples/test_ewm.py
--rw-r--r--   0        0        0     1599 2023-01-22 21:54:41.000000 qis-1.0.8/qis/examples/test_scatter.py
--rw-r--r--   0        0        0    35925 2023-01-23 05:34:42.000000 qis-1.0.8/qis/file_utils.py
--rw-r--r--   0        0        0      991 2023-01-15 20:14:44.000000 qis-1.0.8/qis/local_path.py
--rw-r--r--   0        0        0     2256 2023-01-23 15:03:11.754733 qis-1.0.8/qis/models/__init__.py
--rw-r--r--   0        0        0        0 2021-05-21 09:42:40.000000 qis-1.0.8/qis/models/linear/__init__.py
--rw-r--r--   0        0        0     5458 2023-01-08 14:55:40.000000 qis-1.0.8/qis/models/linear/auto_corr.py
--rw-r--r--   0        0        0     9489 2023-01-08 14:55:40.000000 qis-1.0.8/qis/models/linear/corr_cov_matrix.py
--rw-r--r--   0        0        0    39806 2023-01-07 22:00:28.000000 qis-1.0.8/qis/models/linear/ewm.py
--rw-r--r--   0        0        0     3620 2023-01-08 14:55:40.000000 qis-1.0.8/qis/models/linear/ewm_convolution.py
--rw-r--r--   0        0        0     5821 2023-01-23 14:52:48.658456 qis-1.0.8/qis/models/linear/ewm_factors.py
--rw-r--r--   0        0        0     4032 2023-01-23 14:52:48.489446 qis-1.0.8/qis/models/linear/pca.py
--rw-r--r--   0        0        0     6192 2023-01-23 14:52:48.601311 qis-1.0.8/qis/models/linear/plot_correlations.py
--rw-r--r--   0        0        0    11295 2023-01-23 14:52:48.162777 qis-1.0.8/qis/models/linear/ra_returns.py
--rw-r--r--   0        0        0        0 2021-12-04 12:08:05.000000 qis-1.0.8/qis/models/stats/__init__.py
--rw-r--r--   0        0        0    19009 2023-01-08 14:55:40.000000 qis-1.0.8/qis/models/stats/bootstrap.py
--rw-r--r--   0        0        0     8504 2023-01-08 14:55:40.000000 qis-1.0.8/qis/models/stats/gaussian_mixture.py
--rw-r--r--   0        0        0     2319 2023-01-08 14:55:40.000000 qis-1.0.8/qis/models/stats/ohlc_vol.py
--rw-r--r--   0        0        0     8556 2023-01-23 14:52:48.704524 qis-1.0.8/qis/models/stats/test_bootstrap.py
--rw-r--r--   0        0        0     2432 2023-01-08 15:22:04.000000 qis-1.0.8/qis/perfstats/__init__.py
--rw-r--r--   0        0        0     7178 2023-01-23 14:52:48.780112 qis-1.0.8/qis/perfstats/cond_regression.py
--rw-r--r--   0        0        0    10871 2023-01-07 23:34:31.000000 qis-1.0.8/qis/perfstats/config.py
--rw-r--r--   0        0        0     6243 2023-01-23 14:52:48.824090 qis-1.0.8/qis/perfstats/desc_table.py
--rw-r--r--   0        0        0    18712 2023-01-23 14:52:48.566643 qis-1.0.8/qis/perfstats/perf_table.py
--rw-r--r--   0        0        0    20097 2023-01-23 14:52:48.096487 qis-1.0.8/qis/perfstats/regime_classifier.py
--rw-r--r--   0        0        0    30176 2023-01-23 14:52:48.368640 qis-1.0.8/qis/perfstats/returns.py
--rw-r--r--   0        0        0     8315 2022-12-17 06:54:07.000000 qis-1.0.8/qis/perfstats/timeseries_bfill.py
--rw-r--r--   0        0        0     3685 2023-01-23 14:03:45.874262 qis-1.0.8/qis/plots/__init__.py
--rw-r--r--   0        0        0    17652 2023-01-23 14:52:48.194624 qis-1.0.8/qis/plots/bars.py
--rw-r--r--   0        0        0    18841 2023-01-23 14:52:48.809517 qis-1.0.8/qis/plots/boxplot.py
--rw-r--r--   0        0        0     3917 2023-01-07 22:17:49.000000 qis-1.0.8/qis/plots/contour.py
--rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-1.0.8/qis/plots/derived/__init__.py
--rw-r--r--   0        0        0     2196 2023-01-07 22:34:01.000000 qis-1.0.8/qis/plots/derived/data_timeseries.py
--rw-r--r--   0        0        0     7410 2023-01-23 14:52:48.618324 qis-1.0.8/qis/plots/derived/drawdowns.py
--rw-r--r--   0        0        0    16816 2023-01-23 14:52:48.315699 qis-1.0.8/qis/plots/derived/perf_table.py
--rw-r--r--   0        0        0    21125 2023-01-23 14:52:48.210960 qis-1.0.8/qis/plots/derived/prices.py
--rw-r--r--   0        0        0     3489 2023-01-23 14:52:48.744063 qis-1.0.8/qis/plots/derived/regime_class_table.py
--rw-r--r--   0        0        0    11752 2023-01-23 14:52:48.674672 qis-1.0.8/qis/plots/derived/regime_data.py
--rw-r--r--   0        0        0     3519 2023-01-23 14:52:48.114907 qis-1.0.8/qis/plots/derived/regime_pdf.py
--rw-r--r--   0        0        0     6590 2023-01-23 14:52:48.730139 qis-1.0.8/qis/plots/derived/regime_scatter.py
--rw-r--r--   0        0        0    19263 2023-01-23 14:52:48.257985 qis-1.0.8/qis/plots/derived/returns_heatmap.py
--rw-r--r--   0        0        0     5011 2023-01-23 14:52:48.243433 qis-1.0.8/qis/plots/derived/returns_scatter.py
--rw-r--r--   0        0        0     4008 2023-01-22 21:00:17.000000 qis-1.0.8/qis/plots/errorbar.py
--rw-r--r--   0        0        0     3643 2023-01-23 14:52:48.553076 qis-1.0.8/qis/plots/heatmap.py
--rw-r--r--   0        0        0    10375 2023-01-22 21:01:33.000000 qis-1.0.8/qis/plots/histogram.py
--rw-r--r--   0        0        0     2917 2023-01-07 22:25:33.000000 qis-1.0.8/qis/plots/histplot2d.py
--rw-r--r--   0        0        0     5383 2023-01-23 09:59:51.265680 qis-1.0.8/qis/plots/lineplot.py
--rw-r--r--   0        0        0     1608 2023-01-07 22:25:33.000000 qis-1.0.8/qis/plots/pie.py
--rw-r--r--   0        0        0     5744 2023-01-23 14:52:48.178382 qis-1.0.8/qis/plots/qqplot.py
--rw-r--r--   0        0        0    14041 2023-01-22 21:03:25.000000 qis-1.0.8/qis/plots/scatter.py
--rw-r--r--   0        0        0     5975 2023-01-22 21:04:18.000000 qis-1.0.8/qis/plots/stackplot.py
--rw-r--r--   0        0        0    14245 2023-01-22 21:07:08.000000 qis-1.0.8/qis/plots/table.py
--rw-r--r--   0        0        0    21708 2023-01-23 14:52:48.284386 qis-1.0.8/qis/plots/time_series.py
--rw-r--r--   0        0        0    54271 2023-01-23 14:52:48.636657 qis-1.0.8/qis/plots/utils.py
--rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-1.0.8/qis/portfolio/__init__.py
--rw-r--r--   0        0        0    11449 2023-01-23 14:52:48.082135 qis-1.0.8/qis/portfolio/backtester.py
--rw-r--r--   0        0        0    30334 2023-01-23 14:03:45.887262 qis-1.0.8/qis/portfolio/multi_portfolio_data.py
--rw-r--r--   0        0        0        0 2021-10-10 14:27:53.000000 qis-1.0.8/qis/portfolio/optimization/__init__.py
--rw-r--r--   0        0        0    11693 2022-12-16 17:12:53.000000 qis-1.0.8/qis/portfolio/optimization/opt_solvers.py
--rw-r--r--   0        0        0    20002 2022-09-02 13:03:58.000000 qis-1.0.8/qis/portfolio/optimization/qp_solvers.py
--rw-r--r--   0        0        0    20538 2023-01-23 14:52:48.333676 qis-1.0.8/qis/portfolio/optimization/rolling_portfolios.py
--rw-r--r--   0        0        0    34830 2023-01-23 14:03:45.854056 qis-1.0.8/qis/portfolio/portfolio_data.py
--rw-r--r--   0        0        0        0 2021-03-26 11:07:46.000000 qis-1.0.8/qis/portfolio/reports/__init__.py
--rw-r--r--   0        0        0    17477 2023-01-23 14:52:48.066280 qis-1.0.8/qis/portfolio/reports/multi_asset_factsheet.py
--rw-r--r--   0        0        0    10867 2023-01-23 14:52:48.425999 qis-1.0.8/qis/portfolio/reports/multi_strategy_factsheet.py
--rw-r--r--   0        0        0    13971 2023-01-23 14:52:48.533240 qis-1.0.8/qis/portfolio/reports/portfolio_factsheet.py
--rw-r--r--   0        0        0    17937 2023-01-23 14:52:48.519199 qis-1.0.8/qis/portfolio/reports/strategy_factsheet.py
--rw-r--r--   0        0        0        0 2022-12-17 17:53:19.000000 qis-1.0.8/qis/portfolio/strats/__init__.py
--rw-r--r--   0        0        0     5778 2023-01-22 21:34:07.000000 qis-1.0.8/qis/portfolio/strats/quant_strats_delta1.py
--rw-r--r--   0        0        0      463 2023-01-22 08:39:54.000000 qis-1.0.8/qis/read_qis_modules.py
--rw-r--r--   0        0        0      477 2023-01-15 21:18:11.000000 qis-1.0.8/qis/settings.yaml
--rw-r--r--   0        0        0      443 2023-01-15 20:14:44.000000 qis-1.0.8/qis/sql_engine.py
--rw-r--r--   0        0        0     1199 2023-01-23 14:54:44.261277 qis-1.0.8/qis/test_data.py
--rw-r--r--   0        0        0     5037 2023-01-23 08:10:14.320845 qis-1.0.8/qis/utils/__init__.py
--rw-r--r--   0        0        0    43000 2023-01-23 05:28:35.000000 qis-1.0.8/qis/utils/dates.py
--rw-r--r--   0        0        0     8942 2023-01-07 21:17:28.000000 qis-1.0.8/qis/utils/df_agg.py
--rw-r--r--   0        0        0     8491 2023-01-08 13:32:37.000000 qis-1.0.8/qis/utils/df_cut.py
--rw-r--r--   0        0        0     7812 2023-01-07 22:09:59.000000 qis-1.0.8/qis/utils/df_freq.py
--rw-r--r--   0        0        0    10992 2023-01-07 21:37:16.000000 qis-1.0.8/qis/utils/df_groups.py
--rw-r--r--   0        0        0     6819 2023-01-23 14:52:48.351818 qis-1.0.8/qis/utils/df_melt.py
--rw-r--r--   0        0        0    27227 2023-01-23 10:47:10.720137 qis-1.0.8/qis/utils/df_ops.py
--rw-r--r--   0        0        0     8295 2023-01-22 21:00:17.000000 qis-1.0.8/qis/utils/df_str.py
--rw-r--r--   0        0        0    11344 2022-12-30 16:13:34.000000 qis-1.0.8/qis/utils/df_to_weights.py
--rw-r--r--   0        0        0    10589 2023-01-07 22:05:03.000000 qis-1.0.8/qis/utils/generic.py
--rw-r--r--   0        0        0    14809 2022-12-29 08:28:09.000000 qis-1.0.8/qis/utils/np_ops.py
--rw-r--r--   0        0        0     5534 2023-01-22 21:03:25.000000 qis-1.0.8/qis/utils/ols.py
--rw-r--r--   0        0        0     4589 2022-12-17 17:01:53.000000 qis-1.0.8/qis/utils/sampling.py
--rw-r--r--   0        0        0     5938 2022-12-16 21:08:07.000000 qis-1.0.8/qis/utils/struct_ops.py
--rw-r--r--   0        0        0      926 2023-01-08 14:42:46.000000 qis-1.0.8/README.md
--rw-r--r--   0        0        0     2156 1970-01-01 00:00:00.000000 qis-1.0.8/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 qis-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-12-30 16:28:55.000000 qis-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1792 2023-01-23 21:43:40.064411 qis-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1000 2023-01-23 05:33:44.000000 qis-1.0.9/qis/__init__.py
+-rw-r--r--   0        0        0   351721 2023-01-23 16:05:45.000000 qis-1.0.9/qis/examples/figures/perf1.PNG
+-rw-r--r--   0        0        0   918269 2023-01-23 16:05:46.000000 qis-1.0.9/qis/examples/figures/perf2.PNG
+-rw-r--r--   0        0        0   298282 2023-01-23 16:05:48.000000 qis-1.0.9/qis/examples/figures/perf3.PNG
+-rw-r--r--   0        0        0     2088 2023-01-22 21:54:41.399711 qis-1.0.9/qis/examples/gaussian_mixure_scatter.py
+-rw-r--r--   0        0        0    14511 2023-01-23 06:27:37.000000 qis-1.0.9/qis/examples/move_index.py
+-rw-r--r--   0        0        0     1703 2023-01-23 16:05:37.000000 qis-1.0.9/qis/examples/performances.py
+-rw-r--r--   0        0        0     2311 2023-01-22 21:54:41.359272 qis-1.0.9/qis/examples/portfolio_opt_backtest.py
+-rw-r--r--   0        0        0     5275 2023-01-23 14:33:26.000000 qis-1.0.9/qis/examples/price_plots.py
+-rw-r--r--   0        0        0    11025 2023-01-23 14:47:37.000000 qis-1.0.9/qis/examples/simulate_quant_strats.py
+-rw-r--r--   0        0        0     8042 2023-01-08 15:37:28.000000 qis-1.0.9/qis/examples/test_ewm.py
+-rw-r--r--   0        0        0     1599 2023-01-22 21:54:41.465278 qis-1.0.9/qis/examples/test_scatter.py
+-rw-r--r--   0        0        0    35925 2023-01-23 05:34:42.000000 qis-1.0.9/qis/file_utils.py
+-rw-r--r--   0        0        0      991 2023-01-15 20:14:44.000000 qis-1.0.9/qis/local_path.py
+-rw-r--r--   0        0        0     2256 2023-01-23 15:03:11.000000 qis-1.0.9/qis/models/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-21 09:42:40.000000 qis-1.0.9/qis/models/linear/__init__.py
+-rw-r--r--   0        0        0     5458 2023-01-08 14:55:40.000000 qis-1.0.9/qis/models/linear/auto_corr.py
+-rw-r--r--   0        0        0     9489 2023-01-08 14:55:40.000000 qis-1.0.9/qis/models/linear/corr_cov_matrix.py
+-rw-r--r--   0        0        0    39806 2023-01-07 22:00:28.000000 qis-1.0.9/qis/models/linear/ewm.py
+-rw-r--r--   0        0        0     3620 2023-01-08 14:55:40.000000 qis-1.0.9/qis/models/linear/ewm_convolution.py
+-rw-r--r--   0        0        0     5821 2023-01-23 14:52:48.000000 qis-1.0.9/qis/models/linear/ewm_factors.py
+-rw-r--r--   0        0        0     4032 2023-01-23 14:52:48.000000 qis-1.0.9/qis/models/linear/pca.py
+-rw-r--r--   0        0        0     6192 2023-01-23 14:52:48.000000 qis-1.0.9/qis/models/linear/plot_correlations.py
+-rw-r--r--   0        0        0    11295 2023-01-23 14:52:48.000000 qis-1.0.9/qis/models/linear/ra_returns.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:08:28.691242 qis-1.0.9/qis/models/README.md
+-rw-r--r--   0        0        0        0 2021-12-04 12:08:05.000000 qis-1.0.9/qis/models/stats/__init__.py
+-rw-r--r--   0        0        0    19009 2023-01-08 14:55:40.000000 qis-1.0.9/qis/models/stats/bootstrap.py
+-rw-r--r--   0        0        0     8504 2023-01-08 14:55:40.000000 qis-1.0.9/qis/models/stats/gaussian_mixture.py
+-rw-r--r--   0        0        0     2319 2023-01-08 14:55:40.000000 qis-1.0.9/qis/models/stats/ohlc_vol.py
+-rw-r--r--   0        0        0     8556 2023-01-23 14:52:48.000000 qis-1.0.9/qis/models/stats/test_bootstrap.py
+-rw-r--r--   0        0        0     2432 2023-01-08 15:22:04.000000 qis-1.0.9/qis/perfstats/__init__.py
+-rw-r--r--   0        0        0     7178 2023-01-23 14:52:48.000000 qis-1.0.9/qis/perfstats/cond_regression.py
+-rw-r--r--   0        0        0    10871 2023-01-07 23:34:31.000000 qis-1.0.9/qis/perfstats/config.py
+-rw-r--r--   0        0        0     6243 2023-01-23 14:52:48.000000 qis-1.0.9/qis/perfstats/desc_table.py
+-rw-r--r--   0        0        0    18712 2023-01-23 14:52:48.000000 qis-1.0.9/qis/perfstats/perf_table.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:09:51.558354 qis-1.0.9/qis/perfstats/README.md
+-rw-r--r--   0        0        0    20097 2023-01-23 14:52:48.000000 qis-1.0.9/qis/perfstats/regime_classifier.py
+-rw-r--r--   0        0        0    30176 2023-01-23 14:52:48.000000 qis-1.0.9/qis/perfstats/returns.py
+-rw-r--r--   0        0        0     8315 2022-12-17 06:54:07.000000 qis-1.0.9/qis/perfstats/timeseries_bfill.py
+-rw-r--r--   0        0        0     3685 2023-01-23 14:03:45.000000 qis-1.0.9/qis/plots/__init__.py
+-rw-r--r--   0        0        0    17652 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/bars.py
+-rw-r--r--   0        0        0    18841 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/boxplot.py
+-rw-r--r--   0        0        0     3917 2023-01-07 22:17:49.000000 qis-1.0.9/qis/plots/contour.py
+-rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-1.0.9/qis/plots/derived/__init__.py
+-rw-r--r--   0        0        0     2196 2023-01-07 22:34:01.000000 qis-1.0.9/qis/plots/derived/data_timeseries.py
+-rw-r--r--   0        0        0     7410 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/drawdowns.py
+-rw-r--r--   0        0        0    16816 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/perf_table.py
+-rw-r--r--   0        0        0    21362 2023-01-23 15:53:29.000000 qis-1.0.9/qis/plots/derived/prices.py
+-rw-r--r--   0        0        0     3489 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/regime_class_table.py
+-rw-r--r--   0        0        0    11752 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/regime_data.py
+-rw-r--r--   0        0        0     3519 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/regime_pdf.py
+-rw-r--r--   0        0        0     6590 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/regime_scatter.py
+-rw-r--r--   0        0        0    19263 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/returns_heatmap.py
+-rw-r--r--   0        0        0     5011 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/derived/returns_scatter.py
+-rw-r--r--   0        0        0     4008 2023-01-22 21:00:17.781941 qis-1.0.9/qis/plots/errorbar.py
+-rw-r--r--   0        0        0     3643 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/heatmap.py
+-rw-r--r--   0        0        0    10375 2023-01-22 21:01:33.337414 qis-1.0.9/qis/plots/histogram.py
+-rw-r--r--   0        0        0     2917 2023-01-07 22:25:33.000000 qis-1.0.9/qis/plots/histplot2d.py
+-rw-r--r--   0        0        0     5383 2023-01-23 09:59:51.000000 qis-1.0.9/qis/plots/lineplot.py
+-rw-r--r--   0        0        0     1608 2023-01-07 22:25:33.000000 qis-1.0.9/qis/plots/pie.py
+-rw-r--r--   0        0        0     5744 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/qqplot.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:10:18.632797 qis-1.0.9/qis/plots/README.md
+-rw-r--r--   0        0        0    14041 2023-01-22 21:03:25.730816 qis-1.0.9/qis/plots/scatter.py
+-rw-r--r--   0        0        0     5975 2023-01-22 21:04:18.907813 qis-1.0.9/qis/plots/stackplot.py
+-rw-r--r--   0        0        0    14245 2023-01-22 21:07:08.019541 qis-1.0.9/qis/plots/table.py
+-rw-r--r--   0        0        0    21718 2023-01-23 15:57:49.000000 qis-1.0.9/qis/plots/time_series.py
+-rw-r--r--   0        0        0    54271 2023-01-23 14:52:48.000000 qis-1.0.9/qis/plots/utils.py
+-rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-1.0.9/qis/portfolio/__init__.py
+-rw-r--r--   0        0        0    11449 2023-01-23 14:52:48.000000 qis-1.0.9/qis/portfolio/backtester.py
+-rw-r--r--   0        0        0    30334 2023-01-23 14:03:45.000000 qis-1.0.9/qis/portfolio/multi_portfolio_data.py
+-rw-r--r--   0        0        0        0 2021-10-10 14:27:53.000000 qis-1.0.9/qis/portfolio/optimization/__init__.py
+-rw-r--r--   0        0        0    11693 2022-12-16 17:12:53.000000 qis-1.0.9/qis/portfolio/optimization/opt_solvers.py
+-rw-r--r--   0        0        0    20002 2022-09-02 13:03:58.000000 qis-1.0.9/qis/portfolio/optimization/qp_solvers.py
+-rw-r--r--   0        0        0    20538 2023-01-23 14:52:48.000000 qis-1.0.9/qis/portfolio/optimization/rolling_portfolios.py
+-rw-r--r--   0        0        0    34830 2023-01-23 14:03:45.000000 qis-1.0.9/qis/portfolio/portfolio_data.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:10:46.862039 qis-1.0.9/qis/portfolio/README.md
+-rw-r--r--   0        0        0        0 2021-03-26 11:07:46.000000 qis-1.0.9/qis/portfolio/reports/__init__.py
+-rw-r--r--   0        0        0    17477 2023-01-23 14:52:48.000000 qis-1.0.9/qis/portfolio/reports/multi_asset_factsheet.py
+-rw-r--r--   0        0        0    10867 2023-01-23 14:52:48.000000 qis-1.0.9/qis/portfolio/reports/multi_strategy_factsheet.py
+-rw-r--r--   0        0        0    13971 2023-01-23 14:52:48.000000 qis-1.0.9/qis/portfolio/reports/portfolio_factsheet.py
+-rw-r--r--   0        0        0    17937 2023-01-23 14:52:48.000000 qis-1.0.9/qis/portfolio/reports/strategy_factsheet.py
+-rw-r--r--   0        0        0        0 2022-12-17 17:53:19.000000 qis-1.0.9/qis/portfolio/strats/__init__.py
+-rw-r--r--   0        0        0     5778 2023-01-22 21:34:07.419353 qis-1.0.9/qis/portfolio/strats/quant_strats_delta1.py
+-rw-r--r--   0        0        0      463 2023-01-22 08:39:54.000000 qis-1.0.9/qis/read_qis_modules.py
+-rw-r--r--   0        0        0      477 2023-01-15 21:18:11.000000 qis-1.0.9/qis/settings.yaml
+-rw-r--r--   0        0        0      443 2023-01-15 20:14:44.000000 qis-1.0.9/qis/sql_engine.py
+-rw-r--r--   0        0        0     1199 2023-01-23 14:54:44.000000 qis-1.0.9/qis/test_data.py
+-rw-r--r--   0        0        0     5037 2023-01-23 08:10:14.000000 qis-1.0.9/qis/utils/__init__.py
+-rw-r--r--   0        0        0    43000 2023-01-23 05:28:35.000000 qis-1.0.9/qis/utils/dates.py
+-rw-r--r--   0        0        0     8942 2023-01-07 21:17:28.000000 qis-1.0.9/qis/utils/df_agg.py
+-rw-r--r--   0        0        0     8491 2023-01-08 13:32:37.000000 qis-1.0.9/qis/utils/df_cut.py
+-rw-r--r--   0        0        0     7812 2023-01-07 22:09:59.000000 qis-1.0.9/qis/utils/df_freq.py
+-rw-r--r--   0        0        0    10992 2023-01-07 21:37:16.000000 qis-1.0.9/qis/utils/df_groups.py
+-rw-r--r--   0        0        0     6819 2023-01-23 14:52:48.000000 qis-1.0.9/qis/utils/df_melt.py
+-rw-r--r--   0        0        0    27227 2023-01-23 10:47:10.000000 qis-1.0.9/qis/utils/df_ops.py
+-rw-r--r--   0        0        0     8295 2023-01-22 21:00:17.640637 qis-1.0.9/qis/utils/df_str.py
+-rw-r--r--   0        0        0    11344 2022-12-30 16:13:34.000000 qis-1.0.9/qis/utils/df_to_weights.py
+-rw-r--r--   0        0        0    10613 2023-01-23 21:13:51.001546 qis-1.0.9/qis/utils/generic.py
+-rw-r--r--   0        0        0    14809 2022-12-29 08:28:09.000000 qis-1.0.9/qis/utils/np_ops.py
+-rw-r--r--   0        0        0     5534 2023-01-22 21:03:25.729263 qis-1.0.9/qis/utils/ols.py
+-rw-r--r--   0        0        0       22 2023-01-23 21:14:19.545101 qis-1.0.9/qis/utils/README.md
+-rw-r--r--   0        0        0     4589 2022-12-17 17:01:53.000000 qis-1.0.9/qis/utils/sampling.py
+-rw-r--r--   0        0        0     5938 2022-12-16 21:08:07.680232 qis-1.0.9/qis/utils/struct_ops.py
+-rw-r--r--   0        0        0     4857 2023-01-23 21:37:06.052594 qis-1.0.9/README.md
+-rw-r--r--   0        0        0     6146 1970-01-01 00:00:00.000000 qis-1.0.9/setup.py
+-rw-r--r--   0        0        0     6828 1970-01-01 00:00:00.000000 qis-1.0.9/PKG-INFO
```

### Comparing `qis-1.0.8/LICENSE.txt` & `qis-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/pyproject.toml` & `qis-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2271 6973 220d 0a76 6572  ame = "qis"..ver
-00000020: 7369 6f6e 203d 2022 312e 302e 3822 0d0a  sion = "1.0.8"..
+00000020: 7369 6f6e 203d 2022 312e 302e 3922 0d0a  sion = "1.0.9"..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 2249  description = "I
 00000040: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
 00000050: 2076 6973 7561 6c69 7361 7469 6f6e 2061   visualisation a
 00000060: 6e64 2072 6570 6f72 7469 6e67 2061 6e61  nd reporting ana
 00000070: 6c79 7469 6373 2066 6f72 2051 7561 6e74  lytics for Quant
 00000080: 6974 6174 6976 6520 496e 7665 7374 6d65  itative Investme
 00000090: 6e74 2053 7472 6174 6567 6965 7322 0d0a  nt Strategies"..
```

### Comparing `qis-1.0.8/qis/__init__.py` & `qis-1.0.9/qis/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/asset_perf_report.py` & `qis-1.0.9/qis/examples/price_plots.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/gaussian_mixure_scatter.py` & `qis-1.0.9/qis/examples/gaussian_mixure_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/move_index.py` & `qis-1.0.9/qis/examples/move_index.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/plot_ust_rates.py` & `qis-1.0.9/qis/plots/pie.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,69 @@
-
-
+"""
+pieplot
+"""
+# built in
+import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
+from typing import Optional
 from enum import Enum
 
-from qis.data.ust_rates import load_ust_rates
-import qis
+# qis
+import qis.plots.utils as put
+
+
+def plot_pie(df: [pd.Series, pd.DataFrame],
+             y_column: str = None,
+             ax: plt.Subplot = None,
+             **kwargs
+             ) -> Optional[plt.Figure]:
 
+    if ax is None:
+        fig, ax = plt.subplots()
+    else:
+        fig = None
+
+    if y_column is None and isinstance(df, pd.DataFrame):
+        y_column = df.columns[0]
 
-def plot_ust_rates_data():
-    df = load_ust_rates()
+    df.plot.pie(y=y_column, ax=ax)
 
-    with sns.axes_style("darkgrid"):
-        fig, ax = plt.subplots(1, 1, figsize=(10, 10), tight_layout=True)
-        qis.plot_time_series(df=df,
-                             legend_stats=qis.LegendStats.FIRST_AVG_LAST,
-                             var_format='{:,.2f}',
-                             ax=ax)
-
-        fig, ax = plt.subplots(1, 1, figsize=(10, 10), tight_layout=True)
-        qis.plot_time_series(df=df[['3m', '10y']],
-                             legend_stats=qis.LegendStats.FIRST_AVG_LAST,
-                             var_format='{:,.2f}',
-                             ax=ax)
+    return fig
 
 
 class UnitTests(Enum):
-    PLOT_RATES = 1
+    PORTFOLIO = 1
 
 
 def run_unit_test(unit_test: UnitTests):
 
-    if unit_test == UnitTests.PLOT_RATES:
-        plot_ust_rates_data()
+    if unit_test == UnitTests.PORTFOLIO:
+
+        df = pd.DataFrame({'Conservative': [0.5, 0.25, 0.25],
+                           'Balanced': [0.30, 0.30, 0.40],
+                           'Growth': [0.10, 0.40, 0.50]},
+                          index=['Stables', 'Market-neutral', 'Crypto-Beta'])
+        print(df)
+        kwargs = dict(fontsize=8, linewidth=0.5, weight='normal', markersize=1)
+
+        with sns.axes_style("darkgrid"):
+            fig, ax = plt.subplots(1, 1, figsize=(8, 6))
+
+            plot_pie(df=df,
+                     ax=ax,
+                     **kwargs)
 
     plt.show()
 
 
 if __name__ == '__main__':
 
-    unit_test = UnitTests.PLOT_RATES
+    unit_test = UnitTests.PORTFOLIO
 
     is_run_all_tests = False
     if is_run_all_tests:
         for unit_test in UnitTests:
             run_unit_test(unit_test=unit_test)
     else:
         run_unit_test(unit_test=unit_test)
+
```

### Comparing `qis-1.0.8/qis/examples/portfolio_opt_backtest.py` & `qis-1.0.9/qis/examples/portfolio_opt_backtest.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/simulate_quant_strats.py` & `qis-1.0.9/qis/examples/simulate_quant_strats.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/test_ewm.py` & `qis-1.0.9/qis/examples/test_ewm.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/examples/test_scatter.py` & `qis-1.0.9/qis/examples/test_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/file_utils.py` & `qis-1.0.9/qis/file_utils.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/local_path.py` & `qis-1.0.9/qis/local_path.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/__init__.py` & `qis-1.0.9/qis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/auto_corr.py` & `qis-1.0.9/qis/models/linear/auto_corr.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/corr_cov_matrix.py` & `qis-1.0.9/qis/models/linear/corr_cov_matrix.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/ewm.py` & `qis-1.0.9/qis/models/linear/ewm.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/ewm_convolution.py` & `qis-1.0.9/qis/models/linear/ewm_convolution.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/ewm_factors.py` & `qis-1.0.9/qis/models/linear/ewm_factors.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/pca.py` & `qis-1.0.9/qis/models/linear/pca.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/plot_correlations.py` & `qis-1.0.9/qis/models/linear/plot_correlations.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/linear/ra_returns.py` & `qis-1.0.9/qis/models/linear/ra_returns.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/stats/bootstrap.py` & `qis-1.0.9/qis/models/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/stats/gaussian_mixture.py` & `qis-1.0.9/qis/models/stats/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/stats/ohlc_vol.py` & `qis-1.0.9/qis/models/stats/ohlc_vol.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/models/stats/test_bootstrap.py` & `qis-1.0.9/qis/models/stats/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/__init__.py` & `qis-1.0.9/qis/perfstats/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/cond_regression.py` & `qis-1.0.9/qis/perfstats/cond_regression.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/config.py` & `qis-1.0.9/qis/perfstats/config.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/desc_table.py` & `qis-1.0.9/qis/perfstats/desc_table.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/perf_table.py` & `qis-1.0.9/qis/perfstats/perf_table.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/regime_classifier.py` & `qis-1.0.9/qis/perfstats/regime_classifier.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/returns.py` & `qis-1.0.9/qis/perfstats/returns.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/perfstats/timeseries_bfill.py` & `qis-1.0.9/qis/perfstats/timeseries_bfill.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/__init__.py` & `qis-1.0.9/qis/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/bars.py` & `qis-1.0.9/qis/plots/bars.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/boxplot.py` & `qis-1.0.9/qis/plots/boxplot.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/contour.py` & `qis-1.0.9/qis/plots/contour.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/data_timeseries.py` & `qis-1.0.9/qis/plots/derived/data_timeseries.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/drawdowns.py` & `qis-1.0.9/qis/plots/derived/drawdowns.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/perf_table.py` & `qis-1.0.9/qis/plots/derived/perf_table.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/prices.py` & `qis-1.0.9/qis/plots/derived/prices.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,16 +107,17 @@
 
 def plot_prices(prices: Union[pd.DataFrame, pd.Series],
                 perf_params: PerfParams = None,
                 regime_benchmark_str: str = None,  # to add regimes
                 pivot_prices: pd.Series = None,
                 regime_params: BenchmarkReturnsQuantileRegimeSpecs = BenchmarkReturnsQuantileRegimeSpecs(),
                 var_format: str = '{:,.1f}',
-                digits_to_show: int = 2,
+                digits_to_show: int = 1,
                 sharpe_format: str = '{:.2f}',
+                x_date_freq: str = 'A',
                 trend_line: put.TrendLine = put.TrendLine.NONE,
                 is_log: bool = False,
                 resample_freq: str = None,
                 start_to_one: bool = True,
                 end_to_one: bool = False,
                 performance_label: PerformanceLabel = PerformanceLabel.DETAILED,
                 title: str = None,
@@ -145,14 +146,15 @@
 
     fig = pts.plot_time_series(df=prices,
                                trend_line=trend_line,
                                var_format=var_format,
                                title=title,
                                legend_labels=legend_labels,
                                is_log=is_log,
+                               x_date_freq=x_date_freq,
                                ax=ax,
                                **kwargs)
 
     if regime_benchmark_str is not None and regime_params is not None:
         add_bnb_regime_shadows(ax=ax,
                                data_df=prices,
                                pivot_prices=pivot_prices,
@@ -163,16 +165,17 @@
 
 def plot_prices_with_dd(prices: Union[pd.DataFrame, pd.Series],
                         perf_params: PerfParams = None,
                         regime_benchmark_str: str = None,  # to add regimes
                         pivot_prices: pd.Series = None,
                         regime_params: BenchmarkReturnsQuantileRegimeSpecs = BenchmarkReturnsQuantileRegimeSpecs(),
                         var_format: str = '{:,.1f}',
-                        digits_to_show: int = 2,
+                        digits_to_show: int = 1,
                         sharpe_format: str = '{:.2f}',
+                        x_date_freq: str = 'A',
                         performance_label: PerformanceLabel = PerformanceLabel.WITH_DD,
                         is_log: bool = False,
                         is_remove_xticklabels_ax1: bool = True,
                         title: str = 'Performance',
                         dd_title: str = 'Running Drawdown',
                         dd_legend_type: dra.DdLegendType = dra.DdLegendType.NONE,
                         axs: List[plt.Subplot] = None,
@@ -189,22 +192,24 @@
 
     plot_prices(prices=prices,
                 perf_params=perf_params,
                 var_format=var_format,
                 digits_to_show=digits_to_show,
                 sharpe_format=sharpe_format,
                 performance_label=performance_label,
+                x_date_freq=x_date_freq,
                 title=title,
                 is_log=is_log,
                 ax=axs[0],
                 **kwargs)
 
     dra.plot_drawdown(prices=prices,
                       perf_params=perf_params,
                       dd_legend_type=dd_legend_type,
+                      x_date_freq=x_date_freq,
                       title=dd_title,
                       ax=axs[1],
                       **kwargs)
 
     if is_remove_xticklabels_ax1:
         axs[0].set_xticklabels('')
```

### Comparing `qis-1.0.8/qis/plots/derived/regime_class_table.py` & `qis-1.0.9/qis/plots/derived/regime_class_table.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/regime_data.py` & `qis-1.0.9/qis/plots/derived/regime_data.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/regime_pdf.py` & `qis-1.0.9/qis/plots/derived/regime_pdf.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/regime_scatter.py` & `qis-1.0.9/qis/plots/derived/regime_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/returns_heatmap.py` & `qis-1.0.9/qis/plots/derived/returns_heatmap.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/derived/returns_scatter.py` & `qis-1.0.9/qis/plots/derived/returns_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/errorbar.py` & `qis-1.0.9/qis/plots/errorbar.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/heatmap.py` & `qis-1.0.9/qis/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/histogram.py` & `qis-1.0.9/qis/plots/histogram.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/histplot2d.py` & `qis-1.0.9/qis/plots/histplot2d.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/lineplot.py` & `qis-1.0.9/qis/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/qqplot.py` & `qis-1.0.9/qis/plots/qqplot.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/scatter.py` & `qis-1.0.9/qis/plots/scatter.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/stackplot.py` & `qis-1.0.9/qis/plots/stackplot.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/table.py` & `qis-1.0.9/qis/plots/table.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/plots/time_series.py` & `qis-1.0.9/qis/plots/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                      markersize: int = None,
                      colors: List[str] = None,
                      x_limits: Tuple[Union[float, None], Union[float, None]] = None,
                      y_limits: Tuple[Optional[float], Optional[float]] = None,
                      is_log: bool = False,
                      ax: plt.Subplot = None,
                      **kwargs
-                     ) -> plt.Figure:
+                     ) -> Optional[plt.Figure]:
 
     if trend_line in [TrendLine.AVERAGE, TrendLine.AVERAGE_SHADOWS, TrendLine.ZERO_SHADOWS,
                       TrendLine.TREND_LINE, TrendLine.TREND_LINE_SHADOWS]:  # these features are only available with sns
         is_use_sns_lineplot = True
 
     data1 = df.copy()
     if isinstance(data1, pd.DataFrame):
```

### Comparing `qis-1.0.8/qis/plots/utils.py` & `qis-1.0.9/qis/plots/utils.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/backtester.py` & `qis-1.0.9/qis/portfolio/backtester.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/multi_portfolio_data.py` & `qis-1.0.9/qis/portfolio/multi_portfolio_data.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/optimization/opt_solvers.py` & `qis-1.0.9/qis/portfolio/optimization/opt_solvers.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/optimization/qp_solvers.py` & `qis-1.0.9/qis/portfolio/optimization/qp_solvers.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/optimization/rolling_portfolios.py` & `qis-1.0.9/qis/portfolio/optimization/rolling_portfolios.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/portfolio_data.py` & `qis-1.0.9/qis/portfolio/portfolio_data.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/reports/multi_asset_factsheet.py` & `qis-1.0.9/qis/portfolio/reports/multi_asset_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/reports/multi_strategy_factsheet.py` & `qis-1.0.9/qis/portfolio/reports/multi_strategy_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/reports/portfolio_factsheet.py` & `qis-1.0.9/qis/portfolio/reports/portfolio_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/reports/strategy_factsheet.py` & `qis-1.0.9/qis/portfolio/reports/strategy_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/portfolio/strats/quant_strats_delta1.py` & `qis-1.0.9/qis/portfolio/strats/quant_strats_delta1.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/test_data.py` & `qis-1.0.9/qis/test_data.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/__init__.py` & `qis-1.0.9/qis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/dates.py` & `qis-1.0.9/qis/utils/dates.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_agg.py` & `qis-1.0.9/qis/utils/df_agg.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_cut.py` & `qis-1.0.9/qis/utils/df_cut.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_freq.py` & `qis-1.0.9/qis/utils/df_freq.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_groups.py` & `qis-1.0.9/qis/utils/df_groups.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_melt.py` & `qis-1.0.9/qis/utils/df_melt.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_ops.py` & `qis-1.0.9/qis/utils/df_ops.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_str.py` & `qis-1.0.9/qis/utils/df_str.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/df_to_weights.py` & `qis-1.0.9/qis/utils/df_to_weights.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/generic.py` & `qis-1.0.9/qis/utils/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 
-
-
 # built in
-
-# qis
-
-
-
+import numpy as np
+import pandas as pd
 from dataclasses import dataclass
 from enum import Enum
 from typing import NamedTuple, Optional, Callable, Dict, List
 
-import numpy as np
-import pandas as pd
-
-from qis import file_utils as fu
-from qis.utils import df_groups as dfg, df_agg as dfa, struct_ops as sop, df_to_str as dff
+# qis
+import qis.file_utils as fu
+import qis.utils.df_groups as dfg
+import qis.utils.df_agg as dfa
+import qis.utils.struct_ops as sop
+import qis.utils.df_str as dff
 
 DATE_FORMAT = '%d%b%y' # short y for meta
 
 
 class ValueType(Enum):
     FLOAT0 = 0
     FLOAT = 1
```

### Comparing `qis-1.0.8/qis/utils/np_ops.py` & `qis-1.0.9/qis/utils/np_ops.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/ols.py` & `qis-1.0.9/qis/utils/ols.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/sampling.py` & `qis-1.0.9/qis/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `qis-1.0.8/qis/utils/struct_ops.py` & `qis-1.0.9/qis/utils/struct_ops.py`

 * *Files identical despite different names*

