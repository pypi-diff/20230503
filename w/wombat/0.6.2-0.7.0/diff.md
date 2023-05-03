# Comparing `tmp/wombat-0.6.2.tar.gz` & `tmp/wombat-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombat-0.6.2.tar", last modified: Fri Feb  3 17:24:43 2023, max compression
+gzip compressed data, was "wombat-0.7.0.tar", last modified: Wed May  3 02:43:09 2023, max compression
```

## Comparing `wombat-0.6.2.tar` & `wombat-0.7.0.tar`

### file list

```diff
@@ -1,268 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.579330 wombat-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-02-03 17:24:20.000000 wombat-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-02-03 17:24:43.579330 wombat-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-02-03 17:24:20.000000 wombat-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.531329 wombat-0.6.2/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.531329 wombat-0.6.2/library/code_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.531329 wombat-0.6.2/library/code_comparison/dinwoodie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.531329 wombat-0.6.2/library/code_comparison/dinwoodie/cables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/cables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/cables/array.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/cables/export.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.531329 wombat-0.6.2/library/code_comparison/dinwoodie/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.539329 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/
--rw-r--r--   0 runner    (1001) docker     (123)   151012 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/SAM_Singleowner_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/annual_service_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/annual_service_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base_downtime.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base_requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base_scheduled.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base_tow_to_port.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/failure_200.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/failure_200_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/failure_50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/failure_50_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fewer_ctvs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fewer_ctvs_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fewer_techs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fewer_techs_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fixed_costs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fixed_costs_fewer_techs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fixed_costs_more_ctvs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/fixed_costs_more_techs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/historic_weather.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/historic_weather_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/major_repairs_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/major_repairs_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/major_replacements_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/major_replacements_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/manual_resets_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/manual_resets_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/medium_repairs_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/medium_repairs_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/minor_repairs_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/minor_repairs_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/more_ctvs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/more_ctvs_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/more_techs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/more_techs_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/no_hlvs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/no_hlvs_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/no_weather.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/config/no_weather_100pct_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.543330 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_200.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_200_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_50.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_50_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs_100pct_reduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_port_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_tow_to_port.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.543330 wombat-0.6.2/library/code_comparison/dinwoodie/project/port/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/project/port/base_port.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.547330 wombat-0.6.2/library/code_comparison/dinwoodie/results/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_19-50-53.804474_dinwoodie_base_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_19-53-40.511520_dinwoodie_more_ctvs_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_19-56-35.783433_dinwoodie_fewer_ctvs_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_19-59-33.470119_dinwoodie_more_techs_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-02-25.817560_dinwoodie_fewer_techs_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-05-17.573115_dinwoodie_failure_50_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-07-45.654330_dinwoodie_failure_200_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-11-33.724653_dinwoodie_no_hlvs_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-14-51.236890_dinwoodie_no_weather_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-17-54.871961_dinwoodie_historic_weather_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-20-29.841287_dinwoodie_manual_resets_only_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-22-51.475426_dinwoodie_minor_repairs_only_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-24-53.150464_dinwoodie_medium_repairs_only_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-26-43.081550_dinwoodie_major_repairs_only_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-28-27.409791_dinwoodie_major_replacements_only_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/2022-02-04_20-30-20.875717_dinwoodie_annual_service_only_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_100pct_reduction_v0.4.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_v0.4.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_v0.4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_v0.5.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_100pct_reduction_v0.4.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_v0.4.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18785 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_v0.4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_v0.5.1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.547330 wombat-0.6.2/library/code_comparison/dinwoodie/substations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/substations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/substations/offshore_substation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.551330 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_delete.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_power_curve.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_tow_to_port.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.551330 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/ctv1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/ctv2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/ctv3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/ctv4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/ctv5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/fsv_downtime.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/fsv_requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/fsv_scheduled.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_1_scheduled.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_2_scheduled.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_3_scheduled.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_downtime.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/tugboat1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/tugboat2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/vessels/tugboat3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.555330 wombat-0.6.2/library/code_comparison/dinwoodie/weather/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4252247 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1998694 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014_zeros.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.559330 wombat-0.6.2/library/code_comparison/iea26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.559330 wombat-0.6.2/library/code_comparison/iea26/cables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/cables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/cables/array_33kv_240mm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/cables/array_33kv_630mm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/cables/export_220kv_1600mm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.559330 wombat-0.6.2/library/code_comparison/iea26/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.563330 wombat-0.6.2/library/code_comparison/iea26/project/config/
--rw-r--r--   0 runner    (1001) docker     (123)   151012 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/SAM_Singleowner_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/fixed_costs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/one_mobilization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/one_mobilization_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/requests_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/three_mobilizations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/three_mobilizations_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/two_mobilizations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/config/two_mobilizations_100pct_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.563330 wombat-0.6.2/library/code_comparison/iea26/project/plant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/plant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/plant/layout.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/plant/layout_100pct_reduction.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.563330 wombat-0.6.2/library/code_comparison/iea26/project/port/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/project/port/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.563330 wombat-0.6.2/library/code_comparison/iea26/results/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/2022-02-04_18-43-00.190127_iea_26_one_mobilization_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/2022-02-04_18-51-33.657200_iea_26_one_mobilization_100pct_reduction_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/2022-02-04_18-59-35.103268_iea_26_two_mobilizations_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/2022-02-04_19-11-18.237564_iea_26_two_mobilizations_100pct_reduction_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/2022-02-04_19-21-59.432951_iea_26_three_mobilizations_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/2022-02-04_19-35-03.157461_iea_26_three_mobilizations_100pct_reduction_metrics_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_data_v0.4.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_data_v0.4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_data_v0.5.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_dict_v0.4.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_dict_v0.4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/results/results_dict_v0.5.1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.563330 wombat-0.6.2/library/code_comparison/iea26/substations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/substations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/substations/offshore_substation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/substations/offshore_substation_100pct_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.563330 wombat-0.6.2/library/code_comparison/iea26/turbines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/turbines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/turbines/turbine_csm_4mw.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/turbines/turbine_csm_4mw_100pct_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/turbines/turbine_csm_4mw_power_curve.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.567330 wombat-0.6.2/library/code_comparison/iea26/vessels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/cabling_requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/cabling_scheduled.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/ctv1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/ctv2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/dsv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/dsv_requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/hlv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/vessels/rmt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.567330 wombat-0.6.2/library/code_comparison/iea26/weather/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  6542692 2023-02-03 17:24:21.000000 wombat-0.6.2/library/code_comparison/iea26/weather/hornsrev3_weather_1996_2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-03 17:24:22.000000 wombat-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 17:24:43.579330 wombat-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-03 17:24:22.000000 wombat-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.575330 wombat-0.6.2/wombat/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.575330 wombat-0.6.2/wombat/core/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79270 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31595 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    85754 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18383 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/repair_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    69630 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/service_equipment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16721 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/core/simulation_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.575330 wombat-0.6.2/wombat/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/utilities/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.579330 wombat-0.6.2/wombat/windfarm/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/windfarm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.579330 wombat-0.6.2/wombat/windfarm/system/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/windfarm/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/windfarm/system/cable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/windfarm/system/subassembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/windfarm/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-02-03 17:24:22.000000 wombat-0.6.2/wombat/windfarm/windfarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:24:43.575330 wombat-0.6.2/wombat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-02-03 17:24:43.000000 wombat-0.6.2/wombat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-02-03 17:24:43.000000 wombat-0.6.2/wombat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:24:43.000000 wombat-0.6.2/wombat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-03 17:24:43.000000 wombat-0.6.2/wombat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-03 17:24:43.000000 wombat-0.6.2/wombat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.569509 wombat-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-03 02:42:51.000000 wombat-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-03 02:43:09.569509 wombat-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-03 02:42:51.000000 wombat-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.529509 wombat-0.7.0/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.529509 wombat-0.7.0/library/code_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.529509 wombat-0.7.0/library/code_comparison/dinwoodie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.533509 wombat-0.7.0/library/code_comparison/dinwoodie/cables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/cables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/cables/array.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/cables/export.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.533509 wombat-0.7.0/library/code_comparison/dinwoodie/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.537510 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/
+-rw-r--r--   0 runner    (1001) docker     (123)   151012 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/SAM_Singleowner_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/annual_service_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/annual_service_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base_downtime.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base_requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base_scheduled.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base_tow_to_port.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/failure_200.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/failure_200_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/failure_50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/failure_50_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fewer_ctvs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fewer_ctvs_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fewer_techs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fewer_techs_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fixed_costs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fixed_costs_fewer_techs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fixed_costs_more_ctvs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/fixed_costs_more_techs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/historic_weather.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/historic_weather_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/major_repairs_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/major_repairs_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/major_replacements_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/major_replacements_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/manual_resets_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/manual_resets_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/medium_repairs_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/medium_repairs_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/minor_repairs_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/minor_repairs_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/more_ctvs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/more_ctvs_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/more_techs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/more_techs_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/no_hlvs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/no_hlvs_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/no_weather.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/config/no_weather_100pct_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.541509 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_200.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_200_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_50.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_50_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs_100pct_reduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_port_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_tow_to_port.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.541509 wombat-0.7.0/library/code_comparison/dinwoodie/project/port/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/project/port/base_port.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.541509 wombat-0.7.0/library/code_comparison/dinwoodie/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_100pct_reduction_v0.4.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_v0.4.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_v0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_v0.5.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_100pct_reduction_v0.4.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_v0.4.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18785 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_v0.4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_v0.5.1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.541509 wombat-0.7.0/library/code_comparison/dinwoodie/substations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/substations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/substations/offshore_substation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.545509 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_power_curve.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_tow_to_port.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.545509 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/ctv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/ctv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/ctv3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/ctv4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/ctv5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/fsv_downtime.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/fsv_requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/fsv_scheduled.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_1_scheduled.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_2_scheduled.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_3_scheduled.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_downtime.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/tugboat1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/tugboat2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/vessels/tugboat3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.549509 wombat-0.7.0/library/code_comparison/dinwoodie/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4252247 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1998694 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014_zeros.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.553509 wombat-0.7.0/library/code_comparison/iea26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.553509 wombat-0.7.0/library/code_comparison/iea26/cables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/cables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/cables/array_33kv_240mm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/cables/array_33kv_630mm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/cables/export_220kv_1600mm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.553509 wombat-0.7.0/library/code_comparison/iea26/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.553509 wombat-0.7.0/library/code_comparison/iea26/project/config/
+-rw-r--r--   0 runner    (1001) docker     (123)   151012 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/SAM_Singleowner_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/fixed_costs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/one_mobilization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/one_mobilization_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/requests_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/three_mobilizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/three_mobilizations_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/two_mobilizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/config/two_mobilizations_100pct_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.553509 wombat-0.7.0/library/code_comparison/iea26/project/plant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/plant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/plant/layout.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/plant/layout_100pct_reduction.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.553509 wombat-0.7.0/library/code_comparison/iea26/project/port/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/project/port/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.557509 wombat-0.7.0/library/code_comparison/iea26/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_data_v0.4.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_data_v0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_data_v0.5.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_dict_v0.4.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_dict_v0.4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/results/results_dict_v0.5.1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.557509 wombat-0.7.0/library/code_comparison/iea26/substations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/substations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/substations/offshore_substation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/substations/offshore_substation_100pct_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.557509 wombat-0.7.0/library/code_comparison/iea26/turbines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/turbines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/turbines/turbine_csm_4mw.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/turbines/turbine_csm_4mw_100pct_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/turbines/turbine_csm_4mw_power_curve.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.557509 wombat-0.7.0/library/code_comparison/iea26/vessels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/cabling_requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/cabling_scheduled.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/ctv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/ctv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/dsv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/dsv_requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/hlv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/vessels/rmt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.557509 wombat-0.7.0/library/code_comparison/iea26/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  6542692 2023-05-03 02:42:52.000000 wombat-0.7.0/library/code_comparison/iea26/weather/hornsrev3_weather_1996_2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-03 02:42:53.000000 wombat-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:43:09.569509 wombat-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-03 02:42:53.000000 wombat-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.565509 wombat-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_cable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_repair_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76102 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_service_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_simulation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_subassembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-03 02:42:53.000000 wombat-0.7.0/tests/test_windfarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.565509 wombat-0.7.0/wombat/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.569509 wombat-0.7.0/wombat/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82396 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32814 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86307 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/repair_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71885 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/service_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/core/simulation_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.569509 wombat-0.7.0/wombat/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/utilities/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.569509 wombat-0.7.0/wombat/windfarm/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/windfarm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.569509 wombat-0.7.0/wombat/windfarm/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/windfarm/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/windfarm/system/cable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/windfarm/system/subassembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/windfarm/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20840 2023-05-03 02:42:53.000000 wombat-0.7.0/wombat/windfarm/windfarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:43:09.565509 wombat-0.7.0/wombat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-03 02:43:09.000000 wombat-0.7.0/wombat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-05-03 02:43:09.000000 wombat-0.7.0/wombat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:43:09.000000 wombat-0.7.0/wombat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-03 02:43:09.000000 wombat-0.7.0/wombat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 02:43:09.000000 wombat-0.7.0/wombat.egg-info/top_level.txt
```

### Comparing `wombat-0.6.2/LICENSE` & `wombat-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/PKG-INFO` & `wombat-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wombat
-Version: 0.6.2
+Version: 0.7.0
 Summary: Windfarm operations and maintenance cost-benefit analysis tool
 Author: Rob Hammond
 Author-email: rob.hammond@nrel.gov
 Project-URL: Source, https://github.com/WISDEM/WOMBAT
 Project-URL: Documentation, https://wisdem.github.io/WOMBAT/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wombat-0.6.2/README.md` & `wombat-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/config/SAM_Singleowner_defaults.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/config/SAM_Singleowner_defaults.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/config/base.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/config/base.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_annual_service_only_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_200.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_200.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_200_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_200_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_50.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_50.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_failure_50_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_failure_50_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_repairs_only_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_major_replacements_only_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_manual_resets_only_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_medium_repairs_only_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_no_hlvs_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_port_test.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_port_test.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/project/plant/layout_tow_to_port.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/project/plant/layout_tow_to_port.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_100pct_reduction_v0.4.1.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_100pct_reduction_v0.4.1.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_v0.4.1.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_v0.4.1.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_v0.4.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_v0.4.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_data_v0.5.1.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_data_v0.5.1.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_100pct_reduction_v0.4.1.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_100pct_reduction_v0.4.1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_v0.4.1.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_v0.4.1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_v0.4.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_v0.4.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/results/results_dict_v0.5.1.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/results/results_dict_v0.5.1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -50,11 +50,11 @@
       description: major repair
     5:
       scale: 12.5
       shape: 1
       time: 52
       materials: 334500
       service_equipment: LCN
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_annual_service_only_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200_100pct_reduction.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,42 @@
   failures:
     1:
       scale: 0.0667
       shape: 1
       time: 3
       materials: 0
       service_equipment: CTV
-      operation_reduction: 0.0
+      operation_reduction: 1.0
       level: 1
       description: manual reset
     2:
       scale: 0.1667
       shape: 1
       time: 7.5
       materials: 1000
       service_equipment: CTV
-      operation_reduction: 0.0
+      operation_reduction: 1.0
       level: 2
       description: minor repair
     3:
       scale: 1.8182
       shape: 1
       time: 22
       materials: 18500
       service_equipment: CTV
-      operation_reduction: 0.0
+      operation_reduction: 1.0
       level: 3
       description: medium repair
     4:
       scale: 12.5
       shape: 1
       time: 26
       materials: 73500
       service_equipment: SCN
-      operation_reduction: 0.0
+      operation_reduction: 1.0
       level: 4
       description: major repair
     5:
       scale: 6.25
       shape: 1
       time: 52
       materials: 334500
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_200.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -14,47 +14,47 @@
   failures:
     1:
       scale: 0.0667
       shape: 1
       time: 3
       materials: 0
       service_equipment: CTV
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       level: 1
       description: manual reset
     2:
       scale: 0.1667
       shape: 1
       time: 7.5
       materials: 1000
       service_equipment: CTV
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       level: 2
       description: minor repair
     3:
       scale: 1.8182
       shape: 1
       time: 22
       materials: 18500
       service_equipment: CTV
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       level: 3
       description: medium repair
     4:
       scale: 12.5
       shape: 1
       time: 26
       materials: 73500
       service_equipment: SCN
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       level: 4
       description: major repair
     5:
       scale: 6.25
       shape: 1
       time: 52
       materials: 334500
       service_equipment: LCN
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_tow_to_port.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -9,52 +9,52 @@
   - description: annual service
     time: 60
     materials: 18500
     service_equipment: CTV
     frequency: 365
   failures:
     1:
-      scale: 0.2666
+      scale: 0.1333
       shape: 1
       time: 3
       materials: 0
       service_equipment: CTV
       operation_reduction: 0.0
       level: 1
       description: manual reset
     2:
-      scale: 0.6667
+      scale: 0.3333
       shape: 1
       time: 7.5
       materials: 1000
       service_equipment: CTV
       operation_reduction: 0.0
       level: 2
       description: minor repair
     3:
-      scale: 7.2726
+      scale: 3.6363
       shape: 1
       time: 22
       materials: 18500
       service_equipment: CTV
       operation_reduction: 0.0
       level: 3
       description: medium repair
     4:
-      scale: 50
+      scale: 25
       shape: 1
       time: 26
       materials: 73500
-      service_equipment: SCN
+      service_equipment: TOW
       operation_reduction: 0.0
       level: 4
       description: major repair
     5:
-      scale: 25
+      scale: 12.5
       shape: 1
       time: 52
       materials: 334500
-      service_equipment: LCN
-      operation_reduction: 1.0
+      service_equipment: TOW
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_repairs_only_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -50,11 +50,11 @@
       description: major repair
     5:
       scale: 12.5
       shape: 1
       time: 52
       materials: 334500
       service_equipment: LCN
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_major_replacements_only_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_manual_resets_only_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_medium_repairs_only_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -50,11 +50,11 @@
       description: major repair
     5:
       scale: 0
       shape: 0
       time: 0
       materials: 0
       service_equipment: LCN
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_minor_repairs_only_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_no_hlvs_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/turbines/vestas_v90_tow_to_port.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/turbines/vestas_v90_failure_50.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -9,52 +9,52 @@
   - description: annual service
     time: 60
     materials: 18500
     service_equipment: CTV
     frequency: 365
   failures:
     1:
-      scale: 0.1333
+      scale: 0.2666
       shape: 1
       time: 3
       materials: 0
       service_equipment: CTV
       operation_reduction: 0.0
       level: 1
       description: manual reset
     2:
-      scale: 0.3333
+      scale: 0.6667
       shape: 1
       time: 7.5
       materials: 1000
       service_equipment: CTV
       operation_reduction: 0.0
       level: 2
       description: minor repair
     3:
-      scale: 3.6363
+      scale: 7.2726
       shape: 1
       time: 22
       materials: 18500
       service_equipment: CTV
       operation_reduction: 0.0
       level: 3
       description: medium repair
     4:
-      scale: 25
+      scale: 50
       shape: 1
       time: 26
       materials: 73500
-      service_equipment: TOW
+      service_equipment: SCN
       operation_reduction: 0.0
       level: 4
       description: major repair
     5:
-      scale: 12.5
+      scale: 25
       shape: 1
       time: 52
       materials: 334500
-      service_equipment: TOW
-      operation_reduction: 1.0
+      service_equipment: LCN
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
```

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_1_scheduled.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_1_scheduled.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_2_scheduled.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_2_scheduled.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/vessels/hlv_3_scheduled.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/vessels/hlv_3_scheduled.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/vessels/tugboat1.yaml` & `wombat-0.7.0/library/code_comparison/dinwoodie/vessels/tugboat1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014_zeros.csv` & `wombat-0.7.0/library/code_comparison/dinwoodie/weather/alpha_ventus_weather_2002_2014_zeros.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/project/config/SAM_Singleowner_defaults.yaml` & `wombat-0.7.0/library/code_comparison/iea26/project/config/SAM_Singleowner_defaults.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/project/plant/layout.csv` & `wombat-0.7.0/library/code_comparison/iea26/project/plant/layout.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/project/plant/layout_100pct_reduction.csv` & `wombat-0.7.0/library/code_comparison/iea26/project/plant/layout_100pct_reduction.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_data.csv` & `wombat-0.7.0/library/code_comparison/iea26/results/results_data.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_data_v0.4.1.csv` & `wombat-0.7.0/library/code_comparison/iea26/results/results_data_v0.4.1.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_data_v0.4.csv` & `wombat-0.7.0/library/code_comparison/iea26/results/results_data_v0.4.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_data_v0.5.1.csv` & `wombat-0.7.0/library/code_comparison/iea26/results/results_data_v0.5.1.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_dict_v0.4.1.yaml` & `wombat-0.7.0/library/code_comparison/iea26/results/results_dict_v0.4.1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_dict_v0.4.yaml` & `wombat-0.7.0/library/code_comparison/iea26/results/results_dict_v0.4.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/results/results_dict_v0.5.1.yaml` & `wombat-0.7.0/library/code_comparison/iea26/results/results_dict_v0.5.1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/substations/offshore_substation.yaml` & `wombat-0.7.0/library/code_comparison/iea26/substations/offshore_substation.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/substations/offshore_substation_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/iea26/substations/offshore_substation_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/turbines/turbine_csm_4mw.yaml` & `wombat-0.7.0/library/code_comparison/iea26/turbines/turbine_csm_4mw.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       description: major repair
     5:
       scale: 9.0909
       shape: 1
       time: 41.5  # has 7.5hr inspection time baked in
       materials: 441373
       service_equipment: LCN
-      operation_reduction: 1.0
+      operation_reduction: 0.0
       replacement: true
       level: 5
       description: major replacement
 supporting_structure:
   name: supporting_structure
   maintenance:
   - description: structure inspection
```

### Comparing `wombat-0.6.2/library/code_comparison/iea26/turbines/turbine_csm_4mw_100pct_reduction.yaml` & `wombat-0.7.0/library/code_comparison/iea26/turbines/turbine_csm_4mw_100pct_reduction.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/cabling_requests.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/cabling_requests.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/ctv1.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/ctv1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/ctv2.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/ctv2.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/hlv.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/hlv.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_1.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_1.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_2.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_2.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_3.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_3.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/vessels/hlv_requests.yaml` & `wombat-0.7.0/library/code_comparison/iea26/vessels/hlv_requests.yaml`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/library/code_comparison/iea26/weather/hornsrev3_weather_1996_2015.csv` & `wombat-0.7.0/library/code_comparison/iea26/weather/hornsrev3_weather_1996_2015.csv`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/setup.py` & `wombat-0.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 
 HERE = Path(__file__).parent
 
-with open(HERE / "README.md", "r", newline="") as readme:
+with open(HERE / "README.md", newline="") as readme:
     long_description = readme.read()
     long_description_content_type = "text/markdown"
 
 
 def read(relative_path: Path | str) -> str:
     """Reads the `relative_path` file."""
     with codecs.open(str(HERE / relative_path), "r") as fp:
@@ -61,22 +61,23 @@
     "flake8>=5",
     "flake8-docstrings>=1.6",
     "flake8_sphinx_links==0.2.1",
     "black>=22.1",
     "isort>=5.10",
     "pytest>=7",
     "pytest-cov>=4",
