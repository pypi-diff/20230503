# Comparing `tmp/honeybee-grasshopper-radiance-1.9.4.tar.gz` & `tmp/honeybee-grasshopper-radiance-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-grasshopper-radiance-1.9.4.tar", last modified: Tue May  4 23:30:58 2021, max compression
+gzip compressed data, was "dist/honeybee-grasshopper-radiance-1.9.5.tar", last modified: Thu May 20 16:23:10 2021, max compression
```

## Comparing `honeybee-grasshopper-radiance-1.9.4.tar` & `honeybee-grasshopper-radiance-1.9.5.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2184 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/
--rw-r--r--   0 runner    (1001) docker     (121)     6369 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Daylight Metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Daylight.py
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Radiation Result.py
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Radiation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply Face Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply ModifierSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply Shade Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     5159 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply Window Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Assign Grids and Views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB BSDF Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB CIE Standard Sky.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Certain Illuminance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB ClearSky.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Climatebased Sky.py
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Custom Sky.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Daylight Factor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2669 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet Interior.py
--rw-r--r--   0 runner    (1001) docker     (121)     3571 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct Wea.py
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Direct Sun Hours.py
--rw-r--r--   0 runner    (1001) docker     (121)     3968 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic Aperture Group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic Shade Group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic State Geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic State.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Exterior Modifier Subset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Get Grids and Views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Glass Modifier 3.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Glass Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Interior Modifier Subset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Metal Modifier 3.py
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Metal Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Mirror Modifier 3.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Mirror Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Model to Rad Folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB ModifierSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Opaque Modifier 3.py
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Opaque Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Search Mofidier Sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Search Mofidiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sensor Grid from Rooms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sensor Grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Shade Modifier Subset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sky Matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Subface Modifier Subset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sun Matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Tau Clear Sky from STAT.py
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Translucent Modifier 3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Translucent Modifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB View from Viewport.py
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB View.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Wea From EPW.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Wea from Zhang-Huang.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/
--rw-r--r--   0 runner    (1001) docker     (121)     6086 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight Metrics.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     6161 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5339 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation Result.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5335 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply Face Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply ModifierSet.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply Shade Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply Window Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4737 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Assign Grids and Views.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB BSDF Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5315 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB CIE Standard Sky.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Certain Illuminance.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB ClearSky.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4587 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Climatebased Sky.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5601 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Custom Sky.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Daylight Factor.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet Interior.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Wea.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Direct Sun Hours.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5796 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic Aperture Group.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic Shade Group.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic State Geometry.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic State.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Exterior Modifier Subset.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Face Radiance Attributes.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Get Grids and Views.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier 3.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Interior Modifier Subset.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5209 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier 3.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4767 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier 3.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     6319 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Model to Rad Folder.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5719 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB ModifierSet.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier 3.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Room Radiance Attributes.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4220 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Search Mofidier Sets.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Search Mofidiers.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid from Rooms.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5588 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Shade Modifier Subset.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4998 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sky Matrix.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Subface Modifier Subset.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4836 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sun Matrix.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Tau Clear Sky from STAT.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier 3.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4907 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5053 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB View from Viewport.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4683 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB View.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     4517 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Wea From EPW.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)     5304 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Wea from Zhang-Huang.ghuser
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/samples/
--rw-r--r--   0 runner    (1001) docker     (121)    59371 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/annual_daylight.gh
--rw-r--r--   0 runner    (1001) docker     (121)    64773 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/creating_modifiers.gh
--rw-r--r--   0 runner    (1001) docker     (121)    40901 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/creating_skies.gh
--rw-r--r--   0 runner    (1001) docker     (121)    51792 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/daylight_factor.gh
--rw-r--r--   0 runner    (1001) docker     (121)    90555 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/dynamic_geometry.gh
--rw-r--r--   0 runner    (1001) docker     (121)    66895 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/gridbased.gh
--rw-r--r--   0 runner    (1001) docker     (121)    54990 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/samples/viewbased.gh
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-04 23:30:58.000000 honeybee-grasshopper-radiance-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      914 2021-05-04 23:30:14.000000 honeybee-grasshopper-radiance-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3103 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2184 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     6369 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Daylight Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5075 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Daylight.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3997 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Radiation Result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3764 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Radiation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4388 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply Face Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply ModifierSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4347 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply Shade Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5159 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply Window Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Assign Grids and Views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB BSDF Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB CIE Standard Sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Certain Illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB ClearSky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Climatebased Sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2573 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Custom Sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Daylight Factor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2669 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet Interior.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3571 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1419 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct Wea.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Direct Sun Hours.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3968 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic Aperture Group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4156 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic Shade Group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic State Geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic State.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Exterior Modifier Subset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2448 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Get Grids and Views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2421 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Glass Modifier 3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Glass Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3240 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Interior Modifier Subset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Metal Modifier 3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2593 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Metal Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Mirror Modifier 3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Mirror Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2565 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Model to Rad Folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB ModifierSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Opaque Modifier 3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Opaque Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2140 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Search Mofidier Sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2105 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Search Mofidiers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6481 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sensor Grid from Rooms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sensor Grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Shade Modifier Subset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sky Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Subface Modifier Subset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sun Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Tau Clear Sky from STAT.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3192 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Translucent Modifier 3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Translucent Modifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3126 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB View from Viewport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3849 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB View.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Wea From EPW.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Wea from Zhang-Huang.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/
+-rw-r--r--   0 runner    (1001) docker     (121)     6086 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight Metrics.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     6161 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5339 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation Result.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5335 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4939 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply Face Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply ModifierSet.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4728 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply Shade Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5055 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply Window Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4737 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Assign Grids and Views.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB BSDF Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5324 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB CIE Standard Sky.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4156 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Certain Illuminance.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4646 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB ClearSky.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4587 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Climatebased Sky.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5605 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Custom Sky.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Daylight Factor.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     3981 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4556 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet Interior.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4973 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Wea.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5838 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Direct Sun Hours.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5796 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic Aperture Group.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4829 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic Shade Group.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4164 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic State Geometry.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic State.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     3926 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Exterior Modifier Subset.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Face Radiance Attributes.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5013 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Get Grids and Views.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier 3.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4109 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4148 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Interior Modifier Subset.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5209 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier 3.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4767 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4620 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier 3.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     6319 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Model to Rad Folder.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5719 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB ModifierSet.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5228 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier 3.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4669 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Room Radiance Attributes.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4220 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Search Mofidier Sets.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Search Mofidiers.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid from Rooms.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5588 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Shade Modifier Subset.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4998 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sky Matrix.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Subface Modifier Subset.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4836 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sun Matrix.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     6040 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Tau Clear Sky from STAT.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5422 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier 3.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4907 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5053 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB View from Viewport.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4683 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB View.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     4517 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Wea From EPW.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)     5304 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Wea from Zhang-Huang.ghuser
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3103 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7749 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/samples/
+-rw-r--r--   0 runner    (1001) docker     (121)    59371 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/annual_daylight.gh
+-rw-r--r--   0 runner    (1001) docker     (121)    64773 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/creating_modifiers.gh
+-rw-r--r--   0 runner    (1001) docker     (121)    40901 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/creating_skies.gh
+-rw-r--r--   0 runner    (1001) docker     (121)    51792 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/daylight_factor.gh
+-rw-r--r--   0 runner    (1001) docker     (121)    90555 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/dynamic_geometry.gh
+-rw-r--r--   0 runner    (1001) docker     (121)    66895 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/gridbased.gh
+-rw-r--r--   0 runner    (1001) docker     (121)    54990 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/samples/viewbased.gh
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-20 16:23:10.000000 honeybee-grasshopper-radiance-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2021-05-20 16:22:23.000000 honeybee-grasshopper-radiance-1.9.5/setup.py
```

### Comparing `honeybee-grasshopper-radiance-1.9.4/.github/workflows/ci.yaml` & `honeybee-grasshopper-radiance-1.9.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/LICENSE` & `honeybee-grasshopper-radiance-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/PKG-INFO` & `honeybee-grasshopper-radiance-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-grasshopper-radiance
-Version: 1.9.4
+Version: 1.9.5
 Summary: Honeybee Radiance plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/honeybee-grasshopper-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Description: [![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/actions)
```

### Comparing `honeybee-grasshopper-radiance-1.9.4/README.md` & `honeybee-grasshopper-radiance-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Daylight Metrics.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Daylight Metrics.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Daylight.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Daylight.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Radiation Result.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Radiation Result.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Annual Radiation.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Annual Radiation.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply Face Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply Face Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply ModifierSet.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply ModifierSet.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply Shade Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply Shade Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Apply Window Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Apply Window Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Assign Grids and Views.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Assign Grids and Views.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB BSDF Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB BSDF Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB CIE Standard Sky.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB CIE Standard Sky.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 # You should have received a copy of the GNU General Public License
 # along with Honeybee; If not, see <http://www.gnu.org/licenses/>.
 # 
 # @license GPL-3.0+ <http://spdx.org/licenses/GPL-3.0+>
 
 """
 Create a point-in-time standard Radiance CIE sky.
+-
 
     Args:
         north_: A number between 0 and 360 that represents the degrees off from
             the y-axis to make North. This can also be a vector to set the North.
             Default is 0. The default North direction is the Y-axis (0 degrees).
         _location: A Ladybug location object.
         _month_: An integer between 1 and 12 for the month of the year (default: 6).
         _day_: An integer between 1 and 31 for the day of the month (default: 21).
-        _hour_: A number between 0 and 23.999.. for the hour of the day (default: 12).
+        _hour_: A number between 0 and 23.999 for the hour of the day (default: 12).
         _type_: An integer between 0..5 to indicate CIE Sky Type (default: 0).
-            [0] Sunny with sun
-            [1] sunny without sun
-            [2] intermediate with sun
-            [3] intermediate without sun
-            [4] cloudy sky
-            [5] uniform sky
-    
+            * 0 = Sunny with sun
+            * 1 = sunny without sun
+            * 2 = intermediate with sun
+            * 3 = intermediate without sun
+            * 4 = cloudy sky
+            * 5 = uniform sky
+
     Returns:
         sky: A honeybee sky that can be used to create a point-in-time recipe.
 """
 
 ghenv.Component.Name = 'HB CIE Standard Sky'
 ghenv.Component.NickName = 'CIESky'
-ghenv.Component.Message = '1.2.0'
+ghenv.Component.Message = '1.2.1'
 ghenv.Component.Category = 'HB-Radiance'
 ghenv.Component.SubCategory = '2 :: Light Sources'
 ghenv.Component.AdditionalHelpFromDocStrings = '1'
 
 try:
     from ladybug_geometry.geometry2d.pointvector import Vector2D
 except ImportError as e:
```

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Certain Illuminance.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Certain Illuminance.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB ClearSky.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB ClearSky.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Climatebased Sky.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Climatebased Sky.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Custom Sky.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Custom Sky.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 # You should have received a copy of the GNU General Public License
 # along with Honeybee; If not, see <http://www.gnu.org/licenses/>.
 # 
 # @license GPL-3.0+ <http://spdx.org/licenses/GPL-3.0+>
 
 """
 Create a Custom sky from direct and diffuse irradiance.
+-
 
     Args:
         north_: A number between 0 and 360 that represents the degrees off from
             the y-axis to make North. This can also be a vector to set the North.
             Default is 0. The default North direction is the Y-axis (0 degrees).
         _location: A Ladybug location object.
         _dir_rad: Direct normal irradiance (W/m2).
         _diff_rad: Diffuse horizontal irradiance (W/m2).
         _month_: An integer between 1 and 12 for the month of the year (default: 6).
         _day_: An integer between 1 and 31 for the day of the month (default: 21).
-        _hour_: A number between 0 and 23.999.. for the hour of the day (default: 12).
-    
+        _hour_: A number between 0 and 23.999 for the hour of the day (default: 12).
+
     Returns:
         sky: Honeybee sky. You can use this sky to create a daylight recipe.
 """
 
 ghenv.Component.Name = 'HB Custom Sky'
 ghenv.Component.NickName = 'CustomSky'
-ghenv.Component.Message = '1.2.0'
+ghenv.Component.Message = '1.2.1'
 ghenv.Component.Category = 'HB-Radiance'
 ghenv.Component.SubCategory = '2 :: Light Sources'
 ghenv.Component.AdditionalHelpFromDocStrings = '1'
 
 try:
     from ladybug_geometry.geometry2d.pointvector import Vector2D
 except ImportError as e:
```

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Daylight Factor.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Daylight Factor.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet Interior.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet Interior.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct ModifierSet.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Deconstruct Wea.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Deconstruct Wea.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Direct Sun Hours.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Direct Sun Hours.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic Aperture Group.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic Aperture Group.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic Shade Group.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic Shade Group.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic State Geometry.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic State Geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Dynamic State.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Dynamic State.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Exterior Modifier Subset.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Exterior Modifier Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Get Grids and Views.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Get Grids and Views.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Glass Modifier 3.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Glass Modifier 3.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Glass Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Glass Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Interior Modifier Subset.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Interior Modifier Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Metal Modifier 3.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Metal Modifier 3.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Metal Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Metal Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Mirror Modifier 3.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Mirror Modifier 3.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Mirror Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Mirror Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Model to Rad Folder.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Model to Rad Folder.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB ModifierSet.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB ModifierSet.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Opaque Modifier 3.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Opaque Modifier 3.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Opaque Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Opaque Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Search Mofidier Sets.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Search Mofidier Sets.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Search Mofidiers.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Search Mofidiers.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sensor Grid from Rooms.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sensor Grid from Rooms.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sensor Grid.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sensor Grid.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Shade Modifier Subset.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Shade Modifier Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sky Matrix.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sky Matrix.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Subface Modifier Subset.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Subface Modifier Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Sun Matrix.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Sun Matrix.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Tau Clear Sky from STAT.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Tau Clear Sky from STAT.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Translucent Modifier 3.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Translucent Modifier 3.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Translucent Modifier.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Translucent Modifier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB View from Viewport.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB View from Viewport.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB View.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB View.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Wea From EPW.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Wea From EPW.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/src/HB Wea from Zhang-Huang.py` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/src/HB Wea from Zhang-Huang.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight Metrics.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight Metrics.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Daylight.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation Result.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation Result.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Annual Radiation.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply Face Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply Face Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply ModifierSet.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply ModifierSet.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply Shade Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply Shade Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Apply Window Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Apply Window Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Assign Grids and Views.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Assign Grids and Views.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB BSDF Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB BSDF Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Certain Illuminance.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Certain Illuminance.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB ClearSky.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB ClearSky.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Climatebased Sky.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Climatebased Sky.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Daylight Factor.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Daylight Factor.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet Interior.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet Interior.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct ModifierSet.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Wea.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Deconstruct Wea.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Direct Sun Hours.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Direct Sun Hours.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic Aperture Group.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic Aperture Group.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic Shade Group.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic Shade Group.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic State Geometry.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic State Geometry.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Dynamic State.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Dynamic State.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Exterior Modifier Subset.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Exterior Modifier Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Face Radiance Attributes.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Face Radiance Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Get Grids and Views.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Get Grids and Views.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier 3.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier 3.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Glass Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Interior Modifier Subset.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Interior Modifier Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier 3.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier 3.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Metal Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier 3.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier 3.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Mirror Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Model to Rad Folder.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Model to Rad Folder.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB ModifierSet.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB ModifierSet.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier 3.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier 3.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Opaque Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Room Radiance Attributes.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Room Radiance Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Search Mofidier Sets.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Search Mofidier Sets.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Search Mofidiers.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Search Mofidiers.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid from Rooms.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid from Rooms.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sensor Grid.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Shade Modifier Subset.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Shade Modifier Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sky Matrix.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sky Matrix.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Subface Modifier Subset.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Subface Modifier Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Sun Matrix.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Sun Matrix.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Tau Clear Sky from STAT.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Tau Clear Sky from STAT.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier 3.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier 3.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Translucent Modifier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB View from Viewport.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB View from Viewport.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB View.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB View.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Wea From EPW.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Wea From EPW.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance/user_objects/HB Wea from Zhang-Huang.ghuser` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance/user_objects/HB Wea from Zhang-Huang.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/PKG-INFO` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-grasshopper-radiance
-Version: 1.9.4
+Version: 1.9.5
 Summary: Honeybee Radiance plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/honeybee-grasshopper-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Description: [![Build Status](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/actions)
```

### Comparing `honeybee-grasshopper-radiance-1.9.4/honeybee_grasshopper_radiance.egg-info/SOURCES.txt` & `honeybee-grasshopper-radiance-1.9.5/honeybee_grasshopper_radiance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/annual_daylight.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/annual_daylight.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/creating_modifiers.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/creating_modifiers.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/creating_skies.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/creating_skies.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/daylight_factor.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/daylight_factor.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/dynamic_geometry.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/dynamic_geometry.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/gridbased.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/gridbased.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/samples/viewbased.gh` & `honeybee-grasshopper-radiance-1.9.5/samples/viewbased.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-radiance-1.9.4/setup.py` & `honeybee-grasshopper-radiance-1.9.5/setup.py`

 * *Files identical despite different names*