-    "mypy>=0.991",
+    "mypy==0.991",
+    "ruff==0.0.246",
 ]
 DOCUMENTATION = [
     "Sphinx==4.*",
     "myst-nb>=0.16",
     "myst-parser>=0.17",
     "sphinx-panels>=0.6",
-    "sphinx-book-theme>=0.3.3",
+    "sphinx-book-theme>=0.3.3,<1",
     "sphinxcontrib-spelling>=7",
     "linkify-it-py>=2",
     "sphinxcontrib-bibtex>=2.4",
 ]
 extra_package_requirements = {
     "dev": DEVELOPER,
     "docs": DOCUMENTATION,
```

### Comparing `wombat-0.6.2/wombat/core/__init__.py` & `wombat-0.7.0/wombat/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-"""
-Initializes the simulation modules, classes, and functions.
+"""Initializes the simulation modules, classes, and functions."""
 
-isort:skip_file
-"""
 
 from .data_classes import (
     Maintenance,
     Failure,
     SubassemblyData,
     RepairRequest,
     ServiceEquipmentData,
```

### Comparing `wombat-0.6.2/wombat/core/data_classes.py` & `wombat-0.7.0/wombat/core/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import attr
 import attrs
 import numpy as np
 import pandas as pd
 from attrs import Factory, Attribute, field, define
 from scipy.stats import weibull_min
 
-from wombat.utilities import HOURS_IN_DAY, HOURS_IN_YEAR
-from wombat.utilities.time import parse_date
+from wombat.utilities.time import HOURS_IN_DAY, HOURS_IN_YEAR, parse_date
 
 
 if TYPE_CHECKING:
     from wombat.core import ServiceEquipment
 
 
 # Define the valid servicing equipment types
@@ -30,42 +29,41 @@
     "SCN",  # Small crane
     "LCN",  # Large crane
     "CAB",  # Cabling equipment
     "RMT",  # Remote reset or anything performed remotely
     "DRN",  # Drone
     "DSV",  # Diving support vessel
     "TOW",  # Tugboat or support vessel for moving a turbine to a repair facility
-    "AHV",  # Anchor handling vessel, tpyically a tugboat, but doesn't trigger tow-to-port
+    "AHV",  # Anchor handling vessel, typically a tugboat, w/o trigger tow-to-port
 )
 
 # Define the valid unscheduled and valid strategies
 UNSCHEDULED_STRATEGIES = ("requests", "downtime")
 VALID_STRATEGIES = tuple(["scheduled"] + list(UNSCHEDULED_STRATEGIES))
 
 
 def convert_to_list(
     value: Sequence | str | int | float,
     manipulation: Callable | None = None,
 ) -> list:
-    """Converts an unknown element that could be a list or single, non-sequence element
+    """Convert an unknown element that could be a list or single, non-sequence element
     to a list of elements.
 
     Parameters
     ----------
     value : Sequence | str | int | float
         The unknown element to be converted to a list of element(s).
     manipulation: Callable | None
         A function to be performed upon the individual elements, by default None.
 
     Returns
     -------
     list
         The new list of elements.
     """
-
     if isinstance(value, (str, int, float)):
         value = [value]
     if manipulation is not None:
         return [manipulation(el) for el in value]
     return list(value)
 
 
@@ -73,15 +71,15 @@
 update_wrapper(convert_to_list_upper, convert_to_list)
 
 convert_to_list_lower = partial(convert_to_list, manipulation=str.lower)
 update_wrapper(convert_to_list_lower, convert_to_list)
 
 
 def clean_string_input(value: str | None) -> str | None:
-    """Converts a string to lower case and and removes leading and trailing white spaces.
+    """Convert a string to lower case and and removes leading and trailing white spaces.
 
     Parameters
     ----------
     value: str
         The user input string.
 
     Returns
@@ -98,15 +96,15 @@
     start_day: int,
     end_day: int,
     start_month: int,
     end_month: int,
     start_year: int,
     end_year: int,
 ) -> np.ndarray:
-    """Creates a series of date ranges across multiple years between the starting date
+    """Create a series of date ranges across multiple years between the starting date
     and ending date for each year from starting year to ending year. Will only work if
     the end year is the same as the starting year or later, and the ending month, day
     combinatoion is after the starting month, day combination.
 
     Parameters
     ----------
     start_day : int
@@ -125,30 +123,30 @@
     Raises
     ------
     ValueError: Raised if the ending month, day combination occur after the starting
         month, day combination.
     ValueError: Raised if the ending year is prior to the starting year.
 
     Yields
-    -------
+    ------
     np.ndarray
         A ``numpy.ndarray`` of ``datetime.date`` objects.
     """
     # Check the year bounds
     if end_year < start_year:
         raise ValueError(
             f"The end_year ({start_year}) is later than the start_year ({end_year})."
         )
 
     # Check the month, date combination bounds
     start = datetime.datetime(2022, start_month, start_day)
     end = datetime.datetime(2022, end_month, end_day)
     if end < start:
         raise ValueError(
-            f"The starting month and day {start} is after the ending month and day {end}."
+            f"The starting month/day combination: {start}, is after the ending: {end}."
         )
 
     # Create a list of arrays of date ranges for each year
     start = datetime.datetime(1, start_month, start_day)
     end = datetime.datetime(1, end_month, end_day)
     date_ranges = [
         pd.date_range(start.replace(year=year), end.replace(year=year)).date
@@ -161,31 +159,31 @@
 
 def annualized_date_range(
     start_date: datetime.datetime,
     start_year: int,
     end_date: datetime.datetime,
     end_year: int,
 ) -> np.ndarray:
-    """Creates an annualized list of dates based on the simulation years.
+    """Create an annualized list of dates based on the simulation years.
 
     Parameters
     ----------
     start_date : str
         The string start month and day in MM/DD or MM-DD format.
     start_year : int
-        _description_
+        The starting year in YYYY format.
     end_date : str
         The string end month and day in MM/DD or MM-DD format.
     end_year : int
-        _description_
+        The ending year in YYYY format.
 
     Returns
     -------
     set[datetime.datetime]
-        _description_
+        The set of dates the servicing equipment is available for operations.
     """
     additional = 1 if end_date < start_date else 0
     date_list = [
         pd.date_range(
             start_date.replace(year=year),
             end_date.replace(year=year + additional),
             freq="D",
@@ -196,68 +194,69 @@
     start = datetime.date(start_year, 1, 1)
     end = datetime.date(end_year, 12, 31)
     dates = dates[(dates >= start) & (dates <= end)]
     return dates
 
 
 def convert_ratio_to_absolute(ratio: int | float, total: int | float) -> int | float:
-    """Converts a proportional cost to an absolute cost.
+    """Convert a proportional cost to an absolute cost.
 
     Parameters
     ----------
     ratio : int | float
         The proportional materials cost for a ``Maintenance`` or ``Failure``.
     total: int | float
         The turbine's replacement cost.
 
     Returns
     -------
     int | float
         The absolute cost of the materials.
     """
-
     if ratio <= 1:
         return ratio * total
     return ratio
 
 
 def check_start_stop_dates(
     instance: Any, attribute: attr.Attribute, value: datetime.datetime | None
 ) -> None:
-    """Ensures the date range start and stop points are not the same."""
+    """Ensure the date range start and stop points are not the same."""
     if attribute.name == "non_operational_end":
         start_date = instance.non_operational_start
         start_name = "non_operational_start"
     else:
         start_date = instance.reduced_speed_start
         start_name = "reduced_speed_start"
 
     if value is None:
         if start_date is None:
             return
         raise ValueError(
-            f"A starting date was provided, but no ending date was provided for `{attribute.name}`."
+            "A starting date was provided, but no ending date was provided"
+            f" for `{attribute.name}`."
         )
 
     if start_date is None:
         raise ValueError(
-            f"An ending date was provided, but no starting date was provided for `{start_name}`."
+            "An ending date was provided, but no starting date was provided"
+            f" for `{start_name}`."
         )
 
     if start_date == value:
         raise ValueError(
             f"Starting date (`{start_name}`={start_date} and ending date"
             f" (`{attribute.name}`={value}) cannot be the same date."
         )
 
 
 def valid_hour(
     instance: Any, attribute: Attribute, value: int  # pylint: disable=W0613
 ) -> None:
-    """Validator that ensures that the input is a valid time or null value (-1).
+    """Validate that the input is a valid time or null value (-1).
 
     Parameters
     ----------
     instance : Any
         A class object.
     attribute : Attribute
         The attribute being validated.
@@ -274,33 +273,34 @@
     elif value < 0 or value > 24:
         raise ValueError(f"Input {attribute.name} must be between 0 and 24, inclusive.")
 
 
 def valid_reduction(
     instance, attribute: Attribute, value: int | float  # pylint: disable=W0613
 ) -> None:
-    """Checks to see if the reduction factor is between 0 and 1, inclusive.
+    """Check to see if the reduction factor is between 0 and 1, inclusive.
 
     Parameters
     ----------
     value : int | float
         The input value for `speed_reduction_factor`.
     """
     if value < 0 or value > 1:
         raise ValueError(
-            f"Input for {attribute.name}'s `speed_reduction_factor` must be between 0 and 1, inclusive."
+            f"Input for {attribute.name}'s `speed_reduction_factor` must be between"
+            " 0 and 1, inclusive."
         )
 
 
 def greater_than_zero(
     instance,  # pylint: disable=W0613
     attribute: Attribute,  # pylint: disable=W0613
     value: int | float,
 ) -> None:
-    """Checks if an input is greater than 0.
+    """Check if an input is greater than 0.
 
     Parameters
     ----------
     instance : Any
         The class containing the attribute to be checked.
     attribute : Attribute
         The attribute's properties.
@@ -317,15 +317,15 @@
 
 
 def greater_than_equal_to_zero(
     instance,  # pylint: disable=W0613
     attribute: Attribute,  # pylint: disable=W0613
     value: int | float,
 ) -> None:
-    """Checks if an input is at least 0.
+    """Check if an input is at least 0.
 
     Parameters
     ----------
     instance : Any
         The class containing the attribute to be checked.
     attribute : Attribute
         The attribute's properties.
@@ -351,44 +351,48 @@
     ------
     AttributeError
         Raised if the required class inputs are not provided.
     """
 
     @classmethod
     def from_dict(cls, data: dict):
-        """Maps a data dictionary to an `attrs`-defined class.
+        """Map a data dictionary to an `attrs`-defined class.
 
-        TODO: Add an error to ensure that either none or all the parameters are passed in
+        TODO: Add an error to ensure that either none or all the parameters are passed
 
         Parameters
         ----------
             data : dict
                 The data dictionary to be mapped.
+
         Returns
         -------
             cls : Any
                 The `attrs`-defined class.
         """
-        # Get all parameters from the input dictionary that map to the class initialization
+        # Get all parameters from the input dictionary that map to the class init
         kwargs = {  # type: ignore
             a.name: data[a.name]  # type: ignore
             for a in cls.__attrs_attrs__  # type: ignore
             if a.name in data and a.init  # type: ignore
         }
 
-        # Map the inputs must be provided: 1) must be initialized, 2) no default value defined
+        # Map the inputs that must be provided:
+        # 1) must be initialized
+        # 2) no default value defined
         required_inputs = [  # type: ignore
             a.name  # type: ignore
             for a in cls.__attrs_attrs__  # type: ignore
             if a.init and isinstance(a.default, attr._make._Nothing)  # type: ignore
         ]
         undefined = sorted(set(required_inputs) - set(kwargs))
         if undefined:
             raise AttributeError(
-                f"The class defintion for {cls.__name__} is missing the following inputs: {undefined}"
+                f"The class defintion for {cls.__name__} is missing the following"
+                f" inputs: {undefined}"
             )
         return cls(**kwargs)  # type: ignore
 
 
 @define(frozen=True, auto_attribs=True)
 class Maintenance(FromDictMixin):
     """Data class to store maintenance data used in subassembly and cable modeling.
@@ -397,31 +401,36 @@
     ----------
     time : float
         Amount of time required to perform maintenance, in hours.
     materials : float
         Cost of materials required to perform maintenance, in USD.
     frequency : float
         Optimal number of days between performing maintenance, in days.
-    service_equipment: Union[List[str], str]
-        Any combination of the ``Equipment.capability`` options.
-         - RMT: remote (no actual equipment BUT no special implementation)
-         - DRN: drone
-         - CTV: crew transfer vessel/vehicle
-         - SCN: small crane (i.e., field support vessel)
-         - LCN: large crane (i.e., heavy lift vessel)
-         - CAB: cabling vessel/vehicle
-         - DSV: diving support vessel
-         - TOW: tugboat or towing equipment
-         - AHV: anchor handling vessel (tugboat that doesn't trigger tow-to-port)
+    service_equipment: list[str] | str
+        Any combination of th following ``Equipment.capability`` options.
+
+        - RMT: remote (no actual equipment BUT no special implementation)
+        - DRN: drone
+        - CTV: crew transfer vessel/vehicle
+        - SCN: small crane (i.e., field support vessel)
+        - LCN: large crane (i.e., heavy lift vessel)
+        - CAB: cabling vessel/vehicle
+        - DSV: diving support vessel
+        - TOW: tugboat or towing equipment
+        - AHV: anchor handling vessel (tugboat that doesn't trigger tow-to-port)
     system_value : Union[int, float]
         Turbine replacement value. Used if the materials cost is a proportional cost.
     description : str
         A short text description to be used for logging.
     operation_reduction : float
         Performance reduction caused by the failure, between (0, 1]. Defaults to 0.
+
+        .. warning:: As of v0.7, availability is very sensitive to the usage of this
+            parameter, and so it should be used carefully.
+
     level : int, optional
         Severity level of the maintenance. Defaults to 0.
     """
 
     time: float = field(converter=float)
     materials: float = field(converter=float)
     frequency: float = field(converter=float)
@@ -452,15 +461,15 @@
         object.__setattr__(
             self,
             "materials",
             convert_ratio_to_absolute(self.materials, self.system_value),
         )
 
     def assign_id(self, request_id: str) -> None:
-        """Assigns a unique identifier to the request.
+        """Assign a unique identifier to the request.
 
         Parameters
         ----------
         request_id : str
             The ``wombat.core.RepairManager`` generated identifier.
         """
         object.__setattr__(self, "request_id", request_id)
@@ -478,28 +487,33 @@
         Weibull shape parameter for a failure classification.
     time : float
         Amount of time required to complete the repair, in hours.
     materials : float
         Cost of the materials required to complete the repair, in $USD.
     operation_reduction : float
         Performance reduction caused by the failure, between (0, 1].
+
+        .. warning:: As of v0.7, availability is very sensitive to the usage of this
+            parameter, and so it should be used carefully.
+
     level : int, optional
         Level of severity, will be generated in the ``ComponentData.create_severities``
         method.
-    service_equipment: Union[List[str], str]
-        Any combination of the ``Equipment.capability`` options.
-         - RMT: remote (no actual equipment BUT no special implementation)
-         - DRN: drone
-         - CTV: crew transfer vessel/vehicle
-         - SCN: small crane (i.e., field support vessel)
-         - LCN: large crane (i.e., heavy lift vessel)
-         - CAB: cabling vessel/vehicle
-         - DSV: diving support vessel
-         - TOW: tugboat or towing equipment
-         - AHV: anchor handling vessel (tugboat that doesn't trigger tow-to-port)
+    service_equipment: list[str] | str
+        Any combination of the following ``Equipment.capability`` options:
+
+        - RMT: remote (no actual equipment BUT no special implementation)
+        - DRN: drone
+        - CTV: crew transfer vessel/vehicle
+        - SCN: small crane (i.e., field support vessel)
+        - LCN: large crane (i.e., heavy lift vessel)
+        - CAB: cabling vessel/vehicle
+        - DSV: diving support vessel
+        - TOW: tugboat or towing equipment
+        - AHV: anchor handling vessel (tugboat that doesn't trigger tow-to-port)
     system_value : Union[int, float]
         Turbine replacement value. Used if the materials cost is a proportional cost.
     replacement : bool
         True if triggering the failure requires a subassembly replacement, False, if
         only a repair is necessary. Defaults to False
     description : str
         A short text description to be used for logging.
@@ -521,15 +535,15 @@
     system_value: int | float = field(converter=float)
     replacement: bool = field(default=False, converter=bool)
     description: str = field(default="failure", converter=str)
     weibull: weibull_min = field(init=False, eq=False)
     request_id: str = field(init=False)
 
     def __attrs_post_init__(self):
-        """Creates the actual Weibull distribution and converts equipment requirements
+        """Create the actual Weibull distribution and converts equipment requirements
         to a list.
         """
         object.__setattr__(self, "weibull", weibull_min(self.shape, scale=self.scale))
         object.__setattr__(
             self,
             "service_equipment",
             convert_to_list(self.service_equipment, str.upper),
@@ -537,31 +551,31 @@
         object.__setattr__(
             self,
             "materials",
             convert_ratio_to_absolute(self.materials, self.system_value),
         )
 
     def hours_to_next_failure(self) -> float | None:
-        """Samples the next time to failure in a Weibull distribution. If the ``scale``
-        and ``shape`` parameters are set to 0, then the model will return ``None`` to cause
-        the subassembly to timeout to the end of the simulation.
+        """Sample the next time to failure in a Weibull distribution. If the ``scale``
+        and ``shape`` parameters are set to 0, then the model will return ``None`` to
+        cause the subassembly to timeout to the end of the simulation.
 
         Returns
         -------
         float | None
             Returns ``None`` for a non-modelled failure, or the time until the next
             simulated failure.
         """
         if self.scale == self.shape == 0:
             return None
 
         return self.weibull.rvs(size=1)[0] * HOURS_IN_YEAR
 
     def assign_id(self, request_id: str) -> None:
-        """Assigns a unique identifier to the request.
+        """Assign a unique identifier to the request.
 
         Parameters
         ----------
         request_id : str
             The ``wombat.core.RepairManager`` generated identifier.
         """
         object.__setattr__(self, "request_id", request_id)
@@ -589,15 +603,17 @@
 
     name: str = field(converter=str)
     maintenance: list[Maintenance | dict[str, float | str]]
     failures: dict[int, Failure | dict[str, float | str]]
     system_value: int | float = field(converter=float)
 
     def __attrs_post_init__(self):
-        """Converts the maintenance and failure data to ``Maintenance`` and ``Failure`` objects, respectively."""
+        """Convert the maintenance and failure data to ``Maintenance`` and ``Failure``
+        objects, respectively.
+        """
         for kwargs in self.maintenance:
             assert isinstance(kwargs, dict)
             kwargs.update({"system_value": self.system_value})
         object.__setattr__(
             self,
             "maintenance",
             [
@@ -636,17 +652,19 @@
     severity_level : int
         ``Maintenance.level`` or ``Failure.level``.
     details : Failure | Maintenance
         The actual data class.
     cable : bool
         Indicator that the request is for a cable, by default False.
     upstream_turbines : list[str]
-        The cable's upstream turbines, by default []. No need to use this if ``cable`` == False.
+        The cable's upstream turbines, by default []. No need to use this if
+        ``cable`` == False.
     upstream_cables : list[str]
-        The cable's upstream cables, by default []. No need to use this if ``cable`` == False.
+        The cable's upstream cables, by default []. No need to use this if
+        ``cable`` == False.
     """
 
     system_id: str = field(converter=str)
     system_name: str = field(converter=str)
     subassembly_id: str = field(converter=str)
     subassembly_name: str = field(converter=str)
     severity_level: int = field(converter=int)
@@ -655,28 +673,29 @@
     )
     cable: bool = field(default=False, converter=bool, kw_only=True)
     upstream_turbines: list[str] = field(default=Factory(list), kw_only=True)
     upstream_cables: list[str] = field(default=Factory(list), kw_only=True)
     request_id: str = field(init=False)
 
     def assign_id(self, request_id: str) -> None:
-        """Assigns a unique identifier to the request.
+        """Assign a unique identifier to the request.
 
         Parameters
         ----------
         request_id : str
             The ``wombat.core.RepairManager`` generated identifier.
         """
         object.__setattr__(self, "request_id", request_id)
         self.details.assign_id(request_id)
 
 
 @define(frozen=True, auto_attribs=True)
 class ServiceCrew(FromDictMixin):
-    """An internal data class for the indivdual crew units that are on the servicing equipment.
+    """An internal data class for the indivdual crew units that are on the servicing
+    equipment.
 
     Parameters
     ----------
     n_day_rate: int
         Number of salaried workers.
     day_rate: float
         Day rate for salaried workers, in USD.
@@ -701,28 +720,28 @@
     port_distance: float = field(converter=float)
     non_operational_start: datetime.datetime = field(converter=parse_date)
     non_operational_end: datetime.datetime = field(converter=parse_date)
     reduced_speed_start: datetime.datetime = field(converter=parse_date)
     reduced_speed_end: datetime.datetime = field(converter=parse_date)
 
     def _set_environment_shift(self, start: int, end: int) -> None:
-        """Used to set the ``workday_start`` and ``workday_end`` to the environment's values.
+        """Set the ``workday_start`` and ``workday_end`` to the environment's values.
 
         Parameters
         ----------
         start : int
             Starting hour of a workshift.
         end : int
             Ending hour of a workshift.
         """
         object.__setattr__(self, "workday_start", start)
         object.__setattr__(self, "workday_end", end)
 
     def _set_port_distance(self, distance: int | float | None) -> None:
-        """Used to set ``port_distance`` from the environment's or port's variables.
+        """Set ``port_distance`` from the environment's or port's variables.
 
         Parameters
         ----------
         distance : int | float
             The distance to port that must be traveled for servicing equipment.
         """
         if distance is None:
@@ -734,15 +753,15 @@
 
     def _compare_dates(
         self,
         new_start: datetime.datetime | None,
         new_end: datetime.datetime | None,
         which: str,
     ) -> tuple[datetime.datetime | None, datetime.datetime | None]:
-        """Compares the orignal and newly input starting ane ending date for either the
+        """Compare the orignal and newly input starting ane ending date for either the
         non-operational date range or the reduced speed date range.
 
         Parameters
         ----------
         new_start : datetime.datetime | None
             The overriding start date if it is an earlier date than the original.
         new_end : datetime.datetime | None
@@ -789,30 +808,31 @@
     def set_non_operational_dates(
         self,
         start_date: datetime.datetime | None = None,
         start_year: int | None = None,
         end_date: datetime.datetime | None = None,
         end_year: int | None = None,
     ) -> None:
-        """Creates an annualized list of dates where servicing equipment should be
+        """Create an annualized list of dates where servicing equipment should be
         unavailable. Takes a a ``start_year`` and ``end_year`` to determine how many
         years should be covered.
 
         Parameters
         ----------
         start_date : datetime.datetime | None
             The starting date for the annual date range of non-operational dates, by
             default None.
         start_year : int | None
             The first year that has a non-operational date range, by default None.
         end_date : datetime.datetime | None
             The ending date for the annual range of non-operational dates, by default
             None.
         end_year : int | None
-            The last year that should have a non-operational date range, by default None.
+            The last year that should have a non-operational date range, by default
+            None.
 
         Raises
         ------
         ValueError
             Raised if the starting and ending dates are the same date.
         """
         start_date, end_date = self._compare_dates(
@@ -834,39 +854,40 @@
             raise ValueError(
                 f"Input to `start_year`: {start_year}, must be an integer."
             )
         if not isinstance(end_year, int):
             raise ValueError(f"Input to `end_year`: {end_year}, must be an integer.")
         if end_year < start_year:
             raise ValueError(
-                f"`start_year`: {start_year}, must less than or equal to the `end_year`: {end_year}"
+                "`start_year`: {start_year}, must less than or equal to the"
+                f" `end_year`: {end_year}"
             )
 
         # Create the date range
         dates = annualized_date_range(
             self.non_operational_start, start_year, self.non_operational_end, end_year
         )
         object.__setattr__(self, "non_operational_dates", dates)
         object.__setattr__(self, "non_operational_dates_set", set(dates))
 
         # Update the operating dates field to ensure there is no overlap
-        if hasattr(self, "operating_dates"):
-            operating = np.setdiff1d(self.operating_dates, self.non_operational_dates)  # type: ignore
+        if hasattr(self, "operating_dates") and hasattr(self, "non_operational_dates"):
+            operating = np.setdiff1d(self.operating_dates, self.non_operational_dates)
             object.__setattr__(self, "operating_dates", operating)
             object.__setattr__(self, "operating_dates_set", set(operating))
 
     def set_reduced_speed_parameters(
         self,
         start_date: datetime.datetime | None = None,
         start_year: int | None = None,
         end_date: datetime.datetime | None = None,
         end_year: int | None = None,
         speed: float = 0.0,
     ) -> None:
-        """Creates an annualized list of dates where servicing equipment should be
+        """Create an annualized list of dates where servicing equipment should be
         operating with reduced speeds. The passed ``start_date``, ``end_date``, and
         ``speed`` will override provided values if they are more conservative than the
         current settings, or a value for ``speed`` will only override the existing value
         if the passed value is slower. Takes a ``start_year`` and ``end_year`` to
         determine how many years should be covered by this setting.
 
         Parameters
@@ -906,33 +927,35 @@
             raise ValueError(
                 f"Input to `start_year`: {start_year}, must be an integer."
             )
         if not isinstance(end_year, int):
             raise ValueError(f"Input to `end_year`: {end_year}, must be an integer.")
         if end_year < start_year:
             raise ValueError(
-                f"`start_year`: {start_year}, must less than or equal to the `end_year`: {end_year}"
+                "`start_year`: {start_year}, must less than or equal to the"
+                f" `end_year`: {end_year}"
             )
 
         # Create the date range
         dates = annualized_date_range(
             self.reduced_speed_start, start_year, self.reduced_speed_end, end_year
         )
         object.__setattr__(self, "reduced_speed_dates", dates)
         object.__setattr__(self, "reduced_speed_dates_set", set(dates))
 
         # Update the reduced speed if none was originally provided
-        if speed != 0 and (self.reduced_speed == 0 or speed < self.reduced_speed):  # type: ignore
+        assert hasattr(self, "reduced_speed")  # mypy helper
+        if speed != 0 and (self.reduced_speed == 0 or speed < self.reduced_speed):
             object.__setattr__(self, "reduced_speed", speed)
 
 
 @define(frozen=True, auto_attribs=True)
 class ScheduledServiceEquipmentData(FromDictMixin, DateLimitsMixin):
-    """The data class specification for servicing equipment that will use a pre-scheduled
-    basis for returning to site.
+    """The data class specification for servicing equipment that will use a
+    pre-scheduled basis for returning to site.
 
     Parameters
     ----------
     name: str
         Name of the piece of servicing equipment.
     equipment_rate: float
         Day rate for the equipment/vessel, in USD.
@@ -992,16 +1015,16 @@
         Maximum waveheight for safe operations, m, default 1000 (land-based).
     workday_start : int
         The starting hour of a workshift, in 24 hour time.
     workday_end : int
         The ending hour of a workshift, in 24 hour time.
     crew_transfer_time : float
         The number of hours it takes to transfer the crew from the equipment to the
-        system, e.g. how long does it take to transfer the crew from the CTV to the turbine,
-        default 0.
+        system, e.g. how long does it take to transfer the crew from the CTV to the
+        turbine, default 0.
     onsite : bool
         Indicator for if the rig and crew are based onsite.
 
         .. note:: if the rig and crew are onsite be sure that the start and end dates
             represent the first and last day/month of the year, respectively, and the
             start and end years represent the fist and last year in the weather file.
 
@@ -1063,21 +1086,21 @@
     onsite: bool = field(default=False, converter=bool)
     method: str = field(  # type: ignore
         default="severity",
         converter=[str, str.lower],  # type: ignore
         validator=attrs.validators.in_(["turbine", "severity"]),
     )
     start_month: int = field(
-        default=-1, converter=int, validator=attrs.validators.ge(0)  # type: ignore
+        default=-1, converter=int, validator=attrs.validators.ge(0)
     )
-    start_day: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))  # type: ignore
-    start_year: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))  # type: ignore
-    end_month: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))  # type: ignore
-    end_day: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))  # type: ignore
-    end_year: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))  # type: ignore
+    start_day: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))
+    start_year: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))
+    end_month: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))
+    end_day: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))
+    end_year: int = field(default=-1, converter=int, validator=attrs.validators.ge(0))
     strategy: str = field(
         default="scheduled", validator=attrs.validators.in_(["scheduled"])
     )
     operating_dates: np.ndarray = field(factory=list, init=False)
     operating_dates_set: set = field(factory=set, init=False)
 
     non_operational_start: datetime.datetime = field(default=None, converter=parse_date)
@@ -1090,15 +1113,15 @@
     )
     reduced_speed: float = field(default=0, converter=float)
     non_operational_dates: pd.DatetimeIndex = field(factory=list, init=False)
     non_operational_dates_set: pd.DatetimeIndex = field(factory=set, init=False)
     reduced_speed_dates: pd.DatetimeIndex = field(factory=set, init=False)
 
     def create_date_range(self) -> np.ndarray:
-        """Creates an ``np.ndarray`` of valid operational dates for the service equipment."""
+        """Create an ``np.ndarray`` of valid operational dates."""
         start_date = datetime.datetime(
             self.start_year, self.start_month, self.start_day
         )
 
         # If `onsite` is True, then create the range in one go because there should be
         # no discrepancies in the range.
         # Othewise, create a specified date range between two dates in the year range.
@@ -1113,14 +1136,15 @@
                 self.end_month,
                 self.start_year,
                 self.end_year,
             )
         return date_range
 
     def __attrs_post_init__(self) -> None:
+        """Post-initialization."""
         object.__setattr__(self, "operating_dates", self.create_date_range())
         object.__setattr__(self, "operating_dates_set", set(self.operating_dates))
 
 
 @define(frozen=True, auto_attribs=True)
 class UnscheduledServiceEquipmentData(FromDictMixin, DateLimitsMixin):
     """The data class specification for servicing equipment that will use either a
@@ -1218,31 +1242,31 @@
 
     port_distance : int | float
         The distance, in km, the equipment must travel to go between port and site, by
         default 0.
     non_operational_start : str | datetime.datetime | None
         The starting month and day, e.g., MM/DD, M/D, MM-DD, etc. for an annualized
         period of prohibited operations. When defined at the environment level or the
-        port level, if a tugboat, an undefined or later starting date will be overridden,
-        by default None.
+        port level, if a tugboat, an undefined or later starting date will be
+        overridden, by default None.
     non_operational_end : str | datetime.datetime | None
         The ending month and day, e.g., MM/DD, M/D, MM-DD, etc. for an annualized
         period of prohibited operations. When defined at the environment level or the
-        port level, if a tugboat, an undefined or earlier ending date will be overridden,
-        by default None.
+        port level, if a tugboat, an undefined or earlier ending date will be
+        overridden, by default None.
     reduced_speed_start : str | datetime.datetime | None
         The starting month and day, e.g., MM/DD, M/D, MM-DD, etc. for an annualized
         period of reduced speed operations. When defined at the environment level or the
-        port level, if a tugboat, an undefined or later starting date will be overridden,
-        by default None.
+        port level, if a tugboat, an undefined or later starting date will be
+        overridden, by default None.
     reduced_speed_end : str | datetime.datetime | None
         The ending month and day, e.g., MM/DD, M/D, MM-DD, etc. for an annualized
         period of reduced speed operations. When defined at the environment level or the
-        port level, if a tugboat, an undefined or earlier ending date will be overridden,
-        by default None.
+        port level, if a tugboat, an undefined or earlier ending date will be
+        overridden, by default None.
     reduced_speed : float
         The maximum operating speed during the annualized reduced speed operations.
         When defined at the environment level, an undefined or faster value will be
         overridden, by default 0.0.
     """
 
     name: str = field(converter=str)
@@ -1299,15 +1323,15 @@
 
     @strategy_threshold.validator  # type: ignore
     def _validate_threshold(
         self,
         attribute: Attribute,  # pylint: disable=W0613
         value: int | float,
     ) -> None:
-        """Ensures a valid threshold is provided for a given ``strategy``."""
+        """Ensure a valid threshold is provided for a given ``strategy``."""
         if self.strategy == "downtime":
             if value <= 0 or value >= 1:
                 raise ValueError(
                     "Downtime-based strategies must have a ``strategy_threshold``",
                     "between 0 and 1, non-inclusive!",
                 )
         if self.strategy == "requests":
@@ -1335,20 +1359,21 @@
     strategy : str, optional
         Should be one of "scheduled", "requests", "downtime". If nothing is provided,
         the equipment configuration will be checked.
 
     Raises
     ------
     ValueError
-        If ``strategy`` is not one of "scheduled" or "unscheduled" an error will be raised.
+        Raised if ``strategy`` is not one of "scheduled" or "unscheduled".
 
     Examples
     --------
-    The below workflow is how a new data :py:class:`~data_classes.ScheduledServiceEquipmentData`
-    object could be created via a generic/routinized creation method, and is how the
+    The below workflow is how a new data
+    :py:class:`~data_classes.ScheduledServiceEquipmentData` object could be created via
+    a generic/routinized creation method, and is how the
     :py:class:`~service_equipment.ServiceEquipment`'s ``__init__`` method creates the
     settings data.
 
     >>> from wombat.core.data_classes import  ServiceEquipmentData
     >>>
     >>> data_dict = {
     >>>     "name": "Crew Transfer Vessel 1",
@@ -1385,33 +1410,35 @@
 
     data_dict: dict
     strategy: str | None = field(
         kw_only=True, default=None, converter=clean_string_input
     )
 
     def __attrs_post_init__(self):
+        """Post-initialization."""
         if self.strategy is None:
             object.__setattr__(
                 self, "strategy", clean_string_input(self.data_dict["strategy"])
             )
         if self.strategy not in VALID_STRATEGIES:
             raise ValueError(
-                f"ServiceEquipment strategy should be one of {VALID_STRATEGIES}; input: {self.strategy}."
+                f"ServiceEquipment strategy should be one of {VALID_STRATEGIES};"
+                f" input: {self.strategy}."
             )
 
     def determine_type(
         self,
     ) -> ScheduledServiceEquipmentData | UnscheduledServiceEquipmentData:
-        """Generates the appropriate ServiceEquipmentData variation.
+        """Generate the appropriate ServiceEquipmentData variation.
 
         Returns
         -------
         Union[ScheduledServiceEquipmentData, UnscheduledServiceEquipmentData]
-            The appropriate ``xxServiceEquipmentData`` schema depending on the strategy the
-            ``ServiceEquipment`` will use.
+            The appropriate ``xxServiceEquipmentData`` schema depending on the strategy
+            the ``ServiceEquipment`` will use.
         """
         if self.strategy == "scheduled":
             return ScheduledServiceEquipmentData.from_dict(self.data_dict)
         elif self.strategy in UNSCHEDULED_STRATEGIES:
             return UnscheduledServiceEquipmentData.from_dict(self.data_dict)
         else:
             # This should not be able to be reached
@@ -1443,15 +1470,15 @@
 
     def update(
         self,
         capability: str,
         threshold: int | float,
         equipment: "ServiceEquipment",  # noqa: disable=F821
     ) -> None:
-        """A method to update the strategy mapping between capability types and the
+        """Update the strategy mapping between capability types and the
         available ``ServiceEquipment`` objects.
 
         Parameters
         ----------
         capability : str
             The ``equipment``'s capability.
         threshold : int | float
@@ -1487,14 +1514,87 @@
         else:
             # This should not even be able to be reached
             raise ValueError(
                 f"Invalid servicing equipment '{capability}' has been provided!"
             )
         self.is_running = True
 
+    def get_mapping(self, capability) -> list[EquipmentMap]:
+        """Gets the attribute matching the desired :py:attr:`capability`.
+
+        Parameters
+        ----------
+        capability : str
+            A string matching one of the ``UnscheduledServiceEquipmentData.capability``
+            (or scheduled) options.
+
+        Returns
+        -------
+        list[EquipmentMap]
+            Returns the matching mapping of available servicing equipment.
+        """
+        if capability == "CTV":
+            return self.CTV
+        if capability == "SCN":
+            return self.SCN
+        if capability == "LCN":
+            return self.LCN
+        if capability == "CAB":
+            return self.CAB
+        if capability == "RMT":
+            return self.RMT
+        if capability == "DRN":
+            return self.DRN
+        if capability == "DSV":
+            return self.DSV
+        if capability == "TOW":
+            return self.TOW
+        if capability == "AHV":
+            return self.AHV
+        # This should not even be able to be reached
+        raise ValueError(
+            f"Invalid servicing equipmen capability '{capability}' has been provided!"
+        )
+
+    def move_equipment_to_end(self, capability: str, ix: int) -> None:
+        """Moves a used equipment to the end of the mapping list to ensure a broader
+        variety of servicing equipment are used throughout a simulation.
+
+        Parameters
+        ----------
+        capability : str
+            A string matching one of ``capability`` options for servicing equipment
+            dataclasses.
+        ix : int
+            The index of the used servicing equipent.
+        """
+        if capability == "CTV":
+            self.CTV.append(self.CTV.pop(ix))
+        elif capability == "SCN":
+            self.SCN.append(self.SCN.pop(ix))
+        elif capability == "LCN":
+            self.LCN.append(self.LCN.pop(ix))
+        elif capability == "CAB":
+            self.CAB.append(self.CAB.pop(ix))
+        elif capability == "RMT":
+            self.RMT.append(self.RMT.pop(ix))
+        elif capability == "DRN":
+            self.DRN.append(self.DRN.pop(ix))
+        elif capability == "DSV":
+            self.DSV.append(self.DSV.pop(ix))
+        elif capability == "TOW":
+            self.TOW.append(self.TOW.pop(ix))
+        elif capability == "AHV":
+            self.AHV.append(self.AHV.pop(ix))
+        else:
+            # This should not even be able to be reached
+            raise ValueError(
+                f"Invalid servicing equipmen capability {capability} has been provided!"
+            )
+
 
 @define(frozen=True, auto_attribs=True)
 class PortConfig(FromDictMixin, DateLimitsMixin):
     """Port configurations for offshore wind power plant scenarios.
 
     Parameters
     ----------
@@ -1574,30 +1674,30 @@
     reduced_speed_dates: pd.DatetimeIndex = field(factory=set, init=False)
     non_operational_dates_set: pd.DatetimeIndex = field(factory=set, init=False)
     reduced_speed_dates_set: pd.DatetimeIndex = field(factory=set, init=False)
 
 
 @define(frozen=True, auto_attribs=True)
 class FixedCosts(FromDictMixin):
-    """The fixed costs for operating a windfarm. All values are assumed to be in $/kW/yr.
+    """Fixed costs for operating a windfarm. All values are assumed to be in $/kW/yr.
 
     Parameters
     ----------
     operations : float
         Non-maintenance costs of operating the project. If a value is provided for this
         attribute, then it will zero out all other values, otherwise it will be set to
         the sum of the remaining values.
     operations_management_administration: float
         Activities necessary to forecast, dispatch, sell, and manage the production of
         power from the plant. Includes both the onsite and offsite personnel, software,
         and equipment to coordinate high voltage equipment, switching, port activities,
         and marine activities.
 
-        .. note:: This should only be used when not breaking down the cost into the following
-            categories: ``project_management_administration``,
+        .. note:: This should only be used when not breaking down the cost into the
+            following categories: ``project_management_administration``,
             ``operation_management_administration``, ``marine_management``, and/or
             ``weather_forecasting``
 
     project_management_administration : float
         Financial reporting, public relations, procurement, parts and stock management,
         H&SE management, training, subcontracts, and general administration.
     marine_management : float
@@ -1613,19 +1713,21 @@
         Co-located offices, parts store, quayside facilities, helipad, refueling
         facilities, hanger (if necesssary), etc.
     environmental_health_safety_monitoring : float
         Coordination and monitoring to ensure compliance with HSE requirements during
         operations.
     insurance : float
         Insurance policies during operational period including All Risk Property,
-        Buisness Interuption, Third Party Liability, and Brokers Fee, and Storm Coverage.
+        Buisness Interuption, Third Party Liability, and Brokers Fee, and Storm
+        Coverage.
 
         .. note:: This should only be used when not breaking down the cost into the
             following categories: ``brokers_fee``, ``operations_all_risk``,
-            ``business_interruption``, ``third_party_liability``, and/or ``storm_coverage``
+            ``business_interruption``, ``third_party_liability``, and/or
+            ``storm_coverage``
 
     brokers_fee : float
         Fees for arranging the insurance package.
     operations_all_risk : float
         All Risk Property (physical damage). Sudden and unforseen physical loss or
         physical damage to teh plant/assets during the operational phase of a project.
     business_interruption : float
@@ -1712,14 +1814,15 @@
         if getattr(self, name) <= 0:
             object.__setattr__(self, name, fsum(getattr(self, el) for el in sub_names))
         else:
             for cost in sub_names:
                 object.__setattr__(self, cost, 0)
 
     def __attrs_post_init__(self):
+        """Post-initialization."""
         grouped_names = {
             "operations_management_administration": [
                 "project_management_administration",
                 "marine_management",
                 "weather_forecasting",
                 "condition_monitoring",
             ],
@@ -1813,16 +1916,15 @@
                 }
             },
         )
 
 
 @define(auto_attribs=True)
 class SubString:
-    """
-    A list of the upstream connections for a turbine and its downstream connector.
+    """A list of the upstream connections for a turbine and its downstream connector.
 
     Parameters
     ----------
     downstream : str
         The downstream turbine/substation connection id.
     upstream : list[str]
         A list of the upstream turbine connections.
@@ -1830,16 +1932,15 @@
 
     downstream: str
     upstream: list[str]
 
 
 @define(auto_attribs=True)
 class String:
-    """
-    All of the connection information for a complete string in a wind farm.
+    """All of the connection information for a complete string in a wind farm.
 
     Parameters
     ----------
     start : str
         The substation's ID (``System.id``)
     upstream_map : dict[str, SubString]
         The dictionary of each turbine ID in the string and it's upstream ``SubString``.
@@ -1847,22 +1948,22 @@
 
     start: str
     upstream_map: dict[str, SubString]
 
 
 @define(auto_attribs=True)
 class SubstationMap:
-    """
-    A mapping of every ``String`` connected to a substation, excluding export
+    """A mapping of every ``String`` connected to a substation, excluding export
     connections to other substations.
 
     Parameters
     ----------
     string_starts : list[str]
-        A list of every first turbine's ``System.id`` in a string connected to the substation.
+        A list of every first turbine's ``System.id`` in a string connected to the
+        substation.
     string_map : dict[str, String]
         A dictionary mapping each string starting turbine to its ``String`` data.
     downstream : str
         The ``System.id`` of where the export cable leads. This should be the same
         ``System.id`` as the substation for an interconnection point, or another
         connecting substation.
     """
@@ -1870,16 +1971,15 @@
     string_starts: list[str]
     string_map: dict[str, String]
     downstream: str
 
 
 @define(auto_attribs=True)
 class WindFarmMap:
-    """
-    A list of the upstream connections for a turbine and its downstream connector.
+    """A list of the upstream connections for a turbine and its downstream connector.
 
     Parameters
     ----------
     substation_map : list[str]
         A dictionary mapping of each substation and its ``SubstationMap``.
     export_cables : list[tuple[str, str]]
         A list of the export cable connections.
@@ -1887,15 +1987,16 @@
 
     substation_map: dict[str, SubstationMap]
     export_cables: list[tuple[str, str]]
 
     def get_upstream_connections(
         self, substation: str, string_start: str, node: str, return_cables: bool = True
     ) -> list[str] | tuple[list[str], list[str]]:
-        """Retrieves the upstream turbines (and optionally cables) within the wind farm graph.
+        """Retrieve the upstream turbines (and optionally cables) within the wind farm
+        graph.
 
         Parameters
         ----------
         substation : str
             The substation's ``System.id``.
         string_start : str
             The ``System.id`` of the first turbine in the string.
@@ -1927,34 +2028,36 @@
         self, substation: str, return_cables: bool = True, by_string: bool = True
     ) -> (
         list[str]
         | tuple[list[str], list[str]]
         | list[list[str]]
         | tuple[list[list[str]], list[list[str]]]
     ):
-        """Retrieves the upstream turbines (and optionally, cables) connected to a
+        """Retrieve the upstream turbines (and optionally, cables) connected to a
         py:attr:`substation` in the wind farm graph.
 
         Parameters
         ----------
         substation : str
             The py:attr:`System.id` for the substation.
         return_cables : bool, optional
             Indicates if the ``Cable.id`` should be generated for each of the turbines,
             by default True
         by_string : bool, optional
             Indicates if the list of turbines (and cables) should be a nested list for
-            each string (py:obj:`True`), or as 1-D list (py:obj:`False`), by default True.
+            each string (py:obj:`True`), or as 1-D list (py:obj:`False`), by default
+            True.
 
         Returns
         -------
         list[str] | tuple[list[str], list[str]]
             A list of ``System.id`` for all of the upstream turbines of ``node`` if
-            ``return_cables=False``, otherwise the upstream turbine and the ``Cable.id`` lists
-            are returned. These are bifurcated in lists of lists for each string if ``by_string=True``
+            ``return_cables=False``, otherwise the upstream turbine and the ``Cable.id``
+            lists are returned. These are bifurcated in lists of lists for each string
+            if ``by_string=True``
         """
         turbines, cables = [], []
         substation_map = self.substation_map[substation]
         start_nodes = substation_map.string_starts
         for start_node in start_nodes:
             # Add the starting node of the string and substation-turbine array cable
             _turbines = [start_node]
```

### Comparing `wombat-0.6.2/wombat/core/environment.py` & `wombat-0.7.0/wombat/core/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Provides the O&M Enviroment class; a subclass of simpy.Environment."""
 from __future__ import annotations
 
+import io
 import csv
 import math
 import logging
 import datetime as dt
-from typing import TYPE_CHECKING, Tuple, Union, Optional
+from typing import TYPE_CHECKING
 from pathlib import Path
 from datetime import datetime, timedelta
 
 import numpy as np
 import simpy
 import pandas as pd
 import pyarrow as pa
@@ -50,17 +51,17 @@
     "total_labor_cost",
     "equipment_cost",
     "total_cost",
 ]
 
 
 class WombatEnvironment(simpy.Environment):
-    """The primary mechanism for powering an O&M simulation. This object has insight into
-    all other simulation objects, and controls the timing, date/time stamps, and weather
-    conditions.
+    """The primary mechanism for powering an O&M simulation. This object has insight
+    into all other simulation objects, and controls the timing, date/time stamps, and
+    weather conditions.
 
     Parameters
     ----------
     data_dir : pathlib.Path | str
         Directory where the inputs are stored and where to save outputs.
     weather_file : str
         Name of the weather file. Should be contained within ``data_dir``/weather/, with
@@ -71,15 +72,15 @@
         by an ``ServiceEquipmentData`` object that operates outside of the "typical"
         working hours.
     workday_end : int
         Ending time for the repair crew, in 24 hour local time. This can be overridden
         by an ``ServiceEquipmentData`` object that operates outside of the "typical"
         working hours.
     simulation_name : str | None, optional
-        Name of the simulation; will be used for naming the log file, by default ``None``.
+        Name of the simulation; will be used for naming the log file, by default None.
         If ``None``, then the current time will be used. Will always save to
         ``data_dir``/outputs/logs/``simulation_name``.log.
 
         .. note: spaces (" ") will be replaced with underscores ("_"), for example:
             "my example analysis" becomes "my_example_analysis".
 
     start_year : int | None, optional
@@ -171,21 +172,21 @@
         self.reduced_speed = reduced_speed
 
         self.simulation_name = simulation_name
         self._logging_setup()
         self.process(self._log_actions())
 
     def _register_windfarm(self, windfarm: Windfarm) -> None:
-        """Adds the simulation windfarm to the class attributes"""
+        """Adds the simulation windfarm to the class attributes."""
         self.windfarm = windfarm
 
-    def run(self, until: Optional[Union[int, float, Event]] = None):
-        """Extends the ``simpy.Environment.run`` method to change the default behavior if
-        no argument is passed to ``until``, which will now run a simulation until the end
-        of the weather profile is reached.
+    def run(self, until: int | float | Event | None = None):
+        """Extends the ``simpy.Environment.run`` method to change the default behavior
+        if no argument is passed to ``until``, which will now run a simulation until the
+        end of the weather profile is reached.
 
         Parameters
         ----------
         until : Optional[Union[int, float, Event]], optional
             When to stop the simulation, by default None. See documentation on
             ``simpy.Environment.run`` for more details.
         """
@@ -193,16 +194,18 @@
         # the simulation time is lower than the upper bound
         time_check = self.now < self.max_run_time
         if self._events_csv.closed and time_check:  # type: ignore
             self._events_csv = open(self.events_log_fname, "a")
             self._events_writer = csv.DictWriter(
                 self._events_csv, delimiter="|", fieldnames=EVENTS_COLUMNS
             )
-        if hasattr(self, "windfarm") and self._operations_csv.closed and time_check:  # type: ignore
-            self._operations_csv = open(self.operations_log_fname, "a")
+        if hasattr(self, "windfarm") and self._operations_csv.closed and time_check:
+            self._operations_csv: io.TextIOWrapper = open(
+                self.operations_log_fname, "a"
+            )
             self.windfarm._setup_logger(initial=False)
 
         if until is None:
             until = self.max_run_time
         elif until > self.max_run_time:
             until = self.max_run_time
         try:
@@ -273,24 +276,26 @@
         else:
             _dt = self.weather_dates[math.floor(now)]
 
         minutes, seconds = math.floor(minutes), math.ceil(minutes % 1 * 60)
         return _dt + timedelta(minutes=minutes, seconds=seconds)
 
     def is_workshift(self, workday_start: int = -1, workday_end: int = -1) -> bool:
-        """Checks if the current simulation time is within the windfarm's working hours.
+        """Check if the current simulation time is within the windfarm's working hours.
 
         Parameters
         ----------
         workday_start : int
-            A valid hour in 24 hour time, by default -1. This should only be provided from an
-            ``ServiceEquipmentData`` object. ``workday_end`` must also be provided in order to be used.
+            A valid hour in 24 hour time, by default -1. This should only be provided
+            from an ``ServiceEquipmentData`` object. ``workday_end`` must also be
+            provided in order to be used.
         workday_end : int
-            A valid hour in 24 hour time, by default -1. This should only be provided from an
-            ``ServiceEquipmentData`` object. ``workday_start`` must also be provided in order to be used.
+            A valid hour in 24 hour time, by default -1. This should only be provided
+            from an ``ServiceEquipmentData`` object. ``workday_start`` must also be
+            provided in order to be used.
 
         Returns
         -------
         bool
             True if it's valid working hours, False otherwise.
         """
         if -1 in (workday_start, workday_end):
@@ -311,19 +316,21 @@
         """Checks whether an ``hour`` is within the working hours.
 
         Parameters
         ----------
         hour : int
             Hour of the day.
         workday_start : int
-            A valid hour in 24 hour time, by default -1. This should only be provided from an
-            ``ServiceEquipmentData`` object. ``workday_end`` must also be provided in order to be used.
+            A valid hour in 24 hour time, by default -1. This should only be provided
+            from an ``ServiceEquipmentData`` object. ``workday_end`` must also be
+            provided in order to be used.
         workday_end : int
-            A valid hour in 24 hour time, by default -1. This should only be provided from an
-            ``ServiceEquipmentData`` object. ``workday_start`` must also be provided in order to be used.
+            A valid hour in 24 hour time, by default -1. This should only be provided
+            from an ``ServiceEquipmentData`` object. ``workday_start`` must also be
+            provided in order to be used.
 
         Returns
         -------
         bool
             True if ``hour`` is during working hours, False otherwise.
         """
         if -1 in (workday_start, workday_end):
@@ -381,16 +388,16 @@
         if isinstance(ix, slice):
             return ix.start
         return ix[0]
 
     def _weather_setup(
         self,
         weather_file: str,
-        start_year: Optional[int] = None,
-        end_year: Optional[int] = None,
+        start_year: int | None = None,
+        end_year: int | None = None,
     ) -> pd.DataFrame:
         """Reads the weather data from the "<inputs>/weather" directory, and creates the
         ``start_date`` and ``end_date`` time stamps for the simulation.
 
         This also fills any missing data with zeros and interpolates the values of any
         missing datetime entries.
 
@@ -407,14 +414,16 @@
             greater than the last year of the weather profile, this will be ignored.
 
         Returns
         -------
         pd.DataFrame
             The wind (and  wave) timeseries.
         """
+        REQUIRED = ["windspeed", "waveheight"]
+
         # PyArrow datetime conversion setup
         convert_options = pa.csv.ConvertOptions(
             timestamp_parsers=[
                 "%m/%d/%y %H:%M",
                 "%m/%d/%y %I:%M",
                 "%m/%d/%Y %H:%M",
                 "%m/%d/%Y %I:%M",
@@ -427,15 +436,22 @@
             )
             .to_pandas()
             .set_index("datetime")
         )
         weather = weather.fillna(0.0)
         weather = weather.resample("H").interpolate(limit_direction="both", limit=5)
 
-        # Add in the hour of day column for more efficient handling within the simulation
+        missing = set(REQUIRED).difference(weather.columns)
+        if missing:
+            raise KeyError(
+                "The weather data are missing the following required columns:"
+                f" {missing}"
+            )
+
+        # Add in the hour of day column for efficient handling within the simulation
         weather = weather.assign(hour=weather.index.hour.astype(float))
 
         # Create the start and end points
         self.start_datetime = weather.index[0].to_pydatetime()
         self.end_datetime = weather.index[-1].to_pydatetime()
         self.start_year = self.start_datetime.year
         self.end_year = self.end_datetime.year
@@ -466,42 +482,47 @@
         elif start_year is not None:
             if end_year < start_year:
                 raise ValueError(
                     f"The provided 'end_year' ({end_year}) is before the start_year"
                     f" ({start_year})"
                 )
             else:
-                # Filter for the provided, validated ending year and update the attribute
+                # Filter for the provided, validated ending year and update
                 weather = weather.loc[weather.index.year <= end_year]
                 self.end_datetime = weather.index[-1].to_pydatetime()
                 self.end_year = self.end_datetime.year
         else:
             # Filter for the provided, validated ending year and update the attribute
             weather = weather.loc[weather.index.year <= end_year]
             self.end_datetime = weather.index[-1].to_pydatetime()
             self.end_year = self.end_datetime.year
 
-        return weather
+        column_order = weather.columns.tolist()
+        column_order.insert(0, column_order.pop(column_order.index("hour")))
+        column_order.insert(0, column_order.pop(column_order.index("waveheight")))
+        column_order.insert(0, column_order.pop(column_order.index("windspeed")))
+
+        return weather.loc[:, column_order]
 
     @property
-    def weather_now(self) -> Tuple[float, float, int]:
+    def weather_now(self) -> tuple[float, float, int]:
         """The current weather.
 
         Returns
         -------
         Tuple[float, float, int]
             Wind, wave, and hour data for the current time.
         """
         # Rounds down because we won't arrive at the next weather event until that hour
         now = int(self.now)
         return self.weather.iloc[now].values
 
     def weather_forecast(
-        self, hours: Union[int, float]
-    ) -> Tuple[DatetimeIndex, np.ndarray, np.ndarray, np.ndarray]:
+        self, hours: int | float
+    ) -> tuple[DatetimeIndex, np.ndarray, np.ndarray, np.ndarray]:
         """Returns the wind and wave data for the next ``hours`` hours, starting from
         the current hour's weather.
 
         Parameters
         ----------
         hours : Union[int, float]
             Number of hours to look ahead, rounds up to the nearest hour.
@@ -513,15 +534,15 @@
             hours requested, each with shape (``hours`` + 1).
         """
         start = math.floor(self.now)
 
         # If it's not on the hour, ensure we're looking ``hours`` hours into the future
         end = start + math.ceil(hours) + math.ceil(self.now % 1)
 
-        wind, wave, hour = self.weather.values[start:end].T
+        wind, wave, hour, *_ = self.weather.values[start:end].T
         ix = self.weather.index[start:end]
         return ix, hour, wind, wave
 
     def log_action(
         self,
         *,
         agent: str,
@@ -534,18 +555,18 @@
         part_name: str = "",
         system_ol: float | int = 0,
         part_ol: float | int = 0,
         duration: float = 0,
         distance_km: float = 0,
         request_id: str = "na",
         location: str = "na",
-        materials_cost: Union[int, float] = 0,
-        hourly_labor_cost: Union[int, float] = 0,
-        salary_labor_cost: Union[int, float] = 0,
-        equipment_cost: Union[int, float] = 0,
+        materials_cost: int | float = 0,
+        hourly_labor_cost: int | float = 0,
+        salary_labor_cost: int | float = 0,
+        equipment_cost: int | float = 0,
     ) -> None:
         """Formats the logging messages into the expected format for logging.
 
         Parameters
         ----------
         agent : str
             Agent performing the action.
@@ -560,20 +581,22 @@
         system_name : str
             Turbine name, ``System.name``, by default "".
         part_id : str
             Subassembly, component, or cable ID, ``_.id``, by default "".
         part_name : str
             Subassembly, component, or cable name, ``_.name``, by default "".
         system_ol : float | int
-            Turbine operating level, ``System.operating_level``. Use an empty string for n/a, by default 0.
+            Turbine operating level, ``System.operating_level``. Use an empty string
+            for n/a, by default 0.
         part_ol : float | int
             Subassembly, component, or cable operating level, ``_.operating_level``. Use
             an empty string for n/a, by default 0.
         request_id : str
-            The ``RepairManager`` assigned request_id found in ``RepairRequest.request_id``, by default "na".
+            The ``RepairManager`` assigned request_id found in
+            ``RepairRequest.request_id``, by default "na".
         location : str
             The location of where the event ocurred: should be one of site, port,
             enroute, or system, by default "na".
         duration : float
             Length of time the action lasted, by default 0.
         distance : float
             Distance traveled, in km, if applicable, by default 0.
@@ -589,43 +612,43 @@
         valid_locations = ("site", "system", "port", "enroute", "na")
         if location not in valid_locations:
             raise ValueError(
                 f"Event logging `location` must be one of: {valid_locations}"
             )
         total_labor_cost = hourly_labor_cost + salary_labor_cost
         total_cost = total_labor_cost + equipment_cost + materials_cost
-        row = dict(
-            datetime=dt.datetime.now(),
-            env_datetime=self.simulation_time,
-            env_time=self.now,
-            system_id=system_id,
-            system_name=system_name,
-            part_id=part_id,
-            part_name=part_name,
-            system_operating_level=system_ol,
-            part_operating_level=part_ol,
-            agent=agent,
-            action=action,
-            reason=reason,
-            additional=additional,
-            duration=duration,
-            distance_km=distance_km,
-            request_id=request_id,
-            location=location,
-            materials_cost=materials_cost,
-            hourly_labor_cost=hourly_labor_cost,
-            salary_labor_cost=salary_labor_cost,
-            equipment_cost=equipment_cost,
-            total_labor_cost=total_labor_cost,
-            total_cost=total_cost,
-        )
+        row = {
+            "datetime": dt.datetime.now(),
+            "env_datetime": self.simulation_time,
+            "env_time": self.now,
+            "system_id": system_id,
+            "system_name": system_name,
+            "part_id": part_id,
+            "part_name": part_name,
+            "system_operating_level": system_ol,
+            "part_operating_level": part_ol,
+            "agent": agent,
+            "action": action,
+            "reason": reason,
+            "additional": additional,
+            "duration": duration,
+            "distance_km": distance_km,
+            "request_id": request_id,
+            "location": location,
+            "materials_cost": materials_cost,
+            "hourly_labor_cost": hourly_labor_cost,
+            "salary_labor_cost": salary_labor_cost,
+            "equipment_cost": equipment_cost,
+            "total_labor_cost": total_labor_cost,
+            "total_cost": total_cost,
+        }
         self._events_buffer.append(row)
 
     def _log_actions(self):
-        """Writes the action log items every 8000 hours"""
+        """Writes the action log items every 8000 hours."""
         HOURS = 8000
         while True:
             yield self.timeout(HOURS)
             self._events_writer.writerows(self._events_buffer)
             self._events_buffer.clear()
 
     def load_events_log_dataframe(self) -> pd.DataFrame:
@@ -634,58 +657,70 @@
 
         Returns
         -------
         pd.DataFrame
             The formatted logging data from a simulation.
         """
         convert_options = pa.csv.ConvertOptions(
-            timestamp_parsers=["%y-%m-%d %H:%M:%S.%f", "%y-%m-%d %H:%M:%S"]
+            timestamp_parsers=["%Y-%m-%d %H:%M:%S.%f", "%Y-%m-%d %H:%M:%S"]
         )
         parse_options = pa.csv.ParseOptions(delimiter="|")
         log_df = pa.csv.read_csv(
             self.events_log_fname,
             convert_options=convert_options,
             parse_options=parse_options,
         ).to_pandas()
-        log_df.datetime = pd.to_datetime(log_df.datetime)
-        log_df.env_datetime = pd.to_datetime(log_df.env_datetime)
+        if not pd.api.types.is_datetime64_any_dtype(log_df.datetime):
+            log_df.datetime = pd.to_datetime(
+                log_df.datetime, yearfirst=True, format="mixed"
+            )
+        if not pd.api.types.is_datetime64_any_dtype(log_df.env_datetime):
+            log_df.env_datetime = pd.to_datetime(
+                log_df.env_datetime, yearfirst=True, format="mixed"
+            )
         log_df = log_df.set_index("datetime").sort_values("datetime")
 
         return log_df
 
     def load_operations_log_dataframe(self) -> pd.DataFrame:
         """Imports the logging file created in ``run`` and returns it as a formatted
         ``pandas.DataFrame``.
 
         Returns
         -------
         pd.DataFrame
             The formatted logging data from a simulation.
         """
         convert_options = pa.csv.ConvertOptions(
-            timestamp_parsers=["%y-%m-%d %H:%M:%S.%f", "%y-%m-%d %H:%M:%S"]
+            timestamp_parsers=["%Y-%m-%d %H:%M:%S.%f", "%Y-%m-%d %H:%M:%S"]
         )
         parse_options = pa.csv.ParseOptions(delimiter="|")
         log_df = pa.csv.read_csv(
             self.operations_log_fname,
             convert_options=convert_options,
             parse_options=parse_options,
         ).to_pandas()
-        log_df.datetime = pd.to_datetime(log_df.datetime)
-        log_df.env_datetime = pd.to_datetime(log_df.env_datetime)
+        if not pd.api.types.is_datetime64_any_dtype(log_df.datetime):
+            log_df.datetime = pd.to_datetime(
+                log_df.datetime, yearfirst=True, format="mixed"
+            )
+        if not pd.api.types.is_datetime64_any_dtype(log_df.env_datetime):
+            log_df.env_datetime = pd.to_datetime(
+                log_df.env_datetime, yearfirst=True, format="mixed"
+            )
         log_df = log_df.set_index("datetime").sort_values("datetime")
 
         return log_df
 
     def power_production_potential_to_csv(  # type: ignore
         self,
-        windfarm: "wombat.windfarm.Windfarm",  # type: ignore
-        operations: Optional[pd.DataFrame] = None,
+        windfarm: wombat.windfarm.Windfarm,  # type: ignore
+        operations: pd.DataFrame | None = None,
         return_df: bool = True,
-    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    ) -> tuple[pd.DataFrame, pd.DataFrame]:
         """Creates the power production ``DataFrame`` and optionally returns it.
 
         Parameters
         ----------
         windfarm : wombat.windfarm.Windfarm
             The simulation's windfarm object.
         operations : Optional[pd.DataFrame], optional
@@ -711,15 +746,15 @@
         potential_df = pd.DataFrame(
             [],
             index=operations.env_datetime,
             columns=["env_time", "env_datetime", "windspeed", "windfarm"]
             + turbines.tolist(),
         )
         potential_df[turbines] = np.vstack(
-            ([windfarm.system(t_id).power(windspeed) for t_id in turbines])
+            [windfarm.system(t_id).power(windspeed) for t_id in turbines]
         ).T
         potential_df = potential_df.assign(
             windspeed=windspeed,
             windfarm=potential_df[turbines].sum(axis=1),
             env_time=operations.env_time.values,
             env_datetime=operations.env_datetime.values,
         )
@@ -739,21 +774,20 @@
             self.power_production_fname,
             write_options=write_options,
         )
         if return_df:
             return potential_df, production_df
 
     def cleanup_log_files(self) -> None:
-        """This is a convenience method to clear the output log files in case a large
+        """Convenience method to clear the output log files in case a large
         batch of simulations is being run and there are space limitations.
 
         ... warning:: This shuts down the loggers, so no more logging will be able
             to be performed.
         """
-
         # NOTE: Everything is wrapped in a try/except clause to protect against failure
         # when inevitably a file has already been deleted on accident, or if in the
         # dataframe generation step, the original logs were deleted
 
         logging.shutdown()
         if not self._events_csv.closed:
             self._events_csv.close()
```

### Comparing `wombat-0.6.2/wombat/core/library.py` & `wombat-0.7.0/wombat/core/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         Name of the file (ending in .yaml) to be loaded.
 
     Returns
     -------
     Any
         Whatever content is in the YAML file.
     """
-    return yaml.load(open(os.path.join(path, fname), "r"), Loader=custom_loader)
+    return yaml.load(open(os.path.join(path, fname)), Loader=custom_loader)
 
 
 def create_library_structure(
     library_path: str | Path, create_init: bool = False
 ) -> None:
     """Creates the following library structure at ``library_path``. If ``library_path``
     does not exist, then the method will fail.
```

### Comparing `wombat-0.6.2/wombat/core/mixins.py` & `wombat-0.7.0/wombat/core/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 class RepairsMixin:
     """A Mixin class that provides some common repair and timing methods that are used
     across different repair-providing classes, such as: servicing equipment and ports.
     """
 
     env: WombatEnvironment
-    settings: PortConfig | ScheduledServiceEquipmentData | UnscheduledServiceEquipmentData
+    settings: PortConfig | ScheduledServiceEquipmentData | UnscheduledServiceEquipmentData  # noqa: disable=E501
 
     def initialize_cost_calculators(self, which: str) -> None:
         """Creates the cost calculators for each of the subclasses that will need to
         calculate hourly costs.
 
         Parameters
         ----------
@@ -104,15 +104,15 @@
         is_workshift &= hour_ix <= self.settings.workday_end
         return is_workshift
 
     def wait_until_next_shift(self, **kwargs) -> Generator[Timeout, None, None]:
         """Delays the process until the start of the next shift.
 
         Yields
-        -------
+        ------
         Generator[Timeout, None, None]
             Delay until the start of the next shift.
         """
         kwargs["additional"] = kwargs.get(
             "additional", "work shift has ended; waiting for next shift to start"
         )
         kwargs["action"] = kwargs.get("action", "delay")
@@ -132,41 +132,43 @@
             equipment_cost=equpipment_cost,
             **kwargs,
         )
         yield self.env.timeout(delay)
 
     def process_repair(
         self, hours: int | float, request_details: Maintenance | Failure, **kwargs
-    ) -> None | Generator[Timeout | Process, None, None]:
+    ) -> Generator[Timeout | Process, None, None]:
         """The logging and timeout process for performing a repair or doing maintenance.
 
         Parameters
         ----------
         hours : int | float
             The lenght, in hours, of the repair or maintenance task.
         request_details : Maintenance | Failure
             The deatils of the request, this is only being checked for the type.
+        kwargs : dict
+            Additional parameters to be passed to ``WombatEnvironment.log_action``.
 
         Yields
-        -------
-        None | Generator[Timeout | Process, None, None]
+        ------
+        Generator[Timeout | Process, None, None]
             A ``Timeout`` is yielded of length ``hours``.
         """
         action = "repair" if isinstance(request_details, Failure) else "maintenance"
         salary_cost = self.calculate_salary_cost(hours)
         hourly_cost = self.calculate_hourly_cost(hours)
         equipment_cost = self.calculate_equipment_cost(hours)
         self.env.log_action(
             action=action,
             duration=hours,
             salary_labor_cost=salary_cost,
             hourly_labor_cost=hourly_cost,
             equipment_cost=equipment_cost,
             additional=action,
-            location="port" if isinstance(self.settings, PortConfig) else "site",
+            location="port" if isinstance(self.settings, PortConfig) else "system",
             **kwargs,
         )
         yield self.env.timeout(hours)
 
     def hours_to_next_operational_date(
         self,
         start_search_date: datetime.datetime | datetime.date | pd.Timestamp,
@@ -204,15 +206,15 @@
         )  # get the dates for the next year
         dates = all_dates[np.where(all_dates > start_search_date)[0]]
         if dates.size == 0:
             dates = all_dates[-1:]
 
         # Find the next operational date, and if no available dates, return the time
         # until the end of the forecast period
-        date_diff = set(dates.date).difference(self.settings.non_operational_dates_set)  # type: ignore
+        date_diff = set(dates.date).difference(self.settings.non_operational_dates_set)
         if not date_diff:
             diff = ((max(dates) - current).days + 1) * HOURS_IN_DAY
             return diff
         next_available = min(date_diff)
         next_available = dates[np.where(dates.date == next_available)[0][0]]
 
         # Compute the difference between the current time and the future date
```

### Comparing `wombat-0.6.2/wombat/core/port.py` & `wombat-0.7.0/wombat/core/port.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-"""
-Creates the `Port` class that provies the tow-to-port repair capabilities for offshore
-floating wind farms. The `Port` will control a series of tugboats enabled through the
-"TOW" capability that get automatically dispatched once a tow-to-port repair is
-submitted and a tugboat is available (`ServiceEquipment.at_port`). The `Port` also
+"""Creates the `Port` class that provies the tow-to-port repair capabilities for
+offshore floating wind farms. The `Port` will control a series of tugboats enabled
+through the "TOW" capability that get automatically dispatched once a tow-to-port repair
+is submitted and a tugboat is available (`ServiceEquipment.at_port`). The `Port` also
 controls any mooring repairs through the "AHV" capability, which operates similarly to
 the tow-to-port except that it will not be released until the repair is completed, and
 operates on a strict shift scheduling basis.
 """
 
 from __future__ import annotations
 
@@ -26,33 +25,39 @@
 from wombat.utilities.time import hours_until_future_hour
 from wombat.core.environment import WombatEnvironment
 from wombat.core.data_classes import PortConfig, Maintenance, RepairRequest
 from wombat.core.repair_management import RepairManager
 from wombat.core.service_equipment import ServiceEquipment
 
 
+# Numpy random generation initialization
+random_generator = np.random.default_rng(seed=42)
+
+
 class Port(RepairsMixin, FilterStore):
     """The offshore wind base port that operates tugboats and performs tow-to-port
     repairs.
 
     .. note:: The operating costs for the port are incorporated into the ``FixedCosts``
-        functionality in the high-levl cost bucket: ``operations_management_administration``
-        or the more granula cost bucket: ``marine_management``
+        functionality in the high-levl cost bucket:
+        ``operations_management_administration`` or the more granula cost bucket:
+        ``marine_management``
 
     Parameters
     ----------
     env : WombatEnvironment
         The simulation environment instance.
     windfarm : Windfarm
         The simulation windfarm instance.
     repair_manager : RepairManager
         The simulation repair manager instance.
     config : dict | str | Path
-        A path to a YAML object or dictionary encoding the port's configuration settings.
-        This will be loaded into a ``PortConfig`` object during initialization.
+        A path to a YAML object or dictionary encoding the port's configuration
+        settings. This will be loaded into a ``PortConfig`` object during
+        initialization.
 
     Attributes
     ----------
     env : WombatEnvironment
         The simulation environment instance.
     windfarm : Windfarm
         The simulation windfarm instance.
@@ -66,15 +71,15 @@
     turbine_manager : simpy.Resource
         A SimPy ``Resource`` object that limits the number of turbines that can be towed
         to port, so as not to overload the quayside waters, which is controlled by
         ``settings.max_operations``.
     crew_manager : simpy.Resource
         A SimPy ``Resource`` object that limts the number of repairs that can be
         occurring at any given time, which is controlled by ``settings.n_crews``.
-    tugboat_manager : simpy.FilterStore
+    service_equipment_manager : simpy.FilterStore
         A SimPy ``FilterStore`` object that acts as a coordination system for the
         registered tugboats to tow turbines between port and site. In order to tow
         in either direction they must be filtered by ``ServiceEquipment.at_port``. This
         is generated from the tugboat definitions in ``settings.tugboats``.
     active_repairs : dict[str, dict[str, simpy.events.Event]]
         A nested dictionary of turbines, and its associated request IDs with a SimPy
         ``Event``. The use of events allows them to automatically succeed at the end of
@@ -91,24 +96,26 @@
     ) -> None:
         super().__init__(env, np.inf)
 
         self.env = env
         self.windfarm = windfarm
         self.manager = repair_manager
         self.requests_serviced: set[str] = set()
+        self.invalid_systems: list[str] = []
 
         self.manager._register_port(self)
 
         if not isinstance(config, dict):
             try:
                 config = load_yaml(env.data_dir / "project/port", config)
             except FileNotFoundError:
                 config = load_yaml(env.data_dir / "repair", config)  # type: ignore
                 logging.warning(
-                    "DeprecationWarning: In v0.7, all port configurations must be located in: '<library>/project/port/"
+                    "DeprecationWarning: In v0.8, all port configurations must be"
+                    " located in: '<library>/project/port/"
                 )
         assert isinstance(config, dict)
         self.settings = PortConfig.from_dict(config)
 
         self._check_working_hours(which="env")
         self.settings.set_non_operational_dates(
             self.env.non_operational_start,
@@ -124,34 +131,34 @@
             self.env.reduced_speed,
         )
 
         # Instantiate the crews, tugboats, and turbine availability
         assert isinstance(self.settings, PortConfig)
         self.turbine_manager = simpy.Resource(env, self.settings.max_operations)
         self.crew_manager = simpy.Resource(env, self.settings.n_crews)
-        self.tugboat_manager = simpy.FilterStore(env, len(self.settings.tugboats))
 
-        tugboats = []
+        service_equipment = []
         for t in self.settings.tugboats:
             tugboat = ServiceEquipment(self.env, self.windfarm, repair_manager, t)
             tugboat._register_port(self)
-            tugboats.append(tugboat)
+            service_equipment.append(tugboat)
 
-        self.tugboat_manager.items = tugboats
+        self.service_equipment_manager = simpy.FilterStore(env, len(service_equipment))
+        self.service_equipment_manager.items = service_equipment
         self.active_repairs: dict[str, dict[str, simpy.events.Event]] = {}
 
         # Create partial functions for the labor and equipment costs for clarity
         self.initialize_cost_calculators(which="port")
 
         # Run the annualized fee logger
         if self.settings.annual_fee > 0:
             self.env.process(self._log_annual_fee())
 
     def _log_annual_fee(self):
-        """Logs the annual port lease fee on a monthly-basis"""
+        """Logs the annual port lease fee on a monthly-basis."""
         assert isinstance(self.settings, PortConfig)
         monthly_fee = self.settings.annual_fee / 12.0
         ix_month_starts = self.env.weather.index.day == 1  # 1st of the month
         ix_month_starts &= self.env.weather.index.hour == 0  # at midnight
         ix_month_starts = np.where(ix_month_starts)[0]
         ix_month_starts = ix_month_starts[ix_month_starts > 0]
 
@@ -201,23 +208,23 @@
 
         # Set the default hours to process and remaining hours for the repair
         hours_to_process = hours_remaining = request.details.time
 
         # Create the shared logging among the processes
         system = self.windfarm.system(request.system_id)
         subassembly = getattr(system, request.subassembly_id)
-        shared_logging = dict(
-            agent=self.settings.name,
-            reason=request.details.description,
-            system_id=system.id,
-            system_name=system.name,
-            part_id=subassembly.id,
-            part_name=subassembly.name,
-            request_id=request.request_id,
-        )
+        shared_logging = {
+            "agent": self.settings.name,
+            "reason": request.details.description,
+            "system_id": system.id,
+            "system_name": system.name,
+            "part_id": subassembly.id,
+            "part_name": subassembly.name,
+            "request_id": request.request_id,
+        }
 
         # Continue repairing and waiting a shift until the remaining hours to complete
         # the repair is zero
         while hours_remaining > 0:
             current = self.env.simulation_time
 
             # Check if the workday is limited by shifts and adjust to stay within shift
@@ -232,15 +239,15 @@
                 )
                 continue
 
             # Process the repair for the minimum of remaining hours to completion and
             # hours available in the shift
             hours_to_process = min(hours_to_process, hours_remaining)
             yield self.env.process(
-                self.process_repair(hours_to_process, request.details, **shared_logging)  # type: ignore
+                self.process_repair(hours_to_process, request.details, **shared_logging)
             )
 
             # Decrement the remaining hours and reset the default hours to process back
             # to the remaining repair time
             hours_remaining -= hours_to_process
             hours_to_process = hours_remaining
 
@@ -258,14 +265,15 @@
             request_id=request.request_id,
         )
 
         # Make the crew available again
         self.crew_manager.release(crew_request)
 
         self.active_repairs[request.system_id][request.request_id].succeed()
+        self.env.process(self.manager.register_repair(request, port=True))
 
     def transfer_requests_from_manager(
         self, system_id: str
     ) -> None | list[RepairRequest]:
         """Gets all of a given system's repair requests from the simulation's repair
         manager, removes them from that queue, and puts them in the port's queue.
 
@@ -311,29 +319,30 @@
         system_id : str
             The ``System.id`` that is has been towed to port.
         """
         self.active_repairs[system_id] = {}
         requests = self.transfer_requests_from_manager(system_id)
         if requests is not None:
             self.requests_serviced.update([r.request_id for r in requests])
-            [self.env.process(self.repair_single(request)) for request in requests]  # type: ignore
+            [self.env.process(self.repair_single(request)) for request in requests]
 
     def run_tow_to_port(self, request: RepairRequest) -> Generator[Process, None, None]:
         """The method to initiate a tow-to-port repair sequence.
 
         The process follows the following following routine:
 
         1. Request a tugboat from the tugboat resource manager and wait
         2. Runs ``ServiceEquipment.tow_to_port``, which encapsulates the traveling to
             site, unmooring, and return tow with a turbine
         3. Transfers the the turbine's repair log to the port, and gets all available
            crews to work on repairs immediately
         4. Requests a tugboat to return the turbine to site
         5. Runs ``ServiceEquipment.tow_to_site()``, which encapsulates the tow back to
-           site, reconnection, resetting the operating status, and returning back to port
+           site, reconnection, resetting the operating status, and returning back to
+           port
 
         Parameters
         ----------
         request : RepairRequest
             The request that initiated the process. This is primarily used for logging
             purposes.
 
@@ -342,70 +351,89 @@
         Generator[Process, None, None]
             The series of events constituting the tow-to-port repairs
         """
         # If the request has already been addressed, return
         if request.request_id in self.requests_serviced:
             return
 
+        # Double check in case a delay causes multiple vessels to be interacting with
+        # the same turbine
+
+        # Add the requested system to the list of systems undergoing or registered to be
+        # undergoing repairs, so this method can't be run again on the same system
+        self.invalid_systems.append(request.system_id)
+
         # If the system is already undergoing repairs from other servicing equipment,
         # then wait until it's done being serviced
-        if request.system_id in self.manager.invalid_systems:
-            yield self.windfarm.system(request.system_id).servicing  # type: ignore
+        servicing = self.windfarm.system(request.system_id).servicing
+
+        # Wait for a spot to open up in the port queue
+        turbine_request = self.turbine_manager.request()
+
+        yield turbine_request & servicing
+        seconds_to_wait, *_ = random_generator.integers(low=0, high=30, size=1) / 3600.0
+        yield self.env.timeout(seconds_to_wait)
+        yield self.windfarm.system(request.system_id).servicing
 
         # Halt the turbine before going further to avoid issue with requests being
         # being submitted between now and when the tugboat gets to the turbine
         self.manager.halt_requests_for_system(self.windfarm.system(request.system_id))
 
+        # Request a tugboat to retrieve the turbine
+        tugboat = yield self.service_equipment_manager.get(
+            lambda x: x.at_port
+            and (not x.dispatched)
+            and "TOW" in x.settings.capability
+        )
+
         # Check that there is enough time to complete towing, connection, and repairs
         # before starting the process, otherwise, wait until the next operational period
         # TODO: use a more sophisticated guess on timing, other than 20 days
         current = self.env.simulation_time.date()
         check_range = set(
             pd.date_range(current, current + pd.Timedelta(days=20), freq="D").date
         )
-        intersection = check_range.intersection(self.settings.non_operational_dates_set)  # type: ignore
+        intersection = check_range.intersection(self.settings.non_operational_dates_set)
         if intersection:
             hours_to_next = self.hours_to_next_operational_date(
                 start_search_date=max(intersection)
             )
             self.env.log_action(
                 agent=self.settings.name,
                 action="delay",
                 reason="non-operational period",
                 additional="waiting for next operational period",
                 duration=hours_to_next,
             )
             yield self.env.timeout(hours_to_next)  # type: ignore
 
         self.requests_serviced.update([request.request_id])
-
-        # Wait for a spot to open up in the port queue
-        turbine_request = self.turbine_manager.request()
-        yield turbine_request  # type: ignore
-
-        # Request a tugboat to retrieve the turbine
-        tugboat = yield self.tugboat_manager.get(lambda x: x.at_port)  # type: ignore
         yield self.env.process(tugboat.run_tow_to_port(request))  # type: ignore
 
         # Make the tugboat available again
-        self.tugboat_manager.put(tugboat)
+        yield self.service_equipment_manager.put(tugboat)
 
         # Transfer the repairs to the port queue, which will initiate the repair process
         self.run_repairs(request.system_id)
 
         # Wait for the repairs to complete
-        yield simpy.AllOf(self.env, self.active_repairs[request.system_id].values())  # type: ignore
+        yield simpy.AllOf(self.env, self.active_repairs[request.system_id].values())
 
-        # Request a tugboat to tow the turbine back to site, and open up the turbine queue
-        tugboat = yield self.tugboat_manager.get(lambda x: x.at_port)  # type: ignore
+        # Request a tugboat to tow the turbine back to site, and open the turbine queue
+        tugboat = yield self.service_equipment_manager.get(
+            lambda x: x.at_port
+            and (not x.dispatched)
+            and "TOW" in x.settings.capability
+        )
         self.turbine_manager.release(turbine_request)
         yield self.env.process(tugboat.run_tow_to_site(request))  # type: ignore
+        self.invalid_systems.pop(self.invalid_systems.index(request.system_id))
 
         # Make the tugboat available again
-        self.tugboat_manager.put(tugboat)
+        yield self.service_equipment_manager.put(tugboat)
 
     def run_unscheduled_in_situ(
         self, request: RepairRequest
     ) -> Generator[Process, None, None]:
         """Runs the in-situ repair processes for port-based servicing equipment such as
         tugboats that will always return back to port, but are not necessarily a feature
         of the windfarm itself, such as a crew transfer vessel.
@@ -421,34 +449,48 @@
         Generator[Process, None, None]
             The travel and repair processes.
         """
         # If the request has already been addressed, return
         if request.request_id in self.requests_serviced:
             return
 
+        # If the system is already undergoing repairs from other servicing equipment,
+        # then wait until it's done being serviced, then double check
+        yield self.windfarm.system(request.system_id).servicing
+        seconds_to_wait, *_ = random_generator.integers(low=0, high=30, size=1) / 3600.0
+        yield self.env.timeout(seconds_to_wait)
+        yield self.windfarm.system(request.system_id).servicing
+
+        # Halt the turbine before going further to avoid issue with requests being
+        # being submitted between now and when the tugboat gets to the turbine
+        self.manager.halt_requests_for_system(self.windfarm.system(request.system_id))
         self.requests_serviced.update([request.request_id])
 
-        # Request a tugboat to retrieve the tugboat
-        tugboat = yield self.tugboat_manager.get(lambda x: x.at_port)  # type: ignore
-        assert isinstance(tugboat, ServiceEquipment)  # mypy: helper
+        # Request a vessel that isn't solely a towing vessel
+        vessel = yield self.service_equipment_manager.get(
+            lambda x: x.at_port
+            and (not x.dispatched)
+            and x.settings.capability != ["TOW"]
+        )
+        assert isinstance(vessel, ServiceEquipment)  # mypy: helper
         request = yield self.manager.get(lambda x: x == request)
-        yield self.env.process(tugboat.in_situ_repair(request))
+        yield self.env.process(vessel.in_situ_repair(request))
 
-        # If the tugboat finished mid-shift, the in-situ repair logic will keep it there,
-        # so ensure it returns back to port once it's complete
-        if not tugboat.at_port:
+        # If the tugboat finished mid-shift, the in-situ repair logic will keep it
+        # there, so ensure it returns back to port once it's complete
+        if not vessel.at_port:
             yield self.env.process(
-                tugboat.travel(
+                vessel.travel(
                     start="site",
                     end="port",
-                    agent=tugboat.settings.name,
+                    agent=vessel.settings.name,
                     reason=f"{request.details.description} complete",
                     system_id=request.system_id,
                     system_name=request.system_name,
                     part_id=request.subassembly_id,
                     part_name=request.subassembly_name,
                     request_id=request.request_id,
                 )
             )
 
         # Make the tugboat available again
-        self.tugboat_manager.put(tugboat)
+        yield self.service_equipment_manager.put(vessel)
```

### Comparing `wombat-0.6.2/wombat/core/post_processor.py` & `wombat-0.7.0/wombat/core/post_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The postprocessing metric computation."""
 from __future__ import annotations
 
 import logging
+import warnings
 from copy import deepcopy
 from math import fsum
 from pathlib import Path
 from itertools import product
 
 import numpy as np
 import PySAM
@@ -50,36 +51,39 @@
         raise ValueError(f"``frequency`` must be one of {opts}.")  # type: ignore
     return frequency
 
 
 def _calculate_time_availability(
     availability: np.ndarray, by_turbine: bool = False
 ) -> float | np.ndarray:
-    """Calculates the availability ratio of the whole timeseries or the whole timeseries, by turbine.
+    """Calculates the availability ratio of the whole timeseries or the whole
+    timeseries, by turbine.
 
     Parameters
     ----------
     availability : np.ndarray
         Timeseries array of operating ratios.
     by_turbine : bool, optional
-        If True, calculates the availability rate of each column, otherwise across the whole array, by default False.
+        If True, calculates the availability rate of each column, otherwise across the
+        whole array, by default False.
 
     Returns
     -------
     float | np.ndarray
-        Availability ratio across the whole timeseries, or broken out by column (turbine).
+        Availability ratio across the whole timeseries, or broken out by column
+        (turbine).
     """
     availability = availability > 0
     if by_turbine:
         return availability.sum(axis=0) / availability.shape[0]
     return availability.sum() / availability.size
 
 
 class Metrics:
-    """The metric computation class that will store the logged outputs and compile results."""
+    """The metric computation class for storing logs and compiling results."""
 
     _hourly_cost = "hourly_labor_cost"
     _salary_cost = "salary_labor_cost"
     _labor_cost = "total_labor_cost"
     _equipment_cost = "equipment_cost"
     _materials_cost = "materials_cost"
     _total_cost = "total_cost"
@@ -112,30 +116,33 @@
         """Initializes the Metrics class.
 
         Parameters
         ----------
         data_dir : str | Path
             This should be the same as was used for running the analysis.
         events : str | pd.DataFrame
-            Either a pandas ``DataFrame`` or filename to be used to read the csv log data.
+            Either a pandas ``DataFrame`` or filename to be used to read the csv log
+            data.
         operations : str | pd.DataFrame
-            Either a pandas ``DataFrame`` or filename to be used to read the csv log data.
+            Either a pandas ``DataFrame`` or filename to be used to read the csv log
+            data.
         potential : str | pd.DataFrame
             Either a pandas ``DataFrame`` or a filename to be used to read the csv
             potential power production data.
         production : str | pd.DataFrame
             Either a pandas ``DataFrame`` or a filename to be used to read the csv power
             production data.
         inflation_rate : float
             The inflation rate to be applied to all dollar amounts from the analysis
             starting year to ending year.
         project_capacity : float
             The project's rated capacity, in MW.
         turbine_capacities : Union[float, List[float]]
-            The capacity of each individual turbine corresponding to ``turbine_id``, in kW.
+            The capacity of each individual turbine corresponding to ``turbine_id``, in
+            kW.
         substation_id : str | list[str]
             The substation id(s).
         turbine_id : str | list[str]
             The turbine id(s).
         substation_turbine_map : dict[str, dict[str, list[str]]]
             A copy of ``Windfarm.substation_turbine_map``. This is a dictionary mapping
             of the subation IDs (keys) and a nested dictionary of its associated turbine
@@ -146,16 +153,16 @@
             ``ServiceEquipment.settings.name`` for each ``ServiceEquipment`` in the
             simulation.
         fixed_costs : str | None
             The filename of the project's fixed costs.
         SAM_settings : str | None
             The SAM settings YAML file located in <data_dir>/windfarm/<SAM_settings>
             that should end in ".yaml". If no input is provided, then the model will
-            raise a ``NotImplementedError`` when the SAM-powered metrics are attempted to
-            be accessed.
+            raise a ``NotImplementedError`` when the SAM-powered metrics are attempted
+            to be accessed.
 
             .. warning:: This functionality relies heavily on the user to configure
                 correctly. More information can be found at:
                 https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html
         """
         self.data_dir = Path(data_dir)
         if not self.data_dir.is_dir():
@@ -165,19 +172,22 @@
         self.project_capacity = project_capacity
 
         if fixed_costs is None:
             # Create a zero-cost FixedCosts object
             self.fixed_costs = FixedCosts.from_dict({"operations": 0})  # type: ignore
         else:
             try:
+                assert isinstance(fixed_costs, str)
                 fixed_costs = load_yaml(self.data_dir / "project/config", fixed_costs)
             except FileNotFoundError:
-                fixed_costs = load_yaml(self.data_dir / "windfarm", fixed_costs)  # type: ignore
+                assert isinstance(fixed_costs, str)
+                fixed_costs = load_yaml(self.data_dir / "windfarm", fixed_costs)
                 logging.warning(
-                    "DeprecationWarning: In v0.7, all fixed cost configurations must be located in: '<library>/project/config/"
+                    "DeprecationWarning: In v0.8, all fixed cost configurations must be"
+                    " located in: '<library>/project/config/"
                 )
             self.fixed_costs = FixedCosts.from_dict(fixed_costs)  # type: ignore
 
         if isinstance(substation_id, str):
             substation_id = [substation_id]
         self.substation_id = substation_id
 
@@ -190,15 +200,15 @@
             pd.concat([pd.DataFrame(val) for val in substation_turbine_map.values()])
             .set_index("turbines")
             .T
         )
 
         if isinstance(service_equipment_names, str):
             service_equipment_names = [service_equipment_names]
-        self.service_equipment_names = sorted(list(set(service_equipment_names)))
+        self.service_equipment_names = sorted(set(service_equipment_names))
 
         if isinstance(turbine_capacities, (float, int)):
             turbine_capacities = [turbine_capacities]
         self.turbine_capacities = turbine_capacities
 
         if isinstance(events, str):
             events = self._read_data(events)
@@ -221,15 +231,16 @@
             try:
                 self.sam_settings = load_yaml(
                     self.data_dir / "project/config", SAM_settings
                 )
             except FileNotFoundError:
                 self.sam_settings = load_yaml(self.data_dir / "windfarm", SAM_settings)
                 logging.warning(
-                    "DeprecationWarning: In v0.7, all SAM configurations must be located in: '<library>/project/config/"
+                    "DeprecationWarning: In v0.8, all SAM configurations must be"
+                    " located in: '<library>/project/config/"
                 )
 
             self._setup_pysam()
         else:
             self.sam_settings = None
             self.financial_model = None
 
@@ -252,16 +263,16 @@
             The class object.
         """
         data = load_yaml(fpath, fname)
         metrics = cls(**data)
         return metrics
 
     def _tidy_data(self, data: pd.DataFrame, kind: str) -> pd.DataFrame:
-        """Tidies the "raw" csv-converted data to be able to be used among the ``Metrics``
-        class.
+        """Tidies the "raw" csv-converted data to be able to be used among the
+        ``Metrics`` class.
 
         Parameters
         ----------
         data : pd.DataFrame
             The csv log data.
         kind : str
             The category of the input provided to ``data``. Should be one of:
@@ -271,15 +282,19 @@
              - "production"
 
         Returns
         -------
         pd.DataFrame
             A tidied data frame to be used for all the operations in this class.
         """
-        data = data = data.convert_dtypes()
+        # Ignore odd pandas casting error for pandas>=1.5(?)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            data = data = data.convert_dtypes()
+
         if data.index.name != "datetime":
             try:
                 data.datetime = pd.to_datetime(data.datetime)
             except AttributeError:
                 data["datetime"] = pd.to_datetime(data.env_datetime)
             data.index = data.datetime
             data = data.drop(labels="datetime", axis=1)
@@ -354,19 +369,19 @@
                 adjusted_inflation *= self.inflation_rate
 
         return events
 
     def _setup_pysam(self) -> None:
         """Creates and executes the PySAM model for financial metrics."""
         # Define the model and import the SAM settings file.
-        self.financial_model = pysam_singleowner_financial_model.default(  # type: ignore
+        self.financial_model = pysam_singleowner_financial_model.default(
             "WindPowerSingleOwner"
         )
         model_data = pssc.dict_to_ssc_table(self.sam_settings, "singleowner")
-        self.financial_model = pysam_singleowner_financial_model.wrap(model_data)  # type: ignore
+        self.financial_model = pysam_singleowner_financial_model.wrap(model_data)
 
         # Remove the leap year production
         leap_year_ix = self.production.index.month == 2
         leap_year_ix &= self.production.index.day == 29
         generation = self.production.loc[~leap_year_ix].windfarm.values
 
         # Create a years variable for later use with the PySAM outputs
@@ -409,23 +424,24 @@
         frequency = _check_frequency(frequency, which="all")
 
         by = by.lower().strip()
         if by not in ("windfarm", "turbine"):
             raise ValueError('``by`` must be one of "windfarm" or "turbine".')
         by_turbine = by == "turbine"
 
-        # Determine the operational capacity of each turbine with substation downtime impacts
+        # Determine the operational capacity of each turbine with substation downtime
         operations_cols = ["year", "month", "day", "windfarm"] + self.turbine_id
         turbine_operations = self.operations[operations_cols].copy()
         for sub, val in self.substation_turbine_map.items():
             turbine_operations[val["turbines"]] *= self.operations[[sub]].values
 
         hourly = turbine_operations.loc[:, self.turbine_id].values
 
-        # TODO: The below should be better summarized as: (availability > 0).groupby().sum() / groupby().count()
+        # TODO: The below should be better summarized as:
+        # (availability > 0).groupby().sum() / groupby().count()
 
         if frequency == "project":
             availability = _calculate_time_availability(hourly, by_turbine=by_turbine)
             if not by_turbine:
                 return pd.DataFrame([availability], columns=["windfarm"])
             availability = pd.DataFrame(
                 availability.reshape(1, -1), columns=self.turbine_id  # type: ignore
@@ -584,15 +600,15 @@
         if frequency == "project":
             if not by_turbine:
                 potential = production.shape[0] * self.project_capacity * 1000.0
                 production = production.values.sum()
                 return pd.DataFrame([production / potential], columns=["windfarm"])
 
             potential = production.shape[0] * np.array(self.turbine_capacities)
-            return pd.DataFrame((production.sum(axis=0) / potential)).T
+            return pd.DataFrame(production.sum(axis=0) / potential).T
 
         production["year"] = production.index.year.values
         production["month"] = production.index.month.values
 
         if frequency == "annual":
             group_cols = ["year"]
         elif frequency == "monthly":
@@ -610,16 +626,16 @@
         else:
             capacity = self.project_capacity
             production = production.sum(axis=1)
             columns = [by]
         return pd.DataFrame(production / potential, columns=columns)
 
     def task_completion_rate(self, which: str, frequency: str) -> float | pd.DataFrame:
-        """Calculates the task completion rate over a project's lifetime as a single value,
-        annual average, or monthly average for the whole windfarm or by turbine.
+        """Calculates the task completion rate over a project's lifetime as a single
+        value, annual average, or monthly average for the whole windfarm or by turbine.
 
         .. note:: This currently assumes that if there are multiple substations, that
           the turbines are all connected to multiple.
 
         Parameters
         ----------
         which : str
@@ -739,15 +755,16 @@
                 - year (if appropriate for frequency)
                 - month (if appropriate for frequency)
                 - then any equipment names as they appear in the logs
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_equipment`` is not one of ``True`` or ``False``.
         """
         frequency = _check_frequency(frequency, which="all")
 
         if not isinstance(by_equipment, bool):
             raise ValueError("`by_equipment` must be one of `True` or `False`")
@@ -920,28 +937,30 @@
             - month (if appropriate for frequency)
             - Total Crew Hours at Sea
             - {ServiceEquipment.settings.name} (if broken out)
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_equipment`` is not one of ``True`` or ``False``.
         ValueError
             If ``vessel_crew_assumption`` is not a dictionary.
         """
         frequency = _check_frequency(frequency, which="all")
 
         if not isinstance(by_equipment, bool):
             raise ValueError("``by_equipment`` must be one of ``True`` or ``False``")
 
         if not isinstance(vessel_crew_assumption, dict):
             raise ValueError(
-                "`vessel_crew_assumption` must be a dictionary of vessel name (keys) and number of crew (values)"
+                "`vessel_crew_assumption` must be a dictionary of vessel name (keys)"
+                " and number of crew (values)"
             )
 
         # Filter by the at sea indicators and required columns
         at_sea = self.events
         at_sea = at_sea.loc[
             at_sea.location.isin(("enroute", "site", "system"))
             & at_sea.agent.isin(self.service_equipment_names),
@@ -1035,30 +1054,31 @@
         by_direction : bool, optional
             Indicates whether the values are with respect to the direction a turbine is
             towed (True) or not (False), by default False.
 
         Returns
         -------
         float | pd.DataFrame
-            Returns either a float for whole project-level costs or a pandas ``DataFrame``
-            with columns:
+            Returns either a float for whole project-level costs or a pandas
+            ``DataFrame`` with columns:
 
             - year (if appropriate for frequency)
             - month (if appropriate for frequency)
             - total_tows
             - total_tows_to_port (if broken out)
             - total_tows_to_site (if broken out)
             - {ServiceEquipment.settings.name}_total_tows (if broken out)
             - {ServiceEquipment.settings.name}_to_port (if broken out)
             - {ServiceEquipment.settings.name}_to_site (if broken out)
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_tug`` is not one of ``True`` or ``False``.
         ValueError
             If ``by_direction`` is not one of ``True`` or ``False``.
         """
         frequency = _check_frequency(frequency, which="all")
 
@@ -1160,15 +1180,15 @@
 
             if frequency == "project":
                 tug_sums = pd.DataFrame(tug_sums_by_direction.sum()).T
             else:
                 tug_sums = tug_sums_by_direction.reset_index().groupby(total_cols).sum()
             assert isinstance(tug_sums, pd.DataFrame)  # mypy checking
             tug_sums = tug_sums.rename(
-                columns=dict((t, f"{t}_total_tows") for t in tug_sums.columns)
+                columns={t: f"{t}_total_tows" for t in tug_sums.columns}
             )
             assert isinstance(tug_sums, pd.DataFrame)  # mypy checking
             total = pd.DataFrame(
                 tug_sums.sum(axis=1), columns=["total_tows"]
             ).reset_index()
         else:
             if not by_direction:
@@ -1221,15 +1241,15 @@
                     if frequency == "project":
                         _total = pd.DataFrame(
                             tug_sums_by_direction.loc[s]
                         ).T.reset_index(drop=True)
                     else:
                         _total = tug_sums_by_direction.loc[s]
                     total_tows = total_tows.join(
-                        _total.rename(columns=dict((t, f"{t}_{s}") for t in tugboats)),
+                        _total.rename(columns={t: f"{t}_{s}" for t in tugboats}),
                         how="outer",
                     ).fillna(0)
                 total_tows = total_tows.reset_index()[columns]
                 if time_cols:
                     return total_tows.set_index(time_cols)
                 else:
                     return total_tows
@@ -1266,27 +1286,28 @@
         by_type : bool, optional
             Indicates whether the values are with resepect to the labor types
             (True) or not (False), by default False.
 
         Returns
         -------
         float | pd.DataFrame
-            Returns either a float for whole project-level costs or a pandas ``DataFrame``
-            with columns:
+            Returns either a float for whole project-level costs or a pandas
+            ``DataFrame`` with columns:
 
             - year (if appropriate for frequency)
             - month (if appropriate for frequency)
             - total_labor_cost
             - hourly_labor_cost (if broken out)
             - salary_labor_cost (if broken out)
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_type`` is not one of ``True`` or ``False``.
         """
         frequency = _check_frequency(frequency, which="all")
 
         if not isinstance(by_type, bool):
             raise ValueError("``by_type`` must be one of ``True`` or ``False``")
@@ -1304,26 +1325,32 @@
         if frequency == "annual":
             group_filter = ["year"]
         elif frequency == "monthly":
             group_filter = ["month"]
         elif frequency == "month-year":
             group_filter = ["year", "month"]
 
-        costs = self.events.groupby(group_filter).sum()[labor_cols].fillna(value=0)
+        costs = (
+            self.events.loc[:, labor_cols + group_filter]
+            .groupby(group_filter)
+            .sum()
+            .fillna(value=0)
+        )
         if not by_type:
             return pd.DataFrame(costs[self._labor_cost])
         return costs
 
     def equipment_labor_cost_breakdowns(
         self, frequency: str, by_category: bool = False
     ) -> pd.DataFrame:
-        """Calculates the producitivty cost breakdowns for the simulation at a project, annual, or
-        monthly level that can be broken out to include the equipment and labor components.
+        """Calculates the producitivty cost breakdowns for the simulation at a project,
+        annual, or monthly level that can be broken out to include the equipment and
+        labor components.
 
-        .. note:: Does not produce a value if there is no cost associated with a "reason".
+        .. note:: Doesn't produce a value if there's no cost associated with a "reason".
 
         Parameters
         ----------
         frequency : str
             One of "project", "annual", "monthly", or "month-year".
         by_category : bool, optional
             Indicates whether to include the equipment and labor categories (True) or
@@ -1341,15 +1368,16 @@
                 - total_labor_cost (if by_category == ``True``)
                 - equipment_cost (if by_category == ``True``)
                 - total_cost (if broken out)
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_category`` is not one of ``True`` or ``False``.
         """
         frequency = _check_frequency(frequency, which="all")
         if not isinstance(by_category, bool):
             raise ValueError("``by_equipment`` must be one of ``True`` or ``False``")
 
@@ -1378,15 +1406,14 @@
                 group_filter + self._cost_columns,
             ]
             .groupby(group_filter)
             .sum()
             .reset_index()
         )
         costs["display_reason"] = [""] * costs.shape[0]
-        group_filter.append("display_reason")
 
         non_shift_hours = (
             "not in working hours",
             "work shift has ended; waiting for next shift to start",
             "no more return visits will be made",
             "will return next year",
             "waiting for next operational period",
@@ -1405,28 +1432,27 @@
         costs.loc[costs.action == "mobilization", "display_reason"] = "Mobilization"
         costs.loc[
             costs.additional.isin(weather_hours), "display_reason"
         ] = "Weather Delay"
         costs.loc[costs.reason == "no requests", "display_reason"] = "No Requests"
 
         costs.reason = costs.display_reason
-        group_filter.pop(group_filter.index("action"))
-        group_filter.pop(group_filter.index("display_reason"))
-        group_filter.pop(group_filter.index("additional"))
 
-        drop_columns = [self._materials_cost]
+        drop_columns = [self._materials_cost, "display_reason", "additional", "action"]
         if not by_category:
             drop_columns.extend(
                 [
                     self._hourly_cost,
                     self._salary_cost,
                     self._labor_cost,
                     self._equipment_cost,
                 ]
             )
+        group_filter.pop(group_filter.index("additional"))
+        group_filter.pop(group_filter.index("action"))
         costs = costs.drop(columns=drop_columns)
         costs = costs.groupby(group_filter).sum().reset_index()
 
         month_year = frequency == "month-year"
         if frequency in ("annual", "month-year"):
             years = costs.year.unique()
             reasons = costs.reason.unique()
@@ -1504,45 +1530,46 @@
             Indicates whether component costs are going to be further broken out by the
             action being performed--repair, maintenance, and delay--(True) or not
             (False), by default False.
 
         Returns
         -------
         float | pd.DataFrame
-            Returns either a float for whole project-level costs or a pandas ``DataFrame``
-            with columns:
+            Returns either a float for whole project-level costs or a pandas
+            ``DataFrame`` with columns:
 
             - year (if appropriate for frequency)
             - month (if appropriate for frequency)
             - component
             - action (if broken out)
             - materials_cost (if broken out)
             - total_labor_cost (if broken out)
             - equipment_cost (if broken out)
             - total_cost
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_category`` is not one of ``True`` or ``False``.
         ValueError
             If ``by_action`` is not one of ``True`` or ``False``.
         """
         frequency = _check_frequency(frequency, which="all")
         if not isinstance(by_category, bool):
             raise ValueError("``by_equipment`` must be one of ``True`` or ``False``")
         if not isinstance(by_action, bool):
             raise ValueError("``by_equipment`` must be one of ``True`` or ``False``")
 
         part_filter = ~self.events.part_id.isna() & ~self.events.part_id.isin([""])
         events = self.events.loc[part_filter].copy()
 
-        # Need to simplify the cable identifiers to not include the connection information
+        # Need to simplify the cable identifiers to exclude the connection information
         events.loc[:, "component"] = [el.split("::")[0] for el in events.part_id.values]
 
         group_filter = []
         if frequency == "annual":
             group_filter.extend(["year"])
         elif frequency == "monthly":
             group_filter.extend(["month"])
@@ -1690,15 +1717,15 @@
         Parameters
         ----------
         frequency : str
             One of "project" or "annual", "monthly", ".
         resolution : st
             One of "low", "medium", or "high", where the values correspond to:
 
-            - low: ``FixedCosts.resolution["low"]``, corresponding to the itemized costs.
+            - low: ``FixedCosts.resolution["low"]``, corresponding to itemized costs.
             - medium: ``FixedCosts.resolution["medium"]``, corresponding to the
               overarching cost categories.
             - high: ``FixedCosts.resolution["high"]``, corresponding to a lump sum.
 
             These values can also be seen through the ``FixedCosts.hierarchy``
 
         Returns
@@ -1813,16 +1840,16 @@
         # Join the data frames and sum along the time axis and return
         column = "OpEx"
         opex = pd.concat(opex_items, axis=1)
         opex.loc[:, column] = opex.sum(axis=1)
         return opex[[column]]
 
     def process_times(self) -> pd.DataFrame:
-        """Calculates the time, in hours, to complete a repair/maintenance request, on both a
-        request to completion basis, and the actual time to complete the repair.
+        """Calculates the time, in hours, to complete a repair/maintenance request, on
+        both a request to completion basis, and the actual time to complete the repair.
 
         Returns
         -------
         pd.DataFrame
          - category (index): repair/maintenance category
          - time_to_completion: total number of hours from the time of request to the
            time of completion
@@ -1894,15 +1921,15 @@
         )
         timing = timing.join(
             downtime_df_min[["env_time"]]
             .join(downtime_df_max[["env_time"]], lsuffix="_min", rsuffix="_max")
             .diff(axis=1)[["env_time_max"]]
             .rename(columns={"env_time_max": "downtime"})
         )
-        timing.N = 1
+        timing["N"] = 1
 
         # Return only the categorically summed data
         return timing.groupby("category").sum().sort_index()
 
     def power_production(
         self, frequency: str, by: str = "windfarm", units: str = "gwh"
     ) -> float | pd.DataFrame:
@@ -1917,26 +1944,27 @@
             One of "windfarm" or "turbine".
         units : str
             One of "gwh", "mwh", or "kwh".
 
         Returns
         -------
         float | pd.DataFrame
-            Returns either a float for whole project-level costs or a pandas ``DataFrame``
-            with columns:
+            Returns either a float for whole project-level costs or a pandas
+            ``DataFrame`` with columns:
 
             - year (if appropriate for frequency)
             - month (if appropriate for frequency)
             - total_power_production
             - <turbine_id>_power_production (if broken out)
 
         Raises
         ------
         ValueError
-            If ``frequency`` is not one of "project", "annual", "monthly", or "month-year".
+            If ``frequency`` is not one of "project", "annual", "monthly", or
+            "month-year".
         ValueError
             If ``by_turbine`` is not one of ``True`` or ``False``.
         """
         frequency = _check_frequency(frequency, which="all")
 
         by = by.lower().strip()
         if by not in ("windfarm", "turbine"):
@@ -2029,23 +2057,25 @@
         elif frequency == "monthly":
             return npv.reset_index().groupby("month").sum()[["NPV"]]
         return npv[["NPV"]]
 
     def pysam_npv(self) -> float | pd.DataFrame:
         """Returns the project-level after-tax net present values (NPV).
 
-        See here for more: https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.cf_project_return_aftertax_npv
+        See here for more:
+        https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.cf_project_return_aftertax_npv
 
         .. warning::
             PySAM functionality is currently disabled due to changes made in the new API
             that need to be remapped.
 
         Raises
         ------
-        NotImplementedError: Raised if a PySAM input file is not provided to run the model.
+        NotImplementedError: Raised if a PySAM input file is not provided to run the
+        model.
 
         Returns
         -------
         float
             Final, project-level NPV, in $.
         """
         if self.financial_model is None:
@@ -2055,71 +2085,79 @@
         npv = self.financial_model.Outputs.cf_project_return_aftertax_npv
         npv = npv[len(self.years)]
         return npv
 
     def pysam_lcoe_real(self) -> float:
         """Returns the real levelized cost of energy (LCOE) from PySAM.
 
-        See here for more: https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.lcoe_real
+        See here for more:
+        https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.lcoe_real
 
         .. warning::
             PySAM functionality is currently disabled due to changes made in the new API
             that need to be remapped.
 
         Raises
         ------
-        NotImplementedError: Raised if a PySAM input file is not provided to run the model.
+        NotImplementedError: Raised if a PySAM input file is not provided to run the
+            model.
 
         Returns
         -------
         float
             Real LCOE, in $/kW.
         """
         if self.financial_model is None:
             raise NotImplementedError(
-                "No SAM inputs were provided, and 'pysam_lcoe_real()' cannot be calculated!"
+                "No SAM inputs were provided, and 'pysam_lcoe_real()' cannot be"
+                " calculated!"
             )
         return self.financial_model.Outputs.lcoe_real / 100.0
 
     def pysam_lcoe_nominal(self) -> float:
         """Returns the nominal levelized cost of energy (LCOE) from PySAM.
 
-        See here for more: https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.lcoe_nom
+        See here for more:
+        https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.lcoe_nom
 
         .. warning::
             PySAM functionality is currently disabled due to changes made in the new API
             that need to be remapped.
 
         Raises
         ------
-        NotImplementedError: Raised if a PySAM input file is not provided to run the model.
+        NotImplementedError: Raised if a PySAM input file is not provided to run the
+        model.
 
         Returns
         -------
         float
             Nominal LCOE, in $/kW.
         """
         if self.financial_model is None:
             raise NotImplementedError(
-                "No SAM inputs were provided, and 'pysam_lcoe_nominal()' cannot be calculated!"
+                "No SAM inputs were provided, and 'pysam_lcoe_nominal()' cannot"
+                " be calculated!"
             )
         return self.financial_model.Outputs.lcoe_nom / 100.0
 
     def pysam_irr(self) -> float:
         """Returns the project-level after-tax internal return rate (IRR).
 
-        See here for more: https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.cf_project_return_aftertax_irr
+        See here for more:
+        https://nrel-pysam.readthedocs.io/en/master/modules/Singleowner.html#PySAM.Singleowner.Singleowner.Outputs.cf_project_return_aftertax_irr
 
         .. warning::
             PySAM functionality is currently disabled due to changes made in the new API
             that need to be remapped.
 
         Raises
         ------
-        NotImplementedError: Raised if a PySAM input file is not provided to run the model.
+        NotImplementedError: Raised if a PySAM input file is not provided to run the
+            model.
 
         Returns
         -------
         pd.DataFrame
             Annual after-tax IRR value, in %.
         """
         if self.financial_model is None:
@@ -2128,37 +2166,39 @@
             )
         irr = self.financial_model.Outputs.cf_project_return_aftertax_irr
         irr = irr[len(self.years)]
         return irr
 
     def pysam_all_outputs(self) -> pd.DataFrame:
         """Returns all the possible PySAM outputs that are included in this module as
-        columns in the following order:
+        columns in the following order.
 
         - NPV
         - Nominal LCOE
         - Real LOCE
         - IRR
 
         .. warning::
            PySAM functionality is currently disabled due to changes made in the new API
            that need to be remapped.
 
         Raises
         ------
-        NotImplementedError: Raised if a PySAM input file is not provided to run the model.
+        NotImplementedError: Raised if a PySAM input file is not provided to run the
+            model.
 
         Returns
         -------
         pd.DataFrame
             Project financial values values.
         """
         if self.financial_model is None:
             raise NotImplementedError(
-                "No SAM inputs were provided, and 'pysam_all_outputs()' cannot be calculated!"
+                "No SAM inputs were provided, and 'pysam_all_outputs()' cannot"
+                " be calculated!"
             )
         financials = [
             self.pysam_npv(),
             self.pysam_lcoe_nominal(),
             self.pysam_lcoe_real(),
             self.pysam_irr(),
         ]
```

### Comparing `wombat-0.6.2/wombat/core/service_equipment.py` & `wombat-0.7.0/wombat/core/service_equipment.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 """
 # TODO: NEED A SPECIFIC STARTUP METHOD
 from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from math import ceil
-from typing import TYPE_CHECKING, Any, Optional, Generator
+from typing import TYPE_CHECKING, Any, Generator
 from pathlib import Path
 from datetime import timedelta
+from itertools import zip_longest
 
 import numpy as np
 import pandas as pd
 from simpy.events import Event, Process, Timeout
 from pandas.core.indexes.datetimes import DatetimeIndex
 
 from wombat.core import (
@@ -39,18 +40,22 @@
 from wombat.windfarm.system.subassembly import Subassembly
 
 
 if TYPE_CHECKING:
     from wombat.core import Port
 
 
+# Numpy random generation initialization
+random_generator = np.random.default_rng(seed=42)
+
+
 def consecutive_groups(data: np.ndarray, step_size: int = 1) -> list[np.ndarray]:
     """Generates the subgroups of an array where the difference between two sequential
     elements is equal to the ``step_size``. The intent is to find the length of delays
-    in a weather forecast
+    in a weather forecast.
 
     Parameters
     ----------
     data : np.ndarray
         An array of integers.
     step_size : int, optional
         The step size to be considered a consecutive number, by default 1.
@@ -136,15 +141,14 @@
     ----------
     system : System
         The turbine to be reset.
     """
     for subassembly in system.subassemblies:
         subassembly.operating_level = 1.0
         subassembly.recreate_processes()
-    system.servicing.succeed()
 
 
 class ServiceEquipment(RepairsMixin):
     """Provides a servicing equipment object that can handle various maintenance and
     repair tasks.
 
     Parameters
@@ -162,16 +166,16 @@
     ----------
     env : WombatEnvironment
         The simulation environment instance.
     windfarm : Windfarm
         The simulation windfarm instance.
     manager : RepairManager
         The simulation repair manager instance.
-    settings : PortConfig
-        The port's configuration settings, as provided by the user.
+    settings : ScheduledServiceEquipmentData | UnscheduledServiceEquipmentData
+        The servicing equipment's configuration settings, as provided by the user.
     onsite : bool
         Indicates if the servicing equipment is at the site (``True``), or not
         (``False``).
     enroute : bool
         Indicates if the servicing equipment is on its way to the site (``True``),
         or not (``False``).
     at_port : bool
@@ -207,44 +211,48 @@
             The ``RepairManager`` object.
         equipment_data_file : str
             The equipment settings file name with extension.
         """
         self.env = env
         self.windfarm = windfarm
         self.manager = repair_manager
-        self.onsite = False
+        self.onsite = False  # True: mobilized to the site, but not necessarily at_site
         self.dispatched = False
         self.enroute = False
         self.at_port = False
+        self.at_site = False
         self.at_system = False
         self.transferring_crew = False
         self.current_system = None  # type: str | None
+        self.port_based = False  # Changed to False if port is registered
+        self.settings: ScheduledServiceEquipmentData | UnscheduledServiceEquipmentData
 
         if isinstance(equipment_data_file, (str, Path)):
             try:
                 data = load_yaml(env.data_dir / "vessels", equipment_data_file)
             except FileNotFoundError:
                 data = load_yaml(env.data_dir / "repair/transport", equipment_data_file)
                 logging.warning(
-                    "DeprecationWarning: In v0.7, all servicing equipment configurations must be located in: '<library>/vessels/"
+                    "DeprecationWarning: In v0.8, all servicing equipment"
+                    " configurations must be located in: '<library>/vessels/"
                 )
         else:
             data = equipment_data_file
 
         try:
             if data["start_year"] < self.env.start_year:
                 data["start_year"] = self.env.start_year
             if data["end_year"] > self.env.end_year:
                 data["end_year"] = self.env.end_year
         except KeyError:
-            # Ignores for unscheduled maintenace equipment that would not have this input
+            # Ignores for unscheduled maintenace equipment that won't have this input
             pass
 
         # NOTE: mypy is not caught up with attrs yet :(
-        self.settings: ScheduledServiceEquipmentData | UnscheduledServiceEquipmentData = ServiceEquipmentData(data).determine_type()  # type: ignore
+        self.settings = ServiceEquipmentData(data).determine_type()  # type: ignore
 
         # Register servicing equipment with the repair manager if it is using an
         # unscheduled maintenance scenario, so it can be dispatched as needed
         if self.settings.strategy in UNSCHEDULED_STRATEGIES:
             self.manager._register_equipment(self)
 
         # Only run the equipment if it is on a scheduled basis, otherwise wait
@@ -271,24 +279,25 @@
             self.env.reduced_speed_start,
             self.env.start_year,
             self.env.reduced_speed_end,
             self.env.end_year,
             self.env.reduced_speed,
         )
 
-    def _register_port(self, port: "Port") -> None:
+    def _register_port(self, port: Port) -> None:
         """Method for a tugboat at attach the port for two-way communications. This also
         sets the vessel to be at the port, and updates the port_distance.
 
         Parameters
         ----------
         port : Port
             The port where the tugboat is based.
         """
         self.port = port
+        self.port_based = True
         self.at_port = True
         self.settings._set_port_distance(port.settings.site_distance)  # type: ignore
 
         self._check_working_hours(which="port")
 
         # Set the non-operational start/end dates if needed
         self.settings.set_non_operational_dates(
@@ -303,33 +312,31 @@
             port.settings.reduced_speed_start,
             self.env.start_year,
             port.settings.reduced_speed_end,
             self.env.end_year,
             port.settings.reduced_speed,
         )
 
-    def _set_location(self, end: str, set_current: Optional[str] = None) -> None:
+    def _set_location(self, end: str, set_current: str | None = None) -> None:
         """Keeps track of the servicing equipment by setting the location at either:
-        site, port, or a specific system
+        site, port, or a specific system.
 
         Parameters
         ----------
-        start : str
-            The starting location; one of "site", or "port"
         end : str
             The ending location; one of "site", or "port"
         set_current : str
             The ``System.id`` for the new current location, if one is to be set.
         """
         if end == "port":
             self.at_port = True
-            self.onsite = False
+            self.at_site = False
         else:
             self.at_port = False
-            self.onsite = True
+            self.at_site = True
         self.at_system = True if set_current is not None else False
         self.current_system = set_current
 
     def _weather_forecast(
         self, hours: int | float, which: str
     ) -> tuple[DatetimeIndex, np.ndarray, np.ndarray]:
         """Retrieves the weather forecast from the simulation environment, and
@@ -375,72 +382,81 @@
             and if False, then the traveling speed should be used, by default False.
 
         Returns
         -------
         float
             The maximum speed the servicing equipment should be traveling/towing at.
         """
+        assert hasattr(self.settings, "reduced_speed_dates_set")
         speed = self.settings.tow_speed if tow else self.settings.speed  # type: ignore
-        if self.env.simulation_time.date() in self.settings.reduced_speed_dates_set:  # type: ignore
+        if self.env.simulation_time.date() in self.settings.reduced_speed_dates_set:
             if speed > self.settings.reduced_speed:
                 speed = self.settings.reduced_speed
         return speed
 
     def get_next_request(self):
         """Gets the next request by the rig's method for processing repairs.
 
         Returns
         -------
         simpy.resources.store.FilterStoreGet
             The next ``RepairRequest`` to be processed.
         """
         if self.settings.method == "turbine":
             return self.manager.get_request_by_system(self.settings.capability)
-        elif self.settings.method == "severity":
-            return self.manager.get_next_highest_severity_request(
-                self.settings.capability
-            )
+        if self.settings.method == "severity":
+            return self.manager.get_request_by_severity(self.settings.capability)
 
     def enable_string_operations(self, cable: Cable) -> None:
         """Traverses the upstream cable and turbine connections and resets the
         ``System.cable_failure`` and ``Cable.downstream_failure`` until it hits
         another cable failure, then the loop exits.
 
         Parameters
         ----------
         subassembly : Cable
             The `Cable` or `System`
         """
         farm = self.manager.windfarm
         if cable.connection_type == "array":
             # If there is another failure downstream of the repaired cable, do nothing
-            if cable.downstream_failure:
+            if not cable.downstream_failure.triggered:
                 return
 
             # For each upstream turbine and cable, reset their operations
-            for t_id, c_id in zip(cable.upstream_nodes, cable.upstream_cables):
-                cable = farm.cable(c_id)
-                if cable.operating_level == 0:
-                    break
-                cable.downstream_failure.succeed()
-                farm.system(t_id).cable_failure.succeed()
+            nodes = deepcopy(cable.upstream_nodes)
+            cables = cable.upstream_cables
+            tid = nodes.pop(0)
+            turbine = farm.system(tid)
+            turbine.cable_failure.succeed()
+            for tid, cid in zip_longest(nodes, cables, fillvalue=None):  # type: ignore
+                if cid is not None:
+                    cable = farm.cable(cid)
+                    cable.downstream_failure.succeed()
+                    if not cable.broken.triggered:
+                        break
+                if tid is not None:  # only None for last cable on string
+                    turbine = farm.system(tid)
+                    turbine.cable_failure.succeed()
 
         if cable.connection_type == "export":
             # Reset the substation's cable failure
             farm.system(cable.end_node).cable_failure.succeed()
 
-            # For each string connected to the substation reset all the turbines and cables
-            # until another cable failure is encoountered, then move to the next string
-            for turbines, cables in zip(cable.upstream_nodes, cable.upstream_cables):
-                for t_id, c_id in zip(turbines, cables):
-                    cable = farm.cable(c_id)
-                    if cable.operating_level == 0:
-                        break
-                    cable.downstream_failure.succeed()
-                    farm.system(t_id).cable_failure.succeed()
+            # For each string connected to the substation reset all the turbines and
+            # cables until another cable failure is encoountered, then move to the next
+            # string
+            for t_list, c_list in zip(cable.upstream_nodes, cable.upstream_cables):
+                for t, c in zip_longest(t_list, c_list, fillvalue=None):  # type: ignore
+                    if c is not None:
+                        cable = farm.cable(c)
+                        if not cable.broken.triggered:
+                            break
+                        cable.downstream_failure.succeed()
+                    farm.system(t).cable_failure.succeed()
 
     def register_repair_with_subassembly(
         self,
         subassembly: Subassembly | Cable,
         repair: RepairRequest,
         starting_operating_level: float,
     ) -> None:
@@ -456,36 +472,39 @@
         repair : RepairRequest
             The request for repair that was submitted.
         starting_operating_level : float
             The operating level before a repair was started.
         """
         operation_reduction = repair.details.operation_reduction
 
-        if repair.cable and repair.details.operation_reduction == 1:
-            assert isinstance(subassembly, Cable)  # mypy helper
-            self.enable_string_operations(subassembly)
-
         # Put the subassembly/component back to good as new condition
         if repair.details.replacement:
-            subassembly.operating_level = 1
+            subassembly.operating_level = 1.0
             _ = self.manager.purge_subassembly_requests(
                 repair.system_id, repair.subassembly_id
             )
-        elif operation_reduction == 1:
+        if operation_reduction == 1:
             subassembly.operating_level = starting_operating_level
             subassembly.broken.succeed()
         elif operation_reduction == 0:
             subassembly.operating_level = starting_operating_level
         else:
             subassembly.operating_level /= 1 - operation_reduction
 
-        # Register that the servicing is now over
-        system = subassembly if isinstance(subassembly, Cable) else subassembly.system
-        system.servicing.succeed()
-        self.manager.enable_requests_for_system(repair.system_id)
+        if isinstance(subassembly, Subassembly):
+            self.manager.enable_requests_for_system(subassembly.system)
+        elif isinstance(subassembly, Cable):
+            # If the system is a cable, re-enable the upstream systems and cables
+            self.manager.enable_requests_for_system(subassembly)
+            if operation_reduction == 1:
+                self.enable_string_operations(subassembly)
+        else:
+            raise TypeError("`subassembly` was neither a `Cable` nor `Subassembly`.")
+
+        self.env.process(self.manager.register_repair(repair))
 
     def wait_until_next_operational_period(
         self, *, less_mobilization_hours: int = 0
     ) -> Generator[Timeout, None, None]:
         """Delays the crew and equipment until the start of the next operational
         period.
 
@@ -494,24 +513,25 @@
         Parameters
         ----------
         less_mobilization_hours : int
             The number of hours required for mobilization that will be subtracted from
             the waiting period to account for mobilization, by default 0.
 
         Yields
-        -------
+        ------
         Generator[Timeout, None, None]
             A Timeout event for the number of hours between when the function is called
             and when the next operational period starts.
         """
+        assert isinstance(self.settings, ScheduledServiceEquipmentData)
         current = self.env.simulation_time.date()
-        ix_match = np.where(current < self.settings.operating_dates)[0]  # type: ignore
+        ix_match = np.where(current < self.settings.operating_dates)[0]
         if ix_match.size > 0:
             still_in_operation = True
-            next_operating_date = self.settings.operating_dates[ix_match[0]]  # type: ignore
+            next_operating_date = self.settings.operating_dates[ix_match[0]]
             hours_to_next_shift = (
                 self.env.date_ix(next_operating_date)
                 - self.env.now
                 + self.settings.workday_start
                 - less_mobilization_hours
             )
         else:
@@ -523,14 +543,15 @@
             # the post processor filtering needs to be updated as well
             additional = "will return next year"
         else:
             additional = "no more return visits will be made"
 
         # Ensures that the statuses are correct
         self.at_port = False
+        self.at_site = False
         self.enroute = False
         self.onsite = False
 
         self.env.log_action(
             agent=self.settings.name,
             action="delay",
             reason="work is complete",
@@ -544,15 +565,15 @@
     def mobilize_scheduled(self) -> Generator[Timeout, None, None]:
         """Mobilizes the ServiceEquipment object by waiting for the next operational
         period, less the mobilization time, then logging the mobiliztion cost.
 
         NOTE: weather delays are not accounted for in this process.
 
         Yields
-        -------
+        ------
         Generator[Timeout, None, None]
             A Timeout event for the number of hours between when the function is called
             and when the next operational period starts.
         """
         mobilization_hours = self.settings.mobilization_days * HOURS_IN_DAY
         yield self.env.process(  # type: ignore
             self.wait_until_next_operational_period(
@@ -584,15 +605,15 @@
 
     def mobilize(self) -> Generator[Timeout, None, None]:
         """Mobilizes the ServiceEquipment object.
 
         NOTE: weather delays are not accounted for at this stage.
 
         Yields
-        -------
+        ------
         Generator[Timeout, None, None]
             A Timeout event for the number of hours the ServiceEquipment requires for
             mobilizing to the windfarm site.
         """
         self.env.log_action(
             agent=self.settings.name,
             action="mobilization",
@@ -619,16 +640,16 @@
 
     def find_uninterrupted_weather_window(
         self, hours_required: int | float
     ) -> tuple[int | float, bool]:
         """Finds the delay required before starting on a process that won't be able to
         be interrupted by a weather delay.
 
-        TODO: WEATHER FORECAST NEEDS TO BE DONE FOR ``math.floor(self.now)``, not the ceiling
-        or there will be a whole lot of rounding up errors on process times.
+        TODO: WEATHER FORECAST NEEDS TO BE DONE FOR ``math.floor(self.now)``, not the
+        ceiling or there will be a whole lot of rounding up errors on process times.
 
         Parameters
         ----------
         hours_required : int | float
             The number of uninterrupted of hours that a process requires for completion.
 
         Returns
@@ -722,33 +743,39 @@
 
         Parameters
         ----------
         hours : int | float
             The lenght, in hours, of the weather delay.
 
         Yields
-        -------
+        ------
         Generator[Event, Any, Any]
-            If the delay is more than 0 hours, then a ``Timeout`` is yielded of length ``hours``.
+            If the delay is more than 0 hours, then a ``Timeout`` is yielded of length
+            ``hours``.
         """
-        if hours > 0:
-            salary_cost = self.calculate_salary_cost(hours)
-            hourly_cost = 0  # contractors not paid for delays
-            equipment_cost = self.calculate_equipment_cost(hours)
-            self.env.log_action(
-                duration=hours,
-                action="delay",
-                additional="weather delay",
-                salary_labor_cost=salary_cost,
-                hourly_labor_cost=hourly_cost,
-                equipment_cost=equipment_cost,
-                **kwargs,
+        if hours < 0:
+            raise ValueError(
+                f"`hours` must be greater than 0 for {self.settings.name} to process"
+                " a weather delay"
             )
-            yield self.env.timeout(hours)
+        if hours == 0:
+            return
 
+        salary_cost = self.calculate_salary_cost(hours)
+        hourly_cost = 0  # contractors not paid for delays
+        equipment_cost = self.calculate_equipment_cost(hours)
+        self.env.log_action(
+            duration=hours,
+            action="delay",
+            additional="weather delay",
+            salary_labor_cost=salary_cost,
+            hourly_labor_cost=hourly_cost,
+            equipment_cost=equipment_cost,
+            **kwargs,
+        )
         yield self.env.timeout(hours)
 
     @cache
     def _calculate_intra_site_time(
         self, start: str | None, end: str | None
     ) -> tuple[float, float]:
         """Calculates the time it takes to travel between port and site or between
@@ -795,16 +822,16 @@
             Indicates if this travel is for towing (True), or not (False), by default
             False.
 
         Returns
         -------
         tuple[float, float]
             The length of the delay and the length of travel time, in hours.` -1 is
-            returned if there no weather windows, and the process will have to be attempted
-            again.
+            returned if there no weather windows, and the process will have to be
+            attempted again.
         """
         # Return 0 delay and travel time in the distance is zero
         if distance == 0:
             return 0, 0
 
         speed = self.get_speed(tow=tow)
         hours_required = distance / speed
@@ -863,15 +890,16 @@
         # Get the index for the end of the hour where the distance requred to be
         # traveled is reached.
         try:
             ix_hours = np.where(distance_traveled_sum >= distance)[0][0]
         except IndexError as e:
             # If an error occurs because an index maxes out the weather window, check
             # that it's not due to having reached the end of the simulation. If so,
-            # return the max amount of time, but if that's not the case re-raise the error.
+            # return the max amount of time, but if that's not the case re-raise the
+            # error.
             if self.env.weather.index.values[-1] in dt:
                 ix_hours = distance_traveled.size - 1
             else:
                 raise e
 
         # Shave off the extra timing to get the exact travel time
         total_hours = ix_hours + 1  # add 1 for 0-indexing
@@ -909,87 +937,95 @@
         hours : float, optional
             The number hours required for traveling between ``start`` and ``end``.
             If provided, no internal travel time will be calculated.
         distance : float, optional
             The distance, in km, to be traveled. Only used if hours is provided
 
         Yields
-        -------
+        ------
         Generator[Timeout | Process, None, None]
             The timeout event for traveling.
         """
         validate_end_points(start, end)
         if hours is None:
             hours = 0.0
             distance = 0.0
             additional = f"traveling from {start} to {end}"
 
             if start == end == "system":
                 additional = f"traveling from {self.current_system} to {set_current}"
                 hours, distance = self._calculate_intra_site_time(
                     self.current_system, set_current
                 )
-            elif set((start, end)) == set(("site", "port")):
+            elif {start, end} == {"site", "port"}:
                 additional = f"traveling from {start} to {end}"
                 distance = self.settings.port_distance
                 hours = self._calculate_interrupted_travel_time(distance)
         else:
             if distance is None:
                 raise ValueError("`distance` must be provided if `hours` is provided.")
 
-        # MyPy helper
-        assert isinstance(hours, float)
-        assert isinstance(distance, float)
+        # MyPy helpers
+        assert isinstance(distance, (int, float))
+        assert isinstance(hours, (float, int))
 
         # If the the equipment will arive after the shift is over, then it must travel
         # back to port (if needed), and wait for the next shift
         future_time = self.env.simulation_time + timedelta(hours=hours)
         is_shift = self._is_workshift(future_time.hour)
         if not is_shift and end != "port" and not self.at_port:
-            kw: dict[str, str] = {
-                "additional": "insufficient time to complete travel before end of the shift"
+            kw = {
+                "additional": "insufficient time to complete travel before end of the shift"  # noqa: disabl#501
             }
             kw.update(kwargs)
-            yield self.env.process(self.travel(start=start, end="port", **kw))  # type: ignore
+            yield self.env.process(
+                self.travel(start=start, end="port", **kw)  # type: ignore
+            )
             yield self.env.process(self.wait_until_next_shift(**kwargs))
             yield self.env.process(
                 self.travel(start=start, end=end, set_current=set_current, **kwargs)
             )
             return
         elif not is_shift and self.at_port:
             kw = {
-                "additional": "insufficient time to complete travel before end of the shift"
+                "additional": "insufficient time to complete travel before end of the shift"  # noqa: disabl#501
             }
             kw.update(kwargs)
             yield self.env.process(self.wait_until_next_shift(**kw))
             yield self.env.process(
                 self.travel(start=start, end=end, set_current=set_current, **kwargs)
             )
             return
 
         salary_cost = self.calculate_salary_cost(hours)
         hourly_cost = 0  # contractors not paid for traveling
         equipment_cost = self.calculate_equipment_cost(hours)
+        kwargs.update({"additional": additional})
         self.env.log_action(
             action="traveling",
-            additional=additional,
             duration=hours,
             distance_km=distance,
             salary_labor_cost=salary_cost,
             hourly_labor_cost=hourly_cost,
             equipment_cost=equipment_cost,
             location="enroute",
             **kwargs,
         )
+
+        # Unregister current_system during travel <- partial fix, still need to figure
+        # out where current_system needs to be set to None to allow things to "work"
+        self._set_location("site")
+
         yield self.env.timeout(hours)
 
         self._set_location(end, set_current)
+        where = set_current if set_current is not None else end
+        kwargs.update({"additional": f"arrived at {where}"})
         self.env.log_action(
             action="complete travel",
-            additional=f"arrived at {set_current if set_current is not None else end}",
             location=end,
             **kwargs,
         )
 
     def tow(
         self,
         start: str,
@@ -1064,25 +1100,25 @@
             additional="complete",
             location=end,
             **kwargs,
         )
 
     def crew_transfer(
         self,
-        system: System,
+        system: System | Cable,
         subassembly: Subassembly,
         request: RepairRequest,
         to_system: bool,
-    ) -> None | Generator[Timeout | Process, None, None]:
+    ) -> Generator[Timeout | Process, None, None]:
         """The process of transfering the crew from the equipment to the ``System``
         for servicing using an uninterrupted weather window to ensure safe transfer.
 
         Parameters
         ----------
-        system : System
+        system : System | Cable
             The System where the crew needs to be transferred to.
         subassembly : Subassembly
             The Subassembly that is being worked on.
         request : RepairRequest
             The repair to be processed.
         to_system : bool
             True if the crew is being transferred to the system, or False if the crew
@@ -1101,28 +1137,29 @@
             window can be found.
         """
         hours_to_process = self.settings.crew_transfer_time
         salary_cost = self.calculate_salary_cost(hours_to_process)
         hourly_cost = self.calculate_hourly_cost(hours_to_process)
         equipment_cost = self.calculate_equipment_cost(hours_to_process)
 
-        shared_logging = dict(
-            system_id=system.id,
-            system_name=system.name,
-            part_id=subassembly.id,
-            part_name=subassembly.name,
-            system_ol=system.operating_level,
-            part_ol=subassembly.operating_level,
-            agent=self.settings.name,
-            reason=request.details.description,
-            request_id=request.request_id,
-        )
+        shared_logging = {
+            "system_id": system.id,
+            "system_name": system.name,
+            "part_id": subassembly.id,
+            "part_name": subassembly.name,
+            "system_ol": system.operating_level,
+            "part_ol": subassembly.operating_level,
+            "agent": self.settings.name,
+            "reason": request.details.description,
+            "request_id": request.request_id,
+        }
 
         delay, shift_delay = self.find_uninterrupted_weather_window(hours_to_process)
-        # If there is a shift delay, then travel to port, wait, and travel back, and finally try again.
+        # If there is a shift delay, then travel to port, wait, and travel back, and
+        # finally try again.
         if shift_delay:
             travel_time = self.env.now
             yield self.env.process(
                 self.travel(start="site", end="port", **shared_logging)
             )
             travel_time -= self.env.now  # will be negative value, but is flipped
             delay -= abs(travel_time)  # decrement the delay by the travel time
@@ -1141,22 +1178,20 @@
             )
             yield self.env.process(
                 self.travel(
                     start="port", end="site", set_current=system.id, **shared_logging
                 )
             )
             yield self.env.process(
-                self.crew_transfer(system, subassembly, request, to_system=to_system)  # type: ignore
+                self.crew_transfer(system, subassembly, request, to_system=to_system)
             )
             return
 
         yield self.env.process(
-            self.weather_delay(
-                delay, location="site" if to_system else "system", **shared_logging
-            )
+            self.weather_delay(delay, location="system", **shared_logging)
         )
 
         if to_system:
             additional = f"transferring crew from {self.settings.name} to {system.id}"
         else:
             additional = f"transferring crew from {system.id} to {self.settings.name}"
         self.env.log_action(
@@ -1168,43 +1203,39 @@
             equipment_cost=equipment_cost,
             location="system",
             **shared_logging,
         )
         self.transferring_crew = True
         yield self.env.timeout(hours_to_process)
         self.transferring_crew = False
-        if to_system:
-            self.current_system = system.id
-        else:
-            self.current_system = None
-            self.at_system = False
         self.env.log_action(
             action="complete transfer",
             additional="complete",
-            location="system" if to_system else "site",
+            location="system",
             **shared_logging,
         )
 
     def mooring_connection(
         self,
         system: System,
         request: RepairRequest,
         which: str,
-    ) -> None | Generator[Timeout | Process, None, None]:
+    ) -> Generator[Timeout | Process, None, None]:
         """The process of either umooring a floating turbine to prepare for towing it to
         port, or reconnecting it after its repairs have been completed.
 
         Parameters
         ----------
         system : System
             The System that needs unmooring/reconnecting.
         request : RepairRequest
             The repair to be processed.
         which : bool
-            "unmoor" for unmooring the turbine, "reconnect" for reconnecting the turbine.
+            "unmoor" for unmooring the turbine, "reconnect" for reconnecting the
+            turbine.
 
         Returns
         -------
         None
             None is returned when this is run recursively to not repeat the process.
 
         Yields
@@ -1224,22 +1255,22 @@
                 f"Only `unmoor` and `reconnect` are allowable inputs, not {which}"
             )
 
         salary_cost = self.calculate_salary_cost(hours_to_process)
         hourly_cost = self.calculate_hourly_cost(hours_to_process)
         equipment_cost = self.calculate_equipment_cost(hours_to_process)
 
-        shared_logging = dict(
-            system_id=system.id,
-            system_name=system.name,
-            system_ol=system.operating_level,
-            agent=self.settings.name,
-            reason=request.details.description,
-            request_id=request.request_id,
-        )
+        shared_logging = {
+            "system_id": system.id,
+            "system_name": system.name,
+            "system_ol": system.operating_level,
+            "agent": self.settings.name,
+            "reason": request.details.description,
+            "request_id": request.request_id,
+        }
 
         which_text = "unmooring" if which == "unmoor" else "mooring reconnection"
 
         delay, shift_delay = self.find_uninterrupted_weather_window(hours_to_process)
         # If there is a shift delay, then wait try again.
         if shift_delay:
             yield self.env.process(
@@ -1271,25 +1302,27 @@
         self.env.log_action(
             action=which_text,
             additional=additional,
             duration=hours_to_process,
             salary_labor_cost=salary_cost,
             hourly_labor_cost=hourly_cost,
             equipment_cost=equipment_cost,
-            location="site",
+            location="system",
             **shared_logging,  # type: ignore
         )
 
         if which == "unmoor":
             yield self.env.timeout(self.settings.unmoor_hours)
         else:
             yield self.env.timeout(self.settings.reconnection_hours)
 
         self.env.log_action(
-            action=f"complete {which_text}", additional="complete", **shared_logging  # type: ignore
+            action=f"complete {which_text}",
+            additional="complete",
+            **shared_logging,  # type: ignore
         )
 
     def in_situ_repair(
         self,
         request: RepairRequest,
         time_processed: int | float = 0,
         prior_operation_level: float = -1.0,
@@ -1303,19 +1336,18 @@
         time_processed : int | float, optional
             Time that has already been processed, by default 0.
         prior_operation_level : float, optional
             The operating level of the ``System`` just before the repair has begun, by
             default -1.0.
 
         Yields
-        -------
+        ------
         Generator[Timeout | Process, None, None]
             Timeouts for the repair process.
         """
-
         """
         NOTE: THE PROCESS
         1. Travel to site/turbine, if not there already
         2. Transfer Crew
         3. Number of hours required, or hours until the end of the shift
         4. Do repairs for the above
         5. When shift/repair is complete, transfer crew
@@ -1333,25 +1365,25 @@
         else:
             system = self.windfarm.system(request.system_id)  # type: ignore
             subassembly = getattr(system, request.subassembly_id)
 
         starting_operational_level = max(
             prior_operation_level, subassembly.operating_level
         )
-        shared_logging = dict(
-            system_id=system.id,
-            system_name=system.name,
-            part_id=subassembly.id,
-            part_name=subassembly.name,
-            system_ol=system.operating_level,
-            part_ol=subassembly.operating_level,
-            agent=self.settings.name,
-            reason=request.details.description,
-            request_id=request.request_id,
-        )
+        shared_logging = {
+            "system_id": system.id,
+            "system_name": system.name,
+            "part_id": subassembly.id,
+            "part_name": subassembly.name,
+            "system_ol": system.operating_level,
+            "part_ol": subassembly.operating_level,
+            "agent": self.settings.name,
+            "reason": request.details.description,
+            "request_id": request.request_id,
+        }
 
         # Ensure there is enough time to transfer the crew back and forth with a buffer
         # of twice the travel time or travel back to port and try again the next shift
         start_shift = self.settings.workday_start
         end_shift = self.settings.workday_end
         current = self.env.simulation_time
         hours_required = request.details.time - time_processed
@@ -1377,36 +1409,28 @@
         # Travel to site or the next system on site
         if not self.at_system and self.at_port:
             yield self.env.process(
                 self.travel(
                     start="port", end="site", set_current=system.id, **shared_logging
                 )
             )
-            # First turn off the turbine, then proceed with the servicing so the
-            # turbine is not registered as operating when the turbine is being worked on
-            if system.servicing.triggered:
-                self.manager.halt_requests_for_system(system)
             yield self.env.process(
-                self.crew_transfer(system, subassembly, request, to_system=True)  # type: ignore
+                self.crew_transfer(system, subassembly, request, to_system=True)
             )
         elif self.at_system is not None and not self.at_port:
             yield self.env.process(
                 self.travel(
                     start="system",
                     end="system",
                     set_current=system.id,
                     **shared_logging,
                 )
             )
-            # First turn off the turbine, then proceed with the servicing so the
-            # turbine is not registered as operating when the turbine is being worked on
-            if system.servicing.triggered:
-                self.manager.halt_requests_for_system(system)
             yield self.env.process(
-                self.crew_transfer(system, subassembly, request, to_system=True)  # type: ignore
+                self.crew_transfer(system, subassembly, request, to_system=True)
             )
         else:
             raise RuntimeError(f"{self.settings.name} is lost!")
 
         current = self.env.simulation_time
 
         # If the hours required is longer than the shift time, then reset the available
@@ -1478,15 +1502,15 @@
                     )
                 )
                 hours_available -= hours_to_process
 
         # Reached the end of the shift or the end of the repair, and need to unload crew
         # from the system
         yield self.env.process(
-            self.crew_transfer(system, subassembly, request, to_system=False)  # type: ignore
+            self.crew_transfer(system, subassembly, request, to_system=False)
         )
         if shift_delay:
             yield self.env.process(
                 self.travel(start="site", end="port", **shared_logging)
             )
             yield self.env.process(self.wait_until_next_shift(**shared_logging))
 
@@ -1513,56 +1537,56 @@
             part_ol=subassembly.operating_level,
             agent=self.settings.name,
             action=f"{action} complete",
             reason=request.details.description,
             materials_cost=request.details.materials,
             additional="complete",
             request_id=request.request_id,
-            location="site",
+            location="system",
         )
 
         # If this is the end of the shift, ensure that we're traveling back to port
         if not self.env.is_workshift(start_shift, end_shift):
             yield self.env.process(
                 self.travel(start="site", end="port", **shared_logging)
             )
 
     def run_scheduled_in_situ(self) -> Generator[Process, None, None]:
         """Runs the simulation of in situ repairs for scheduled servicing equipment
         that have the `onsite` designation or don't require mobilization.
 
         Yields
-        -------
+        ------
         Generator[Process, None, None]
             The simulation.
         """
         assert isinstance(self.settings, ScheduledServiceEquipmentData)  # mypy controls
 
-        # If the starting operation date is the same as the simulations, set to be onsite
+        # If the starting operation date is the same as the simulations, set to onsite
         if self.settings.operating_dates[0] == self.env.simulation_time.date():
-            self.onsite = True
+            yield self.env.process(self.mobilize_scheduled())
 
         while True:
             # Wait for a valid operational period to start
-            if self.env.simulation_time.date() not in self.settings.operating_dates_set:  # type: ignore
+            if self.env.simulation_time.date() not in self.settings.operating_dates_set:
                 yield self.env.process(self.mobilize_scheduled())
 
             # Wait for next shift to start
             is_workshift = self.env.is_workshift(
                 workday_start=self.settings.workday_start,
                 workday_end=self.settings.workday_end,
             )
             if not is_workshift:
                 yield self.env.process(
                     self.wait_until_next_shift(
-                        **dict(
-                            agent=self.settings.name,
-                            reason="not in working hours",
-                            additional="not in working hours",
-                        )
+                        **{
+                            "agent": self.settings.name,
+                            "reason": "not in working hours",
+                            "additional": "not in working hours",
+                        }
                     )
                 )
 
             request = self.get_next_request()
             if request is None:
                 if not self.at_port:
                     yield self.env.process(
@@ -1571,30 +1595,44 @@
                             end="port",
                             reason="no requests",
                             agent=self.settings.name,
                         )
                     )
                 yield self.env.process(
                     self.wait_until_next_shift(
-                        **dict(
-                            agent=self.settings.name,
-                            reason="no requests",
-                            additional="no work requests, waiting until the next shift",
-                        )
+                        **{
+                            "agent": self.settings.name,
+                            "reason": "no requests",
+                            "additional": "no work requests, waiting until the next shift",  # noqa: disabl#501
+                        }
                     )
                 )
             else:
-                yield self.env.process(self.in_situ_repair(request.value))
+                request = request.value
+                if request.cable:
+                    system = self.windfarm.cable(request.system_id)
+                else:
+                    system = self.windfarm.system(request.system_id)  # type: ignore
+                yield system.servicing
+                self.manager.halt_requests_for_system(system)
+                yield self.env.process(self.in_situ_repair(request))
 
-    def run_unscheduled_in_situ(self) -> Generator[Process, None, None]:
+    def run_unscheduled_in_situ(
+        self, request: RepairRequest
+    ) -> Generator[Process, None, None]:
         """Runs an in situ repair simulation for unscheduled servicing equipment, or
         those that have to be mobilized before performing repairs and maintenance.
 
+        Parameters
+        ----------
+        request : RepairRequest
+            The repair request that triggered the repair process.
+
         Yields
-        -------
+        ------
         Generator[Process, None, None]
             The simulation
         """
         self.dispatched = True
         assert isinstance(self.settings, UnscheduledServiceEquipmentData)  # mypy helper
         mobilization_days = self.settings.mobilization_days
         charter_end_env_time = self.settings.charter_days * HOURS_IN_DAY
@@ -1624,62 +1662,91 @@
                 agent=self.settings.name,
                 action="delay",
                 reason="non-operational period",
                 additional="waiting for next operational period",
                 duration=hours_to_next,
             )
             yield self.env.timeout(hours_to_next)  # type: ignore
-            yield self.env.process(self.run_unscheduled_in_situ())
+            yield self.env.process(self.run_unscheduled_in_situ(request))
             return
 
+        # Ensure the system isn't in service already during the checking stages, then
+        # halt its ongoing processes for the current repair.
+        # NOTE: port-based equipment will have already halted the system's processes.
+        if not hasattr(self, "port"):
+            if request.cable:
+                system = self.windfarm.cable(request.system_id)
+            else:
+                system = self.windfarm.system(request.system_id)  # type: ignore
+            yield system.servicing
+            seconds_to_wait, *_ = (
+                random_generator.integers(low=0, high=30, size=1) / 3600.0
+            )
+            yield self.env.timeout(seconds_to_wait)
+            yield system.servicing
+            self.manager.halt_requests_for_system(system)
+
         while True:
             if self.env.now >= charter_end_env_time:
                 self.onsite = False
                 self.at_port = False
+                self.at_site = False
                 self.at_system = False
                 self.dispatched = False
                 self.current_system = None
                 self.env.log_action(
                     agent=self.settings.name,
                     action="leaving site",
                     reason="charter period has ended",
                 )
                 break
 
             if not self.onsite:
                 yield self.env.process(self.mobilize())
+                yield self.env.process(self.in_situ_repair(request))
 
             # Wait for next shift to start
             is_workshift = self.env.is_workshift(
                 workday_start=self.settings.workday_start,
                 workday_end=self.settings.workday_end,
             )
             if not is_workshift:
                 yield self.env.process(
                     self.wait_until_next_shift(
-                        **dict(
-                            agent=self.settings.name,
-                            reason="not in working hours",
-                            additional="not in working hours",
-                        )
+                        **{
+                            "agent": self.settings.name,
+                            "reason": "not in working hours",
+                            "additional": "not in working hours",
+                        }
                     )
                 )
+
+            # Wait one second to ensure there are no timing collisions
+            yield self.env.timeout(1.0 / 3600)
             request = self.get_next_request()
             if request is None:
                 yield self.env.process(
                     self.wait_until_next_shift(
-                        **dict(
-                            agent=self.settings.name,
-                            reason="no requests",
-                            additional="no work requests submitted by start of shift",
-                        )
+                        **{
+                            "agent": self.settings.name,
+                            "reason": "no requests",
+                            "additional": "no work requests submitted by start of shift",  # noqa: disabl#501
+                        }
                     )
                 )
             else:
-                yield self.env.process(self.in_situ_repair(request.value))
+                request = request.value  # type: ignore
+                if request.cable:
+                    system = self.windfarm.cable(request.system_id)
+                else:
+                    system = self.windfarm.system(request.system_id)  # type: ignore
+                yield system.servicing
+                self.manager.halt_requests_for_system(system)
+                yield self.env.process(self.in_situ_repair(request))
+        self.dispatched = False
 
     def run_tow_to_port(self, request: RepairRequest) -> Generator[Process, None, None]:
         """Runs the tow to port logic, so a turbine can be repaired at port.
 
         Parameters
         ----------
         request : RepairRequest
@@ -1691,33 +1758,41 @@
             The series of events that simulate the complete towing logic.
 
         Raises
         ------
         ValueError
             Raised if the equipment is not currently at port
         """
+        self.dispatched = True
         system = self.windfarm.system(request.system_id)
 
-        shared_logging = dict(
-            system_id=request.system_id,
-            system_name=request.system_name,
-            request_id=request.request_id,
-            agent=self.settings.name,
-        )
+        shared_logging = {
+            "system_id": request.system_id,
+            "system_name": request.system_name,
+            "request_id": request.request_id,
+            "agent": self.settings.name,
+        }
 
         # Travel to the turbine
         yield self.env.process(
-            self.travel("port", "site", set_current=system.id, reason=request.details.description, **shared_logging)  # type: ignore
+            self.travel(
+                "port",
+                "site",
+                set_current=system.id,
+                reason=request.details.description,
+                **shared_logging,  # type: ignore
+            )
         )
 
         # Unmoor the turbine and tow it back to port
-        yield self.env.process(self.mooring_connection(system, request, which="unmoor"))  # type: ignore
+        yield self.env.process(self.mooring_connection(system, request, which="unmoor"))
         yield self.env.process(
             self.tow("site", "port", reason="towing turbine to port", **shared_logging)
         )
+        self.dispatched = False
 
     def run_tow_to_site(self, request: RepairRequest) -> Generator[Process, None, None]:
         """Runs the tow to site logic for after a turbine has had its repairs completed
         at port.
 
         Parameters
         ----------
@@ -1730,23 +1805,24 @@
             The series of events that simulate the complete towing logic.
 
         Raises
         ------
         ValueError
             Raised if the equipment is not currently at port
         """
+        self.dispatched = True
         system = self.windfarm.system(request.system_id)
-        shared_logging = dict(
-            agent=self.settings.name,
-            request_id=request.request_id,
-            system_id=request.system_id,
-            system_name=request.system_name,
-        )
+        shared_logging = {
+            "agent": self.settings.name,
+            "request_id": request.request_id,
+            "system_id": request.system_id,
+            "system_name": request.system_name,
+        }
 
-        # Tow the turbine back to site and reconnect it to the mooring and electrical systems
+        # Tow the turbine back to site and reconnect it to the mooring system
         yield self.env.process(
             self.tow(
                 "port",
                 "site",
                 set_current=system.id,
                 reason="towing turbine back to site",
                 **shared_logging,
@@ -1754,32 +1830,17 @@
         )
         yield self.env.process(
             self.mooring_connection(system, request, which="reconnect")  # type: ignore
         )
 
         # Reset the turbine back to operating and return to port
         reset_system_operations(system)
-        self.manager.enable_requests_for_system(system.id)
+        self.manager.enable_requests_for_system(system)
         yield self.env.process(
             self.travel(
                 "site",
                 "port",
                 reason="traveling back to port after returning turbine",
                 **shared_logging,  # type: ignore
             )
         )
-
-    def run_unscheduled(self, request: RepairRequest):
-        """Runs the appropriate repair logic for unscheduled servicing equipment, or
-        those that can be immediately dispatched.
-
-        Parameters
-        ----------
-        request : RepairRequest
-            The request that trigged the repair logic.
-        """
-        if "TOW" in request.details.service_equipment:
-            yield self.env.process(self.port.run_tow_to_port(request))
-        elif "AHV" in request.details.service_equipment:
-            yield self.env.process(self.port.run_unscheduled_in_situ(request))
-        else:
-            yield self.env.process(self.run_unscheduled_in_situ())
+        self.dispatched = False
```

### Comparing `wombat-0.6.2/wombat/core/simulation_api.py` & `wombat-0.7.0/wombat/core/simulation_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """The main API for the ``wombat``."""
 from __future__ import annotations
 
 import logging
 import datetime
-from typing import Optional
 from pathlib import Path
 
 import yaml
 import pandas as pd
 from attrs import Attribute, field, define
 from simpy.events import Event
 
@@ -40,22 +39,24 @@
         The library path.
     """
     return Path(library_map.get(file_path, file_path)).resolve()  # type: ignore
 
 
 @define(frozen=True, auto_attribs=True)
 class Configuration(FromDictMixin):
-    """The ``Simulation`` configuration data class that provides all the necessary definitions.
+    """The ``Simulation`` configuration data class that provides all the necessary
+    definitions.
 
     Parameters
     ----------
     name: str
         Name of the simulation. Used for logging files.
     library : str
-        The data directory. See ``wombat.simulation.WombatEnvironment`` for more details.
+        The data directory. See ``wombat.simulation.WombatEnvironment`` for more
+        details.
     layout : str
         The windfarm layout file. See ``wombat.Windfarm`` for more details.
     service_equipment : str | list[str]
         The equpiment that will be used in the simulation. See
         ``wombat.core.ServiceEquipment`` for more details.
     weather : str
         The weather profile to be used. See ``wombat.simulation.WombatEnvironment``
@@ -159,58 +160,61 @@
     windfarm: Windfarm = field(init=False)
     env: WombatEnvironment = field(init=False)
     repair_manager: RepairManager = field(init=False)
     service_equipment: list[ServiceEquipment] = field(init=False)
     port: Port = field(init=False)
 
     def __attrs_post_init__(self) -> None:
+        """Post-initialization hook."""
         self._setup_simulation()
 
     @config.validator  # type: ignore
     def _create_configuration(
         self, attribute: Attribute, value: str | Path | dict | Configuration
     ) -> None:
         """Validates the configuration object and creates the ``Configuration`` object
-        for the simulation.Raises:
+        for the simulation.
 
         Raises
         ------
         TypeError
             Raised if the value provided is not able to create a valid ``Configuration``
             object
         ValueError
-            Raised if ``name`` and ``config.name`` or ``library_path`` and ``config.library``
-            are not aligned.
+            Raised if ``name`` and ``config.name`` or ``library_path`` and
+            ``config.library`` are not aligned.
 
         Returns
         -------
         Configuration
             The validated simulation configuration
         """
         if isinstance(value, (str, Path)):
             try:
                 value = load_yaml(self.library_path / "project/config", value)
             except FileNotFoundError:
                 value = load_yaml(self.library_path / "config", value)  # type: ignore
                 logging.warning(
-                    "DeprecationWarning: In v0.7, all project configurations must be located in: '<library>/project/config/"
+                    "DeprecationWarning: In v0.8, all project configurations must be"
+                    " located in: '<library>/project/config/"
                 )
         if isinstance(value, dict):
             value = Configuration.from_dict(value)
         if isinstance(value, Configuration):
             object.__setattr__(self, attribute.name, value)
         else:
             raise TypeError(
                 "``config`` must be a dictionary, valid file path to a yaml-enocoded",
                 "dictionary, or ``Configuration`` object!",
             )
 
         if self.config.library != self.library_path:
             raise ValueError(
-                "``library_path`` and the library in ``config`` do not match!"
+                f"`library_path`: {self.library_path} and the library in `config`:"
+                f" {self.config.library} do not match!"
             )
 
     @classmethod
     def from_config(cls, config: str | Path | dict | Configuration):
         """Creates the ``Simulation`` object only the configuration contents as either a
         full file path to the configuration file, a dictionary of the configuration
         contents, or pre-loaded ``Configuration`` object.
@@ -224,16 +228,15 @@
             - ``str`` : the full file path of the configuration yaml file.
             - ``dict`` : a dictionary with the requried configuration settings.
             - ``Configuration`` : a pre-created ``Configuration`` object.
 
         Raises
         ------
         TypeError
-            If ``config`` is not one of the three acceptable input types, then an error is
-            raised.
+            Raised if ``config`` is not one of the three acceptable input types.
 
         Returns
         -------
         Simulation
             A ready-to-run ``Simulation`` object.
         """
         if isinstance(config, (str, Path)):
@@ -280,40 +283,41 @@
             self.service_equipment.append(equipment)
 
         # Create the port and add any tugboats to the available servicing equipment list
         if self.config.port is not None:
             self.port = Port(
                 self.env, self.windfarm, self.repair_manager, self.config.port
             )
-            self.service_equipment.extend(self.port.tugboat_manager.items)
+            self.service_equipment.extend(self.port.service_equipment_manager.items)
 
         if self.config.project_capacity * 1000 != round(self.windfarm.capacity, 6):
             raise ValueError(
                 f"Input `project_capacity`: {self.config.project_capacity:,.6f} MW is"
                 f" not equal to the sum of turbine capacities:"
                 f" {self.windfarm.capacity / 1000:,.6f} MW"
             )
 
     def run(
         self,
-        until: Optional[int | float | Event] = None,
+        until: int | float | Event | None = None,
         create_metrics: bool = True,
         save_metrics_inputs: bool = True,
     ):
-        """Calls ``WombatEnvironment.run()`` and gathers the results for post-processing.
-        See ``wombat.simulation.WombatEnvironment.run`` or ``simpy.Environment.run`` for more
-        details.
+        """Calls ``WombatEnvironment.run()`` and gathers the results for
+        post-processing. See ``wombat.simulation.WombatEnvironment.run`` or
+        ``simpy.Environment.run`` for more details.
 
         Parameters
         ----------
         until : Optional[int | float | Event], optional
             When to stop the simulation, by default None. See documentation on
             ``simpy.Environment.run`` for more details.
         create_metrics : bool, optional
-            If True, the metrics object will be created, and not, if False, by default True.
+            If True, the metrics object will be created, and not, if False, by default
+            True.
         save_metrics_inputs : bool, optional
             If True, the metrics inputs data will be saved to a yaml file, with file
             references to any larger data structures that can be reloaded later. If
             False, the data will not be saved, by default True.
         """
         self.env.run(until=until)
         if save_metrics_inputs:
@@ -344,40 +348,42 @@
             inflation_rate=self.config.inflation_rate,
             project_capacity=self.config.project_capacity,
             turbine_capacities=capacities,
             fixed_costs=self.config.fixed_costs,  # type: ignore
             substation_id=self.windfarm.substation_id.tolist(),
             turbine_id=self.windfarm.turbine_id.tolist(),
             substation_turbine_map=substation_turbine_map,
-            service_equipment_names=[el.settings.name for el in self.service_equipment],  # type: ignore
+            service_equipment_names=[el.settings.name for el in self.service_equipment],
             SAM_settings=self.config.SAM_settings,
         )
 
     def save_metrics_inputs(self) -> None:
         """Saves the inputs for the `Metrics` initialization with either a direct
         copy of the data or a file reference that can be loaded later.
         """
         substation_turbine_map = {
             s_id: {k: v.tolist() for k, v in dict.items()}
             for s_id, dict in self.windfarm.substation_turbine_map.items()
         }
-        data = dict(
-            data_dir=str(self.config.library),
-            events=str(self.env.events_log_fname.with_suffix(".csv")),
-            operations=str(self.env.operations_log_fname.with_suffix(".csv")),
-            potential=str(self.env.power_potential_fname),
-            production=str(self.env.power_production_fname),
-            inflation_rate=self.config.inflation_rate,
-            project_capacity=self.config.project_capacity,
-            turbine_capacities=[
+        data = {
+            "data_dir": str(self.config.library),
+            "events": str(self.env.events_log_fname.with_suffix(".csv")),
+            "operations": str(self.env.operations_log_fname.with_suffix(".csv")),
+            "potential": str(self.env.power_potential_fname),
+            "production": str(self.env.power_production_fname),
+            "inflation_rate": self.config.inflation_rate,
+            "project_capacity": self.config.project_capacity,
+            "turbine_capacities": [
                 self.windfarm.system(t_id).capacity for t_id in self.windfarm.turbine_id
             ],
-            fixed_costs=self.config.fixed_costs,
-            substation_id=self.windfarm.substation_id.tolist(),
-            turbine_id=self.windfarm.turbine_id.tolist(),
-            substation_turbine_map=substation_turbine_map,
-            service_equipment_names=[el.settings.name for el in self.service_equipment],  # type: ignore
-            SAM_settings=self.config.SAM_settings,
-        )
+            "fixed_costs": self.config.fixed_costs,
+            "substation_id": self.windfarm.substation_id.tolist(),
+            "turbine_id": self.windfarm.turbine_id.tolist(),
+            "substation_turbine_map": substation_turbine_map,
+            "service_equipment_names": [
+                el.settings.name for el in self.service_equipment
+            ],
+            "SAM_settings": self.config.SAM_settings,
+        }
 
         with open(self.env.metrics_input_fname, "w") as f:
             yaml.dump(data, f, default_flow_style=False, sort_keys=False)
```

### Comparing `wombat-0.6.2/wombat/utilities/logging.py` & `wombat-0.7.0/wombat/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `wombat-0.6.2/wombat/utilities/time.py` & `wombat-0.7.0/wombat/utilities/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         return value
 
     # Ensure there is a common comparison year for all datetime values
     return parse(value).replace(year=2022)
 
 
 def convert_dt_to_hours(diff: datetime.timedelta) -> float:
-    """Converts a ``datetime.timedelta`` object to number of hours at the seconds resolution.
+    """Convert a ``datetime.timedelta`` object to number of hours at the seconds
+    resolution.
 
     Parameters
     ----------
     diff : datetime.timedelta
         The difference between two ``datetime.datetime`` objects.
 
     Returns
@@ -51,16 +52,16 @@
     """
     days = diff.days * 24 if diff.days > 0 else 0
     seconds = diff.seconds / 60 / 60
     return days + seconds
 
 
 def hours_until_future_hour(dt: datetime.datetime, hour: int) -> float:
-    """Number of hours until a future hour in the same day for ``hour`` <= 24, otherwise,
-    it is the number of hours until a time in the proceeding days.
+    """Number of hours until a future hour in the same day for ``hour`` <= 24,
+    otherwise, it is the number of hours until a time in the proceeding days.
 
     Parameters
     ----------
     dt : datetime.datetime
         Focal datetime.
     hour : int
         Hour that is later in the day, in 24 hour time.
@@ -101,29 +102,31 @@
         The starting hour to be checked.
     workday_end : int
         The ending hour to be checked.
 
     Returns
     -------
     tuple[int, int]
-        The starting and ending hour to be applied back to the port or servicing equipment.
+        The starting and ending hour to be applied back to the port or servicing
+        equipment.
     """
     start_is_invalid = workday_start == -1
     end_is_invalid = workday_end == -1
 
     start = env_start if start_is_invalid else workday_start
     end = env_end if end_is_invalid else workday_end
 
     return start, end
 
 
 def calculate_cost(
     duration: int | float, rate: float, n_rate: int = 1, daily_rate: bool = False
 ) -> float:
-    """Calculates the equipment cost, or labor cost for either salaried or hourly employees.
+    """Calculates the equipment cost, or labor cost for either salaried or hourly
+    employees.
 
     Parameters
     ----------
     duration : int | float
         Length of time, in hours.
     rate : float
         The labor or equipment rate, in $USD/hour.
```

### Comparing `wombat-0.6.2/wombat/utilities/utilities.py` & `wombat-0.7.0/wombat/utilities/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,58 +68,62 @@
 def IEC_power_curve(
     windspeed_column: np.ndarray | pd.Series,
     power_column: np.ndarray | pd.Series,
     bin_width: float = 0.5,
     windspeed_start: float = 0.0,
     windspeed_end: float = 30.0,
 ) -> Callable:
-    """
-    Direct copyfrom OpenOA: https://github.com/NREL/OpenOA/blob/main/operational_analysis/toolkits/power_curve/functions.py#L16-L57
+    """Direct copyfrom OpenOA:
+    https://github.com/NREL/OpenOA/blob/main/operational_analysis/toolkits/power_curve/functions.py#L16-L57
     Use IEC 61400-12-1-2 method for creating wind-speed binned power curve.
 
     Parameters
     ----------
         windspeed_column : np.ndarray | pandas.Series
             The power curve's windspeed values, in m/s.
         power_column : np.ndarray | pandas.Series
             The power curve's output power values, in kW.
         bin_width : float
-            Width of windspeed bin, default is 0.5 m/s according to standard, by default 0.5.
+            Width of windspeed bin, default is 0.5 m/s according to standard, by default
+            0.5.
         windspeed_start : float
-            Left edge of first windspeed bin, where all proceeding values will be 0.0, by default 0.0.
+            Left edge of first windspeed bin, where all proceeding values will be 0.0,
+            by default 0.0.
         windspeed_end : float
             Right edge of last windspeed bin, where all following values will be 0.0, by
             default 30.0.
-    Returns:
+
+    Returns
+    -------
         Callable
             Python function of the power curve, of type (Array[float] -> Array[float]),
             that maps input windspeed value(s) to ouptut power value(s).
     """
-
     if not isinstance(windspeed_column, pd.Series):
         windspeed_column = pd.Series(windspeed_column)
     if not isinstance(power_column, pd.Series):
         power_column = pd.Series(power_column)
 
-    # Set up evenly spaced bins of fixed width, with any value over the maximum getting np.inf
+    # Set up evenly spaced bins of fixed width, with np.inf for any value over the max
     n_bins = int(np.ceil((windspeed_end - windspeed_start) / bin_width)) + 1
     bins = np.append(np.linspace(windspeed_start, windspeed_end, n_bins), [np.inf])
 
     # Initialize an array which will hold the mean values of each bin
     P_bin = np.ones(len(bins) - 1) * np.nan
 
     # Compute the mean of each bin and set corresponding P_bin
     for ibin in range(0, len(bins) - 1):
         indices = (windspeed_column >= bins[ibin]) & (windspeed_column < bins[ibin + 1])
         P_bin[ibin] = power_column.loc[indices].mean()
 
     # Linearly interpolate any missing bins
     P_bin = pd.Series(data=P_bin).interpolate(method="linear").bfill().values
 
-    # Create a closure over the computed bins which computes the power curve value for arbitrary array-like input
+    # Create a closure over the computed bins which computes the power curve value for
+    # arbitrary array-like input
     def pc_iec(x):
         P = np.zeros(np.shape(x))
         for i in range(0, len(bins) - 1):
             idx = np.where((x >= bins[i]) & (x < bins[i + 1]))
             P[idx] = P_bin[i]
         cutoff_idx = (x < windspeed_start) | (x > windspeed_end)
         P[cutoff_idx] = 0.0
```

### Comparing `wombat-0.6.2/wombat/windfarm/system/cable.py` & `wombat-0.7.0/wombat/windfarm/system/cable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """"Defines the Cable class and cable simulations."""
 from __future__ import annotations
 
 from typing import Generator
+from itertools import zip_longest
 
 import numpy as np
 import simpy
 
 from wombat.core import (
     Failure,
     Maintenance,
@@ -53,34 +54,36 @@
         env : WombatEnvironment
             The simulation environment.
         connection_type : str
             One of "export" or "array".
         cable_id : str
             The unique identifier for the cable.
         start_node : str
-            The starting point (``system.id``) (turbine or substation) of the cable segment.
+            The starting point (``system.id``) (turbine or substation) of the cable
+            segment.
         end_node : str
-            The ending point (``system.id``) (turbine or substation) of the cable segment.
+            The ending point (``system.id``) (turbine or substation) of the cable
+            segment.
         cable_data : dict
             The dictionary defining the cable segment.
         name : str | None
             The name of the cable to use during logging.
         """
-
         self.env = env
         self.windfarm = windfarm
         self.connection_type = connection_type
         self.start_node = start_node
         self.end_node = end_node
         self.id = f"cable::{start_node}::{end_node}"
         self.system = windfarm.system(start_node)
 
         if self.connection_type not in ("array", "export"):
             raise ValueError(
-                f"Input to `connection_type` for {self.id} must be one of 'array' or 'export'."
+                f"Input to `connection_type` for {self.id} must be one of 'array'"
+                " or 'export'."
             )
 
         cable_data = {**cable_data, "system_value": self.system.value}
         self.data = SubassemblyData.from_dict(cable_data)
         self.name = self.data.name if name is None else name
 
         self.operating_level = 1.0
@@ -111,20 +114,18 @@
         self.substation = substation
 
     def finish_setup(self) -> None:
         """Creates the ``upstream_nodes`` and ``upstream_cables`` attributes for use by
         the cable when triggering usptream failures and resetting them after the repair
         is complete.
         """
-
         wf_map = self.windfarm.wind_farm_map
         if self.connection_type == "array":
-            turbines = []
+            turbines = [self.end_node]
             if self.end_node == self.string_start:
-                turbines.append(self.end_node)
                 _turbines, cables = wf_map.get_upstream_connections(
                     self.substation, self.string_start, self.string_start
                 )
             else:
                 _turbines, cables = wf_map.get_upstream_connections(
                     self.substation, self.string_start, self.end_node
                 )
@@ -138,15 +139,15 @@
         self.upstream_nodes = turbines
         self.upstream_cables = cables
 
     def _create_processes(self):
         """Creates the processes for each of the failure and maintenance types.
 
         Yields
-        -------
+        ------
         Tuple[Union[str, int], simpy.events.Process]
             Creates a dictionary to keep track of the running processes within the
             subassembly.
         """
         for level, failure in self.data.failures.items():
             yield level, self.env.process(self.run_single_failure(failure))
 
@@ -166,68 +167,73 @@
             try:
                 process.interrupt()
             except RuntimeError:
                 # This error occurs for the process halting all other processes.
                 pass
 
     def interrupt_all_subassembly_processes(self) -> None:
-        """Thin wrapper for ``interrupt_processes`` to keep usage the same as systems."""
+        """Thin wrapper for ``interrupt_processes`` for consistent usage with system."""
         self.interrupt_processes()
 
     def stop_all_upstream_processes(self, failure: Failure | Maintenance) -> None:
         """Stops all upstream turbines and cables from producing power by creating a
         ``env.event()`` for each ``System.cable_failure`` and
         ``Cable.downstream_failure``, respectively. In the case of an export cable, each
         string is traversed to stop the substation and upstream turbines and cables.
 
         Parameters
         ----------
         failure : Failre
             The ``Failure`` that is causing a string shutdown.
         """
-        shared_logging = dict(
-            agent=self.id,
-            action="repair_request",
-            reason=failure.description,
-            additional="downstream cable failure",
-            request_id=failure.request_id,
-        )
+        shared_logging = {
+            "agent": self.id,
+            "action": "repair request",
+            "reason": failure.description,
+            "additional": "downstream cable failure",
+            "request_id": failure.request_id,
+        }
         upstream_nodes = self.upstream_nodes
         upstream_cables = self.upstream_cables
         if self.connection_type == "export":
             # Flatten the list of lists for shutting down the upstream connections
             upstream_nodes = [el for string in upstream_nodes for el in string]
             upstream_cables = [el for string in upstream_cables for el in string]
 
             # Turn off the subation
             substation = self.windfarm.system(self.end_node)
-            substation.interrupt_all_subassembly_processes()
             substation.cable_failure = self.env.event()
+            substation.interrupt_all_subassembly_processes()
             self.env.log_action(
                 system_id=self.end_node,
                 system_name=substation.name,
                 system_ol=substation.operating_level,
                 part_ol=np.nan,
                 **shared_logging,  # type: ignore
             )
 
-        for t_id, c_id in zip(upstream_nodes, upstream_cables):
+        for t_id, c_id in zip_longest(upstream_nodes, upstream_cables, fillvalue=None):
+            assert isinstance(t_id, str)
             turbine = self.windfarm.system(t_id)
             turbine.cable_failure = self.env.event()
             turbine.interrupt_all_subassembly_processes()
             self.env.log_action(
                 system_id=t_id,
                 system_name=turbine.name,
                 system_ol=turbine.operating_level,
                 part_ol=np.nan,
                 **shared_logging,  # type: ignore
             )
+
+            # If at the end of the string, skip any operations on non-existent cables
+            if c_id is None:
+                continue
             cable = self.windfarm.cable(c_id)
-            cable.interrupt_processes()
             cable.downstream_failure = self.env.event()
+            cable.interrupt_all_subassembly_processes()
             self.env.log_action(
                 system_id=c_id,
                 system_name=cable.name,
                 part_id=c_id,
                 part_name=cable.name,
                 system_ol=np.nan,
                 part_ol=cable.operating_level,
@@ -245,20 +251,20 @@
         """
         which = "maintenance" if isinstance(action, Maintenance) else "repair"
         self.operating_level *= 1 - action.operation_reduction
 
         # Automatically submit a repair request
         # NOTE: mypy is not caught up with attrs yet :(
         repair_request = RepairRequest(  # type: ignore
-            self.id,
-            self.name,
-            self.id,
-            self.name,
-            action.level,
-            action,
+            system_id=self.id,
+            system_name=self.name,
+            subassembly_id=self.id,
+            subassembly_name=self.name,
+            severity_level=action.level,
+            details=action,
             cable=True,
             upstream_turbines=self.upstream_nodes,
             upstream_cables=self.upstream_cables,
         )
         repair_request = self.system.repair_manager.register_request(repair_request)
         self.env.log_action(
             system_id=self.id,
@@ -272,95 +278,100 @@
             reason=action.description,
             additional=f"severity level {action.level}",
             request_id=repair_request.request_id,
         )
 
         if action.operation_reduction == 1:
             self.broken = self.env.event()
-            self.interrupt_processes()
+            self.interrupt_all_subassembly_processes()
             self.stop_all_upstream_processes(action)
 
         # Remove previously submitted requests as a replacement is required
         if action.replacement:
             _ = self.system.repair_manager.purge_subassembly_requests(
                 self.id, self.id, exclude=[repair_request.request_id]
             )
-
         self.system.repair_manager.submit_request(repair_request)
 
     def run_single_maintenance(self, maintenance: Maintenance) -> Generator:
-        """Runs a process to trigger one type of maintenance request throughout the simulation.
+        """Runs a process to trigger one type of maintenance request throughout the
+        simulation.
 
         Parameters
         ----------
         maintenance : Maintenance
             A maintenance category.
 
         Yields
-        -------
+        ------
         simpy.events.Timeout
             Time between maintenance requests.
         """
         while True:
             hours_to_next = maintenance.frequency
             if hours_to_next == 0:
                 remainder = self.env.max_run_time - self.env.now
                 try:
                     yield self.env.timeout(remainder)
                 except simpy.Interrupt:
                     remainder -= self.env.now
 
             while hours_to_next > 0:
+                start = -1  # Ensure an interruption before processing is caught
                 try:
-                    # If the replacement has not been completed, then wait another minute
+                    # If the replacement has not been completed, then wait
                     yield self.servicing & self.downstream_failure & self.broken
 
                     start = self.env.now
                     yield self.env.timeout(hours_to_next)
                     hours_to_next = 0
                     self.trigger_request(maintenance)
                 except simpy.Interrupt:
                     if not self.broken.triggered:
                         # The subassembly had to restart the maintenance cycle
                         hours_to_next = 0
                     else:
-                        # A different interruption occurred, so subtract the elapsed time
-                        hours_to_next -= self.env.now - start  # pylint: disable=E0601
+                        # A different process failed, so subtract the elapsed time
+                        # only if it had started to be processed
+                        hours_to_next -= 0 if start == -1 else self.env.now - start
 
     def run_single_failure(self, failure: Failure) -> Generator:
-        """Runs a process to trigger one type of failure repair request throughout the simulation.
+        """Runs a process to trigger one type of failure repair request throughout the
+        simulation.
 
         Parameters
         ----------
         failure : Failure
             A failure classification.
 
         Yields
-        -------
+        ------
         simpy.events.Timeout
             Time between failure events that need to request a repair.
         """
         while True:
             hours_to_next = failure.hours_to_next_failure()
             if hours_to_next is None:
                 remainder = self.env.max_run_time - self.env.now
                 try:
                     yield self.env.timeout(remainder)
                 except simpy.Interrupt:
                     remainder -= self.env.now
 
             assert isinstance(hours_to_next, (int, float))  # mypy helper
             while hours_to_next > 0:  # type: ignore
+                start = -1  # Ensure an interruption before processing is caught
                 try:
                     yield self.servicing & self.downstream_failure & self.broken
 
                     start = self.env.now
                     yield self.env.timeout(hours_to_next)
                     hours_to_next = 0
                     self.trigger_request(failure)
                 except simpy.Interrupt:
                     if not self.broken.triggered:
                         # Restart after fixing
                         hours_to_next = 0
                     else:
-                        # A different interruption occurred, so subtract the elapsed time
-                        hours_to_next -= self.env.now - start  # pylint: disable=E0601
+                        # A different process failed, so subtract the elapsed time
+                        # only if it had started to be processed
+                        hours_to_next -= 0 if start == -1 else self.env.now - start
```

### Comparing `wombat-0.6.2/wombat/windfarm/system/subassembly.py` & `wombat-0.7.0/wombat/windfarm/system/subassembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provides the Subassembly class"""
+"""Provides the Subassembly class."""
 
 from __future__ import annotations
 
 from typing import Generator
 
 import simpy
 
@@ -21,28 +21,29 @@
     def __init__(
         self,
         system,
         env: WombatEnvironment,
         s_id: str,
         subassembly_data: dict,
     ) -> None:
-        """Creates a subassembly object that models various maintenance and failure types.
+        """Creates a subassembly object that models various maintenance and failure
+        types.
 
         Parameters
         ----------
         system : wombat.windfarm.System
             The system containing subassembly object(s).
         env : WombatEnvironment
             The simulation environment.
         s_id : str
             A unique identifier for the subassembly within the system.
         subassembly_data : dict
-            A dictionary to be passed to ``SubassemblyData`` for creation and validation.
+            A dictionary to be passed to ``SubassemblyData`` for creation and
+            validation.
         """
-
         self.env = env
         self.system = system
         self.id = s_id
 
         subassembly_data = {**subassembly_data, "system_value": self.system.value}
         self.data = SubassemblyData.from_dict(subassembly_data)
         self.name = self.data.name
@@ -53,50 +54,57 @@
 
         self.processes = dict(self._create_processes())
 
     def _create_processes(self):
         """Creates the processes for each of the failure and maintenance types.
 
         Yields
-        -------
+        ------
         Tuple[Union[str, int], simpy.events.Process]
             Creates a dictionary to keep track of the running processes within the
             subassembly.
         """
         for level, failure in self.data.failures.items():
             yield level, self.env.process(self.run_single_failure(failure))
 
         for i, maintenance in enumerate(self.data.maintenance):
             yield f"m{i}", self.env.process(self.run_single_maintenance(maintenance))
 
     def recreate_processes(self) -> None:
-        """If a turbine is being entirely reset after a tow-to-port repair, then all
-        processes are assumed to be reset to 0, and not pick back up where they left off.
+        """If a turbine is being reset after a tow-to-port repair, then all processes
+        are assumed to be reset to 0, and not pick back up where they left off.
         """
         self.processes = dict(self._create_processes())
 
-    def interrupt_processes(self) -> None:
+    def interrupt_processes(self, origin: Subassembly | None = None) -> None:
         """Interrupts all of the running processes within the subassembly except for the
         process associated with failure that triggers the catastrophic failure.
 
         Parameters
         ----------
-        subassembly : Subassembly
-            The subassembly that should have all processes interrupted.
+        origin : Subassembly
+            The subassembly that triggered the request, if the method call is coming
+            from a subassembly shutdown event. If provided, and it is the same as the
+            current subassembly, then a try/except flow is used to ensure the process
+            that initiated the shutdown is not interrupting itself.
         """
+        if origin is not None and id(origin) == id(self):
+            for _, process in self.processes.items():
+                try:
+                    process.interrupt()
+                except RuntimeError:  # Process initiating process can't be interrupted
+                    pass
+            return
+
         for _, process in self.processes.items():
-            try:
-                process.interrupt()
-            except RuntimeError:
-                # This error occurs for the process halting all other processes.
-                pass
+            process.interrupt()
 
     def interrupt_all_subassembly_processes(self) -> None:
         """Thin wrapper for ``system.interrupt_all_subassembly_processes``."""
-        self.system.interrupt_all_subassembly_processes()
+        self.system.interrupt_all_subassembly_processes(origin=self)
 
     def trigger_request(self, action: Maintenance | Failure):
         """Triggers the actual repair or maintenance logic for a failure or maintenance
         event, respectively.
 
         Parameters
         ----------
@@ -138,83 +146,93 @@
             reason=action.description,
             additional=f"severity level {action.level}",
             request_id=repair_request.request_id,
         )
         self.system.repair_manager.submit_request(repair_request)
 
     def run_single_maintenance(self, maintenance: Maintenance) -> Generator:
-        """Runs a process to trigger one type of maintenance request throughout the simulation.
+        """Runs a process to trigger one type of maintenance request throughout the
+        simulation.
 
         Parameters
         ----------
         maintenance : Maintenance
             A maintenance category.
 
         Yields
-        -------
+        ------
         simpy.events. HOURS_IN_DAY
             Time between maintenance requests.
         """
         while True:
             hours_to_next = maintenance.frequency
             if hours_to_next == 0:
                 remainder = self.env.max_run_time - self.env.now
                 try:
                     yield self.env.timeout(remainder)
                 except simpy.Interrupt:
                     remainder -= self.env.now
 
             while hours_to_next > 0:
+                start = -1  # Ensure an interruption before processing is caught
                 try:
                     # Wait until these events are triggered and back to operational
-                    yield self.system.servicing & self.system.cable_failure & self.broken
+                    yield (
+                        self.system.servicing & self.system.cable_failure & self.broken
+                    )
 
                     start = self.env.now
                     yield self.env.timeout(hours_to_next)
                     hours_to_next = 0
                     self.trigger_request(maintenance)
 
                 except simpy.Interrupt:
                     if not self.broken.triggered:
                         # The subassembly had to restart the maintenance cycle
                         hours_to_next = 0
                     else:
-                        # A different subassembly failed, so subtract the elapsed time
-                        hours_to_next -= self.env.now - start  # pylint: disable=E0601
+                        # A different process failed, so subtract the elapsed time
+                        # only if it had started to be processed
+                        hours_to_next -= 0 if start == -1 else self.env.now - start
 
     def run_single_failure(self, failure: Failure) -> Generator:
-        """Runs a process to trigger one type of failure repair request throughout the simulation.
+        """Runs a process to trigger one type of failure repair request throughout the
+        simulation.
 
         Parameters
         ----------
         failure : Failure
             A failure classification.
 
         Yields
-        -------
+        ------
         simpy.events. HOURS_IN_DAY
             Time between failure events that need to request a repair.
         """
         while True:
             hours_to_next = failure.hours_to_next_failure()
             if hours_to_next is None:
                 remainder = self.env.max_run_time - self.env.now
                 try:
                     yield self.env.timeout(remainder)
                 except simpy.Interrupt:
                     remainder -= self.env.now
                 continue
             while hours_to_next > 0:  # type: ignore
+                start = -1  # Ensure an interruption before processing is caught
                 try:
-                    yield self.system.servicing & self.system.cable_failure & self.broken
+                    yield (
+                        self.system.servicing & self.system.cable_failure & self.broken
+                    )
                     start = self.env.now
                     yield self.env.timeout(hours_to_next)
                     hours_to_next = 0
                     self.trigger_request(failure)
 
                 except simpy.Interrupt:
                     if not self.broken.triggered:
                         # The subassembly had to be replaced so reset the timing
                         hours_to_next = 0
                     else:
-                        # A different subassembly failed, so subtract the elapsed time
-                        hours_to_next -= self.env.now - start  # pylint: disable=E0601
+                        # A different process failed, so subtract the elapsed time
+                        # only if it had started to be processed
+                        hours_to_next -= 0 if start == -1 else self.env.now - start
```

### Comparing `wombat-0.6.2/wombat/windfarm/system/system.py` & `wombat-0.7.0/wombat/windfarm/system/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,60 +150,71 @@
             try:
                 power_curve_file = self.env.data_dir / "turbines" / power_curve
                 power_curve = pd.read_csv(power_curve_file)
             except FileNotFoundError:
                 power_curve_file = self.env.data_dir / "windfarm" / power_curve
                 power_curve = pd.read_csv(power_curve_file)
                 logging.warning(
-                    "DeprecationWarning: In v0.7, all power curve files must be located in: '<library>/turbines"
+                    "DeprecationWarning: In v0.8, all power curve files must be located"
+                    " in: '<library>/turbines"
                 )
             power_curve = power_curve.loc[power_curve.power_kw != 0].reset_index(
                 drop=True
             )
             bin_width = power_curve_dict.get("bin_width", 0.5)
             self.power_curve = IEC_power_curve(
                 power_curve.windspeed_ms,
                 power_curve.power_kw,
                 windspeed_start=power_curve.windspeed_ms.min(),
                 windspeed_end=power_curve.windspeed_ms.max(),
                 bin_width=bin_width,
             )
 
-    def interrupt_all_subassembly_processes(self) -> None:
-        """Interrupts the running processes in all of the system's subassemblies."""
-        [subassembly.interrupt_processes() for subassembly in self.subassemblies]  # type: ignore
+    def interrupt_all_subassembly_processes(
+        self, origin: Subassembly | None = None
+    ) -> None:
+        """Interrupts the running processes in all of the system's subassemblies.
+
+        Parameters
+        ----------
+        origin : Subassembly
+            The subassembly that triggered the request, if the method call is coming
+            from a subassembly shutdown event.
+        """
+        [
+            subassembly.interrupt_processes(origin=origin)  # type: ignore
+            for subassembly in self.subassemblies
+        ]
 
     @property
     def operating_level(self) -> float:
         """The turbine's operating level, based on subassembly and cable performance.
 
         Returns
         -------
         float
             Operating level of the turbine.
         """
-        if not self.cable_failure.triggered or not self.servicing.triggered:
-            return 0.0
-        else:
+        if self.cable_failure.triggered and self.servicing.triggered:
             return reduce(mul, [sub.operating_level for sub in self.subassemblies])
+        return 0.0
 
     @property
     def operating_level_wo_servicing(self) -> float:
         """The turbine's operating level, based on subassembly and cable performance,
         without accounting for servicing status.
 
         Returns
         -------
         float
             Operating level of the turbine.
         """
-        if not self.cable_failure.triggered:
-            return 0.0
-        else:
+        if self.cable_failure.triggered:
             return reduce(mul, [sub.operating_level for sub in self.subassemblies])
+        return 0.0
 
     def power(self, windspeed: list[float] | np.ndarray) -> np.ndarray:
         """Generates the power output for an iterable of windspeed values.
 
         Parameters
         ----------
         windspeed : list[float] | np.ndarrays
```

### Comparing `wombat-0.6.2/wombat/windfarm/windfarm.py` & `wombat-0.7.0/wombat/windfarm/windfarm.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from wombat.windfarm.system import Cable, System
 from wombat.core.data_classes import String, SubString, WindFarmMap, SubstationMap
 from wombat.utilities.utilities import cache
 
 
 class Windfarm:
     """The primary class for operating on objects within a windfarm. The substations,
-    cables, and turbines are created as a network object to be more appropriately accessed
-    and controlled.
+    cables, and turbines are created as a network object to be more appropriately
+    accessed and controlled.
     """
 
     def __init__(
         self,
         env: WombatEnvironment,
         windfarm_layout: str,
         repair_manager: RepairManager,
@@ -53,15 +53,16 @@
         # Register the windfarm and start the logger
         self.repair_manager._register_windfarm(self)
         self.env._register_windfarm(self)
         self.env.process(self._log_operations())
 
     def _create_graph_layout(self, windfarm_layout: str) -> None:
         """Creates a network layout of the windfarm start from the substation(s) to
-        be able to capture downstream turbines that can be cut off in the event of a cable failure.
+        be able to capture downstream turbines that can be cut off in the event of a
+        cable failure.
 
         Parameters
         ----------
         windfarm_layout : str
             Filename to use for reading in the windfarm layout; must be a csv file.
         """
         try:
@@ -75,15 +76,16 @@
             layout_path = str(self.env.data_dir / "windfarm" / windfarm_layout)
             layout = (
                 pd.read_csv(layout_path)
                 .sort_values(by=["string", "order"])
                 .reset_index(drop=True)
             )
             logging.warning(
-                "DeprecationWarning: In v0.7, all wind farm layout files must be located in: '<library>/project/plant/"
+                "DeprecationWarning: In v0.8, all wind farm layout files must be"
+                " located in: '<library>/project/plant/"
             )
         layout.subassembly = layout.subassembly.fillna("")
         layout.upstream_cable = layout.upstream_cable.fillna("")
 
         windfarm = nx.DiGraph()
         windfarm.add_nodes_from(layout.id.values)
 
@@ -91,15 +93,16 @@
         for col in ("name", "latitude", "longitude", "subassembly"):
             nx.set_node_attributes(windfarm, dict(layout[["id", col]].values), name=col)
 
         # Determine which nodes are substations and which are turbines
         if "type" in layout.columns:
             if layout.loc[~layout.type.isin(("substation", "turbine"))].size > 0:
                 raise ValueError(
-                    "At least one value in the 'type' column are not one of 'substation' or 'turbine'."
+                    "At least one value in the 'type' column are not one of:"
+                    " 'substation' or 'turbine'."
                 )
             substation_filter = layout.type == "substation"
             nx.set_node_attributes(
                 windfarm, dict(layout[["id", "type"]].values), name="type"
             )
         else:
             substation_filter = layout.id == layout.substation_id
@@ -152,26 +155,30 @@
         ValueError
             Raised if the subassembly data is not provided in the layout file.
         """
         bad_data_location_messages = []
         for system_id, data in self.graph.nodes(data=True):
             if data["subassembly"] == "":
                 raise ValueError(
-                    "A 'subassembly' file must be specified for all nodes in the windfarm layout!"
+                    "A 'subassembly' file must be specified for all nodes in the"
+                    " windfarm layout!"
                 )
 
             try:
                 subassembly_dict = load_yaml(
                     self.env.data_dir / f"{data['type']}s", data["subassembly"]
                 )
             except FileNotFoundError:
                 subassembly_dict = load_yaml(
                     self.env.data_dir / "windfarm", data["subassembly"]
                 )
-                message = f"In v0.7, all {data['type']} configurations must be located in: '<library>/{data['type']}s"
+                message = (
+                    f"In v0.7, all {data['type']} configurations must be located in:"
+                    f" '<library>/{data['type']}s"
+                )
                 bad_data_location_messages.append(message)
             self.graph.nodes[system_id]["system"] = System(
                 self.env,
                 self.repair_manager,
                 system_id,
                 data["name"],
                 subassembly_dict,
@@ -195,22 +202,24 @@
         """
         get_name = "upstream_cable_name" in self.layout_df
         bad_data_location_messages = []
         for start_node, end_node, data in self.graph.edges(data=True):
             # Check that the cable data is provided
             if data["cable"] == "":
                 raise ValueError(
-                    "A 'cable' file must be specified for all nodes in the windfarm layout!"
+                    "A 'cable' file must be specified for all nodes in the"
+                    " windfarm layout!"
                 )
             try:
                 cable_dict = load_yaml(self.env.data_dir / "cables", data["cable"])
             except FileNotFoundError:
                 cable_dict = load_yaml(self.env.data_dir / "windfarm", data["cable"])
                 bad_data_location_messages.append(
-                    "In v0.7, all cable configurations must be located in: '<library>/cables/"
+                    "In v0.7, all cable configurations must be located in:"
+                    " '<library>/cables/"
                 )
 
             start_coordinates = (
                 self.graph.nodes[start_node]["latitude"],
                 self.graph.nodes[start_node]["longitude"],
             )
             end_coordinates = (
@@ -246,16 +255,16 @@
 
         # Raise the warning for soon-to-be deprecated library structure
         bad_data_location_messages = list(set(bad_data_location_messages))
         for message in bad_data_location_messages:
             logging.warning(f"DeprecationWarning: {message}")
 
     def calculate_distance_matrix(self) -> None:
-        """Calculates the geodesic distance, in km, between all of the windfarm's nodes, e.g.,
-        substations and turbines, and cables.
+        """Calculates the geodesic distance, in km, between all of the windfarm's nodes,
+        e.g., substations and turbines, and cables.
         """
         ids = list(self.graph.nodes())
         ids.extend([data["cable"].id for *_, data in self.graph.edges(data=True)])
         coords = [
             (data["latitude"], data["longitude"])
             for *_, data in (*self.graph.nodes(data=True), *self.graph.edges(data=True))
         ]
@@ -276,15 +285,15 @@
     def _create_substation_turbine_map(self) -> None:
         """Creates ``substation_turbine_map``, a dictionary, that maps substation(s) to
         the dependent turbines in the windfarm, and the weighting of each turbine in the
         windfarm.
         """
         # Get all turbines connected to each substation, excepting any connected via
         # export cables that connect substations as these operate independently
-        s_t_map = {s: {"turbines": [], "weights": []} for s in self.substation_id}  # type: ignore
+        s_t_map: dict = {s: {"turbines": [], "weights": []} for s in self.substation_id}
         for substation_id in self.substation_id:
             nodes = set(
                 nx.bfs_tree(self.graph, substation_id, depth_limit=1).nodes
             ).difference(self.substation_id)
             for node in list(nodes):
                 nodes.update(
                     list(itertools.chain(*nx.dfs_successors(self.graph, node).values()))
@@ -315,45 +324,50 @@
 
         for s_id in self.substation_id:
             start_nodes = list(
                 set(nx.bfs_tree(graph, s_id, depth_limit=1).nodes).difference(
                     substations
                 )
             )
-            wind_map[s_id] = dict(strings=dict(zip(start_nodes, itertools.repeat({}))))
+            wind_map[s_id] = {"strings": dict(zip(start_nodes, itertools.repeat({})))}
 
             for start_node in start_nodes:
                 upstream = list(
                     itertools.chain(*nx.dfs_successors(graph, start_node).values())
                 )
                 wind_map[s_id]["strings"][start_node] = {
-                    start_node: SubString(downstream=s_id, upstream=upstream)  # type: ignore
+                    start_node: SubString(
+                        downstream=s_id,  # type: ignore
+                        upstream=upstream,  # type: ignore
+                    )
                 }
                 self.cable((s_id, start_node)).set_string_details(start_node, s_id)
 
                 downstream = start_node
                 for node in upstream:
-                    wind_map[s_id]["strings"][start_node][node] = SubString(  # type: ignore
-                        downstream=downstream,
-                        upstream=list(
+                    wind_map[s_id]["strings"][start_node][node] = SubString(
+                        downstream=downstream,  # type: ignore
+                        upstream=list(  # tye: ignore
                             itertools.chain(*nx.dfs_successors(graph, node).values())
                         ),
                     )
                     self.cable((downstream, node)).set_string_details(start_node, s_id)
                     downstream = node
 
                 wind_map[s_id]["strings"][start_node] = String(  # type: ignore
                     start=start_node, upstream_map=wind_map[s_id]["strings"][start_node]
                 )
             wind_map[s_id] = SubstationMap(  # type: ignore
                 string_starts=start_nodes,
                 string_map=wind_map[s_id]["strings"],
                 downstream=graph.nodes[s_id]["connection"],
             )
-        self.wind_farm_map = WindFarmMap(substation_map=wind_map, export_cables=export)  # type: ignore
+        self.wind_farm_map = WindFarmMap(
+            substation_map=wind_map, export_cables=export  # type: ignore
+        )
 
     def finish_setup(self) -> None:
         """Final initialization hook for any substations, turbines, or cables."""
         for start_node, end_node in self.graph.edges():
             self.cable((start_node, end_node)).finish_setup()
 
     def _setup_logger(self, initial: bool = True):
@@ -367,33 +381,33 @@
             self.env._operations_csv, delimiter="|", fieldnames=self._log_columns
         )
         if initial:
             self.env._operations_writer.writeheader()
 
     def _log_operations(self):
         """Logs the operational data for a simulation."""
-        message = dict(
-            datetime=dt.datetime.now(),
-            env_datetime=self.env.simulation_time,
-            env_time=self.env.now,
-        )
+        message = {
+            "datetime": dt.datetime.now(),
+            "env_datetime": self.env.simulation_time,
+            "env_time": self.env.now,
+        }
         message.update(
             {system: self.system(system).operating_level for system in self.system_list}
         )
         self.env._operations_writer.writerow(message)
 
         HOURS = 1
         while True:
             for _ in range(10000):
                 yield self.env.timeout(HOURS)
-                message = dict(
-                    datetime=dt.datetime.now(),
-                    env_datetime=self.env.simulation_time,
-                    env_time=self.env.now,
-                )
+                message = {
+                    "datetime": dt.datetime.now(),
+                    "env_datetime": self.env.simulation_time,
+                    "env_time": self.env.now,
+                }
                 message.update(
                     {
                         system: self.system(system).operating_level
                         for system in self.system_list
                     }
                 )
                 self.env._operations_buffer.append(message)
@@ -422,16 +436,16 @@
         """Convenience function to returns the desired `Cable` object for a cable in the
         windfarm.
 
         Parameters
         ----------
         cable_id : tuple[str, str] | str
             The cable's unique identifier, of the form: (``wombat.windfarm.System.id``,
-            ``wombat.windfarm.System.id``), for the (downstream node id, upstream node id),
-            or the ``Cable.id``.
+            ``wombat.windfarm.System.id``), for the (downstream node id, upstream node
+            id), or the ``Cable.id``.
 
         Returns
         -------
         Cable
             The ``Cable`` object.
         """
         if isinstance(cable_id, str):
@@ -441,16 +455,16 @@
         try:
             return self.graph.edges[edge_id]["cable"]
         except KeyError:
             raise KeyError(f"Edge {edge_id} is invalid.")
 
     @property
     def current_availability(self) -> float:
-        """Calculates the product of all system ``operating_level`` variables across the
-        windfarm using the following forumation
+        r"""Calculates the product of all system ``operating_level`` variables across
+        the windfarm using the following forumation.
 
         .. math::
             \sum{
                 OperatingLevel_{substation_{i}} *
                 \sum{OperatingLevel_{turbine_{j}} * Weight_{turbine_{j}}}
             }
 
@@ -476,17 +490,17 @@
                 for s_id in self.substation_turbine_map
             ]
         )
         return availability
 
     @property
     def current_availability_wo_servicing(self) -> float:
-        """Calculates the product of all system ``operating_level`` variables across the
-        windfarm using the following forumation, ignoring 0 operating level due to ongoing
-        servicing.
+        r"""Calculates the product of all system ``operating_level`` variables across
+        the windfarm using the following forumation, ignoring 0 operating level due to
+        ongoing servicing.
 
         .. math::
             \sum{
                 OperatingLevel_{substation_{i}} *
                 \sum{OperatingLevel_{turbine_{j}} * Weight_{turbine_{j}}}
             }
```

### Comparing `wombat-0.6.2/wombat.egg-info/PKG-INFO` & `wombat-0.7.0/wombat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wombat
-Version: 0.6.2
+Version: 0.7.0
 Summary: Windfarm operations and maintenance cost-benefit analysis tool
 Author: Rob Hammond
 Author-email: rob.hammond@nrel.gov
 Project-URL: Source, https://github.com/WISDEM/WOMBAT
 Project-URL: Documentation, https://wisdem.github.io/WOMBAT/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wombat-0.6.2/wombat.egg-info/SOURCES.txt` & `wombat-0.7.0/wombat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -72,30 +72,14 @@
 library/code_comparison/dinwoodie/project/plant/layout_minor_repairs_only_100pct_reduction.csv
 library/code_comparison/dinwoodie/project/plant/layout_no_hlvs.csv
 library/code_comparison/dinwoodie/project/plant/layout_no_hlvs_100pct_reduction.csv
 library/code_comparison/dinwoodie/project/plant/layout_port_test.csv
 library/code_comparison/dinwoodie/project/plant/layout_tow_to_port.csv
 library/code_comparison/dinwoodie/project/port/__init__.py
 library/code_comparison/dinwoodie/project/port/base_port.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_19-50-53.804474_dinwoodie_base_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_19-53-40.511520_dinwoodie_more_ctvs_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_19-56-35.783433_dinwoodie_fewer_ctvs_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_19-59-33.470119_dinwoodie_more_techs_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-02-25.817560_dinwoodie_fewer_techs_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-05-17.573115_dinwoodie_failure_50_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-07-45.654330_dinwoodie_failure_200_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-11-33.724653_dinwoodie_no_hlvs_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-14-51.236890_dinwoodie_no_weather_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-17-54.871961_dinwoodie_historic_weather_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-20-29.841287_dinwoodie_manual_resets_only_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-22-51.475426_dinwoodie_minor_repairs_only_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-24-53.150464_dinwoodie_medium_repairs_only_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-26-43.081550_dinwoodie_major_repairs_only_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-28-27.409791_dinwoodie_major_replacements_only_metrics_inputs.yaml
-library/code_comparison/dinwoodie/results/2022-02-04_20-30-20.875717_dinwoodie_annual_service_only_metrics_inputs.yaml
 library/code_comparison/dinwoodie/results/__init__.py
 library/code_comparison/dinwoodie/results/results_data.csv
 library/code_comparison/dinwoodie/results/results_data_100pct_reduction_v0.4.1.csv
 library/code_comparison/dinwoodie/results/results_data_v0.4.1.csv
 library/code_comparison/dinwoodie/results/results_data_v0.4.csv
 library/code_comparison/dinwoodie/results/results_data_v0.5.1.csv
 library/code_comparison/dinwoodie/results/results_dict_100pct_reduction_v0.4.1.yaml
@@ -165,20 +149,14 @@
 library/code_comparison/iea26/project/config/three_mobilizations_100pct_reduction.yaml
 library/code_comparison/iea26/project/config/two_mobilizations.yaml
 library/code_comparison/iea26/project/config/two_mobilizations_100pct_reduction.yaml
 library/code_comparison/iea26/project/plant/__init__.py
 library/code_comparison/iea26/project/plant/layout.csv
 library/code_comparison/iea26/project/plant/layout_100pct_reduction.csv
 library/code_comparison/iea26/project/port/__init__.py
-library/code_comparison/iea26/results/2022-02-04_18-43-00.190127_iea_26_one_mobilization_metrics_inputs.yaml
-library/code_comparison/iea26/results/2022-02-04_18-51-33.657200_iea_26_one_mobilization_100pct_reduction_metrics_inputs.yaml
-library/code_comparison/iea26/results/2022-02-04_18-59-35.103268_iea_26_two_mobilizations_metrics_inputs.yaml
-library/code_comparison/iea26/results/2022-02-04_19-11-18.237564_iea_26_two_mobilizations_100pct_reduction_metrics_inputs.yaml
-library/code_comparison/iea26/results/2022-02-04_19-21-59.432951_iea_26_three_mobilizations_metrics_inputs.yaml
-library/code_comparison/iea26/results/2022-02-04_19-35-03.157461_iea_26_three_mobilizations_100pct_reduction_metrics_inputs.yaml
 library/code_comparison/iea26/results/__init__.py
 library/code_comparison/iea26/results/results_data.csv
 library/code_comparison/iea26/results/results_data_v0.4.1.csv
 library/code_comparison/iea26/results/results_data_v0.4.csv
 library/code_comparison/iea26/results/results_data_v0.5.1.csv
 library/code_comparison/iea26/results/results_dict_v0.4.1.yaml
 library/code_comparison/iea26/results/results_dict_v0.4.yaml
@@ -201,14 +179,26 @@
 library/code_comparison/iea26/vessels/hlv_1.yaml
 library/code_comparison/iea26/vessels/hlv_2.yaml
 library/code_comparison/iea26/vessels/hlv_3.yaml
 library/code_comparison/iea26/vessels/hlv_requests.yaml
 library/code_comparison/iea26/vessels/rmt.yaml
 library/code_comparison/iea26/weather/__init__.py
 library/code_comparison/iea26/weather/hornsrev3_weather_1996_2015.csv
+tests/test_cable.py
+tests/test_data_classes.py
+tests/test_environment.py
+tests/test_library.py
+tests/test_post_processor.py
+tests/test_repair_manager.py
+tests/test_service_equipment.py
+tests/test_simulation_api.py
+tests/test_subassembly.py
+tests/test_system.py
+tests/test_utilities.py
+tests/test_windfarm.py
 wombat/__init__.py
 wombat/__main__.py
 wombat.egg-info/PKG-INFO
 wombat.egg-info/SOURCES.txt
 wombat.egg-info/dependency_links.txt
 wombat.egg-info/requires.txt
 wombat.egg-info/top_level.txt
```

### Comparing `wombat-0.6.2/wombat.egg-info/requires.txt` & `wombat-0.7.0/wombat.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -21,38 +21,40 @@
 flake8>=5
 flake8-docstrings>=1.6
 flake8_sphinx_links==0.2.1
 black>=22.1
 isort>=5.10
 pytest>=7
 pytest-cov>=4
-mypy>=0.991
+mypy==0.991
+ruff==0.0.246
 Sphinx==4.*
 myst-nb>=0.16
 myst-parser>=0.17
 sphinx-panels>=0.6
-sphinx-book-theme>=0.3.3
+sphinx-book-theme<1,>=0.3.3
 sphinxcontrib-spelling>=7
 linkify-it-py>=2
 sphinxcontrib-bibtex>=2.4
 
 [dev]
 pre-commit>=2.20
 pylint>=2.14
 flake8>=5
 flake8-docstrings>=1.6
 flake8_sphinx_links==0.2.1
 black>=22.1
 isort>=5.10
 pytest>=7
 pytest-cov>=4
-mypy>=0.991
+mypy==0.991
+ruff==0.0.246
 
 [docs]
 Sphinx==4.*
 myst-nb>=0.16
 myst-parser>=0.17
 sphinx-panels>=0.6
-sphinx-book-theme>=0.3.3
+sphinx-book-theme<1,>=0.3.3
 sphinxcontrib-spelling>=7
 linkify-it-py>=2
 sphinxcontrib-bibtex>=2.4
```

