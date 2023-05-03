# Comparing `tmp/saenopy-0.8.0.tar.gz` & `tmp/saenopy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saenopy-0.8.0.tar", max compression
+gzip compressed data, was "saenopy-0.9.0.tar", max compression
```

## Comparing `saenopy-0.8.0.tar` & `saenopy-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,117 @@
--rw-r--r--   0        0        0     1065 2022-11-15 20:41:59.874962 saenopy-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0      622 2022-11-15 20:41:59.874962 saenopy-0.8.0/README.md
--rw-r--r--   0        0        0      874 2022-11-15 20:41:59.878962 saenopy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    23506 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/VirtualBeads.py
--rw-r--r--   0        0        0      377 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/__init__.py
--rw-r--r--   0        0        0     1467 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/buildBeams.py
--rw-r--r--   0        0        0     3723 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/configHelper.py
--rw-r--r--   0        0        0     1329 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/conjugateGradient.py
--rw-r--r--   0        0        0     1518 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/convert_solver_to_result.py
--rw-r--r--   0        0        0     1296 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/examples.py
--rw-r--r--   0        0        0    10095 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/getDeformations.py
--rw-r--r--   0        0        0    16759 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/QExtendedGraphicsView.py
--rw-r--r--   0        0        0    28101 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/QtShortCuts.py
--rw-r--r--   0        0        0        0 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/__init__.py
--rw-r--r--   0        0        0    19506 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/gui_classes.py
--rw-r--r--   0        0        0     6027 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/patch_lifreader.py
--rw-r--r--   0        0        0    22392 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/stack_selector.py
--rw-r--r--   0        0        0     2740 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/stack_selector_leica.py
--rw-r--r--   0        0        0    11885 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui/stack_selector_tif.py
--rw-r--r--   0        0        0    15298 2022-11-15 20:41:59.878962 saenopy-0.8.0/saenopy/gui_deformation.py
--rw-r--r--   0        0        0    93266 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_deformation_spheriod.py
--rw-r--r--   0        0        0   106812 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_deformation_whole2.py
--rw-r--r--   0        0        0    25356 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_deformation_wizard.py
--rw-r--r--   0        0        0     5371 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_master.py
--rw-r--r--   0        0        0    13945 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_mpl.py
--rw-r--r--   0        0        0    51627 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_orientation.py
--rw-r--r--   0        0        0     3582 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_reorder.py
--rw-r--r--   0        0        0    14360 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/gui_vtk.py
--rw-r--r--   0        0        0   121584 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/img/Icon.ico
--rw-r--r--   0        0        0    42003 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/img/Logo.png
--rw-r--r--   0        0        0    73872 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/img/Logo.svg
--rw-r--r--   0        0        0    23199 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/load.py
--rw-r--r--   0        0        0     8317 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/loadHelpers.py
--rw-r--r--   0        0        0    17511 2022-11-15 20:41:59.882962 saenopy-0.8.0/saenopy/macro.py
--rw-r--r--   0        0        0    14374 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/main.py
--rw-r--r--   0        0        0    12588 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/materials.py
--rw-r--r--   0        0        0    12913 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/meshViewer.py
--rw-r--r--   0        0        0    21848 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/multigridHelper.py
--rw-r--r--   0        0        0      923 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/numbaOverload.py
--rw-r--r--   0        0        0     5811 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/save.py
--rw-r--r--   0        0        0    77881 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/solver.py
--rw-r--r--   0        0        0    28379 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/stack3DHelper.py
--rw-r--r--   0        0        0    12310 2022-11-15 20:41:59.886962 saenopy-0.8.0/saenopy/tfjit.py
--rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 saenopy-0.8.0/setup.py
--rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 saenopy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-03 13:41:00.082380 saenopy-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1187 2023-05-03 13:41:00.082380 saenopy-0.9.0/README.md
+-rw-r--r--   0        0        0     1268 2023-05-03 13:41:00.202382 saenopy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      451 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/__init__.py
+-rw-r--r--   0        0        0     1467 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/buildBeams.py
+-rw-r--r--   0        0        0     1329 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/conjugateGradient.py
+-rw-r--r--   0        0        0     6868 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/examples.py
+-rw-r--r--   0        0        0    15348 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/getDeformations.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/__init__.py
+-rw-r--r--   0        0        0     3918 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/code_editor.py
+-rw-r--r--   0        0        0     7389 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/gui_code.py
+-rw-r--r--   0        0        0     4605 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/script_file.py
+-rw-r--r--   0        0        0     7099 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/syntax.py
+-rw-r--r--   0        0        0    19372 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/QExtendedGraphicsView.py
+-rw-r--r--   0        0        0    45878 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/QtShortCuts.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/__init__.py
+-rw-r--r--   0        0        0    21865 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/gui_classes.py
+-rw-r--r--   0        0        0    33197 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/lif_reader.py
+-rw-r--r--   0        0        0     6027 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/patch_lifreader.py
+-rw-r--r--   0        0        0      282 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/resources.py
+-rw-r--r--   0        0        0    15449 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/sigmoid_widget.py
+-rw-r--r--   0        0        0     6583 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_preview.py
+-rw-r--r--   0        0        0     3888 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector.py
+-rw-r--r--   0        0        0     9342 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector_crop.py
+-rw-r--r--   0        0        0     3096 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector_leica.py
+-rw-r--r--   0        0        0    11924 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector_tif.py
+-rw-r--r--   0        0        0     6616 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/gui_master.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/orientation/__init__.py
+-rw-r--r--   0        0        0    51641 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/orientation/gui_orientation.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/analyze/__init__.py
+-rw-r--r--   0        0        0    20407 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/analyze/plot_window.py
+-rw-r--r--   0        0        0     1575 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/gui_solver.py
+-rw-r--r--   0        0        0    16164 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0    11509 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/DeformationDetector.py
+-rw-r--r--   0        0        0     4242 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/FittedMesh.py
+-rw-r--r--   0        0        0    11457 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/MeshCreator.py
+-rw-r--r--   0        0        0     9449 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/PipelineModule.py
+-rw-r--r--   0        0        0     1103 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/QTimeSlider.py
+-rw-r--r--   0        0        0    13629 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/Regularizer.py
+-rw-r--r--   0        0        0    10923 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/ResultView.py
+-rw-r--r--   0        0        0    19430 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/StackDisplay.py
+-rw-r--r--   0        0        0    12999 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/VTK_Toolbar.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/__init__.py
+-rw-r--r--   0        0        0      541 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/code_export.py
+-rw-r--r--   0        0        0     6446 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
+-rw-r--r--   0        0        0    47962 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/Exporter.py
+-rw-r--r--   0        0        0    13663 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
+-rw-r--r--   0        0        0    17535 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
+-rw-r--r--   0        0        0    18777 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/FiberViewer.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/__init__.py
+-rw-r--r--   0        0        0    11018 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/load_measurement_dialog.py
+-rw-r--r--   0        0        0     3854 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/path_editor.py
+-rw-r--r--   0        0        0    11908 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/showVectorField.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/spheroid/__init__.py
+-rw-r--r--   0        0        0    92474 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/spheroid/gui_deformation_spheroid.py
+-rw-r--r--   0        0        0    53944 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/img/Icon.ico
+-rw-r--r--   0        0        0    42003 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/Logo.png
+-rw-r--r--   0        0        0    77561 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/Logo.svg
+-rw-r--r--   0        0        0    37691 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/Logo_black.png
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/arrowscale.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/autoscale0.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/autoscale1.ico
+-rw-r--r--   0        0        0    48947 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/buttons.svg
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/center0.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/center1.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/contrast0.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/contrast1.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/grid.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/grid2.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/grid3.ico
+-rw-r--r--   0        0        0    38885 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/logo_splash.png
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/nan0.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/nan1.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/show_image.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/show_image2.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/show_image3.ico
+-rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice0.ico
+-rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice1.ico
+-rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice2.ico
+-rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice_all.ico
+-rw-r--r--   0        0        0   121664 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/thumbnails/BFTFM.png
+-rw-r--r--   0        0        0   132449 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/thumbnails/BFTFM_2.png
+-rw-r--r--   0        0        0   180081 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/Bead_example_icon.png
+-rw-r--r--   0        0        0   202759 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/Dynamic_icon.png
+-rw-r--r--   0        0        0   554429 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/StainedOrganoid_icon.png
+-rw-r--r--   0        0        0   263760 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/liver_fibroblast_icon.png
+-rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/view_single.ico
+-rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/view_two.ico
+-rw-r--r--   0        0        0     4021 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/loadHelpers.py
+-rw-r--r--   0        0        0    17511 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/macro.py
+-rw-r--r--   0        0        0    12590 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/materials.py
+-rw-r--r--   0        0        0    22326 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/multigridHelper.py
+-rw-r--r--   0        0        0      923 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/numbaOverload.py
+-rw-r--r--   0        0        0    13782 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/result_file.py
+-rw-r--r--   0        0        0     6611 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/saveable.py
+-rw-r--r--   0        0        0    75256 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/solver.py
+-rw-r--r--   0        0        0    11684 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/stack.py
+-rw-r--r--   0        0        0    22838 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/VirtualBeads.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/__init__.py
+-rw-r--r--   0        0        0     3583 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/configHelper.py
+-rw-r--r--   0        0        0     2788 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/convert_solver_to_result.py
+-rw-r--r--   0        0        0    15114 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_deformation.py
+-rw-r--r--   0        0        0    24879 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_deformation_wizard.py
+-rw-r--r--   0        0        0     1225 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_master.spec
+-rw-r--r--   0        0        0    13703 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_mpl.py
+-rw-r--r--   0        0        0     3016 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_reorder.py
+-rw-r--r--   0        0        0    15886 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_vtk.py
+-rw-r--r--   0        0        0    22642 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/load.py
+-rw-r--r--   0        0        0    14055 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/main.py
+-rw-r--r--   0        0        0    12568 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/meshViewer.py
+-rw-r--r--   0        0        0      167 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/requirements.txt
+-rw-r--r--   0        0        0     5639 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/save.py
+-rw-r--r--   0        0        0    28379 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/stack3DHelper.py
+-rw-r--r--   0        0        0    12051 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/tfjit.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 saenopy-0.9.0/PKG-INFO
```

### Comparing `saenopy-0.8.0/LICENSE.txt` & `saenopy-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/pyproject.toml` & `saenopy-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 [tool.poetry]
 name = "saenopy"
-version = "0.8.0"
+version = "0.9.0"
 description = "Semi-elastic fiber optimisation in python."
 authors = ["rgerum <14153051+rgerum@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "saenopy"}]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8,<3.12"
 numpy = "^1.23.4"
 scipy = "^1.9.3"
 tqdm = "^4.64.1"
 qimage2ndarray = "^1.9.0"
 natsort = "^8.2.0"
 pyvista = "^0.37.0"
 pyvistaqt = "^0.9.0"
 imagecodecs = "^2022.9.26"
 openpiv = "^0.24.2"
 pyqt5 = "^5.15.7"
 qtawesome = "^1.2.1"
 jointforces = "^1.0.1"
 numba = "^0.56.4"
-sphinx-rtd-theme = { version = "^1.1.1", optional = true }
+sphinx = { version = "^6.1.3", optional = true }
+sphinx-rtd-theme = { version = "^1.2.0", optional = true }
 nbsphinx = { version = "^0.8.10", optional = true }
+sphinx-gallery = {version = "^0.11.1", optional = true }
+appdirs = "^1.4.4"
+nptyping = "^2.4.1"
+qtrangeslider = "^0.1.5"
+h5py = "^3.8.0"
 
 
 [tool.poetry.extras]
-docs = ["sphinx-rtd-theme", "nbsphinx"]
+docs = ["sphinx", "sphinx-rtd-theme", "nbsphinx", "sphinx-gallery"]
 
 
 [tool.poetry.scripts]
-saenopy = "saenopy.gui_master:main"
+saenopy = "saenopy.gui.gui_master:main"
 
 
+[tool.poetry.group.dev.dependencies]
+pyinstaller = "^5.9.0"
+auto-py-to-exe = "^2.33.0"
+pytest = "^7.2.2"
+coverage = "^5.0.0"
+hypothesis = "^6.74.1"
+coveralls = "^3.3.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `saenopy-0.8.0/saenopy/VirtualBeads.py` & `saenopy-0.9.0/saenopy/unused/VirtualBeads.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,696 +1,696 @@
-import time
-
-import numpy as np
-import scipy.sparse as ssp
-
-from .solver import Solver
-from .conjugateGradient import cg
-from .stack3DHelper import crosscorrelateStacks, getSubstack, findLocalDisplacement
-
-
-class timeit:
-
-    def __init__(self, name):
-        self.name = name
-
-    def __enter__(self):
-        self.start = time.time()
-        print("Start", self.name)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        print("End", self.name, "%.3fs" % (time.time() - self.start))
-
-
-class IA:
-    def __init__(self, A, I):
-        self.A = A
-        self.I = I
-
-    def __matmul__(self, other):
-        return self.I * other + self.A @ other
-
-
-def norm(x):
-    return np.sum(x**2)
-
-
-class VirtualBeads:
-    def __init__(self, CFG, ssX=None, ssY=None, ssZ=None, ddX=None, ddY=None, ddZ=None):
-        self.CFG = CFG
-        self.sX = ssX
-        self.sY = ssY
-        self.sZ = ssZ
-        self.dX = ddX
-        self.dY = ddY
-        self.dZ = ddZ
-
-        self.S_0 = []
-
-        self.U_found = []
-        self.R_found = []
-        self.U_guess = []
-
-        self.I = None
-        self.Itrans = None
-        self.ItransI = None
-
-        self.vbead = []
-        self.outofstack = []
-
-        self.u_x = []
-        self.u_y = []
-        self.u_z = []
-
-        self.localweight = []
-        self.conconnections = None
-        self.oldconconnections = None
-        self.b = []
-
-        self.Drift = np.array([0, 0, 0])
-
-    def allBeads(self, M):
-        thresh = self.CFG["VB_SX"] * self.dX + 2.0 * self.CFG["DRIFT_STEP"]
-
-        self.vbead = np.zeros(M.N_c, dtype=bool)
-
-        Scale = np.eye(3) * np.array([self.dX, self.dY, self.dZ])
-
-        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
-
-        Trans = Scale
-
-        for t in range(M.N_c):
-            R = Trans @ M.R[t] + scaledShift
-
-            if thresh < R[0] < (self.sX - thresh) and \
-                    thresh < R[1] < (self.sY - thresh) and \
-                    thresh < R[2] < (self.sZ - thresh):
-                self.vbead[t] = True
-
-    def computeOutOfStack(self, M):
-        thresh = self.CFG["VB_SX"] * self.dX + 2.0 * self.CFG["DRIFT_STEP"]
-
-        self.outofstack = np.array(M.N_c, dtype=bool)
-
-        Scale = np.eye(3) * np.array([self.dX, self.dY, self.dZ])
-
-        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
-
-        Trans = Scale
-
-        for t in range(M.N_c):
-            R = Trans @ M.R[t] + scaledShift
-
-            if thresh < R[0] < (self.sX - thresh) and \
-                    thresh < R[1] < (self.sY - thresh) and \
-                    thresh < R[2] < (self.sZ - thresh):
-                self.outofstack[t] = False
-
-    def loadVbeads(self, VBname):
-        vbead_temp = np.loadtxt(VBname)
-
-        self.vbead = vbead_temp[:, 0] > 0.5
-
-    def loadGuess(self, M, ugname):
-        from .loadHelpers import loadBoundaryConditions
-        var, U, f_ext = loadBoundaryConditions(ugname)
-        M.var = var
-        M.f_ext = f_ext
-        self.U_guess = U
-        M._computeConnections()
-
-    def updateLocalWeigth(self, M, method):
-
-        self.localweight[:] = 1
-
-        Fvalues = np.linalg.norm(M.f_glo, axis=1)
-        Fmedian = np.median(Fvalues[M.var])
-
-        if method == "singlepoint":
-            self.localweight[int(self.CFG["REG_FORCEPOINT"])] = 1.0e-10
-
-        if method == "bisquare":
-            k = 4.685
-
-            index = Fvalues < k * Fmedian
-            self.localweight[index * M.var] *= (1 - (Fvalues / k / Fmedian) * (Fvalues / k / Fmedian)) * (
-                    1 - (Fvalues / k / Fmedian) * (Fvalues / k / Fmedian))
-            self.localweight[~index * M.var] *= 1e-10
-
-        if method == "cauchy":
-            k = 2.385
-
-            if Fmedian > 0:
-                self.localweight[M.var] *= 1.0 / (1.0 + np.power((Fvalues / k / Fmedian), 2.0))
-            else:
-                self.localweight *= 1.0
-
-        if method == "huber":
-            k = 1.345
-
-            index = (Fvalues > (k * Fmedian)) * M.var
-            self.localweight[index] = k * Fmedian / Fvalues[index]
-
-        index = self.localweight < 1e-10
-        self.localweight[index * M.var] = 1e-10
-
-        counter = np.sum(1.0 - self.localweight[M.var])
-        counterall = np.sum(M.var)
-
-        print("total weight: ", counter, "/", counterall)
-
-    def loadUfound(self, Uname, Sname):
-        self.U_found = np.loadtxt(Uname)
-        self.S_0 = np.loadtxt(Sname)
-        self.vbead = self.S_0 > 0.7
-
-    def computeConconnections(self, M):
-        """
-        conconections seem to be the indirect connections e.g. A->B->C
-        this means a has an indirect connection (or 2. order connection) to c
-        """
-        self.conconnections = []
-        for c1 in range(M.N_c):
-            self.conconnections.append(set())
-
-        for c1 in range(M.N_c):
-            for c2 in M.connections[c1]:
-                for c3 in M.connections[c2]:
-                    if c3 not in self.conconnections[c1]:
-                        self.conconnections[c1].add(c3)
-
-    def computeConconnections_Laplace(self, M):
-        """
-        seems to adanve the order of which connections to look at
-        """
-        self.conconnections = []
-        self.oldconconnections = []
-        for c1 in range(M.N_c):
-            self.oldconconnections[c1] = self.conconnections[c1]
-            self.conconnections.append(set())
-
-        for c1 in range(M.N_c):
-            for c2 in self.oldconconnections[c1]:
-                for c3 in self.oldconconnections[c2]:
-                    if c3 not in self.conconnections[c1]:
-                        self.conconnections[c1].add(c3)
-
-    def substractMedianDisplacements(self):
-        index = np.abs(self.U_found) > 0.01 * self.CFG["VOXELSIZEX"]
-        u_median = np.median(self.U_found[index], axis=0)
-        print("Median displacement calculated to", u_median)
-
-        self.U_found -= u_median
-
-    def findDriftCoarse(self, stackr: np.ndarray, stacka: np.ndarray, abs_range: float, step: float) -> np.ndarray:
-
-        Smax = -1.0
-        best_shift = np.array([0, 0, 0])
-
-        # iterate over all shifts in the rage and step and find the best correlation
-        for dx in np.arange(-abs_range, abs_range, step):
-            for dy in np.arange(-abs_range, abs_range, step):
-                for dz in np.arange(-abs_range, abs_range, step):
-                    shift = np.array([dx, dy, dz])
-
-                    # get the correlation for this shift
-                    Stemp = self.testDrift(stackr, stacka, shift)
-
-                    # if it is better than the previous best, store it
-                    if Stemp > Smax:
-                        best_shift = shift
-                        Smax = Stemp
-
-        # return the best shift
-        return best_shift
-
-    def findDrift(self, stackr: np.ndarray, stacka: np.ndarray) -> np.ndarray:
-
-        lambd = 0.0
-
-        hinit = float(self.CFG["DRIFT_STEP"])
-        subpixel = float(self.CFG["SUBPIXEL"])
-
-        vsx = float(self.CFG["VOXELSIZEX"])
-        vsy = float(self.CFG["VOXELSIZEY"])
-        vsz = float(self.CFG["VOXELSIZEZ"])
-
-        P = np.array([
-            [1, 1, 1],
-            [-1, -1, 1],
-            [-1, 1, -1],
-            [1, -1, -1],
-        ]) * hinit
-
-        S = [
-            self.testDrift(stackr, stacka, P[0] + self.Drift) - lambd * norm(P[0]),
-            self.testDrift(stackr, stacka, P[1] + self.Drift) - lambd * norm(P[1]),
-            self.testDrift(stackr, stacka, P[2] + self.Drift) - lambd * norm(P[2]),
-            self.testDrift(stackr, stacka, P[3] + self.Drift) - lambd * norm(P[3]),
-        ]
-
-        # std::cout<<S[0]<<" "<<S[1]<<" "<<S[2]<<" "<<S[3]<<" \n";
-        done = False
-        for ii in range(100000):
-            if done:
-                break
-
-            mini = np.argmin(S)
-            maxi = np.argmax(S)
-
-            # std::cout<<"| new cycle mini = "<<mini<<std::endl;
-            # reflect
-            P_plane = np.array([0.0, 0.0, 0.0])
-            for i in range(4):
-                if i != mini:
-                    P_plane += P[i]
-            P_plane /= 3
-
-            P_ref = P[mini] + (P_plane - P[mini]) * 2.0
-
-            S_ref = self.testDrift(stackr, stacka, P_ref + self.Drift) - lambd * norm(P_ref)
-
-            if S_ref > S[maxi]:
-                # expand
-                # std::cout<<"| expanding "<<std::endl;
-                P_exp = P[mini] + (P_plane - P[mini]) * 3.0
-                S_exp = self.testDrift(stackr, stacka, P_exp + self.Drift) - lambd * norm(P_exp)
-
-                if S_exp > S_ref:
-                    # std::cout<<"| took expanded "<<std::endl;
-                    P[mini] = P_exp
-                    S[mini] = S_exp
-
-                else:
-                    # std::cout<<"| took reflected (expanded was worse)"<<std::endl;
-                    P[mini] = P_ref
-                    S[mini] = S_ref
-            else:
-                bsw = False
-                for i in range(4):
-                    if i != mini:
-                        if S_ref > S[i]:
-                            bsw = True
-
-                if bsw:
-                    # std::cout<<"| took reflected (better than second worst)"<<std::endl;
-                    P[mini] = P_ref
-                    S[mini] = S_ref
-
-                else:
-                    if S_ref > S[maxi]:
-                        # std::cout<<"| took reflected (not better than second worst)"<<std::endl;
-                        P[mini] = P_ref
-                        S[mini] = S_ref
-                    else:
-                        P_con = P[mini] + (P_plane - P[mini]) * 0.5
-                        S_con = self.testDrift(stackr, stacka, P_con + self.Drift) - lambd * norm(P_con)
-
-                        if S_con > S[mini]:
-                            # std::cout<<"| took contracted"<<std::endl;
-                            P[mini] = P_con
-                            S[mini] = S_con
-                        else:
-                            # std::cout<<"| contracting myself"<<std::endl;
-                            for i in range(4):
-                                if i != maxi:
-                                    P[i] = (P[maxi] + P[i]) * 0.5
-                                    S[i] = self.testDrift(stackr, stacka, P[i] + self.Drift) - lambd * norm(P[i])
-
-            # std::cout<<" S_ref = "<<S_ref<<std::endl;
-            mx = np.mean(P[:, 0])
-            my = np.mean(P[:, 1])
-            mz = np.mean(P[:, 2])
-
-            stdx = np.sqrt(np.sum((P[:, 0] - mx)**2)) / 4
-            stdy = np.sqrt(np.sum((P[:, 1] - my)**2)) / 4
-            stdz = np.sqrt(np.sum((P[:, 2] - mz)**2)) / 4
-
-            # std::cout<<"stdx = "<<stdx<<" ; stdy = "<<stdy<<" ; stdz = ";
-            if stdx < subpixel * vsx and stdy < subpixel * vsy and stdz < subpixel * vsz:
-                done = True
-
-        mini = np.argmin(S)
-        maxi = np.argmax(S)
-
-        return P[maxi] + self.Drift
-
-    def testDrift(self, stack1: np.ndarray, stack2: np.ndarray, D: np.ndarray) -> float:
-
-        Scale = np.array([[1.0 / self.dX, 0.0, 0.0], [0.0, 1.0 / self.dY], [0.0, 0.0, 0.0, 1.0 / self.dZ]])
-
-        U = Scale @ D
-
-        return crosscorrelateStacks(stack1, stack2, U)
-
-    def findDisplacements(self, stack_r: np.ndarray, stack_a: np.ndarray, M: Solver, lambd: float):
-
-        Srec = []
-
-        R = []
-        U = []
-
-        self.U_found = np.zeros((M.N_c, 4))
-        self.S_0 = np.zeros(M.N_c)
-
-        Scale = np.array([[1.0 / self.dX, 0.0, 0.0], [0.0, 1.0 / self.dY, 0.0], [0.0, 0.0, 1.0 / self.dZ]])
-
-        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
-
-        Trans = Scale
-        Transinv = np.linalg.inv(Trans)
-
-        tend = M.R.shape[0]
-
-        U_new = []
-        Umean = []
-
-        Stemp = 0.0
-
-        n = 0
-
-        Sd = []
-        Ud = []
-
-        """ NEW CHRISTOPH """
-
-        sgX = int(self.CFG["VB_SX"])
-        sgY = int(self.CFG["VB_SY"])
-        sgZ = int(self.CFG["VB_SZ"])
-
-        weight = np.zeros([sgX, sgY, sgZ])
-
-        for ii in range(sgX):
-            for jj in range(sgY):
-                for kk in range(sgZ):
-                    xxx = (ii - sgX / 2) * self.dX
-                    yyy = (jj - sgY / 2) * self.dY
-                    zzz = (kk - sgZ / 2) * self.dZ
-
-                    width = sgX * self.dX * 0.25
-
-                    weight[ii][jj][kk] = np.exp(-(xxx * xxx + yyy * yyy + zzz * zzz) / (2 * width))
-
-        weight /= np.mean(weight)
-
-        # sumweight=0.0;
-
-        # for(int ii=0; ii<sgX; ii++) for(int jj=0; jj<sgY; jj++) for(int kk=0; kk<sgZ; kk++) sumweight+=weight[ii][jj][kk];
-
-        # std::cout<<"sumweight = "<<sumweight<<"\n\n";
-
-        """ END NEW CHRISTOPH """
-
-        # iterate over all nodes
-        for t in range(tend):
-            # only if the node is selected as a "bead"
-            if self.vbead[t]:
-                # which method to use
-                if int(self.CFG["VB_N"]) == 1:
-                    print("finding Displacements", (np.floor((t / (tend + 0.0)) * 1000) + 0.0) / 10.0, "% S=", Stemp,
-                          "        \r", end="")
-
-                    R = Trans @ M.R[t] + scaledShift
-
-                    # get the mean from the overall drift
-                    Umean = self.Drift
-
-                    # maybe add the intial guess
-                    if bool(self.CFG["INITIALGUESS"]):
-                        Umean += self.U_guess[t]
-
-                    # transform with the scaling (µm -> pixel)
-                    Umean = Trans * Umean
-
-                    # get a substack
-                    substackr = getSubstack(stack_r, R, sgX, sgY, sgZ)
-
-                    # NEW CHRSITOPH
-                    substackr *= weight
-
-                    # get the displacement
-                    U_new = findLocalDisplacement(substackr, stack_a, R, Umean, Srec, lambd, self.CFG["subpixel"])
-                    # store the correlation
-                    self.S_0[t] = Srec[-1]
-                    Stemp = Srec[-1]
-
-                    # rescale (pixel -> µm)
-                    U_new = Transinv @ U_new
-
-                    # and store
-                    self.U_found[t] = U_new
-
-                else:
-
-                    print("finding Displacements", (np.floor((t / (tend + 0.0)) * 1000) + 0.0) / 10.0, "% S=", Stemp,
-                          "n=", n, "      \r", end="")
-
-                    Ud = []
-                    Sd = []
-
-                    imax = int(self.CFG["VB_N"]) - 1
-
-                    for i in range(imax + 1):
-                        for j in range(imax + 1):
-                            for k in range(imax + 1):
-
-                                dx = (i - (imax * 0.5)) / (imax + 1.0) * float(self.CFG["VB_SX"])
-                                dy = (j - (imax * 0.5)) / (imax + 1.0) * float(self.CFG["VB_SY"])
-                                dz = (k - (imax * 0.5)) / (imax + 1.0) * float(self.CFG["VB_SZ"])
-
-                                R = Trans * M.R[t] + scaledShift + np.array([dx, dy, dz])
-
-                                Umean = self.Drift
-
-                                Umean = Trans @ Umean
-
-                                substackr = self.getSubstack(stack_r, R)
-                                U_new = self.findLocalDisplacement(substackr, stack_a, R, Umean, Srec, lambd)
-                                Stemp = Srec[-1]
-
-                                U_new = Transinv @ U_new
-
-                                if Stemp > float(self.CFG["VB_MINMATCH"]):
-                                    Ud.append(U_new)
-                                    Sd.append(Stemp)
-
-                    if Sd.size() > 0:
-
-                        U_new = np.array([0.0, 0.0, 0.0])
-                        Stemp = 0.0
-
-                        for it in Sd:
-                            Stemp += it
-                        for it in Ud:
-                            U_new += it
-
-                        U_new = U_new * (1.0 / len(Sd))
-                        Stemp = Stemp * (1.0 / len(Sd))
-
-                        n = len(Sd)
-
-                    else:
-
-                        U_new = np.array([0.0, 0.0, 0.0])
-                        Stemp = -1.0
-                        n = 0
-
-                    self.S_0[t] = Srec[-1]
-                    self.U_found[t] = U_new
-
-    def refineDisplacements(self, stack_r: np.ndarray, stack_a: np.ndarray, M: Solver, lambd: float):
-
-        Srec = []
-
-        Scale = np.array([[1.0 / self.dX, 0.0, 0.0], [0.0, 1.0 / self.dY, 0.0], [0.0, 0.0, 1.0 / self.dZ]])
-
-        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
-
-        Trans = Scale
-
-        Transinv = np.linalg.inv(Trans)
-
-        indices = []
-        Svalues = []
-
-        vbeadcount = 0
-
-        for c in range(M.N_c):
-            if self.vbead[c]:
-                indices.append(c)
-                Svalues.append(self.S_0[c])
-                vbeadcount += 1
-
-        # TODO BubbleSort_IVEC_using_associated_dVals(indices,Svalues)
-
-        Nrenew = np.floor(vbeadcount)
-
-        it = []
-
-        Umean = []
-        U_new = []
-        R = []
-        Stemp = 0.0
-
-        for i in range(Nrenew):
-            print("refining displacements:", (np.floor((i / (Nrenew + 0.0)) * 1000) + 0.0) / 10.0, "%     S=", Stemp,
-                  "           \r", end="")
-
-            c = indices[i]
-            cccount = 0
-
-            Umean = np.array([0.0, 0.0, 0.0])
-
-            for it in M.connections:
-                cc = it
-
-                if self.vbead[cc]:
-                    Umean += self.U_found[cc]
-                    cccount += 1
-
-            if cccount > 0:
-                Umean = Umean / (cccount + 0.0)
-
-                R = (Trans @ ((M.R[c])) + scaledShift)
-                Umean = (Trans @ ((Umean)))
-
-                substackr = getSubstack(stack_r, R)
-
-                U_new = findLocalDisplacement(substackr, stack_a, R, Umean, Srec, lambd)
-                self.S_0[c] = Srec[-1]
-                substacka = getSubstack(stack_a, R)
-                U_new -= findLocalDisplacement(substacka, stack_r, R + Umean, Umean * (-1.0), Srec, lambd)
-                self.S_0[c] += Srec[-1]
-
-                self.S_0[c] *= 0.5
-
-                U_new = Transinv @ U_new * 0.5
-
-                self.U_found[c] = U_new
-
-                Stemp = self.S_0[c]
-
-    def _computeRegularizationAAndb(self, M, alpha):
-        KA = M.K_glo.multiply(np.repeat(self.localweight * alpha, 3)[None, :])
-        self.KAK = KA @ M.K_glo
-        self.A = self.I + self.KAK
-
-        self.b = (KA @ M.f_glo.ravel()).reshape(M.f_glo.shape)
-
-        index = M.var * self.vbead
-        self.b[index] += self.U_found[index] - M.U[index]
-
-    def _recordRegularizationStatus(self, relrecname, M, relrec):
-        alpha = self.CFG["ALPHA"]
-
-        indices = M.var & self.vbead
-        btemp = self.U_found[indices] - M.U[indices]
-        uuf2 = np.sum(btemp ** 2)
-        suuf = np.sum(np.linalg.norm(btemp, axis=1))
-        bcount = btemp.shape[0]
-
-        u2 = np.sum(M.U[M.var] ** 2)
-
-        f = np.zeros((M.N_c, 3))
-        f[M.var] = M.f_glo[M.var]
-
-        ff = np.sum(np.sum(f ** 2, axis=1) * self.localweight * M.var)
-
-        L = alpha * ff + uuf2
-
-        print("|u-uf|^2 =", uuf2, "\t\tperbead=", suuf / bcount)
-        print("|w*f|^2  =", ff, "\t\t|u|^2 =", u2)
-        print("L = |u-uf|^2 + lambda*|w*f|^2 = ", L)
-
-        relrec.append((L, uuf2, ff))
-
-        np.savetxt(relrecname, relrec)
-
-    def regularize(self, M, stepper=0.33, REG_SOLVER_PRECISION=1e-18, i_max=100, rel_conv_crit=0.01, alpha=1.0,
-                   method="huber", relrecname=None):
-        self.I = ssp.lil_matrix((self.vbead.shape[0] * 3, self.vbead.shape[0] * 3))
-        self.I.setdiag(np.repeat(self.vbead, 3))
-
-        self.M = M
-
-        # if the shape tensors are not valid, calculate them
-        if self.M.Phi_valid is False:
-            self.M._computePhi()
-
-        # if the connections are not valid, calculate them
-        if self.M.connections_valid is False:
-            self.M._computeConnections()
-
-        self.localweight = np.ones(M.N_c)
-
-        # update the forces on each tetrahedron and the global stiffness tensor
-        print("going to update glo f and K")
-        M._updateGloFAndK()
-
-        # log and store values (if a target file was provided)
-        if relrecname is not None:
-            relrec = []
-            self._recordRegularizationStatus(relrecname, M, relrec)
-
-        print("check before relax !")
-        # start the iteration
-        for i in range(i_max):
-            # compute the weight matrix
-            if method != "normal":
-                self.updateLocalWeigth(M, method)
-
-            # compute A and b for the linear equation that solves the regularisation problem
-            self._computeRegularizationAAndb(M, alpha)
-
-            # get and apply the displacements that solve the regularisation term
-            uu = self._solve_regularization_CG(M, stepper, REG_SOLVER_PRECISION)
-
-            # update the forces on each tetrahedron and the global stiffness tensor
-            M._updateGloFAndK()
-
-            print("Round", i + 1, " |du|=", uu)
-
-            # log and store values (if a target file was provided)
-            if relrecname is not None:
-                self._recordRegularizationStatus(relrecname, M, relrec)
-
-            # if we have passed 6 iterations calculate average and std
-            if i > 6:
-                # calculate the average energy over the last 6 iterations
-                last_Ls = np.array(relrec)[:-6:-1, 1]
-                Lmean = np.mean(last_Ls)
-                Lstd = np.std(last_Ls) / np.sqrt(5)  # the original formula just had /N instead of /sqrt(N)
-
-                # if the iterations converge, stop the iteration
-                if Lstd / Lmean < rel_conv_crit:
-                    break
-
-        return relrec
-
-    def _solve_regularization_CG(self, M, stepper=0.33, REG_SOLVER_PRECISION=1e-18):
-        """
-        Solve the displacements from the current stiffness tensor using conjugate gradient.
-        """
-
-        # solve the conjugate gradient which solves the equation A x = b for x
-        # where A is (I - KAK) (K: stiffness matrix, A: weight matrix) and b is (u_meas - u - KAf)
-        uu = cg(self.A, self.b.flatten(), maxiter=25 * int(pow(M.N_c, 0.33333) + 0.5),
-                tol=M.N_c * REG_SOLVER_PRECISION).reshape((M.N_c, 3))
-
-        # add the new displacements to the stored displacements
-        self.M.U += uu * stepper
-        # sum the applied displacements
-        du = np.sum(uu ** 2) * stepper * stepper
-
-        # return the total applied displacement
-        return np.sqrt(du / M.N_c)
-
-    def storeUfound(self, Uname, Sname):
-        np.savetxt(Uname, self.U_found)
-        np.savetxt(Sname, self.S_0)
-
-    def storeRfound(self, Rname):
-        np.savetxt(Rname, self.R_found)
-
-    def storeLocalweights(self, wname):
-        np.savetxt(wname, self.localweight)
+import time
+
+import numpy as np
+import scipy.sparse as ssp
+
+from saenopy.solver import Solver
+from saenopy.conjugateGradient import cg
+from saenopy.unused.stack3DHelper import crosscorrelateStacks, getSubstack, findLocalDisplacement
+
+
+class timeit:
+
+    def __init__(self, name):
+        self.name = name
+
+    def __enter__(self):
+        self.start = time.time()
+        print("Start", self.name)
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        print("End", self.name, "%.3fs" % (time.time() - self.start))
+
+
+class IA:
+    def __init__(self, A, I):
+        self.A = A
+        self.I = I
+
+    def __matmul__(self, other):
+        return self.I * other + self.A @ other
+
+
+def norm(x):
+    return np.sum(x**2)
+
+
+class VirtualBeads:
+    def __init__(self, CFG, ssX=None, ssY=None, ssZ=None, ddX=None, ddY=None, ddZ=None):
+        self.CFG = CFG
+        self.sX = ssX
+        self.sY = ssY
+        self.sZ = ssZ
+        self.dX = ddX
+        self.dY = ddY
+        self.dZ = ddZ
+
+        self.S_0 = []
+
+        self.U_found = []
+        self.R_found = []
+        self.U_guess = []
+
+        self.I = None
+        self.Itrans = None
+        self.ItransI = None
+
+        self.vbead = []
+        self.outofstack = []
+
+        self.u_x = []
+        self.u_y = []
+        self.u_z = []
+
+        self.localweight = []
+        self.conconnections = None
+        self.oldconconnections = None
+        self.b = []
+
+        self.Drift = np.array([0, 0, 0])
+
+    def allBeads(self, M):
+        thresh = self.CFG["VB_SX"] * self.dX + 2.0 * self.CFG["DRIFT_STEP"]
+
+        self.vbead = np.zeros(M.N_c, dtype=bool)
+
+        Scale = np.eye(3) * np.array([self.dX, self.dY, self.dZ])
+
+        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
+
+        Trans = Scale
+
+        for t in range(M.N_c):
+            R = Trans @ M.R[t] + scaledShift
+
+            if thresh < R[0] < (self.sX - thresh) and \
+                    thresh < R[1] < (self.sY - thresh) and \
+                    thresh < R[2] < (self.sZ - thresh):
+                self.vbead[t] = True
+
+    def computeOutOfStack(self, M):
+        thresh = self.CFG["VB_SX"] * self.dX + 2.0 * self.CFG["DRIFT_STEP"]
+
+        self.outofstack = np.array(M.N_c, dtype=bool)
+
+        Scale = np.eye(3) * np.array([self.dX, self.dY, self.dZ])
+
+        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
+
+        Trans = Scale
+
+        for t in range(M.N_c):
+            R = Trans @ M.R[t] + scaledShift
+
+            if thresh < R[0] < (self.sX - thresh) and \
+                    thresh < R[1] < (self.sY - thresh) and \
+                    thresh < R[2] < (self.sZ - thresh):
+                self.outofstack[t] = False
+
+    def loadVbeads(self, VBname):
+        vbead_temp = np.loadtxt(VBname)
+
+        self.vbead = vbead_temp[:, 0] > 0.5
+
+    def loadGuess(self, M, ugname):
+        from .loadHelpers import loadBoundaryConditions
+        var, U, f_ext = loadBoundaryConditions(ugname)
+        M.var = var
+        M.f_ext = f_ext
+        self.U_guess = U
+        M._computeConnections()
+
+    def updateLocalWeigth(self, M, method):
+
+        self.localweight[:] = 1
+
+        Fvalues = np.linalg.norm(M.f_glo, axis=1)
+        Fmedian = np.median(Fvalues[M.var])
+
+        if method == "singlepoint":
+            self.localweight[int(self.CFG["REG_FORCEPOINT"])] = 1.0e-10
+
+        if method == "bisquare":
+            k = 4.685
+
+            index = Fvalues < k * Fmedian
+            self.localweight[index * M.var] *= (1 - (Fvalues / k / Fmedian) * (Fvalues / k / Fmedian)) * (
+                    1 - (Fvalues / k / Fmedian) * (Fvalues / k / Fmedian))
+            self.localweight[~index * M.var] *= 1e-10
+
+        if method == "cauchy":
+            k = 2.385
+
+            if Fmedian > 0:
+                self.localweight[M.var] *= 1.0 / (1.0 + np.power((Fvalues / k / Fmedian), 2.0))
+            else:
+                self.localweight *= 1.0
+
+        if method == "huber":
+            k = 1.345
+
+            index = (Fvalues > (k * Fmedian)) * M.var
+            self.localweight[index] = k * Fmedian / Fvalues[index]
+
+        index = self.localweight < 1e-10
+        self.localweight[index * M.var] = 1e-10
+
+        counter = np.sum(1.0 - self.localweight[M.var])
+        counterall = np.sum(M.var)
+
+        print("total weight: ", counter, "/", counterall)
+
+    def loadUfound(self, Uname, Sname):
+        self.U_found = np.loadtxt(Uname)
+        self.S_0 = np.loadtxt(Sname)
+        self.vbead = self.S_0 > 0.7
+
+    def computeConconnections(self, M):
+        """
+        conconections seem to be the indirect connections e.g. A->B->C
+        this means a has an indirect connection (or 2. order connection) to c
+        """
+        self.conconnections = []
+        for c1 in range(M.N_c):
+            self.conconnections.append(set())
+
+        for c1 in range(M.N_c):
+            for c2 in M.connections[c1]:
+                for c3 in M.connections[c2]:
+                    if c3 not in self.conconnections[c1]:
+                        self.conconnections[c1].add(c3)
+
+    def computeConconnections_Laplace(self, M):
+        """
+        seems to adanve the order of which connections to look at
+        """
+        self.conconnections = []
+        self.oldconconnections = []
+        for c1 in range(M.N_c):
+            self.oldconconnections[c1] = self.conconnections[c1]
+            self.conconnections.append(set())
+
+        for c1 in range(M.N_c):
+            for c2 in self.oldconconnections[c1]:
+                for c3 in self.oldconconnections[c2]:
+                    if c3 not in self.conconnections[c1]:
+                        self.conconnections[c1].add(c3)
+
+    def substractMedianDisplacements(self):
+        index = np.abs(self.U_found) > 0.01 * self.CFG["VOXELSIZEX"]
+        u_median = np.median(self.U_found[index], axis=0)
+        print("Median displacement calculated to", u_median)
+
+        self.U_found -= u_median
+
+    def findDriftCoarse(self, stackr: np.ndarray, stacka: np.ndarray, abs_range: float, step: float) -> np.ndarray:
+
+        Smax = -1.0
+        best_shift = np.array([0, 0, 0])
+
+        # iterate over all shifts in the rage and step and find the best correlation
+        for dx in np.arange(-abs_range, abs_range, step):
+            for dy in np.arange(-abs_range, abs_range, step):
+                for dz in np.arange(-abs_range, abs_range, step):
+                    shift = np.array([dx, dy, dz])
+
+                    # get the correlation for this shift
+                    Stemp = self.testDrift(stackr, stacka, shift)
+
+                    # if it is better than the previous best, store it
+                    if Stemp > Smax:
+                        best_shift = shift
+                        Smax = Stemp
+
+        # return the best shift
+        return best_shift
+
+    def findDrift(self, stackr: np.ndarray, stacka: np.ndarray) -> np.ndarray:
+
+        lambd = 0.0
+
+        hinit = float(self.CFG["DRIFT_STEP"])
+        subpixel = float(self.CFG["SUBPIXEL"])
+
+        vsx = float(self.CFG["VOXELSIZEX"])
+        vsy = float(self.CFG["VOXELSIZEY"])
+        vsz = float(self.CFG["VOXELSIZEZ"])
+
+        P = np.array([
+            [1, 1, 1],
+            [-1, -1, 1],
+            [-1, 1, -1],
+            [1, -1, -1],
+        ]) * hinit
+
+        S = [
+            self.testDrift(stackr, stacka, P[0] + self.Drift) - lambd * norm(P[0]),
+            self.testDrift(stackr, stacka, P[1] + self.Drift) - lambd * norm(P[1]),
+            self.testDrift(stackr, stacka, P[2] + self.Drift) - lambd * norm(P[2]),
+            self.testDrift(stackr, stacka, P[3] + self.Drift) - lambd * norm(P[3]),
+        ]
+
+        # std::cout<<S[0]<<" "<<S[1]<<" "<<S[2]<<" "<<S[3]<<" \n";
+        done = False
+        for ii in range(100000):
+            if done:
+                break
+
+            mini = np.argmin(S)
+            maxi = np.argmax(S)
+
+            # std::cout<<"| new cycle mini = "<<mini<<std::endl;
+            # reflect
+            P_plane = np.array([0.0, 0.0, 0.0])
+            for i in range(4):
+                if i != mini:
+                    P_plane += P[i]
+            P_plane /= 3
+
+            P_ref = P[mini] + (P_plane - P[mini]) * 2.0
+
+            S_ref = self.testDrift(stackr, stacka, P_ref + self.Drift) - lambd * norm(P_ref)
+
+            if S_ref > S[maxi]:
+                # expand
+                # std::cout<<"| expanding "<<std::endl;
+                P_exp = P[mini] + (P_plane - P[mini]) * 3.0
+                S_exp = self.testDrift(stackr, stacka, P_exp + self.Drift) - lambd * norm(P_exp)
+
+                if S_exp > S_ref:
+                    # std::cout<<"| took expanded "<<std::endl;
+                    P[mini] = P_exp
+                    S[mini] = S_exp
+
+                else:
+                    # std::cout<<"| took reflected (expanded was worse)"<<std::endl;
+                    P[mini] = P_ref
+                    S[mini] = S_ref
+            else:
+                bsw = False
+                for i in range(4):
+                    if i != mini:
+                        if S_ref > S[i]:
+                            bsw = True
+
+                if bsw:
+                    # std::cout<<"| took reflected (better than second worst)"<<std::endl;
+                    P[mini] = P_ref
+                    S[mini] = S_ref
+
+                else:
+                    if S_ref > S[maxi]:
+                        # std::cout<<"| took reflected (not better than second worst)"<<std::endl;
+                        P[mini] = P_ref
+                        S[mini] = S_ref
+                    else:
+                        P_con = P[mini] + (P_plane - P[mini]) * 0.5
+                        S_con = self.testDrift(stackr, stacka, P_con + self.Drift) - lambd * norm(P_con)
+
+                        if S_con > S[mini]:
+                            # std::cout<<"| took contracted"<<std::endl;
+                            P[mini] = P_con
+                            S[mini] = S_con
+                        else:
+                            # std::cout<<"| contracting myself"<<std::endl;
+                            for i in range(4):
+                                if i != maxi:
+                                    P[i] = (P[maxi] + P[i]) * 0.5
+                                    S[i] = self.testDrift(stackr, stacka, P[i] + self.Drift) - lambd * norm(P[i])
+
+            # std::cout<<" S_ref = "<<S_ref<<std::endl;
+            mx = np.mean(P[:, 0])
+            my = np.mean(P[:, 1])
+            mz = np.mean(P[:, 2])
+
+            stdx = np.sqrt(np.sum((P[:, 0] - mx)**2)) / 4
+            stdy = np.sqrt(np.sum((P[:, 1] - my)**2)) / 4
+            stdz = np.sqrt(np.sum((P[:, 2] - mz)**2)) / 4
+
+            # std::cout<<"stdx = "<<stdx<<" ; stdy = "<<stdy<<" ; stdz = ";
+            if stdx < subpixel * vsx and stdy < subpixel * vsy and stdz < subpixel * vsz:
+                done = True
+
+        mini = np.argmin(S)
+        maxi = np.argmax(S)
+
+        return P[maxi] + self.Drift
+
+    def testDrift(self, stack1: np.ndarray, stack2: np.ndarray, D: np.ndarray) -> float:
+
+        Scale = np.array([[1.0 / self.dX, 0.0, 0.0], [0.0, 1.0 / self.dY], [0.0, 0.0, 0.0, 1.0 / self.dZ]])
+
+        U = Scale @ D
+
+        return crosscorrelateStacks(stack1, stack2, U)
+
+    def findDisplacements(self, stack_r: np.ndarray, stack_a: np.ndarray, M: Solver, lambd: float):
+
+        Srec = []
+
+        R = []
+        U = []
+
+        self.U_found = np.zeros((M.N_c, 4))
+        self.S_0 = np.zeros(M.N_c)
+
+        Scale = np.array([[1.0 / self.dX, 0.0, 0.0], [0.0, 1.0 / self.dY, 0.0], [0.0, 0.0, 1.0 / self.dZ]])
+
+        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
+
+        Trans = Scale
+        Transinv = np.linalg.inv(Trans)
+
+        tend = M.R.shape[0]
+
+        U_new = []
+        Umean = []
+
+        Stemp = 0.0
+
+        n = 0
+
+        Sd = []
+        Ud = []
+
+        """ NEW CHRISTOPH """
+
+        sgX = int(self.CFG["VB_SX"])
+        sgY = int(self.CFG["VB_SY"])
+        sgZ = int(self.CFG["VB_SZ"])
+
+        weight = np.zeros([sgX, sgY, sgZ])
+
+        for ii in range(sgX):
+            for jj in range(sgY):
+                for kk in range(sgZ):
+                    xxx = (ii - sgX / 2) * self.dX
+                    yyy = (jj - sgY / 2) * self.dY
+                    zzz = (kk - sgZ / 2) * self.dZ
+
+                    width = sgX * self.dX * 0.25
+
+                    weight[ii][jj][kk] = np.exp(-(xxx * xxx + yyy * yyy + zzz * zzz) / (2 * width))
+
+        weight /= np.mean(weight)
+
+        # sumweight=0.0;
+
+        # for(int ii=0; ii<sgX; ii++) for(int jj=0; jj<sgY; jj++) for(int kk=0; kk<sgZ; kk++) sumweight+=weight[ii][jj][kk];
+
+        # std::cout<<"sumweight = "<<sumweight<<"\n\n";
+
+        """ END NEW CHRISTOPH """
+
+        # iterate over all nodes
+        for t in range(tend):
+            # only if the node is selected as a "bead"
+            if self.vbead[t]:
+                # which method to use
+                if int(self.CFG["VB_N"]) == 1:
+                    print("finding Displacements", (np.floor((t / (tend + 0.0)) * 1000) + 0.0) / 10.0, "% S=", Stemp,
+                          "        \r", end="")
+
+                    R = Trans @ M.R[t] + scaledShift
+
+                    # get the mean from the overall drift
+                    Umean = self.Drift
+
+                    # maybe add the intial guess
+                    if bool(self.CFG["INITIALGUESS"]):
+                        Umean += self.U_guess[t]
+
+                    # transform with the scaling (µm -> pixel)
+                    Umean = Trans * Umean
+
+                    # get a substack
+                    substackr = getSubstack(stack_r, R, sgX, sgY, sgZ)
+
+                    # NEW CHRSITOPH
+                    substackr *= weight
+
+                    # get the displacement
+                    U_new = findLocalDisplacement(substackr, stack_a, R, Umean, Srec, lambd, self.CFG["subpixel"])
+                    # store the correlation
+                    self.S_0[t] = Srec[-1]
+                    Stemp = Srec[-1]
+
+                    # rescale (pixel -> µm)
+                    U_new = Transinv @ U_new
+
+                    # and store
+                    self.U_found[t] = U_new
+
+                else:
+
+                    print("finding Displacements", (np.floor((t / (tend + 0.0)) * 1000) + 0.0) / 10.0, "% S=", Stemp,
+                          "n=", n, "      \r", end="")
+
+                    Ud = []
+                    Sd = []
+
+                    imax = int(self.CFG["VB_N"]) - 1
+
+                    for i in range(imax + 1):
+                        for j in range(imax + 1):
+                            for k in range(imax + 1):
+
+                                dx = (i - (imax * 0.5)) / (imax + 1.0) * float(self.CFG["VB_SX"])
+                                dy = (j - (imax * 0.5)) / (imax + 1.0) * float(self.CFG["VB_SY"])
+                                dz = (k - (imax * 0.5)) / (imax + 1.0) * float(self.CFG["VB_SZ"])
+
+                                R = Trans * M.R[t] + scaledShift + np.array([dx, dy, dz])
+
+                                Umean = self.Drift
+
+                                Umean = Trans @ Umean
+
+                                substackr = self.getSubstack(stack_r, R)
+                                U_new = self.findLocalDisplacement(substackr, stack_a, R, Umean, Srec, lambd)
+                                Stemp = Srec[-1]
+
+                                U_new = Transinv @ U_new
+
+                                if Stemp > float(self.CFG["VB_MINMATCH"]):
+                                    Ud.append(U_new)
+                                    Sd.append(Stemp)
+
+                    if Sd.size() > 0:
+
+                        U_new = np.array([0.0, 0.0, 0.0])
+                        Stemp = 0.0
+
+                        for it in Sd:
+                            Stemp += it
+                        for it in Ud:
+                            U_new += it
+
+                        U_new = U_new * (1.0 / len(Sd))
+                        Stemp = Stemp * (1.0 / len(Sd))
+
+                        n = len(Sd)
+
+                    else:
+
+                        U_new = np.array([0.0, 0.0, 0.0])
+                        Stemp = -1.0
+                        n = 0
+
+                    self.S_0[t] = Srec[-1]
+                    self.U_found[t] = U_new
+
+    def refineDisplacements(self, stack_r: np.ndarray, stack_a: np.ndarray, M: Solver, lambd: float):
+
+        Srec = []
+
+        Scale = np.array([[1.0 / self.dX, 0.0, 0.0], [0.0, 1.0 / self.dY, 0.0], [0.0, 0.0, 1.0 / self.dZ]])
+
+        scaledShift = np.array([self.sX / 2, self.sY / 2, self.sZ / 2])
+
+        Trans = Scale
+
+        Transinv = np.linalg.inv(Trans)
+
+        indices = []
+        Svalues = []
+
+        vbeadcount = 0
+
+        for c in range(M.N_c):
+            if self.vbead[c]:
+                indices.append(c)
+                Svalues.append(self.S_0[c])
+                vbeadcount += 1
+
+        # TODO BubbleSort_IVEC_using_associated_dVals(indices,Svalues)
+
+        Nrenew = np.floor(vbeadcount)
+
+        it = []
+
+        Umean = []
+        U_new = []
+        R = []
+        Stemp = 0.0
+
+        for i in range(Nrenew):
+            print("refining displacements:", (np.floor((i / (Nrenew + 0.0)) * 1000) + 0.0) / 10.0, "%     S=", Stemp,
+                  "           \r", end="")
+
+            c = indices[i]
+            cccount = 0
+
+            Umean = np.array([0.0, 0.0, 0.0])
+
+            for it in M.connections:
+                cc = it
+
+                if self.vbead[cc]:
+                    Umean += self.U_found[cc]
+                    cccount += 1
+
+            if cccount > 0:
+                Umean = Umean / (cccount + 0.0)
+
+                R = (Trans @ ((M.R[c])) + scaledShift)
+                Umean = (Trans @ ((Umean)))
+
+                substackr = getSubstack(stack_r, R)
+
+                U_new = findLocalDisplacement(substackr, stack_a, R, Umean, Srec, lambd)
+                self.S_0[c] = Srec[-1]
+                substacka = getSubstack(stack_a, R)
+                U_new -= findLocalDisplacement(substacka, stack_r, R + Umean, Umean * (-1.0), Srec, lambd)
+                self.S_0[c] += Srec[-1]
+
+                self.S_0[c] *= 0.5
+
+                U_new = Transinv @ U_new * 0.5
+
+                self.U_found[c] = U_new
+
+                Stemp = self.S_0[c]
+
+    def _computeRegularizationAAndb(self, M, alpha):
+        KA = M.K_glo.multiply(np.repeat(self.localweight * alpha, 3)[None, :])
+        self.KAK = KA @ M.K_glo
+        self.A = self.I + self.KAK
+
+        self.b = (KA @ M.f_glo.ravel()).reshape(M.f_glo.shape)
+
+        index = M.var * self.vbead
+        self.b[index] += self.U_found[index] - M.U[index]
+
+    def _recordRegularizationStatus(self, relrecname, M, relrec):
+        alpha = self.CFG["ALPHA"]
+
+        indices = M.var & self.vbead
+        btemp = self.U_found[indices] - M.U[indices]
+        uuf2 = np.sum(btemp ** 2)
+        suuf = np.sum(np.linalg.norm(btemp, axis=1))
+        bcount = btemp.shape[0]
+
+        u2 = np.sum(M.U[M.var] ** 2)
+
+        f = np.zeros((M.N_c, 3))
+        f[M.var] = M.f_glo[M.var]
+
+        ff = np.sum(np.sum(f ** 2, axis=1) * self.localweight * M.var)
+
+        L = alpha * ff + uuf2
+
+        print("|u-uf|^2 =", uuf2, "\t\tperbead=", suuf / bcount)
+        print("|w*f|^2  =", ff, "\t\t|u|^2 =", u2)
+        print("L = |u-uf|^2 + lambda*|w*f|^2 = ", L)
+
+        relrec.append((L, uuf2, ff))
+
+        np.savetxt(relrecname, relrec)
+
+    def regularize(self, M, stepper=0.33, REG_SOLVER_PRECISION=1e-18, i_max=100, rel_conv_crit=0.01, alpha=1.0,
+                   method="huber", relrecname=None):
+        self.I = ssp.lil_matrix((self.vbead.shape[0] * 3, self.vbead.shape[0] * 3))
+        self.I.setdiag(np.repeat(self.vbead, 3))
+
+        self.M = M
+
+        # if the shape tensors are not valid, calculate them
+        if self.M.Phi_valid is False:
+            self.M._computePhi()
+
+        # if the connections are not valid, calculate them
+        if self.M.connections_valid is False:
+            self.M._computeConnections()
+
+        self.localweight = np.ones(M.N_c)
+
+        # update the forces on each tetrahedron and the global stiffness tensor
+        print("going to update glo f and K")
+        M._updateGloFAndK()
+
+        # log and store values (if a target file was provided)
+        if relrecname is not None:
+            relrec = []
+            self._recordRegularizationStatus(relrecname, M, relrec)
+
+        print("check before relax !")
+        # start the iteration
+        for i in range(i_max):
+            # compute the weight matrix
+            if method != "normal":
+                self.updateLocalWeigth(M, method)
+
+            # compute A and b for the linear equation that solves the regularisation problem
+            self._computeRegularizationAAndb(M, alpha)
+
+            # get and apply the displacements that solve the regularisation term
+            uu = self._solve_regularization_CG(M, stepper, REG_SOLVER_PRECISION)
+
+            # update the forces on each tetrahedron and the global stiffness tensor
+            M._updateGloFAndK()
+
+            print("Round", i + 1, " |du|=", uu)
+
+            # log and store values (if a target file was provided)
+            if relrecname is not None:
+                self._recordRegularizationStatus(relrecname, M, relrec)
+
+            # if we have passed 6 iterations calculate average and std
+            if i > 6:
+                # calculate the average energy over the last 6 iterations
+                last_Ls = np.array(relrec)[:-6:-1, 1]
+                Lmean = np.mean(last_Ls)
+                Lstd = np.std(last_Ls) / np.sqrt(5)  # the original formula just had /N instead of /sqrt(N)
+
+                # if the iterations converge, stop the iteration
+                if Lstd / Lmean < rel_conv_crit:
+                    break
+
+        return relrec
+
+    def _solve_regularization_CG(self, M, stepper=0.33, REG_SOLVER_PRECISION=1e-18):
+        """
+        Solve the displacements from the current stiffness tensor using conjugate gradient.
+        """
+
+        # solve the conjugate gradient which solves the equation A x = b for x
+        # where A is (I - KAK) (K: stiffness matrix, A: weight matrix) and b is (u_meas - u - KAf)
+        uu = cg(self.A, self.b.flatten(), maxiter=25 * int(pow(M.N_c, 0.33333) + 0.5),
+                tol=M.N_c * REG_SOLVER_PRECISION).reshape((M.N_c, 3))
+
+        # add the new displacements to the stored displacements
+        self.M.U += uu * stepper
+        # sum the applied displacements
+        du = np.sum(uu ** 2) * stepper * stepper
+
+        # return the total applied displacement
+        return np.sqrt(du / M.N_c)
+
+    def storeUfound(self, Uname, Sname):
+        np.savetxt(Uname, self.U_found)
+        np.savetxt(Sname, self.S_0)
+
+    def storeRfound(self, Rname):
+        np.savetxt(Rname, self.R_found)
+
+    def storeLocalweights(self, wname):
+        np.savetxt(wname, self.localweight)
```

### Comparing `saenopy-0.8.0/saenopy/buildBeams.py` & `saenopy-0.9.0/saenopy/buildBeams.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/conjugateGradient.py` & `saenopy-0.9.0/saenopy/conjugateGradient.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/gui/gui_classes.py` & `saenopy-0.9.0/saenopy/gui/common/gui_classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 import sys
-
-# Setting the Qt bindings for QtPy
-import os
-
-import pandas as pd
 import qtawesome as qta
-
-os.environ["QT_API"] = "pyqt5"
-
 from qtpy import QtCore, QtWidgets, QtGui
 
-import numpy as np
-
-from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-import imageio
-from qimage2ndarray import array2qimage
 import matplotlib.pyplot as plt
-import glob
-import imageio
-import threading
-import glob
-import re
+
+from saenopy.gui.common import QtShortCuts
 
 
 def trace_function(func, data):
     import time
     last_time = 0
     def trace_lines(frame, event, arg):
         nonlocal t, last_time
@@ -55,30 +39,16 @@
             return trace_lines
         return None
 
     TRACE_INTO = [func]
 
     sys.settrace(trace_calls)
 
-if QtCore.qVersion() >= "5.":
-    from matplotlib.backends.backend_qt5agg import (
-        FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
-else:
-    from matplotlib.backends.backend_qt4agg import (
-        FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
-from matplotlib.figure import Figure
-
-import urllib
-from pathlib import Path
 
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
+from matplotlib.figure import Figure
 
 import ctypes
 
 from qtpy import API_NAME as QT_API_NAME
 if QT_API_NAME.startswith("PyQt4"):
     from matplotlib.backends.backend_qt4agg import FigureCanvasQTAgg as Canvas
     from matplotlib.backends.backend_qt4agg import FigureManager
@@ -121,50 +91,55 @@
         _pylab_helpers.Gcf.set_active(self.manager)
 
     def setActive(self):
         from matplotlib import _pylab_helpers
         self.manager._cidgcf = self.figure
         _pylab_helpers.Gcf.set_active(self.manager)
 
+
 def execute(func, *args, **kwargs):
     func(*args, **kwargs)
     import inspect
     code_lines = inspect.getsource(func).split("\n")[1:]
     indent = len(code_lines[0]) - len(code_lines[0].lstrip())
     code = "\n".join(line[indent:] for line in code_lines)
     for key, value in kwargs.items():
         if isinstance(value, str):
             code = code.replace(key, "'"+value+"'")
         else:
             code = code.replace(key, str(value))
     code = code.replace("self.canvas.draw()", "plt.show()")
     return code
 
+
 def kill_thread(thread):
     """
     thread: a threading.Thread object
     """
     thread_id = thread.ident
     res = ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, ctypes.py_object(SystemExit))
     if res > 1:
         ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, 0)
         print('Exception raise failure')
 
+
 class QHLine(QtWidgets.QFrame):
     def __init__(self):
         super().__init__()
         self.setFrameShape(QtWidgets.QFrame.HLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
 
+
 class QVLine(QtWidgets.QFrame):
     def __init__(self):
         super().__init__()
         self.setFrameShape(QtWidgets.QFrame.VLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
 
+
 class Spoiler(QtWidgets.QWidget):
     def __init__(self, parent=None, title='', animationDuration=300):
         """
         References:
             # Adapted from c++ version
             http://stackoverflow.com/questions/32476006/how-to-make-an-expandable-collapsable-section-widget-in-qt
         """
@@ -236,15 +211,15 @@
         contentAnimation.setStartValue(0)
         contentAnimation.setEndValue(contentHeight)
 
 
 class CheckAbleGroup(QtWidgets.QWidget, QtShortCuts.EnterableLayout):
     value_changed = QtCore.Signal(bool)
     main_layout = None
-    def __init__(self, parent=None, title='', animationDuration=300):
+    def __init__(self, parent=None, title='', animationDuration=300, url=None):
         super().__init__(parent=parent)
 
         self.headerLine = QtWidgets.QFrame()
         self.checkbox = QtWidgets.QCheckBox()
         self.toggleButton = QtWidgets.QToolButton()
         self.mainLayout = QtWidgets.QGridLayout()
 
@@ -257,14 +232,22 @@
                 self.label.setStyleSheet("QPushButton { border: none; }")
                 self.label.clicked.connect(self.toggle)
 
                 headerLine = QtWidgets.QFrame().addToLayout()
                 headerLine.setFrameShape(QtWidgets.QFrame.HLine)
                 headerLine.setFrameShadow(QtWidgets.QFrame.Sunken)
                 headerLine.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Maximum)
+
+                #QtShortCuts.current_layout.addStretch()
+                if url is not None:
+                    self.label2 = QtWidgets.QPushButton(qta.icon("fa5s.question"), "").addToLayout()
+                    self.label2.setToolTip("open the documentation in the browser")
+                    #self.label2.setMaximumWidth(30)
+                    self.label2.setStyleSheet("QPushButton { border: none; background: none; }")
+                    self.label2.clicked.connect(lambda x: QtGui.QDesktopServices.openUrl(QtCore.QUrl(url)))
             self.child_widget = QtWidgets.QWidget().addToLayout()
         self.layout = self
         self.value = self.toggleButton.value
         #self.setValue = self.toggleButton.setValue
         self.valueChanged = self.toggleButton.valueChanged
         self.toggleButton.valueChanged.connect(self.changedActive)
 
@@ -294,34 +277,47 @@
     def addLayout(self, layout):
         if self.main_layout is None:
             self.setLayout(layout)
         else:
             self.child_widget.setLayout(layout)
         return layout
 
+
 class ListWidget(QtWidgets.QListWidget):
     itemSelectionChanged2 = QtCore.Signal()
     itemChanged2 = QtCore.Signal()
     addItemClicked = QtCore.Signal()
+    signal_act_copy_clicked = QtCore.Signal()
+    signal_act_paste_clicked = QtCore.Signal()
+    signal_act_paths_clicked = QtCore.Signal()
 
     data = []
-    def __init__(self, layout, editable=False, add_item_button=False, color_picker=False):
+    def __init__(self, layout, editable=False, add_item_button=False, color_picker=False, copy_params=False, allow_paste_callback=None):
         super().__init__()
         layout.addWidget(self)
         self.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.list2_context_menu)
         self.itemChanged.connect(self.list2_checked_changed)
         self.itemChanged = self.itemChanged2
-        self.act_delete = QtWidgets.QAction(qta.icon("fa5.trash-alt"), "Delete", self)
+        self.act_delete = QtWidgets.QAction(qta.icon("fa5.trash-alt"), "Remove", self)
         self.act_delete.triggered.connect(self.delete_item)
 
         self.act_color = None
         if color_picker is True:
             self.act_color = QtWidgets.QAction(qta.icon("fa5s.paint-brush"), "Change Color", self)
             self.act_color.triggered.connect(self.change_color)
+        self.act_copy = None
+        if copy_params is True:
+            self.act_copy = QtWidgets.QAction(qta.icon("fa5.copy"), "Copy Parameters", self)
+            self.act_copy.triggered.connect(self.signal_act_copy_clicked)
+            self.act_paste = QtWidgets.QAction(qta.icon("fa5s.paste"), "Paste Parameters", self)
+            self.act_paste.triggered.connect(self.signal_act_paste_clicked)
+            self.allow_paste_callback = allow_paste_callback
+            self.act_path = QtWidgets.QAction(qta.icon("mdi.folder-multiple-image"), "Adjust Paths", self)
+            self.act_path.triggered.connect(self.signal_act_paths_clicked)
 
         self.setDragDropMode(QtWidgets.QAbstractItemView.InternalMove)
 
         self.flags = QtCore.Qt.ItemIsSelectable | QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsUserCheckable
         if editable:
             self.flags |= QtCore.Qt.ItemIsEditable | QtCore.Qt.ItemIsDragEnabled
 
@@ -369,14 +365,19 @@
     def list2_context_menu(self, position):
         if self.currentItem() and self.currentItem() != self.add_item:
             # context menu
             menu = QtWidgets.QMenu()
 
             if self.act_color is not None:
                 menu.addAction(self.act_color)
+            if self.act_copy is not None:
+                menu.addAction(self.act_copy)
+                self.act_paste.setDisabled(not self.allow_paste_callback())
+                menu.addAction(self.act_paste)
+                menu.addAction(self.act_path)
 
             menu.addAction(self.act_delete)
 
             # open menu at mouse click position
             if menu:
                 menu.exec_(self.viewport().mapToGlobal(position))
 
@@ -391,14 +392,15 @@
             self.data[index][3] = "#%02x%02x%02x" % color.getRgb()[:3]
             self.item(index).setIcon(qta.icon("fa5.circle", options=[dict(color=color)]))
 
     def delete_item(self):
         index = self.currentRow()
         self.data.pop(index)
         self.takeItem(index)
+        self.setCurrentRow(index)
 
     def setData(self, data):
         self.no_list_change = True
         self.data = data
         self.clear()
         for d, checked, _, color in data:
             self.customAddItem(d, checked, color)
@@ -436,46 +438,74 @@
         if color is not None:
             item.setIcon(qta.icon("fa5.circle", options=[dict(color=color)]))
         item.setFlags(self.flags)
         item.setCheckState(QtCore.Qt.Checked if checked else QtCore.Qt.Unchecked)
         return item
 
 
-
-"""  """
-
 from multiprocessing import Process, Queue
 
 
 class SignalReturn:
     pass
 
 def call_func(func: callable, queue_in: Queue, queue_out: Queue):
     args = queue_in.get()
     kwargs = queue_in.get()
     returns = func(queue_out, *args, **kwargs)
     queue_out.put(SignalReturn())
     queue_out.put(returns)
 
 
+class PseudoPipe:
+    def __init__(self, progress_signal):
+        self.progress_signal = progress_signal
+    def put(self, data):
+        self.progress_signal.emit(data)
+
+import threading
+
+class ConciseRobustResult(threading.Thread):
+    def run(self):
+        try:
+            if self._target is not None:
+                self.result = self._target(*self._args, **self._kwargs)
+        finally:
+            # Avoid a refcycle if the thread is running a function with
+            # an argument that has a member that points to the thread.
+            del self._target, self._args, self._kwargs
+
+
 class ProcessSimple:
-    def __init__(self, target, args=[], kwargs={}, progress_signal=None):
-        self.queue_in = Queue()
-        self.queue_out = Queue()
+    thread = None
+    process = None
+
+    def __init__(self, target, args=[], kwargs={}, progress_signal=None, use_thread=False):
         self.args = args
         self.kwargs = kwargs
         self.progress_signal = progress_signal
-        self.process = Process(target=call_func, args=(target, self.queue_in, self.queue_out))
+        if use_thread:
+            self.thread = ConciseRobustResult(target=target, args=tuple([PseudoPipe(progress_signal)]+list(args)), kwargs=kwargs)
+        else:
+            self.queue_in = Queue()
+            self.queue_out = Queue()
+            self.process = Process(target=call_func, args=(target, self.queue_in, self.queue_out))
 
     def start(self):
-        self.process.start()
-        self.queue_in.put(self.args)
-        self.queue_in.put(self.kwargs)
+        if self.thread is not None:
+            self.thread.start()
+        else:
+            self.process.start()
+            self.queue_in.put(self.args)
+            self.queue_in.put(self.kwargs)
 
     def join(self):
+        if self.thread:
+            self.thread.join(timeout=10)
+            return self.thread.result
         while True:
             result = self.queue_out.get()
             if isinstance(result, SignalReturn):
                 result = self.queue_out.get()
                 break
             elif self.progress_signal is not None:
                 self.progress_signal.emit(result)
@@ -533,7 +563,20 @@
     def set_result(self, result):
         self.result = result
         self.thread.quit()
         self.worker.deleteLater()
         self.finished.emit()
 
 
+def wrap_string(func):
+    def call(*args, **kwargs):
+        new_path = func(*args, **kwargs)
+        if new_path:
+            if isinstance(new_path, tuple):
+                new_path = new_path[0]
+            else:
+                new_path = str(new_path)
+        return new_path
+    return call
+
+QtWidgets.QFileDialog.getSaveFileName = wrap_string(QtWidgets.QFileDialog.getSaveFileName)
+QtWidgets.QFileDialog.getOpenFileName = wrap_string(QtWidgets.QFileDialog.getOpenFileName)
```

### Comparing `saenopy-0.8.0/saenopy/gui/patch_lifreader.py` & `saenopy-0.9.0/saenopy/gui/common/patch_lifreader.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/gui/stack_selector_leica.py` & `saenopy-0.9.0/saenopy/gui/common/stack_selector_leica.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-# Setting the Qt bindings for QtPy
-import os
-import sys
 import numpy as np
 from qtpy import QtWidgets
-from saenopy.gui import QtShortCuts
+from saenopy.gui.common import QtShortCuts
 
 
 class StackSelectorLeica(QtWidgets.QWidget):
     no_update = False
     def __init__(self, parent, use_time=False):
         super().__init__()
         self.parent = parent
@@ -27,47 +24,61 @@
     def validator(self, value=None):
         return True
 
     def checkAcceptFilename(self, filename):
         return filename.endswith(".lif")
 
     def setImage(self, filename):
-        from readlif.reader import LifFile
-        from saenopy.gui import patch_lifreader
+        from .lif_reader import LifFile
+        #from saenopy.gui import patch_lifreader
         new = LifFile(filename)
+        self.filename = filename
         self.new = new
         print([(im.info["path"], im.info["name"], im.channels, im.dims) for im in new.get_iter_image()])
         self.setVisible(True)
         self.input_folder.setValues(list(np.arange(new.num_images)), [im.info["path"]+ im.info["name"] for im in new.get_iter_image()])
+        self.setFolder(0)
 
     def setFolder(self, index):
-        print("setFolder")
         self.im = self.new.get_image(index)
+        self.folder_index = index
         try:
             self.no_update = True
             self.channel.setValues(list(np.arange(self.im.channels)))
             self.time.setValues(list(np.arange(self.im.nt)))
-            self.parent.setZCount(self.im.nz)
         finally:
             self.no_update = False
-        print("showImage")
         self.showImage()
 
     def showImage(self):
-        print("showing Image", self.no_update)
+        self.parent.stack_changed.emit()
+
+        self.target_glob = f"{self.filename[:-4]}{{f:{self.folder_index}}}{{c:{self.channel.value()}}}.lif"
+        self.parent.glob_string_changed.emit('getstack', self.target_glob)
         if self.no_update is True:
             return
 
-        if self.parent.z_slider.active_range != 0:
-            im = np.max(self.im[self.time.value(), self.parent.getZRange(), self.channel.value()], axis=0)
-            self.parent.setImage(im)
+        im = self.get_image(0, 0, 0)
+        # if there is no z channel
+        if self.im.scale[2] is None:
+            self.label.setText(
+                f"Voxel {self.im.scale[0]:.3}µm x {self.im.scale[1]:.3}µm x {0}µm ({im.shape[1]}, {im.shape[0]}, {self.im.dims.z})")
         else:
-            im = self.im[self.time.value(), self.parent.getZ(), self.channel.value()]
-            self.parent.setImage(im)
-
-        self.label.setText(f"Voxel {self.im.scale[0]:.3}µm x {self.im.scale[1]:.3}µm x {self.im.scale[2]:.3}µm ({im.shape[1]}, {im.shape[0]}, {self.im.nz})")
+            self.label.setText(f"Voxel {self.im.scale[0]:.3}µm x {self.im.scale[1]:.3}µm x {self.im.scale[2]:.3}µm ({im.shape[1]}, {im.shape[0]}, {self.im.dims.z})")
 
     def getVoxelSize(self):
-        return self.im.scale[0:2]
+        return self.im.scale[0:3]
 
     def getStack(self):
-        return self.im[self.time.value(), :, self.channel.value()].transpose(1, 2, 0)
+        return self.im[self.time.value(), :, self.channel.value()].transpose(1, 2, 0)
+
+    def get_image(self, t, z, c=0):
+        return np.asarray(self.im.get_frame(z, t, self.channel.value()))
+
+    def get_t_count(self):
+        return self.im.dims.t
+
+    def get_z_count(self):
+        return self.im.dims.z
+
+    def get_crop(self):
+        return {}
```

### Comparing `saenopy-0.8.0/saenopy/gui_deformation.py` & `saenopy-0.9.0/saenopy/unused/gui_deformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pyvista as pv
 import vtk
 from pyvistaqt import QtInteractor
 
 import saenopy
 import saenopy.multigridHelper
 from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.stack_selector import StackSelector
+from saenopy.gui.common.stack_selector import StackSelector
 import imageio
 from qimage2ndarray import array2qimage
 import matplotlib.pyplot as plt
 import glob
 import imageio
 import threading
 import saenopy.getDeformations
@@ -32,48 +32,40 @@
         FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
 else:
     from matplotlib.backends.backend_qt4agg import (
         FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
 from matplotlib.figure import Figure
 
 
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
-
-
-
 class DeformationDetector(QtWidgets.QWidget):
     detection_finished = QtCore.Signal()
     detection_error = QtCore.Signal(str)
 
     def __init__(self, layout, stack_deformed, stack_relaxed):
         super().__init__()
         layout.addWidget(self)
 
         main_layout = QtWidgets.QVBoxLayout(self)
 
         self.stack_deformed = stack_deformed
         self.stack_relaxed = stack_relaxed
 
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.input_overlap = QtShortCuts.QInputNumber(main_layout, "overlap", 0.6, step=0.1)
         self.input_win = QtShortCuts.QInputNumber(main_layout, "window size", 30)
         self.input_signoise = QtShortCuts.QInputNumber(main_layout, "signoise", 1.3, step=0.1)
         self.input_driftcorrection = QtShortCuts.QInputBool(main_layout, "driftcorrection", True)
         self.input_button = QtWidgets.QPushButton("detect deformations")
         main_layout.addWidget(self.input_button)
         self.input_button.clicked.connect(self.start_detect)
 
         self.progressbar = QProgressBar(main_layout)
 
-        self.plotter = QtInteractor(self)
+        self.plotter = QtInteractor(self, auto_update=False)
         self.plotter.set_background("black")
         main_layout.addWidget(self.plotter.interactor)
 
         self.detection_finished.connect(self.finished_detection)
         self.detection_error.connect(self.errored_detection)
 
     def start_detect(self):
@@ -162,26 +154,26 @@
         super().__init__()
         layout.addWidget(self)
 
         main_layout = QtWidgets.QVBoxLayout(self)
 
         self.deformation_detector = deformation_detector
 
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.input_element_size = QtShortCuts.QInputString(main_layout, "element_size", "7")
         self.input_inner_region = QtShortCuts.QInputString(main_layout, "inner_region", "100")
         self.input_thinning_factor = QtShortCuts.QInputNumber(main_layout, "thinning factor", 0.2, step=0.1)
         self.input_button = QtWidgets.QPushButton("interpolate mesh")
         main_layout.addWidget(self.input_button)
         self.input_button.clicked.connect(self.start_interpolation)
 
         self.progressbar = QProgressBar(main_layout)
 
-        self.plotter = QtInteractor(self)
+        self.plotter = QtInteractor(self, auto_update=False)
         self.plotter.set_background("black")
         main_layout.addWidget(self.plotter.interactor)
 
         self.detection_finished.connect(self.finished_detection)
 
     def start_interpolation(self):
         self.input_button.setEnabled(False)
@@ -233,15 +225,15 @@
         super().__init__()
         layout.addWidget(self)
 
         main_layout = QtWidgets.QVBoxLayout(self)
 
         self.mesh_creator = mesh_creator
 
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.input_k = QtShortCuts.QInputString(main_layout, "k", "1645")
         self.input_d0 = QtShortCuts.QInputString(main_layout, "d0", "0.0008")
         self.input_lamda_s = QtShortCuts.QInputString(main_layout, "lamdba_s", "0.0075")
         self.input_ds = QtShortCuts.QInputString(main_layout, "ds", "0.033")
         self.input_alpha = QtShortCuts.QInputString(main_layout, "alpha", "9")
         self.input_stepper = QtShortCuts.QInputString(main_layout, "stepper", "0.33")
@@ -252,15 +244,15 @@
 
         self.progressbar = QProgressBar(main_layout)
 
         self.canvas = FigureCanvas(Figure(figsize=(5, 3)))
         self.canvas.figure.add_axes([0.2, 0.2, 0.8, 0.8])
         main_layout.addWidget(self.canvas)
 
-        self.plotter = QtInteractor(self)
+        self.plotter = QtInteractor(self, auto_update=False)
         self.plotter.set_background("black")
         main_layout.addWidget(self.plotter.interactor)
 
         self.detection_finished.connect(self.finished_detection)
         self.iteration_finished.connect(self.iteration_callback)
 
         self.iteration_finished.emit(np.ones([10, 3]))
@@ -344,15 +336,15 @@
 
 class MainWindow(QtWidgets.QWidget):
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Viewer")
 
         main_layout = QtWidgets.QHBoxLayout(self)
```

### Comparing `saenopy-0.8.0/saenopy/gui_deformation_spheriod.py` & `saenopy-0.9.0/saenopy/gui/spheroid/gui_deformation_spheroid.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,64 +8,42 @@
 
 os.environ["QT_API"] = "pyqt5"
 
 from qtpy import QtCore, QtWidgets, QtGui
 
 import numpy as np
 from natsort import natsorted
-import pyvista as pv
-import vtk
-from pyvistaqt import QtInteractor
-
-import saenopy
-import saenopy.multigridHelper
-from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.stack_selector import StackSelector
-import imageio
+
+
+from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
 from qimage2ndarray import array2qimage
 import matplotlib.pyplot as plt
-import glob
 import imageio
 import threading
 import glob
-import re
-import saenopy.getDeformations
-import saenopy.multigridHelper
-import saenopy.materials
-
-if QtCore.qVersion() >= "5.":
-    from matplotlib.backends.backend_qt5agg import (
-        FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
-else:
-    from matplotlib.backends.backend_qt4agg import (
-        FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
+
+
 from matplotlib.figure import Figure
 import jointforces as jf
 import urllib
 from pathlib import Path
 
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
-
 import ctypes
 
 from qtpy import API_NAME as QT_API_NAME
 if QT_API_NAME.startswith("PyQt4"):
     from matplotlib.backends.backend_qt4agg import FigureCanvasQTAgg as Canvas
     from matplotlib.backends.backend_qt4agg import FigureManager
     from matplotlib.backends.backend_qt4 import NavigationToolbar2QT as NavigationToolbar
 else:
     from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as Canvas
     from matplotlib.backends.backend_qt5agg import FigureManager
     from matplotlib.backends.backend_qt5 import NavigationToolbar2QT as NavigationToolbar
 
-settings = QtCore.QSettings("Saenopy", "Seanopy")
+settings = QtCore.QSettings("Saenopy", "Saenopy")
 
 
 class MatplotlibWidget(Canvas):
 
     def __init__(self, parent=None, width=4, height=3, dpi=100):
         from matplotlib import _pylab_helpers
         plt.ioff()
@@ -96,50 +74,55 @@
         _pylab_helpers.Gcf.set_active(self.manager)
 
     def setActive(self):
         from matplotlib import _pylab_helpers
         self.manager._cidgcf = self.figure
         _pylab_helpers.Gcf.set_active(self.manager)
 
+
 def execute(func, *args, **kwargs):
     func(*args, **kwargs)
     import inspect
     code_lines = inspect.getsource(func).split("\n")[1:]
     indent = len(code_lines[0]) - len(code_lines[0].lstrip())
     code = "\n".join(line[indent:] for line in code_lines)
     for key, value in kwargs.items():
         if isinstance(value, str):
             code = code.replace(key, "'"+value+"'")
         else:
             code = code.replace(key, str(value))
     code = code.replace("self.canvas.draw()", "plt.show()")
     return code
 
+
 def kill_thread(thread):
     """
     thread: a threading.Thread object
     """
     thread_id = thread.ident
     res = ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, ctypes.py_object(SystemExit))
     if res > 1:
         ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, 0)
         print('Exception raise failure')
 
+
 class QHLine(QtWidgets.QFrame):
     def __init__(self):
         super().__init__()
         self.setFrameShape(QtWidgets.QFrame.HLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
 
+
 class QVLine(QtWidgets.QFrame):
     def __init__(self):
         super().__init__()
         self.setFrameShape(QtWidgets.QFrame.VLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
 
+
 class Spoiler(QtWidgets.QWidget):
     def __init__(self, parent=None, title='', animationDuration=300):
         """
         References:
             # Adapted from c++ version
             http://stackoverflow.com/questions/32476006/how-to-make-an-expandable-collapsable-section-widget-in-qt
         """
@@ -270,22 +253,23 @@
     def addLayout(self, layout):
         if self.main_layout is None:
             self.setLayout(layout)
         else:
             self.child_widget.setLayout(layout)
         return layout
 
+
 class LookUpTable(QtWidgets.QDialog):
     progress_signal = QtCore.Signal(int, int)
     finished_signal = QtCore.Signal()
     thread = None
 
     def __init__(self):
         super().__init__()
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         with QtShortCuts.QHBoxLayout(self):
             with QtShortCuts.QVBoxLayout() as main_layout:
                 with QtShortCuts.QGroupBox(None, "Material Parameters") as (self.material_parameters, layout):
                     with QtShortCuts.QHBoxLayout():
                         self.input_k = QtShortCuts.QInputString(None, "k", "1449", type=float)
                         self.input_d0 = QtShortCuts.QInputString(None, "d0", "0.00215", type=float)
@@ -654,15 +638,15 @@
 
 class MainWindow(QtWidgets.QWidget):
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Viewer")
 
         main_layout = QtWidgets.QHBoxLayout(self)
 
@@ -800,15 +784,15 @@
     finished_signal = QtCore.Signal()
     thread = None
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Viewer")
 
         with QtShortCuts.QHBoxLayout(self) as main_layout:
             with QtShortCuts.QSplitter() as lay:
@@ -987,15 +971,15 @@
                     def changed():
                         import glob, re
                         text = os.path.normpath(self.inputText.value())
 
                         glob_string = text.replace("?", "*")
                         files =natsorted( glob.glob(glob_string))
                                               
-                        regex_string = re.escape(text).replace("\*", "(.*)").replace("\?", ".*")
+                        regex_string = re.escape(text).replace(r"\*", "(.*)").replace(r"\?", ".*")
 
                         data = {}
                         for file in files:
                             file = os.path.normpath(file)
                             print(file, regex_string)
                             match = re.match(regex_string, file).groups()
                             reconstructed_file = regex_string
@@ -1063,15 +1047,15 @@
         print("globbing", glob_string)
         files = natsorted(glob.glob(glob_string))
 
         output_base = glob_string
         while "*" in str(output_base):
             output_base = Path(output_base).parent
 
-        regex_string = re.escape(text).replace("\*", "(.*)").replace("\?", ".*")
+        regex_string = re.escape(text).replace(r"\*", "(.*)").replace(r"\?", ".*")
 
         data = {}
         for file in files:
             file = os.path.normpath(file)
             print(file, regex_string)
             match = re.match(regex_string, file).groups()
             reconstructed_file = regex_string
@@ -1332,15 +1316,15 @@
                                                        dt_min=(self.dt_min.value()),
                                                        cutoff=None, cmap="turbo",
                                                        callback=lambda ii, nn: self.progress_signal.emit(i, n, ii, nn))
 
                     elif self.plot_data.value() is True:
                         images = data["images"]
                         for ii in range(0, len(images)):
-                            im = imageio.imread(images[i]).astype(np.float)
+                            im = imageio.imread(images[i]).astype(float)
                             if ii == 0 or self.continous_segmentation.value() is True:
                                 seg0 = jf.piv.segment_spheroid(im, True, self.thres_segmentation.value())
                             if ii > 0:
                                 print("self.dt_min.value()*ii if self.dt_min.value() is not None else None", self.dt_min.value()*ii if self.dt_min.value() is not None else None)
                                 from jointforces.piv import save_displacement_plot
                                 dis_sum = np.load(str(data["output"]) + '/def' + str(ii).zfill(6) + '.npy', allow_pickle=True).item()
                                 save_displacement_plot(str(data["output"]) + '/plot' + str(ii).zfill(6) + '.png', im,
@@ -1513,15 +1497,15 @@
     finished_signal = QtCore.Signal()
     thread = None
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Evaluation")
 
         self.images = []
         self.data_folders = []
```

### Comparing `saenopy-0.8.0/saenopy/gui_deformation_wizard.py` & `saenopy-0.9.0/saenopy/unused/gui_deformation_wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 import sys
 
 # Setting the Qt bindings for QtPy
 import os
 
 os.environ["QT_API"] = "pyqt5"
 
-from qtpy import QtCore, QtWidgets, QtGui
+from qtpy import QtCore, QtWidgets
 
 import numpy as np
 
 import pyvista as pv
-import vtk
 from pyvistaqt import QtInteractor
 
 import saenopy
 import saenopy.multigridHelper
-from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.stack_selector import StackSelector
-import imageio
-from qimage2ndarray import array2qimage
-import matplotlib.pyplot as plt
+from saenopy.gui import QtShortCuts
+from saenopy.gui.common.stack_selector import StackSelector
 import glob
-import imageio
 import threading
 import saenopy.getDeformations
 import saenopy.multigridHelper
 import saenopy.materials
 
 if QtCore.qVersion() >= "5.":
-    from matplotlib.backends.backend_qt5agg import (
-        FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
+    pass
 else:
     from matplotlib.backends.backend_qt4agg import (
-        FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
+        FigureCanvas)
 from matplotlib.figure import Figure
 
 
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
-
 class QHLine(QtWidgets.QFrame):
     def __init__(self):
         super().__init__()
         self.setFrameShape(QtWidgets.QFrame.HLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
 
 
@@ -61,15 +49,15 @@
             layout.addWidget(self)
 
         main_layout = QtWidgets.QVBoxLayout(self)
 
         self.stack_deformed = stack_deformed
         self.stack_relaxed = stack_relaxed
 
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         with QtShortCuts.QHBoxLayout(main_layout) as layout2:
             self.input_overlap = QtShortCuts.QInputNumber(None, "overlap", 0.6, step=0.1, value_changed=self.valueChanged)
             self.input_win = QtShortCuts.QInputNumber(None, "window size", 30, value_changed=self.valueChanged, unit="μm")
         with QtShortCuts.QHBoxLayout(main_layout) as layout2:
             self.input_signoise = QtShortCuts.QInputNumber(None, "signoise", 1.3, step=0.1)
             self.input_driftcorrection = QtShortCuts.QInputBool(None, "driftcorrection", True)
@@ -77,15 +65,15 @@
         main_layout.addWidget(self.label)
         self.input_button = QtWidgets.QPushButton("detect deformations")
         main_layout.addWidget(self.input_button)
         self.input_button.clicked.connect(self.start_detect)
 
         self.progressbar = QProgressBar(main_layout)
 
-        self.plotter = QtInteractor(self)
+        self.plotter = QtInteractor(self, auto_update=False)
         self.plotter.set_background("black")
         main_layout.addWidget(self.plotter.interactor)
 
         self.detection_finished.connect(self.finished_detection)
         self.detection_error.connect(self.errored_detection)
 
     def valueChanged(self):
@@ -188,15 +176,15 @@
         if layout is not None:
             layout.addWidget(self)
 
         main_layout = QtWidgets.QVBoxLayout(self)
 
         self.deformation_detector = deformation_detector
 
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.input_element_size = QtShortCuts.QInputNumber(main_layout, "element_size", 7, unit="μm")
         with QtShortCuts.QHBoxLayout(main_layout) as layout2:
             self.input_inner_region = QtShortCuts.QInputNumber(None, "inner_region", 100, unit="μm")
             self.input_thinning_factor = QtShortCuts.QInputNumber(None, "thinning factor", 0.2, step=0.1)
         with QtShortCuts.QHBoxLayout(main_layout) as layout2:
             def changed_same_as():
@@ -221,15 +209,15 @@
             changed_same_as()
         self.input_button = QtWidgets.QPushButton("interpolate mesh")
         main_layout.addWidget(self.input_button)
         self.input_button.clicked.connect(self.start_interpolation)
 
         self.progressbar = QProgressBar(main_layout)
 
-        self.plotter = QtInteractor(self)
+        self.plotter = QtInteractor(self, auto_update=False)
         self.plotter.set_background("black")
         main_layout.addWidget(self.plotter.interactor)
 
         self.detection_finished.connect(self.finished_detection)
 
     def start_interpolation(self):
         self.input_button.setEnabled(False)
@@ -283,15 +271,15 @@
         super().__init__()
         layout.addWidget(self)
 
         main_layout = QtWidgets.QVBoxLayout(self)
 
         self.mesh_creator = mesh_creator
 
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.material_parameters = QtWidgets.QGroupBox("Material Parameters")
         main_layout.addWidget(self.material_parameters)
         with QtShortCuts.QVBoxLayout(self.material_parameters) as layout:
             with QtShortCuts.QHBoxLayout(None) as layout2:
                 self.input_k = QtShortCuts.QInputString(None, "k", "1645", type=float)
                 self.input_d0 = QtShortCuts.QInputString(None, "d0", "0.0008", type=float)
@@ -313,15 +301,15 @@
 
         self.progressbar = QProgressBar(main_layout)
 
         self.canvas = FigureCanvas(Figure(figsize=(5, 3)))
         self.canvas.figure.add_axes([0.2, 0.2, 0.8, 0.8])
         main_layout.addWidget(self.canvas)
 
-        self.plotter = QtInteractor(self)
+        self.plotter = QtInteractor(self, auto_update=False)
         self.plotter.set_background("black")
         main_layout.addWidget(self.plotter.interactor)
 
         self.detection_finished.connect(self.finished_detection)
         self.iteration_finished.connect(self.iteration_callback)
 
         self.iteration_finished.emit(np.ones([10, 3]))
@@ -405,15 +393,15 @@
 
 class MainWindow(QtWidgets.QWidget):
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Viewer")
 
         main_layout = QtWidgets.QHBoxLayout(self)
```

### Comparing `saenopy-0.8.0/saenopy/gui_master.py` & `saenopy-0.9.0/saenopy/gui/gui_master.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,158 @@
 import sys
-
-# Setting the Qt bindings for QtPy
-import os
-
-os.environ["QT_API"] = "pyqt5"
-
 from qtpy import QtCore, QtWidgets, QtGui
+import multiprocessing
+# keep import for pyinstaller
+import skimage.filters.ridges
+import skimage.filters.thresholding
+
+from saenopy.gui.common import QtShortCuts
+from saenopy.gui.solver.gui_solver import MainWindowSolver as SolverMain
+from saenopy.gui.spheroid.gui_deformation_spheroid import MainWindow as SpheroidMain
+from saenopy.gui.orientation.gui_orientation import MainWindow as OrientationMain
+from saenopy.gui.code.gui_code import MainWindowCode
+from saenopy.gui.common.resources import resource_path, resource_icon
 
-import numpy as np
-
-import pyvista as pv
-import vtk
-from pyvistaqt import QtInteractor
-
-import saenopy
-import saenopy.multigridHelper
-from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.stack_selector import StackSelector
-import imageio
-from qimage2ndarray import array2qimage
-import matplotlib.pyplot as plt
-import glob
-import imageio
-import threading
-from pathlib import Path
-import saenopy.getDeformations
-import saenopy.multigridHelper
-import saenopy.materials
-from saenopy.gui_deformation_whole2 import MainWindow as SolverMain
-from saenopy.gui_deformation_spheriod import MainWindow as SpheriodMain
-from saenopy.gui_orientation import MainWindow as OrientationMain
 
 class InfoBox(QtWidgets.QWidget):
     def __init__(self, name, func):
         super().__init__()
         self.setMinimumWidth(200)
         self.setMaximumHeight(500)
         with QtShortCuts.QHBoxLayout(self) as l:
             with QtShortCuts.QGroupBox(l, name):
                 with QtShortCuts.QVBoxLayout() as l2:
                     if name == "Solver":
                         self.text = QtWidgets.QLabel("Calculate the forces from a\n3D stack or a series of 3D stacks.").addToLayout()
-                    elif name == "Spheriod":
+                    elif name == "Spheroid":
                         self.text = QtWidgets.QLabel("Calculate the forces of\nmulticellular aggregates\nfrom a timeseries of 2D images.").addToLayout()
                     else:
                         self.text = QtWidgets.QLabel("Measure the orientations\nof fiberes in 2D images.\n\nAs a proxy for contractility.").addToLayout()
                     self.button1 = QtShortCuts.QPushButton(None, name, func)
 
+
 class MainWindow(QtWidgets.QWidget):
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy")
-        self.setWindowIcon(QtGui.QIcon(str(Path(__file__).parent / "img/Icon.ico")))
-
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.setWindowIcon(resource_icon("Icon.ico"))
 
         with QtShortCuts.QHBoxLayout(self) as main_layout:
             main_layout.setContentsMargins(0, 0, 0, 0)
             with QtShortCuts.QTabWidget(main_layout) as self.tabs:
                 self.tabs.currentChanged.connect(self.changedTab)
                 self.tabs.setTabPosition(QtWidgets.QTabWidget.West)
                 with self.tabs.createTab("Home") as layout:
                     layout.addStretch()
                     with QtShortCuts.QHBoxLayout() as layout2:
                         layout.addStretch()
                         self.image = QtWidgets.QLabel("x").addToLayout()
-                        self.image.setPixmap(QtGui.QPixmap(str(Path(__file__).parent / "img/Logo.png")))
+                        self.image.setPixmap(QtGui.QPixmap(resource_path("Logo.png")))
                         self.image.setScaledContents(True)
                         self.image.setMaximumWidth(400)
                         self.image.setMaximumHeight(200)
                         layout.addStretch()
                     with QtShortCuts.QHBoxLayout() as layout2:
                         layout2.addStretch()
                         InfoBox("Solver", lambda: self.setTab(1)).addToLayout()
                         layout2.addStretch()
-                        InfoBox("Spheriod", lambda: self.setTab(2)).addToLayout()
+                        InfoBox("Spheroid", lambda: self.setTab(2)).addToLayout()
                         layout2.addStretch()
                         InfoBox("Orientation", lambda: self.setTab(3)).addToLayout()
                         layout2.addStretch()
                     layout.addStretch()
                 with self.tabs.createTab("Solver") as self.layout_solver:
-                    self.layout_solver.setContentsMargins(0, 0, 0, 0)
-                with self.tabs.createTab("Spheriod") as self.layout_spheriod:
-                    self.layout_spheriod.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+
+                with self.tabs.createTab("Spheroid") as self.layout_spheroid:
+                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+
                 with self.tabs.createTab("Orientation") as self.layout_orientation:
-                    self.layout_orientation.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+
+                with self.tabs.createTab("Code") as self.layout_code:
+                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    self.coder = MainWindowCode().addToLayout()
 
         #self.tabs.setCurrentIndex(self.settings.value("master_tab", 0))
         self.first_tab_change = False
 
     first_tab_change = True
     solver = None
-    spheriod = None
+    spheroid = None
     orientation = None
     def changedTab(self, value):
         if self.first_tab_change is False:
             self.settings.setValue("master_tab", value)
 
         if value == 1 and self.solver is None:
             self.solver = SolverMain().addToLayout(self.layout_solver)
-        if value == 2 and self.spheriod is None:
-            self.spheriod = SpheriodMain().addToLayout(self.layout_spheriod)
+            self.setMinimumWidth(1600)
+            self.setMinimumHeight(900)
+        if value == 2 and self.spheroid is None:
+            self.spheroid = SpheroidMain().addToLayout(self.layout_spheroid)
+            self.setMinimumWidth(1600)
+            self.setMinimumHeight(900)
         if value == 3 and self.orientation is None:
             self.orientation = OrientationMain().addToLayout(self.layout_orientation)
+            self.setMinimumWidth(1600)
+            self.setMinimumHeight(900)
 
     def setTab(self, value):
         self.tabs.setCurrentIndex(value)
 
 
-def main():
+def main():  # pragma: no cover
     app = QtWidgets.QApplication(sys.argv)
     if sys.platform.startswith('win'):
         import ctypes
         myappid = 'fabrylab.saenopy.master'  # arbitrary string
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
     print(sys.argv)
     window = MainWindow()
-    if len(sys.argv) >= 2:
-        window.loadFile(sys.argv[1])
     window.show()
+    try:
+        import pyi_splash
+
+        # Update the text on the splash screen
+        pyi_splash.update_text("PyInstaller is a great software!")
+        pyi_splash.update_text("Second time's a charm!")
+
+        # Close the splash screen. It does not matter when the call
+        # to this function is made, the splash screen remains open until
+        # this function is called or the Python program is terminated.
+        pyi_splash.close()
+    except (ImportError, RuntimeError):
+        pass
     sys.exit(app.exec_())
 
 
-if __name__ == '__main__':
+if __name__ == '__main__':  # pragma: no cover
+    # On Windows calling this function is necessary.
+    multiprocessing.freeze_support()
+
+    if len(sys.argv) >= 2 and sys.argv[1].endswith(".py"):
+        source = open(sys.argv[1]).read()
+        code = compile(source, sys.argv[1], 'exec')
+        exec(code)
+        exit(0)
+
+
+    """ some magic to prevent PyQt5 from swallowing exceptions """
+    # Back up the reference to the exceptionhook
+    sys._excepthook = sys.excepthook
+    # Set the exception hook to our wrapping function
+    sys.excepthook = lambda *args: sys._excepthook(*args)
+
+    for arg in sys.argv:
+        if arg == "--demo":
+            import os
+            os.environ["DEMO"] = "true"
+
     main()
```

### Comparing `saenopy-0.8.0/saenopy/gui_mpl.py` & `saenopy-0.9.0/saenopy/unused/gui_mpl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import os, sys
+import os
+import sys
 import re
 import numpy as np
 import matplotlib.pyplot as plt
 from qtpy import QtWidgets, QtCore
 from qtpy import API_NAME as QT_API_NAME
 if QT_API_NAME.startswith("PyQt4"):
     from matplotlib.backends.backend_qt4agg import FigureCanvasQTAgg as Canvas
@@ -180,22 +181,14 @@
     ax.w_xaxis.set_pane_color((0.2, 0.2, 0.2, 1.0))
     ax.w_yaxis.set_pane_color((0.2, 0.2, 0.2, 1.0))
     ax.w_zaxis.set_pane_color((0.2, 0.2, 0.2, 1.0))
     
     return fig
 
 
-
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
-
-
 class MatplotlibWidget(Canvas):
 
     def __init__(self, parent=None, width=4, height=3, dpi=100):
         plt.ioff()
         self.figure = Figure(figsize=(width, height), dpi=dpi)
         self.figure.patch.set_facecolor([0, 1, 0, 0])
         self.axes = self.figure.add_subplot(111)
```

### Comparing `saenopy-0.8.0/saenopy/gui_orientation.py` & `saenopy-0.9.0/saenopy/gui/orientation/gui_orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Setting the Qt bindings for QtPy
 import os
 
 import pandas as pd
 import qtawesome as qta
 from qtpy import QtCore, QtWidgets, QtGui
 import numpy as np
-from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.gui_classes import Spoiler, CheckAbleGroup, QHLine, QVLine, MatplotlibWidget, NavigationToolbar, execute, kill_thread, ListWidget
+from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
+from saenopy.gui.common.gui_classes import Spoiler, CheckAbleGroup, QHLine, QVLine, MatplotlibWidget, NavigationToolbar, execute, kill_thread, ListWidget
 import imageio
 from qimage2ndarray import array2qimage
 import matplotlib.pyplot as plt
 import glob
 import imageio
 import threading
 import glob
```

### Comparing `saenopy-0.8.0/saenopy/gui_reorder.py` & `saenopy-0.9.0/saenopy/unused/gui_reorder.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,42 +8,31 @@
 os.environ["QT_API"] = "pyqt5"
 
 from qtpy import QtCore, QtWidgets, QtGui
 
 import numpy as np
 
 import pyvista as pv
-import vtk
 from pyvistaqt import QtInteractor
 
-import saenopy
-import saenopy.multigridHelper
 from saenopy.gui import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.stack_selector import StackSelector
-from saenopy.gui.gui_classes import Spoiler, CheckAbleGroup, QHLine, QVLine, MatplotlibWidget, execute, kill_thread, ListWidget
+from saenopy.gui.common.stack_selector import StackSelector
 import imageio
 from qimage2ndarray import array2qimage
 import matplotlib.pyplot as plt
 import glob
 import imageio
 import threading
-import saenopy.getDeformations
 import saenopy.multigridHelper
 import saenopy.materials
-from saenopy.gui.stack_selector import StackSelector
+from saenopy.gui.common.stack_selector import StackSelector
 import matplotlib as mpl
 from pathlib import Path
 import re
 
-# \\131.188.117.96\biophysDS\lbischof\tif_and_analysis_backup\2021-06-21-NK92_BlebbRock\Blebb_round4\Mark_and_Find_001
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
 
 def format_glob(pattern):
     pattern = str(Path(pattern))
     regexp_string = re.sub(r"\\{([^}]*)\\}", r"(?P<\1>.*)", re.escape(pattern).replace("\\*\\*", ".*").replace("\\*", ".*"))
     regexp_string2 = re.compile(regexp_string)
     glob_string = re.sub(r"({[^}]*})", "*", pattern)
```

### Comparing `saenopy-0.8.0/saenopy/gui_vtk.py` & `saenopy-0.9.0/saenopy/unused/gui_vtk.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,22 +13,14 @@
 import vtk
 from pyvistaqt import QtInteractor
 
 import saenopy
 import saenopy.multigridHelper
 from saenopy.gui import QtShortCuts, QExtendedGraphicsView
 import imageio
-from qimage2ndarray import array2qimage
-import matplotlib.pyplot as plt
-
-""" some magic to prevent PyQt5 from swallowing exceptions """
-# Back up the reference to the exceptionhook
-sys._excepthook = sys.excepthook
-# Set the exception hook to our wrapping function
-sys.excepthook = lambda *args: sys._excepthook(*args)
 
 
 def pathParts(path):
     if path.parent == path:
         return [path]
     return pathParts(path.parent) + [path]
 
@@ -38,15 +30,15 @@
     scale = 1
     im = None
 
     def __init__(self, parent=None):
         QtWidgets.QMainWindow.__init__(self, parent)
 
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy")
+        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Viewer")
 
         # create the frame
         self.frame = QtWidgets.QFrame()
@@ -102,15 +94,15 @@
         layout_vert_plot.addStretch()
         self.button_export = QtWidgets.QPushButton("save image")
         layout_vert_plot.addWidget(self.button_export)
         self.button_export.clicked.connect(self.saveScreenshot)
 
         # add the pyvista interactor object
         self.plotter_layout = QtWidgets.QHBoxLayout()
-        self.plotter = QtInteractor(self.frame)
+        self.plotter = QtInteractor(self.frame, auto_update=False)
         self.plotter_layout.addWidget(self.plotter.interactor)
         vlayout.addLayout(self.plotter_layout)
 
         # simple menu to demo functions
         mainMenu = self.menuBar()
         fileMenu = mainMenu.addMenu('File')
         exitButton = QtWidgets.QAction('Load', self)
@@ -159,15 +151,19 @@
         for url in event.mimeData().urls():
             print(url)
             url = str(url.toString()).strip()
             if url.startswith("file:///"):
                 url = url[len("file:///"):]
             if url.startswith("file:"):
                 url = url[len("file:"):]
-            self.loadFile(url)
+            try:
+                self.loadFile(url)
+            except:
+                self.loadFileOld(url)
+                
 
 
     def openLoadDialog(self):
         # opening last directory von sttings
         self._open_dir = self.settings.value("_open_dir")
         if self._open_dir is None:
             self._open_dir = os.getcwd()
@@ -220,15 +216,59 @@
         self.offset = np.min(self.M.R, axis=0)
         if 0:
             self.stats_label.setText(f"""
             Nodes = {self.M.R.shape[0]}
             Tets = {self.M.T.shape[0]}
             """)
         self.replot()
+    
+    def loadFileOld(self, filename):
+        print("Loading", filename)
+        from saenopy.solver import load_solver 
+        self.set_path(Path(filename))
+        # load in solver object
+        self.M = load_solver(filename)
+        # alternative way
+        # self.M = saenopy.Solver.load_old(saenopy.Solver(),filename)
+         
+        def scale(m):
+            vmin, vmax = np.nanpercentile(m, [1, 99.9])
+            return np.clip((m-vmin)/(vmax-vmin), 0, 1)*(vmax-vmin)
 
+        R = self.M.R
+        minR = np.min(R, axis=0)
+        maxR = np.max(R, axis=0)
+        
+        if self.M.reg_mask is None: 
+            border = (R[:, 0] < minR[0] + 0.5e-6) | (R[:, 0] > maxR[0] - 0.5e-6) | \
+                     (R[:, 1] < minR[1] + 0.5e-6) | (R[:, 1] > maxR[1] - 0.5e-6) | \
+                     (R[:, 2] < minR[2] + 0.5e-6) | (R[:, 2] > maxR[2] - 0.5e-6)
+            self.M.reg_mask = ~border 
+                 
+
+        self.point_cloud = pv.PolyData(self.M.R)
+        self.point_cloud.point_arrays["f"] = -self.M.f*self.M.reg_mask[:, None]
+        self.point_cloud["f_mag"] = np.linalg.norm(self.M.f*self.M.reg_mask[:, None], axis=1)
+        self.point_cloud.point_arrays["U"] = self.M.U
+        self.point_cloud["U_mag"] = np.linalg.norm(self.M.U, axis=1)
+        self.point_cloud.point_arrays["U_target"] = self.M.U_target
+        self.point_cloud["U_target_mag"] = np.linalg.norm(self.M.U_target, axis=1)
+
+        self.point_cloud2 = None
+
+        self.offset = np.min(self.M.R, axis=0)
+        if 0:
+            self.stats_label.setText(f"""
+            Nodes = {self.M.R.shape[0]}
+            Tets = {self.M.T.shape[0]}
+            """)
+        self.replot()   
+        
+        
+        
     def calculateStiffness(self):
         self.point_cloud2 = pv.PolyData(np.mean(self.M.R[self.M.T], axis=1))
         from saenopy.materials import SemiAffineFiberMaterial
         #self.M.setMaterialModel(SemiAffineFiberMaterial(1645, 0.0008, 0.0075, 0.033), generate_lookup=False)
         if self.M.material_parameters is not None:
             print("loading material")
             self.M.setMaterialModel(SemiAffineFiberMaterial(*self.M.material_parameters[1:]), generate_lookup=False)
@@ -249,15 +289,15 @@
             shape = (1, len(names))
         else:
             shape = (2, 2)
         if self.plotter.shape != shape:
             self.plotter_layout.removeWidget(self.plotter)
             self.plotter.close()
 
-            self.plotter = QtInteractor(self.frame, shape=shape, border=False)
+            self.plotter = QtInteractor(self.frame, shape=shape, border=False, auto_update=False)
             self.plotter.set_background("black")
             #pv.set_plot_theme("document")
             self.plotter_layout.addWidget(self.plotter.interactor)
 
         plotter = self.plotter
         # color bar design properties
         # Set a custom position and size
```

### Comparing `saenopy-0.8.0/saenopy/img/Logo.png` & `saenopy-0.9.0/saenopy/img/Logo.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/img/Logo.svg` & `saenopy-0.9.0/saenopy/img/Logo.svg`

 * *Files 16% similar despite different names*

```diff
@@ -1,4617 +1,4848 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0a3c 7376 670a 2020 2078  "no"?>.<svg.   x
-00000040: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
-00000050: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
-00000060: 656e 7473 2f31 2e31 2f22 0a20 2020 786d  ents/1.1/".   xm
-00000070: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
-00000080: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00000090: 7267 2f6e 7323 220a 2020 2078 6d6c 6e73  rg/ns#".   xmlns
-000000a0: 3a72 6466 3d22 6874 7470 3a2f 2f77 7777  :rdf="http://www
-000000b0: 2e77 332e 6f72 672f 3139 3939 2f30 322f  .w3.org/1999/02/
-000000c0: 3232 2d72 6466 2d73 796e 7461 782d 6e73  22-rdf-syntax-ns
-000000d0: 2322 0a20 2020 786d 6c6e 733a 7376 673d  #".   xmlns:svg=
-000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000000f0: 7267 2f32 3030 302f 7376 6722 0a20 2020  rg/2000/svg".   
-00000100: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00000110: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
-00000120: 6722 0a20 2020 786d 6c6e 733a 736f 6469  g".   xmlns:sodi
-00000130: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
-00000140: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
-00000150: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
-00000160: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
-00000170: 6e73 3a69 6e6b 7363 6170 653d 2268 7474  ns:inkscape="htt
-00000180: 703a 2f2f 7777 772e 696e 6b73 6361 7065  p://www.inkscape
-00000190: 2e6f 7267 2f6e 616d 6573 7061 6365 732f  .org/namespaces/
-000001a0: 696e 6b73 6361 7065 220a 2020 2077 6964  inkscape".   wid
-000001b0: 7468 3d22 3231 312e 3437 3839 346d 6d22  th="211.47894mm"
-000001c0: 0a20 2020 6865 6967 6874 3d22 3130 372e  .   height="107.
-000001d0: 3335 386d 6d22 0a20 2020 7669 6577 426f  358mm".   viewBo
-000001e0: 783d 2230 2030 2032 3131 2e34 3738 3934  x="0 0 211.47894
-000001f0: 2031 3037 2e33 3538 220a 2020 2076 6572   107.358".   ver
-00000200: 7369 6f6e 3d22 312e 3122 0a20 2020 6964  sion="1.1".   id
-00000210: 3d22 7376 6736 3335 3422 0a20 2020 696e  ="svg6354".   in
-00000220: 6b73 6361 7065 3a76 6572 7369 6f6e 3d22  kscape:version="
-00000230: 312e 302e 3120 2833 6263 3265 3831 3366  1.0.1 (3bc2e813f
-00000240: 352c 2032 3032 302d 3039 2d30 3729 220a  5, 2020-09-07)".
-00000250: 2020 2073 6f64 6970 6f64 693a 646f 636e     sodipodi:docn
-00000260: 616d 653d 224c 6f67 6f2e 7376 6722 0a20  ame="Logo.svg". 
-00000270: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00000280: 742d 6669 6c65 6e61 6d65 3d22 2f68 6f6d  t-filename="/hom
-00000290: 652f 7269 6368 6172 642f 4472 6f70 626f  e/richard/Dropbo
-000002a0: 782f 5072 6f6a 6563 7473 2f32 3032 3020  x/Projects/2020 
-000002b0: 5361 6e6f 7079 2f73 6165 6e6f 7079 2f4c  Sanopy/saenopy/L
-000002c0: 6f67 6f2e 706e 6722 0a20 2020 696e 6b73  ogo.png".   inks
-000002d0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-000002e0: 3d22 3330 3022 0a20 2020 696e 6b73 6361  ="300".   inksca
-000002f0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00000300: 3330 3022 3e0a 2020 3c64 6566 730a 2020  300">.  <defs.  
-00000310: 2020 2069 643d 2264 6566 7336 3334 3822     id="defs6348"
-00000320: 3e0a 2020 2020 3c66 696c 7465 720a 2020  >.    <filter.  
-00000330: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00000340: 6c6c 6563 743d 2261 6c77 6179 7322 0a20  llect="always". 
-00000350: 2020 2020 2020 7374 796c 653d 2263 6f6c        style="col
-00000360: 6f72 2d69 6e74 6572 706f 6c61 7469 6f6e  or-interpolation
-00000370: 2d66 696c 7465 7273 3a73 5247 4222 0a20  -filters:sRGB". 
-00000380: 2020 2020 2020 6964 3d22 6669 6c74 6572        id="filter
-00000390: 3135 3035 3122 0a20 2020 2020 2020 783d  15051".       x=
-000003a0: 222d 302e 3136 3733 3333 3839 220a 2020  "-0.16733389".  
-000003b0: 2020 2020 2077 6964 7468 3d22 312e 3333       width="1.33
-000003c0: 3436 3637 3822 0a20 2020 2020 2020 793d  46678".       y=
-000003d0: 222d 302e 3635 3239 3833 3733 220a 2020  "-0.65298373".  
-000003e0: 2020 2020 2068 6569 6768 743d 2232 2e33       height="2.3
-000003f0: 3035 3936 3733 223e 0a20 2020 2020 203c  059673">.      <
-00000400: 6665 4761 7573 7369 616e 426c 7572 0a20  feGaussianBlur. 
-00000410: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00000420: 3a63 6f6c 6c65 6374 3d22 616c 7761 7973  :collect="always
-00000430: 220a 2020 2020 2020 2020 2073 7464 4465  ".         stdDe
-00000440: 7669 6174 696f 6e3d 2235 2e32 3236 3032  viation="5.22602
-00000450: 3039 220a 2020 2020 2020 2020 2069 643d  09".         id=
-00000460: 2266 6547 6175 7373 6961 6e42 6c75 7231  "feGaussianBlur1
-00000470: 3530 3533 2220 2f3e 0a20 2020 203c 2f66  5053" />.    </f
-00000480: 696c 7465 723e 0a20 203c 2f64 6566 733e  ilter>.  </defs>
-00000490: 0a20 203c 736f 6469 706f 6469 3a6e 616d  .  <sodipodi:nam
-000004a0: 6564 7669 6577 0a20 2020 2020 6964 3d22  edview.     id="
-000004b0: 6261 7365 220a 2020 2020 2070 6167 6563  base".     pagec
-000004c0: 6f6c 6f72 3d22 2366 6666 6666 6622 0a20  olor="#ffffff". 
-000004d0: 2020 2020 626f 7264 6572 636f 6c6f 723d      bordercolor=
-000004e0: 2223 3636 3636 3636 220a 2020 2020 2062  "#666666".     b
-000004f0: 6f72 6465 726f 7061 6369 7479 3d22 312e  orderopacity="1.
-00000500: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
-00000510: 3a70 6167 656f 7061 6369 7479 3d22 302e  :pageopacity="0.
-00000520: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
-00000530: 3a70 6167 6573 6861 646f 773d 2232 220a  :pageshadow="2".
-00000540: 2020 2020 2069 6e6b 7363 6170 653a 7a6f       inkscape:zo
-00000550: 6f6d 3d22 3822 0a20 2020 2020 696e 6b73  om="8".     inks
-00000560: 6361 7065 3a63 783d 2236 3333 2e39 3432  cape:cx="633.942
-00000570: 3036 220a 2020 2020 2069 6e6b 7363 6170  06".     inkscap
-00000580: 653a 6379 3d22 3534 312e 3631 3539 3522  e:cy="541.61595"
-00000590: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-000005a0: 6f63 756d 656e 742d 756e 6974 733d 226d  ocument-units="m
-000005b0: 6d22 0a20 2020 2020 696e 6b73 6361 7065  m".     inkscape
-000005c0: 3a63 7572 7265 6e74 2d6c 6179 6572 3d22  :current-layer="
-000005d0: 6731 3338 3122 0a20 2020 2020 7368 6f77  g1381".     show
-000005e0: 6772 6964 3d22 6661 6c73 6522 0a20 2020  grid="false".   
-000005f0: 2020 6669 742d 6d61 7267 696e 2d6c 6566    fit-margin-lef
-00000600: 743d 2231 3022 0a20 2020 2020 6669 742d  t="10".     fit-
-00000610: 6d61 7267 696e 2d74 6f70 3d22 3130 220a  margin-top="10".
-00000620: 2020 2020 2066 6974 2d6d 6172 6769 6e2d       fit-margin-
-00000630: 626f 7474 6f6d 3d22 3130 220a 2020 2020  bottom="10".    
-00000640: 2066 6974 2d6d 6172 6769 6e2d 7269 6768   fit-margin-righ
-00000650: 743d 2231 3022 0a20 2020 2020 696e 6b73  t="10".     inks
-00000660: 6361 7065 3a77 696e 646f 772d 7769 6474  cape:window-widt
-00000670: 683d 2231 3830 3222 0a20 2020 2020 696e  h="1802".     in
-00000680: 6b73 6361 7065 3a77 696e 646f 772d 6865  kscape:window-he
-00000690: 6967 6874 3d22 3931 3422 0a20 2020 2020  ight="914".     
-000006a0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-000006b0: 783d 222d 3822 0a20 2020 2020 696e 6b73  x="-8".     inks
-000006c0: 6361 7065 3a77 696e 646f 772d 793d 222d  cape:window-y="-
-000006d0: 3822 0a20 2020 2020 696e 6b73 6361 7065  8".     inkscape
-000006e0: 3a77 696e 646f 772d 6d61 7869 6d69 7a65  :window-maximize
-000006f0: 643d 2231 220a 2020 2020 2069 6e6b 7363  d="1".     inksc
-00000700: 6170 653a 646f 6375 6d65 6e74 2d72 6f74  ape:document-rot
-00000710: 6174 696f 6e3d 2230 2220 2f3e 0a20 203c  ation="0" />.  <
-00000720: 6d65 7461 6461 7461 0a20 2020 2020 6964  metadata.     id
-00000730: 3d22 6d65 7461 6461 7461 3633 3531 223e  ="metadata6351">
-00000740: 0a20 2020 203c 7264 663a 5244 463e 0a20  .    <rdf:RDF>. 
-00000750: 2020 2020 203c 6363 3a57 6f72 6b0a 2020       <cc:Work.  
-00000760: 2020 2020 2020 2072 6466 3a61 626f 7574         rdf:about
-00000770: 3d22 223e 0a20 2020 2020 2020 203c 6463  ="">.        <dc
-00000780: 3a66 6f72 6d61 743e 696d 6167 652f 7376  :format>image/sv
-00000790: 672b 786d 6c3c 2f64 633a 666f 726d 6174  g+xml</dc:format
-000007a0: 3e0a 2020 2020 2020 2020 3c64 633a 7479  >.        <dc:ty
-000007b0: 7065 0a20 2020 2020 2020 2020 2020 7264  pe.           rd
-000007c0: 663a 7265 736f 7572 6365 3d22 6874 7470  f:resource="http
-000007d0: 3a2f 2f70 7572 6c2e 6f72 672f 6463 2f64  ://purl.org/dc/d
-000007e0: 636d 6974 7970 652f 5374 696c 6c49 6d61  cmitype/StillIma
-000007f0: 6765 2220 2f3e 0a20 2020 2020 2020 203c  ge" />.        <
-00000800: 6463 3a74 6974 6c65 202f 3e0a 2020 2020  dc:title />.    
-00000810: 2020 3c2f 6363 3a57 6f72 6b3e 0a20 2020    </cc:Work>.   
-00000820: 203c 2f72 6466 3a52 4446 3e0a 2020 3c2f   </rdf:RDF>.  </
-00000830: 6d65 7461 6461 7461 3e0a 2020 3c67 0a20  metadata>.  <g. 
-00000840: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
-00000850: 656c 3d22 4c61 7965 7220 3122 0a20 2020  el="Layer 1".   
-00000860: 2020 696e 6b73 6361 7065 3a67 726f 7570    inkscape:group
-00000870: 6d6f 6465 3d22 6c61 7965 7222 0a20 2020  mode="layer".   
-00000880: 2020 6964 3d22 6c61 7965 7231 220a 2020    id="layer1".  
-00000890: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-000008a0: 616e 736c 6174 6528 342e 3438 3030 3732  anslate(4.480072
-000008b0: 392c 332e 3138 3933 3639 2922 3e0a 2020  9,3.189369)">.  
-000008c0: 2020 3c72 6563 740a 2020 2020 2020 2073    <rect.       s
-000008d0: 7479 6c65 3d22 6f70 6163 6974 793a 313b  tyle="opacity:1;
-000008e0: 6669 6c6c 3a23 6666 6666 6666 3b66 696c  fill:#ffffff;fil
-000008f0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00000900: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00000910: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00000920: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00000930: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00000940: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00000950: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00000960: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00000970: 0a20 2020 2020 2020 6964 3d22 7265 6374  .       id="rect
-00000980: 3135 3037 3422 0a20 2020 2020 2020 7769  15074".       wi
-00000990: 6474 683d 2232 3130 2e36 3236 3031 220a  dth="210.62601".
-000009a0: 2020 2020 2020 2068 6569 6768 743d 2231         height="1
-000009b0: 3035 2e35 3130 3622 0a20 2020 2020 2020  05.5106".       
-000009c0: 783d 222d 332e 3239 3435 3630 3722 0a20  x="-3.2945607". 
-000009d0: 2020 2020 2020 793d 222d 322e 3932 3236        y="-2.9226
-000009e0: 3531 3122 202f 3e0a 2020 2020 3c70 6174  511" />.    <pat
-000009f0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-00000a00: 6669 6c6c 3a23 3030 3030 3030 3b66 696c  fill:#000000;fil
-00000a10: 6c2d 6f70 6163 6974 793a 302e 3939 3834  l-opacity:0.9984
-00000a20: 3038 3b73 7472 6f6b 653a 2330 3030 3030  08;stroke:#00000
-00000a30: 303b 7374 726f 6b65 2d77 6964 7468 3a30  0;stroke-width:0
-00000a40: 2e32 3634 3538 3370 783b 7374 726f 6b65  .264583px;stroke
-00000a50: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00000a60: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00000a70: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
-00000a80: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-00000a90: 4d20 3838 2e32 3131 3532 362c 3434 2e30  M 88.211526,44.0
-00000aa0: 3335 3830 3220 3137 342e 3639 3134 2c33  35802 174.6914,3
-00000ab0: 312e 3234 3431 3733 2038 372e 3136 3935  1.244173 87.1695
-00000ac0: 3334 2c33 392e 3630 3437 3520 5a22 0a20  34,39.60475 Z". 
-00000ad0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00000ae0: 3635 3722 0a20 2020 2020 2020 696e 6b73  657".       inks
-00000af0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00000b00: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-00000b10: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-00000b20: 6574 7970 6573 3d22 6363 6363 2220 2f3e  etypes="cccc" />
-00000b30: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00000b40: 2020 7374 796c 653d 2266 696c 6c3a 2333    style="fill:#3
-00000b50: 6534 6237 373b 6669 6c6c 2d6f 7061 6369  e4b77;fill-opaci
-00000b60: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00000b70: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00000b80: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
-00000b90: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00000ba0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00000bb0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-00000bc0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00000bd0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00000be0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00000bf0: 2020 2020 2020 2064 3d22 4d20 362e 3737         d="M 6.77
-00000c00: 3737 3131 352c 3332 2e36 3739 3839 3620  77115,32.679896 
-00000c10: 3339 2e31 3137 3332 352c 3331 2e32 3039  39.117325,31.209
-00000c20: 3931 3620 3630 2e33 3635 3235 332c 372e  916 60.365253,7.
-00000c30: 3535 3635 3634 3620 4320 3333 2e35 3937  5565646 C 33.597
-00000c40: 3336 362c 3235 2e35 3538 3433 3620 3230  366,25.558436 20
-00000c50: 2e38 3038 3831 382c 3238 2e34 3437 3531  .808818,28.44751
-00000c60: 3620 362e 3737 3737 3131 352c 3332 2e36  6 6.7777115,32.6
-00000c70: 3739 3839 3620 5a22 0a20 2020 2020 2020  79896 Z".       
-00000c80: 6964 3d22 7061 7468 3134 3534 3722 0a20  id="path14547". 
-00000c90: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00000ca0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00000cb0: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-00000cc0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00000cd0: 3d22 6363 6363 2220 2f3e 0a20 2020 203c  ="cccc" />.    <
-00000ce0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-00000cf0: 653d 2266 696c 6c3a 2331 6332 6336 383b  e="fill:#1c2c68;
-00000d00: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00000d10: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00000d20: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
-00000d30: 3632 353b 7374 726f 6b65 2d6c 696e 6563  625;stroke-linec
-00000d40: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00000d50: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00000d60: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00000d70: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00000d80: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00000d90: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00000da0: 2064 3d22 6d20 3339 2e31 3137 3332 352c   d="m 39.117325,
-00000db0: 3331 2e32 3039 3931 3620 3134 2e30 3331  31.209916 14.031
-00000dc0: 3635 2c33 2e32 3037 3234 2037 2e32 3136  65,3.20724 7.216
-00000dd0: 3237 382c 2d32 362e 3836 3035 3933 3420  278,-26.8605934 
-00000de0: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
-00000df0: 7468 3134 3534 3922 0a20 2020 2020 2020  th14549".       
-00000e00: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00000e10: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00000e20: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-00000e30: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00000e40: 3a23 3036 3035 3038 3b66 696c 6c2d 6f70  :#060508;fill-op
-00000e50: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00000e60: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00000e70: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
-00000e80: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00000e90: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00000ea0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-00000eb0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00000ec0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00000ed0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00000ee0: 3122 0a20 2020 2020 2020 643d 226d 2035  1".       d="m 5
-00000ef0: 332e 3134 3839 3733 2c33 342e 3431 3731  3.148973,34.4171
-00000f00: 3536 2033 372e 3535 3133 3734 2c36 2e36  56 37.551374,6.6
-00000f10: 3831 3734 2043 2037 362e 3036 3732 3237  8174 C 76.067227
-00000f20: 2c33 332e 3336 3330 3036 2036 372e 3539  ,33.363006 67.59
-00000f30: 3334 3037 2c32 302e 3933 3433 3238 2036  3407,20.934328 6
-00000f40: 302e 3336 3532 3533 2c37 2e35 3536 3536  0.365253,7.55656
-00000f50: 3236 205a 220a 2020 2020 2020 2069 643d  26 Z".       id=
-00000f60: 2270 6174 6831 3435 3531 220a 2020 2020  "path14551".    
-00000f70: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00000f80: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00000f90: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
-00000fa0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-00000fb0: 6363 6322 202f 3e0a 2020 2020 3c70 6174  ccc" />.    <pat
-00000fc0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-00000fd0: 6669 6c6c 3a23 3237 3337 3733 3b66 696c  fill:#273773;fil
-00000fe0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00000ff0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00001000: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00001010: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00001020: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00001030: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00001040: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00001050: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00001060: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00001070: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-00001080: 226d 2036 2e37 3737 3731 3135 2c33 322e  "m 6.7777115,32.
-00001090: 3637 3938 3936 2063 2037 2e31 3136 3431  679896 c 7.11641
-000010a0: 3535 2c34 2e30 3832 3433 2031 342e 3936  55,4.08243 14.96
-000010b0: 3237 3134 352c 372e 3630 3334 3220 3137  27145,7.60342 17
-000010c0: 2e36 3339 3738 3935 2c31 352e 3130 3037  .6397895,15.1007
-000010d0: 3320 6c20 3134 2e36 3939 3832 342c 2d31  3 l 14.699824,-1
-000010e0: 362e 3537 3037 3120 7a22 0a20 2020 2020  6.57071 z".     
-000010f0: 2020 6964 3d22 7061 7468 3134 3535 3322    id="path14553"
-00001100: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00001110: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-00001120: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-00001130: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00001140: 6573 3d22 6363 6363 2220 2f3e 0a20 2020  es="cccc" />.   
-00001150: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00001160: 796c 653d 2266 696c 6c3a 2331 3432 3637  yle="fill:#14267
-00001170: 323b 6669 6c6c 2d6f 7061 6369 7479 3a31  2;fill-opacity:1
-00001180: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-00001190: 7374 726f 6b65 2d77 6964 7468 3a30 2e35  stroke-width:0.5
-000011a0: 3535 3632 353b 7374 726f 6b65 2d6c 696e  55625;stroke-lin
-000011b0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-000011c0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-000011d0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-000011e0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-000011f0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00001200: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00001210: 2020 2064 3d22 6d20 3234 2e34 3137 3530     d="m 24.41750
-00001220: 312c 3437 2e37 3830 3632 3620 3636 2e32  1,47.780626 66.2
-00001230: 3832 3834 362c 2d36 2e36 3831 3733 202d  82846,-6.68173 -
-00001240: 3531 2e35 3833 3032 322c 2d39 2e38 3838  51.583022,-9.888
-00001250: 3938 207a 220a 2020 2020 2020 2069 643d  98 z".       id=
-00001260: 2270 6174 6831 3435 3535 220a 2020 2020  "path14555".    
-00001270: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00001280: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00001290: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
-000012a0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000012b0: 696c 6c3a 2335 3436 3638 633b 6669 6c6c  ill:#54668c;fill
-000012c0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-000012d0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-000012e0: 2d77 6964 7468 3a30 2e35 3535 3632 353b  -width:0.555625;
-000012f0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00001300: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00001310: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00001320: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00001330: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00001340: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-00001350: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-00001360: 6d20 3234 2e34 3137 3530 312c 3437 2e37  m 24.417501,47.7
-00001370: 3830 3632 3620 3338 2e32 3139 3534 342c  80626 38.219544,
-00001380: 342e 3030 3930 3520 3238 2e30 3633 3330  4.00905 28.06330
-00001390: 322c 2d31 302e 3639 3037 3820 7a22 0a20  2,-10.69078 z". 
-000013a0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000013b0: 3535 3722 0a20 2020 2020 2020 696e 6b73  557".       inks
-000013c0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-000013d0: 7572 7661 7475 7265 3d22 3022 202f 3e0a  urvature="0" />.
-000013e0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-000013f0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3232   style="fill:#22
-00001400: 3334 3765 3b66 696c 6c2d 6f70 6163 6974  347e;fill-opacit
-00001410: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00001420: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00001430: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00001440: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00001450: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00001460: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00001470: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00001480: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00001490: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000014a0: 2020 2020 2020 643d 226d 2032 342e 3431        d="m 24.41
-000014b0: 3735 3031 2c34 372e 3738 3036 3236 2063  7501,47.780626 c
-000014c0: 2030 2e38 3539 3431 322c 372e 3431 3031   0.859412,7.4101
-000014d0: 3520 2d32 2e31 3135 3337 392c 3132 2e30  5 -2.115379,12.0
-000014e0: 3831 3538 202d 332e 3437 3435 3033 2c31  8158 -3.474503,1
-000014f0: 372e 3930 3730 3620 6c20 3431 2e36 3934  7.90706 l 41.694
-00001500: 3034 372c 2d31 332e 3839 3830 3120 7a22  047,-13.89801 z"
-00001510: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00001520: 3134 3535 3922 0a20 2020 2020 2020 696e  14559".       in
-00001530: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00001540: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00001550: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00001560: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
-00001570: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00001580: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00001590: 2330 3831 3036 393b 6669 6c6c 2d6f 7061  #081069;fill-opa
-000015a0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-000015b0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000015c0: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-000015d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000015e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000015f0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-00001600: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00001610: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00001620: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00001630: 220a 2020 2020 2020 2064 3d22 6d20 3230  ".       d="m 20
-00001640: 2e39 3432 3939 382c 3635 2e36 3837 3638  .942998,65.68768
-00001650: 3620 3238 2e38 3635 3130 382c 342e 3237  6 28.865108,4.27
-00001660: 3633 3120 3430 2e38 3932 3234 312c 2d32  631 40.892241,-2
-00001670: 382e 3836 3531 207a 220a 2020 2020 2020  8.8651 z".      
-00001680: 2069 643d 2270 6174 6831 3435 3631 220a   id="path14561".
-00001690: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000016a0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-000016b0: 7572 653d 2230 2220 2f3e 0a20 2020 203c  ure="0" />.    <
-000016c0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-000016d0: 653d 2266 696c 6c3a 2330 3730 6532 623b  e="fill:#070e2b;
-000016e0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-000016f0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00001700: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
-00001710: 3632 353b 7374 726f 6b65 2d6c 696e 6563  625;stroke-linec
-00001720: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00001730: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00001740: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00001750: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00001760: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00001770: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00001780: 2064 3d22 4d20 3439 2e38 3038 3130 362c   d="M 49.808106,
-00001790: 3639 2e39 3633 3939 3620 3636 2e37 3739  69.963996 66.779
-000017a0: 3731 372c 3932 2e32 3831 3030 3820 3630  717,92.281008 60
-000017b0: 2e34 3938 3838 392c 3632 2e32 3133 3138  .498889,62.21318
-000017c0: 3620 5a22 0a20 2020 2020 2020 6964 3d22  6 Z".       id="
-000017d0: 7061 7468 3134 3536 3322 0a20 2020 2020  path14563".     
-000017e0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-000017f0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00001800: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-00001810: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00001820: 6c6c 3a23 3238 3364 3837 3b66 696c 6c2d  ll:#283d87;fill-
-00001830: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00001840: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00001850: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
-00001860: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00001870: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00001880: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00001890: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-000018a0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-000018b0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-000018c0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-000018d0: 2036 302e 3439 3838 3839 2c36 322e 3231   60.498889,62.21
-000018e0: 3331 3836 2036 2e32 3830 3832 382c 3330  3186 6.280828,30
-000018f0: 2e30 3637 3832 3220 6320 332e 3235 3134  .067822 c 3.2514
-00001900: 352c 2d32 372e 3032 3935 3632 2031 342e  5,-27.029562 14.
-00001910: 3639 3336 352c 2d33 362e 3736 3735 3532  69365,-36.767552
-00001920: 2032 332e 3932 3036 332c 2d35 312e 3138   23.92063,-51.18
-00001930: 3231 3132 207a 220a 2020 2020 2020 2069  2112 z".       i
-00001940: 643d 2270 6174 6831 3435 3635 220a 2020  d="path14565".  
-00001950: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00001960: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-00001970: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
-00001980: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-00001990: 2263 6363 6322 202f 3e0a 2020 2020 3c65  "cccc" />.    <e
-000019a0: 6c6c 6970 7365 0a20 2020 2020 2020 7374  llipse.       st
-000019b0: 796c 653d 226f 7061 6369 7479 3a31 3b66  yle="opacity:1;f
-000019c0: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
-000019d0: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-000019e0: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-000019f0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00001a00: 3535 3536 3235 3b73 7472 6f6b 652d 6d69  555625;stroke-mi
-00001a10: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00001a20: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00001a30: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
-00001a40: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
-00001a50: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
-00001a60: 3d22 7061 7468 3134 3536 3722 0a20 2020  ="path14567".   
-00001a70: 2020 2020 6378 3d22 372e 3436 3430 3732      cx="7.464072
-00001a80: 3222 0a20 2020 2020 2020 6379 3d22 3332  2".       cy="32
-00001a90: 2e37 3134 3139 3522 0a20 2020 2020 2020  .714195".       
-00001aa0: 7278 3d22 312e 3636 3633 3332 3622 0a20  rx="1.6663326". 
-00001ab0: 2020 2020 2020 7279 3d22 312e 3636 3633        ry="1.6663
-00001ac0: 3332 3722 202f 3e0a 2020 2020 3c65 6c6c  327" />.    <ell
-00001ad0: 6970 7365 0a20 2020 2020 2020 7374 796c  ipse.       styl
-00001ae0: 653d 226f 7061 6369 7479 3a31 3b66 696c  e="opacity:1;fil
-00001af0: 6c3a 2332 3533 6137 643b 6669 6c6c 2d6f  l:#253a7d;fill-o
-00001b00: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00001b10: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00001b20: 6964 7468 3a30 2e35 3535 3632 353b 7374  idth:0.555625;st
-00001b30: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00001b40: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00001b50: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00001b60: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00001b70: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00001b80: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00001b90: 3637 2d33 220a 2020 2020 2020 2063 783d  67-3".       cx=
-00001ba0: 2232 302e 3637 3438 3437 220a 2020 2020  "20.674847".    
-00001bb0: 2020 2063 793d 2236 352e 3333 3232 3232     cy="65.332222
-00001bc0: 220a 2020 2020 2020 2072 783d 2231 2e36  ".       rx="1.6
-00001bd0: 3636 3333 3237 220a 2020 2020 2020 2072  663327".       r
-00001be0: 793d 2231 2e36 3636 3333 3238 220a 2020  y="1.6663328".  
-00001bf0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-00001c00: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
-00001c10: 3d22 342e 3634 3332 3536 3622 0a20 2020  ="4.6432566".   
-00001c20: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-00001c30: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
-00001c40: 222d 392e 3937 3830 3632 3122 202f 3e0a  "-9.9780621" />.
-00001c50: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-00001c60: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-00001c70: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00001c80: 7061 6369 7479 3a31 3b66 696c 6c3a 2332  pacity:1;fill:#2
-00001c90: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
-00001ca0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00001cb0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00001cc0: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
-00001cd0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00001ce0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00001cf0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-00001d00: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-00001d10: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00001d20: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
-00001d30: 2d37 220a 2020 2020 2020 2063 783d 2236  -7".       cx="6
-00001d40: 302e 3039 3331 3332 220a 2020 2020 2020  0.093132".      
-00001d50: 2063 793d 2235 312e 3839 3633 3937 220a   cy="51.896397".
-00001d60: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00001d70: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00001d80: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
-00001d90: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-00001da0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-00001db0: 793d 222d 392e 3937 3830 3632 3122 202f  y="-9.9780621" /
-00001dc0: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
-00001dd0: 2020 2020 2072 3d22 312e 3636 3633 3332       r="1.666332
-00001de0: 3822 0a20 2020 2020 2020 7374 796c 653d  8".       style=
-00001df0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-00001e00: 2361 3861 3961 613b 6669 6c6c 2d6f 7061  #a8a9aa;fill-opa
-00001e10: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00001e20: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00001e30: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-00001e40: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00001e50: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00001e60: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-00001e70: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00001e80: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00001e90: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-00001ea0: 2d33 2d35 220a 2020 2020 2020 2063 783d  -3-5".       cx=
-00001eb0: 2236 302e 3438 3833 3034 220a 2020 2020  "60.488304".    
-00001ec0: 2020 2063 793d 2236 312e 3937 3332 3535     cy="61.973255
-00001ed0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00001ee0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-00001ef0: 6572 2d78 3d22 342e 3634 3332 3536 3622  er-x="4.6432566"
-00001f00: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00001f10: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00001f20: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
-00001f30: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-00001f40: 2020 2020 2020 2072 3d22 312e 3636 3633         r="1.6663
-00001f50: 3332 3822 0a20 2020 2020 2020 7374 796c  328".       styl
-00001f60: 653d 226f 7061 6369 7479 3a31 3b66 696c  e="opacity:1;fil
-00001f70: 6c3a 2361 6261 6139 633b 6669 6c6c 2d6f  l:#abaa9c;fill-o
-00001f80: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00001f90: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00001fa0: 6964 7468 3a30 2e35 3535 3632 353b 7374  idth:0.555625;st
-00001fb0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00001fc0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00001fd0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00001fe0: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00001ff0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00002000: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00002010: 3637 2d33 2d39 220a 2020 2020 2020 2063  67-3-9".       c
-00002020: 783d 2235 302e 3231 3338 3622 0a20 2020  x="50.21386".   
-00002030: 2020 2020 6379 3d22 3639 2e38 3736 3637      cy="69.87667
-00002040: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
-00002050: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-00002060: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
-00002070: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00002080: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-00002090: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
-000020a0: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
-000020b0: 0a20 2020 2020 2020 723d 2232 2e35 3731  .       r="2.571
-000020c0: 3735 3131 220a 2020 2020 2020 2073 7479  7511".       sty
-000020d0: 6c65 3d22 6f70 6163 6974 793a 313b 6669  le="opacity:1;fi
-000020e0: 6c6c 3a23 3131 3230 3636 3b66 696c 6c2d  ll:#112066;fill-
-000020f0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00002100: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00002110: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
-00002120: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00002130: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00002140: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00002150: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00002160: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00002170: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00002180: 3536 372d 332d 3222 0a20 2020 2020 2020  567-3-2".       
-00002190: 6378 3d22 3339 2e33 3436 3636 3422 0a20  cx="39.346664". 
-000021a0: 2020 2020 2020 6379 3d22 3330 2e38 3533        cy="30.853
-000021b0: 3536 3322 0a20 2020 2020 2020 696e 6b73  563".       inks
-000021c0: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
-000021d0: 656e 7465 722d 783d 2237 2e31 3636 3231  enter-x="7.16621
-000021e0: 3136 220a 2020 2020 2020 2069 6e6b 7363  16".       inksc
-000021f0: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-00002200: 6e74 6572 2d79 3d22 2d31 352e 3339 3937  nter-y="-15.3997
-00002210: 3531 2220 2f3e 0a20 2020 203c 656c 6c69  51" />.    <elli
-00002220: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
-00002230: 3d22 6f70 6163 6974 793a 313b 6669 6c6c  ="opacity:1;fill
-00002240: 3a23 6564 6630 6663 3b66 696c 6c2d 6f70  :#edf0fc;fill-op
-00002250: 6163 6974 793a 302e 3939 3034 3436 3b73  acity:0.990446;s
-00002260: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00002270: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
-00002280: 3632 353b 7374 726f 6b65 2d6d 6974 6572  625;stroke-miter
-00002290: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-000022a0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-000022b0: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-000022c0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-000022d0: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
-000022e0: 6174 6831 3435 3637 2d32 220a 2020 2020  ath14567-2".    
-000022f0: 2020 2063 783d 2235 332e 3237 3634 3336     cx="53.276436
-00002300: 220a 2020 2020 2020 2063 793d 2233 332e  ".       cy="33.
-00002310: 3731 3835 3532 220a 2020 2020 2020 2072  718552".       r
-00002320: 783d 2231 2e36 3636 3333 3237 220a 2020  x="1.6663327".  
-00002330: 2020 2020 2072 793d 2231 2e36 3636 3333       ry="1.66633
-00002340: 3238 2220 2f3e 0a20 2020 203c 6369 7263  28" />.    <circ
-00002350: 6c65 0a20 2020 2020 2020 723d 2231 2e36  le.       r="1.6
-00002360: 3636 3333 3238 220a 2020 2020 2020 2073  663328".       s
-00002370: 7479 6c65 3d22 6f70 6163 6974 793a 313b  tyle="opacity:1;
-00002380: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
-00002390: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
-000023a0: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
-000023b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-000023c0: 2e35 3535 3632 353b 7374 726f 6b65 2d6d  .555625;stroke-m
-000023d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-000023e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-000023f0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-00002400: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-00002410: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-00002420: 643d 2270 6174 6831 3435 3637 2d32 2d38  d="path14567-2-8
-00002430: 220a 2020 2020 2020 2063 783d 2232 342e  ".       cx="24.
-00002440: 3432 3839 3633 220a 2020 2020 2020 2063  428963".       c
-00002450: 793d 2234 372e 3534 3935 3334 2220 2f3e  y="47.549534" />
-00002460: 0a20 2020 203c 666c 6f77 526f 6f74 0a20  .    <flowRoot. 
-00002470: 2020 2020 2020 786d 6c3a 7370 6163 653d        xml:space=
-00002480: 2270 7265 7365 7276 6522 0a20 2020 2020  "preserve".     
-00002490: 2020 6964 3d22 666c 6f77 526f 6f74 3134    id="flowRoot14
-000024a0: 3634 3722 0a20 2020 2020 2020 7374 796c  647".       styl
-000024b0: 653d 2266 6f6e 742d 7374 796c 653a 6e6f  e="font-style:no
-000024c0: 726d 616c 3b66 6f6e 742d 7765 6967 6874  rmal;font-weight
-000024d0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 697a  :normal;font-siz
-000024e0: 653a 3134 2e36 3636 3770 783b 6c69 6e65  e:14.6667px;line
-000024f0: 2d68 6569 6768 743a 312e 3235 3b66 6f6e  -height:1.25;fon
-00002500: 742d 6661 6d69 6c79 3a73 616e 732d 7365  t-family:sans-se
-00002510: 7269 663b 6c65 7474 6572 2d73 7061 6369  rif;letter-spaci
-00002520: 6e67 3a30 7078 3b77 6f72 642d 7370 6163  ng:0px;word-spac
-00002530: 696e 673a 3070 783b 6669 6c6c 3a23 3030  ing:0px;fill:#00
-00002540: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
-00002550: 793a 313b 7374 726f 6b65 3a6e 6f6e 6522  y:1;stroke:none"
-00002560: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-00002570: 6d3d 2273 6361 6c65 2830 2e32 3634 3538  m="scale(0.26458
-00002580: 3333 3329 223e 3c66 6c6f 7752 6567 696f  333)"><flowRegio
-00002590: 6e0a 2020 2020 2020 2020 2069 643d 2266  n.         id="f
-000025a0: 6c6f 7752 6567 696f 6e31 3436 3439 223e  lowRegion14649">
-000025b0: 3c72 6563 740a 2020 2020 2020 2020 2020  <rect.          
-000025c0: 2069 643d 2272 6563 7431 3436 3531 220a   id="rect14651".
-000025d0: 2020 2020 2020 2020 2020 2077 6964 7468             width
-000025e0: 3d22 3339 372e 3039 3537 220a 2020 2020  ="397.0957".    
-000025f0: 2020 2020 2020 2068 6569 6768 743d 2236         height="6
-00002600: 3237 2e33 3236 3732 220a 2020 2020 2020  27.32672".      
-00002610: 2020 2020 2078 3d22 3131 352e 3131 3535       x="115.1155
-00002620: 3122 0a20 2020 2020 2020 2020 2020 793d  1".           y=
-00002630: 2231 3733 2e30 3830 3736 2220 2f3e 3c2f  "173.08076" /></
-00002640: 666c 6f77 5265 6769 6f6e 3e3c 666c 6f77  flowRegion><flow
-00002650: 5061 7261 0a20 2020 2020 2020 2020 6964  Para.         id
-00002660: 3d22 666c 6f77 5061 7261 3134 3635 3322  ="flowPara14653"
-00002670: 202f 3e3c 2f66 6c6f 7752 6f6f 743e 0a20   /></flowRoot>. 
-00002680: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00002690: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-000026a0: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
-000026b0: 3a30 2e39 3938 3430 383b 7374 726f 6b65  :0.998408;stroke
-000026c0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-000026d0: 7769 6474 683a 302e 3137 3132 3234 7078  width:0.171224px
-000026e0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000026f0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00002700: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00002710: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00002720: 2020 2020 643d 226d 2031 3634 2e36 3836      d="m 164.686
-00002730: 3932 2c33 352e 3335 3533 3531 2031 342e  92,35.355351 14.
-00002740: 3034 3539 312c 2d34 2e36 3539 3938 3620  04591,-4.659986 
-00002750: 2d31 342e 3938 3533 332c 2d30 2e37 3832  -14.98533,-0.782
-00002760: 3730 3220 6320 352e 3831 3032 342c 312e  702 c 5.81024,1.
-00002770: 3639 3935 3534 2035 2e38 3336 3635 2c31  699554 5.83665,1
-00002780: 2e37 3839 3530 3320 302e 3933 3934 322c  .789503 0.93942,
-00002790: 352e 3434 3236 3838 207a 220a 2020 2020  5.442688 z".    
-000027a0: 2020 2069 643d 2270 6174 6831 3436 3537     id="path14657
-000027b0: 2d39 220a 2020 2020 2020 2069 6e6b 7363  -9".       inksc
-000027c0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-000027d0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-000027e0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-000027f0: 7479 7065 733d 2263 6363 6322 202f 3e0a  types="cccc" />.
-00002800: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-00002810: 2020 2072 3d22 332e 3136 3734 3533 3822     r="3.1674538"
-00002820: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00002830: 7061 6369 7479 3a31 3b66 696c 6c3a 2365  pacity:1;fill:#e
-00002840: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
-00002850: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-00002860: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00002870: 652d 7769 6474 683a 312e 3035 3631 363b  e-width:1.05616;
-00002880: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00002890: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-000028a0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-000028b0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-000028c0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-000028d0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-000028e0: 3435 3637 2d32 2d37 220a 2020 2020 2020  4567-2-7".      
-000028f0: 2063 783d 2239 302e 3132 3631 3134 220a   cx="90.126114".
-00002900: 2020 2020 2020 2063 793d 2234 312e 3532         cy="41.52
-00002910: 3331 3734 2220 2f3e 0a20 2020 203c 7465  3174" />.    <te
-00002920: 7874 0a20 2020 2020 2020 786d 6c3a 7370  xt.       xml:sp
-00002930: 6163 653d 2270 7265 7365 7276 6522 0a20  ace="preserve". 
-00002940: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
-00002950: 742d 7374 796c 653a 6e6f 726d 616c 3b66  t-style:normal;f
-00002960: 6f6e 742d 7765 6967 6874 3a6e 6f72 6d61  ont-weight:norma
-00002970: 6c3b 666f 6e74 2d73 697a 653a 352e 3837  l;font-size:5.87
-00002980: 3239 3170 783b 6c69 6e65 2d68 6569 6768  291px;line-heigh
-00002990: 743a 312e 3235 3b66 6f6e 742d 6661 6d69  t:1.25;font-fami
-000029a0: 6c79 3a73 616e 732d 7365 7269 663b 6c65  ly:sans-serif;le
-000029b0: 7474 6572 2d73 7061 6369 6e67 3a30 7078  tter-spacing:0px
-000029c0: 3b77 6f72 642d 7370 6163 696e 673a 3070  ;word-spacing:0p
-000029d0: 783b 6669 6c6c 3a23 6666 6666 6666 3b66  x;fill:#ffffff;f
-000029e0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-000029f0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-00002a00: 2d77 6964 7468 3a30 2e34 3030 3432 353b  -width:0.400425;
-00002a10: 6669 6c74 6572 3a75 726c 2823 6669 6c74  filter:url(#filt
-00002a20: 6572 3135 3035 3129 220a 2020 2020 2020  er15051)".      
-00002a30: 2078 3d22 3737 2e36 3934 3839 3322 0a20   x="77.694893". 
-00002a40: 2020 2020 2020 793d 2239 312e 3938 3834        y="91.9884
-00002a50: 3439 220a 2020 2020 2020 2069 643d 2274  49".       id="t
-00002a60: 6578 7431 3436 3931 2d36 220a 2020 2020  ext14691-6".    
-00002a70: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
-00002a80: 7472 6978 2831 2e34 3532 3439 3434 2c30  trix(1.4524944,0
-00002a90: 2c30 2c31 2e34 3532 3439 3434 2c2d 3433  ,0,1.4524944,-43
-00002aa0: 2e36 3833 3731 362c 2d36 302e 3532 3435  .683716,-60.5245
-00002ab0: 3439 2922 3e3c 7473 7061 6e0a 2020 2020  49)"><tspan.    
-00002ac0: 2020 2020 2073 6f64 6970 6f64 693a 726f       sodipodi:ro
-00002ad0: 6c65 3d22 6c69 6e65 220a 2020 2020 2020  le="line".      
-00002ae0: 2020 2069 643d 2274 7370 616e 3134 3638     id="tspan1468
-00002af0: 392d 3222 0a20 2020 2020 2020 2020 783d  9-2".         x=
-00002b00: 2237 372e 3639 3438 3933 220a 2020 2020  "77.694893".    
-00002b10: 2020 2020 2079 3d22 3931 2e39 3838 3434       y="91.98844
-00002b20: 3922 0a20 2020 2020 2020 2020 7374 796c  9".         styl
-00002b30: 653d 2266 6f6e 742d 7374 796c 653a 6e6f  e="font-style:no
-00002b40: 726d 616c 3b66 6f6e 742d 7661 7269 616e  rmal;font-varian
-00002b50: 743a 6e6f 726d 616c 3b66 6f6e 742d 7765  t:normal;font-we
-00002b60: 6967 6874 3a6e 6f72 6d61 6c3b 666f 6e74  ight:normal;font
-00002b70: 2d73 7472 6574 6368 3a6e 6f72 6d61 6c3b  -stretch:normal;
-00002b80: 666f 6e74 2d73 697a 653a 3231 2e33 3536  font-size:21.356
-00002b90: 7078 3b66 6f6e 742d 6661 6d69 6c79 3a49  px;font-family:I
-00002ba0: 6d70 6163 743b 2d69 6e6b 7363 6170 652d  mpact;-inkscape-
-00002bb0: 666f 6e74 2d73 7065 6369 6669 6361 7469  font-specificati
-00002bc0: 6f6e 3a49 6d70 6163 743b 6669 6c6c 3a23  on:Impact;fill:#
-00002bd0: 6666 6666 6666 3b66 696c 6c2d 6f70 6163  ffffff;fill-opac
-00002be0: 6974 793a 313b 7374 726f 6b65 2d77 6964  ity:1;stroke-wid
-00002bf0: 7468 3a30 2e34 3030 3432 3522 3e53 6165  th:0.400425">Sae
-00002c00: 6e6f 7079 3c2f 7473 7061 6e3e 3c2f 7465  nopy</tspan></te
-00002c10: 7874 3e0a 2020 2020 3c74 6578 740a 2020  xt>.    <text.  
-00002c20: 2020 2020 2078 6d6c 3a73 7061 6365 3d22       xml:space="
-00002c30: 7072 6573 6572 7665 220a 2020 2020 2020  preserve".      
-00002c40: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
-00002c50: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
-00002c60: 6569 6768 743a 6e6f 726d 616c 3b66 6f6e  eight:normal;fon
-00002c70: 742d 7369 7a65 3a38 2e35 3330 3336 7078  t-size:8.53036px
-00002c80: 3b6c 696e 652d 6865 6967 6874 3a31 2e32  ;line-height:1.2
-00002c90: 353b 666f 6e74 2d66 616d 696c 793a 7361  5;font-family:sa
-00002ca0: 6e73 2d73 6572 6966 3b6c 6574 7465 722d  ns-serif;letter-
-00002cb0: 7370 6163 696e 673a 3070 783b 776f 7264  spacing:0px;word
-00002cc0: 2d73 7061 6369 6e67 3a30 7078 3b66 696c  -spacing:0px;fil
-00002cd0: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
-00002ce0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00002cf0: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
-00002d00: 683a 302e 3538 3136 3136 220a 2020 2020  h:0.581616".    
-00002d10: 2020 2078 3d22 3638 2e31 3136 3032 3822     x="68.116028"
-00002d20: 0a20 2020 2020 2020 793d 2236 382e 3936  .       y="68.96
-00002d30: 3734 3931 220a 2020 2020 2020 2069 643d  7491".       id=
-00002d40: 2274 6578 7431 3436 3931 223e 3c74 7370  "text14691"><tsp
-00002d50: 616e 0a20 2020 2020 2020 2020 736f 6469  an.         sodi
-00002d60: 706f 6469 3a72 6f6c 653d 226c 696e 6522  podi:role="line"
-00002d70: 0a20 2020 2020 2020 2020 6964 3d22 7473  .         id="ts
-00002d80: 7061 6e31 3436 3839 220a 2020 2020 2020  pan14689".      
-00002d90: 2020 2078 3d22 3638 2e31 3136 3032 3822     x="68.116028"
-00002da0: 0a20 2020 2020 2020 2020 793d 2236 382e  .         y="68.
-00002db0: 3936 3734 3931 220a 2020 2020 2020 2020  967491".        
-00002dc0: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
-00002dd0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
-00002de0: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
-00002df0: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
-00002e00: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
-00002e10: 726d 616c 3b66 6f6e 742d 7369 7a65 3a33  rmal;font-size:3
-00002e20: 312e 3031 3935 7078 3b66 6f6e 742d 6661  1.0195px;font-fa
-00002e30: 6d69 6c79 3a27 546c 7767 2054 7970 6973  mily:'Tlwg Typis
-00002e40: 7427 3b2d 696e 6b73 6361 7065 2d66 6f6e  t';-inkscape-fon
-00002e50: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
-00002e60: 2754 6c77 6720 5479 7069 7374 273b 7374  'Tlwg Typist';st
-00002e70: 726f 6b65 2d77 6964 7468 3a30 2e35 3831  roke-width:0.581
-00002e80: 3631 3622 3e53 6165 6e6f 7079 3c2f 7473  616">Saenopy</ts
-00002e90: 7061 6e3e 3c2f 7465 7874 3e0a 2020 2020  pan></text>.    
-00002ea0: 3c67 0a20 2020 2020 2020 6964 3d22 6739  <g.       id="g9
-00002eb0: 3034 220a 2020 2020 2020 2074 7261 6e73  04".       trans
-00002ec0: 666f 726d 3d22 6d61 7472 6978 2830 2e37  form="matrix(0.7
-00002ed0: 3131 3139 3332 2c30 2c30 2c30 2e37 3131  111932,0,0,0.711
-00002ee0: 3139 3332 2c30 2e35 3033 3139 3732 322c  1932,0.50319722,
-00002ef0: 3337 2e36 3435 3231 3529 223e 0a20 2020  37.645215)">.   
-00002f00: 2020 203c 7265 6374 0a20 2020 2020 2020     <rect.       
-00002f10: 2020 7374 796c 653d 226f 7061 6369 7479    style="opacity
-00002f20: 3a31 3b66 696c 6c3a 2362 3362 3362 333b  :1;fill:#b3b3b3;
-00002f30: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00002f40: 7472 6f6b 653a 6e6f 6e65 3b73 7472 6f6b  troke:none;strok
-00002f50: 652d 7769 6474 683a 302e 3335 3439 3731  e-width:0.354971
-00002f60: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00002f70: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00002f80: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00002f90: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00002fa0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00002fb0: 0a20 2020 2020 2020 2020 6964 3d22 7265  .         id="re
-00002fc0: 6374 3135 3037 342d 3022 0a20 2020 2020  ct15074-0".     
-00002fd0: 2020 2020 7769 6474 683d 2239 352e 3233      width="95.23
-00002fe0: 3930 3036 220a 2020 2020 2020 2020 2068  9006".         h
-00002ff0: 6569 6768 743d 2239 352e 3233 3930 3036  eight="95.239006
-00003000: 220a 2020 2020 2020 2020 2078 3d22 312e  ".         x="1.
-00003010: 3734 3233 3331 3622 0a20 2020 2020 2020  7423316".       
-00003020: 2020 793d 2231 3330 2e33 3437 3422 0a20    y="130.3474". 
-00003030: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00003040: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00003050: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00003060: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00003070: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00003080: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00003090: 7479 6c65 3d22 6669 6c6c 3a23 3365 3462  tyle="fill:#3e4b
-000030a0: 3737 3b66 696c 6c2d 6f70 6163 6974 793a  77;fill-opacity:
-000030b0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-000030c0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000030d0: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-000030e0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-000030f0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00003100: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00003110: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00003120: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00003130: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00003140: 2020 2020 2020 643d 226d 2035 2e37 3538        d="m 5.758
-00003150: 3439 3036 2c31 3631 2e38 3336 3531 2033  4906,161.83651 3
-00003160: 322e 3333 3936 3230 342c 2d31 2e34 3639  2.3396204,-1.469
-00003170: 3938 2032 312e 3234 3739 332c 2d32 332e  98 21.24793,-23.
-00003180: 3635 3333 3520 6320 2d32 362e 3736 3738  65335 c -26.7678
-00003190: 392c 3138 2e30 3031 3837 202d 3339 2e35  9,18.00187 -39.5
-000031a0: 3536 3434 2c32 302e 3839 3039 3520 2d35  5644,20.89095 -5
-000031b0: 332e 3538 3735 3530 342c 3235 2e31 3233  3.5875504,25.123
-000031c0: 3333 207a 220a 2020 2020 2020 2020 2069  33 z".         i
-000031d0: 643d 2270 6174 6831 3435 3437 2d31 220a  d="path14547-1".
-000031e0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-000031f0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00003200: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-00003210: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00003220: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
-00003230: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00003240: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00003250: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00003260: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00003270: 3330 3022 202f 3e0a 2020 2020 2020 3c70  300" />.      <p
-00003280: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
-00003290: 6c65 3d22 6669 6c6c 3a23 3163 3263 3638  le="fill:#1c2c68
-000032a0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-000032b0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-000032c0: 7472 6f6b 652d 7769 6474 683a 302e 3535  troke-width:0.55
-000032d0: 3536 3235 3b73 7472 6f6b 652d 6c69 6e65  5625;stroke-line
-000032e0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-000032f0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00003300: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00003310: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00003320: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00003330: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00003340: 2020 2020 643d 226d 2033 382e 3039 3831      d="m 38.0981
-00003350: 3131 2c31 3630 2e33 3636 3533 2031 342e  11,160.36653 14.
-00003360: 3033 3136 352c 332e 3230 3732 3420 372e  03165,3.20724 7.
-00003370: 3231 3632 382c 2d32 362e 3836 3035 3920  21628,-26.86059 
-00003380: 7a22 0a20 2020 2020 2020 2020 6964 3d22  z".         id="
-00003390: 7061 7468 3134 3534 392d 3122 0a20 2020  path14549-1".   
-000033a0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-000033b0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-000033c0: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
-000033d0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-000033e0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-000033f0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00003400: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-00003410: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
-00003420: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00003430: 6c6c 3a23 3036 3035 3038 3b66 696c 6c2d  ll:#060508;fill-
-00003440: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00003450: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00003460: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
-00003470: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00003480: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00003490: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-000034a0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-000034b0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-000034c0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-000034d0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-000034e0: 226d 2035 322e 3132 3937 3631 2c31 3633  "m 52.129761,163
-000034f0: 2e35 3733 3737 2033 372e 3535 3133 372c  .57377 37.55137,
-00003500: 362e 3638 3137 3420 6320 2d31 342e 3633  6.68174 c -14.63
-00003510: 3331 322c 2d37 2e37 3335 3839 202d 3233  312,-7.73589 -23
-00003520: 2e31 3036 3934 2c2d 3230 2e31 3634 3536  .10694,-20.16456
-00003530: 202d 3330 2e33 3335 3039 2c2d 3333 2e35   -30.33509,-33.5
-00003540: 3432 3333 207a 220a 2020 2020 2020 2020  4233 z".        
-00003550: 2069 643d 2270 6174 6831 3435 3531 2d30   id="path14551-0
-00003560: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00003570: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00003580: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-00003590: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-000035a0: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
-000035b0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000035c0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-000035d0: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-000035e0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-000035f0: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00003600: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00003610: 7479 6c65 3d22 6669 6c6c 3a23 3237 3337  tyle="fill:#2737
-00003620: 3733 3b66 696c 6c2d 6f70 6163 6974 793a  73;fill-opacity:
-00003630: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00003640: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00003650: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-00003660: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00003670: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00003680: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00003690: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-000036a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000036b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000036c0: 2020 2020 2020 643d 226d 2035 2e37 3538        d="m 5.758
-000036d0: 3439 3036 2c31 3631 2e38 3336 3531 2063  4906,161.83651 c
-000036e0: 2037 2e31 3136 3432 3034 2c34 2e30 3832   7.1164204,4.082
-000036f0: 3434 2031 342e 3936 3237 3230 342c 372e  44 14.9627204,7.
-00003700: 3630 3334 3320 3137 2e36 3339 3739 3034  60343 17.6397904
-00003710: 2c31 352e 3130 3037 3420 6c20 3134 2e36  ,15.10074 l 14.6
-00003720: 3939 3833 2c2d 3136 2e35 3730 3732 207a  9983,-16.57072 z
-00003730: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
-00003740: 6174 6831 3435 3533 2d33 220a 2020 2020  ath14553-3".    
-00003750: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00003760: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-00003770: 653d 2230 220a 2020 2020 2020 2020 2073  e="0".         s
-00003780: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00003790: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
-000037a0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-000037b0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-000037c0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-000037d0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-000037e0: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
-000037f0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00003800: 6669 6c6c 3a23 3134 3236 3732 3b66 696c  fill:#142672;fil
-00003810: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00003820: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00003830: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00003840: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00003850: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00003860: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00003870: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00003880: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00003890: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-000038a0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-000038b0: 643d 226d 2032 332e 3339 3832 3831 2c31  d="m 23.398281,1
-000038c0: 3736 2e39 3337 3235 2036 362e 3238 3238  76.93725 66.2828
-000038d0: 352c 2d36 2e36 3831 3734 202d 3531 2e35  5,-6.68174 -51.5
-000038e0: 3833 3032 2c2d 392e 3838 3839 3820 7a22  8302,-9.88898 z"
-000038f0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00003900: 7468 3134 3535 352d 3422 0a20 2020 2020  th14555-4".     
-00003910: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-00003920: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-00003930: 3d22 3022 0a20 2020 2020 2020 2020 696e  ="0".         in
-00003940: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-00003950: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-00003960: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00003970: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-00003980: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
-00003990: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000039a0: 3a23 3534 3636 3863 3b66 696c 6c2d 6f70  :#54668c;fill-op
-000039b0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-000039c0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-000039d0: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
-000039e0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-000039f0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00003a00: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-00003a10: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00003a20: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00003a30: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00003a40: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
-00003a50: 2032 332e 3339 3832 3831 2c31 3736 2e39   23.398281,176.9
-00003a60: 3337 3235 2033 382e 3231 3935 352c 342e  3725 38.21955,4.
-00003a70: 3030 3930 3420 3238 2e30 3633 332c 2d31  00904 28.0633,-1
-00003a80: 302e 3639 3037 3820 7a22 0a20 2020 2020  0.69078 z".     
-00003a90: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
-00003aa0: 372d 3022 0a20 2020 2020 2020 2020 696e  7-0".         in
-00003ab0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00003ac0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00003ad0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00003ae0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00003af0: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00003b00: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00003b10: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00003b20: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00003b30: 7479 6c65 3d22 6669 6c6c 3a23 3232 3334  tyle="fill:#2234
-00003b40: 3765 3b66 696c 6c2d 6f70 6163 6974 793a  7e;fill-opacity:
-00003b50: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00003b60: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00003b70: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-00003b80: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00003b90: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00003ba0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00003bb0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00003bc0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00003bd0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00003be0: 2020 2020 2020 643d 226d 2032 332e 3339        d="m 23.39
-00003bf0: 3832 3831 2c31 3736 2e39 3337 3235 2063  8281,176.93725 c
-00003c00: 2030 2e38 3539 3432 2c37 2e34 3130 3134   0.85942,7.41014
-00003c10: 202d 322e 3131 3533 372c 3132 2e30 3831   -2.11537,12.081
-00003c20: 3537 202d 332e 3437 3435 2c31 372e 3930  57 -3.4745,17.90
-00003c30: 3730 3520 6c20 3431 2e36 3934 3035 2c2d  705 l 41.69405,-
-00003c40: 3133 2e38 3938 3031 207a 220a 2020 2020  13.89801 z".    
-00003c50: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00003c60: 3539 2d33 220a 2020 2020 2020 2020 2069  59-3".         i
-00003c70: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-00003c80: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-00003c90: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00003ca0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-00003cb0: 6322 0a20 2020 2020 2020 2020 696e 6b73  c".         inks
-00003cc0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-00003cd0: 3d22 3330 3022 0a20 2020 2020 2020 2020  ="300".         
-00003ce0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00003cf0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00003d00: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00003d10: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00003d20: 3038 3130 3639 3b66 696c 6c2d 6f70 6163  081069;fill-opac
-00003d30: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-00003d40: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-00003d50: 683a 302e 3535 3536 3235 3b73 7472 6f6b  h:0.555625;strok
-00003d60: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00003d70: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00003d80: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00003d90: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00003da0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00003db0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00003dc0: 0a20 2020 2020 2020 2020 643d 226d 2031  .         d="m 1
-00003dd0: 392e 3932 3337 3831 2c31 3934 2e38 3434  9.923781,194.844
-00003de0: 3320 3238 2e38 3635 3131 2c34 2e32 3736  3 28.86511,4.276
-00003df0: 3332 2034 302e 3839 3232 342c 2d32 382e  32 40.89224,-28.
-00003e00: 3836 3531 3120 7a22 0a20 2020 2020 2020  86511 z".       
-00003e10: 2020 6964 3d22 7061 7468 3134 3536 312d    id="path14561-
-00003e20: 3922 0a20 2020 2020 2020 2020 696e 6b73  9".         inks
-00003e30: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00003e40: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-00003e50: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00003e60: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00003e70: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00003e80: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00003e90: 3330 3022 202f 3e0a 2020 2020 2020 3c70  300" />.      <p
-00003ea0: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
-00003eb0: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
-00003ec0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00003ed0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00003ee0: 7472 6f6b 652d 7769 6474 683a 302e 3535  troke-width:0.55
-00003ef0: 3536 3235 3b73 7472 6f6b 652d 6c69 6e65  5625;stroke-line
-00003f00: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00003f10: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00003f20: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00003f30: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00003f40: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00003f50: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00003f60: 2020 2020 643d 226d 2034 382e 3738 3838      d="m 48.7888
-00003f70: 3931 2c31 3939 2e31 3230 3632 2031 362e  91,199.12062 16.
-00003f80: 3937 3136 312c 3232 2e33 3137 3031 202d  97161,22.31701 -
-00003f90: 362e 3238 3038 332c 2d33 302e 3036 3738  6.28083,-30.0678
-00003fa0: 3220 7a22 0a20 2020 2020 2020 2020 6964  2 z".         id
-00003fb0: 3d22 7061 7468 3134 3536 332d 3122 0a20  ="path14563-1". 
-00003fc0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00003fd0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-00003fe0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-00003ff0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00004000: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-00004010: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00004020: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00004030: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
-00004040: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00004050: 6669 6c6c 3a23 3238 3364 3837 3b66 696c  fill:#283d87;fil
-00004060: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00004070: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00004080: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00004090: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000040a0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-000040b0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-000040c0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-000040d0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-000040e0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-000040f0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00004100: 643d 226d 2035 392e 3437 3936 3731 2c31  d="m 59.479671,1
-00004110: 3931 2e33 3639 3831 2036 2e32 3830 3833  91.36981 6.28083
-00004120: 2c33 302e 3036 3738 3220 6320 332e 3235  ,30.06782 c 3.25
-00004130: 3134 352c 2d32 372e 3032 3935 3720 3134  145,-27.02957 14
-00004140: 2e36 3933 3635 2c2d 3336 2e37 3637 3536  .69365,-36.76756
-00004150: 2032 332e 3932 3036 332c 2d35 312e 3138   23.92063,-51.18
-00004160: 3231 3220 7a22 0a20 2020 2020 2020 2020  212 z".         
-00004170: 6964 3d22 7061 7468 3134 3536 352d 3922  id="path14565-9"
-00004180: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00004190: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-000041a0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-000041b0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-000041c0: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
-000041d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000041e0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-000041f0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00004200: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-00004210: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-00004220: 656c 6c69 7073 650a 2020 2020 2020 2020  ellipse.        
-00004230: 2073 7479 6c65 3d22 6f70 6163 6974 793a   style="opacity:
-00004240: 313b 6669 6c6c 3a23 3037 3065 3262 3b66  1;fill:#070e2b;f
-00004250: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
-00004260: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
-00004270: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00004280: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
-00004290: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-000042a0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-000042b0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-000042c0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-000042d0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-000042e0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-000042f0: 2d36 220a 2020 2020 2020 2020 2063 783d  -6".         cx=
-00004300: 2236 2e34 3434 3836 3238 220a 2020 2020  "6.4448628".    
-00004310: 2020 2020 2063 793d 2231 3631 2e38 3730       cy="161.870
-00004320: 3832 220a 2020 2020 2020 2020 2072 783d  82".         rx=
-00004330: 2231 2e36 3636 3333 3237 220a 2020 2020  "1.6663327".    
-00004340: 2020 2020 2072 793d 2231 2e36 3636 3333       ry="1.66633
-00004350: 3238 220a 2020 2020 2020 2020 2069 6e6b  28".         ink
-00004360: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00004370: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
-00004380: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00004390: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-000043a0: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
-000043b0: 2020 2020 2020 723d 2231 2e36 3636 3333        r="1.66633
-000043c0: 3238 220a 2020 2020 2020 2020 2073 7479  28".         sty
-000043d0: 6c65 3d22 6f70 6163 6974 793a 313b 6669  le="opacity:1;fi
-000043e0: 6c6c 3a23 3235 3361 3764 3b66 696c 6c2d  ll:#253a7d;fill-
-000043f0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00004400: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00004410: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
-00004420: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00004430: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00004440: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00004450: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00004460: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00004470: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00004480: 3134 3536 372d 332d 3933 220a 2020 2020  14567-3-93".    
-00004490: 2020 2020 2063 783d 2231 392e 3635 3536       cx="19.6556
-000044a0: 3332 220a 2020 2020 2020 2020 2063 793d  32".         cy=
-000044b0: 2231 3934 2e34 3838 3835 220a 2020 2020  "194.48885".    
-000044c0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-000044d0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
-000044e0: 3d22 342e 3634 3332 3536 3622 0a20 2020  ="4.6432566".   
-000044f0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-00004500: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-00004510: 793d 222d 392e 3937 3830 3632 3122 0a20  y="-9.9780621". 
-00004520: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00004530: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00004540: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00004550: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00004560: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00004570: 3c63 6972 636c 650a 2020 2020 2020 2020  <circle.        
-00004580: 2072 3d22 312e 3636 3633 3332 3822 0a20   r="1.6663328". 
-00004590: 2020 2020 2020 2020 7374 796c 653d 226f          style="o
-000045a0: 7061 6369 7479 3a31 3b66 696c 6c3a 2332  pacity:1;fill:#2
-000045b0: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
-000045c0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-000045d0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-000045e0: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
-000045f0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00004600: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00004610: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-00004620: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-00004630: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00004640: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-00004650: 2d33 2d37 2d33 220a 2020 2020 2020 2020  -3-7-3".        
-00004660: 2063 783d 2235 392e 3037 3339 3231 220a   cx="59.073921".
-00004670: 2020 2020 2020 2020 2063 793d 2231 3831           cy="181
-00004680: 2e30 3533 3031 220a 2020 2020 2020 2020  .05301".        
-00004690: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-000046a0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 342e  orm-center-x="4.
-000046b0: 3634 3332 3536 3622 0a20 2020 2020 2020  6432566".       
-000046c0: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-000046d0: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
-000046e0: 392e 3937 3830 3632 3122 0a20 2020 2020  9.9780621".     
-000046f0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00004700: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00004710: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00004720: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00004730: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
-00004740: 636c 650a 2020 2020 2020 2020 2072 3d22  cle.         r="
-00004750: 312e 3636 3633 3332 3822 0a20 2020 2020  1.6663328".     
-00004760: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
-00004770: 7479 3a31 3b66 696c 6c3a 2361 3861 3961  ty:1;fill:#a8a9a
-00004780: 613b 6669 6c6c 2d6f 7061 6369 7479 3a31  a;fill-opacity:1
-00004790: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-000047a0: 7374 726f 6b65 2d77 6964 7468 3a30 2e35  stroke-width:0.5
-000047b0: 3535 3632 353b 7374 726f 6b65 2d6d 6974  55625;stroke-mit
-000047c0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-000047d0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-000047e0: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-000047f0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-00004800: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
-00004810: 643d 2270 6174 6831 3435 3637 2d33 2d35  d="path14567-3-5
-00004820: 2d38 220a 2020 2020 2020 2020 2063 783d  -8".         cx=
-00004830: 2235 392e 3436 3930 3933 220a 2020 2020  "59.469093".    
-00004840: 2020 2020 2063 793d 2231 3931 2e31 3239       cy="191.129
-00004850: 3837 220a 2020 2020 2020 2020 2069 6e6b  87".         ink
-00004860: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
-00004870: 6365 6e74 6572 2d78 3d22 342e 3634 3332  center-x="4.6432
-00004880: 3536 3622 0a20 2020 2020 2020 2020 696e  566".         in
-00004890: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-000048a0: 2d63 656e 7465 722d 793d 222d 392e 3937  -center-y="-9.97
-000048b0: 3830 3632 3122 0a20 2020 2020 2020 2020  80621".         
-000048c0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-000048d0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-000048e0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-000048f0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-00004900: 3e0a 2020 2020 2020 3c63 6972 636c 650a  >.      <circle.
-00004910: 2020 2020 2020 2020 2072 3d22 312e 3636           r="1.66
-00004920: 3633 3332 3822 0a20 2020 2020 2020 2020  63328".         
-00004930: 7374 796c 653d 226f 7061 6369 7479 3a31  style="opacity:1
-00004940: 3b66 696c 6c3a 2361 6261 6139 633b 6669  ;fill:#abaa9c;fi
-00004950: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-00004960: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-00004970: 6b65 2d77 6964 7468 3a30 2e35 3535 3632  ke-width:0.55562
-00004980: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-00004990: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-000049a0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-000049b0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-000049c0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-000049d0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
-000049e0: 6174 6831 3435 3637 2d33 2d39 2d30 220a  ath14567-3-9-0".
-000049f0: 2020 2020 2020 2020 2063 783d 2234 392e           cx="49.
-00004a00: 3139 3436 3439 220a 2020 2020 2020 2020  194649".        
-00004a10: 2063 793d 2231 3939 2e30 3333 3238 220a   cy="199.03328".
-00004a20: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00004a30: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-00004a40: 6572 2d78 3d22 342e 3634 3332 3536 3622  er-x="4.6432566"
-00004a50: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00004a60: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-00004a70: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
-00004a80: 3122 0a20 2020 2020 2020 2020 696e 6b73  1".         inks
-00004a90: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-00004aa0: 3d22 3330 3022 0a20 2020 2020 2020 2020  ="300".         
-00004ab0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00004ac0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00004ad0: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-00004ae0: 2020 2020 2072 3d22 322e 3537 3137 3531       r="2.571751
-00004af0: 3122 0a20 2020 2020 2020 2020 7374 796c  1".         styl
-00004b00: 653d 226f 7061 6369 7479 3a31 3b66 696c  e="opacity:1;fil
-00004b10: 6c3a 2331 3132 3036 363b 6669 6c6c 2d6f  l:#112066;fill-o
-00004b20: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00004b30: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00004b40: 6964 7468 3a30 2e35 3535 3632 353b 7374  idth:0.555625;st
-00004b50: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00004b60: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00004b70: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00004b80: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00004b90: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00004ba0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00004bb0: 3435 3637 2d33 2d32 2d35 220a 2020 2020  4567-3-2-5".    
-00004bc0: 2020 2020 2063 783d 2233 382e 3332 3734       cx="38.3274
-00004bd0: 3436 220a 2020 2020 2020 2020 2063 793d  46".         cy=
-00004be0: 2231 3630 2e30 3130 3138 220a 2020 2020  "160.01018".    
-00004bf0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-00004c00: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
-00004c10: 3d22 372e 3136 3632 3131 3622 0a20 2020  ="7.1662116".   
-00004c20: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-00004c30: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-00004c40: 793d 222d 3135 2e33 3939 3735 3122 0a20  y="-15.399751". 
-00004c50: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00004c60: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00004c70: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00004c80: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00004c90: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00004ca0: 3c63 6972 636c 650a 2020 2020 2020 2020  <circle.        
-00004cb0: 2072 3d22 312e 3636 3633 3332 3822 0a20   r="1.6663328". 
-00004cc0: 2020 2020 2020 2020 7374 796c 653d 226f          style="o
-00004cd0: 7061 6369 7479 3a31 3b66 696c 6c3a 2365  pacity:1;fill:#e
-00004ce0: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
-00004cf0: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-00004d00: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00004d10: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00004d20: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00004d30: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00004d40: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00004d50: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00004d60: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00004d70: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00004d80: 7468 3134 3536 372d 322d 3622 0a20 2020  th14567-2-6".   
-00004d90: 2020 2020 2020 6378 3d22 3532 2e32 3537        cx="52.257
-00004da0: 3232 3522 0a20 2020 2020 2020 2020 6379  225".         cy
-00004db0: 3d22 3136 322e 3837 3531 3722 0a20 2020  ="162.87517".   
-00004dc0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00004dd0: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00004de0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00004df0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00004e00: 3330 3022 202f 3e0a 2020 2020 2020 3c63  300" />.      <c
-00004e10: 6972 636c 650a 2020 2020 2020 2020 2072  ircle.         r
-00004e20: 3d22 312e 3636 3633 3332 3822 0a20 2020  ="1.6663328".   
-00004e30: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
-00004e40: 6369 7479 3a31 3b66 696c 6c3a 2365 6466  city:1;fill:#edf
-00004e50: 3066 633b 6669 6c6c 2d6f 7061 6369 7479  0fc;fill-opacity
-00004e60: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
-00004e70: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00004e80: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
-00004e90: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00004ea0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00004eb0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00004ec0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00004ed0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00004ee0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00004ef0: 3134 3536 372d 322d 382d 3622 0a20 2020  14567-2-8-6".   
-00004f00: 2020 2020 2020 6378 3d22 3233 2e34 3039        cx="23.409
-00004f10: 3735 3222 0a20 2020 2020 2020 2020 6379  752".         cy
-00004f20: 3d22 3137 362e 3730 3631 3522 0a20 2020  ="176.70615".   
-00004f30: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00004f40: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00004f50: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00004f60: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00004f70: 3330 3022 202f 3e0a 2020 2020 2020 3c63  300" />.      <c
-00004f80: 6972 636c 650a 2020 2020 2020 2020 2072  ircle.         r
-00004f90: 3d22 332e 3136 3734 3533 3822 0a20 2020  ="3.1674538".   
-00004fa0: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
-00004fb0: 6369 7479 3a31 3b66 696c 6c3a 2365 6466  city:1;fill:#edf
-00004fc0: 3066 633b 6669 6c6c 2d6f 7061 6369 7479  0fc;fill-opacity
-00004fd0: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
-00004fe0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00004ff0: 7769 6474 683a 312e 3035 3631 363b 7374  width:1.05616;st
-00005000: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00005010: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00005020: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00005030: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00005040: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00005050: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00005060: 3435 3637 2d32 2d37 2d30 220a 2020 2020  4567-2-7-0".    
-00005070: 2020 2020 2063 783d 2238 392e 3130 3638       cx="89.1068
-00005080: 3935 220a 2020 2020 2020 2020 2063 793d  95".         cy=
-00005090: 2231 3730 2e36 3739 3739 220a 2020 2020  "170.67979".    
-000050a0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-000050b0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-000050c0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-000050d0: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-000050e0: 3030 2220 2f3e 0a20 2020 203c 2f67 3e0a  00" />.    </g>.
-000050f0: 2020 2020 3c72 6563 740a 2020 2020 2020      <rect.      
-00005100: 2073 7479 6c65 3d22 6669 6c6c 3a23 6233   style="fill:#b3
-00005110: 6233 6233 3b66 696c 6c2d 6f70 6163 6974  b3b3;fill-opacit
-00005120: 793a 313b 7374 726f 6b65 3a6e 6f6e 653b  y:1;stroke:none;
-00005130: 7374 726f 6b65 2d77 6964 7468 3a30 2e32  stroke-width:0.2
-00005140: 3634 3538 333b 7374 726f 6b65 2d6d 6974  64583;stroke-mit
-00005150: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00005160: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00005170: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-00005180: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-00005190: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-000051a0: 2272 6563 7431 3530 3734 2d30 2d39 220a  "rect15074-0-9".
-000051b0: 2020 2020 2020 2077 6964 7468 3d22 3333         width="33
-000051c0: 2e38 3636 3636 3522 0a20 2020 2020 2020  .866665".       
-000051d0: 6865 6967 6874 3d22 3333 2e38 3636 3636  height="33.86666
-000051e0: 3522 0a20 2020 2020 2020 783d 2237 392e  5".       x="79.
-000051f0: 3835 3132 3822 0a20 2020 2020 2020 793d  85128".       y=
-00005200: 2231 3331 2e34 3339 3031 220a 2020 2020  "131.43901".    
-00005210: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-00005220: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
-00005230: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-00005240: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-00005250: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00005260: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00005270: 2333 6534 6237 373b 6669 6c6c 2d6f 7061  #3e4b77;fill-opa
-00005280: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00005290: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000052a0: 7468 3a30 2e32 3634 3538 333b 7374 726f  th:0.264583;stro
-000052b0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000052c0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000052d0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-000052e0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-000052f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00005300: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00005310: 220a 2020 2020 2020 2064 3d22 6d20 3831  ".       d="m 81
-00005320: 2e32 3739 3431 2c31 3432 2e36 3336 3433  .27941,142.63643
-00005330: 2031 312e 3439 3938 3539 2c2d 302e 3532   11.499859,-0.52
-00005340: 3237 3220 372e 3535 3536 3931 2c2d 382e  272 7.555691,-8.
-00005350: 3431 3130 3520 6320 2d39 2e35 3138 3537  41105 c -9.51857
-00005360: 2c36 2e34 3031 3420 2d31 342e 3036 3631  ,6.4014 -14.0661
-00005370: 3335 2c37 2e34 3238 3735 202d 3139 2e30  35,7.42875 -19.0
-00005380: 3535 3535 2c38 2e39 3333 3737 207a 220a  5555,8.93377 z".
-00005390: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-000053a0: 3435 3437 2d31 2d37 220a 2020 2020 2020  4547-1-7".      
-000053b0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-000053c0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-000053d0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
-000053e0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-000053f0: 6322 0a20 2020 2020 2020 696e 6b73 6361  c".       inksca
-00005400: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00005410: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-00005420: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00005430: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-00005440: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-00005450: 3d22 6669 6c6c 3a23 3163 3263 3638 3b66  ="fill:#1c2c68;f
+00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
+00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
+00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
+00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
+00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
+00000080: 2234 3030 220a 2020 2068 6569 6768 743d  "400".   height=
+00000090: 2232 3030 220a 2020 2076 6965 7742 6f78  "200".   viewBox
+000000a0: 3d22 3020 3020 3430 3020 3230 3022 0a20  ="0 0 400 200". 
+000000b0: 2020 7665 7273 696f 6e3d 2231 2e31 220a    version="1.1".
+000000c0: 2020 2069 643d 2273 7667 3522 0a20 2020     id="svg5".   
+000000d0: 696e 6b73 6361 7065 3a76 6572 7369 6f6e  inkscape:version
+000000e0: 3d22 312e 322e 3220 2837 3332 6130 3164  ="1.2.2 (732a01d
+000000f0: 6136 332c 2032 3032 322d 3132 2d30 392c  a63, 2022-12-09,
+00000100: 2063 7573 746f 6d29 220a 2020 2073 6f64   custom)".   sod
+00000110: 6970 6f64 693a 646f 636e 616d 653d 224c  ipodi:docname="L
+00000120: 6f67 6f2e 7376 6722 0a20 2020 786d 6c6e  ogo.svg".   xmln
+00000130: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
+00000140: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
+00000150: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
+00000160: 6e6b 7363 6170 6522 0a20 2020 786d 6c6e  nkscape".   xmln
+00000170: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
+00000180: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
+00000190: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
+000001a0: 736f 6469 706f 6469 2d30 2e64 7464 220a  sodipodi-0.dtd".
+000001b0: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
+000001c0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+000001d0: 2f73 7667 220a 2020 2078 6d6c 6e73 3a73  /svg".   xmlns:s
+000001e0: 7667 3d22 6874 7470 3a2f 2f77 7777 2e77  vg="http://www.w
+000001f0: 332e 6f72 672f 3230 3030 2f73 7667 223e  3.org/2000/svg">
+00000200: 0a20 203c 736f 6469 706f 6469 3a6e 616d  .  <sodipodi:nam
+00000210: 6564 7669 6577 0a20 2020 2020 6964 3d22  edview.     id="
+00000220: 6e61 6d65 6476 6965 7737 220a 2020 2020  namedview7".    
+00000230: 2070 6167 6563 6f6c 6f72 3d22 2361 6161   pagecolor="#aaa
+00000240: 6161 6122 0a20 2020 2020 626f 7264 6572  aaa".     border
+00000250: 636f 6c6f 723d 2223 3636 3636 3636 220a  color="#666666".
+00000260: 2020 2020 2062 6f72 6465 726f 7061 6369       borderopaci
+00000270: 7479 3d22 312e 3022 0a20 2020 2020 696e  ty="1.0".     in
+00000280: 6b73 6361 7065 3a73 686f 7770 6167 6573  kscape:showpages
+00000290: 6861 646f 773d 2232 220a 2020 2020 2069  hadow="2".     i
+000002a0: 6e6b 7363 6170 653a 7061 6765 6f70 6163  nkscape:pageopac
+000002b0: 6974 793d 2230 220a 2020 2020 2069 6e6b  ity="0".     ink
+000002c0: 7363 6170 653a 7061 6765 6368 6563 6b65  scape:pagechecke
+000002d0: 7262 6f61 7264 3d22 6661 6c73 6522 0a20  rboard="false". 
+000002e0: 2020 2020 696e 6b73 6361 7065 3a64 6573      inkscape:des
+000002f0: 6b63 6f6c 6f72 3d22 2364 3164 3164 3122  kcolor="#d1d1d1"
+00000300: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
+00000310: 6f63 756d 656e 742d 756e 6974 733d 2270  ocument-units="p
+00000320: 7822 0a20 2020 2020 7368 6f77 6772 6964  x".     showgrid
+00000330: 3d22 6661 6c73 6522 0a20 2020 2020 696e  ="false".     in
+00000340: 6b73 6361 7065 3a7a 6f6f 6d3d 2230 2e37  kscape:zoom="0.7
+00000350: 3732 3437 3733 3522 0a20 2020 2020 696e  7247735".     in
+00000360: 6b73 6361 7065 3a63 783d 2234 3236 2e35  kscape:cx="426.5
+00000370: 3439 3733 220a 2020 2020 2069 6e6b 7363  4973".     inksc
+00000380: 6170 653a 6379 3d22 3237 322e 3439 3939  ape:cy="272.4999
+00000390: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+000003a0: 7769 6e64 6f77 2d77 6964 7468 3d22 3138  window-width="18
+000003b0: 3436 220a 2020 2020 2069 6e6b 7363 6170  46".     inkscap
+000003c0: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
+000003d0: 2231 3031 3622 0a20 2020 2020 696e 6b73  "1016".     inks
+000003e0: 6361 7065 3a77 696e 646f 772d 783d 2237  cape:window-x="7
+000003f0: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
+00000400: 3a77 696e 646f 772d 793d 2232 3722 0a20  :window-y="27". 
+00000410: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+00000420: 646f 772d 6d61 7869 6d69 7a65 643d 2231  dow-maximized="1
+00000430: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000440: 6375 7272 656e 742d 6c61 7965 723d 226c  current-layer="l
+00000450: 6179 6572 3122 3e0a 2020 2020 3c69 6e6b  ayer1">.    <ink
+00000460: 7363 6170 653a 7061 6765 0a20 2020 2020  scape:page.     
+00000470: 2020 783d 2230 220a 2020 2020 2020 2079    x="0".       y
+00000480: 3d22 3022 0a20 2020 2020 2020 7769 6474  ="0".       widt
+00000490: 683d 2234 3030 220a 2020 2020 2020 2068  h="400".       h
+000004a0: 6569 6768 743d 2232 3030 220a 2020 2020  eight="200".    
+000004b0: 2020 2069 643d 2270 6167 6533 3236 220a     id="page326".
+000004c0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000004d0: 6c61 6265 6c3d 224c 6f67 6f22 202f 3e0a  label="Logo" />.
+000004e0: 2020 2020 3c69 6e6b 7363 6170 653a 7061      <inkscape:pa
+000004f0: 6765 0a20 2020 2020 2020 783d 222d 302e  ge.       x="-0.
+00000500: 3638 3031 3539 3633 220a 2020 2020 2020  68015963".      
+00000510: 2079 3d22 3235 302e 3632 3835 3422 0a20   y="250.62854". 
+00000520: 2020 2020 2020 7769 6474 683d 2232 3536        width="256
+00000530: 220a 2020 2020 2020 2068 6569 6768 743d  ".       height=
+00000540: 2232 3536 220a 2020 2020 2020 2069 643d  "256".       id=
+00000550: 2270 6167 6533 3238 220a 2020 2020 2020  "page328".      
+00000560: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
+00000570: 2249 636f 6e32 3536 2220 2f3e 0a20 2020  "Icon256" />.   
+00000580: 203c 696e 6b73 6361 7065 3a70 6167 650a   <inkscape:page.
+00000590: 2020 2020 2020 2078 3d22 3331 312e 3635         x="311.65
+000005a0: 3437 3222 0a20 2020 2020 2020 793d 2232  472".       y="2
+000005b0: 3539 2e34 3130 3433 220a 2020 2020 2020  59.41043".      
+000005c0: 2077 6964 7468 3d22 3132 3822 0a20 2020   width="128".   
+000005d0: 2020 2020 6865 6967 6874 3d22 3132 3822      height="128"
+000005e0: 0a20 2020 2020 2020 6964 3d22 7061 6765  .       id="page
+000005f0: 3338 3122 0a20 2020 2020 2020 696e 6b73  381".       inks
+00000600: 6361 7065 3a6c 6162 656c 3d22 4963 6f6e  cape:label="Icon
+00000610: 3132 3822 202f 3e0a 2020 2020 3c69 6e6b  128" />.    <ink
+00000620: 7363 6170 653a 7061 6765 0a20 2020 2020  scape:page.     
+00000630: 2020 783d 2233 3136 2e32 3732 3634 220a    x="316.27264".
+00000640: 2020 2020 2020 2079 3d22 3431 382e 3937         y="418.97
+00000650: 3837 3622 0a20 2020 2020 2020 7769 6474  876".       widt
+00000660: 683d 2236 3422 0a20 2020 2020 2020 6865  h="64".       he
+00000670: 6967 6874 3d22 3634 220a 2020 2020 2020  ight="64".      
+00000680: 2069 643d 2270 6167 6533 3833 220a 2020   id="page383".  
+00000690: 2020 2020 2069 6e6b 7363 6170 653a 6c61       inkscape:la
+000006a0: 6265 6c3d 2249 636f 6e36 3422 0a20 2020  bel="Icon64".   
+000006b0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+000006c0: 6f72 742d 6669 6c65 6e61 6d65 3d22 2e2f  ort-filename="./
+000006d0: 4963 6f6e 3634 2e70 6e67 220a 2020 2020  Icon64.png".    
+000006e0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+000006f0: 7274 2d78 6470 693d 2239 3622 0a20 2020  rt-xdpi="96".   
+00000700: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00000710: 6f72 742d 7964 7069 3d22 3936 2220 2f3e  ort-ydpi="96" />
+00000720: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
+00000730: 6167 650a 2020 2020 2020 2078 3d22 3436  age.       x="46
+00000740: 382e 3832 3332 3422 0a20 2020 2020 2020  8.82324".       
+00000750: 793d 2232 3631 2e33 3132 3431 220a 2020  y="261.31241".  
+00000760: 2020 2020 2077 6964 7468 3d22 3332 220a       width="32".
+00000770: 2020 2020 2020 2068 6569 6768 743d 2233         height="3
+00000780: 3222 0a20 2020 2020 2020 6964 3d22 7061  2".       id="pa
+00000790: 6765 3338 3522 0a20 2020 2020 2020 696e  ge385".       in
+000007a0: 6b73 6361 7065 3a6c 6162 656c 3d22 4963  kscape:label="Ic
+000007b0: 6f6e 3332 2220 2f3e 0a20 2020 203c 696e  on32" />.    <in
+000007c0: 6b73 6361 7065 3a70 6167 650a 2020 2020  kscape:page.    
+000007d0: 2020 2078 3d22 3437 302e 3931 3434 3322     x="470.91443"
+000007e0: 0a20 2020 2020 2020 793d 2233 3236 2e30  .       y="326.0
+000007f0: 3831 3032 220a 2020 2020 2020 2077 6964  8102".       wid
+00000800: 7468 3d22 3136 220a 2020 2020 2020 2068  th="16".       h
+00000810: 6569 6768 743d 2231 3622 0a20 2020 2020  eight="16".     
+00000820: 2020 6964 3d22 7061 6765 3338 3722 0a20    id="page387". 
+00000830: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
+00000840: 6162 656c 3d22 4963 6f6e 3136 2220 2f3e  abel="Icon16" />
+00000850: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
+00000860: 6167 650a 2020 2020 2020 2078 3d22 3430  age.       x="40
+00000870: 352e 3639 3738 3122 0a20 2020 2020 2020  5.69781".       
+00000880: 793d 2234 3236 2e31 3333 3234 220a 2020  y="426.13324".  
+00000890: 2020 2020 2077 6964 7468 3d22 3438 220a       width="48".
+000008a0: 2020 2020 2020 2068 6569 6768 743d 2234         height="4
+000008b0: 3822 0a20 2020 2020 2020 6964 3d22 7061  8".       id="pa
+000008c0: 6765 3738 3032 220a 2020 2020 2020 2069  ge7802".       i
+000008d0: 6e6b 7363 6170 653a 6c61 6265 6c3d 2249  nkscape:label="I
+000008e0: 636f 6e34 3822 0a20 2020 2020 2020 696e  con48".       in
+000008f0: 6b73 6361 7065 3a65 7870 6f72 742d 6669  kscape:export-fi
+00000900: 6c65 6e61 6d65 3d22 2e2f 4963 6f6e 3438  lename="./Icon48
+00000910: 2e70 6e67 220a 2020 2020 2020 2069 6e6b  .png".       ink
+00000920: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+00000930: 693d 2239 3622 0a20 2020 2020 2020 696e  i="96".       in
+00000940: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+00000950: 7069 3d22 3936 2220 2f3e 0a20 2020 203c  pi="96" />.    <
+00000960: 696e 6b73 6361 7065 3a70 6167 650a 2020  inkscape:page.  
+00000970: 2020 2020 2078 3d22 3435 3022 0a20 2020       x="450".   
+00000980: 2020 2020 793d 222d 312e 3835 3230 3631      y="-1.852061
+00000990: 3165 2d30 3622 0a20 2020 2020 2020 7769  1e-06".       wi
+000009a0: 6474 683d 2234 3030 220a 2020 2020 2020  dth="400".      
+000009b0: 2068 6569 6768 743d 2232 3030 220a 2020   height="200".  
+000009c0: 2020 2020 2069 643d 2270 6167 6536 3532       id="page652
+000009d0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+000009e0: 653a 6c61 6265 6c3d 224c 6f67 6f5f 626c  e:label="Logo_bl
+000009f0: 6163 6b22 0a20 2020 2020 2020 696e 6b73  ack".       inks
+00000a00: 6361 7065 3a65 7870 6f72 742d 6669 6c65  cape:export-file
+00000a10: 6e61 6d65 3d22 2e2e 2f62 6237 6635 3866  name="../bb7f58f
+00000a20: 352f 4c6f 676f 5f62 6c61 636b 2e70 6e67  5/Logo_black.png
+00000a30: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00000a40: 653a 6578 706f 7274 2d78 6470 693d 2239  e:export-xdpi="9
+00000a50: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+00000a60: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+00000a70: 3936 2220 2f3e 0a20 2020 203c 696e 6b73  96" />.    <inks
+00000a80: 6361 7065 3a70 6167 650a 2020 2020 2020  cape:page.      
+00000a90: 2078 3d22 3930 3022 0a20 2020 2020 2020   x="900".       
+00000aa0: 793d 222d 312e 3835 3230 3631 3165 2d30  y="-1.8520611e-0
+00000ab0: 3622 0a20 2020 2020 2020 7769 6474 683d  6".       width=
+00000ac0: 2234 3030 220a 2020 2020 2020 2068 6569  "400".       hei
+00000ad0: 6768 743d 2232 3030 220a 2020 2020 2020  ght="200".      
+00000ae0: 2069 643d 2270 6167 6532 3031 3422 202f   id="page2014" /
+00000af0: 3e0a 2020 3c2f 736f 6469 706f 6469 3a6e  >.  </sodipodi:n
+00000b00: 616d 6564 7669 6577 3e0a 2020 3c64 6566  amedview>.  <def
+00000b10: 730a 2020 2020 2069 643d 2264 6566 7332  s.     id="defs2
+00000b20: 223e 0a20 2020 203c 6669 6c74 6572 0a20  ">.    <filter. 
+00000b30: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00000b40: 6f6c 6c65 6374 3d22 616c 7761 7973 220a  ollect="always".
+00000b50: 2020 2020 2020 2073 7479 6c65 3d22 636f         style="co
+00000b60: 6c6f 722d 696e 7465 7270 6f6c 6174 696f  lor-interpolatio
+00000b70: 6e2d 6669 6c74 6572 733a 7352 4742 220a  n-filters:sRGB".
+00000b80: 2020 2020 2020 2069 643d 2266 696c 7465         id="filte
+00000b90: 7231 3530 3531 220a 2020 2020 2020 2078  r15051".       x
+00000ba0: 3d22 2d30 2e31 3637 3333 3430 3622 0a20  ="-0.16733406". 
+00000bb0: 2020 2020 2020 7769 6474 683d 2231 2e33        width="1.3
+00000bc0: 3334 3636 3831 220a 2020 2020 2020 2079  346681".       y
+00000bd0: 3d22 2d30 2e36 3532 3938 3433 3522 0a20  ="-0.65298435". 
+00000be0: 2020 2020 2020 6865 6967 6874 3d22 322e        height="2.
+00000bf0: 3330 3539 3638 3722 3e0a 2020 2020 2020  3059687">.      
+00000c00: 3c66 6547 6175 7373 6961 6e42 6c75 720a  <feGaussianBlur.
+00000c10: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00000c20: 653a 636f 6c6c 6563 743d 2261 6c77 6179  e:collect="alway
+00000c30: 7322 0a20 2020 2020 2020 2020 7374 6444  s".         stdD
+00000c40: 6576 6961 7469 6f6e 3d22 352e 3232 3630  eviation="5.2260
+00000c50: 3230 3922 0a20 2020 2020 2020 2020 6964  209".         id
+00000c60: 3d22 6665 4761 7573 7369 616e 426c 7572  ="feGaussianBlur
+00000c70: 3135 3035 3322 202f 3e0a 2020 2020 3c2f  15053" />.    </
+00000c80: 6669 6c74 6572 3e0a 2020 2020 3c66 696c  filter>.    <fil
+00000c90: 7465 720a 2020 2020 2020 2069 6e6b 7363  ter.       inksc
+00000ca0: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
+00000cb0: 6179 7322 0a20 2020 2020 2020 7374 796c  ays".       styl
+00000cc0: 653d 2263 6f6c 6f72 2d69 6e74 6572 706f  e="color-interpo
+00000cd0: 6c61 7469 6f6e 2d66 696c 7465 7273 3a73  lation-filters:s
+00000ce0: 5247 4222 0a20 2020 2020 2020 6964 3d22  RGB".       id="
+00000cf0: 6669 6c74 6572 3135 3035 312d 3322 0a20  filter15051-3". 
+00000d00: 2020 2020 2020 783d 222d 302e 3136 3733        x="-0.1673
+00000d10: 3334 3036 220a 2020 2020 2020 2077 6964  3406".       wid
+00000d20: 7468 3d22 312e 3333 3436 3638 3122 0a20  th="1.3346681". 
+00000d30: 2020 2020 2020 793d 222d 302e 3635 3239        y="-0.6529
+00000d40: 3834 3335 220a 2020 2020 2020 2068 6569  8435".       hei
+00000d50: 6768 743d 2232 2e33 3035 3936 3837 223e  ght="2.3059687">
+00000d60: 0a20 2020 2020 203c 6665 4761 7573 7369  .      <feGaussi
+00000d70: 616e 426c 7572 0a20 2020 2020 2020 2020  anBlur.         
+00000d80: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
+00000d90: 3d22 616c 7761 7973 220a 2020 2020 2020  ="always".      
+00000da0: 2020 2073 7464 4465 7669 6174 696f 6e3d     stdDeviation=
+00000db0: 2235 2e32 3236 3032 3039 220a 2020 2020  "5.2260209".    
+00000dc0: 2020 2020 2069 643d 2266 6547 6175 7373       id="feGauss
+00000dd0: 6961 6e42 6c75 7231 3530 3533 2d36 2220  ianBlur15053-6" 
+00000de0: 2f3e 0a20 2020 203c 2f66 696c 7465 723e  />.    </filter>
+00000df0: 0a20 2020 203c 6669 6c74 6572 0a20 2020  .    <filter.   
+00000e00: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
+00000e10: 6c65 6374 3d22 616c 7761 7973 220a 2020  lect="always".  
+00000e20: 2020 2020 2073 7479 6c65 3d22 636f 6c6f       style="colo
+00000e30: 722d 696e 7465 7270 6f6c 6174 696f 6e2d  r-interpolation-
+00000e40: 6669 6c74 6572 733a 7352 4742 220a 2020  filters:sRGB".  
+00000e50: 2020 2020 2069 643d 2266 696c 7465 7231       id="filter1
+00000e60: 3530 3531 2d33 2d32 220a 2020 2020 2020  5051-3-2".      
+00000e70: 2078 3d22 2d30 2e31 3637 3333 3430 3622   x="-0.16733406"
+00000e80: 0a20 2020 2020 2020 7769 6474 683d 2231  .       width="1
+00000e90: 2e33 3334 3636 3831 220a 2020 2020 2020  .3346681".      
+00000ea0: 2079 3d22 2d30 2e36 3532 3938 3433 3522   y="-0.65298435"
+00000eb0: 0a20 2020 2020 2020 6865 6967 6874 3d22  .       height="
+00000ec0: 322e 3330 3539 3638 3722 3e0a 2020 2020  2.3059687">.    
+00000ed0: 2020 3c66 6547 6175 7373 6961 6e42 6c75    <feGaussianBlu
+00000ee0: 720a 2020 2020 2020 2020 2069 6e6b 7363  r.         inksc
+00000ef0: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
+00000f00: 6179 7322 0a20 2020 2020 2020 2020 7374  ays".         st
+00000f10: 6444 6576 6961 7469 6f6e 3d22 352e 3232  dDeviation="5.22
+00000f20: 3630 3230 3922 0a20 2020 2020 2020 2020  60209".         
+00000f30: 6964 3d22 6665 4761 7573 7369 616e 426c  id="feGaussianBl
+00000f40: 7572 3135 3035 332d 362d 3222 202f 3e0a  ur15053-6-2" />.
+00000f50: 2020 2020 3c2f 6669 6c74 6572 3e0a 2020      </filter>.  
+00000f60: 3c2f 6465 6673 3e0a 2020 3c67 0a20 2020  </defs>.  <g.   
+00000f70: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
+00000f80: 3d22 4c61 7965 7220 3122 0a20 2020 2020  ="Layer 1".     
+00000f90: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
+00000fa0: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
+00000fb0: 6964 3d22 6c61 7965 7231 223e 0a20 2020  id="layer1">.   
+00000fc0: 203c 7265 6374 0a20 2020 2020 2020 7374   <rect.       st
+00000fd0: 796c 653d 2266 696c 6c3a 2366 6666 6666  yle="fill:#fffff
+00000fe0: 663b 7374 726f 6b65 3a6e 6f6e 653b 7374  f;stroke:none;st
+00000ff0: 726f 6b65 2d77 6964 7468 3a35 2e30 3834  roke-width:5.084
+00001000: 3736 3b73 7472 6f6b 652d 6c69 6e65 6361  76;stroke-lineca
+00001010: 703a 726f 756e 643b 7374 726f 6b65 2d6c  p:round;stroke-l
+00001020: 696e 656a 6f69 6e3a 726f 756e 643b 6669  inejoin:round;fi
+00001030: 6c6c 2d6f 7061 6369 7479 3a30 2e30 3230  ll-opacity:0.020
+00001040: 3039 3730 3622 0a20 2020 2020 2020 6964  09706".       id
+00001050: 3d22 7265 6374 3730 3622 0a20 2020 2020  ="rect706".     
+00001060: 2020 7769 6474 683d 2234 3030 220a 2020    width="400".  
+00001070: 2020 2020 2068 6569 6768 743d 2232 3030       height="200
+00001080: 220a 2020 2020 2020 2078 3d22 2d36 2e36  ".       x="-6.6
+00001090: 3936 3531 3331 652d 3036 220a 2020 2020  965131e-06".    
+000010a0: 2020 2079 3d22 2d31 2e38 3532 3036 3131     y="-1.8520611
+000010b0: 652d 3036 220a 2020 2020 2020 2072 793d  e-06".       ry=
+000010c0: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
+000010d0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+000010e0: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
+000010f0: 2d6f 7061 6369 7479 3a30 2e39 3938 3430  -opacity:0.99840
+00001100: 383b 7374 726f 6b65 3a23 3030 3030 3030  8;stroke:#000000
+00001110: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00001120: 3530 3030 3232 7078 3b73 7472 6f6b 652d  500022px;stroke-
+00001130: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00001140: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00001150: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
+00001160: 793a 3122 0a20 2020 2020 2020 643d 224d  y:1".       d="M
+00001170: 2031 3733 2e38 3438 3131 2c38 392e 3036   173.84811,89.06
+00001180: 3935 3120 3333 372e 3635 3039 362c 3634  951 337.65096,64
+00001190: 2e39 3439 3731 2031 3731 2e38 3734 3435  .94971 171.87445
+000011a0: 2c38 302e 3731 3433 3620 5a22 0a20 2020  ,80.71436 Z".   
+000011b0: 2020 2020 6964 3d22 7061 7468 3134 3635      id="path1465
+000011c0: 3722 0a20 2020 2020 2020 696e 6b73 6361  7".       inksca
+000011d0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+000011e0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+000011f0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+00001200: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
+00001210: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00001220: 7374 796c 653d 2266 696c 6c3a 2333 6534  style="fill:#3e4
+00001230: 6237 373b 6669 6c6c 2d6f 7061 6369 7479  b77;fill-opacity
+00001240: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00001250: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00001260: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
+00001270: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00001280: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00001290: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+000012a0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000012b0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000012c0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000012d0: 2020 2020 643d 224d 2031 392e 3630 3330      d="M 19.6030
+000012e0: 372c 3637 2e36 3536 3920 3830 2e38 3538  7,67.6569 80.858
+000012f0: 3032 382c 3634 2e38 3835 3132 2031 3231  028,64.88512 121
+00001300: 2e31 3034 3035 2c32 302e 3238 3435 3420  .10405,20.28454 
+00001310: 4320 3730 2e34 3032 3538 372c 3534 2e32  C 70.402587,54.2
+00001320: 3238 3733 2034 362e 3137 3936 3035 2c35  2873 46.179605,5
+00001330: 392e 3637 3633 3720 3139 2e36 3033 3037  9.67637 19.60307
+00001340: 2c36 372e 3635 3639 205a 220a 2020 2020  ,67.6569 Z".    
+00001350: 2020 2069 643d 2270 6174 6831 3435 3437     id="path14547
+00001360: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00001370: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001380: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+00001390: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+000013a0: 7065 733d 2263 6363 6322 202f 3e0a 2020  pes="cccc" />.  
+000013b0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+000013c0: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
+000013d0: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
+000013e0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+000013f0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00001400: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00001410: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00001420: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00001430: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00001440: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00001450: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00001460: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001470: 2020 2064 3d22 6d20 3830 2e38 3538 3032     d="m 80.85802
+00001480: 382c 3634 2e38 3835 3132 2032 362e 3537  8,64.88512 26.57
+00001490: 3735 3632 2c36 2e30 3437 3534 2031 332e  7562,6.04754 13.
+000014a0: 3636 3834 362c 2d35 302e 3634 3831 3220  66846,-50.64812 
+000014b0: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
+000014c0: 7468 3134 3534 3922 0a20 2020 2020 2020  th14549".       
+000014d0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+000014e0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+000014f0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00001500: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00001510: 3a23 3036 3035 3038 3b66 696c 6c2d 6f70  :#060508;fill-op
+00001520: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00001530: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00001540: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+00001550: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00001560: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00001570: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00001580: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00001590: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+000015a0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+000015b0: 220a 2020 2020 2020 2064 3d22 4d20 3130  ".       d="M 10
+000015c0: 372e 3433 3535 392c 3730 2e39 3332 3636  7.43559,70.93266
+000015d0: 2031 3738 2e35 3632 3233 2c38 332e 3533   178.56223,83.53
+000015e0: 3137 2043 2031 3530 2e38 3435 3431 2c36  17 C 150.84541,6
+000015f0: 382e 3934 3439 3720 3133 342e 3739 3530  8.94497 134.7950
+00001600: 312c 3435 2e35 3039 3535 2031 3231 2e31  1,45.50955 121.1
+00001610: 3034 3035 2c32 302e 3238 3435 3420 5a22  0405,20.28454 Z"
+00001620: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00001630: 3134 3535 3122 0a20 2020 2020 2020 696e  14551".       in
+00001640: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00001650: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00001660: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00001670: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+00001680: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+00001690: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+000016a0: 2332 3733 3737 333b 6669 6c6c 2d6f 7061  #273773;fill-opa
+000016b0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+000016c0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+000016d0: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+000016e0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+000016f0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00001700: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00001710: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00001720: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00001730: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00001740: 0a20 2020 2020 2020 643d 226d 2031 392e  .       d="m 19.
+00001750: 3630 3330 372c 3637 2e36 3536 3920 6320  60307,67.6569 c 
+00001760: 3133 2e34 3739 3331 322c 372e 3639 3738  13.479312,7.6978
+00001770: 2032 382e 3334 3131 3037 2c31 342e 3333   28.341107,14.33
+00001780: 3639 3520 3333 2e34 3131 3739 362c 3238  695 33.411796,28
+00001790: 2e34 3733 3832 206c 2032 372e 3834 3331  .47382 l 27.8431
+000017a0: 3632 2c2d 3331 2e32 3435 3620 7a22 0a20  62,-31.2456 z". 
+000017b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+000017c0: 3535 3322 0a20 2020 2020 2020 696e 6b73  553".       inks
+000017d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+000017e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+000017f0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00001800: 6574 7970 6573 3d22 6363 6363 2220 2f3e  etypes="cccc" />
+00001810: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00001820: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
+00001830: 3432 3637 323b 6669 6c6c 2d6f 7061 6369  42672;fill-opaci
+00001840: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00001850: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00001860: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00001870: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00001880: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00001890: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+000018a0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000018b0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+000018c0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+000018d0: 2020 2020 2020 643d 224d 2035 332e 3031        d="M 53.01
+000018e0: 3438 3636 2c39 362e 3133 3037 3220 3137  4866,96.13072 17
+000018f0: 382e 3536 3232 332c 3833 2e35 3331 3720  8.56223,83.5317 
+00001900: 3830 2e38 3538 3032 382c 3634 2e38 3835  80.858028,64.885
+00001910: 3132 205a 220a 2020 2020 2020 2069 643d  12 Z".       id=
+00001920: 2270 6174 6831 3435 3535 220a 2020 2020  "path14555".    
+00001930: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00001940: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00001950: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
+00001960: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00001970: 696c 6c3a 2335 3436 3638 633b 6669 6c6c  ill:#54668c;fill
+00001980: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00001990: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+000019a0: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+000019b0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+000019c0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+000019d0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+000019e0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+000019f0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00001a00: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00001a10: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00001a20: 2035 332e 3031 3438 3636 2c39 362e 3133   53.014866,96.13
+00001a30: 3037 3220 3732 2e33 3932 3232 342c 372e  072 72.392224,7.
+00001a40: 3535 3934 3420 3533 2e31 3535 3134 2c2d  55944 53.15514,-
+00001a50: 3230 2e31 3538 3436 207a 220a 2020 2020  20.15846 z".    
+00001a60: 2020 2069 643d 2270 6174 6831 3435 3537     id="path14557
+00001a70: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00001a80: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001a90: 6174 7572 653d 2230 2220 2f3e 0a20 2020  ature="0" />.   
+00001aa0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+00001ab0: 796c 653d 2266 696c 6c3a 2332 3233 3437  yle="fill:#22347
+00001ac0: 653b 6669 6c6c 2d6f 7061 6369 7479 3a31  e;fill-opacity:1
+00001ad0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00001ae0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+00001af0: 3530 3035 3b73 7472 6f6b 652d 6c69 6e65  5005;stroke-line
+00001b00: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00001b10: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00001b20: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00001b30: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00001b40: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00001b50: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00001b60: 2020 643d 226d 2035 332e 3031 3438 3636    d="m 53.014866
+00001b70: 2c39 362e 3133 3037 3220 6320 312e 3632  ,96.13072 c 1.62
+00001b80: 3738 3235 2c31 332e 3937 3235 3220 2d34  7825,13.97252 -4
+00001b90: 2e30 3036 3737 322c 3232 2e37 3830 3933  .006772,22.78093
+00001ba0: 202d 362e 3538 3131 3039 2c33 332e 3736   -6.581109,33.76
+00001bb0: 3534 3120 6c20 3738 2e39 3733 3333 332c  541 l 78.973333,
+00001bc0: 2d32 362e 3230 3539 3720 7a22 0a20 2020  -26.20597 z".   
+00001bd0: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+00001be0: 3922 0a20 2020 2020 2020 696e 6b73 6361  9".       inksca
+00001bf0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00001c00: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+00001c10: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+00001c20: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
+00001c30: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00001c40: 7374 796c 653d 2266 696c 6c3a 2330 3831  style="fill:#081
+00001c50: 3036 393b 6669 6c6c 2d6f 7061 6369 7479  069;fill-opacity
+00001c60: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00001c70: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00001c80: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
+00001c90: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00001ca0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00001cb0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00001cc0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00001cd0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00001ce0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00001cf0: 2020 2020 643d 224d 2034 362e 3433 3337      d="M 46.4337
+00001d00: 3537 2c31 3239 2e38 3936 3133 2031 3031  57,129.89613 101
+00001d10: 2e31 3037 362c 3133 372e 3935 3935 3120  .1076,137.95951 
+00001d20: 3137 382e 3536 3232 332c 3833 2e35 3331  178.56223,83.531
+00001d30: 3720 5a22 0a20 2020 2020 2020 6964 3d22  7 Z".       id="
+00001d40: 7061 7468 3134 3536 3122 0a20 2020 2020  path14561".     
+00001d50: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00001d60: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00001d70: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
+00001d80: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00001d90: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
+00001da0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00001db0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00001dc0: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
+00001dd0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00001de0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00001df0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+00001e00: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00001e10: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00001e20: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+00001e30: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+00001e40: 3130 312e 3130 3736 2c31 3337 2e39 3539  101.1076,137.959
+00001e50: 3531 2033 322e 3134 3631 392c 3432 2e30  51 32.14619,42.0
+00001e60: 3830 3739 202d 3131 2e38 3936 3632 2c2d  8079 -11.89662,-
+00001e70: 3536 2e36 3935 3636 207a 220a 2020 2020  56.69566 z".    
+00001e80: 2020 2069 643d 2270 6174 6831 3435 3633     id="path14563
+00001e90: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00001ea0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001eb0: 6174 7572 653d 2230 2220 2f3e 0a20 2020  ature="0" />.   
+00001ec0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+00001ed0: 796c 653d 2266 696c 6c3a 2332 3833 6438  yle="fill:#283d8
+00001ee0: 373b 6669 6c6c 2d6f 7061 6369 7479 3a31  7;fill-opacity:1
+00001ef0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00001f00: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+00001f10: 3530 3035 3b73 7472 6f6b 652d 6c69 6e65  5005;stroke-line
+00001f20: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00001f30: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00001f40: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00001f50: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00001f60: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00001f70: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00001f80: 2020 643d 226d 2031 3231 2e33 3537 3137    d="m 121.35717
+00001f90: 2c31 3233 2e33 3434 3634 2031 312e 3839  ,123.34464 11.89
+00001fa0: 3636 322c 3536 2e36 3935 3636 2063 2036  662,56.69566 c 6
+00001fb0: 2e31 3538 3632 2c2d 3530 2e39 3636 3733  .15862,-50.96673
+00001fc0: 2032 372e 3833 3134 372c 2d36 392e 3332   27.83147,-69.32
+00001fd0: 3836 3120 3435 2e33 3038 3434 2c2d 3936  861 45.30844,-96
+00001fe0: 2e35 3038 3620 7a22 0a20 2020 2020 2020  .5086 z".       
+00001ff0: 6964 3d22 7061 7468 3134 3536 3522 0a20  id="path14565". 
+00002000: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00002010: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00002020: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
+00002030: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+00002040: 3d22 6363 6363 2220 2f3e 0a20 2020 203c  ="cccc" />.    <
+00002050: 656c 6c69 7073 650a 2020 2020 2020 2073  ellipse.       s
+00002060: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
+00002070: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
+00002080: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
+00002090: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+000020a0: 6964 7468 3a31 2e30 3530 3035 3b73 7472  idth:1.05005;str
+000020b0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+000020c0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+000020d0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+000020e0: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+000020f0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00002100: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00002110: 3722 0a20 2020 2020 2020 6378 3d22 3230  7".       cx="20
+00002120: 2e39 3033 3131 3822 0a20 2020 2020 2020  .903118".       
+00002130: 6379 3d22 3637 2e37 3231 3538 3822 0a20  cy="67.721588". 
+00002140: 2020 2020 2020 7278 3d22 332e 3135 3632        rx="3.1562
+00002150: 3236 3422 0a20 2020 2020 2020 7279 3d22  264".       ry="
+00002160: 332e 3134 3230 3234 2220 2f3e 0a20 2020  3.142024" />.   
+00002170: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
+00002180: 2073 7479 6c65 3d22 6669 6c6c 3a23 3235   style="fill:#25
+00002190: 3361 3764 3b66 696c 6c2d 6f70 6163 6974  3a7d;fill-opacit
+000021a0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+000021b0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+000021c0: 312e 3035 3030 353b 7374 726f 6b65 2d6d  1.05005;stroke-m
+000021d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000021e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000021f0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+00002200: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+00002210: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
+00002220: 643d 2270 6174 6831 3435 3637 2d33 220a  d="path14567-3".
+00002230: 2020 2020 2020 2063 783d 2234 352e 3932         cx="45.92
+00002240: 3538 3436 220a 2020 2020 2020 2063 793d  5846".       cy=
+00002250: 2231 3239 2e32 3235 3838 220a 2020 2020  "129.22588".    
+00002260: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+00002270: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
+00002280: 322e 3332 3639 3734 3522 0a20 2020 2020  2.3269745".     
+00002290: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+000022a0: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
+000022b0: 342e 3937 3830 3136 3322 0a20 2020 2020  4.9780163".     
+000022c0: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
+000022d0: 0a20 2020 2020 2020 7279 3d22 332e 3134  .       ry="3.14
+000022e0: 3230 3234 2220 2f3e 0a20 2020 203c 656c  2024" />.    <el
+000022f0: 6c69 7073 650a 2020 2020 2020 2073 7479  lipse.       sty
+00002300: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
+00002310: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00002320: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00002330: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
+00002340: 3030 353b 7374 726f 6b65 2d6d 6974 6572  005;stroke-miter
+00002350: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00002360: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00002370: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
+00002380: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
+00002390: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
+000023a0: 6174 6831 3435 3637 2d33 2d37 220a 2020  ath14567-3-7".  
+000023b0: 2020 2020 2063 783d 2231 3230 2e35 3838       cx="120.588
+000023c0: 3632 220a 2020 2020 2020 2063 793d 2231  62".       cy="1
+000023d0: 3033 2e38 3931 3339 220a 2020 2020 2020  03.89139".      
+000023e0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+000023f0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+00002400: 3332 3639 3739 3222 0a20 2020 2020 2020  3269792".       
+00002410: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00002420: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
+00002430: 3937 3830 3230 3422 0a20 2020 2020 2020  9780204".       
+00002440: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
+00002450: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+00002460: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
+00002470: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
+00002480: 3d22 6669 6c6c 3a23 6138 6139 6161 3b66  ="fill:#a8a9aa;f
+00002490: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+000024a0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+000024b0: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+000024c0: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+000024d0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+000024e0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+000024f0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00002500: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00002510: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00002520: 6831 3435 3637 2d33 2d35 220a 2020 2020  h14567-3-5".    
+00002530: 2020 2063 783d 2231 3231 2e33 3337 3134     cx="121.33714
+00002540: 220a 2020 2020 2020 2063 793d 2231 3232  ".       cy="122
+00002550: 2e38 3932 3234 220a 2020 2020 2020 2069  .89224".       i
+00002560: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00002570: 6d2d 6365 6e74 6572 2d78 3d22 322e 3332  m-center-x="2.32
+00002580: 3639 3637 220a 2020 2020 2020 2069 6e6b  6967".       ink
+00002590: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
+000025a0: 6365 6e74 6572 2d79 3d22 2d34 2e39 3738  center-y="-4.978
+000025b0: 3030 3539 220a 2020 2020 2020 2072 783d  0059".       rx=
+000025c0: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
+000025d0: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
+000025e0: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
+000025f0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00002600: 696c 6c3a 2361 6261 6139 633b 6669 6c6c  ill:#abaa9c;fill
+00002610: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00002620: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00002630: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00002640: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00002650: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00002660: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00002670: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+00002680: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00002690: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+000026a0: 3536 372d 332d 3922 0a20 2020 2020 2020  567-3-9".       
+000026b0: 6378 3d22 3130 312e 3837 3631 3422 0a20  cx="101.87614". 
+000026c0: 2020 2020 2020 6379 3d22 3133 372e 3739        cy="137.79
+000026d0: 3438 3522 0a20 2020 2020 2020 696e 6b73  485".       inks
+000026e0: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+000026f0: 656e 7465 722d 783d 2232 2e33 3236 3937  enter-x="2.32697
+00002700: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
+00002710: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+00002720: 7465 722d 793d 222d 342e 3937 3830 3235  ter-y="-4.978025
+00002730: 3122 0a20 2020 2020 2020 7278 3d22 332e  1".       rx="3.
+00002740: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
+00002750: 7279 3d22 332e 3134 3230 3234 2220 2f3e  ry="3.142024" />
+00002760: 0a20 2020 203c 656c 6c69 7073 650a 2020  .    <ellipse.  
+00002770: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00002780: 3a23 3131 3230 3636 3b66 696c 6c2d 6f70  :#112066;fill-op
+00002790: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+000027a0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+000027b0: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+000027c0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+000027d0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000027e0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+000027f0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+00002800: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00002810: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+00002820: 2d33 2d32 220a 2020 2020 2020 2063 783d  -3-2".       cx=
+00002830: 2238 312e 3239 3234 3139 220a 2020 2020  "81.292419".    
+00002840: 2020 2063 793d 2236 342e 3231 3331 3635     cy="64.213165
+00002850: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00002860: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+00002870: 6572 2d78 3d22 332e 3539 3133 3630 3922  er-x="3.5913609"
+00002880: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00002890: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+000028a0: 722d 793d 222d 372e 3638 3238 3935 3622  r-y="-7.6828956"
+000028b0: 0a20 2020 2020 2020 7278 3d22 342e 3837  .       rx="4.87
+000028c0: 3131 3932 3922 0a20 2020 2020 2020 7279  11929".       ry
+000028d0: 3d22 342e 3834 3932 3733 3722 202f 3e0a  ="4.8492737" />.
+000028e0: 2020 2020 3c65 6c6c 6970 7365 0a20 2020      <ellipse.   
+000028f0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00002900: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
+00002910: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
+00002920: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00002930: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00002940: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+00002950: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00002960: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00002970: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00002980: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00002990: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+000029a0: 6831 3435 3637 2d32 220a 2020 2020 2020  h14567-2".      
+000029b0: 2063 783d 2231 3037 2e36 3737 3032 220a   cx="107.67702".
+000029c0: 2020 2020 2020 2063 793d 2236 392e 3631         cy="69.61
+000029d0: 3533 3536 220a 2020 2020 2020 2072 783d  5356".       rx=
+000029e0: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
+000029f0: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
+00002a00: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
+00002a10: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00002a20: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
+00002a30: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
+00002a40: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
+00002a50: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00002a60: 3035 3030 353b 7374 726f 6b65 2d6d 6974  05005;stroke-mit
+00002a70: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00002a80: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00002a90: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00002aa0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00002ab0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+00002ac0: 2270 6174 6831 3435 3637 2d32 2d38 220a  "path14567-2-8".
+00002ad0: 2020 2020 2020 2063 783d 2235 332e 3033         cx="53.03
+00002ae0: 3635 3735 220a 2020 2020 2020 2063 793d  6575".       cy=
+00002af0: 2239 352e 3639 3439 3737 220a 2020 2020  "95.694977".    
+00002b00: 2020 2072 783d 2233 2e31 3536 3232 3634     rx="3.1562264
+00002b10: 220a 2020 2020 2020 2072 793d 2233 2e31  ".       ry="3.1
+00002b20: 3432 3032 3422 202f 3e0a 2020 2020 3c70  42024" />.    <p
+00002b30: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00002b40: 3d22 6669 6c6c 3a23 3030 3030 3030 3b66  ="fill:#000000;f
+00002b50: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00002b60: 3834 3038 3b73 7472 6f6b 653a 2330 3030  8408;stroke:#000
+00002b70: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00002b80: 3a30 2e33 3233 3538 3870 783b 7374 726f  :0.323588px;stro
+00002b90: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00002ba0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00002bb0: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+00002bc0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00002bd0: 3d22 6d20 3331 382e 3730 3133 332c 3732  ="m 318.70133,72
+00002be0: 2e37 3031 3732 2032 362e 3630 3435 372c  .70172 26.60457,
+00002bf0: 2d38 2e37 3836 3833 202d 3238 2e33 3833  -8.78683 -28.383
+00002c00: 3935 2c2d 312e 3437 3538 3620 6320 3131  95,-1.47586 c 11
+00002c10: 2e30 3035 3236 2c33 2e32 3034 3636 2031  .00526,3.20466 1
+00002c20: 312e 3035 3533 2c33 2e33 3734 3237 2031  1.0553,3.37427 1
+00002c30: 2e37 3739 3338 2c31 302e 3236 3236 3920  .77938,10.26269 
+00002c40: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
+00002c50: 7468 3134 3635 372d 3922 0a20 2020 2020  th14657-9".     
+00002c60: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00002c70: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00002c80: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+00002c90: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00002ca0: 6363 2220 2f3e 0a20 2020 203c 656c 6c69  cc" />.    <elli
+00002cb0: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
+00002cc0: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
+00002cd0: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00002ce0: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
+00002cf0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00002d00: 3a31 2e39 3935 3938 3b73 7472 6f6b 652d  :1.99598;stroke-
+00002d10: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00002d20: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00002d30: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00002d40: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00002d50: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00002d60: 6964 3d22 7061 7468 3134 3536 372d 322d  id="path14567-2-
+00002d70: 3722 0a20 2020 2020 2020 6378 3d22 3137  7".       cx="17
+00002d80: 372e 3437 3435 3622 0a20 2020 2020 2020  7.47456".       
+00002d90: 6379 3d22 3834 2e33 3331 3732 3622 0a20  cy="84.331726". 
+00002da0: 2020 2020 2020 7278 3d22 352e 3939 3935        rx="5.9995
+00002db0: 3232 3222 0a20 2020 2020 2020 7279 3d22  222".       ry="
+00002dc0: 352e 3937 3235 3235 3622 202f 3e0a 2020  5.9725256" />.  
+00002dd0: 2020 3c74 6578 740a 2020 2020 2020 2078    <text.       x
+00002de0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+00002df0: 7665 220a 2020 2020 2020 2073 7479 6c65  ve".       style
+00002e00: 3d22 666f 6e74 2d73 7479 6c65 3a6e 6f72  ="font-style:nor
+00002e10: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
+00002e20: 6e6f 726d 616c 3b66 6f6e 742d 7369 7a65  normal;font-size
+00002e30: 3a35 2e38 3732 3931 7078 3b6c 696e 652d  :5.87291px;line-
+00002e40: 6865 6967 6874 3a31 2e32 353b 666f 6e74  height:1.25;font
+00002e50: 2d66 616d 696c 793a 7361 6e73 2d73 6572  -family:sans-ser
+00002e60: 6966 3b6c 6574 7465 722d 7370 6163 696e  if;letter-spacin
+00002e70: 673a 3070 783b 776f 7264 2d73 7061 6369  g:0px;word-spaci
+00002e80: 6e67 3a30 7078 3b66 696c 6c3a 2366 6666  ng:0px;fill:#fff
+00002e90: 6666 663b 6669 6c6c 2d6f 7061 6369 7479  fff;fill-opacity
+00002ea0: 3a31 3b73 7472 6f6b 653a 6e6f 6e65 3b73  :1;stroke:none;s
+00002eb0: 7472 6f6b 652d 7769 6474 683a 302e 3430  troke-width:0.40
+00002ec0: 3034 3235 3b66 696c 7465 723a 7572 6c28  0425;filter:url(
+00002ed0: 2366 696c 7465 7231 3530 3531 2922 0a20  #filter15051)". 
+00002ee0: 2020 2020 2020 783d 2237 372e 3639 3438        x="77.6948
+00002ef0: 3933 220a 2020 2020 2020 2079 3d22 3931  93".       y="91
+00002f00: 2e39 3838 3434 3922 0a20 2020 2020 2020  .988449".       
+00002f10: 6964 3d22 7465 7874 3134 3639 312d 3622  id="text14691-6"
+00002f20: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
+00002f30: 6d3d 226d 6174 7269 7828 322e 3735 3131  m="matrix(2.7511
+00002f40: 3931 392c 302c 302c 322e 3733 3838 3132  919,0,0,2.738812
+00002f50: 2c2d 3735 2e39 3736 3639 362c 2d31 3038  ,-75.976696,-108
+00002f60: 2e30 3838 3636 2922 3e3c 7473 7061 6e0a  .08866)"><tspan.
+00002f70: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00002f80: 693a 726f 6c65 3d22 6c69 6e65 220a 2020  i:role="line".  
+00002f90: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
+00002fa0: 3134 3638 392d 3222 0a20 2020 2020 2020  14689-2".       
+00002fb0: 2020 783d 2237 372e 3639 3438 3933 220a    x="77.694893".
+00002fc0: 2020 2020 2020 2020 2079 3d22 3931 2e39           y="91.9
+00002fd0: 3838 3434 3922 0a20 2020 2020 2020 2020  88449".         
+00002fe0: 7374 796c 653d 2266 6f6e 742d 7374 796c  style="font-styl
+00002ff0: 653a 6e6f 726d 616c 3b66 6f6e 742d 7661  e:normal;font-va
+00003000: 7269 616e 743a 6e6f 726d 616c 3b66 6f6e  riant:normal;fon
+00003010: 742d 7765 6967 6874 3a6e 6f72 6d61 6c3b  t-weight:normal;
+00003020: 666f 6e74 2d73 7472 6574 6368 3a6e 6f72  font-stretch:nor
+00003030: 6d61 6c3b 666f 6e74 2d73 697a 653a 3231  mal;font-size:21
+00003040: 2e33 3536 7078 3b66 6f6e 742d 6661 6d69  .356px;font-fami
+00003050: 6c79 3a49 6d70 6163 743b 2d69 6e6b 7363  ly:Impact;-inksc
+00003060: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
+00003070: 6361 7469 6f6e 3a49 6d70 6163 743b 6669  cation:Impact;fi
+00003080: 6c6c 3a23 6666 6666 6666 3b66 696c 6c2d  ll:#ffffff;fill-
+00003090: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+000030a0: 2d77 6964 7468 3a30 2e34 3030 3432 3522  -width:0.400425"
+000030b0: 3e53 6165 6e6f 7079 3c2f 7473 7061 6e3e  >Saenopy</tspan>
+000030c0: 3c2f 7465 7874 3e0a 2020 2020 3c74 6578  </text>.    <tex
+000030d0: 740a 2020 2020 2020 2078 6d6c 3a73 7061  t.       xml:spa
+000030e0: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
+000030f0: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
+00003100: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
+00003110: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
+00003120: 3b66 6f6e 742d 7369 7a65 3a31 362e 3132  ;font-size:16.12
+00003130: 3131 7078 3b6c 696e 652d 6865 6967 6874  11px;line-height
+00003140: 3a31 2e32 353b 666f 6e74 2d66 616d 696c  :1.25;font-famil
+00003150: 793a 7361 6e73 2d73 6572 6966 3b6c 6574  y:sans-serif;let
+00003160: 7465 722d 7370 6163 696e 673a 3070 783b  ter-spacing:0px;
+00003170: 776f 7264 2d73 7061 6369 6e67 3a30 7078  word-spacing:0px
+00003180: 3b66 696c 6c3a 2330 3030 3030 303b 6669  ;fill:#000000;fi
+00003190: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000031a0: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
+000031b0: 7769 6474 683a 312e 3039 3931 3722 0a20  width:1.09917". 
+000031c0: 2020 2020 2020 783d 2231 3335 2e34 3739        x="135.479
+000031d0: 3036 220a 2020 2020 2020 2079 3d22 3133  06".       y="13
+000031e0: 362e 3338 3737 220a 2020 2020 2020 2069  6.3877".       i
+000031f0: 643d 2274 6578 7431 3436 3931 220a 2020  d="text14691".  
+00003200: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+00003210: 7363 616c 6528 312e 3030 3232 3537 352c  scale(1.0022575,
+00003220: 302e 3939 3737 3437 3538 2922 3e3c 7473  0.99774758)"><ts
+00003230: 7061 6e0a 2020 2020 2020 2020 2073 6f64  pan.         sod
+00003240: 6970 6f64 693a 726f 6c65 3d22 6c69 6e65  ipodi:role="line
+00003250: 220a 2020 2020 2020 2020 2069 643d 2274  ".         id="t
+00003260: 7370 616e 3134 3638 3922 0a20 2020 2020  span14689".     
+00003270: 2020 2020 783d 2231 3335 2e34 3739 3036      x="135.47906
+00003280: 220a 2020 2020 2020 2020 2079 3d22 3133  ".         y="13
+00003290: 362e 3338 3737 220a 2020 2020 2020 2020  6.3877".        
+000032a0: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
+000032b0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
+000032c0: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
+000032d0: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
+000032e0: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
+000032f0: 726d 616c 3b66 6f6e 742d 7369 7a65 3a35  rmal;font-size:5
+00003300: 382e 3632 3231 7078 3b66 6f6e 742d 6661  8.6221px;font-fa
+00003310: 6d69 6c79 3a27 546c 7767 2054 7970 6973  mily:'Tlwg Typis
+00003320: 7427 3b2d 696e 6b73 6361 7065 2d66 6f6e  t';-inkscape-fon
+00003330: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
+00003340: 2754 6c77 6720 5479 7069 7374 273b 7374  'Tlwg Typist';st
+00003350: 726f 6b65 2d77 6964 7468 3a31 2e30 3939  roke-width:1.099
+00003360: 3137 223e 5361 656e 6f70 793c 2f74 7370  17">Saenopy</tsp
+00003370: 616e 3e3c 2f74 6578 743e 0a20 2020 203c  an></text>.    <
+00003380: 7265 6374 0a20 2020 2020 2020 7374 796c  rect.       styl
+00003390: 653d 2266 696c 6c3a 2330 3030 3030 303b  e="fill:#000000;
+000033a0: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+000033b0: 6b65 2d77 6964 7468 3a35 2e30 3834 3736  ke-width:5.08476
+000033c0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+000033d0: 726f 756e 643b 7374 726f 6b65 2d6c 696e  round;stroke-lin
+000033e0: 656a 6f69 6e3a 726f 756e 643b 6669 6c6c  ejoin:round;fill
+000033f0: 2d6f 7061 6369 7479 3a30 220a 2020 2020  -opacity:0".    
+00003400: 2020 2069 643d 2272 6563 7437 3036 2d35     id="rect706-5
+00003410: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
+00003420: 3430 3022 0a20 2020 2020 2020 6865 6967  400".       heig
+00003430: 6874 3d22 3230 3022 0a20 2020 2020 2020  ht="200".       
+00003440: 783d 2234 3530 220a 2020 2020 2020 2079  x="450".       y
+00003450: 3d22 2d31 2e38 3532 3036 3131 652d 3036  ="-1.8520611e-06
+00003460: 220a 2020 2020 2020 2072 793d 2230 2220  ".       ry="0" 
+00003470: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+00003480: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00003490: 2366 6666 6666 663b 6669 6c6c 2d6f 7061  #ffffff;fill-opa
+000034a0: 6369 7479 3a30 2e39 3938 3430 3830 383b  city:0.99840808;
+000034b0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+000034c0: 7472 6f6b 652d 7769 6474 683a 302e 3530  troke-width:0.50
+000034d0: 3030 3232 7078 3b73 7472 6f6b 652d 6c69  0022px;stroke-li
+000034e0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+000034f0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00003500: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00003510: 3122 0a20 2020 2020 2020 643d 224d 2036  1".       d="M 6
+00003520: 3233 2e38 3438 3132 2c38 392e 3036 3935  23.84812,89.0695
+00003530: 3120 3738 372e 3635 3039 372c 3634 2e39  1 787.65097,64.9
+00003540: 3439 3731 2036 3231 2e38 3734 3436 2c38  4971 621.87446,8
+00003550: 302e 3731 3433 3620 5a22 0a20 2020 2020  0.71436 Z".     
+00003560: 2020 6964 3d22 7061 7468 3134 3635 372d    id="path14657-
+00003570: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
+00003580: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00003590: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+000035a0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+000035b0: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
+000035c0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+000035d0: 7374 796c 653d 2266 696c 6c3a 2333 6534  style="fill:#3e4
+000035e0: 6237 373b 6669 6c6c 2d6f 7061 6369 7479  b77;fill-opacity
+000035f0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00003600: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00003610: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
+00003620: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00003630: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00003640: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00003650: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00003660: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00003670: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00003680: 2020 2020 643d 226d 2034 3639 2e36 3033      d="m 469.603
+00003690: 3038 2c36 372e 3635 3639 2036 312e 3235  08,67.6569 61.25
+000036a0: 3439 362c 2d32 2e37 3731 3738 2034 302e  496,-2.77178 40.
+000036b0: 3234 3630 322c 2d34 342e 3630 3035 3820  24602,-44.60058 
+000036c0: 4320 3532 302e 3430 3236 2c35 342e 3232  C 520.4026,54.22
+000036d0: 3837 3320 3439 362e 3137 3936 312c 3539  873 496.17961,59
+000036e0: 2e36 3736 3337 2034 3639 2e36 3033 3038  .67637 469.60308
+000036f0: 2c36 372e 3635 3639 205a 220a 2020 2020  ,67.6569 Z".    
+00003700: 2020 2069 643d 2270 6174 6831 3435 3437     id="path14547
+00003710: 2d35 220a 2020 2020 2020 2069 6e6b 7363  -5".       inksc
+00003720: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00003730: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00003740: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00003750: 7479 7065 733d 2263 6363 6322 202f 3e0a  types="cccc" />.
+00003760: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00003770: 2073 7479 6c65 3d22 6669 6c6c 3a23 3163   style="fill:#1c
+00003780: 3263 3638 3b66 696c 6c2d 6f70 6163 6974  2c68;fill-opacit
+00003790: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+000037a0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+000037b0: 312e 3035 3030 353b 7374 726f 6b65 2d6c  1.05005;stroke-l
+000037c0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+000037d0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+000037e0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+000037f0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00003800: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00003810: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00003820: 2020 2020 2064 3d22 6d20 3533 302e 3835       d="m 530.85
+00003830: 3830 342c 3634 2e38 3835 3132 2032 362e  804,64.88512 26.
+00003840: 3537 3735 362c 362e 3034 3735 3420 3133  57756,6.04754 13
+00003850: 2e36 3638 3436 2c2d 3530 2e36 3438 3132  .66846,-50.64812
+00003860: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
+00003870: 6174 6831 3435 3439 2d36 220a 2020 2020  ath14549-6".    
+00003880: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00003890: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000038a0: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
+000038b0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+000038c0: 696c 6c3a 2330 3630 3530 383b 6669 6c6c  ill:#060508;fill
+000038d0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+000038e0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+000038f0: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00003900: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00003910: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00003920: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00003930: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00003940: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00003950: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00003960: 793a 3122 0a20 2020 2020 2020 643d 224d  y:1".       d="M
+00003970: 2035 3537 2e34 3335 362c 3730 2e39 3332   557.4356,70.932
+00003980: 3636 2036 3238 2e35 3632 3234 2c38 332e  66 628.56224,83.
+00003990: 3533 3137 2043 2036 3030 2e38 3435 3432  5317 C 600.84542
+000039a0: 2c36 382e 3934 3439 3720 3538 342e 3739  ,68.94497 584.79
+000039b0: 3530 322c 3435 2e35 3039 3535 2035 3731  502,45.50955 571
+000039c0: 2e31 3034 3036 2c32 302e 3238 3435 3420  .10406,20.28454 
+000039d0: 5a22 0a20 2020 2020 2020 6964 3d22 7061  Z".       id="pa
+000039e0: 7468 3134 3535 312d 3222 0a20 2020 2020  th14551-2".     
+000039f0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00003a00: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00003a10: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+00003a20: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00003a30: 6363 2220 2f3e 0a20 2020 203c 7061 7468  cc" />.    <path
+00003a40: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00003a50: 696c 6c3a 2332 3733 3737 333b 6669 6c6c  ill:#273773;fill
+00003a60: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00003a70: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00003a80: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00003a90: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00003aa0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00003ab0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00003ac0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00003ad0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00003ae0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00003af0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00003b00: 2034 3639 2e36 3033 3038 2c36 372e 3635   469.60308,67.65
+00003b10: 3639 2063 2031 332e 3437 3933 312c 372e  69 c 13.47931,7.
+00003b20: 3639 3738 2032 382e 3334 3131 312c 3134  6978 28.34111,14
+00003b30: 2e33 3336 3935 2033 332e 3431 3138 2c32  .33695 33.4118,2
+00003b40: 382e 3437 3338 3220 6c20 3237 2e38 3433  8.47382 l 27.843
+00003b50: 3136 2c2d 3331 2e32 3435 3620 7a22 0a20  16,-31.2456 z". 
+00003b60: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00003b70: 3535 332d 3922 0a20 2020 2020 2020 696e  553-9".       in
+00003b80: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00003b90: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00003ba0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00003bb0: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+00003bc0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+00003bd0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00003be0: 2331 3432 3637 323b 6669 6c6c 2d6f 7061  #142672;fill-opa
+00003bf0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+00003c00: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00003c10: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+00003c20: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00003c30: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00003c40: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00003c50: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00003c60: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00003c70: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00003c80: 0a20 2020 2020 2020 643d 224d 2035 3033  .       d="M 503
+00003c90: 2e30 3134 3838 2c39 362e 3133 3037 3220  .01488,96.13072 
+00003ca0: 3632 382e 3536 3232 342c 3833 2e35 3331  628.56224,83.531
+00003cb0: 3720 3533 302e 3835 3830 342c 3634 2e38  7 530.85804,64.8
+00003cc0: 3835 3132 205a 220a 2020 2020 2020 2069  8512 Z".       i
+00003cd0: 643d 2270 6174 6831 3435 3535 2d31 220a  d="path14555-1".
+00003ce0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00003cf0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00003d00: 7572 653d 2230 2220 2f3e 0a20 2020 203c  ure="0" />.    <
+00003d10: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+00003d20: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
+00003d30: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00003d40: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00003d50: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+00003d60: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
+00003d70: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00003d80: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00003d90: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00003da0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00003db0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00003dc0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00003dd0: 643d 226d 2035 3033 2e30 3134 3838 2c39  d="m 503.01488,9
+00003de0: 362e 3133 3037 3220 3732 2e33 3932 3232  6.13072 72.39222
+00003df0: 2c37 2e35 3539 3434 2035 332e 3135 3531  ,7.55944 53.1551
+00003e00: 342c 2d32 302e 3135 3834 3620 7a22 0a20  4,-20.15846 z". 
+00003e10: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00003e20: 3535 372d 3222 0a20 2020 2020 2020 696e  557-2".       in
+00003e30: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00003e40: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00003e50: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+00003e60: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00003e70: 3232 3334 3765 3b66 696c 6c2d 6f70 6163  22347e;fill-opac
+00003e80: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+00003e90: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00003ea0: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+00003eb0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00003ec0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00003ed0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+00003ee0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00003ef0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00003f00: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00003f10: 2020 2020 2020 2064 3d22 6d20 3530 332e         d="m 503.
+00003f20: 3031 3438 382c 3936 2e31 3330 3732 2063  01488,96.13072 c
+00003f30: 2031 2e36 3237 3832 2c31 332e 3937 3235   1.62782,13.9725
+00003f40: 3220 2d34 2e30 3036 3738 2c32 322e 3738  2 -4.00678,22.78
+00003f50: 3039 3320 2d36 2e35 3831 3131 2c33 332e  093 -6.58111,33.
+00003f60: 3736 3534 3120 6c20 3738 2e39 3733 3333  76541 l 78.97333
+00003f70: 2c2d 3236 2e32 3035 3937 207a 220a 2020  ,-26.20597 z".  
+00003f80: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00003f90: 3539 2d37 220a 2020 2020 2020 2069 6e6b  59-7".       ink
+00003fa0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00003fb0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00003fc0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00003fd0: 6465 7479 7065 733d 2263 6363 6322 202f  detypes="cccc" /
+00003fe0: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+00003ff0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00004000: 3038 3130 3639 3b66 696c 6c2d 6f70 6163  081069;fill-opac
+00004010: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+00004020: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00004030: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+00004040: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00004050: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00004060: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+00004070: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00004080: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00004090: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+000040a0: 2020 2020 2020 2064 3d22 6d20 3439 362e         d="m 496.
+000040b0: 3433 3337 372c 3132 392e 3839 3631 3320  43377,129.89613 
+000040c0: 3534 2e36 3733 3834 2c38 2e30 3633 3338  54.67384,8.06338
+000040d0: 2037 372e 3435 3436 332c 2d35 342e 3432   77.45463,-54.42
+000040e0: 3738 3120 7a22 0a20 2020 2020 2020 6964  781 z".       id
+000040f0: 3d22 7061 7468 3134 3536 312d 3022 0a20  ="path14561-0". 
+00004100: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00004110: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00004120: 7265 3d22 3022 202f 3e0a 2020 2020 3c70  re="0" />.    <p
+00004130: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00004140: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
+00004150: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00004160: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00004170: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00004180: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
+00004190: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+000041a0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+000041b0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+000041c0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000041d0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+000041e0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+000041f0: 3d22 4d20 3535 312e 3130 3736 312c 3133  ="M 551.10761,13
+00004200: 372e 3935 3935 3120 3538 332e 3235 3338  7.95951 583.2538
+00004210: 2c31 3830 2e30 3430 3320 3537 312e 3335  ,180.0403 571.35
+00004220: 3731 382c 3132 332e 3334 3436 3420 5a22  718,123.34464 Z"
+00004230: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00004240: 3134 3536 332d 3922 0a20 2020 2020 2020  14563-9".       
+00004250: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00004260: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00004270: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00004280: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00004290: 3a23 3238 3364 3837 3b66 696c 6c2d 6f70  :#283d87;fill-op
+000042a0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+000042b0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+000042c0: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+000042d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+000042e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000042f0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00004300: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00004310: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00004320: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00004330: 220a 2020 2020 2020 2064 3d22 6d20 3537  ".       d="m 57
+00004340: 312e 3335 3731 382c 3132 332e 3334 3436  1.35718,123.3446
+00004350: 3420 3131 2e38 3936 3632 2c35 362e 3639  4 11.89662,56.69
+00004360: 3536 3620 6320 362e 3135 3836 322c 2d35  566 c 6.15862,-5
+00004370: 302e 3936 3637 3320 3237 2e38 3331 3437  0.96673 27.83147
+00004380: 2c2d 3639 2e33 3238 3631 2034 352e 3330  ,-69.32861 45.30
+00004390: 3834 342c 2d39 362e 3530 3836 207a 220a  844,-96.5086 z".
+000043a0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000043b0: 3435 3635 2d33 220a 2020 2020 2020 2069  4565-3".       i
+000043c0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+000043d0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+000043e0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000043f0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00004400: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
+00004410: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00004420: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
+00004430: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
+00004440: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
+00004450: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00004460: 3035 3030 353b 7374 726f 6b65 2d6d 6974  05005;stroke-mit
+00004470: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00004480: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00004490: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+000044a0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+000044b0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+000044c0: 2270 6174 6831 3435 3637 2d36 3022 0a20  "path14567-60". 
+000044d0: 2020 2020 2020 6378 3d22 3437 302e 3930        cx="470.90
+000044e0: 3331 3422 0a20 2020 2020 2020 6379 3d22  314".       cy="
+000044f0: 3637 2e37 3231 3538 3822 0a20 2020 2020  67.721588".     
+00004500: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
+00004510: 0a20 2020 2020 2020 7279 3d22 332e 3134  .       ry="3.14
+00004520: 3230 3234 2220 2f3e 0a20 2020 203c 656c  2024" />.    <el
+00004530: 6c69 7073 650a 2020 2020 2020 2073 7479  lipse.       sty
+00004540: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
+00004550: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00004560: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00004570: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
+00004580: 3030 353b 7374 726f 6b65 2d6d 6974 6572  005;stroke-miter
+00004590: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+000045a0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+000045b0: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
+000045c0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
+000045d0: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
+000045e0: 6174 6831 3435 3637 2d33 2d36 220a 2020  ath14567-3-6".  
+000045f0: 2020 2020 2063 783d 2234 3935 2e39 3235       cx="495.925
+00004600: 3834 220a 2020 2020 2020 2063 793d 2231  84".       cy="1
+00004610: 3239 2e32 3235 3838 220a 2020 2020 2020  29.22588".      
+00004620: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00004630: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+00004640: 3332 3639 3734 3522 0a20 2020 2020 2020  3269745".       
+00004650: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00004660: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
+00004670: 3937 3830 3136 3322 0a20 2020 2020 2020  9780163".       
+00004680: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
+00004690: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+000046a0: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
+000046b0: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
+000046c0: 3d22 6669 6c6c 3a23 3235 3361 3764 3b66  ="fill:#253a7d;f
+000046d0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+000046e0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+000046f0: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00004700: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+00004710: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00004720: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00004730: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00004740: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00004750: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00004760: 6831 3435 3637 2d33 2d37 2d32 220a 2020  h14567-3-7-2".  
+00004770: 2020 2020 2063 783d 2235 3730 2e35 3838       cx="570.588
+00004780: 3632 220a 2020 2020 2020 2063 793d 2231  62".       cy="1
+00004790: 3033 2e38 3931 3339 220a 2020 2020 2020  03.89139".      
+000047a0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+000047b0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+000047c0: 3332 3639 3739 3222 0a20 2020 2020 2020  3269792".       
+000047d0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+000047e0: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
+000047f0: 3937 3830 3230 3422 0a20 2020 2020 2020  9780204".       
+00004800: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
+00004810: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+00004820: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
+00004830: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
+00004840: 3d22 6669 6c6c 3a23 6138 6139 6161 3b66  ="fill:#a8a9aa;f
+00004850: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00004860: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00004870: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00004880: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+00004890: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+000048a0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+000048b0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+000048c0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+000048d0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+000048e0: 6831 3435 3637 2d33 2d35 2d36 220a 2020  h14567-3-5-6".  
+000048f0: 2020 2020 2063 783d 2235 3731 2e33 3337       cx="571.337
+00004900: 3136 220a 2020 2020 2020 2063 793d 2231  16".       cy="1
+00004910: 3232 2e38 3932 3234 220a 2020 2020 2020  22.89224".      
+00004920: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00004930: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+00004940: 3332 3639 3637 220a 2020 2020 2020 2069  326967".       i
+00004950: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00004960: 6d2d 6365 6e74 6572 2d79 3d22 2d34 2e39  m-center-y="-4.9
+00004970: 3738 3030 3539 220a 2020 2020 2020 2072  780059".       r
+00004980: 783d 2233 2e31 3536 3232 3634 220a 2020  x="3.1562264".  
+00004990: 2020 2020 2072 793d 2233 2e31 3432 3032       ry="3.14202
+000049a0: 3422 202f 3e0a 2020 2020 3c65 6c6c 6970  4" />.    <ellip
+000049b0: 7365 0a20 2020 2020 2020 7374 796c 653d  se.       style=
+000049c0: 2266 696c 6c3a 2361 6261 6139 633b 6669  "fill:#abaa9c;fi
+000049d0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000049e0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+000049f0: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00004a00: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00004a10: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00004a20: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00004a30: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+00004a40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00004a50: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00004a60: 3134 3536 372d 332d 392d 3122 0a20 2020  14567-3-9-1".   
+00004a70: 2020 2020 6378 3d22 3535 312e 3837 3631      cx="551.8761
+00004a80: 3622 0a20 2020 2020 2020 6379 3d22 3133  6".       cy="13
+00004a90: 372e 3739 3438 3522 0a20 2020 2020 2020  7.79485".       
+00004aa0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00004ab0: 726d 2d63 656e 7465 722d 783d 2232 2e33  rm-center-x="2.3
+00004ac0: 3236 3937 3322 0a20 2020 2020 2020 696e  26973".       in
+00004ad0: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
+00004ae0: 2d63 656e 7465 722d 793d 222d 342e 3937  -center-y="-4.97
+00004af0: 3830 3235 3122 0a20 2020 2020 2020 7278  80251".       rx
+00004b00: 3d22 332e 3135 3632 3236 3422 0a20 2020  ="3.1562264".   
+00004b10: 2020 2020 7279 3d22 332e 3134 3230 3234      ry="3.142024
+00004b20: 2220 2f3e 0a20 2020 203c 656c 6c69 7073  " />.    <ellips
+00004b30: 650a 2020 2020 2020 2073 7479 6c65 3d22  e.       style="
+00004b40: 6669 6c6c 3a23 3131 3230 3636 3b66 696c  fill:#112066;fil
+00004b50: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00004b60: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00004b70: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+00004b80: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00004b90: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00004ba0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00004bb0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00004bc0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00004bd0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00004be0: 3435 3637 2d33 2d32 2d38 220a 2020 2020  4567-3-2-8".    
+00004bf0: 2020 2063 783d 2235 3331 2e32 3932 3432     cx="531.29242
+00004c00: 220a 2020 2020 2020 2063 793d 2236 342e  ".       cy="64.
+00004c10: 3231 3331 3635 220a 2020 2020 2020 2069  213165".       i
+00004c20: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00004c30: 6d2d 6365 6e74 6572 2d78 3d22 332e 3539  m-center-x="3.59
+00004c40: 3133 3630 3922 0a20 2020 2020 2020 696e  13609".       in
+00004c50: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
+00004c60: 2d63 656e 7465 722d 793d 222d 372e 3638  -center-y="-7.68
+00004c70: 3238 3935 3622 0a20 2020 2020 2020 7278  28956".       rx
+00004c80: 3d22 342e 3837 3131 3932 3922 0a20 2020  ="4.8711929".   
+00004c90: 2020 2020 7279 3d22 342e 3834 3932 3733      ry="4.849273
+00004ca0: 3722 202f 3e0a 2020 2020 3c65 6c6c 6970  7" />.    <ellip
+00004cb0: 7365 0a20 2020 2020 2020 7374 796c 653d  se.       style=
+00004cc0: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
+00004cd0: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
+00004ce0: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
+00004cf0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00004d00: 312e 3035 3030 353b 7374 726f 6b65 2d6d  1.05005;stroke-m
+00004d10: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00004d20: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00004d30: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+00004d40: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+00004d50: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
+00004d60: 643d 2270 6174 6831 3435 3637 2d32 2d37  d="path14567-2-7
+00004d70: 3922 0a20 2020 2020 2020 6378 3d22 3535  9".       cx="55
+00004d80: 372e 3637 3722 0a20 2020 2020 2020 6379  7.677".       cy
+00004d90: 3d22 3639 2e36 3135 3335 3622 0a20 2020  ="69.615356".   
+00004da0: 2020 2020 7278 3d22 332e 3135 3632 3236      rx="3.156226
+00004db0: 3422 0a20 2020 2020 2020 7279 3d22 332e  4".       ry="3.
+00004dc0: 3134 3230 3234 2220 2f3e 0a20 2020 203c  142024" />.    <
+00004dd0: 656c 6c69 7073 650a 2020 2020 2020 2073  ellipse.       s
+00004de0: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
+00004df0: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
+00004e00: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
+00004e10: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00004e20: 6964 7468 3a31 2e30 3530 3035 3b73 7472  idth:1.05005;str
+00004e30: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00004e40: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00004e50: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+00004e60: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+00004e70: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00004e80: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00004e90: 372d 322d 382d 3222 0a20 2020 2020 2020  7-2-8-2".       
+00004ea0: 6378 3d22 3530 332e 3033 3635 3922 0a20  cx="503.03659". 
+00004eb0: 2020 2020 2020 6379 3d22 3935 2e36 3934        cy="95.694
+00004ec0: 3937 3722 0a20 2020 2020 2020 7278 3d22  977".       rx="
+00004ed0: 332e 3135 3632 3236 3422 0a20 2020 2020  3.1562264".     
+00004ee0: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
+00004ef0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+00004f00: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00004f10: 2366 6666 6666 663b 6669 6c6c 2d6f 7061  #ffffff;fill-opa
+00004f20: 6369 7479 3a30 2e39 3938 3430 3830 383b  city:0.99840808;
+00004f30: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00004f40: 7472 6f6b 652d 7769 6474 683a 302e 3332  troke-width:0.32
+00004f50: 3335 3838 7078 3b73 7472 6f6b 652d 6c69  3588px;stroke-li
+00004f60: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00004f70: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00004f80: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00004f90: 3122 0a20 2020 2020 2020 643d 226d 2037  1".       d="m 7
+00004fa0: 3638 2e37 3031 3334 2c37 322e 3730 3137  68.70134,72.7017
+00004fb0: 3220 3236 2e36 3034 3537 2c2d 382e 3738  2 26.60457,-8.78
+00004fc0: 3638 3320 2d32 382e 3338 3339 352c 2d31  683 -28.38395,-1
+00004fd0: 2e34 3735 3836 2063 2031 312e 3030 3532  .47586 c 11.0052
+00004fe0: 362c 332e 3230 3436 3620 3131 2e30 3535  6,3.20466 11.055
+00004ff0: 332c 332e 3337 3432 3720 312e 3737 3933  3,3.37427 1.7793
+00005000: 382c 3130 2e32 3632 3639 207a 220a 2020  8,10.26269 z".  
+00005010: 2020 2020 2069 643d 2270 6174 6831 3436       id="path146
+00005020: 3537 2d39 2d30 220a 2020 2020 2020 2069  57-9-0".       i
+00005030: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00005040: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+00005050: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00005060: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00005070: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
+00005080: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00005090: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
+000050a0: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
+000050b0: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
+000050c0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+000050d0: 3939 3539 383b 7374 726f 6b65 2d6d 6974  99598;stroke-mit
+000050e0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+000050f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00005100: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00005110: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00005120: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+00005130: 2270 6174 6831 3435 3637 2d32 2d37 2d32  "path14567-2-7-2
+00005140: 220a 2020 2020 2020 2063 783d 2236 3237  ".       cx="627
+00005150: 2e34 3734 3535 220a 2020 2020 2020 2063  .47455".       c
+00005160: 793d 2238 342e 3333 3137 3236 220a 2020  y="84.331726".  
+00005170: 2020 2020 2072 783d 2235 2e39 3939 3532       rx="5.99952
+00005180: 3232 220a 2020 2020 2020 2072 793d 2235  22".       ry="5
+00005190: 2e39 3732 3532 3536 2220 2f3e 0a20 2020  .9725256" />.   
+000051a0: 203c 7465 7874 0a20 2020 2020 2020 786d   <text.       xm
+000051b0: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
+000051c0: 6522 0a20 2020 2020 2020 7374 796c 653d  e".       style=
+000051d0: 2266 6f6e 742d 7374 796c 653a 6e6f 726d  "font-style:norm
+000051e0: 616c 3b66 6f6e 742d 7765 6967 6874 3a6e  al;font-weight:n
+000051f0: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
+00005200: 352e 3837 3239 3170 783b 6c69 6e65 2d68  5.87291px;line-h
+00005210: 6569 6768 743a 312e 3235 3b66 6f6e 742d  eight:1.25;font-
+00005220: 6661 6d69 6c79 3a73 616e 732d 7365 7269  family:sans-seri
+00005230: 663b 6c65 7474 6572 2d73 7061 6369 6e67  f;letter-spacing
+00005240: 3a30 7078 3b77 6f72 642d 7370 6163 696e  :0px;word-spacin
+00005250: 673a 3070 783b 6669 6c6c 3a23 3534 3534  g:0px;fill:#5454
+00005260: 3534 3b66 696c 6c2d 6f70 6163 6974 793a  54;fill-opacity:
+00005270: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
+00005280: 726f 6b65 2d77 6964 7468 3a30 2e34 3030  roke-width:0.400
+00005290: 3432 353b 6669 6c74 6572 3a75 726c 2823  425;filter:url(#
+000052a0: 6669 6c74 6572 3135 3035 312d 3329 220a  filter15051-3)".
+000052b0: 2020 2020 2020 2078 3d22 3737 2e36 3934         x="77.694
+000052c0: 3839 3322 0a20 2020 2020 2020 793d 2239  893".       y="9
+000052d0: 312e 3938 3834 3439 220a 2020 2020 2020  1.988449".      
+000052e0: 2069 643d 2274 6578 7431 3436 3931 2d36   id="text14691-6
+000052f0: 2d33 220a 2020 2020 2020 2074 7261 6e73  -3".       trans
+00005300: 666f 726d 3d22 6d61 7472 6978 2832 2e37  form="matrix(2.7
+00005310: 3531 3139 3139 2c30 2c30 2c32 2e37 3338  511919,0,0,2.738
+00005320: 3831 322c 3337 342e 3032 3333 312c 2d31  812,374.02331,-1
+00005330: 3038 2e30 3838 3636 2922 3e3c 7473 7061  08.08866)"><tspa
+00005340: 6e0a 2020 2020 2020 2020 2073 6f64 6970  n.         sodip
+00005350: 6f64 693a 726f 6c65 3d22 6c69 6e65 220a  odi:role="line".
+00005360: 2020 2020 2020 2020 2069 643d 2274 7370           id="tsp
+00005370: 616e 3134 3638 392d 322d 3722 0a20 2020  an14689-2-7".   
+00005380: 2020 2020 2020 783d 2237 372e 3639 3438        x="77.6948
+00005390: 3933 220a 2020 2020 2020 2020 2079 3d22  93".         y="
+000053a0: 3931 2e39 3838 3434 3922 0a20 2020 2020  91.988449".     
+000053b0: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
+000053c0: 7374 796c 653a 6e6f 726d 616c 3b66 6f6e  style:normal;fon
+000053d0: 742d 7661 7269 616e 743a 6e6f 726d 616c  t-variant:normal
+000053e0: 3b66 6f6e 742d 7765 6967 6874 3a6e 6f72  ;font-weight:nor
+000053f0: 6d61 6c3b 666f 6e74 2d73 7472 6574 6368  mal;font-stretch
+00005400: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 697a  :normal;font-siz
+00005410: 653a 3231 2e33 3536 7078 3b66 6f6e 742d  e:21.356px;font-
+00005420: 6661 6d69 6c79 3a49 6d70 6163 743b 2d69  family:Impact;-i
+00005430: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
+00005440: 6369 6669 6361 7469 6f6e 3a49 6d70 6163  cification:Impac
+00005450: 743b 6669 6c6c 3a23 3534 3534 3534 3b66  t;fill:#545454;f
 00005460: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00005470: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00005480: 6f6b 652d 7769 6474 683a 302e 3236 3435  oke-width:0.2645
-00005490: 3833 3b73 7472 6f6b 652d 6c69 6e65 6361  83;stroke-lineca
-000054a0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-000054b0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-000054c0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000054d0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000054e0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-000054f0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00005500: 643d 226d 2039 322e 3737 3932 3639 2c31  d="m 92.779269,1
-00005510: 3432 2e31 3133 3731 2034 2e39 3839 3630  42.11371 4.98960
-00005520: 372c 312e 3134 3034 3920 322e 3536 3630  7,1.14049 2.5660
-00005530: 3834 2c2d 392e 3535 3135 3420 7a22 0a20  84,-9.55154 z". 
-00005540: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00005550: 3534 392d 312d 3022 0a20 2020 2020 2020  549-1-0".       
-00005560: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00005570: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00005580: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00005590: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-000055a0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-000055b0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-000055c0: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-000055d0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-000055e0: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
-000055f0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00005600: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00005610: 652d 7769 6474 683a 302e 3236 3435 3833  e-width:0.264583
-00005620: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00005630: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00005640: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00005650: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00005660: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00005670: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00005680: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-00005690: 226d 2039 372e 3736 3838 3736 2c31 3433  "m 97.768876,143
-000056a0: 2e32 3534 3220 3133 2e33 3533 3134 342c  .2542 13.353144,
-000056b0: 322e 3337 3620 6320 2d35 2e32 3033 3439  2.376 c -5.20349
-000056c0: 2c2d 322e 3735 3038 3620 2d38 2e32 3136  ,-2.75086 -8.216
-000056d0: 3735 2c2d 372e 3137 3034 3520 2d31 302e  75,-7.17045 -10.
-000056e0: 3738 3730 362c 2d31 312e 3932 3735 3420  78706,-11.92754 
-000056f0: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
-00005700: 7468 3134 3535 312d 302d 3322 0a20 2020  th14551-0-3".   
-00005710: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-00005720: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-00005730: 3d22 3022 0a20 2020 2020 2020 736f 6469  ="0".       sodi
-00005740: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-00005750: 6363 6363 220a 2020 2020 2020 2069 6e6b  cccc".       ink
-00005760: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00005770: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-00005780: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-00005790: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-000057a0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-000057b0: 796c 653d 2266 696c 6c3a 2332 3733 3737  yle="fill:#27377
-000057c0: 333b 6669 6c6c 2d6f 7061 6369 7479 3a31  3;fill-opacity:1
-000057d0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-000057e0: 7374 726f 6b65 2d77 6964 7468 3a30 2e32  stroke-width:0.2
-000057f0: 3634 3538 333b 7374 726f 6b65 2d6c 696e  64583;stroke-lin
-00005800: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00005810: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00005820: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00005830: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00005840: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00005850: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00005860: 2020 2064 3d22 6d20 3831 2e32 3739 3431     d="m 81.27941
-00005870: 2c31 3432 2e36 3336 3433 2063 2032 2e35  ,142.63643 c 2.5
-00005880: 3330 3537 352c 312e 3435 3137 2035 2e33  30575,1.4517 5.3
-00005890: 3230 3639 322c 322e 3730 3337 3620 362e  20692,2.70376 6.
-000058a0: 3237 3236 3439 2c35 2e33 3639 3737 206c  272649,5.36977 l
-000058b0: 2035 2e32 3237 3231 2c2d 352e 3839 3234   5.22721,-5.8924
-000058c0: 3920 7a22 0a20 2020 2020 2020 6964 3d22  9 z".       id="
-000058d0: 7061 7468 3134 3535 332d 332d 3222 0a20  path14553-3-2". 
-000058e0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-000058f0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00005900: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-00005910: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00005920: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
-00005930: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00005940: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00005950: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00005960: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00005970: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00005980: 7374 796c 653d 2266 696c 6c3a 2331 3432  style="fill:#142
-00005990: 3637 323b 6669 6c6c 2d6f 7061 6369 7479  672;fill-opacity
-000059a0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-000059b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-000059c0: 2e32 3634 3538 333b 7374 726f 6b65 2d6c  .264583;stroke-l
-000059d0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-000059e0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-000059f0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
-00005a00: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00005a10: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-00005a20: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00005a30: 2020 2020 2064 3d22 6d20 3837 2e35 3532       d="m 87.552
-00005a40: 3035 392c 3134 382e 3030 3632 2032 332e  059,148.0062 23.
-00005a50: 3536 3939 3631 2c2d 322e 3337 3620 2d31  569961,-2.376 -1
-00005a60: 382e 3334 3237 3531 2c2d 332e 3531 3634  8.342751,-3.5164
-00005a70: 3920 7a22 0a20 2020 2020 2020 6964 3d22  9 z".       id="
-00005a80: 7061 7468 3134 3535 352d 342d 3122 0a20  path14555-4-1". 
-00005a90: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00005aa0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00005ab0: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
-00005ac0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-00005ad0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-00005ae0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00005af0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00005b00: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-00005b10: 7479 6c65 3d22 6669 6c6c 3a23 3534 3636  tyle="fill:#5466
-00005b20: 3863 3b66 696c 6c2d 6f70 6163 6974 793a  8c;fill-opacity:
-00005b30: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00005b40: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00005b50: 3236 3435 3833 3b73 7472 6f6b 652d 6c69  264583;stroke-li
-00005b60: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00005b70: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00005b80: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00005b90: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00005ba0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00005bb0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00005bc0: 2020 2020 643d 226d 2038 372e 3535 3230      d="m 87.5520
-00005bd0: 3539 2c31 3438 2e30 3036 3220 3133 2e35  59,148.0062 13.5
-00005be0: 3930 3734 312c 312e 3432 3536 2039 2e39  90741,1.4256 9.9
-00005bf0: 3739 3232 2c2d 332e 3830 3136 207a 220a  7922,-3.8016 z".
-00005c00: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00005c10: 3435 3537 2d30 2d37 220a 2020 2020 2020  4557-0-7".      
-00005c20: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-00005c30: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-00005c40: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00005c50: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-00005c60: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-00005c70: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-00005c80: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
-00005c90: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-00005ca0: 2266 696c 6c3a 2332 3233 3437 653b 6669  "fill:#22347e;fi
-00005cb0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-00005cc0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-00005cd0: 6b65 2d77 6964 7468 3a30 2e32 3634 3538  ke-width:0.26458
-00005ce0: 333b 7374 726f 6b65 2d6c 696e 6563 6170  3;stroke-linecap
-00005cf0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00005d00: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00005d10: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00005d20: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00005d30: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00005d40: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-00005d50: 3d22 6d20 3837 2e35 3532 3035 392c 3134  ="m 87.552059,14
-00005d60: 382e 3030 3632 2063 2030 2e33 3035 3630  8.0062 c 0.30560
-00005d70: 372c 322e 3633 3530 3220 2d30 2e37 3532  7,2.63502 -0.752
-00005d80: 3231 382c 342e 3239 3631 3720 2d31 2e32  218,4.29617 -1.2
-00005d90: 3335 3532 2c36 2e33 3637 3639 204c 2031  3552,6.36769 L 1
-00005da0: 3031 2e31 3432 382c 3134 392e 3433 3138  01.1428,149.4318
-00005db0: 205a 220a 2020 2020 2020 2069 643d 2270   Z".       id="p
-00005dc0: 6174 6831 3435 3539 2d33 2d34 220a 2020  ath14559-3-4".  
-00005dd0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00005de0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-00005df0: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
-00005e00: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-00005e10: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
-00005e20: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-00005e30: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-00005e40: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00005e50: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00005e60: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-00005e70: 7479 6c65 3d22 6669 6c6c 3a23 3038 3130  tyle="fill:#0810
-00005e80: 3639 3b66 696c 6c2d 6f70 6163 6974 793a  69;fill-opacity:
-00005e90: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00005ea0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00005eb0: 3236 3435 3833 3b73 7472 6f6b 652d 6c69  264583;stroke-li
-00005ec0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00005ed0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00005ee0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00005ef0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00005f00: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00005f10: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00005f20: 2020 2020 643d 226d 2038 362e 3331 3635      d="m 86.3165
-00005f30: 3339 2c31 3534 2e33 3733 3839 2031 302e  39,154.37389 10.
-00005f40: 3236 3433 3335 2c31 2e35 3230 3634 2031  264335,1.52064 1
-00005f50: 342e 3534 3131 3436 2c2d 3130 2e32 3634  4.541146,-10.264
-00005f60: 3333 207a 220a 2020 2020 2020 2069 643d  33 z".       id=
-00005f70: 2270 6174 6831 3435 3631 2d39 2d32 220a  "path14561-9-2".
-00005f80: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00005f90: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00005fa0: 7572 653d 2230 220a 2020 2020 2020 2069  ure="0".       i
-00005fb0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00005fc0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00005fd0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00005fe0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00005ff0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00006000: 7374 796c 653d 2266 696c 6c3a 2330 3730  style="fill:#070
-00006010: 6532 623b 6669 6c6c 2d6f 7061 6369 7479  e2b;fill-opacity
-00006020: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00006030: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-00006040: 2e32 3634 3538 333b 7374 726f 6b65 2d6c  .264583;stroke-l
-00006050: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-00006060: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-00006070: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
-00006080: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00006090: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-000060a0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-000060b0: 2020 2020 2064 3d22 6d20 3936 2e35 3830       d="m 96.580
-000060c0: 3837 342c 3135 352e 3839 3435 3320 362e  874,155.89453 6.
-000060d0: 3033 3530 3436 2c37 2e39 3335 3836 202d  035046,7.93586 -
-000060e0: 322e 3233 3334 342c 2d31 302e 3639 3230  2.23344,-10.6920
-000060f0: 3220 7a22 0a20 2020 2020 2020 6964 3d22  2 z".       id="
-00006100: 7061 7468 3134 3536 332d 312d 3022 0a20  path14563-1-0". 
-00006110: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00006120: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00006130: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
-00006140: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-00006150: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-00006160: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00006170: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00006180: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-00006190: 7479 6c65 3d22 6669 6c6c 3a23 3238 3364  tyle="fill:#283d
-000061a0: 3837 3b66 696c 6c2d 6f70 6163 6974 793a  87;fill-opacity:
-000061b0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-000061c0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000061d0: 3236 3435 3833 3b73 7472 6f6b 652d 6c69  264583;stroke-li
-000061e0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-000061f0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00006200: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00006210: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00006220: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00006230: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00006240: 2020 2020 643d 226d 2031 3030 2e33 3832      d="m 100.382
-00006250: 3438 2c31 3533 2e31 3338 3337 2032 2e32  48,153.13837 2.2
-00006260: 3333 3434 2c31 302e 3639 3230 3220 6320  3344,10.69202 c 
-00006270: 312e 3135 3632 312c 2d39 2e36 3131 3633  1.15621,-9.61163
-00006280: 2035 2e32 3235 3031 2c2d 3133 2e30 3734   5.22501,-13.074
-00006290: 3432 2038 2e35 3036 312c 2d31 382e 3230  42 8.5061,-18.20
-000062a0: 3031 3920 7a22 0a20 2020 2020 2020 6964  019 z".       id
-000062b0: 3d22 7061 7468 3134 3536 352d 392d 3522  ="path14565-9-5"
-000062c0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-000062d0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-000062e0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-000062f0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00006300: 6573 3d22 6363 6363 220a 2020 2020 2020  es="cccc".      
-00006310: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00006320: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-00006330: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-00006340: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-00006350: 0a20 2020 203c 656c 6c69 7073 650a 2020  .    <ellipse.  
-00006360: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00006370: 3a23 3037 3065 3262 3b66 696c 6c2d 6f70  :#070e2b;fill-op
-00006380: 6163 6974 793a 302e 3939 3034 3436 3b73  acity:0.990446;s
-00006390: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-000063a0: 726f 6b65 2d77 6964 7468 3a30 2e32 3634  roke-width:0.264
-000063b0: 3538 333b 7374 726f 6b65 2d6d 6974 6572  583;stroke-miter
-000063c0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-000063d0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-000063e0: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-000063f0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-00006400: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
-00006410: 6174 6831 3435 3637 2d36 2d31 220a 2020  ath14567-6-1".  
-00006420: 2020 2020 2063 783d 2238 312e 3532 3334       cx="81.5234
-00006430: 3833 220a 2020 2020 2020 2063 793d 2231  83".       cy="1
-00006440: 3432 2e36 3438 3634 220a 2020 2020 2020  42.64864".      
-00006450: 2072 783d 2230 2e35 3932 3534 3232 3322   rx="0.59254223"
-00006460: 0a20 2020 2020 2020 7279 3d22 302e 3539  .       ry="0.59
-00006470: 3235 3432 3239 220a 2020 2020 2020 2069  254229".       i
-00006480: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00006490: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-000064a0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000064b0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-000064c0: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-000064d0: 2020 723d 2230 2e35 3932 3534 3232 3922    r="0.59254229"
-000064e0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000064f0: 696c 6c3a 2332 3533 6137 643b 6669 6c6c  ill:#253a7d;fill
-00006500: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00006510: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00006520: 2d77 6964 7468 3a30 2e32 3634 3538 333b  -width:0.264583;
-00006530: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00006540: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00006550: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00006560: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00006570: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00006580: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00006590: 3435 3637 2d33 2d39 332d 3122 0a20 2020  4567-3-93-1".   
-000065a0: 2020 2020 6378 3d22 3836 2e32 3231 3138      cx="86.22118
-000065b0: 3422 0a20 2020 2020 2020 6379 3d22 3135  4".       cy="15
-000065c0: 342e 3234 3735 220a 2020 2020 2020 2069  4.2475".       i
-000065d0: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-000065e0: 6d2d 6365 6e74 6572 2d78 3d22 342e 3634  m-center-x="4.64
-000065f0: 3332 3536 3622 0a20 2020 2020 2020 696e  32566".       in
-00006600: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-00006610: 2d63 656e 7465 722d 793d 222d 392e 3937  -center-y="-9.97
-00006620: 3830 3632 3122 0a20 2020 2020 2020 696e  80621".       in
-00006630: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-00006640: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-00006650: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00006660: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00006670: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00006680: 2072 3d22 302e 3539 3235 3432 3239 220a   r="0.59254229".
-00006690: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000066a0: 6c6c 3a23 3235 3361 3764 3b66 696c 6c2d  ll:#253a7d;fill-
-000066b0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-000066c0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-000066d0: 7769 6474 683a 302e 3236 3435 3833 3b73  width:0.264583;s
-000066e0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-000066f0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00006700: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00006710: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00006720: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00006730: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00006740: 3536 372d 332d 372d 332d 3022 0a20 2020  567-3-7-3-0".   
-00006750: 2020 2020 6378 3d22 3130 302e 3233 3832      cx="100.2382
-00006760: 220a 2020 2020 2020 2063 793d 2231 3439  ".       cy="149
-00006770: 2e34 3639 3736 220a 2020 2020 2020 2069  .46976".       i
-00006780: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00006790: 6d2d 6365 6e74 6572 2d78 3d22 342e 3634  m-center-x="4.64
-000067a0: 3332 3536 3622 0a20 2020 2020 2020 696e  32566".       in
-000067b0: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-000067c0: 2d63 656e 7465 722d 793d 222d 392e 3937  -center-y="-9.97
-000067d0: 3830 3632 3122 0a20 2020 2020 2020 696e  80621".       in
-000067e0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-000067f0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-00006800: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00006810: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00006820: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00006830: 2072 3d22 302e 3539 3235 3432 3239 220a   r="0.59254229".
-00006840: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00006850: 6c6c 3a23 6138 6139 6161 3b66 696c 6c2d  ll:#a8a9aa;fill-
-00006860: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00006870: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00006880: 7769 6474 683a 302e 3236 3435 3833 3b73  width:0.264583;s
-00006890: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-000068a0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-000068b0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-000068c0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-000068d0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000068e0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000068f0: 3536 372d 332d 352d 382d 3822 0a20 2020  567-3-5-8-8".   
-00006900: 2020 2020 6378 3d22 3130 302e 3337 3837      cx="100.3787
-00006910: 3222 0a20 2020 2020 2020 6379 3d22 3135  2".       cy="15
-00006920: 332e 3035 3330 3522 0a20 2020 2020 2020  3.05305".       
-00006930: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00006940: 726d 2d63 656e 7465 722d 783d 2234 2e36  rm-center-x="4.6
-00006950: 3433 3235 3636 220a 2020 2020 2020 2069  432566".       i
-00006960: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00006970: 6d2d 6365 6e74 6572 2d79 3d22 2d39 2e39  m-center-y="-9.9
-00006980: 3738 3036 3231 220a 2020 2020 2020 2069  780621".       i
-00006990: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-000069a0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-000069b0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000069c0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-000069d0: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-000069e0: 2020 723d 2230 2e35 3932 3534 3232 3922    r="0.59254229"
-000069f0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00006a00: 696c 6c3a 2361 6261 6139 633b 6669 6c6c  ill:#abaa9c;fill
-00006a10: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00006a20: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00006a30: 2d77 6964 7468 3a30 2e32 3634 3538 333b  -width:0.264583;
-00006a40: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00006a50: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00006a60: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00006a70: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00006a80: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00006a90: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00006aa0: 3435 3637 2d33 2d39 2d30 2d39 220a 2020  4567-3-9-0-9".  
-00006ab0: 2020 2020 2063 783d 2239 362e 3732 3531       cx="96.7251
-00006ac0: 3539 220a 2020 2020 2020 2063 793d 2231  59".       cy="1
-00006ad0: 3535 2e38 3633 3438 220a 2020 2020 2020  55.86348".      
-00006ae0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00006af0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 342e  orm-center-x="4.
-00006b00: 3634 3332 3536 3622 0a20 2020 2020 2020  6432566".       
-00006b10: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00006b20: 726d 2d63 656e 7465 722d 793d 222d 392e  rm-center-y="-9.
-00006b30: 3937 3830 3632 3122 0a20 2020 2020 2020  9780621".       
-00006b40: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00006b50: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-00006b60: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00006b70: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-00006b80: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-00006b90: 2020 2072 3d22 302e 3931 3435 3035 3936     r="0.91450596
-00006ba0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-00006bb0: 6669 6c6c 3a23 3131 3230 3636 3b66 696c  fill:#112066;fil
-00006bc0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00006bd0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00006be0: 652d 7769 6474 683a 302e 3236 3435 3833  e-width:0.264583
-00006bf0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00006c00: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00006c10: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00006c20: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00006c30: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00006c40: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00006c50: 3134 3536 372d 332d 322d 352d 3422 0a20  14567-3-2-5-4". 
-00006c60: 2020 2020 2020 6378 3d22 3932 2e38 3630        cx="92.860
-00006c70: 3831 3722 0a20 2020 2020 2020 6379 3d22  817".       cy="
-00006c80: 3134 312e 3938 3722 0a20 2020 2020 2020  141.987".       
-00006c90: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00006ca0: 726d 2d63 656e 7465 722d 783d 2237 2e31  rm-center-x="7.1
-00006cb0: 3636 3231 3136 220a 2020 2020 2020 2069  662116".       i
-00006cc0: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00006cd0: 6d2d 6365 6e74 6572 2d79 3d22 2d31 352e  m-center-y="-15.
-00006ce0: 3339 3937 3531 220a 2020 2020 2020 2069  399751".       i
-00006cf0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00006d00: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00006d10: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00006d20: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00006d30: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-00006d40: 2020 723d 2230 2e35 3932 3534 3232 3922    r="0.59254229"
-00006d50: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00006d60: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
-00006d70: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-00006d80: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-00006d90: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00006da0: 3236 3435 3833 3b73 7472 6f6b 652d 6d69  264583;stroke-mi
-00006db0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00006dc0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00006dd0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
-00006de0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
-00006df0: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
-00006e00: 3d22 7061 7468 3134 3536 372d 322d 362d  ="path14567-2-6-
-00006e10: 3022 0a20 2020 2020 2020 6378 3d22 3937  0".       cx="97
-00006e20: 2e38 3134 3230 3122 0a20 2020 2020 2020  .814201".       
-00006e30: 6379 3d22 3134 332e 3030 3537 3722 0a20  cy="143.00577". 
-00006e40: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00006e50: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00006e60: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00006e70: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00006e80: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
-00006e90: 650a 2020 2020 2020 2072 3d22 302e 3539  e.       r="0.59
-00006ea0: 3235 3432 3239 220a 2020 2020 2020 2073  254229".       s
-00006eb0: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
-00006ec0: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
-00006ed0: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
-00006ee0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00006ef0: 6964 7468 3a30 2e32 3634 3538 333b 7374  idth:0.264583;st
-00006f00: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00006f10: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00006f20: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00006f30: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00006f40: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00006f50: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00006f60: 3637 2d32 2d38 2d36 2d37 220a 2020 2020  67-2-8-6-7".    
-00006f70: 2020 2063 783d 2238 372e 3535 3631 3337     cx="87.556137
-00006f80: 220a 2020 2020 2020 2063 793d 2231 3437  ".       cy="147
-00006f90: 2e39 3234 3033 220a 2020 2020 2020 2069  .92403".       i
-00006fa0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00006fb0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00006fc0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00006fd0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00006fe0: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-00006ff0: 2020 723d 2231 2e31 3236 3333 3537 220a    r="1.1263357".
-00007000: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00007010: 6c6c 3a23 6564 6630 6663 3b66 696c 6c2d  ll:#edf0fc;fill-
-00007020: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
-00007030: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-00007040: 7374 726f 6b65 2d77 6964 7468 3a30 2e32  stroke-width:0.2
-00007050: 3634 3538 333b 7374 726f 6b65 2d6d 6974  64583;stroke-mit
-00007060: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00007070: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00007080: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-00007090: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-000070a0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-000070b0: 2270 6174 6831 3435 3637 2d32 2d37 2d30  "path14567-2-7-0
-000070c0: 2d39 220a 2020 2020 2020 2063 783d 2231  -9".       cx="1
-000070d0: 3130 2e39 3137 3832 220a 2020 2020 2020  10.91782".      
-000070e0: 2063 793d 2231 3435 2e37 3831 3037 220a   cy="145.78107".
-000070f0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00007100: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-00007110: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00007120: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-00007130: 3030 2220 2f3e 0a20 2020 203c 670a 2020  00" />.    <g.  
-00007140: 2020 2020 2069 643d 2267 3930 342d 372d       id="g904-7-
-00007150: 3122 0a20 2020 2020 2020 7472 616e 7366  1".       transf
-00007160: 6f72 6d3d 226d 6174 7269 7828 302e 3137  orm="matrix(0.17
-00007170: 3737 3938 332c 302c 302c 302e 3137 3737  77983,0,0,0.1777
-00007180: 3938 332c 3132 352e 3831 3437 362c 3130  983,125.81476,10
-00007190: 382e 3135 3136 3929 223e 0a20 2020 2020  8.15169)">.     
-000071a0: 203c 7265 6374 0a20 2020 2020 2020 2020   <rect.         
-000071b0: 7374 796c 653d 226f 7061 6369 7479 3a31  style="opacity:1
-000071c0: 3b66 696c 6c3a 2362 3362 3362 333b 6669  ;fill:#b3b3b3;fi
-000071d0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-000071e0: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-000071f0: 7769 6474 683a 302e 3335 3439 3731 3b73  width:0.354971;s
-00007200: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00007210: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00007220: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00007230: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00007240: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00007250: 2020 2020 2020 2020 6964 3d22 7265 6374          id="rect
-00007260: 3135 3037 342d 302d 392d 3222 0a20 2020  15074-0-9-2".   
-00007270: 2020 2020 2020 7769 6474 683d 2239 352e        width="95.
-00007280: 3233 3930 3036 220a 2020 2020 2020 2020  239006".        
-00007290: 2068 6569 6768 743d 2239 352e 3233 3930   height="95.2390
-000072a0: 3036 220a 2020 2020 2020 2020 2078 3d22  06".         x="
-000072b0: 312e 3734 3233 3331 3622 0a20 2020 2020  1.7423316".     
-000072c0: 2020 2020 793d 2231 3330 2e33 3437 3422      y="130.3474"
-000072d0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000072e0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-000072f0: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00007300: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00007310: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00007320: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00007330: 2073 7479 6c65 3d22 6669 6c6c 3a23 3365   style="fill:#3e
-00007340: 3462 3737 3b66 696c 6c2d 6f70 6163 6974  4b77;fill-opacit
-00007350: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00007360: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00007370: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00007380: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00007390: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-000073a0: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-000073b0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-000073c0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-000073d0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000073e0: 2020 2020 2020 2020 643d 226d 2035 2e37          d="m 5.7
-000073f0: 3538 3439 3036 2c31 3631 2e38 3336 3531  584906,161.83651
-00007400: 2033 322e 3333 3936 3230 342c 2d31 2e34   32.3396204,-1.4
-00007410: 3639 3938 2032 312e 3234 3739 332c 2d32  6998 21.24793,-2
-00007420: 332e 3635 3333 3520 6320 2d32 362e 3736  3.65335 c -26.76
-00007430: 3738 392c 3138 2e30 3031 3837 202d 3339  789,18.00187 -39
-00007440: 2e35 3536 3434 2c32 302e 3839 3039 3520  .55644,20.89095 
-00007450: 2d35 332e 3538 3735 3530 342c 3235 2e31  -53.5875504,25.1
-00007460: 3233 3333 207a 220a 2020 2020 2020 2020  2333 z".        
-00007470: 2069 643d 2270 6174 6831 3435 3437 2d31   id="path14547-1
-00007480: 2d37 2d38 220a 2020 2020 2020 2020 2069  -7-8".         i
-00007490: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-000074a0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-000074b0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-000074c0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-000074d0: 6322 0a20 2020 2020 2020 2020 696e 6b73  c".         inks
-000074e0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-000074f0: 3d22 3330 3022 0a20 2020 2020 2020 2020  ="300".         
-00007500: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00007510: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00007520: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00007530: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00007540: 3163 3263 3638 3b66 696c 6c2d 6f70 6163  1c2c68;fill-opac
-00007550: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-00007560: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-00007570: 683a 302e 3535 3536 3235 3b73 7472 6f6b  h:0.555625;strok
-00007580: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00007590: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-000075a0: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-000075b0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-000075c0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-000075d0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-000075e0: 0a20 2020 2020 2020 2020 643d 226d 2033  .         d="m 3
-000075f0: 382e 3039 3831 3131 2c31 3630 2e33 3636  8.098111,160.366
-00007600: 3533 2031 342e 3033 3136 352c 332e 3230  53 14.03165,3.20
-00007610: 3732 3420 372e 3231 3632 382c 2d32 362e  724 7.21628,-26.
-00007620: 3836 3035 3920 7a22 0a20 2020 2020 2020  86059 z".       
-00007630: 2020 6964 3d22 7061 7468 3134 3534 392d    id="path14549-
-00007640: 312d 302d 3122 0a20 2020 2020 2020 2020  1-0-1".         
-00007650: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00007660: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00007670: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00007680: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00007690: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-000076a0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-000076b0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-000076c0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-000076d0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3036   style="fill:#06
-000076e0: 3035 3038 3b66 696c 6c2d 6f70 6163 6974  0508;fill-opacit
-000076f0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00007700: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00007710: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00007720: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00007730: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00007740: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00007750: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00007760: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00007770: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00007780: 2020 2020 2020 2020 643d 226d 2035 322e          d="m 52.
-00007790: 3132 3937 3631 2c31 3633 2e35 3733 3737  129761,163.57377
-000077a0: 2033 372e 3535 3133 372c 362e 3638 3137   37.55137,6.6817
-000077b0: 3420 6320 2d31 342e 3633 3331 322c 2d37  4 c -14.63312,-7
-000077c0: 2e37 3335 3839 202d 3233 2e31 3036 3934  .73589 -23.10694
-000077d0: 2c2d 3230 2e31 3634 3536 202d 3330 2e33  ,-20.16456 -30.3
-000077e0: 3335 3039 2c2d 3333 2e35 3432 3333 207a  3509,-33.54233 z
-000077f0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
-00007800: 6174 6831 3435 3531 2d30 2d33 2d39 220a  ath14551-0-3-9".
-00007810: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00007820: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00007830: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-00007840: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00007850: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
-00007860: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00007870: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00007880: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00007890: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-000078a0: 3330 3022 202f 3e0a 2020 2020 2020 3c70  300" />.      <p
-000078b0: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
-000078c0: 6c65 3d22 6669 6c6c 3a23 3237 3337 3733  le="fill:#273773
-000078d0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-000078e0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-000078f0: 7472 6f6b 652d 7769 6474 683a 302e 3535  troke-width:0.55
-00007900: 3536 3235 3b73 7472 6f6b 652d 6c69 6e65  5625;stroke-line
-00007910: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00007920: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00007930: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00007940: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00007950: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00007960: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00007970: 2020 2020 643d 226d 2035 2e37 3538 3439      d="m 5.75849
-00007980: 3036 2c31 3631 2e38 3336 3531 2063 2037  06,161.83651 c 7
-00007990: 2e31 3136 3432 3034 2c34 2e30 3832 3434  .1164204,4.08244
-000079a0: 2031 342e 3936 3237 3230 342c 372e 3630   14.9627204,7.60
-000079b0: 3334 3320 3137 2e36 3339 3739 3034 2c31  343 17.6397904,1
-000079c0: 352e 3130 3037 3420 6c20 3134 2e36 3939  5.10074 l 14.699
-000079d0: 3833 2c2d 3136 2e35 3730 3732 207a 220a  83,-16.57072 z".
-000079e0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-000079f0: 6831 3435 3533 2d33 2d32 2d32 220a 2020  h14553-3-2-2".  
-00007a00: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00007a10: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00007a20: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
-00007a30: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00007a40: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
-00007a50: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00007a60: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00007a70: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00007a80: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00007a90: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00007aa0: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00007ab0: 3d22 6669 6c6c 3a23 3134 3236 3732 3b66  ="fill:#142672;f
-00007ac0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00007ad0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00007ae0: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
-00007af0: 3235 3b73 7472 6f6b 652d 6c69 6e65 6361  25;stroke-lineca
-00007b00: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00007b10: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00007b20: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00007b30: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00007b40: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00007b50: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00007b60: 2020 643d 226d 2032 332e 3339 3832 3831    d="m 23.398281
-00007b70: 2c31 3736 2e39 3337 3235 2036 362e 3238  ,176.93725 66.28
-00007b80: 3238 352c 2d36 2e36 3831 3734 202d 3531  285,-6.68174 -51
-00007b90: 2e35 3833 3032 2c2d 392e 3838 3839 3820  .58302,-9.88898 
-00007ba0: 7a22 0a20 2020 2020 2020 2020 6964 3d22  z".         id="
-00007bb0: 7061 7468 3134 3535 352d 342d 312d 3622  path14555-4-1-6"
-00007bc0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00007bd0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00007be0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-00007bf0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00007c00: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00007c10: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00007c20: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00007c30: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00007c40: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00007c50: 3d22 6669 6c6c 3a23 3534 3636 3863 3b66  ="fill:#54668c;f
-00007c60: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00007c70: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00007c80: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
-00007c90: 3235 3b73 7472 6f6b 652d 6c69 6e65 6361  25;stroke-lineca
-00007ca0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00007cb0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00007cc0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00007cd0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00007ce0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00007cf0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00007d00: 2020 643d 226d 2032 332e 3339 3832 3831    d="m 23.398281
-00007d10: 2c31 3736 2e39 3337 3235 2033 382e 3231  ,176.93725 38.21
-00007d20: 3935 352c 342e 3030 3930 3420 3238 2e30  955,4.00904 28.0
-00007d30: 3633 332c 2d31 302e 3639 3037 3820 7a22  633,-10.69078 z"
-00007d40: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00007d50: 7468 3134 3535 372d 302d 372d 3322 0a20  th14557-0-7-3". 
-00007d60: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00007d70: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-00007d80: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-00007d90: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00007da0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-00007db0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00007dc0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00007dd0: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
-00007de0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00007df0: 6669 6c6c 3a23 3232 3334 3765 3b66 696c  fill:#22347e;fil
-00007e00: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00007e10: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00007e20: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00007e30: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00007e40: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00007e50: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00007e60: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00007e70: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00007e80: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00007e90: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00007ea0: 643d 226d 2032 332e 3339 3832 3831 2c31  d="m 23.398281,1
-00007eb0: 3736 2e39 3337 3235 2063 2030 2e38 3539  76.93725 c 0.859
-00007ec0: 3432 2c37 2e34 3130 3134 202d 322e 3131  42,7.41014 -2.11
-00007ed0: 3533 372c 3132 2e30 3831 3537 202d 332e  537,12.08157 -3.
-00007ee0: 3437 3435 2c31 372e 3930 3730 3520 6c20  4745,17.90705 l 
-00007ef0: 3431 2e36 3934 3035 2c2d 3133 2e38 3938  41.69405,-13.898
-00007f00: 3031 207a 220a 2020 2020 2020 2020 2069  01 z".         i
-00007f10: 643d 2270 6174 6831 3435 3539 2d33 2d34  d="path14559-3-4
-00007f20: 2d32 220a 2020 2020 2020 2020 2069 6e6b  -2".         ink
-00007f30: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-00007f40: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-00007f50: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00007f60: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-00007f70: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00007f80: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00007f90: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00007fa0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00007fb0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00007fc0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00007fd0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3038   style="fill:#08
-00007fe0: 3130 3639 3b66 696c 6c2d 6f70 6163 6974  1069;fill-opacit
-00007ff0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00008000: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00008010: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00008020: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00008030: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00008040: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00008050: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00008060: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00008070: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00008080: 2020 2020 2020 2020 643d 226d 2031 392e          d="m 19.
-00008090: 3932 3337 3831 2c31 3934 2e38 3434 3320  923781,194.8443 
-000080a0: 3238 2e38 3635 3131 2c34 2e32 3736 3332  28.86511,4.27632
-000080b0: 2034 302e 3839 3232 342c 2d32 382e 3836   40.89224,-28.86
-000080c0: 3531 3120 7a22 0a20 2020 2020 2020 2020  511 z".         
-000080d0: 6964 3d22 7061 7468 3134 3536 312d 392d  id="path14561-9-
-000080e0: 322d 3222 0a20 2020 2020 2020 2020 696e  2-2".         in
-000080f0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00008100: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00008110: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00008120: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00008130: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00008140: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00008150: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00008160: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00008170: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
-00008180: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
-00008190: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-000081a0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000081b0: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-000081c0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-000081d0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-000081e0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-000081f0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00008200: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00008210: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00008220: 2020 2020 2020 643d 226d 2034 382e 3738        d="m 48.78
-00008230: 3838 3931 2c31 3939 2e31 3230 3632 2031  8891,199.12062 1
-00008240: 362e 3937 3136 312c 3232 2e33 3137 3031  6.97161,22.31701
-00008250: 202d 362e 3238 3038 332c 2d33 302e 3036   -6.28083,-30.06
-00008260: 3738 3220 7a22 0a20 2020 2020 2020 2020  782 z".         
-00008270: 6964 3d22 7061 7468 3134 3536 332d 312d  id="path14563-1-
-00008280: 302d 3622 0a20 2020 2020 2020 2020 696e  0-6".         in
-00008290: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-000082a0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-000082b0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000082c0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-000082d0: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-000082e0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-000082f0: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00008300: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00008310: 7479 6c65 3d22 6669 6c6c 3a23 3238 3364  tyle="fill:#283d
-00008320: 3837 3b66 696c 6c2d 6f70 6163 6974 793a  87;fill-opacity:
-00008330: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00008340: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00008350: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-00008360: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00008370: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00008380: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00008390: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-000083a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000083b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000083c0: 2020 2020 2020 643d 226d 2035 392e 3437        d="m 59.47
-000083d0: 3936 3731 2c31 3931 2e33 3639 3831 2036  9671,191.36981 6
-000083e0: 2e32 3830 3833 2c33 302e 3036 3738 3220  .28083,30.06782 
-000083f0: 6320 332e 3235 3134 352c 2d32 372e 3032  c 3.25145,-27.02
-00008400: 3935 3720 3134 2e36 3933 3635 2c2d 3336  957 14.69365,-36
-00008410: 2e37 3637 3536 2032 332e 3932 3036 332c  .76756 23.92063,
-00008420: 2d35 312e 3138 3231 3220 7a22 0a20 2020  -51.18212 z".   
-00008430: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00008440: 3536 352d 392d 352d 3922 0a20 2020 2020  565-9-5-9".     
-00008450: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-00008460: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-00008470: 3d22 3022 0a20 2020 2020 2020 2020 736f  ="0".         so
-00008480: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00008490: 3d22 6363 6363 220a 2020 2020 2020 2020  ="cccc".        
-000084a0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000084b0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-000084c0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-000084d0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-000084e0: 2f3e 0a20 2020 2020 203c 656c 6c69 7073  />.      <ellips
-000084f0: 650a 2020 2020 2020 2020 2073 7479 6c65  e.         style
-00008500: 3d22 6f70 6163 6974 793a 313b 6669 6c6c  ="opacity:1;fill
-00008510: 3a23 3037 3065 3262 3b66 696c 6c2d 6f70  :#070e2b;fill-op
-00008520: 6163 6974 793a 302e 3939 3034 3436 3b73  acity:0.990446;s
-00008530: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00008540: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
-00008550: 3632 353b 7374 726f 6b65 2d6d 6974 6572  625;stroke-miter
-00008560: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00008570: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00008580: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-00008590: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-000085a0: 3a31 220a 2020 2020 2020 2020 2069 643d  :1".         id=
-000085b0: 2270 6174 6831 3435 3637 2d36 2d31 2d39  "path14567-6-1-9
-000085c0: 220a 2020 2020 2020 2020 2063 783d 2236  ".         cx="6
-000085d0: 2e34 3434 3836 3238 220a 2020 2020 2020  .4448628".      
-000085e0: 2020 2063 793d 2231 3631 2e38 3730 3832     cy="161.87082
-000085f0: 220a 2020 2020 2020 2020 2072 783d 2231  ".         rx="1
-00008600: 2e36 3636 3333 3237 220a 2020 2020 2020  .6663327".      
-00008610: 2020 2072 793d 2231 2e36 3636 3333 3238     ry="1.6663328
-00008620: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00008630: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-00008640: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
-00008650: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-00008660: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-00008670: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-00008680: 2020 2020 723d 2231 2e36 3636 3333 3238      r="1.6663328
-00008690: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
-000086a0: 3d22 6f70 6163 6974 793a 313b 6669 6c6c  ="opacity:1;fill
-000086b0: 3a23 3235 3361 3764 3b66 696c 6c2d 6f70  :#253a7d;fill-op
-000086c0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-000086d0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-000086e0: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
-000086f0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00008700: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00008710: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00008720: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-00008730: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00008740: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00008750: 3536 372d 332d 3933 2d31 2d36 220a 2020  567-3-93-1-6".  
-00008760: 2020 2020 2020 2063 783d 2231 392e 3635         cx="19.65
-00008770: 3536 3332 220a 2020 2020 2020 2020 2063  5632".         c
-00008780: 793d 2231 3934 2e34 3838 3835 220a 2020  y="194.48885".  
-00008790: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000087a0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-000087b0: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
-000087c0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000087d0: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-000087e0: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
-000087f0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00008800: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00008810: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00008820: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008830: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008840: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00008850: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-00008860: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00008870: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-00008880: 2332 3533 6137 643b 6669 6c6c 2d6f 7061  #253a7d;fill-opa
-00008890: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-000088a0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000088b0: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-000088c0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-000088d0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-000088e0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-000088f0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00008900: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00008910: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00008920: 3637 2d33 2d37 2d33 2d30 2d39 220a 2020  67-3-7-3-0-9".  
-00008930: 2020 2020 2020 2063 783d 2235 392e 3037         cx="59.07
-00008940: 3339 3231 220a 2020 2020 2020 2020 2063  3921".         c
-00008950: 793d 2231 3831 2e30 3533 3031 220a 2020  y="181.05301".  
-00008960: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00008970: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00008980: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
-00008990: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000089a0: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-000089b0: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
-000089c0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000089d0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-000089e0: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-000089f0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008a00: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008a10: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00008a20: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-00008a30: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00008a40: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-00008a50: 2361 3861 3961 613b 6669 6c6c 2d6f 7061  #a8a9aa;fill-opa
-00008a60: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00008a70: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00008a80: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-00008a90: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00008aa0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00008ab0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-00008ac0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00008ad0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00008ae0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00008af0: 3637 2d33 2d35 2d38 2d38 2d35 220a 2020  67-3-5-8-8-5".  
-00008b00: 2020 2020 2020 2063 783d 2235 392e 3436         cx="59.46
-00008b10: 3930 3933 220a 2020 2020 2020 2020 2063  9093".         c
-00008b20: 793d 2231 3931 2e31 3239 3837 220a 2020  y="191.12987".  
-00008b30: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00008b40: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00008b50: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
+00005470: 726f 6b65 2d77 6964 7468 3a30 2e34 3030  roke-width:0.400
+00005480: 3432 3522 3e53 6165 6e6f 7079 3c2f 7473  425">Saenopy</ts
+00005490: 7061 6e3e 3c2f 7465 7874 3e0a 2020 2020  pan></text>.    
+000054a0: 3c74 6578 740a 2020 2020 2020 2078 6d6c  <text.       xml
+000054b0: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+000054c0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+000054d0: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
+000054e0: 6c3b 666f 6e74 2d77 6569 6768 743a 6e6f  l;font-weight:no
+000054f0: 726d 616c 3b66 6f6e 742d 7369 7a65 3a31  rmal;font-size:1
+00005500: 362e 3132 3131 7078 3b6c 696e 652d 6865  6.1211px;line-he
+00005510: 6967 6874 3a31 2e32 353b 666f 6e74 2d66  ight:1.25;font-f
+00005520: 616d 696c 793a 7361 6e73 2d73 6572 6966  amily:sans-serif
+00005530: 3b6c 6574 7465 722d 7370 6163 696e 673a  ;letter-spacing:
+00005540: 3070 783b 776f 7264 2d73 7061 6369 6e67  0px;word-spacing
+00005550: 3a30 7078 3b66 696c 6c3a 2366 6666 6666  :0px;fill:#fffff
+00005560: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+00005570: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
+00005580: 6f6b 652d 7769 6474 683a 312e 3039 3931  oke-width:1.0991
+00005590: 3722 0a20 2020 2020 2020 783d 2235 3834  7".       x="584
+000055a0: 2e34 3635 3532 220a 2020 2020 2020 2079  .46552".       y
+000055b0: 3d22 3133 362e 3338 3737 220a 2020 2020  ="136.3877".    
+000055c0: 2020 2069 643d 2274 6578 7431 3436 3931     id="text14691
+000055d0: 2d35 220a 2020 2020 2020 2074 7261 6e73  -5".       trans
+000055e0: 666f 726d 3d22 7363 616c 6528 312e 3030  form="scale(1.00
+000055f0: 3232 3537 352c 302e 3939 3737 3437 3538  22575,0.99774758
+00005600: 2922 3e3c 7473 7061 6e0a 2020 2020 2020  )"><tspan.      
+00005610: 2020 2073 6f64 6970 6f64 693a 726f 6c65     sodipodi:role
+00005620: 3d22 6c69 6e65 220a 2020 2020 2020 2020  ="line".        
+00005630: 2069 643d 2274 7370 616e 3134 3638 392d   id="tspan14689-
+00005640: 3922 0a20 2020 2020 2020 2020 783d 2235  9".         x="5
+00005650: 3834 2e34 3635 3532 220a 2020 2020 2020  84.46552".      
+00005660: 2020 2079 3d22 3133 362e 3338 3737 220a     y="136.3877".
+00005670: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00005680: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
+00005690: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
+000056a0: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
+000056b0: 743a 6e6f 726d 616c 3b66 6f6e 742d 7374  t:normal;font-st
+000056c0: 7265 7463 683a 6e6f 726d 616c 3b66 6f6e  retch:normal;fon
+000056d0: 742d 7369 7a65 3a35 382e 3632 3231 7078  t-size:58.6221px
+000056e0: 3b66 6f6e 742d 6661 6d69 6c79 3a27 546c  ;font-family:'Tl
+000056f0: 7767 2054 7970 6973 7427 3b2d 696e 6b73  wg Typist';-inks
+00005700: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
+00005710: 6963 6174 696f 6e3a 2754 6c77 6720 5479  ication:'Tlwg Ty
+00005720: 7069 7374 273b 7374 726f 6b65 2d77 6964  pist';stroke-wid
+00005730: 7468 3a31 2e30 3939 3137 3b66 696c 6c3a  th:1.09917;fill:
+00005740: 2366 6666 6666 663b 6669 6c6c 2d6f 7061  #ffffff;fill-opa
+00005750: 6369 7479 3a31 223e 5361 656e 6f70 793c  city:1">Saenopy<
+00005760: 2f74 7370 616e 3e3c 2f74 6578 743e 0a20  /tspan></text>. 
+00005770: 2020 203c 670a 2020 2020 2020 2069 643d     <g.       id=
+00005780: 2267 3134 3238 2d37 2d38 220a 2020 2020  "g1428-7-8".    
+00005790: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+000057a0: 616e 736c 6174 6528 3930 302e 3030 3030  anslate(900.0000
+000057b0: 3129 223e 0a20 2020 2020 203c 7265 6374  1)">.      <rect
+000057c0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000057d0: 2266 696c 6c3a 2366 6666 6666 663b 7374  "fill:#ffffff;st
+000057e0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
+000057f0: 2d77 6964 7468 3a35 2e30 3834 3736 3b73  -width:5.08476;s
+00005800: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
+00005810: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
+00005820: 6f69 6e3a 726f 756e 6422 0a20 2020 2020  oin:round".     
+00005830: 2020 2020 6964 3d22 7265 6374 3730 362d      id="rect706-
+00005840: 352d 3922 0a20 2020 2020 2020 2020 7769  5-9".         wi
+00005850: 6474 683d 2234 3030 220a 2020 2020 2020  dth="400".      
+00005860: 2020 2068 6569 6768 743d 2232 3030 220a     height="200".
+00005870: 2020 2020 2020 2020 2078 3d22 2d36 2e36           x="-6.6
+00005880: 3936 3531 3331 652d 3036 220a 2020 2020  965131e-06".    
+00005890: 2020 2020 2079 3d22 2d31 2e38 3532 3036       y="-1.85206
+000058a0: 3131 652d 3036 220a 2020 2020 2020 2020  11e-06".        
+000058b0: 2072 793d 2230 2220 2f3e 0a20 2020 2020   ry="0" />.     
+000058c0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+000058d0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+000058e0: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
+000058f0: 3a30 2e39 3938 3430 383b 7374 726f 6b65  :0.998408;stroke
+00005900: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00005910: 7769 6474 683a 302e 3530 3030 3232 7078  width:0.500022px
+00005920: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00005930: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00005940: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00005950: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00005960: 2020 2020 2020 643d 224d 2031 3733 2e38        d="M 173.8
+00005970: 3438 3131 2c38 392e 3036 3935 3120 3333  4811,89.06951 33
+00005980: 372e 3635 3039 362c 3634 2e39 3439 3731  7.65096,64.94971
+00005990: 2031 3731 2e38 3734 3435 2c38 302e 3731   171.87445,80.71
+000059a0: 3433 3620 5a22 0a20 2020 2020 2020 2020  436 Z".         
+000059b0: 6964 3d22 7061 7468 3134 3635 372d 332d  id="path14657-3-
+000059c0: 3722 0a20 2020 2020 2020 2020 696e 6b73  7".         inks
+000059d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+000059e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+000059f0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00005a00: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+00005a10: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+00005a20: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00005a30: 696c 6c3a 2333 6534 6237 373b 6669 6c6c  ill:#3e4b77;fill
+00005a40: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00005a50: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00005a60: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00005a70: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00005a80: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00005a90: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00005aa0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00005ab0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00005ac0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00005ad0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+00005ae0: 224d 2031 392e 3630 3330 372c 3637 2e36  "M 19.60307,67.6
+00005af0: 3536 3920 3830 2e38 3538 3032 382c 3634  569 80.858028,64
+00005b00: 2e38 3835 3132 2031 3231 2e31 3034 3035  .88512 121.10405
+00005b10: 2c32 302e 3238 3435 3420 4320 3730 2e34  ,20.28454 C 70.4
+00005b20: 3032 3538 372c 3534 2e32 3238 3733 2034  02587,54.22873 4
+00005b30: 362e 3137 3936 3035 2c35 392e 3637 3633  6.179605,59.6763
+00005b40: 3720 3139 2e36 3033 3037 2c36 372e 3635  7 19.60307,67.65
+00005b50: 3639 205a 220a 2020 2020 2020 2020 2069  69 Z".         i
+00005b60: 643d 2270 6174 6831 3435 3437 2d35 2d33  d="path14547-5-3
+00005b70: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00005b80: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00005b90: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00005ba0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00005bb0: 6465 7479 7065 733d 2263 6363 6322 202f  detypes="cccc" /
+00005bc0: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+00005bd0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00005be0: 6c6c 3a23 3163 3263 3638 3b66 696c 6c2d  ll:#1c2c68;fill-
+00005bf0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00005c00: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00005c10: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
+00005c20: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00005c30: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00005c40: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+00005c50: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00005c60: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00005c70: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+00005c80: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+00005c90: 6d20 3830 2e38 3538 3032 382c 3634 2e38  m 80.858028,64.8
+00005ca0: 3835 3132 2032 362e 3537 3735 3632 2c36  8512 26.577562,6
+00005cb0: 2e30 3437 3534 2031 332e 3636 3834 362c  .04754 13.66846,
+00005cc0: 2d35 302e 3634 3831 3220 7a22 0a20 2020  -50.64812 z".   
+00005cd0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00005ce0: 3534 392d 362d 3622 0a20 2020 2020 2020  549-6-6".       
+00005cf0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00005d00: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00005d10: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
+00005d20: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00005d30: 3d22 6669 6c6c 3a23 3036 3035 3038 3b66  ="fill:#060508;f
+00005d40: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00005d50: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00005d60: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00005d70: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
+00005d80: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00005d90: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00005da0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00005db0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00005dc0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00005dd0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00005de0: 2064 3d22 4d20 3130 372e 3433 3535 392c   d="M 107.43559,
+00005df0: 3730 2e39 3332 3636 2031 3738 2e35 3632  70.93266 178.562
+00005e00: 3233 2c38 332e 3533 3137 2043 2031 3530  23,83.5317 C 150
+00005e10: 2e38 3435 3431 2c36 382e 3934 3439 3720  .84541,68.94497 
+00005e20: 3133 342e 3739 3530 312c 3435 2e35 3039  134.79501,45.509
+00005e30: 3535 2031 3231 2e31 3034 3035 2c32 302e  55 121.10405,20.
+00005e40: 3238 3435 3420 5a22 0a20 2020 2020 2020  28454 Z".       
+00005e50: 2020 6964 3d22 7061 7468 3134 3535 312d    id="path14551-
+00005e60: 322d 3122 0a20 2020 2020 2020 2020 696e  2-1".         in
+00005e70: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00005e80: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00005e90: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+00005ea0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00005eb0: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+00005ec0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00005ed0: 2266 696c 6c3a 2332 3733 3737 333b 6669  "fill:#273773;fi
+00005ee0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00005ef0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00005f00: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00005f10: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00005f20: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00005f30: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00005f40: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00005f50: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00005f60: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00005f70: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00005f80: 643d 226d 2031 392e 3630 3330 372c 3637  d="m 19.60307,67
+00005f90: 2e36 3536 3920 6320 3133 2e34 3739 3331  .6569 c 13.47931
+00005fa0: 322c 372e 3639 3738 2032 382e 3334 3131  2,7.6978 28.3411
+00005fb0: 3037 2c31 342e 3333 3639 3520 3333 2e34  07,14.33695 33.4
+00005fc0: 3131 3739 362c 3238 2e34 3733 3832 206c  11796,28.47382 l
+00005fd0: 2032 372e 3834 3331 3632 2c2d 3331 2e32   27.843162,-31.2
+00005fe0: 3435 3620 7a22 0a20 2020 2020 2020 2020  456 z".         
+00005ff0: 6964 3d22 7061 7468 3134 3535 332d 392d  id="path14553-9-
+00006000: 3222 0a20 2020 2020 2020 2020 696e 6b73  2".         inks
+00006010: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00006020: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+00006030: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00006040: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+00006050: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+00006060: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00006070: 696c 6c3a 2331 3432 3637 323b 6669 6c6c  ill:#142672;fill
+00006080: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00006090: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+000060a0: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+000060b0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+000060c0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+000060d0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+000060e0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+000060f0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00006100: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00006110: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+00006120: 224d 2035 332e 3031 3438 3636 2c39 362e  "M 53.014866,96.
+00006130: 3133 3037 3220 3137 382e 3536 3232 332c  13072 178.56223,
+00006140: 3833 2e35 3331 3720 3830 2e38 3538 3032  83.5317 80.85802
+00006150: 382c 3634 2e38 3835 3132 205a 220a 2020  8,64.88512 Z".  
+00006160: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00006170: 3435 3535 2d31 2d39 220a 2020 2020 2020  4555-1-9".      
+00006180: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00006190: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000061a0: 2230 2220 2f3e 0a20 2020 2020 203c 7061  "0" />.      <pa
+000061b0: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+000061c0: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
+000061d0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+000061e0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+000061f0: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+00006200: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
+00006210: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00006220: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00006230: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00006240: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00006250: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00006260: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00006270: 2020 643d 226d 2035 332e 3031 3438 3636    d="m 53.014866
+00006280: 2c39 362e 3133 3037 3220 3732 2e33 3932  ,96.13072 72.392
+00006290: 3232 342c 372e 3535 3934 3420 3533 2e31  224,7.55944 53.1
+000062a0: 3535 3134 2c2d 3230 2e31 3538 3436 207a  5514,-20.15846 z
+000062b0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+000062c0: 6174 6831 3435 3537 2d32 2d33 220a 2020  ath14557-2-3".  
+000062d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000062e0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+000062f0: 7572 653d 2230 2220 2f3e 0a20 2020 2020  ure="0" />.     
+00006300: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+00006310: 7374 796c 653d 2266 696c 6c3a 2332 3233  style="fill:#223
+00006320: 3437 653b 6669 6c6c 2d6f 7061 6369 7479  47e;fill-opacity
+00006330: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00006340: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00006350: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
+00006360: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00006370: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00006380: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00006390: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000063a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000063b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000063c0: 2020 2020 2020 643d 226d 2035 332e 3031        d="m 53.01
+000063d0: 3438 3636 2c39 362e 3133 3037 3220 6320  4866,96.13072 c 
+000063e0: 312e 3632 3738 3235 2c31 332e 3937 3235  1.627825,13.9725
+000063f0: 3220 2d34 2e30 3036 3737 322c 3232 2e37  2 -4.006772,22.7
+00006400: 3830 3933 202d 362e 3538 3131 3039 2c33  8093 -6.581109,3
+00006410: 332e 3736 3534 3120 6c20 3738 2e39 3733  3.76541 l 78.973
+00006420: 3333 332c 2d32 362e 3230 3539 3720 7a22  333,-26.20597 z"
+00006430: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00006440: 7468 3134 3535 392d 372d 3122 0a20 2020  th14559-7-1".   
+00006450: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00006460: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00006470: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
+00006480: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+00006490: 6573 3d22 6363 6363 2220 2f3e 0a20 2020  es="cccc" />.   
+000064a0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+000064b0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+000064c0: 3831 3036 393b 6669 6c6c 2d6f 7061 6369  81069;fill-opaci
+000064d0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+000064e0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+000064f0: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00006500: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00006510: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00006520: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+00006530: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00006540: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00006550: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00006560: 2020 2020 2020 2020 643d 224d 2034 362e          d="M 46.
+00006570: 3433 3337 3537 2c31 3239 2e38 3936 3133  433757,129.89613
+00006580: 2031 3031 2e31 3037 362c 3133 372e 3935   101.1076,137.95
+00006590: 3935 3120 3137 382e 3536 3232 332c 3833  951 178.56223,83
+000065a0: 2e35 3331 3720 5a22 0a20 2020 2020 2020  .5317 Z".       
+000065b0: 2020 6964 3d22 7061 7468 3134 3536 312d    id="path14561-
+000065c0: 302d 3922 0a20 2020 2020 2020 2020 696e  0-9".         in
+000065d0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+000065e0: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+000065f0: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+00006600: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00006610: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
+00006620: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00006630: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00006640: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
+00006650: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00006660: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00006670: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+00006680: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00006690: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000066a0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+000066b0: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+000066c0: 6d20 3130 312e 3130 3736 2c31 3337 2e39  m 101.1076,137.9
+000066d0: 3539 3531 2033 322e 3134 3631 392c 3432  5951 32.14619,42
+000066e0: 2e30 3830 3739 202d 3131 2e38 3936 3632  .08079 -11.89662
+000066f0: 2c2d 3536 2e36 3935 3636 207a 220a 2020  ,-56.69566 z".  
+00006700: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00006710: 3435 3633 2d39 2d34 220a 2020 2020 2020  4563-9-4".      
+00006720: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00006730: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00006740: 2230 2220 2f3e 0a20 2020 2020 203c 7061  "0" />.      <pa
+00006750: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+00006760: 653d 2266 696c 6c3a 2332 3833 6438 373b  e="fill:#283d87;
+00006770: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00006780: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00006790: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+000067a0: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
+000067b0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+000067c0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+000067d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+000067e0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+000067f0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00006800: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00006810: 2020 643d 226d 2031 3231 2e33 3537 3137    d="m 121.35717
+00006820: 2c31 3233 2e33 3434 3634 2031 312e 3839  ,123.34464 11.89
+00006830: 3636 322c 3536 2e36 3935 3636 2063 2036  662,56.69566 c 6
+00006840: 2e31 3538 3632 2c2d 3530 2e39 3636 3733  .15862,-50.96673
+00006850: 2032 372e 3833 3134 372c 2d36 392e 3332   27.83147,-69.32
+00006860: 3836 3120 3435 2e33 3038 3434 2c2d 3936  861 45.30844,-96
+00006870: 2e35 3038 3620 7a22 0a20 2020 2020 2020  .5086 z".       
+00006880: 2020 6964 3d22 7061 7468 3134 3536 352d    id="path14565-
+00006890: 332d 3722 0a20 2020 2020 2020 2020 696e  3-7".         in
+000068a0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+000068b0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+000068c0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+000068d0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+000068e0: 2220 2f3e 0a20 2020 2020 203c 656c 6c69  " />.      <elli
+000068f0: 7073 650a 2020 2020 2020 2020 2073 7479  pse.         sty
+00006900: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
+00006910: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
+00006920: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
+00006930: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00006940: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+00006950: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00006960: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00006970: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+00006980: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+00006990: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+000069a0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+000069b0: 372d 3630 2d38 220a 2020 2020 2020 2020  7-60-8".        
+000069c0: 2063 783d 2232 302e 3930 3331 3138 220a   cx="20.903118".
+000069d0: 2020 2020 2020 2020 2063 793d 2236 372e           cy="67.
+000069e0: 3732 3135 3838 220a 2020 2020 2020 2020  721588".        
+000069f0: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
+00006a00: 2020 2020 2020 2020 2072 793d 2233 2e31           ry="3.1
+00006a10: 3432 3032 3422 202f 3e0a 2020 2020 2020  42024" />.      
+00006a20: 3c65 6c6c 6970 7365 0a20 2020 2020 2020  <ellipse.       
+00006a30: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
+00006a40: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
+00006a50: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00006a60: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00006a70: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00006a80: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00006a90: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00006aa0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00006ab0: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00006ac0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00006ad0: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+00006ae0: 332d 362d 3422 0a20 2020 2020 2020 2020  3-6-4".         
+00006af0: 6378 3d22 3435 2e39 3235 3834 3622 0a20  cx="45.925846". 
+00006b00: 2020 2020 2020 2020 6379 3d22 3132 392e          cy="129.
+00006b10: 3232 3538 3822 0a20 2020 2020 2020 2020  22588".         
+00006b20: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00006b30: 726d 2d63 656e 7465 722d 783d 2232 2e33  rm-center-x="2.3
+00006b40: 3236 3937 3435 220a 2020 2020 2020 2020  269745".        
+00006b50: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00006b60: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d34  orm-center-y="-4
+00006b70: 2e39 3738 3031 3633 220a 2020 2020 2020  .9780163".      
+00006b80: 2020 2072 783d 2233 2e31 3536 3232 3634     rx="3.1562264
+00006b90: 220a 2020 2020 2020 2020 2072 793d 2233  ".         ry="3
+00006ba0: 2e31 3432 3032 3422 202f 3e0a 2020 2020  .142024" />.    
+00006bb0: 2020 3c65 6c6c 6970 7365 0a20 2020 2020    <ellipse.     
+00006bc0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00006bd0: 2332 3533 6137 643b 6669 6c6c 2d6f 7061  #253a7d;fill-opa
+00006be0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+00006bf0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00006c00: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+00006c10: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00006c20: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00006c30: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+00006c40: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+00006c50: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00006c60: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00006c70: 372d 332d 372d 322d 3522 0a20 2020 2020  7-3-7-2-5".     
+00006c80: 2020 2020 6378 3d22 3132 302e 3538 3836      cx="120.5886
+00006c90: 3222 0a20 2020 2020 2020 2020 6379 3d22  2".         cy="
+00006ca0: 3130 332e 3839 3133 3922 0a20 2020 2020  103.89139".     
+00006cb0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+00006cc0: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
+00006cd0: 2232 2e33 3236 3937 3932 220a 2020 2020  "2.3269792".    
+00006ce0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+00006cf0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+00006d00: 3d22 2d34 2e39 3738 3032 3034 220a 2020  ="-4.9780204".  
+00006d10: 2020 2020 2020 2072 783d 2233 2e31 3536         rx="3.156
+00006d20: 3232 3634 220a 2020 2020 2020 2020 2072  2264".         r
+00006d30: 793d 2233 2e31 3432 3032 3422 202f 3e0a  y="3.142024" />.
+00006d40: 2020 2020 2020 3c65 6c6c 6970 7365 0a20        <ellipse. 
+00006d50: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00006d60: 696c 6c3a 2361 3861 3961 613b 6669 6c6c  ill:#a8a9aa;fill
+00006d70: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00006d80: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00006d90: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00006da0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00006db0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00006dc0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00006dd0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+00006de0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00006df0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00006e00: 3134 3536 372d 332d 352d 362d 3022 0a20  14567-3-5-6-0". 
+00006e10: 2020 2020 2020 2020 6378 3d22 3132 312e          cx="121.
+00006e20: 3333 3731 3422 0a20 2020 2020 2020 2020  33714".         
+00006e30: 6379 3d22 3132 322e 3839 3232 3422 0a20  cy="122.89224". 
+00006e40: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00006e50: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+00006e60: 722d 783d 2232 2e33 3236 3936 3722 0a20  r-x="2.326967". 
+00006e70: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00006e80: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+00006e90: 722d 793d 222d 342e 3937 3830 3035 3922  r-y="-4.9780059"
+00006ea0: 0a20 2020 2020 2020 2020 7278 3d22 332e  .         rx="3.
+00006eb0: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
+00006ec0: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
+00006ed0: 2f3e 0a20 2020 2020 203c 656c 6c69 7073  />.      <ellips
+00006ee0: 650a 2020 2020 2020 2020 2073 7479 6c65  e.         style
+00006ef0: 3d22 6669 6c6c 3a23 6162 6161 3963 3b66  ="fill:#abaa9c;f
+00006f00: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00006f10: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00006f20: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00006f30: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+00006f40: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00006f50: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00006f60: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00006f70: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00006f80: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00006f90: 6174 6831 3435 3637 2d33 2d39 2d31 2d33  ath14567-3-9-1-3
+00006fa0: 220a 2020 2020 2020 2020 2063 783d 2231  ".         cx="1
+00006fb0: 3031 2e38 3736 3134 220a 2020 2020 2020  01.87614".      
+00006fc0: 2020 2063 793d 2231 3337 2e37 3934 3835     cy="137.79485
+00006fd0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00006fe0: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+00006ff0: 6e74 6572 2d78 3d22 322e 3332 3639 3733  nter-x="2.326973
+00007000: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00007010: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+00007020: 6e74 6572 2d79 3d22 2d34 2e39 3738 3032  nter-y="-4.97802
+00007030: 3531 220a 2020 2020 2020 2020 2072 783d  51".         rx=
+00007040: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
+00007050: 2020 2020 2072 793d 2233 2e31 3432 3032       ry="3.14202
+00007060: 3422 202f 3e0a 2020 2020 2020 3c65 6c6c  4" />.      <ell
+00007070: 6970 7365 0a20 2020 2020 2020 2020 7374  ipse.         st
+00007080: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
+00007090: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
+000070a0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000070b0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+000070c0: 3530 3035 3b73 7472 6f6b 652d 6d69 7465  5005;stroke-mite
+000070d0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+000070e0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+000070f0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+00007100: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+00007110: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
+00007120: 3d22 7061 7468 3134 3536 372d 332d 322d  ="path14567-3-2-
+00007130: 382d 3622 0a20 2020 2020 2020 2020 6378  8-6".         cx
+00007140: 3d22 3831 2e32 3932 3431 3922 0a20 2020  ="81.292419".   
+00007150: 2020 2020 2020 6379 3d22 3634 2e32 3133        cy="64.213
+00007160: 3136 3522 0a20 2020 2020 2020 2020 696e  165".         in
+00007170: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
+00007180: 2d63 656e 7465 722d 783d 2233 2e35 3931  -center-x="3.591
+00007190: 3336 3039 220a 2020 2020 2020 2020 2069  3609".         i
+000071a0: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+000071b0: 6d2d 6365 6e74 6572 2d79 3d22 2d37 2e36  m-center-y="-7.6
+000071c0: 3832 3839 3536 220a 2020 2020 2020 2020  828956".        
+000071d0: 2072 783d 2234 2e38 3731 3139 3239 220a   rx="4.8711929".
+000071e0: 2020 2020 2020 2020 2072 793d 2234 2e38           ry="4.8
+000071f0: 3439 3237 3337 2220 2f3e 0a20 2020 2020  492737" />.     
+00007200: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
+00007210: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00007220: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
+00007230: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+00007240: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00007250: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00007260: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00007270: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00007280: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00007290: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+000072a0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+000072b0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+000072c0: 7468 3134 3536 372d 322d 3739 2d31 220a  th14567-2-79-1".
+000072d0: 2020 2020 2020 2020 2063 783d 2231 3037           cx="107
+000072e0: 2e36 3737 3032 220a 2020 2020 2020 2020  .67702".        
+000072f0: 2063 793d 2236 392e 3631 3533 3536 220a   cy="69.615356".
+00007300: 2020 2020 2020 2020 2072 783d 2233 2e31           rx="3.1
+00007310: 3536 3232 3634 220a 2020 2020 2020 2020  562264".        
+00007320: 2072 793d 2233 2e31 3432 3032 3422 202f   ry="3.142024" /
+00007330: 3e0a 2020 2020 2020 3c65 6c6c 6970 7365  >.      <ellipse
+00007340: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00007350: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
+00007360: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
+00007370: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
+00007380: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00007390: 312e 3035 3030 353b 7374 726f 6b65 2d6d  1.05005;stroke-m
+000073a0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000073b0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000073c0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+000073d0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+000073e0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+000073f0: 2069 643d 2270 6174 6831 3435 3637 2d32   id="path14567-2
+00007400: 2d38 2d32 2d30 220a 2020 2020 2020 2020  -8-2-0".        
+00007410: 2063 783d 2235 332e 3033 3635 3735 220a   cx="53.036575".
+00007420: 2020 2020 2020 2020 2063 793d 2239 352e           cy="95.
+00007430: 3639 3439 3737 220a 2020 2020 2020 2020  694977".        
+00007440: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
+00007450: 2020 2020 2020 2020 2072 793d 2233 2e31           ry="3.1
+00007460: 3432 3032 3422 202f 3e0a 2020 2020 2020  42024" />.      
+00007470: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00007480: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
+00007490: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
+000074a0: 302e 3939 3834 3038 3b73 7472 6f6b 653a  0.998408;stroke:
+000074b0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+000074c0: 6964 7468 3a30 2e33 3233 3538 3870 783b  idth:0.323588px;
+000074d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+000074e0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+000074f0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00007500: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00007510: 2020 2020 2064 3d22 6d20 3331 382e 3730       d="m 318.70
+00007520: 3133 332c 3732 2e37 3031 3732 2032 362e  133,72.70172 26.
+00007530: 3630 3435 372c 2d38 2e37 3836 3833 202d  60457,-8.78683 -
+00007540: 3238 2e33 3833 3935 2c2d 312e 3437 3538  28.38395,-1.4758
+00007550: 3620 6320 3131 2e30 3035 3236 2c33 2e32  6 c 11.00526,3.2
+00007560: 3034 3636 2031 312e 3035 3533 2c33 2e33  0466 11.0553,3.3
+00007570: 3734 3237 2031 2e37 3739 3338 2c31 302e  7427 1.77938,10.
+00007580: 3236 3236 3920 7a22 0a20 2020 2020 2020  26269 z".       
+00007590: 2020 6964 3d22 7061 7468 3134 3635 372d    id="path14657-
+000075a0: 392d 302d 3622 0a20 2020 2020 2020 2020  9-0-6".         
+000075b0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+000075c0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+000075d0: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
+000075e0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+000075f0: 6363 2220 2f3e 0a20 2020 2020 203c 656c  cc" />.      <el
+00007600: 6c69 7073 650a 2020 2020 2020 2020 2073  lipse.         s
+00007610: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
+00007620: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
+00007630: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
+00007640: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00007650: 6964 7468 3a31 2e39 3935 3938 3b73 7472  idth:1.99598;str
+00007660: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00007670: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00007680: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+00007690: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+000076a0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000076b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+000076c0: 3536 372d 322d 372d 322d 3322 0a20 2020  567-2-7-2-3".   
+000076d0: 2020 2020 2020 6378 3d22 3137 372e 3437        cx="177.47
+000076e0: 3435 3622 0a20 2020 2020 2020 2020 6379  456".         cy
+000076f0: 3d22 3834 2e33 3331 3732 3622 0a20 2020  ="84.331726".   
+00007700: 2020 2020 2020 7278 3d22 352e 3939 3935        rx="5.9995
+00007710: 3232 3222 0a20 2020 2020 2020 2020 7279  222".         ry
+00007720: 3d22 352e 3937 3235 3235 3622 202f 3e0a  ="5.9725256" />.
+00007730: 2020 2020 2020 3c74 6578 740a 2020 2020        <text.    
+00007740: 2020 2020 2078 6d6c 3a73 7061 6365 3d22       xml:space="
+00007750: 7072 6573 6572 7665 220a 2020 2020 2020  preserve".      
+00007760: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
+00007770: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
+00007780: 2d77 6569 6768 743a 6e6f 726d 616c 3b66  -weight:normal;f
+00007790: 6f6e 742d 7369 7a65 3a35 2e38 3732 3931  ont-size:5.87291
+000077a0: 7078 3b6c 696e 652d 6865 6967 6874 3a31  px;line-height:1
+000077b0: 2e32 353b 666f 6e74 2d66 616d 696c 793a  .25;font-family:
+000077c0: 7361 6e73 2d73 6572 6966 3b6c 6574 7465  sans-serif;lette
+000077d0: 722d 7370 6163 696e 673a 3070 783b 776f  r-spacing:0px;wo
+000077e0: 7264 2d73 7061 6369 6e67 3a30 7078 3b66  rd-spacing:0px;f
+000077f0: 696c 6c3a 2366 6666 6666 663b 6669 6c6c  ill:#ffffff;fill
+00007800: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00007810: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
+00007820: 6474 683a 302e 3430 3034 3235 3b66 696c  dth:0.400425;fil
+00007830: 7465 723a 7572 6c28 2366 696c 7465 7231  ter:url(#filter1
+00007840: 3530 3531 2d33 2d32 2922 0a20 2020 2020  5051-3-2)".     
+00007850: 2020 2020 783d 2237 372e 3639 3438 3933      x="77.694893
+00007860: 220a 2020 2020 2020 2020 2079 3d22 3931  ".         y="91
+00007870: 2e39 3838 3434 3922 0a20 2020 2020 2020  .988449".       
+00007880: 2020 6964 3d22 7465 7874 3134 3639 312d    id="text14691-
+00007890: 362d 332d 3222 0a20 2020 2020 2020 2020  6-3-2".         
+000078a0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+000078b0: 7828 322e 3735 3131 3931 392c 302c 302c  x(2.7511919,0,0,
+000078c0: 322e 3733 3838 3132 2c2d 3735 2e39 3736  2.738812,-75.976
+000078d0: 3639 362c 2d31 3038 2e30 3838 3636 2922  696,-108.08866)"
+000078e0: 3e3c 7473 7061 6e0a 2020 2020 2020 2020  ><tspan.        
+000078f0: 2020 2073 6f64 6970 6f64 693a 726f 6c65     sodipodi:role
+00007900: 3d22 6c69 6e65 220a 2020 2020 2020 2020  ="line".        
+00007910: 2020 2069 643d 2274 7370 616e 3134 3638     id="tspan1468
+00007920: 392d 322d 372d 3022 0a20 2020 2020 2020  9-2-7-0".       
+00007930: 2020 2020 783d 2237 372e 3639 3438 3933      x="77.694893
+00007940: 220a 2020 2020 2020 2020 2020 2079 3d22  ".           y="
+00007950: 3931 2e39 3838 3434 3922 0a20 2020 2020  91.988449".     
+00007960: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
+00007970: 742d 7374 796c 653a 6e6f 726d 616c 3b66  t-style:normal;f
+00007980: 6f6e 742d 7661 7269 616e 743a 6e6f 726d  ont-variant:norm
+00007990: 616c 3b66 6f6e 742d 7765 6967 6874 3a6e  al;font-weight:n
+000079a0: 6f72 6d61 6c3b 666f 6e74 2d73 7472 6574  ormal;font-stret
+000079b0: 6368 3a6e 6f72 6d61 6c3b 666f 6e74 2d73  ch:normal;font-s
+000079c0: 697a 653a 3231 2e33 3536 7078 3b66 6f6e  ize:21.356px;fon
+000079d0: 742d 6661 6d69 6c79 3a49 6d70 6163 743b  t-family:Impact;
+000079e0: 2d69 6e6b 7363 6170 652d 666f 6e74 2d73  -inkscape-font-s
+000079f0: 7065 6369 6669 6361 7469 6f6e 3a49 6d70  pecification:Imp
+00007a00: 6163 743b 6669 6c6c 3a23 6666 6666 6666  act;fill:#ffffff
+00007a10: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00007a20: 7374 726f 6b65 2d77 6964 7468 3a30 2e34  stroke-width:0.4
+00007a30: 3030 3432 3522 3e53 6165 6e6f 7079 3c2f  00425">Saenopy</
+00007a40: 7473 7061 6e3e 3c2f 7465 7874 3e0a 2020  tspan></text>.  
+00007a50: 2020 2020 3c74 6578 740a 2020 2020 2020      <text.      
+00007a60: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
+00007a70: 6573 6572 7665 220a 2020 2020 2020 2020  eserve".        
+00007a80: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
+00007a90: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
+00007aa0: 6569 6768 743a 6e6f 726d 616c 3b66 6f6e  eight:normal;fon
+00007ab0: 742d 7369 7a65 3a31 362e 3132 3131 7078  t-size:16.1211px
+00007ac0: 3b6c 696e 652d 6865 6967 6874 3a31 2e32  ;line-height:1.2
+00007ad0: 353b 666f 6e74 2d66 616d 696c 793a 7361  5;font-family:sa
+00007ae0: 6e73 2d73 6572 6966 3b6c 6574 7465 722d  ns-serif;letter-
+00007af0: 7370 6163 696e 673a 3070 783b 776f 7264  spacing:0px;word
+00007b00: 2d73 7061 6369 6e67 3a30 7078 3b66 696c  -spacing:0px;fil
+00007b10: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
+00007b20: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00007b30: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
+00007b40: 683a 312e 3039 3931 3722 0a20 2020 2020  h:1.09917".     
+00007b50: 2020 2020 783d 2231 3335 2e34 3739 3036      x="135.47906
+00007b60: 220a 2020 2020 2020 2020 2079 3d22 3133  ".         y="13
+00007b70: 362e 3338 3737 220a 2020 2020 2020 2020  6.3877".        
+00007b80: 2069 643d 2274 6578 7431 3436 3931 2d35   id="text14691-5
+00007b90: 2d36 220a 2020 2020 2020 2020 2074 7261  -6".         tra
+00007ba0: 6e73 666f 726d 3d22 7363 616c 6528 312e  nsform="scale(1.
+00007bb0: 3030 3232 3537 352c 302e 3939 3737 3437  0022575,0.997747
+00007bc0: 3538 2922 3e3c 7473 7061 6e0a 2020 2020  58)"><tspan.    
+00007bd0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00007be0: 726f 6c65 3d22 6c69 6e65 220a 2020 2020  role="line".    
+00007bf0: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
+00007c00: 3134 3638 392d 392d 3122 0a20 2020 2020  14689-9-1".     
+00007c10: 2020 2020 2020 783d 2231 3335 2e34 3739        x="135.479
+00007c20: 3036 220a 2020 2020 2020 2020 2020 2079  06".           y
+00007c30: 3d22 3133 362e 3338 3737 220a 2020 2020  ="136.3877".    
+00007c40: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
+00007c50: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
+00007c60: 666f 6e74 2d76 6172 6961 6e74 3a6e 6f72  font-variant:nor
+00007c70: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
+00007c80: 6e6f 726d 616c 3b66 6f6e 742d 7374 7265  normal;font-stre
+00007c90: 7463 683a 6e6f 726d 616c 3b66 6f6e 742d  tch:normal;font-
+00007ca0: 7369 7a65 3a35 382e 3632 3231 7078 3b66  size:58.6221px;f
+00007cb0: 6f6e 742d 6661 6d69 6c79 3a27 546c 7767  ont-family:'Tlwg
+00007cc0: 2054 7970 6973 7427 3b2d 696e 6b73 6361   Typist';-inksca
+00007cd0: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
+00007ce0: 6174 696f 6e3a 2754 6c77 6720 5479 7069  ation:'Tlwg Typi
+00007cf0: 7374 273b 7374 726f 6b65 2d77 6964 7468  st';stroke-width
+00007d00: 3a31 2e30 3939 3137 223e 5361 656e 6f70  :1.09917">Saenop
+00007d10: 793c 2f74 7370 616e 3e3c 2f74 6578 743e  y</tspan></text>
+00007d20: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
+00007d30: 0a20 2020 2020 2020 6964 3d22 6739 3034  .       id="g904
+00007d40: 220a 2020 2020 2020 2074 7261 6e73 666f  ".       transfo
+00007d50: 726d 3d22 6d61 7472 6978 2832 2e36 3837  rm="matrix(2.687
+00007d60: 3937 3433 2c30 2c30 2c32 2e36 3837 3937  9743,0,0,2.68797
+00007d70: 3433 2c2d 352e 3030 3430 3331 352c 2d39  43,-5.0040315,-9
+00007d80: 392e 3932 3838 3935 2922 3e0a 2020 2020  9.928895)">.    
+00007d90: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00007da0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3365   style="fill:#3e
+00007db0: 3462 3737 3b66 696c 6c2d 6f70 6163 6974  4b77;fill-opacit
+00007dc0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00007dd0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00007de0: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
+00007df0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00007e00: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00007e10: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+00007e20: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00007e30: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00007e40: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00007e50: 2020 2020 2020 2020 643d 226d 2035 2e37          d="m 5.7
+00007e60: 3538 3439 3036 2c31 3631 2e38 3336 3531  584906,161.83651
+00007e70: 2033 322e 3333 3936 3230 342c 2d31 2e34   32.3396204,-1.4
+00007e80: 3639 3938 2032 312e 3234 3739 332c 2d32  6998 21.24793,-2
+00007e90: 332e 3635 3333 3520 6320 2d32 362e 3736  3.65335 c -26.76
+00007ea0: 3738 392c 3138 2e30 3031 3837 202d 3339  789,18.00187 -39
+00007eb0: 2e35 3536 3434 2c32 302e 3839 3039 3520  .55644,20.89095 
+00007ec0: 2d35 332e 3538 3735 3530 342c 3235 2e31  -53.5875504,25.1
+00007ed0: 3233 3333 207a 220a 2020 2020 2020 2020  2333 z".        
+00007ee0: 2069 643d 2270 6174 6831 3435 3437 2d31   id="path14547-1
+00007ef0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00007f00: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00007f10: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00007f20: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00007f30: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
+00007f40: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00007f50: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00007f60: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+00007f70: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00007f80: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
+00007f90: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00007fa0: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
+00007fb0: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
+00007fc0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00007fd0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00007fe0: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
+00007ff0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00008000: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00008010: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00008020: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00008030: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00008040: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00008050: 2020 2020 2020 643d 226d 2033 382e 3039        d="m 38.09
+00008060: 3831 3131 2c31 3630 2e33 3636 3533 2031  8111,160.36653 1
+00008070: 342e 3033 3136 352c 332e 3230 3732 3420  4.03165,3.20724 
+00008080: 372e 3231 3632 382c 2d32 362e 3836 3035  7.21628,-26.8605
+00008090: 3920 7a22 0a20 2020 2020 2020 2020 6964  9 z".         id
+000080a0: 3d22 7061 7468 3134 3534 392d 3122 0a20  ="path14549-1". 
+000080b0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+000080c0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+000080d0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+000080e0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+000080f0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+00008100: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00008110: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00008120: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00008130: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00008140: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
+00008150: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00008160: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00008170: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
+00008180: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00008190: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000081a0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+000081b0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+000081c0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+000081d0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+000081e0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+000081f0: 643d 226d 2035 322e 3132 3937 3631 2c31  d="m 52.129761,1
+00008200: 3633 2e35 3733 3737 2033 372e 3535 3133  63.57377 37.5513
+00008210: 372c 362e 3638 3137 3420 6320 2d31 342e  7,6.68174 c -14.
+00008220: 3633 3331 322c 2d37 2e37 3335 3839 202d  63312,-7.73589 -
+00008230: 3233 2e31 3036 3934 2c2d 3230 2e31 3634  23.10694,-20.164
+00008240: 3536 202d 3330 2e33 3335 3039 2c2d 3333  56 -30.33509,-33
+00008250: 2e35 3432 3333 207a 220a 2020 2020 2020  .54233 z".      
+00008260: 2020 2069 643d 2270 6174 6831 3435 3531     id="path14551
+00008270: 2d30 220a 2020 2020 2020 2020 2069 6e6b  -0".         ink
+00008280: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00008290: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+000082a0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000082b0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+000082c0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+000082d0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+000082e0: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
+000082f0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+00008300: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+00008310: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00008320: 2073 7479 6c65 3d22 6669 6c6c 3a23 3237   style="fill:#27
+00008330: 3337 3733 3b66 696c 6c2d 6f70 6163 6974  3773;fill-opacit
+00008340: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00008350: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00008360: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
+00008370: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00008380: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00008390: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+000083a0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000083b0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+000083c0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+000083d0: 2020 2020 2020 2020 643d 226d 2035 2e37          d="m 5.7
+000083e0: 3538 3439 3036 2c31 3631 2e38 3336 3531  584906,161.83651
+000083f0: 2063 2037 2e31 3136 3432 3034 2c34 2e30   c 7.1164204,4.0
+00008400: 3832 3434 2031 342e 3936 3237 3230 342c  8244 14.9627204,
+00008410: 372e 3630 3334 3320 3137 2e36 3339 3739  7.60343 17.63979
+00008420: 3034 2c31 352e 3130 3037 3420 6c20 3134  04,15.10074 l 14
+00008430: 2e36 3939 3833 2c2d 3136 2e35 3730 3732  .69983,-16.57072
+00008440: 207a 220a 2020 2020 2020 2020 2069 643d   z".         id=
+00008450: 2270 6174 6831 3435 3533 2d33 220a 2020  "path14553-3".  
+00008460: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00008470: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00008480: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+00008490: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+000084a0: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
+000084b0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+000084c0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+000084d0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+000084e0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+000084f0: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
+00008500: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00008510: 3d22 6669 6c6c 3a23 3134 3236 3732 3b66  ="fill:#142672;f
+00008520: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00008530: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00008540: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
+00008550: 3235 3b73 7472 6f6b 652d 6c69 6e65 6361  25;stroke-lineca
+00008560: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00008570: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00008580: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00008590: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+000085a0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+000085b0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+000085c0: 2020 643d 226d 2032 332e 3339 3832 3831    d="m 23.398281
+000085d0: 2c31 3736 2e39 3337 3235 2036 362e 3238  ,176.93725 66.28
+000085e0: 3238 352c 2d36 2e36 3831 3734 202d 3531  285,-6.68174 -51
+000085f0: 2e35 3833 3032 2c2d 392e 3838 3839 3820  .58302,-9.88898 
+00008600: 7a22 0a20 2020 2020 2020 2020 6964 3d22  z".         id="
+00008610: 7061 7468 3134 3535 352d 3422 0a20 2020  path14555-4".   
+00008620: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00008630: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00008640: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
+00008650: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00008660: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+00008670: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00008680: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+00008690: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+000086a0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+000086b0: 6c6c 3a23 3534 3636 3863 3b66 696c 6c2d  ll:#54668c;fill-
+000086c0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+000086d0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+000086e0: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
+000086f0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00008700: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00008710: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00008720: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00008730: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00008740: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00008750: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+00008760: 226d 2032 332e 3339 3832 3831 2c31 3736  "m 23.398281,176
+00008770: 2e39 3337 3235 2033 382e 3231 3935 352c  .93725 38.21955,
+00008780: 342e 3030 3930 3420 3238 2e30 3633 332c  4.00904 28.0633,
+00008790: 2d31 302e 3639 3037 3820 7a22 0a20 2020  -10.69078 z".   
+000087a0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+000087b0: 3535 372d 3022 0a20 2020 2020 2020 2020  557-0".         
+000087c0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+000087d0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+000087e0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+000087f0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+00008800: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
+00008810: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+00008820: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+00008830: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00008840: 2073 7479 6c65 3d22 6669 6c6c 3a23 3232   style="fill:#22
+00008850: 3334 3765 3b66 696c 6c2d 6f70 6163 6974  347e;fill-opacit
+00008860: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00008870: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00008880: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
+00008890: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+000088a0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+000088b0: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+000088c0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000088d0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+000088e0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+000088f0: 2020 2020 2020 2020 643d 226d 2032 332e          d="m 23.
+00008900: 3339 3832 3831 2c31 3736 2e39 3337 3235  398281,176.93725
+00008910: 2063 2030 2e38 3539 3432 2c37 2e34 3130   c 0.85942,7.410
+00008920: 3134 202d 322e 3131 3533 372c 3132 2e30  14 -2.11537,12.0
+00008930: 3831 3537 202d 332e 3437 3435 2c31 372e  8157 -3.4745,17.
+00008940: 3930 3730 3520 6c20 3431 2e36 3934 3035  90705 l 41.69405
+00008950: 2c2d 3133 2e38 3938 3031 207a 220a 2020  ,-13.89801 z".  
+00008960: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00008970: 3435 3539 2d33 220a 2020 2020 2020 2020  4559-3".        
+00008980: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+00008990: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+000089a0: 220a 2020 2020 2020 2020 2073 6f64 6970  ".         sodip
+000089b0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+000089c0: 6363 6322 0a20 2020 2020 2020 2020 696e  ccc".         in
+000089d0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+000089e0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+000089f0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00008a00: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+00008a10: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00008a20: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00008a30: 3a23 3038 3130 3639 3b66 696c 6c2d 6f70  :#081069;fill-op
+00008a40: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00008a50: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00008a60: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
+00008a70: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00008a80: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00008a90: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+00008aa0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00008ab0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00008ac0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00008ad0: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
+00008ae0: 2031 392e 3932 3337 3831 2c31 3934 2e38   19.923781,194.8
+00008af0: 3434 3320 3238 2e38 3635 3131 2c34 2e32  443 28.86511,4.2
+00008b00: 3736 3332 2034 302e 3839 3232 342c 2d32  7632 40.89224,-2
+00008b10: 382e 3836 3531 3120 7a22 0a20 2020 2020  8.86511 z".     
+00008b20: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00008b30: 312d 3922 0a20 2020 2020 2020 2020 696e  1-9".         in
+00008b40: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00008b50: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
 00008b60: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00008b70: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00008b80: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
-00008b90: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00008ba0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00008bb0: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00008bc0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008bd0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008be0: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00008bf0: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-00008c00: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00008c10: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-00008c20: 2361 6261 6139 633b 6669 6c6c 2d6f 7061  #abaa9c;fill-opa
-00008c30: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00008c40: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00008c50: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-00008c60: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00008c70: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00008c80: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-00008c90: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00008ca0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00008cb0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00008cc0: 3637 2d33 2d39 2d30 2d39 2d38 220a 2020  67-3-9-0-9-8".  
-00008cd0: 2020 2020 2020 2063 783d 2234 392e 3139         cx="49.19
-00008ce0: 3436 3439 220a 2020 2020 2020 2020 2063  4649".         c
-00008cf0: 793d 2231 3939 2e30 3333 3238 220a 2020  y="199.03328".  
-00008d00: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00008d10: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00008d20: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
-00008d30: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00008d40: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00008d50: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
-00008d60: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00008d70: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00008d80: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00008d90: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008da0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008db0: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00008dc0: 2020 2072 3d22 322e 3537 3137 3531 3122     r="2.5717511"
-00008dd0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00008de0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-00008df0: 2331 3132 3036 363b 6669 6c6c 2d6f 7061  #112066;fill-opa
-00008e00: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00008e10: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00008e20: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-00008e30: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00008e40: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00008e50: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-00008e60: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00008e70: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00008e80: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00008e90: 3637 2d33 2d32 2d35 2d34 2d33 220a 2020  67-3-2-5-4-3".  
-00008ea0: 2020 2020 2020 2063 783d 2233 382e 3332         cx="38.32
-00008eb0: 3734 3436 220a 2020 2020 2020 2020 2063  7446".         c
-00008ec0: 793d 2231 3630 2e30 3130 3138 220a 2020  y="160.01018".  
-00008ed0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00008ee0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00008ef0: 2d78 3d22 372e 3136 3632 3131 3622 0a20  -x="7.1662116". 
-00008f00: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00008f10: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00008f20: 722d 793d 222d 3135 2e33 3939 3735 3122  r-y="-15.399751"
-00008f30: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00008f40: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00008f50: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00008f60: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008f70: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008f80: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00008f90: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-00008fa0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00008fb0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-00008fc0: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
-00008fd0: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
-00008fe0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00008ff0: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
-00009000: 3235 3b73 7472 6f6b 652d 6d69 7465 726c  25;stroke-miterl
-00009010: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00009020: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00009030: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-00009040: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00009050: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
-00009060: 7061 7468 3134 3536 372d 322d 362d 302d  path14567-2-6-0-
-00009070: 3022 0a20 2020 2020 2020 2020 6378 3d22  0".         cx="
-00009080: 3532 2e32 3537 3232 3522 0a20 2020 2020  52.257225".     
-00009090: 2020 2020 6379 3d22 3136 322e 3837 3531      cy="162.8751
-000090a0: 3722 0a20 2020 2020 2020 2020 696e 6b73  7".         inks
-000090b0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-000090c0: 3d22 3330 3022 0a20 2020 2020 2020 2020  ="300".         
-000090d0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-000090e0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-000090f0: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-00009100: 2020 2020 2072 3d22 312e 3636 3633 3332       r="1.666332
-00009110: 3822 0a20 2020 2020 2020 2020 7374 796c  8".         styl
-00009120: 653d 226f 7061 6369 7479 3a31 3b66 696c  e="opacity:1;fil
-00009130: 6c3a 2365 6466 3066 633b 6669 6c6c 2d6f  l:#edf0fc;fill-o
-00009140: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
-00009150: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00009160: 7472 6f6b 652d 7769 6474 683a 302e 3535  troke-width:0.55
-00009170: 3536 3235 3b73 7472 6f6b 652d 6d69 7465  5625;stroke-mite
-00009180: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00009190: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-000091a0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-000091b0: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-000091c0: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
-000091d0: 3d22 7061 7468 3134 3536 372d 322d 382d  ="path14567-2-8-
-000091e0: 362d 372d 3822 0a20 2020 2020 2020 2020  6-7-8".         
-000091f0: 6378 3d22 3233 2e34 3039 3735 3222 0a20  cx="23.409752". 
-00009200: 2020 2020 2020 2020 6379 3d22 3137 362e          cy="176.
-00009210: 3730 3631 3522 0a20 2020 2020 2020 2020  70615".         
-00009220: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00009230: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-00009240: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00009250: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-00009260: 3e0a 2020 2020 2020 3c63 6972 636c 650a  >.      <circle.
-00009270: 2020 2020 2020 2020 2072 3d22 332e 3136           r="3.16
-00009280: 3734 3533 3822 0a20 2020 2020 2020 2020  74538".         
-00009290: 7374 796c 653d 226f 7061 6369 7479 3a31  style="opacity:1
-000092a0: 3b66 696c 6c3a 2365 6466 3066 633b 6669  ;fill:#edf0fc;fi
-000092b0: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
-000092c0: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
-000092d0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-000092e0: 312e 3035 3631 363b 7374 726f 6b65 2d6d  1.05616;stroke-m
-000092f0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00009300: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00009310: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-00009320: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-00009330: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-00009340: 2069 643d 2270 6174 6831 3435 3637 2d32   id="path14567-2
-00009350: 2d37 2d30 2d39 2d30 220a 2020 2020 2020  -7-0-9-0".      
-00009360: 2020 2063 783d 2238 392e 3130 3638 3935     cx="89.106895
-00009370: 220a 2020 2020 2020 2020 2063 793d 2231  ".         cy="1
-00009380: 3730 2e36 3739 3739 220a 2020 2020 2020  70.67979".      
-00009390: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-000093a0: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
-000093b0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000093c0: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-000093d0: 2220 2f3e 0a20 2020 203c 2f67 3e0a 2020  " />.    </g>.  
-000093e0: 2020 3c72 6563 740a 2020 2020 2020 2073    <rect.       s
-000093f0: 7479 6c65 3d22 6669 6c6c 3a23 6233 6233  tyle="fill:#b3b3
-00009400: 6233 3b66 696c 6c2d 6f70 6163 6974 793a  b3;fill-opacity:
-00009410: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
-00009420: 726f 6b65 2d77 6964 7468 3a30 2e31 3332  roke-width:0.132
-00009430: 3239 323b 7374 726f 6b65 2d6d 6974 6572  292;stroke-miter
-00009440: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00009450: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00009460: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-00009470: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-00009480: 3a31 220a 2020 2020 2020 2069 643d 2272  :1".       id="r
-00009490: 6563 7431 3530 3734 2d30 2d39 2d32 2d39  ect15074-0-9-2-9
-000094a0: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
-000094b0: 382e 3436 3636 3636 3222 0a20 2020 2020  8.4666662".     
-000094c0: 2020 6865 6967 6874 3d22 382e 3436 3636    height="8.4666
-000094d0: 3636 3222 0a20 2020 2020 2020 783d 2231  662".       x="1
-000094e0: 3532 2e32 3738 3939 220a 2020 2020 2020  52.27899".      
-000094f0: 2079 3d22 3133 312e 3630 3636 3622 0a20   y="131.60666". 
-00009500: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00009510: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00009520: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00009530: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00009540: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-00009550: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00009560: 6c6c 3a23 3365 3462 3737 3b66 696c 6c2d  ll:#3e4b77;fill-
-00009570: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00009580: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00009590: 7769 6474 683a 302e 3133 3232 3932 3b73  width:0.132292;s
-000095a0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-000095b0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-000095c0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-000095d0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-000095e0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-000095f0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00009600: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00009610: 2031 3532 2e36 3336 3032 2c31 3334 2e34   152.63602,134.4
-00009620: 3036 3032 2032 2e38 3734 3937 2c2d 302e  0602 2.87497,-0.
-00009630: 3133 3036 3820 312e 3838 3839 322c 2d32  13068 1.88892,-2
-00009640: 2e31 3032 3736 2063 202d 322e 3337 3936  .10276 c -2.3796
-00009650: 342c 312e 3630 3033 3520 2d33 2e35 3136  4,1.60035 -3.516
-00009660: 3533 2c31 2e38 3537 3138 202d 342e 3736  53,1.85718 -4.76
-00009670: 3338 392c 322e 3233 3334 3420 7a22 0a20  389,2.23344 z". 
-00009680: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00009690: 3534 372d 312d 372d 382d 3522 0a20 2020  547-1-7-8-5".   
-000096a0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-000096b0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-000096c0: 3d22 3022 0a20 2020 2020 2020 736f 6469  ="0".       sodi
-000096d0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-000096e0: 6363 6363 220a 2020 2020 2020 2069 6e6b  cccc".       ink
-000096f0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00009700: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-00009710: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-00009720: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-00009730: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00009740: 796c 653d 2266 696c 6c3a 2331 6332 6336  yle="fill:#1c2c6
-00009750: 383b 6669 6c6c 2d6f 7061 6369 7479 3a31  8;fill-opacity:1
-00009760: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-00009770: 7374 726f 6b65 2d77 6964 7468 3a30 2e31  stroke-width:0.1
-00009780: 3332 3239 323b 7374 726f 6b65 2d6c 696e  32292;stroke-lin
-00009790: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-000097a0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-000097b0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-000097c0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-000097d0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-000097e0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-000097f0: 2020 2064 3d22 6d20 3135 352e 3531 3039     d="m 155.5109
-00009800: 392c 3133 342e 3237 3533 3420 312e 3234  9,134.27534 1.24
-00009810: 3734 2c30 2e32 3835 3132 2030 2e36 3431  74,0.28512 0.641
-00009820: 3532 2c2d 322e 3338 3738 3820 7a22 0a20  52,-2.38788 z". 
-00009830: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00009840: 3534 392d 312d 302d 312d 3122 0a20 2020  549-1-0-1-1".   
-00009850: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-00009860: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-00009870: 3d22 3022 0a20 2020 2020 2020 696e 6b73  ="0".       inks
-00009880: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-00009890: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
-000098a0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-000098b0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-000098c0: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-000098d0: 6c65 3d22 6669 6c6c 3a23 3036 3035 3038  le="fill:#060508
-000098e0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-000098f0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00009900: 7472 6f6b 652d 7769 6474 683a 302e 3133  troke-width:0.13
-00009910: 3232 3932 3b73 7472 6f6b 652d 6c69 6e65  2292;stroke-line
-00009920: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00009930: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00009940: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00009950: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00009960: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00009970: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00009980: 2020 643d 226d 2031 3536 2e37 3538 3339    d="m 156.75839
-00009990: 2c31 3334 2e35 3630 3436 2033 2e33 3338  ,134.56046 3.338
-000099a0: 3239 2c30 2e35 3934 2063 202d 312e 3330  29,0.594 c -1.30
-000099b0: 3038 382c 2d30 2e36 3837 3731 202d 322e  088,-0.68771 -2.
-000099c0: 3035 3431 392c 2d31 2e37 3932 3631 202d  05419,-1.79261 -
-000099d0: 322e 3639 3637 372c 2d32 2e39 3831 3838  2.69677,-2.98188
-000099e0: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-000099f0: 6174 6831 3435 3531 2d30 2d33 2d39 2d39  ath14551-0-3-9-9
-00009a00: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00009a10: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00009a20: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-00009a30: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00009a40: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
-00009a50: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00009a60: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-00009a70: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00009a80: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-00009a90: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
-00009aa0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00009ab0: 3237 3337 3733 3b66 696c 6c2d 6f70 6163  273773;fill-opac
-00009ac0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-00009ad0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-00009ae0: 683a 302e 3133 3232 3932 3b73 7472 6f6b  h:0.132292;strok
-00009af0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00009b00: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00009b10: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00009b20: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00009b30: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00009b40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00009b50: 0a20 2020 2020 2020 643d 226d 2031 3532  .       d="m 152
-00009b60: 2e36 3336 3032 2c31 3334 2e34 3036 3032  .63602,134.40602
-00009b70: 2063 2030 2e36 3332 3635 2c30 2e33 3632   c 0.63265,0.362
-00009b80: 3932 2031 2e33 3330 3138 2c30 2e36 3735  92 1.33018,0.675
-00009b90: 3934 2031 2e35 3638 3137 2c31 2e33 3432  94 1.56817,1.342
-00009ba0: 3434 206c 2031 2e33 3036 382c 2d31 2e34  44 l 1.3068,-1.4
-00009bb0: 3733 3132 207a 220a 2020 2020 2020 2069  7312 z".       i
-00009bc0: 643d 2270 6174 6831 3435 3533 2d33 2d32  d="path14553-3-2
-00009bd0: 2d32 2d31 220a 2020 2020 2020 2069 6e6b  -2-1".       ink
-00009be0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-00009bf0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-00009c00: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00009c10: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
-00009c20: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00009c30: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00009c40: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00009c50: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00009c60: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-00009c70: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00009c80: 6c6c 3a23 3134 3236 3732 3b66 696c 6c2d  ll:#142672;fill-
-00009c90: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00009ca0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00009cb0: 7769 6474 683a 302e 3133 3232 3932 3b73  width:0.132292;s
-00009cc0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00009cd0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00009ce0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00009cf0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00009d00: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00009d10: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00009d20: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00009d30: 2031 3534 2e32 3034 3139 2c31 3335 2e37   154.20419,135.7
-00009d40: 3438 3436 2035 2e38 3932 3439 2c2d 302e  4846 5.89249,-0.
-00009d50: 3539 3420 2d34 2e35 3835 3639 2c2d 302e  594 -4.58569,-0.
-00009d60: 3837 3931 3220 7a22 0a20 2020 2020 2020  87912 z".       
-00009d70: 6964 3d22 7061 7468 3134 3535 352d 342d  id="path14555-4-
-00009d80: 312d 362d 3722 0a20 2020 2020 2020 696e  1-6-7".       in
-00009d90: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00009da0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00009db0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00009dc0: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00009dd0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00009de0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00009df0: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-00009e00: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00009e10: 6c6c 3a23 3534 3636 3863 3b66 696c 6c2d  ll:#54668c;fill-
-00009e20: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00009e30: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00009e40: 7769 6474 683a 302e 3133 3232 3932 3b73  width:0.132292;s
-00009e50: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00009e60: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00009e70: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00009e80: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00009e90: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00009ea0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00009eb0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00009ec0: 2031 3534 2e32 3034 3139 2c31 3335 2e37   154.20419,135.7
-00009ed0: 3438 3436 2033 2e33 3937 3638 2c30 2e33  4846 3.39768,0.3
-00009ee0: 3536 3420 322e 3439 3438 312c 2d30 2e39  564 2.49481,-0.9
-00009ef0: 3530 3420 7a22 0a20 2020 2020 2020 6964  504 z".       id
-00009f00: 3d22 7061 7468 3134 3535 372d 302d 372d  ="path14557-0-7-
-00009f10: 332d 3922 0a20 2020 2020 2020 696e 6b73  3-9".       inks
-00009f20: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00009f30: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-00009f40: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00009f50: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00009f60: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00009f70: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00009f80: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-00009f90: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00009fa0: 3a23 3232 3334 3765 3b66 696c 6c2d 6f70  :#22347e;fill-op
-00009fb0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00009fc0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00009fd0: 6474 683a 302e 3133 3232 3932 3b73 7472  dth:0.132292;str
-00009fe0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00009ff0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000a000: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000a010: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000a020: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000a030: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000a040: 3122 0a20 2020 2020 2020 643d 226d 2031  1".       d="m 1
-0000a050: 3534 2e32 3034 3139 2c31 3335 2e37 3438  54.20419,135.748
-0000a060: 3436 2063 2030 2e30 3736 342c 302e 3635  46 c 0.0764,0.65
-0000a070: 3837 3620 2d30 2e31 3838 3036 2c31 2e30  876 -0.18806,1.0
-0000a080: 3734 3034 202d 302e 3330 3838 382c 312e  7404 -0.30888,1.
-0000a090: 3539 3139 3220 6c20 332e 3730 3635 362c  59192 l 3.70656,
-0000a0a0: 2d31 2e32 3335 3532 207a 220a 2020 2020  -1.23552 z".    
-0000a0b0: 2020 2069 643d 2270 6174 6831 3435 3539     id="path14559
-0000a0c0: 2d33 2d34 2d32 2d34 220a 2020 2020 2020  -3-4-2-4".      
-0000a0d0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-0000a0e0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-0000a0f0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
-0000a100: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-0000a110: 6322 0a20 2020 2020 2020 696e 6b73 6361  c".       inksca
-0000a120: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000a130: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000a140: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000a150: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-0000a160: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-0000a170: 3d22 6669 6c6c 3a23 3038 3130 3639 3b66  ="fill:#081069;f
-0000a180: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000a190: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000a1a0: 6f6b 652d 7769 6474 683a 302e 3133 3232  oke-width:0.1322
-0000a1b0: 3932 3b73 7472 6f6b 652d 6c69 6e65 6361  92;stroke-lineca
-0000a1c0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-0000a1d0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-0000a1e0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000a1f0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000a200: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-0000a210: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000a220: 643d 226d 2031 3533 2e38 3935 3331 2c31  d="m 153.89531,1
-0000a230: 3337 2e33 3430 3338 2032 2e35 3636 3038  37.34038 2.56608
-0000a240: 2c30 2e33 3830 3136 2033 2e36 3335 3239  ,0.38016 3.63529
-0000a250: 2c2d 322e 3536 3630 3820 7a22 0a20 2020  ,-2.56608 z".   
-0000a260: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-0000a270: 312d 392d 322d 322d 3822 0a20 2020 2020  1-9-2-2-8".     
-0000a280: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000a290: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000a2a0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000a2b0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000a2c0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000a2d0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000a2e0: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-0000a2f0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-0000a300: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
-0000a310: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000a320: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000a330: 6f6b 652d 7769 6474 683a 302e 3133 3232  oke-width:0.1322
-0000a340: 3932 3b73 7472 6f6b 652d 6c69 6e65 6361  92;stroke-lineca
-0000a350: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-0000a360: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-0000a370: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000a380: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000a390: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-0000a3a0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000a3b0: 643d 226d 2031 3536 2e34 3631 3339 2c31  d="m 156.46139,1
-0000a3c0: 3337 2e37 3230 3534 2031 2e35 3038 3736  37.72054 1.50876
-0000a3d0: 2c31 2e39 3833 3937 202d 302e 3535 3833  ,1.98397 -0.5583
-0000a3e0: 362c 2d32 2e36 3733 3031 207a 220a 2020  6,-2.67301 z".  
-0000a3f0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000a400: 3633 2d31 2d30 2d36 2d38 220a 2020 2020  63-1-0-6-8".    
-0000a410: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-0000a420: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-0000a430: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
-0000a440: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000a450: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000a460: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000a470: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000a480: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000a490: 653d 2266 696c 6c3a 2332 3833 6438 373b  e="fill:#283d87;
-0000a4a0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000a4b0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000a4c0: 726f 6b65 2d77 6964 7468 3a30 2e31 3332  roke-width:0.132
-0000a4d0: 3239 323b 7374 726f 6b65 2d6c 696e 6563  292;stroke-linec
-0000a4e0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000a4f0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000a500: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000a510: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000a520: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000a530: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000a540: 2064 3d22 6d20 3135 372e 3431 3137 392c   d="m 157.41179,
-0000a550: 3133 372e 3033 3135 2030 2e35 3538 3336  137.0315 0.55836
-0000a560: 2c32 2e36 3733 3031 2063 2030 2e32 3839  ,2.67301 c 0.289
-0000a570: 3035 2c2d 322e 3430 3239 3120 312e 3330  05,-2.40291 1.30
-0000a580: 3632 362c 2d33 2e32 3638 3631 2032 2e31  626,-3.26861 2.1
-0000a590: 3236 3533 2c2d 342e 3535 3030 3520 7a22  2653,-4.55005 z"
-0000a5a0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000a5b0: 3134 3536 352d 392d 352d 392d 3722 0a20  14565-9-5-9-7". 
-0000a5c0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-0000a5d0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-0000a5e0: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-0000a5f0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-0000a600: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
-0000a610: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-0000a620: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-0000a630: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000a640: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-0000a650: 2020 203c 656c 6c69 7073 650a 2020 2020     <ellipse.    
-0000a660: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000a670: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
-0000a680: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
-0000a690: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000a6a0: 6b65 2d77 6964 7468 3a30 2e31 3332 3239  ke-width:0.13229
-0000a6b0: 323b 7374 726f 6b65 2d6d 6974 6572 6c69  2;stroke-miterli
-0000a6c0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-0000a6d0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-0000a6e0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-0000a6f0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000a700: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-0000a710: 6831 3435 3637 2d36 2d31 2d39 2d37 220a  h14567-6-1-9-7".
-0000a720: 2020 2020 2020 2063 783d 2231 3532 2e36         cx="152.6
-0000a730: 3937 3034 220a 2020 2020 2020 2063 793d  9704".       cy=
-0000a740: 2231 3334 2e34 3039 3037 220a 2020 2020  "134.40907".    
-0000a750: 2020 2072 783d 2230 2e31 3438 3133 3535     rx="0.1481355
-0000a760: 3622 0a20 2020 2020 2020 7279 3d22 302e  6".       ry="0.
-0000a770: 3134 3831 3335 3537 220a 2020 2020 2020  14813557".      
-0000a780: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000a790: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-0000a7a0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000a7b0: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-0000a7c0: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
-0000a7d0: 2020 2020 723d 2230 2e31 3438 3133 3535      r="0.1481355
-0000a7e0: 3722 0a20 2020 2020 2020 7374 796c 653d  7".       style=
-0000a7f0: 2266 696c 6c3a 2332 3533 6137 643b 6669  "fill:#253a7d;fi
-0000a800: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-0000a810: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000a820: 6b65 2d77 6964 7468 3a30 2e31 3332 3239  ke-width:0.13229
-0000a830: 323b 7374 726f 6b65 2d6d 6974 6572 6c69  2;stroke-miterli
-0000a840: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-0000a850: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-0000a860: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-0000a870: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000a880: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-0000a890: 6831 3435 3637 2d33 2d39 332d 312d 362d  h14567-3-93-1-6-
-0000a8a0: 3922 0a20 2020 2020 2020 6378 3d22 3135  9".       cx="15
-0000a8b0: 332e 3837 3134 3822 0a20 2020 2020 2020  3.87148".       
-0000a8c0: 6379 3d22 3133 372e 3330 3837 3822 0a20  cy="137.30878". 
-0000a8d0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-0000a8e0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-0000a8f0: 783d 2234 2e36 3433 3235 3636 220a 2020  x="4.6432566".  
-0000a900: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-0000a910: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-0000a920: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
-0000a930: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000a940: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000a950: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000a960: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-0000a970: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
-0000a980: 0a20 2020 2020 2020 723d 2230 2e31 3438  .       r="0.148
-0000a990: 3133 3535 3722 0a20 2020 2020 2020 7374  13557".       st
-0000a9a0: 796c 653d 2266 696c 6c3a 2332 3533 6137  yle="fill:#253a7
-0000a9b0: 643b 6669 6c6c 2d6f 7061 6369 7479 3a31  d;fill-opacity:1
-0000a9c0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000a9d0: 7374 726f 6b65 2d77 6964 7468 3a30 2e31  stroke-width:0.1
-0000a9e0: 3332 3239 323b 7374 726f 6b65 2d6d 6974  32292;stroke-mit
-0000a9f0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000aa00: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000aa10: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-0000aa20: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-0000aa30: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-0000aa40: 2270 6174 6831 3435 3637 2d33 2d37 2d33  "path14567-3-7-3
-0000aa50: 2d30 2d39 2d31 220a 2020 2020 2020 2063  -0-9-1".       c
-0000aa60: 783d 2231 3537 2e33 3735 3732 220a 2020  x="157.37572".  
-0000aa70: 2020 2020 2063 793d 2231 3336 2e31 3134       cy="136.114
-0000aa80: 3335 220a 2020 2020 2020 2069 6e6b 7363  35".       inksc
-0000aa90: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-0000aaa0: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
-0000aab0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-0000aac0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000aad0: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
-0000aae0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
-0000aaf0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000ab00: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000ab10: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000ab20: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
-0000ab30: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
-0000ab40: 302e 3134 3831 3335 3537 220a 2020 2020  0.14813557".    
-0000ab50: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000ab60: 6138 6139 6161 3b66 696c 6c2d 6f70 6163  a8a9aa;fill-opac
-0000ab70: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-0000ab80: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-0000ab90: 683a 302e 3133 3232 3932 3b73 7472 6f6b  h:0.132292;strok
-0000aba0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000abb0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000abc0: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
-0000abd0: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
-0000abe0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-0000abf0: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
-0000ac00: 332d 352d 382d 382d 352d 3822 0a20 2020  3-5-8-8-5-8".   
-0000ac10: 2020 2020 6378 3d22 3135 372e 3431 3038      cx="157.4108
-0000ac20: 3622 0a20 2020 2020 2020 6379 3d22 3133  6".       cy="13
-0000ac30: 372e 3031 3031 3822 0a20 2020 2020 2020  7.01018".       
-0000ac40: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-0000ac50: 726d 2d63 656e 7465 722d 783d 2234 2e36  rm-center-x="4.6
-0000ac60: 3433 3235 3636 220a 2020 2020 2020 2069  432566".       i
-0000ac70: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-0000ac80: 6d2d 6365 6e74 6572 2d79 3d22 2d39 2e39  m-center-y="-9.9
-0000ac90: 3738 3036 3231 220a 2020 2020 2020 2069  780621".       i
-0000aca0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-0000acb0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-0000acc0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000acd0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-0000ace0: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-0000acf0: 2020 723d 2230 2e31 3438 3133 3535 3722    r="0.14813557"
-0000ad00: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-0000ad10: 696c 6c3a 2361 6261 6139 633b 6669 6c6c  ill:#abaa9c;fill
-0000ad20: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000ad30: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000ad40: 2d77 6964 7468 3a30 2e31 3332 3239 323b  -width:0.132292;
-0000ad50: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-0000ad60: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-0000ad70: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-0000ad80: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-0000ad90: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000ada0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000adb0: 3435 3637 2d33 2d39 2d30 2d39 2d38 2d32  4567-3-9-0-9-8-2
-0000adc0: 220a 2020 2020 2020 2063 783d 2231 3536  ".       cx="156
-0000add0: 2e34 3937 3437 220a 2020 2020 2020 2063  .49747".       c
-0000ade0: 793d 2231 3337 2e37 3132 3738 220a 2020  y="137.71278".  
-0000adf0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-0000ae00: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
-0000ae10: 3d22 342e 3634 3332 3536 3622 0a20 2020  ="4.6432566".   
-0000ae20: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-0000ae30: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
-0000ae40: 222d 392e 3937 3830 3632 3122 0a20 2020  "-9.9780621".   
-0000ae50: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000ae60: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000ae70: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000ae80: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000ae90: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-0000aea0: 2020 2020 2020 2072 3d22 302e 3232 3836         r="0.2286
-0000aeb0: 3236 3439 220a 2020 2020 2020 2073 7479  2649".       sty
-0000aec0: 6c65 3d22 6669 6c6c 3a23 3131 3230 3636  le="fill:#112066
-0000aed0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000aee0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000aef0: 7472 6f6b 652d 7769 6474 683a 302e 3133  troke-width:0.13
-0000af00: 3232 3932 3b73 7472 6f6b 652d 6d69 7465  2292;stroke-mite
-0000af10: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000af20: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000af30: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0000af40: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-0000af50: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
-0000af60: 7061 7468 3134 3536 372d 332d 322d 352d  path14567-3-2-5-
-0000af70: 342d 332d 3822 0a20 2020 2020 2020 6378  4-3-8".       cx
-0000af80: 3d22 3135 352e 3533 3133 3722 0a20 2020  ="155.53137".   
-0000af90: 2020 2020 6379 3d22 3133 342e 3234 3336      cy="134.2436
-0000afa0: 3522 0a20 2020 2020 2020 696e 6b73 6361  5".       inksca
-0000afb0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000afc0: 7465 722d 783d 2237 2e31 3636 3231 3136  ter-x="7.1662116
-0000afd0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000afe0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000aff0: 6572 2d79 3d22 2d31 352e 3339 3937 3531  er-y="-15.399751
-0000b000: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b010: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000b020: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000b030: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000b040: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
-0000b050: 7263 6c65 0a20 2020 2020 2020 723d 2230  rcle.       r="0
-0000b060: 2e31 3438 3133 3535 3722 0a20 2020 2020  .14813557".     
-0000b070: 2020 7374 796c 653d 2266 696c 6c3a 2365    style="fill:#e
-0000b080: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
-0000b090: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-0000b0a0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000b0b0: 652d 7769 6474 683a 302e 3133 3232 3932  e-width:0.132292
-0000b0c0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000b0d0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000b0e0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000b0f0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000b100: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000b110: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000b120: 3134 3536 372d 322d 362d 302d 302d 3222  14567-2-6-0-0-2"
-0000b130: 0a20 2020 2020 2020 6378 3d22 3135 362e  .       cx="156.
-0000b140: 3736 3937 3322 0a20 2020 2020 2020 6379  76973".       cy
-0000b150: 3d22 3133 342e 3439 3833 3522 0a20 2020  ="134.49835".   
-0000b160: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000b170: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000b180: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000b190: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000b1a0: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-0000b1b0: 2020 2020 2020 2072 3d22 302e 3134 3831         r="0.1481
-0000b1c0: 3335 3537 220a 2020 2020 2020 2073 7479  3557".       sty
-0000b1d0: 6c65 3d22 6669 6c6c 3a23 6564 6630 6663  le="fill:#edf0fc
-0000b1e0: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
-0000b1f0: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
-0000b200: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-0000b210: 7468 3a30 2e31 3332 3239 323b 7374 726f  th:0.132292;stro
-0000b220: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000b230: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000b240: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-0000b250: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-0000b260: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-0000b270: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-0000b280: 2d32 2d38 2d36 2d37 2d38 2d32 220a 2020  -2-8-6-7-8-2".  
-0000b290: 2020 2020 2063 783d 2231 3534 2e32 3035       cx="154.205
-0000b2a0: 3222 0a20 2020 2020 2020 6379 3d22 3133  2".       cy="13
-0000b2b0: 352e 3732 3739 3222 0a20 2020 2020 2020  5.72792".       
-0000b2c0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000b2d0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-0000b2e0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000b2f0: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-0000b300: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-0000b310: 2020 2072 3d22 302e 3238 3135 3833 3934     r="0.28158394
-0000b320: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-0000b330: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
-0000b340: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
-0000b350: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
-0000b360: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-0000b370: 2e31 3332 3239 323b 7374 726f 6b65 2d6d  .132292;stroke-m
-0000b380: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000b390: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000b3a0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-0000b3b0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-0000b3c0: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-0000b3d0: 643d 2270 6174 6831 3435 3637 2d32 2d37  d="path14567-2-7
-0000b3e0: 2d30 2d39 2d30 2d35 220a 2020 2020 2020  -0-9-0-5".      
-0000b3f0: 2063 783d 2231 3630 2e30 3435 3632 220a   cx="160.04562".
-0000b400: 2020 2020 2020 2063 793d 2231 3335 2e31         cy="135.1
-0000b410: 3932 3138 220a 2020 2020 2020 2069 6e6b  9218".       ink
-0000b420: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-0000b430: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-0000b440: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-0000b450: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-0000b460: 203c 7265 6374 0a20 2020 2020 2020 7374   <rect.       st
-0000b470: 796c 653d 2266 696c 6c3a 2362 3362 3362  yle="fill:#b3b3b
-0000b480: 333b 6669 6c6c 2d6f 7061 6369 7479 3a31  3;fill-opacity:1
-0000b490: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-0000b4a0: 6f6b 652d 7769 6474 683a 302e 3133 3232  oke-width:0.1322
-0000b4b0: 3932 3b73 7472 6f6b 652d 6d69 7465 726c  92;stroke-miterl
-0000b4c0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000b4d0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000b4e0: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-0000b4f0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000b500: 3122 0a20 2020 2020 2020 6964 3d22 7265  1".       id="re
-0000b510: 6374 3135 3037 342d 302d 392d 322d 392d  ct15074-0-9-2-9-
-0000b520: 3422 0a20 2020 2020 2020 7769 6474 683d  4".       width=
-0000b530: 2234 2e32 3333 3333 3236 220a 2020 2020  "4.2333326".    
-0000b540: 2020 2068 6569 6768 743d 2234 2e32 3333     height="4.233
-0000b550: 3333 3236 220a 2020 2020 2020 2078 3d22  3326".       x="
-0000b560: 3136 372e 3733 3133 3722 0a20 2020 2020  167.73137".     
-0000b570: 2020 793d 2231 3331 2e36 3036 3636 220a    y="131.60666".
-0000b580: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000b590: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000b5a0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b5b0: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-0000b5c0: 3030 2220 2f3e 0a20 2020 203c 7061 7468  00" />.    <path
-0000b5d0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-0000b5e0: 696c 6c3a 2333 6534 6237 373b 6669 6c6c  ill:#3e4b77;fill
-0000b5f0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000b600: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000b610: 2d77 6964 7468 3a30 2e31 3332 3239 323b  -width:0.132292;
-0000b620: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-0000b630: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-0000b640: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-0000b650: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000b660: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000b670: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-0000b680: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-0000b690: 6d20 3136 372e 3930 3938 382c 3133 332e  m 167.90988,133.
-0000b6a0: 3030 3633 3420 312e 3433 3734 382c 2d30  00634 1.43748,-0
-0000b6b0: 2e30 3635 3320 302e 3934 3434 372c 2d31  .0653 0.94447,-1
-0000b6c0: 2e30 3531 3338 2063 202d 312e 3138 3938  .05138 c -1.1898
-0000b6d0: 332c 302e 3830 3031 3820 2d31 2e37 3538  3,0.80018 -1.758
-0000b6e0: 3237 2c30 2e39 3238 3620 2d32 2e33 3831  27,0.9286 -2.381
-0000b6f0: 3935 2c31 2e31 3136 3732 207a 220a 2020  95,1.11672 z".  
-0000b700: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000b710: 3437 2d31 2d37 2d38 2d35 2d30 220a 2020  47-1-7-8-5-0".  
-0000b720: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-0000b730: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-0000b740: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
-0000b750: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-0000b760: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
-0000b770: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000b780: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000b790: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000b7a0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000b7b0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-0000b7c0: 7479 6c65 3d22 6669 6c6c 3a23 3036 3035  tyle="fill:#0605
-0000b7d0: 3038 3b66 696c 6c2d 6f70 6163 6974 793a  08;fill-opacity:
-0000b7e0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-0000b7f0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-0000b800: 3133 3232 3932 3b73 7472 6f6b 652d 6c69  132292;stroke-li
-0000b810: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-0000b820: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-0000b830: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000b840: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000b850: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000b860: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000b870: 2020 2020 643d 226d 2031 3639 2e33 3437      d="m 169.347
-0000b880: 3336 2c31 3332 2e39 3431 3034 2032 2e32  36,132.94104 2.2
-0000b890: 3932 3835 2c30 2e34 3339 3532 2063 202d  9285,0.43952 c -
-0000b8a0: 302e 3635 3034 342c 2d30 2e33 3433 3835  0.65044,-0.34385
-0000b8b0: 202d 312e 3032 3731 2c2d 302e 3839 3633   -1.0271,-0.8963
-0000b8c0: 202d 312e 3334 3833 382c 2d31 2e34 3930   -1.34838,-1.490
-0000b8d0: 3934 207a 220a 2020 2020 2020 2069 643d  94 z".       id=
-0000b8e0: 2270 6174 6831 3435 3531 2d30 2d33 2d39  "path14551-0-3-9
-0000b8f0: 2d39 2d34 220a 2020 2020 2020 2069 6e6b  -9-4".       ink
-0000b900: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-0000b910: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-0000b920: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-0000b930: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
-0000b940: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000b950: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000b960: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000b970: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000b980: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-0000b990: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-0000b9a0: 6c6c 3a23 3237 3337 3733 3b66 696c 6c2d  ll:#273773;fill-
-0000b9b0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-0000b9c0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-0000b9d0: 7769 6474 683a 302e 3133 3232 3932 3b73  width:0.132292;s
-0000b9e0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000b9f0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000ba00: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000ba10: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000ba20: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000ba30: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-0000ba40: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-0000ba50: 2031 3637 2e39 3039 3838 2c31 3333 2e30   167.90988,133.0
-0000ba60: 3036 3334 2063 2030 2e33 3136 3332 2c30  0634 c 0.31632,0
-0000ba70: 2e31 3831 3437 2030 2e36 3635 3039 2c30  .18147 0.66509,0
-0000ba80: 2e33 3337 3937 2030 2e37 3834 3038 2c30  .33797 0.78408,0
-0000ba90: 2e36 3731 3232 206c 2030 2e36 3533 342c  .67122 l 0.6534,
-0000baa0: 2d30 2e37 3336 3536 207a 220a 2020 2020  -0.73656 z".    
-0000bab0: 2020 2069 643d 2270 6174 6831 3435 3533     id="path14553
-0000bac0: 2d33 2d32 2d32 2d31 2d33 220a 2020 2020  -3-2-2-1-3".    
-0000bad0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-0000bae0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-0000baf0: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
-0000bb00: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-0000bb10: 6363 6322 0a20 2020 2020 2020 696e 6b73  ccc".       inks
-0000bb20: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-0000bb30: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
-0000bb40: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-0000bb50: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-0000bb60: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-0000bb70: 6c65 3d22 6669 6c6c 3a23 3134 3236 3732  le="fill:#142672
-0000bb80: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000bb90: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000bba0: 7472 6f6b 652d 7769 6474 683a 302e 3133  troke-width:0.13
-0000bbb0: 3232 3932 3b73 7472 6f6b 652d 6c69 6e65  2292;stroke-line
-0000bbc0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-0000bbd0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-0000bbe0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000bbf0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-0000bc00: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-0000bc10: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-0000bc20: 2020 643d 226d 2031 3638 2e36 3933 3936    d="m 168.69396
-0000bc30: 2c31 3333 2e36 3737 3536 2032 2e39 3436  ,133.67756 2.946
-0000bc40: 3235 2c2d 302e 3239 3720 2d32 2e32 3932  25,-0.297 -2.292
-0000bc50: 3835 2c2d 302e 3433 3935 3620 7a22 0a20  85,-0.43956 z". 
-0000bc60: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000bc70: 3535 352d 342d 312d 362d 372d 3222 0a20  555-4-1-6-7-2". 
-0000bc80: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-0000bc90: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-0000bca0: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
+00008b70: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00008b80: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+00008b90: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00008ba0: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
+00008bb0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00008bc0: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
+00008bd0: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
+00008be0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00008bf0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00008c00: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
+00008c10: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00008c20: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00008c30: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00008c40: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00008c50: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00008c60: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00008c70: 2020 2020 2020 643d 226d 2034 382e 3738        d="m 48.78
+00008c80: 3838 3931 2c31 3939 2e31 3230 3632 2031  8891,199.12062 1
+00008c90: 362e 3937 3136 312c 3232 2e33 3137 3031  6.97161,22.31701
+00008ca0: 202d 362e 3238 3038 332c 2d33 302e 3036   -6.28083,-30.06
+00008cb0: 3738 3220 7a22 0a20 2020 2020 2020 2020  782 z".         
+00008cc0: 6964 3d22 7061 7468 3134 3536 332d 3122  id="path14563-1"
+00008cd0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00008ce0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00008cf0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+00008d00: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00008d10: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00008d20: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00008d30: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00008d40: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
+00008d50: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00008d60: 3d22 6669 6c6c 3a23 3238 3364 3837 3b66  ="fill:#283d87;f
+00008d70: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00008d80: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00008d90: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
+00008da0: 3235 3b73 7472 6f6b 652d 6c69 6e65 6361  25;stroke-lineca
+00008db0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00008dc0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00008dd0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00008de0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00008df0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00008e00: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00008e10: 2020 643d 226d 2035 392e 3437 3936 3731    d="m 59.479671
+00008e20: 2c31 3931 2e33 3639 3831 2036 2e32 3830  ,191.36981 6.280
+00008e30: 3833 2c33 302e 3036 3738 3220 6320 332e  83,30.06782 c 3.
+00008e40: 3235 3134 352c 2d32 372e 3032 3935 3720  25145,-27.02957 
+00008e50: 3134 2e36 3933 3635 2c2d 3336 2e37 3637  14.69365,-36.767
+00008e60: 3536 2032 332e 3932 3036 332c 2d35 312e  56 23.92063,-51.
+00008e70: 3138 3231 3220 7a22 0a20 2020 2020 2020  18212 z".       
+00008e80: 2020 6964 3d22 7061 7468 3134 3536 352d    id="path14565-
+00008e90: 3922 0a20 2020 2020 2020 2020 696e 6b73  9".         inks
+00008ea0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00008eb0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+00008ec0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00008ed0: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
+00008ee0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00008ef0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+00008f00: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
+00008f10: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+00008f20: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
+00008f30: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
+00008f40: 2020 2073 7479 6c65 3d22 6f70 6163 6974     style="opacit
+00008f50: 793a 313b 6669 6c6c 3a23 3037 3065 3262  y:1;fill:#070e2b
+00008f60: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
+00008f70: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
+00008f80: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00008f90: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
+00008fa0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00008fb0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00008fc0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+00008fd0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+00008fe0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00008ff0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00009000: 3637 2d36 220a 2020 2020 2020 2020 2063  67-6".         c
+00009010: 783d 2236 2e34 3434 3836 3238 220a 2020  x="6.4448628".  
+00009020: 2020 2020 2020 2063 793d 2231 3631 2e38         cy="161.8
+00009030: 3730 3832 220a 2020 2020 2020 2020 2072  7082".         r
+00009040: 783d 2231 2e36 3636 3333 3237 220a 2020  x="1.6663327".  
+00009050: 2020 2020 2020 2072 793d 2231 2e36 3636         ry="1.666
+00009060: 3333 3238 220a 2020 2020 2020 2020 2069  3328".         i
+00009070: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00009080: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+00009090: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+000090a0: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+000090b0: 0a20 2020 2020 203c 6369 7263 6c65 0a20  .      <circle. 
+000090c0: 2020 2020 2020 2020 723d 2231 2e36 3636          r="1.666
+000090d0: 3333 3238 220a 2020 2020 2020 2020 2073  3328".         s
+000090e0: 7479 6c65 3d22 6f70 6163 6974 793a 313b  tyle="opacity:1;
+000090f0: 6669 6c6c 3a23 3235 3361 3764 3b66 696c  fill:#253a7d;fil
+00009100: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00009110: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00009120: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
+00009130: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00009140: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00009150: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00009160: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+00009170: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00009180: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00009190: 7468 3134 3536 372d 332d 3933 220a 2020  th14567-3-93".  
+000091a0: 2020 2020 2020 2063 783d 2231 392e 3635         cx="19.65
+000091b0: 3536 3332 220a 2020 2020 2020 2020 2063  5632".         c
+000091c0: 793d 2231 3934 2e34 3838 3835 220a 2020  y="194.48885".  
+000091d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000091e0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+000091f0: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
+00009200: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00009210: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+00009220: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
+00009230: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00009240: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+00009250: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
+00009260: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+00009270: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+00009280: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
+00009290: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
+000092a0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000092b0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
+000092c0: 2332 3533 6137 643b 6669 6c6c 2d6f 7061  #253a7d;fill-opa
+000092d0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+000092e0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+000092f0: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
+00009300: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00009310: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00009320: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+00009330: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+00009340: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00009350: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00009360: 3637 2d33 2d37 2d33 220a 2020 2020 2020  67-3-7-3".      
+00009370: 2020 2063 783d 2235 392e 3037 3339 3231     cx="59.073921
+00009380: 220a 2020 2020 2020 2020 2063 793d 2231  ".         cy="1
+00009390: 3831 2e30 3533 3031 220a 2020 2020 2020  81.05301".      
+000093a0: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+000093b0: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
+000093c0: 342e 3634 3332 3536 3622 0a20 2020 2020  4.6432566".     
+000093d0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+000093e0: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
+000093f0: 222d 392e 3937 3830 3632 3122 0a20 2020  "-9.9780621".   
+00009400: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00009410: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+00009420: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00009430: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+00009440: 3330 3022 202f 3e0a 2020 2020 2020 3c63  300" />.      <c
+00009450: 6972 636c 650a 2020 2020 2020 2020 2072  ircle.         r
+00009460: 3d22 312e 3636 3633 3332 3822 0a20 2020  ="1.6663328".   
+00009470: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
+00009480: 6369 7479 3a31 3b66 696c 6c3a 2361 3861  city:1;fill:#a8a
+00009490: 3961 613b 6669 6c6c 2d6f 7061 6369 7479  9aa;fill-opacity
+000094a0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+000094b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+000094c0: 2e35 3535 3632 353b 7374 726f 6b65 2d6d  .555625;stroke-m
+000094d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000094e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000094f0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+00009500: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+00009510: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00009520: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+00009530: 2d35 2d38 220a 2020 2020 2020 2020 2063  -5-8".         c
+00009540: 783d 2235 392e 3436 3930 3933 220a 2020  x="59.469093".  
+00009550: 2020 2020 2020 2063 793d 2231 3931 2e31         cy="191.1
+00009560: 3239 3837 220a 2020 2020 2020 2020 2069  2987".         i
+00009570: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00009580: 6d2d 6365 6e74 6572 2d78 3d22 342e 3634  m-center-x="4.64
+00009590: 3332 3536 3622 0a20 2020 2020 2020 2020  32566".         
+000095a0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+000095b0: 726d 2d63 656e 7465 722d 793d 222d 392e  rm-center-y="-9.
+000095c0: 3937 3830 3632 3122 0a20 2020 2020 2020  9780621".       
+000095d0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+000095e0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+000095f0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00009600: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00009610: 202f 3e0a 2020 2020 2020 3c63 6972 636c   />.      <circl
+00009620: 650a 2020 2020 2020 2020 2072 3d22 312e  e.         r="1.
+00009630: 3636 3633 3332 3822 0a20 2020 2020 2020  6663328".       
+00009640: 2020 7374 796c 653d 226f 7061 6369 7479    style="opacity
+00009650: 3a31 3b66 696c 6c3a 2361 6261 6139 633b  :1;fill:#abaa9c;
+00009660: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00009670: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00009680: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
+00009690: 3632 353b 7374 726f 6b65 2d6d 6974 6572  625;stroke-miter
+000096a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+000096b0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+000096c0: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
+000096d0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
+000096e0: 3a31 220a 2020 2020 2020 2020 2069 643d  :1".         id=
+000096f0: 2270 6174 6831 3435 3637 2d33 2d39 2d30  "path14567-3-9-0
+00009700: 220a 2020 2020 2020 2020 2063 783d 2234  ".         cx="4
+00009710: 392e 3139 3436 3439 220a 2020 2020 2020  9.194649".      
+00009720: 2020 2063 793d 2231 3939 2e30 3333 3238     cy="199.03328
+00009730: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00009740: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+00009750: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
+00009760: 3622 0a20 2020 2020 2020 2020 696e 6b73  6".         inks
+00009770: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+00009780: 656e 7465 722d 793d 222d 392e 3937 3830  enter-y="-9.9780
+00009790: 3632 3122 0a20 2020 2020 2020 2020 696e  621".         in
+000097a0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+000097b0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+000097c0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+000097d0: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+000097e0: 2020 2020 2020 3c63 6972 636c 650a 2020        <circle.  
+000097f0: 2020 2020 2020 2072 3d22 322e 3537 3137         r="2.5717
+00009800: 3531 3122 0a20 2020 2020 2020 2020 7374  511".         st
+00009810: 796c 653d 226f 7061 6369 7479 3a31 3b66  yle="opacity:1;f
+00009820: 696c 6c3a 2331 3132 3036 363b 6669 6c6c  ill:#112066;fill
+00009830: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00009840: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00009850: 2d77 6964 7468 3a30 2e35 3535 3632 353b  -width:0.555625;
+00009860: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00009870: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00009880: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00009890: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+000098a0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+000098b0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+000098c0: 6831 3435 3637 2d33 2d32 2d35 220a 2020  h14567-3-2-5".  
+000098d0: 2020 2020 2020 2063 783d 2233 382e 3332         cx="38.32
+000098e0: 3734 3436 220a 2020 2020 2020 2020 2063  7446".         c
+000098f0: 793d 2231 3630 2e30 3130 3138 220a 2020  y="160.01018".  
+00009900: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00009910: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+00009920: 2d78 3d22 372e 3136 3632 3131 3622 0a20  -x="7.1662116". 
+00009930: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00009940: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+00009950: 722d 793d 222d 3135 2e33 3939 3735 3122  r-y="-15.399751"
+00009960: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00009970: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+00009980: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
+00009990: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+000099a0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+000099b0: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
+000099c0: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
+000099d0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000099e0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
+000099f0: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
+00009a00: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
+00009a10: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00009a20: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
+00009a30: 3235 3b73 7472 6f6b 652d 6d69 7465 726c  25;stroke-miterl
+00009a40: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00009a50: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00009a60: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+00009a70: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00009a80: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
+00009a90: 7061 7468 3134 3536 372d 322d 3622 0a20  path14567-2-6". 
+00009aa0: 2020 2020 2020 2020 6378 3d22 3532 2e32          cx="52.2
+00009ab0: 3537 3232 3522 0a20 2020 2020 2020 2020  57225".         
+00009ac0: 6379 3d22 3136 322e 3837 3531 3722 0a20  cy="162.87517". 
+00009ad0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00009ae0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00009af0: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+00009b00: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00009b10: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
+00009b20: 3c63 6972 636c 650a 2020 2020 2020 2020  <circle.        
+00009b30: 2072 3d22 312e 3636 3633 3332 3822 0a20   r="1.6663328". 
+00009b40: 2020 2020 2020 2020 7374 796c 653d 226f          style="o
+00009b50: 7061 6369 7479 3a31 3b66 696c 6c3a 2365  pacity:1;fill:#e
+00009b60: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
+00009b70: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
+00009b80: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00009b90: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
+00009ba0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00009bb0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00009bc0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00009bd0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+00009be0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00009bf0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00009c00: 7468 3134 3536 372d 322d 382d 3622 0a20  th14567-2-8-6". 
+00009c10: 2020 2020 2020 2020 6378 3d22 3233 2e34          cx="23.4
+00009c20: 3039 3735 3222 0a20 2020 2020 2020 2020  09752".         
+00009c30: 6379 3d22 3137 362e 3730 3631 3522 0a20  cy="176.70615". 
+00009c40: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00009c50: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00009c60: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+00009c70: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00009c80: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
+00009c90: 3c63 6972 636c 650a 2020 2020 2020 2020  <circle.        
+00009ca0: 2072 3d22 332e 3136 3734 3533 3822 0a20   r="3.1674538". 
+00009cb0: 2020 2020 2020 2020 7374 796c 653d 226f          style="o
+00009cc0: 7061 6369 7479 3a31 3b66 696c 6c3a 2365  pacity:1;fill:#e
+00009cd0: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
+00009ce0: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
+00009cf0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00009d00: 652d 7769 6474 683a 312e 3035 3631 363b  e-width:1.05616;
+00009d10: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00009d20: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00009d30: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00009d40: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00009d50: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00009d60: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00009d70: 6831 3435 3637 2d32 2d37 2d30 220a 2020  h14567-2-7-0".  
+00009d80: 2020 2020 2020 2063 783d 2238 392e 3130         cx="89.10
+00009d90: 3638 3935 220a 2020 2020 2020 2020 2063  6895".         c
+00009da0: 793d 2231 3730 2e36 3739 3739 220a 2020  y="170.67979".  
+00009db0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00009dc0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+00009dd0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00009de0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+00009df0: 2233 3030 2220 2f3e 0a20 2020 203c 2f67  "300" />.    </g
+00009e00: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+00009e10: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00009e20: 3365 3462 3737 3b66 696c 6c2d 6f70 6163  3e4b77;fill-opac
+00009e30: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+00009e40: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00009e50: 683a 302e 3939 3939 3939 3b73 7472 6f6b  h:0.999999;strok
+00009e60: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00009e70: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00009e80: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00009e90: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00009ea0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00009eb0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00009ec0: 0a20 2020 2020 2020 643d 226d 2033 3137  .       d="m 317
+00009ed0: 2e30 3239 3335 2c33 3031 2e35 3339 3434  .02935,301.53944
+00009ee0: 2034 332e 3436 3430 332c 2d31 2e39 3735   43.46403,-1.975
+00009ef0: 3634 2032 382e 3535 3639 352c 2d33 312e  64 28.55695,-31.
+00009f00: 3738 3937 3920 6320 2d33 352e 3937 3537  78979 c -35.9757
+00009f10: 2c32 342e 3139 3432 3720 2d35 332e 3136  ,24.19427 -53.16
+00009f20: 3333 352c 3238 2e30 3737 3136 202d 3732  335,28.07716 -72
+00009f30: 2e30 3230 3938 2c33 332e 3736 3534 3320  .02098,33.76543 
+00009f40: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
+00009f50: 7468 3134 3534 372d 312d 3722 0a20 2020  th14547-1-7".   
+00009f60: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+00009f70: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+00009f80: 3d22 3022 0a20 2020 2020 2020 736f 6469  ="0".       sodi
+00009f90: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
+00009fa0: 6363 6363 220a 2020 2020 2020 2069 6e6b  cccc".       ink
+00009fb0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+00009fc0: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
+00009fd0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+00009fe0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+00009ff0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+0000a000: 796c 653d 2266 696c 6c3a 2331 6332 6336  yle="fill:#1c2c6
+0000a010: 383b 6669 6c6c 2d6f 7061 6369 7479 3a31  8;fill-opacity:1
+0000a020: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+0000a030: 7374 726f 6b65 2d77 6964 7468 3a30 2e39  stroke-width:0.9
+0000a040: 3939 3939 393b 7374 726f 6b65 2d6c 696e  99999;stroke-lin
+0000a050: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+0000a060: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+0000a070: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+0000a080: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+0000a090: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+0000a0a0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+0000a0b0: 2020 2064 3d22 6d20 3336 302e 3439 3333     d="m 360.4933
+0000a0c0: 382c 3239 392e 3536 3338 2031 382e 3835  8,299.5638 18.85
+0000a0d0: 3833 362c 342e 3331 3035 3220 392e 3639  836,4.31052 9.69
+0000a0e0: 3835 392c 2d33 362e 3130 3033 3120 7a22  859,-36.10031 z"
+0000a0f0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000a100: 3134 3534 392d 312d 3022 0a20 2020 2020  14549-1-0".     
+0000a110: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000a120: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000a130: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000a140: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000a150: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000a160: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000a170: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+0000a180: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+0000a190: 3d22 6669 6c6c 3a23 3036 3035 3038 3b66  ="fill:#060508;f
+0000a1a0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000a1b0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000a1c0: 6f6b 652d 7769 6474 683a 302e 3939 3939  oke-width:0.9999
+0000a1d0: 3939 3b73 7472 6f6b 652d 6c69 6e65 6361  99;stroke-lineca
+0000a1e0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+0000a1f0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+0000a200: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000a210: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000a220: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+0000a230: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000a240: 643d 226d 2033 3739 2e33 3531 3734 2c33  d="m 379.35174,3
+0000a250: 3033 2e38 3734 3332 2035 302e 3436 3835  03.87432 50.4685
+0000a260: 382c 382e 3938 3031 3520 6320 2d31 392e  8,8.98015 c -19.
+0000a270: 3636 3637 342c 2d31 302e 3339 3639 3520  66674,-10.39695 
+0000a280: 2d33 312e 3035 3534 342c 2d32 372e 3130  -31.05544,-27.10
+0000a290: 3039 3120 2d34 302e 3736 3939 392c 2d34  091 -40.76999,-4
+0000a2a0: 352e 3038 3034 3620 7a22 0a20 2020 2020  5.08046 z".     
+0000a2b0: 2020 6964 3d22 7061 7468 3134 3535 312d    id="path14551-
+0000a2c0: 302d 3322 0a20 2020 2020 2020 696e 6b73  0-3".       inks
+0000a2d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+0000a2e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+0000a2f0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+0000a300: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
+0000a310: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000a320: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000a330: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000a340: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000a350: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+0000a360: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000a370: 6c3a 2332 3733 3737 333b 6669 6c6c 2d6f  l:#273773;fill-o
+0000a380: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+0000a390: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+0000a3a0: 6964 7468 3a30 2e39 3939 3939 393b 7374  idth:0.999999;st
+0000a3b0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+0000a3c0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+0000a3d0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+0000a3e0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000a3f0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000a400: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+0000a410: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+0000a420: 3331 372e 3032 3933 352c 3330 312e 3533  317.02935,301.53
+0000a430: 3934 3420 6320 392e 3536 3433 382c 352e  944 c 9.56438,5.
+0000a440: 3438 3637 3420 3230 2e31 3039 372c 3130  48674 20.1097,10
+0000a450: 2e32 3138 3933 2032 332e 3730 3736 352c  .21893 23.70765,
+0000a460: 3230 2e32 3935 3139 206c 2031 392e 3735  20.29519 l 19.75
+0000a470: 3633 382c 2d32 322e 3237 3038 3320 7a22  638,-22.27083 z"
+0000a480: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000a490: 3134 3535 332d 332d 3222 0a20 2020 2020  14553-3-2".     
+0000a4a0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000a4b0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000a4c0: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+0000a4d0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+0000a4e0: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
+0000a4f0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000a500: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000a510: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000a520: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000a530: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000a540: 653d 2266 696c 6c3a 2331 3432 3637 323b  e="fill:#142672;
+0000a550: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000a560: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000a570: 726f 6b65 2d77 6964 7468 3a30 2e39 3939  roke-width:0.999
+0000a580: 3939 393b 7374 726f 6b65 2d6c 696e 6563  999;stroke-linec
+0000a590: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000a5a0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000a5b0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000a5c0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000a5d0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000a5e0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000a5f0: 2064 3d22 6d20 3334 302e 3733 372c 3332   d="m 340.737,32
+0000a600: 312e 3833 3436 3320 3839 2e30 3833 3332  1.83463 89.08332
+0000a610: 2c2d 382e 3938 3031 3620 2d36 392e 3332  ,-8.98016 -69.32
+0000a620: 3639 342c 2d31 332e 3239 3036 3720 7a22  694,-13.29067 z"
+0000a630: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000a640: 3134 3535 352d 342d 3122 0a20 2020 2020  14555-4-1".     
+0000a650: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000a660: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000a670: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000a680: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000a690: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000a6a0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000a6b0: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+0000a6c0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+0000a6d0: 3d22 6669 6c6c 3a23 3534 3636 3863 3b66  ="fill:#54668c;f
+0000a6e0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000a6f0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000a700: 6f6b 652d 7769 6474 683a 302e 3939 3939  oke-width:0.9999
+0000a710: 3939 3b73 7472 6f6b 652d 6c69 6e65 6361  99;stroke-lineca
+0000a720: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+0000a730: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+0000a740: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000a750: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000a760: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+0000a770: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000a780: 643d 226d 2033 3430 2e37 3337 2c33 3231  d="m 340.737,321
+0000a790: 2e38 3334 3633 2035 312e 3336 3635 382c  .83463 51.36658,
+0000a7a0: 352e 3338 3831 2033 372e 3731 3637 342c  5.3881 37.71674,
+0000a7b0: 2d31 342e 3336 3832 3620 7a22 0a20 2020  -14.36826 z".   
+0000a7c0: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+0000a7d0: 372d 302d 3722 0a20 2020 2020 2020 696e  7-0-7".       in
+0000a7e0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+0000a7f0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+0000a800: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000a810: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+0000a820: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000a830: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+0000a840: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
+0000a850: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+0000a860: 6c6c 3a23 3232 3334 3765 3b66 696c 6c2d  ll:#22347e;fill-
+0000a870: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+0000a880: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+0000a890: 7769 6474 683a 302e 3939 3939 3939 3b73  width:0.999999;s
+0000a8a0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+0000a8b0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+0000a8c0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+0000a8d0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000a8e0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000a8f0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+0000a900: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+0000a910: 2033 3430 2e37 3337 2c33 3231 2e38 3334   340.737,321.834
+0000a920: 3633 2063 2031 2e31 3535 3035 2c39 2e39  63 c 1.15505,9.9
+0000a930: 3539 3133 202d 322e 3834 3330 332c 3136  5913 -2.84303,16
+0000a940: 2e32 3337 3439 202d 342e 3636 3936 382c  .23749 -4.66968,
+0000a950: 3234 2e30 3636 3836 206c 2035 362e 3033  24.06686 l 56.03
+0000a960: 3632 362c 2d31 382e 3637 3837 3620 7a22  626,-18.67876 z"
+0000a970: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000a980: 3134 3535 392d 332d 3422 0a20 2020 2020  14559-3-4".     
+0000a990: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000a9a0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000a9b0: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+0000a9c0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+0000a9d0: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
+0000a9e0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000a9f0: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000aa00: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000aa10: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000aa20: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000aa30: 653d 2266 696c 6c3a 2330 3831 3036 393b  e="fill:#081069;
+0000aa40: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000aa50: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000aa60: 726f 6b65 2d77 6964 7468 3a30 2e39 3939  roke-width:0.999
+0000aa70: 3939 393b 7374 726f 6b65 2d6c 696e 6563  999;stroke-linec
+0000aa80: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000aa90: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000aaa0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000aab0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000aac0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000aad0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000aae0: 2064 3d22 6d20 3333 362e 3036 3733 322c   d="m 336.06732,
+0000aaf0: 3334 352e 3930 3134 3920 3338 2e37 3934  345.90149 38.794
+0000ab00: 3333 2c35 2e37 3437 3320 3534 2e39 3538  33,5.7473 54.958
+0000ab10: 3637 2c2d 3338 2e37 3934 3332 207a 220a  67,-38.79432 z".
+0000ab20: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000ab30: 3435 3631 2d39 2d32 220a 2020 2020 2020  4561-9-2".      
+0000ab40: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000ab50: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000ab60: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000ab70: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000ab80: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000ab90: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000aba0: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+0000abb0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+0000abc0: 2266 696c 6c3a 2330 3730 6532 623b 6669  "fill:#070e2b;fi
+0000abd0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000abe0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000abf0: 6b65 2d77 6964 7468 3a30 2e39 3939 3939  ke-width:0.99999
+0000ac00: 393b 7374 726f 6b65 2d6c 696e 6563 6170  9;stroke-linecap
+0000ac10: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+0000ac20: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+0000ac30: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000ac40: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000ac50: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+0000ac60: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+0000ac70: 3d22 6d20 3337 342e 3836 3136 352c 3335  ="m 374.86165,35
+0000ac80: 312e 3634 3837 3920 3232 2e38 3039 3633  1.64879 22.80963
+0000ac90: 2c32 392e 3939 3338 202d 382e 3434 3133  ,29.9938 -8.4413
+0000aca0: 352c 2d34 302e 3431 3037 3820 7a22 0a20  5,-40.41078 z". 
+0000acb0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000acc0: 3536 332d 312d 3022 0a20 2020 2020 2020  563-1-0".       
+0000acd0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+0000ace0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+0000acf0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000ad00: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+0000ad10: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000ad20: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+0000ad30: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
+0000ad40: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+0000ad50: 6669 6c6c 3a23 3238 3364 3837 3b66 696c  fill:#283d87;fil
+0000ad60: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000ad70: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000ad80: 652d 7769 6474 683a 302e 3939 3939 3939  e-width:0.999999
+0000ad90: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+0000ada0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+0000adb0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+0000adc0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+0000add0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+0000ade0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+0000adf0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+0000ae00: 226d 2033 3839 2e32 3239 3933 2c33 3431  "m 389.22993,341
+0000ae10: 2e32 3331 3831 2038 2e34 3431 3335 2c34  .23181 8.44135,4
+0000ae20: 302e 3431 3037 3820 6320 342e 3336 3939  0.41078 c 4.3699
+0000ae30: 332c 2d33 362e 3332 3734 3220 3139 2e37  3,-36.32742 19.7
+0000ae40: 3438 3037 2c2d 3439 2e34 3135 3133 2033  4807,-49.41513 3
+0000ae50: 322e 3134 3930 342c 2d36 382e 3738 3831  2.14904,-68.7881
+0000ae60: 3220 7a22 0a20 2020 2020 2020 6964 3d22  2 z".       id="
+0000ae70: 7061 7468 3134 3536 352d 392d 3522 0a20  path14565-9-5". 
+0000ae80: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+0000ae90: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+0000aea0: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
+0000aeb0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+0000aec0: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
+0000aed0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+0000aee0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+0000aef0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000af00: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+0000af10: 2020 203c 656c 6c69 7073 650a 2020 2020     <ellipse.    
+0000af20: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000af30: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
+0000af40: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+0000af50: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000af60: 6b65 2d77 6964 7468 3a30 2e39 3939 3939  ke-width:0.99999
+0000af70: 393b 7374 726f 6b65 2d6d 6974 6572 6c69  9;stroke-miterli
+0000af80: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000af90: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000afa0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+0000afb0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000afc0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000afd0: 6831 3435 3637 2d36 2d31 220a 2020 2020  h14567-6-1".    
+0000afe0: 2020 2063 783d 2233 3137 2e39 3531 3834     cx="317.95184
+0000aff0: 220a 2020 2020 2020 2063 793d 2233 3031  ".       cy="301
+0000b000: 2e35 3835 3537 220a 2020 2020 2020 2072  .58557".       r
+0000b010: 783d 2232 2e32 3339 3532 3936 220a 2020  x="2.2395296".  
+0000b020: 2020 2020 2072 793d 2232 2e32 3339 3532       ry="2.23952
+0000b030: 3938 220a 2020 2020 2020 2069 6e6b 7363  98".       inksc
+0000b040: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000b050: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000b060: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000b070: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000b080: 6369 7263 6c65 0a20 2020 2020 2020 723d  circle.       r=
+0000b090: 2232 2e32 3339 3532 3938 220a 2020 2020  "2.2395298".    
+0000b0a0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000b0b0: 3235 3361 3764 3b66 696c 6c2d 6f70 6163  253a7d;fill-opac
+0000b0c0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+0000b0d0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+0000b0e0: 683a 302e 3939 3939 3939 3b73 7472 6f6b  h:0.999999;strok
+0000b0f0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+0000b100: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+0000b110: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+0000b120: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+0000b130: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000b140: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+0000b150: 332d 3933 2d31 220a 2020 2020 2020 2063  3-93-1".       c
+0000b160: 783d 2233 3335 2e37 3036 3931 220a 2020  x="335.70691".  
+0000b170: 2020 2020 2063 793d 2233 3435 2e34 3233       cy="345.423
+0000b180: 3737 220a 2020 2020 2020 2069 6e6b 7363  77".       inksc
+0000b190: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+0000b1a0: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
+0000b1b0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000b1c0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000b1d0: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
+0000b1e0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+0000b1f0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000b200: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000b210: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000b220: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+0000b230: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
+0000b240: 322e 3233 3935 3239 3822 0a20 2020 2020  2.2395298".     
+0000b250: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
+0000b260: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
+0000b270: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000b280: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000b290: 3a30 2e39 3939 3939 393b 7374 726f 6b65  :0.999999;stroke
+0000b2a0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000b2b0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000b2c0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+0000b2d0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+0000b2e0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000b2f0: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+0000b300: 2d37 2d33 2d30 220a 2020 2020 2020 2063  -7-3-0".       c
+0000b310: 783d 2233 3838 2e36 3834 3622 0a20 2020  x="388.6846".   
+0000b320: 2020 2020 6379 3d22 3332 372e 3336 3632      cy="327.3662
+0000b330: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+0000b340: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000b350: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
+0000b360: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b370: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000b380: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
+0000b390: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b3a0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000b3b0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000b3c0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000b3d0: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
+0000b3e0: 7263 6c65 0a20 2020 2020 2020 723d 2232  rcle.       r="2
+0000b3f0: 2e32 3339 3532 3938 220a 2020 2020 2020  .2395298".      
+0000b400: 2073 7479 6c65 3d22 6669 6c6c 3a23 6138   style="fill:#a8
+0000b410: 6139 6161 3b66 696c 6c2d 6f70 6163 6974  a9aa;fill-opacit
+0000b420: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+0000b430: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+0000b440: 302e 3939 3939 3939 3b73 7472 6f6b 652d  0.999999;stroke-
+0000b450: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000b460: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000b470: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+0000b480: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+0000b490: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000b4a0: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
+0000b4b0: 352d 382d 3822 0a20 2020 2020 2020 6378  5-8-8".       cx
+0000b4c0: 3d22 3338 392e 3231 3537 3322 0a20 2020  ="389.21573".   
+0000b4d0: 2020 2020 6379 3d22 3334 302e 3930 3933      cy="340.9093
+0000b4e0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000b4f0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000b500: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
+0000b510: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b520: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000b530: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
+0000b540: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b550: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000b560: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000b570: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000b580: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
+0000b590: 7263 6c65 0a20 2020 2020 2020 723d 2232  rcle.       r="2
+0000b5a0: 2e32 3339 3532 3938 220a 2020 2020 2020  .2395298".      
+0000b5b0: 2073 7479 6c65 3d22 6669 6c6c 3a23 6162   style="fill:#ab
+0000b5c0: 6161 3963 3b66 696c 6c2d 6f70 6163 6974  aa9c;fill-opacit
+0000b5d0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+0000b5e0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+0000b5f0: 302e 3939 3939 3939 3b73 7472 6f6b 652d  0.999999;stroke-
+0000b600: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000b610: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000b620: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+0000b630: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+0000b640: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000b650: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
+0000b660: 392d 302d 3922 0a20 2020 2020 2020 6378  9-0-9".       cx
+0000b670: 3d22 3337 352e 3430 3639 3822 0a20 2020  ="375.40698".   
+0000b680: 2020 2020 6379 3d22 3335 312e 3533 3134      cy="351.5314
+0000b690: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
+0000b6a0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000b6b0: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
+0000b6c0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b6d0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000b6e0: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
+0000b6f0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b700: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000b710: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000b720: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000b730: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
+0000b740: 7263 6c65 0a20 2020 2020 2020 723d 2233  rcle.       r="3
+0000b750: 2e34 3536 3430 3034 220a 2020 2020 2020  .4564004".      
+0000b760: 2073 7479 6c65 3d22 6669 6c6c 3a23 3131   style="fill:#11
+0000b770: 3230 3636 3b66 696c 6c2d 6f70 6163 6974  2066;fill-opacit
+0000b780: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+0000b790: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+0000b7a0: 302e 3939 3939 3939 3b73 7472 6f6b 652d  0.999999;stroke-
+0000b7b0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000b7c0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000b7d0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+0000b7e0: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+0000b7f0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000b800: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
+0000b810: 322d 352d 3422 0a20 2020 2020 2020 6378  2-5-4".       cx
+0000b820: 3d22 3336 302e 3830 3136 3122 0a20 2020  ="360.80161".   
+0000b830: 2020 2020 6379 3d22 3239 392e 3038 3439      cy="299.0849
+0000b840: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000b850: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000b860: 6572 2d78 3d22 372e 3136 3632 3131 3622  er-x="7.1662116"
+0000b870: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000b880: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+0000b890: 722d 793d 222d 3135 2e33 3939 3735 3122  r-y="-15.399751"
+0000b8a0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000b8b0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+0000b8c0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000b8d0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+0000b8e0: 3330 3022 202f 3e0a 2020 2020 3c63 6972  300" />.    <cir
+0000b8f0: 636c 650a 2020 2020 2020 2072 3d22 322e  cle.       r="2.
+0000b900: 3233 3935 3239 3822 0a20 2020 2020 2020  2395298".       
+0000b910: 7374 796c 653d 2266 696c 6c3a 2365 6466  style="fill:#edf
+0000b920: 3066 633b 6669 6c6c 2d6f 7061 6369 7479  0fc;fill-opacity
+0000b930: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
+0000b940: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+0000b950: 7769 6474 683a 302e 3939 3939 3939 3b73  width:0.999999;s
+0000b960: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000b970: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000b980: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000b990: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+0000b9a0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+0000b9b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000b9c0: 3536 372d 322d 362d 3022 0a20 2020 2020  567-2-6-0".     
+0000b9d0: 2020 6378 3d22 3337 392e 3532 3330 3422    cx="379.52304"
+0000b9e0: 0a20 2020 2020 2020 6379 3d22 3330 322e  .       cy="302.
+0000b9f0: 3933 3533 3622 0a20 2020 2020 2020 696e  93536".       in
+0000ba00: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+0000ba10: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+0000ba20: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+0000ba30: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+0000ba40: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
+0000ba50: 2072 3d22 322e 3233 3935 3239 3822 0a20   r="2.2395298". 
+0000ba60: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000ba70: 6c3a 2365 6466 3066 633b 6669 6c6c 2d6f  l:#edf0fc;fill-o
+0000ba80: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
+0000ba90: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000baa0: 7472 6f6b 652d 7769 6474 683a 302e 3939  troke-width:0.99
+0000bab0: 3939 3939 3b73 7472 6f6b 652d 6d69 7465  9999;stroke-mite
+0000bac0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000bad0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000bae0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+0000baf0: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+0000bb00: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
+0000bb10: 7061 7468 3134 3536 372d 322d 382d 362d  path14567-2-8-6-
+0000bb20: 3722 0a20 2020 2020 2020 6378 3d22 3334  7".       cx="34
+0000bb30: 302e 3735 3234 3122 0a20 2020 2020 2020  0.75241".       
+0000bb40: 6379 3d22 3332 312e 3532 3430 3522 0a20  cy="321.52405". 
+0000bb50: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000bb60: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+0000bb70: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000bb80: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+0000bb90: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
+0000bba0: 650a 2020 2020 2020 2072 3d22 342e 3235  e.       r="4.25
+0000bbb0: 3730 3137 3122 0a20 2020 2020 2020 7374  70171".       st
+0000bbc0: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
+0000bbd0: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
+0000bbe0: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+0000bbf0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000bc00: 6474 683a 302e 3939 3939 3939 3b73 7472  dth:0.999999;str
+0000bc10: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000bc20: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000bc30: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+0000bc40: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+0000bc50: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000bc60: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+0000bc70: 372d 322d 372d 302d 3922 0a20 2020 2020  7-2-7-0-9".     
+0000bc80: 2020 6378 3d22 3432 392e 3034 3835 3522    cx="429.04855"
+0000bc90: 0a20 2020 2020 2020 6379 3d22 3331 332e  .       cy="313.
+0000bca0: 3432 3436 3822 0a20 2020 2020 2020 696e  42468".       in
 0000bcb0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
 0000bcc0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
 0000bcd0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
 0000bce0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
 0000bcf0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-0000bd00: 7479 6c65 3d22 6669 6c6c 3a23 3534 3636  tyle="fill:#5466
-0000bd10: 3863 3b66 696c 6c2d 6f70 6163 6974 793a  8c;fill-opacity:
+0000bd00: 7479 6c65 3d22 6669 6c6c 3a23 3365 3462  tyle="fill:#3e4b
+0000bd10: 3737 3b66 696c 6c2d 6f70 6163 6974 793a  77;fill-opacity:
 0000bd20: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
 0000bd30: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-0000bd40: 3133 3232 3932 3b73 7472 6f6b 652d 6c69  132292;stroke-li
+0000bd40: 3734 3839 3937 3b73 7472 6f6b 652d 6c69  748997;stroke-li
 0000bd50: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
 0000bd60: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
 0000bd70: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
 0000bd80: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
 0000bd90: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
 0000bda0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000bdb0: 2020 2020 643d 226d 2031 3638 2e36 3933      d="m 168.693
-0000bdc0: 3936 2c31 3333 2e36 3737 3536 2063 2030  96,133.67756 c 0
-0000bdd0: 2e30 3338 322c 302e 3332 3933 3820 2d30  .0382,0.32938 -0
-0000bde0: 2e30 3934 2c30 2e35 3337 3033 202d 302e  .094,0.53703 -0.
-0000bdf0: 3135 3434 342c 302e 3739 3539 3720 6c20  15444,0.79597 l 
-0000be00: 332e 3130 3036 392c 2d31 2e30 3932 3937  3.10069,-1.09297
-0000be10: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-0000be20: 6174 6831 3435 3539 2d33 2d34 2d32 2d34  ath14559-3-4-2-4
-0000be30: 2d34 220a 2020 2020 2020 2069 6e6b 7363  -4".       inksc
-0000be40: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-0000be50: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-0000be60: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-0000be70: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
-0000be80: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000be90: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000bea0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000beb0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000bec0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-0000bed0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-0000bee0: 3a23 3038 3130 3639 3b66 696c 6c2d 6f70  :#081069;fill-op
-0000bef0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-0000bf00: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000bf10: 6474 683a 302e 3133 3232 3932 3b73 7472  dth:0.132292;str
-0000bf20: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000bf30: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000bf40: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000bf50: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000bf60: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000bf70: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000bf80: 3122 0a20 2020 2020 2020 643d 226d 2031  1".       d="m 1
-0000bf90: 3638 2e35 3339 3532 2c31 3334 2e34 3733  68.53952,134.473
-0000bfa0: 3533 2031 2e32 3833 3035 2c30 2e31 3930  53 1.28305,0.190
-0000bfb0: 3038 2031 2e38 3137 3634 2c2d 312e 3238  08 1.81764,-1.28
-0000bfc0: 3330 3520 7a22 0a20 2020 2020 2020 6964  305 z".       id
-0000bfd0: 3d22 7061 7468 3134 3536 312d 392d 322d  ="path14561-9-2-
-0000bfe0: 322d 382d 3022 0a20 2020 2020 2020 696e  2-8-0".       in
-0000bff0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-0000c000: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-0000c010: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000c020: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000c030: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000c040: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000c050: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-0000c060: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-0000c070: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
-0000c080: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-0000c090: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-0000c0a0: 7769 6474 683a 302e 3133 3232 3932 3b73  width:0.132292;s
-0000c0b0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000c0c0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000c0d0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000c0e0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000c0f0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000c100: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-0000c110: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-0000c120: 2031 3639 2e38 3232 3537 2c31 3334 2e36   169.82257,134.6
-0000c130: 3633 3631 2030 2e37 3534 3338 2c30 2e39  6361 0.75438,0.9
-0000c140: 3931 3938 202d 302e 3237 3931 382c 2d31  9198 -0.27918,-1
-0000c150: 2e33 3336 3520 7a22 0a20 2020 2020 2020  .3365 z".       
-0000c160: 6964 3d22 7061 7468 3134 3536 332d 312d  id="path14563-1-
-0000c170: 302d 362d 382d 3722 0a20 2020 2020 2020  0-6-8-7".       
-0000c180: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000c190: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000c1a0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000c1b0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000c1c0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000c1d0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000c1e0: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-0000c1f0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-0000c200: 6669 6c6c 3a23 3037 3065 3262 3b66 696c  fill:#070e2b;fil
-0000c210: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000c220: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000c230: 652d 7769 6474 683a 302e 3133 3232 3932  e-width:0.132292
-0000c240: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000c250: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000c260: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000c270: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000c280: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000c290: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000c2a0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-0000c2b0: 226d 2031 3639 2e38 3232 3537 2c31 3334  "m 169.82257,134
-0000c2c0: 2e36 3633 3631 2030 2e37 3534 3338 2c30  .66361 0.75438,0
-0000c2d0: 2e39 3931 3938 2063 2030 2e31 3434 3532  .99198 c 0.14452
-0000c2e0: 2c2d 312e 3230 3134 3620 302e 3635 3331  ,-1.20146 0.6531
-0000c2f0: 322c 2d31 2e36 3334 3320 312e 3036 3332  2,-1.6343 1.0632
-0000c300: 362c 2d32 2e32 3735 3033 207a 220a 2020  6,-2.27503 z".  
-0000c310: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000c320: 3635 2d39 2d35 2d39 2d37 2d37 220a 2020  65-9-5-9-7-7".  
-0000c330: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-0000c340: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-0000c350: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
-0000c360: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-0000c370: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
-0000c380: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000c390: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000c3a0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000c3b0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000c3c0: 2020 3c65 6c6c 6970 7365 0a20 2020 2020    <ellipse.     
-0000c3d0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-0000c3e0: 3730 6532 623b 6669 6c6c 2d6f 7061 6369  70e2b;fill-opaci
-0000c3f0: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-0000c400: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000c410: 652d 7769 6474 683a 302e 3133 3232 3932  e-width:0.132292
-0000c420: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000c430: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000c440: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000c450: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000c460: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000c470: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000c480: 3134 3536 372d 362d 312d 392d 372d 3722  14567-6-1-9-7-7"
-0000c490: 0a20 2020 2020 2020 6378 3d22 3136 372e  .       cx="167.
-0000c4a0: 3934 3033 3822 0a20 2020 2020 2020 6379  94038".       cy
-0000c4b0: 3d22 3133 332e 3030 3738 3722 0a20 2020  ="133.00787".   
-0000c4c0: 2020 2020 7278 3d22 302e 3037 3430 3637      rx="0.074067
-0000c4d0: 3737 3122 0a20 2020 2020 2020 7279 3d22  771".       ry="
-0000c4e0: 302e 3037 3430 3637 3737 3922 0a20 2020  0.074067779".   
-0000c4f0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000c500: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000c510: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000c520: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000c530: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-0000c540: 2020 2020 2020 2072 3d22 302e 3037 3430         r="0.0740
-0000c550: 3637 3737 3922 0a20 2020 2020 2020 7374  67779".       st
-0000c560: 796c 653d 2266 696c 6c3a 2332 3533 6137  yle="fill:#253a7
-0000c570: 643b 6669 6c6c 2d6f 7061 6369 7479 3a31  d;fill-opacity:1
-0000c580: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000c590: 7374 726f 6b65 2d77 6964 7468 3a30 2e31  stroke-width:0.1
-0000c5a0: 3332 3239 323b 7374 726f 6b65 2d6d 6974  32292;stroke-mit
-0000c5b0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000c5c0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000c5d0: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-0000c5e0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-0000c5f0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-0000c600: 2270 6174 6831 3435 3637 2d33 2d39 332d  "path14567-3-93-
-0000c610: 312d 362d 392d 3322 0a20 2020 2020 2020  1-6-9-3".       
-0000c620: 6378 3d22 3136 382e 3532 3736 220a 2020  cx="168.5276".  
-0000c630: 2020 2020 2063 793d 2231 3334 2e34 3537       cy="134.457
-0000c640: 3733 220a 2020 2020 2020 2069 6e6b 7363  73".       inksc
-0000c650: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-0000c660: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
-0000c670: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-0000c680: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000c690: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
-0000c6a0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
-0000c6b0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000c6c0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000c6d0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000c6e0: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
-0000c6f0: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
-0000c700: 302e 3037 3430 3637 3737 3922 0a20 2020  0.074067779".   
-0000c710: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-0000c720: 2361 6261 6139 633b 6669 6c6c 2d6f 7061  #abaa9c;fill-opa
-0000c730: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-0000c740: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-0000c750: 7468 3a30 2e31 3332 3239 323b 7374 726f  th:0.132292;stro
-0000c760: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000c770: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000c780: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-0000c790: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-0000c7a0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-0000c7b0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-0000c7c0: 2d33 2d39 2d30 2d39 2d38 2d32 2d38 220a  -3-9-0-9-8-2-8".
-0000c7d0: 2020 2020 2020 2063 783d 2231 3639 2e38         cx="169.8
-0000c7e0: 3430 3631 220a 2020 2020 2020 2063 793d  4061".       cy=
-0000c7f0: 2231 3334 2e36 3539 3733 220a 2020 2020  "134.65973".    
-0000c800: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
-0000c810: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
-0000c820: 342e 3634 3332 3536 3622 0a20 2020 2020  4.6432566".     
-0000c830: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-0000c840: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
-0000c850: 392e 3937 3830 3632 3122 0a20 2020 2020  9.9780621".     
-0000c860: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000c870: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-0000c880: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000c890: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-0000c8a0: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
-0000c8b0: 2020 2020 2072 3d22 302e 3131 3433 3133       r="0.114313
-0000c8c0: 3233 220a 2020 2020 2020 2073 7479 6c65  23".       style
-0000c8d0: 3d22 6669 6c6c 3a23 3131 3230 3636 3b66  ="fill:#112066;f
-0000c8e0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000c8f0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000c900: 6f6b 652d 7769 6474 683a 302e 3133 3232  oke-width:0.1322
-0000c910: 3932 3b73 7472 6f6b 652d 6d69 7465 726c  92;stroke-miterl
-0000c920: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000c930: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000c940: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-0000c950: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000c960: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
-0000c970: 7468 3134 3536 372d 332d 322d 352d 342d  th14567-3-2-5-4-
-0000c980: 332d 382d 3022 0a20 2020 2020 2020 6378  3-8-0".       cx
-0000c990: 3d22 3136 392e 3335 3735 3622 0a20 2020  ="169.35756".   
-0000c9a0: 2020 2020 6379 3d22 3133 322e 3932 3531      cy="132.9251
-0000c9b0: 3722 0a20 2020 2020 2020 696e 6b73 6361  7".       inksca
-0000c9c0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000c9d0: 7465 722d 783d 2237 2e31 3636 3231 3136  ter-x="7.1662116
-0000c9e0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000c9f0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000ca00: 6572 2d79 3d22 2d31 352e 3339 3937 3531  er-y="-15.399751
-0000ca10: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000ca20: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000ca30: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000ca40: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000ca50: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
-0000ca60: 7263 6c65 0a20 2020 2020 2020 723d 2230  rcle.       r="0
-0000ca70: 2e30 3734 3036 3737 3739 220a 2020 2020  .074067779".    
-0000ca80: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000ca90: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
-0000caa0: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
-0000cab0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000cac0: 6b65 2d77 6964 7468 3a30 2e31 3332 3239  ke-width:0.13229
-0000cad0: 323b 7374 726f 6b65 2d6d 6974 6572 6c69  2;stroke-miterli
-0000cae0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-0000caf0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-0000cb00: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-0000cb10: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000cb20: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-0000cb30: 6831 3435 3637 2d32 2d38 2d36 2d37 2d38  h14567-2-8-6-7-8
-0000cb40: 2d32 2d32 220a 2020 2020 2020 2063 783d  -2-2".       cx=
-0000cb50: 2231 3638 2e36 3934 3437 220a 2020 2020  "168.69447".    
-0000cb60: 2020 2063 793d 2231 3333 2e36 3637 3322     cy="133.6673"
-0000cb70: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000cb80: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000cb90: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000cba0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000cbb0: 3330 3022 202f 3e0a 2020 2020 3c63 6972  300" />.    <cir
-0000cbc0: 636c 650a 2020 2020 2020 2072 3d22 302e  cle.       r="0.
-0000cbd0: 3134 3037 3931 3935 220a 2020 2020 2020  14079195".      
-0000cbe0: 2073 7479 6c65 3d22 6669 6c6c 3a23 6564   style="fill:#ed
-0000cbf0: 6630 6663 3b66 696c 6c2d 6f70 6163 6974  f0fc;fill-opacit
-0000cc00: 793a 302e 3939 3034 3436 3b73 7472 6f6b  y:0.990446;strok
-0000cc10: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000cc20: 2d77 6964 7468 3a30 2e31 3332 3239 323b  -width:0.132292;
-0000cc30: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-0000cc40: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-0000cc50: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-0000cc60: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-0000cc70: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000cc80: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000cc90: 3435 3637 2d32 2d37 2d30 2d39 2d30 2d35  4567-2-7-0-9-0-5
-0000cca0: 2d31 220a 2020 2020 2020 2063 783d 2231  -1".       cx="1
-0000ccb0: 3731 2e36 3134 3639 220a 2020 2020 2020  71.61469".      
-0000ccc0: 2063 793d 2231 3333 2e33 3939 3433 220a   cy="133.39943".
-0000ccd0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000cce0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000ccf0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000cd00: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-0000cd10: 3030 2220 2f3e 0a20 2020 203c 7265 6374  00" />.    <rect
-0000cd20: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-0000cd30: 696c 6c3a 2362 3362 3362 333b 6669 6c6c  ill:#b3b3b3;fill
-0000cd40: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000cd50: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-0000cd60: 6474 683a 303b 7374 726f 6b65 2d6d 6974  dth:0;stroke-mit
-0000cd70: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000cd80: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000cd90: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-0000cda0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-0000cdb0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-0000cdc0: 2272 6563 7431 3530 3734 2d30 2d39 2d32  "rect15074-0-9-2
-0000cdd0: 2d39 2d34 2d32 220a 2020 2020 2020 2077  -9-4-2".       w
-0000cde0: 6964 7468 3d22 342e 3233 3333 3332 3622  idth="4.2333326"
-0000cdf0: 0a20 2020 2020 2020 6865 6967 6874 3d22  .       height="
-0000ce00: 342e 3233 3333 3332 3622 0a20 2020 2020  4.2333326".     
-0000ce10: 2020 783d 2231 3637 2e39 3934 3439 220a    x="167.99449".
-0000ce20: 2020 2020 2020 2079 3d22 3133 372e 3038         y="137.08
-0000ce30: 3031 3422 0a20 2020 2020 2020 696e 6b73  014".       inks
-0000ce40: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-0000ce50: 3d22 3936 220a 2020 2020 2020 2069 6e6b  ="96".       ink
-0000ce60: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000ce70: 693d 2239 3622 0a20 2020 2020 2020 696e  i="96".       in
-0000ce80: 6b73 6361 7065 3a65 7870 6f72 742d 6669  kscape:export-fi
-0000ce90: 6c65 6e61 6d65 3d22 6963 6f6e 3136 2e70  lename="icon16.p
-0000cea0: 6e67 2220 2f3e 0a20 2020 203c 7061 7468  ng" />.    <path
-0000ceb0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-0000cec0: 696c 6c3a 2333 6534 6237 373b 6669 6c6c  ill:#3e4b77;fill
-0000ced0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000cee0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000cef0: 2d77 6964 7468 3a30 3b73 7472 6f6b 652d  -width:0;stroke-
-0000cf00: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-0000cf10: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-0000cf20: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-0000cf30: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000cf40: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000cf50: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-0000cf60: 2020 2020 2020 643d 226d 2031 3638 2e31        d="m 168.1
-0000cf70: 3732 3939 2c31 3338 2e34 3739 3832 2031  7299,138.47982 1
-0000cf80: 2e34 3337 3438 2c2d 302e 3036 3533 2030  .43748,-0.0653 0
-0000cf90: 2e39 3434 3437 2c2d 312e 3035 3133 3820  .94447,-1.05138 
-0000cfa0: 6320 2d31 2e31 3839 3833 2c30 2e38 3030  c -1.18983,0.800
-0000cfb0: 3138 202d 312e 3735 3832 372c 302e 3932  18 -1.75827,0.92
-0000cfc0: 3836 202d 322e 3338 3139 352c 312e 3131  86 -2.38195,1.11
-0000cfd0: 3637 3220 7a22 0a20 2020 2020 2020 6964  672 z".       id
-0000cfe0: 3d22 7061 7468 3134 3534 372d 312d 372d  ="path14547-1-7-
-0000cff0: 382d 352d 302d 3322 0a20 2020 2020 2020  8-5-0-3".       
-0000d000: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000d010: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000d020: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-0000d030: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-0000d040: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000d050: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000d060: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000d070: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000d080: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
-0000d090: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-0000d0a0: 2266 696c 6c3a 2330 3630 3530 383b 6669  "fill:#060508;fi
-0000d0b0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-0000d0c0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000d0d0: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
-0000d0e0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-0000d0f0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-0000d100: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-0000d110: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000d120: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000d130: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000d140: 0a20 2020 2020 2020 643d 226d 2031 3639  .       d="m 169
-0000d150: 2e36 3130 3437 2c31 3338 2e34 3134 3532  .61047,138.41452
-0000d160: 2032 2e32 3932 3835 2c30 2e34 3339 3532   2.29285,0.43952
-0000d170: 2063 202d 302e 3635 3034 342c 2d30 2e33   c -0.65044,-0.3
-0000d180: 3433 3835 202d 312e 3032 3731 2c2d 302e  4385 -1.0271,-0.
-0000d190: 3839 3633 202d 312e 3334 3833 382c 2d31  8963 -1.34838,-1
-0000d1a0: 2e34 3930 3934 207a 220a 2020 2020 2020  .49094 z".      
-0000d1b0: 2069 643d 2270 6174 6831 3435 3531 2d30   id="path14551-0
-0000d1c0: 2d33 2d39 2d39 2d34 2d39 220a 2020 2020  -3-9-9-4-9".    
-0000d1d0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-0000d1e0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-0000d1f0: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
-0000d200: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-0000d210: 6363 6322 0a20 2020 2020 2020 696e 6b73  ccc".       inks
-0000d220: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-0000d230: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
-0000d240: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-0000d250: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-0000d260: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-0000d270: 6c65 3d22 6669 6c6c 3a23 3237 3337 3733  le="fill:#273773
-0000d280: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000d290: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000d2a0: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
-0000d2b0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-0000d2c0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-0000d2d0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-0000d2e0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000d2f0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000d300: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-0000d310: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
-0000d320: 3136 382e 3137 3239 392c 3133 382e 3437  168.17299,138.47
-0000d330: 3938 3220 6320 302e 3331 3633 322c 302e  982 c 0.31632,0.
-0000d340: 3138 3134 3720 302e 3636 3530 392c 302e  18147 0.66509,0.
-0000d350: 3333 3739 3720 302e 3738 3430 382c 302e  33797 0.78408,0.
-0000d360: 3637 3132 3220 6c20 302e 3635 3334 2c2d  67122 l 0.6534,-
-0000d370: 302e 3733 3635 3620 7a22 0a20 2020 2020  0.73656 z".     
-0000d380: 2020 6964 3d22 7061 7468 3134 3535 332d    id="path14553-
-0000d390: 332d 322d 322d 312d 332d 3822 0a20 2020  3-2-2-1-3-8".   
-0000d3a0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-0000d3b0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-0000d3c0: 3d22 3022 0a20 2020 2020 2020 736f 6469  ="0".       sodi
-0000d3d0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-0000d3e0: 6363 6363 220a 2020 2020 2020 2069 6e6b  cccc".       ink
-0000d3f0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-0000d400: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-0000d410: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-0000d420: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-0000d430: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-0000d440: 796c 653d 2266 696c 6c3a 2331 3432 3637  yle="fill:#14267
-0000d450: 323b 6669 6c6c 2d6f 7061 6369 7479 3a31  2;fill-opacity:1
-0000d460: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000d470: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-0000d480: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000d490: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000d4a0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000d4b0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000d4c0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000d4d0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-0000d4e0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-0000d4f0: 2031 3638 2e39 3537 3037 2c31 3339 2e31   168.95707,139.1
-0000d500: 3531 3034 2032 2e39 3436 3235 2c2d 302e  5104 2.94625,-0.
-0000d510: 3239 3720 2d32 2e32 3932 3835 2c2d 302e  297 -2.29285,-0.
-0000d520: 3433 3935 3620 7a22 0a20 2020 2020 2020  43956 z".       
-0000d530: 6964 3d22 7061 7468 3134 3535 352d 342d  id="path14555-4-
-0000d540: 312d 362d 372d 322d 3222 0a20 2020 2020  1-6-7-2-2".     
-0000d550: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000d560: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000d570: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000d580: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000d590: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000d5a0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000d5b0: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-0000d5c0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-0000d5d0: 3d22 6669 6c6c 3a23 3534 3636 3863 3b66  ="fill:#54668c;f
-0000d5e0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000d5f0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000d600: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
-0000d610: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-0000d620: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-0000d630: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-0000d640: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000d650: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000d660: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000d670: 220a 2020 2020 2020 2064 3d22 6d20 3136  ".       d="m 16
-0000d680: 382e 3935 3730 372c 3133 392e 3135 3130  8.95707,139.1510
-0000d690: 3420 6320 302e 3033 3832 2c30 2e33 3239  4 c 0.0382,0.329
-0000d6a0: 3338 202d 302e 3039 342c 302e 3533 3730  38 -0.094,0.5370
-0000d6b0: 3320 2d30 2e31 3534 3434 2c30 2e37 3935  3 -0.15444,0.795
-0000d6c0: 3937 206c 2033 2e31 3030 3639 2c2d 312e  97 l 3.10069,-1.
-0000d6d0: 3039 3239 3720 7a22 0a20 2020 2020 2020  09297 z".       
-0000d6e0: 6964 3d22 7061 7468 3134 3535 392d 332d  id="path14559-3-
-0000d6f0: 342d 322d 342d 342d 3322 0a20 2020 2020  4-2-4-4-3".     
-0000d700: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000d710: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000d720: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-0000d730: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-0000d740: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
-0000d750: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000d760: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000d770: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000d780: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000d790: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000d7a0: 653d 2266 696c 6c3a 2330 3831 3036 393b  e="fill:#081069;
-0000d7b0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000d7c0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000d7d0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-0000d7e0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000d7f0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000d800: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000d810: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000d820: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000d830: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000d840: 3122 0a20 2020 2020 2020 643d 226d 2031  1".       d="m 1
-0000d850: 3638 2e38 3032 3633 2c31 3339 2e39 3437  68.80263,139.947
-0000d860: 3031 2031 2e32 3833 3035 2c30 2e31 3930  01 1.28305,0.190
-0000d870: 3038 2031 2e38 3137 3634 2c2d 312e 3238  08 1.81764,-1.28
-0000d880: 3330 3520 7a22 0a20 2020 2020 2020 6964  305 z".       id
-0000d890: 3d22 7061 7468 3134 3536 312d 392d 322d  ="path14561-9-2-
-0000d8a0: 322d 382d 302d 3122 0a20 2020 2020 2020  2-8-0-1".       
-0000d8b0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000d8c0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000d8d0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000d8e0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000d8f0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000d900: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000d910: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-0000d920: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-0000d930: 6669 6c6c 3a23 3037 3065 3262 3b66 696c  fill:#070e2b;fil
-0000d940: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000d950: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000d960: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-0000d970: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-0000d980: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-0000d990: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-0000d9a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-0000d9b0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-0000d9c0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000d9d0: 2020 2020 2020 2064 3d22 6d20 3137 302e         d="m 170.
-0000d9e0: 3038 3536 382c 3134 302e 3133 3730 3920  08568,140.13709 
-0000d9f0: 302e 3735 3433 382c 302e 3939 3139 3820  0.75438,0.99198 
-0000da00: 2d30 2e32 3739 3138 2c2d 312e 3333 3635  -0.27918,-1.3365
-0000da10: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-0000da20: 6174 6831 3435 3633 2d31 2d30 2d36 2d38  ath14563-1-0-6-8
-0000da30: 2d37 2d32 220a 2020 2020 2020 2069 6e6b  -7-2".       ink
-0000da40: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-0000da50: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-0000da60: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000da70: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000da80: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000da90: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-0000daa0: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
-0000dab0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000dac0: 6c3a 2330 3730 6532 623b 6669 6c6c 2d6f  l:#070e2b;fill-o
-0000dad0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-0000dae0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-0000daf0: 6964 7468 3a30 3b73 7472 6f6b 652d 6c69  idth:0;stroke-li
-0000db00: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-0000db10: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-0000db20: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000db30: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000db40: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000db50: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000db60: 2020 2020 643d 226d 2031 3730 2e30 3835      d="m 170.085
-0000db70: 3638 2c31 3430 2e31 3337 3039 2030 2e37  68,140.13709 0.7
-0000db80: 3534 3338 2c30 2e39 3931 3938 2063 2030  5438,0.99198 c 0
-0000db90: 2e31 3434 3532 2c2d 312e 3230 3134 3620  .14452,-1.20146 
-0000dba0: 302e 3635 3331 322c 2d31 2e36 3334 3320  0.65312,-1.6343 
-0000dbb0: 312e 3036 3332 362c 2d32 2e32 3735 3033  1.06326,-2.27503
-0000dbc0: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-0000dbd0: 6174 6831 3435 3635 2d39 2d35 2d39 2d37  ath14565-9-5-9-7
-0000dbe0: 2d37 2d33 220a 2020 2020 2020 2069 6e6b  -7-3".       ink
-0000dbf0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-0000dc00: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-0000dc10: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-0000dc20: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
-0000dc30: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000dc40: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000dc50: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000dc60: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000dc70: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
-0000dc80: 650a 2020 2020 2020 2073 7479 6c65 3d22  e.       style="
-0000dc90: 6669 6c6c 3a23 3037 3065 3262 3b66 696c  fill:#070e2b;fil
-0000dca0: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
-0000dcb0: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
-0000dcc0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-0000dcd0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000dce0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000dcf0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000dd00: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000dd10: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000dd20: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000dd30: 3134 3536 372d 362d 312d 392d 372d 372d  14567-6-1-9-7-7-
-0000dd40: 3522 0a20 2020 2020 2020 6378 3d22 3136  5".       cx="16
-0000dd50: 382e 3230 3335 3122 0a20 2020 2020 2020  8.20351".       
-0000dd60: 6379 3d22 3133 382e 3438 3133 3522 0a20  cy="138.48135". 
-0000dd70: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000dd80: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000dd90: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000dda0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000ddb0: 3022 0a20 2020 2020 2020 723d 2230 2e30  0".       r="0.0
-0000ddc0: 3734 3036 3737 3739 2220 2f3e 0a20 2020  74067779" />.   
-0000ddd0: 203c 6369 7263 6c65 0a20 2020 2020 2020   <circle.       
-0000dde0: 723d 2230 2e30 3734 3036 3737 3739 220a  r="0.074067779".
-0000ddf0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-0000de00: 6c6c 3a23 3235 3361 3764 3b66 696c 6c2d  ll:#253a7d;fill-
-0000de10: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-0000de20: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-0000de30: 7769 6474 683a 303b 7374 726f 6b65 2d6d  width:0;stroke-m
-0000de40: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000de50: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000de60: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-0000de70: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-0000de80: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-0000de90: 643d 2270 6174 6831 3435 3637 2d33 2d39  d="path14567-3-9
-0000dea0: 332d 312d 362d 392d 332d 3722 0a20 2020  3-1-6-9-3-7".   
-0000deb0: 2020 2020 6378 3d22 3136 382e 3739 3037      cx="168.7907
-0000dec0: 3322 0a20 2020 2020 2020 6379 3d22 3133  3".       cy="13
-0000ded0: 392e 3933 3132 3122 0a20 2020 2020 2020  9.93121".       
-0000dee0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-0000def0: 726d 2d63 656e 7465 722d 783d 2234 2e36  rm-center-x="4.6
-0000df00: 3433 3235 3636 220a 2020 2020 2020 2069  432566".       i
-0000df10: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-0000df20: 6d2d 6365 6e74 6572 2d79 3d22 2d39 2e39  m-center-y="-9.9
-0000df30: 3738 3036 3231 220a 2020 2020 2020 2069  780621".       i
-0000df40: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-0000df50: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-0000df60: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000df70: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-0000df80: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-0000df90: 2020 723d 2230 2e30 3734 3036 3737 3739    r="0.074067779
-0000dfa0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-0000dfb0: 6669 6c6c 3a23 6162 6161 3963 3b66 696c  fill:#abaa9c;fil
-0000dfc0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000dfd0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000dfe0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-0000dff0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000e000: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000e010: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-0000e020: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-0000e030: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000e040: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
-0000e050: 2d39 2d30 2d39 2d38 2d32 2d38 2d30 220a  -9-0-9-8-2-8-0".
-0000e060: 2020 2020 2020 2063 783d 2231 3730 2e31         cx="170.1
-0000e070: 3033 3733 220a 2020 2020 2020 2063 793d  0373".       cy=
-0000e080: 2231 3430 2e31 3333 3231 220a 2020 2020  "140.13321".    
-0000e090: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
-0000e0a0: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
-0000e0b0: 342e 3634 3332 3536 3622 0a20 2020 2020  4.6432566".     
-0000e0c0: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-0000e0d0: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
-0000e0e0: 392e 3937 3830 3632 3122 0a20 2020 2020  9.9780621".     
-0000e0f0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000e100: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-0000e110: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000e120: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-0000e130: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
-0000e140: 2020 2020 2072 3d22 302e 3131 3433 3133       r="0.114313
-0000e150: 3234 220a 2020 2020 2020 2073 7479 6c65  24".       style
-0000e160: 3d22 6669 6c6c 3a23 3131 3230 3636 3b66  ="fill:#112066;f
-0000e170: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000e180: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000e190: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
-0000e1a0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000e1b0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000e1c0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-0000e1d0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-0000e1e0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-0000e1f0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-0000e200: 2d33 2d32 2d35 2d34 2d33 2d38 2d30 2d37  -3-2-5-4-3-8-0-7
-0000e210: 220a 2020 2020 2020 2063 783d 2231 3639  ".       cx="169
-0000e220: 2e36 3230 3638 220a 2020 2020 2020 2063  .62068".       c
-0000e230: 793d 2231 3338 2e33 3938 3635 220a 2020  y="138.39865".  
-0000e240: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-0000e250: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
-0000e260: 3d22 372e 3136 3632 3131 3622 0a20 2020  ="7.1662116".   
-0000e270: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-0000e280: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
-0000e290: 222d 3135 2e33 3939 3735 3122 0a20 2020  "-15.399751".   
-0000e2a0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000e2b0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000e2c0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000e2d0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000e2e0: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-0000e2f0: 2020 2020 2020 2072 3d22 302e 3037 3430         r="0.0740
-0000e300: 3637 3737 3922 0a20 2020 2020 2020 7374  67779".       st
-0000e310: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
-0000e320: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
-0000e330: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
-0000e340: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000e350: 6474 683a 303b 7374 726f 6b65 2d6d 6974  dth:0;stroke-mit
-0000e360: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000e370: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000e380: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-0000e390: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-0000e3a0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-0000e3b0: 2270 6174 6831 3435 3637 2d32 2d38 2d36  "path14567-2-8-6
-0000e3c0: 2d37 2d38 2d32 2d32 2d36 220a 2020 2020  -7-8-2-2-6".    
-0000e3d0: 2020 2063 783d 2231 3638 2e39 3537 3622     cx="168.9576"
-0000e3e0: 0a20 2020 2020 2020 6379 3d22 3133 392e  .       cy="139.
-0000e3f0: 3134 3037 3822 0a20 2020 2020 2020 696e  14078".       in
-0000e400: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000e410: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000e420: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000e430: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000e440: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-0000e450: 2072 3d22 302e 3134 3037 3931 3935 220a   r="0.14079195".
-0000e460: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-0000e470: 6c6c 3a23 6564 6630 6663 3b66 696c 6c2d  ll:#edf0fc;fill-
-0000e480: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
-0000e490: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000e4a0: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-0000e4b0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000e4c0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-0000e4d0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-0000e4e0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-0000e4f0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-0000e500: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000e510: 3536 372d 322d 372d 302d 392d 302d 352d  567-2-7-0-9-0-5-
-0000e520: 312d 3122 0a20 2020 2020 2020 6378 3d22  1-1".       cx="
-0000e530: 3137 312e 3837 3738 3122 0a20 2020 2020  171.87781".     
-0000e540: 2020 6379 3d22 3133 382e 3837 3239 3122    cy="138.87291"
-0000e550: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000e560: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000e570: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000e580: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000e590: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-0000e5a0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-0000e5b0: 6669 6c6c 3a6e 6f6e 653b 6669 6c6c 2d72  fill:none;fill-r
-0000e5c0: 756c 653a 6576 656e 6f64 643b 7374 726f  ule:evenodd;stro
-0000e5d0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000e5e0: 652d 7769 6474 683a 302e 3133 3232 3932  e-width:0.132292
-0000e5f0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000e600: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000e610: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000e620: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000e630: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000e640: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000e650: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-0000e660: 226d 2031 3638 2e31 3732 3939 2c31 3338  "m 168.17299,138
-0000e670: 2e34 3739 3832 2063 2030 2e38 3839 3438  .47982 c 0.88948
-0000e680: 2c2d 302e 3138 3132 3320 312e 3634 3634  ,-0.18123 1.6464
-0000e690: 332c 2d30 2e36 3237 3532 2032 2e33 3831  3,-0.62752 2.381
-0000e6a0: 3935 2c2d 312e 3131 3636 3820 302e 3333  95,-1.11668 0.33
-0000e6b0: 3234 362c 302e 3630 3432 3120 302e 3635  246,0.60421 0.65
-0000e6c0: 322c 312e 3232 3032 3720 312e 3334 3833  2,1.22027 1.3483
-0000e6d0: 382c 312e 3439 3039 202d 302e 3432 3232  8,1.4909 -0.4222
-0000e6e0: 352c 302e 3537 3536 3520 2d30 2e38 3432  5,0.57565 -0.842
-0000e6f0: 3537 2c31 2e31 3536 3531 202d 312e 3036  57,1.15651 -1.06
-0000e700: 3332 362c 322e 3237 3530 3320 6c20 2d30  326,2.27503 l -0
-0000e710: 2e37 3534 3338 2c2d 302e 3939 3139 3820  .75438,-0.99198 
-0000e720: 2d31 2e32 3833 3035 2c2d 302e 3139 3030  -1.28305,-0.1900
-0000e730: 3820 6320 302e 3133 3739 362c 2d30 2e33  8 c 0.13796,-0.3
-0000e740: 3038 3536 2030 2e32 3033 3335 2c2d 302e  0856 0.20335,-0.
-0000e750: 3538 3038 3420 302e 3135 3434 342c 2d30  58084 0.15444,-0
-0000e760: 2e37 3935 3937 202d 302e 3230 3137 342c  .79597 -0.20174,
-0000e770: 2d30 2e32 3533 3535 202d 302e 3435 3736  -0.25355 -0.4576
-0000e780: 362c 2d30 2e34 3830 3031 202d 302e 3738  6,-0.48001 -0.78
-0000e790: 3430 382c 2d30 2e36 3731 3232 207a 220a  408,-0.67122 z".
-0000e7a0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000e7b0: 3330 3322 0a20 2020 2020 2020 736f 6469  303".       sodi
-0000e7c0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-0000e7d0: 6363 6363 6363 6363 2220 2f3e 0a20 2020  cccccccc" />.   
-0000e7e0: 203c 670a 2020 2020 2020 2069 643d 2267   <g.       id="g
-0000e7f0: 3133 3831 220a 2020 2020 2020 2074 7261  1381".       tra
-0000e800: 6e73 666f 726d 3d22 6d61 7472 6978 2831  nsform="matrix(1
-0000e810: 2e39 3938 3036 3431 2c30 2c30 2c31 2e39  .9980641,0,0,1.9
-0000e820: 3938 3036 3431 2c2d 3135 342e 3938 3136  980641,-154.9816
-0000e830: 312c 2d31 3434 2e38 3334 3737 2922 3e0a  1,-144.83477)">.
-0000e840: 2020 2020 2020 3c72 6563 740a 2020 2020        <rect.    
-0000e850: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-0000e860: 3a23 6233 6233 6233 3b66 696c 6c2d 6f70  :#b3b3b3;fill-op
-0000e870: 6163 6974 793a 313b 7374 726f 6b65 3a6e  acity:1;stroke:n
-0000e880: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
-0000e890: 3a30 3b73 7472 6f6b 652d 6d69 7465 726c  :0;stroke-miterl
-0000e8a0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000e8b0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000e8c0: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-0000e8d0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000e8e0: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
-0000e8f0: 7265 6374 3135 3037 342d 302d 392d 322d  rect15074-0-9-2-
-0000e900: 392d 342d 322d 3522 0a20 2020 2020 2020  9-4-2-5".       
-0000e910: 2020 7769 6474 683d 2234 2e32 3333 3333    width="4.23333
-0000e920: 3236 220a 2020 2020 2020 2020 2068 6569  26".         hei
-0000e930: 6768 743d 2234 2e32 3333 3333 3236 220a  ght="4.2333326".
-0000e940: 2020 2020 2020 2020 2078 3d22 3135 332e           x="153.
-0000e950: 3937 3431 3722 0a20 2020 2020 2020 2020  97417".         
-0000e960: 793d 2231 3433 2e38 3530 3422 0a20 2020  y="143.8504".   
-0000e970: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000e980: 7870 6f72 742d 7864 7069 3d22 3936 2e30  xport-xdpi="96.0
-0000e990: 3839 3939 3622 0a20 2020 2020 2020 2020  89996".         
-0000e9a0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000e9b0: 7964 7069 3d22 3936 2e30 3839 3939 3622  ydpi="96.089996"
-0000e9c0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-0000e9d0: 7065 3a65 7870 6f72 742d 6669 6c65 6e61  pe:export-filena
-0000e9e0: 6d65 3d22 6963 6f6e 3332 2e70 6e67 2220  me="icon32.png" 
-0000e9f0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
-0000ea00: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-0000ea10: 696c 6c3a 2333 6534 6237 373b 6669 6c6c  ill:#3e4b77;fill
-0000ea20: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000ea30: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000ea40: 2d77 6964 7468 3a30 3b73 7472 6f6b 652d  -width:0;stroke-
-0000ea50: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-0000ea60: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-0000ea70: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-0000ea80: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000ea90: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000eaa0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-0000eab0: 2020 2020 2020 2020 643d 226d 2031 3534          d="m 154
-0000eac0: 2e31 3532 3636 2c31 3435 2e32 3530 3038  .15266,145.25008
-0000ead0: 2031 2e34 3337 3438 2c2d 302e 3036 3533   1.43748,-0.0653
-0000eae0: 2030 2e39 3434 3437 2c2d 312e 3035 3133   0.94447,-1.0513
-0000eaf0: 3820 6320 2d31 2e31 3839 3833 2c30 2e38  8 c -1.18983,0.8
-0000eb00: 3030 3138 202d 312e 3735 3832 372c 302e  0018 -1.75827,0.
-0000eb10: 3932 3836 202d 322e 3338 3139 352c 312e  9286 -2.38195,1.
-0000eb20: 3131 3637 3220 7a22 0a20 2020 2020 2020  11672 z".       
-0000eb30: 2020 6964 3d22 7061 7468 3134 3534 372d    id="path14547-
-0000eb40: 312d 372d 382d 352d 302d 332d 3422 0a20  1-7-8-5-0-3-4". 
-0000eb50: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-0000eb60: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-0000eb70: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-0000eb80: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-0000eb90: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
-0000eba0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000ebb0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000ebc0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-0000ebd0: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-0000ebe0: 3030 2220 2f3e 0a20 2020 2020 203c 7061  00" />.      <pa
-0000ebf0: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
-0000ec00: 653d 2266 696c 6c3a 2330 3630 3530 383b  e="fill:#060508;
-0000ec10: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000ec20: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000ec30: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-0000ec40: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000ec50: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000ec60: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000ec70: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000ec80: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000ec90: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000eca0: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
-0000ecb0: 2031 3535 2e35 3930 3134 2c31 3435 2e31   155.59014,145.1
-0000ecc0: 3834 3738 2032 2e32 3932 3835 2c30 2e34  8478 2.29285,0.4
-0000ecd0: 3339 3532 2063 202d 302e 3635 3034 342c  3952 c -0.65044,
-0000ece0: 2d30 2e33 3433 3835 202d 312e 3032 3731  -0.34385 -1.0271
-0000ecf0: 2c2d 302e 3839 3633 202d 312e 3334 3833  ,-0.8963 -1.3483
-0000ed00: 382c 2d31 2e34 3930 3934 207a 220a 2020  8,-1.49094 z".  
-0000ed10: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000ed20: 3435 3531 2d30 2d33 2d39 2d39 2d34 2d39  4551-0-3-9-9-4-9
-0000ed30: 2d30 220a 2020 2020 2020 2020 2069 6e6b  -0".         ink
-0000ed40: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-0000ed50: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-0000ed60: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-0000ed70: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-0000ed80: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-0000ed90: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000eda0: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-0000edb0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-0000edc0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-0000edd0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-0000ede0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3237   style="fill:#27
-0000edf0: 3337 3733 3b66 696c 6c2d 6f70 6163 6974  3773;fill-opacit
-0000ee00: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-0000ee10: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-0000ee20: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
-0000ee30: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-0000ee40: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-0000ee50: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000ee60: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000ee70: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-0000ee80: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-0000ee90: 2064 3d22 6d20 3135 342e 3135 3236 362c   d="m 154.15266,
-0000eea0: 3134 352e 3235 3030 3820 6320 302e 3331  145.25008 c 0.31
-0000eeb0: 3633 322c 302e 3138 3134 3720 302e 3636  632,0.18147 0.66
-0000eec0: 3530 392c 302e 3333 3739 3720 302e 3738  509,0.33797 0.78
-0000eed0: 3430 382c 302e 3637 3132 3220 6c20 302e  408,0.67122 l 0.
-0000eee0: 3635 3334 2c2d 302e 3733 3635 3620 7a22  6534,-0.73656 z"
-0000eef0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-0000ef00: 7468 3134 3535 332d 332d 322d 322d 312d  th14553-3-2-2-1-
-0000ef10: 332d 382d 3922 0a20 2020 2020 2020 2020  3-8-9".         
-0000ef20: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000ef30: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000ef40: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-0000ef50: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-0000ef60: 6363 220a 2020 2020 2020 2020 2069 6e6b  cc".         ink
-0000ef70: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-0000ef80: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
-0000ef90: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000efa0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-0000efb0: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
-0000efc0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-0000efd0: 2331 3432 3637 323b 6669 6c6c 2d6f 7061  #142672;fill-opa
-0000efe0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-0000eff0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-0000f000: 7468 3a30 3b73 7472 6f6b 652d 6c69 6e65  th:0;stroke-line
-0000f010: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-0000f020: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-0000f030: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000f040: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-0000f050: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-0000f060: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-0000f070: 2020 2020 643d 226d 2031 3534 2e39 3336      d="m 154.936
-0000f080: 3734 2c31 3435 2e39 3231 3320 322e 3934  74,145.9213 2.94
-0000f090: 3632 352c 2d30 2e32 3937 202d 322e 3239  625,-0.297 -2.29
-0000f0a0: 3238 352c 2d30 2e34 3339 3536 207a 220a  285,-0.43956 z".
-0000f0b0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-0000f0c0: 6831 3435 3535 2d34 2d31 2d36 2d37 2d32  h14555-4-1-6-7-2
-0000f0d0: 2d32 2d33 220a 2020 2020 2020 2020 2069  -2-3".         i
-0000f0e0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-0000f0f0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-0000f100: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-0000f110: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000f120: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
-0000f130: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000f140: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
-0000f150: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-0000f160: 7374 796c 653d 2266 696c 6c3a 2335 3436  style="fill:#546
-0000f170: 3638 633b 6669 6c6c 2d6f 7061 6369 7479  68c;fill-opacity
-0000f180: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-0000f190: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-0000f1a0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000f1b0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000f1c0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000f1d0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000f1e0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000f1f0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000f200: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-0000f210: 643d 226d 2031 3534 2e39 3336 3734 2c31  d="m 154.93674,1
-0000f220: 3435 2e39 3231 3320 6320 302e 3033 3832  45.9213 c 0.0382
-0000f230: 2c30 2e33 3239 3338 202d 302e 3039 342c  ,0.32938 -0.094,
-0000f240: 302e 3533 3730 3320 2d30 2e31 3534 3434  0.53703 -0.15444
-0000f250: 2c30 2e37 3935 3937 206c 2033 2e31 3030  ,0.79597 l 3.100
-0000f260: 3639 2c2d 312e 3039 3239 3720 7a22 0a20  69,-1.09297 z". 
-0000f270: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-0000f280: 3134 3535 392d 332d 342d 322d 342d 342d  14559-3-4-2-4-4-
-0000f290: 332d 3522 0a20 2020 2020 2020 2020 696e  3-5".         in
-0000f2a0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-0000f2b0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-0000f2c0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-0000f2d0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-0000f2e0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000f2f0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000f300: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
-0000f310: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-0000f320: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-0000f330: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-0000f340: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-0000f350: 3831 3036 393b 6669 6c6c 2d6f 7061 6369  81069;fill-opaci
-0000f360: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-0000f370: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-0000f380: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
-0000f390: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-0000f3a0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-0000f3b0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000f3c0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000f3d0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-0000f3e0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000f3f0: 2020 643d 226d 2031 3534 2e37 3832 332c    d="m 154.7823,
-0000f400: 3134 362e 3731 3732 3720 312e 3238 3330  146.71727 1.2830
-0000f410: 352c 302e 3139 3030 3820 312e 3831 3736  5,0.19008 1.8176
-0000f420: 342c 2d31 2e32 3833 3035 207a 220a 2020  4,-1.28305 z".  
-0000f430: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000f440: 3435 3631 2d39 2d32 2d32 2d38 2d30 2d31  4561-9-2-2-8-0-1
-0000f450: 2d37 220a 2020 2020 2020 2020 2069 6e6b  -7".         ink
-0000f460: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-0000f470: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-0000f480: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000f490: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000f4a0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000f4b0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000f4c0: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-0000f4d0: 7061 7468 0a20 2020 2020 2020 2020 7374  path.         st
-0000f4e0: 796c 653d 2266 696c 6c3a 2330 3730 6532  yle="fill:#070e2
-0000f4f0: 623b 6669 6c6c 2d6f 7061 6369 7479 3a31  b;fill-opacity:1
-0000f500: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000f510: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-0000f520: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000f530: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000f540: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000f550: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000f560: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000f570: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-0000f580: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-0000f590: 226d 2031 3536 2e30 3635 3335 2c31 3436  "m 156.06535,146
-0000f5a0: 2e39 3037 3335 2030 2e37 3534 3338 2c30  .90735 0.75438,0
-0000f5b0: 2e39 3931 3938 202d 302e 3237 3931 382c  .99198 -0.27918,
-0000f5c0: 2d31 2e33 3336 3520 7a22 0a20 2020 2020  -1.3365 z".     
-0000f5d0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-0000f5e0: 332d 312d 302d 362d 382d 372d 322d 3222  3-1-0-6-8-7-2-2"
-0000f5f0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-0000f600: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-0000f610: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-0000f620: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000f630: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000f640: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-0000f650: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000f660: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-0000f670: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-0000f680: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
-0000f690: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000f6a0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000f6b0: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
-0000f6c0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-0000f6d0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-0000f6e0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-0000f6f0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000f700: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000f710: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000f720: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
-0000f730: 3135 362e 3036 3533 352c 3134 362e 3930  156.06535,146.90
-0000f740: 3733 3520 302e 3735 3433 382c 302e 3939  735 0.75438,0.99
-0000f750: 3139 3820 6320 302e 3134 3435 322c 2d31  198 c 0.14452,-1
-0000f760: 2e32 3031 3436 2030 2e36 3533 3132 2c2d  .20146 0.65312,-
-0000f770: 312e 3633 3433 2031 2e30 3633 3236 2c2d  1.6343 1.06326,-
-0000f780: 322e 3237 3530 3320 7a22 0a20 2020 2020  2.27503 z".     
-0000f790: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-0000f7a0: 352d 392d 352d 392d 372d 372d 332d 3422  5-9-5-9-7-7-3-4"
-0000f7b0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-0000f7c0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-0000f7d0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-0000f7e0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-0000f7f0: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
-0000f800: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000f810: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000f820: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000f830: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000f840: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-0000f850: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
-0000f860: 7374 796c 653d 2266 696c 6c3a 2330 3730  style="fill:#070
-0000f870: 6532 623b 6669 6c6c 2d6f 7061 6369 7479  e2b;fill-opacity
-0000f880: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
-0000f890: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-0000f8a0: 7769 6474 683a 303b 7374 726f 6b65 2d6d  width:0;stroke-m
-0000f8b0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000f8c0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000f8d0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-0000f8e0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-0000f8f0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-0000f900: 2069 643d 2270 6174 6831 3435 3637 2d36   id="path14567-6
-0000f910: 2d31 2d39 2d37 2d37 2d35 2d39 220a 2020  -1-9-7-7-5-9".  
-0000f920: 2020 2020 2020 2063 783d 2231 3534 2e31         cx="154.1
-0000f930: 3833 3138 220a 2020 2020 2020 2020 2063  8318".         c
-0000f940: 793d 2231 3435 2e32 3531 3632 220a 2020  y="145.25162".  
-0000f950: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000f960: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000f970: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000f980: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000f990: 2233 3030 220a 2020 2020 2020 2020 2072  "300".         r
-0000f9a0: 3d22 302e 3037 3430 3637 3737 3922 202f  ="0.074067779" /
-0000f9b0: 3e0a 2020 2020 2020 3c63 6972 636c 650a  >.      <circle.
-0000f9c0: 2020 2020 2020 2020 2072 3d22 302e 3037           r="0.07
-0000f9d0: 3430 3637 3737 3922 0a20 2020 2020 2020  4067779".       
-0000f9e0: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
-0000f9f0: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
-0000fa00: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-0000fa10: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-0000fa20: 3a30 3b73 7472 6f6b 652d 6d69 7465 726c  :0;stroke-miterl
-0000fa30: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000fa40: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000fa50: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-0000fa60: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000fa70: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
-0000fa80: 7061 7468 3134 3536 372d 332d 3933 2d31  path14567-3-93-1
-0000fa90: 2d36 2d39 2d33 2d37 2d38 220a 2020 2020  -6-9-3-7-8".    
-0000faa0: 2020 2020 2063 783d 2231 3534 2e37 3730       cx="154.770
-0000fab0: 3422 0a20 2020 2020 2020 2020 6379 3d22  4".         cy="
-0000fac0: 3134 362e 3730 3134 3822 0a20 2020 2020  146.70148".     
-0000fad0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-0000fae0: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
-0000faf0: 2234 2e36 3433 3235 3636 220a 2020 2020  "4.6432566".    
-0000fb00: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-0000fb10: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-0000fb20: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
-0000fb30: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000fb40: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000fb50: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000fb60: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000fb70: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-0000fb80: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
-0000fb90: 723d 2230 2e30 3734 3036 3737 3739 220a  r="0.074067779".
-0000fba0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-0000fbb0: 6669 6c6c 3a23 6162 6161 3963 3b66 696c  fill:#abaa9c;fil
-0000fbc0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000fbd0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000fbe0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-0000fbf0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000fc00: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000fc10: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-0000fc20: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-0000fc30: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000fc40: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-0000fc50: 2d33 2d39 2d30 2d39 2d38 2d32 2d38 2d30  -3-9-0-9-8-2-8-0
-0000fc60: 2d35 220a 2020 2020 2020 2020 2063 783d  -5".         cx=
-0000fc70: 2231 3536 2e30 3833 3422 0a20 2020 2020  "156.0834".     
-0000fc80: 2020 2020 6379 3d22 3134 362e 3930 3334      cy="146.9034
-0000fc90: 3722 0a20 2020 2020 2020 2020 696e 6b73  7".         inks
-0000fca0: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
-0000fcb0: 656e 7465 722d 783d 2234 2e36 3433 3235  enter-x="4.64325
-0000fcc0: 3636 220a 2020 2020 2020 2020 2069 6e6b  66".         ink
-0000fcd0: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
-0000fce0: 6365 6e74 6572 2d79 3d22 2d39 2e39 3738  center-y="-9.978
-0000fcf0: 3036 3231 220a 2020 2020 2020 2020 2069  0621".         i
-0000fd00: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-0000fd10: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-0000fd20: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000fd30: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-0000fd40: 0a20 2020 2020 203c 6369 7263 6c65 0a20  .      <circle. 
-0000fd50: 2020 2020 2020 2020 723d 2230 2e31 3134          r="0.114
-0000fd60: 3331 3332 3422 0a20 2020 2020 2020 2020  31324".         
-0000fd70: 7374 796c 653d 2266 696c 6c3a 2331 3132  style="fill:#112
-0000fd80: 3036 363b 6669 6c6c 2d6f 7061 6369 7479  066;fill-opacity
-0000fd90: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-0000fda0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-0000fdb0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000fdc0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000fdd0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000fde0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000fdf0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000fe00: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-0000fe10: 7468 3134 3536 372d 332d 322d 352d 342d  th14567-3-2-5-4-
-0000fe20: 332d 382d 302d 372d 3722 0a20 2020 2020  3-8-0-7-7".     
-0000fe30: 2020 2020 6378 3d22 3135 352e 3630 3033      cx="155.6003
-0000fe40: 3622 0a20 2020 2020 2020 2020 6379 3d22  6".         cy="
-0000fe50: 3134 352e 3136 3839 3122 0a20 2020 2020  145.16891".     
-0000fe60: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-0000fe70: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
-0000fe80: 2237 2e31 3636 3231 3136 220a 2020 2020  "7.1662116".    
-0000fe90: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-0000fea0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-0000feb0: 3d22 2d31 352e 3339 3937 3531 220a 2020  ="-15.399751".  
-0000fec0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000fed0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000fee0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000fef0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000ff00: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-0000ff10: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
-0000ff20: 723d 2230 2e30 3734 3036 3737 3739 220a  r="0.074067779".
-0000ff30: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-0000ff40: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
-0000ff50: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
-0000ff60: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
-0000ff70: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-0000ff80: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000ff90: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000ffa0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000ffb0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000ffc0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000ffd0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-0000ffe0: 7468 3134 3536 372d 322d 382d 362d 372d  th14567-2-8-6-7-
-0000fff0: 382d 322d 322d 362d 3922 0a20 2020 2020  8-2-2-6-9".     
-00010000: 2020 2020 6378 3d22 3135 342e 3933 3732      cx="154.9372
-00010010: 3722 0a20 2020 2020 2020 2020 6379 3d22  7".         cy="
-00010020: 3134 352e 3931 3130 3422 0a20 2020 2020  145.91104".     
-00010030: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00010040: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00010050: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00010060: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00010070: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
-00010080: 636c 650a 2020 2020 2020 2020 2072 3d22  cle.         r="
-00010090: 302e 3134 3037 3931 3935 220a 2020 2020  0.14079195".    
-000100a0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000100b0: 3a23 6564 6630 6663 3b66 696c 6c2d 6f70  :#edf0fc;fill-op
-000100c0: 6163 6974 793a 302e 3939 3034 3436 3b73  acity:0.990446;s
-000100d0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-000100e0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-000100f0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00010100: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00010110: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00010120: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-00010130: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00010140: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00010150: 3536 372d 322d 372d 302d 392d 302d 352d  567-2-7-0-9-0-5-
-00010160: 312d 312d 3322 0a20 2020 2020 2020 2020  1-1-3".         
-00010170: 6378 3d22 3135 372e 3835 3734 3822 0a20  cx="157.85748". 
-00010180: 2020 2020 2020 2020 6379 3d22 3134 352e          cy="145.
-00010190: 3634 3331 3722 0a20 2020 2020 2020 2020  64317".         
-000101a0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-000101b0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-000101c0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-000101d0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-000101e0: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
-000101f0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00010200: 6c6c 3a6e 6f6e 653b 6669 6c6c 2d72 756c  ll:none;fill-rul
-00010210: 653a 6576 656e 6f64 643b 7374 726f 6b65  e:evenodd;stroke
-00010220: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00010230: 7769 6474 683a 302e 3133 3232 3932 3b73  width:0.132292;s
-00010240: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00010250: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00010260: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00010270: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00010280: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00010290: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-000102a0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-000102b0: 226d 2031 3534 2e31 3532 3636 2c31 3435  "m 154.15266,145
-000102c0: 2e32 3530 3038 2063 2030 2e38 3839 3438  .25008 c 0.88948
-000102d0: 2c2d 302e 3138 3132 3320 312e 3634 3634  ,-0.18123 1.6464
-000102e0: 332c 2d30 2e36 3237 3532 2032 2e33 3831  3,-0.62752 2.381
-000102f0: 3935 2c2d 312e 3131 3636 3820 302e 3333  95,-1.11668 0.33
-00010300: 3234 362c 302e 3630 3432 3120 302e 3635  246,0.60421 0.65
-00010310: 322c 312e 3232 3032 3720 312e 3334 3833  2,1.22027 1.3483
-00010320: 382c 312e 3439 3039 202d 302e 3432 3232  8,1.4909 -0.4222
-00010330: 352c 302e 3537 3536 3520 2d30 2e38 3432  5,0.57565 -0.842
-00010340: 3537 2c31 2e31 3536 3531 202d 312e 3036  57,1.15651 -1.06
-00010350: 3332 362c 322e 3237 3530 3320 6c20 2d30  326,2.27503 l -0
-00010360: 2e37 3534 3338 2c2d 302e 3939 3139 3820  .75438,-0.99198 
-00010370: 2d31 2e32 3833 3035 2c2d 302e 3139 3030  -1.28305,-0.1900
-00010380: 3820 6320 302e 3133 3739 362c 2d30 2e33  8 c 0.13796,-0.3
-00010390: 3038 3536 2030 2e32 3033 3335 2c2d 302e  0856 0.20335,-0.
-000103a0: 3538 3038 3420 302e 3135 3434 342c 2d30  58084 0.15444,-0
-000103b0: 2e37 3935 3937 202d 302e 3230 3137 342c  .79597 -0.20174,
-000103c0: 2d30 2e32 3533 3535 202d 302e 3435 3736  -0.25355 -0.4576
-000103d0: 362c 2d30 2e34 3830 3031 202d 302e 3738  6,-0.48001 -0.78
-000103e0: 3430 382c 2d30 2e36 3731 3232 207a 220a  408,-0.67122 z".
-000103f0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00010400: 6831 3330 332d 3722 0a20 2020 2020 2020  h1303-7".       
-00010410: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-00010420: 7970 6573 3d22 6363 6363 6363 6363 2220  ypes="cccccccc" 
-00010430: 2f3e 0a20 2020 203c 2f67 3e0a 2020 2020  />.    </g>.    
-00010440: 3c67 0a20 2020 2020 2020 6964 3d22 6731  <g.       id="g1
-00010450: 3338 312d 3322 0a20 2020 2020 2020 7472  381-3".       tr
-00010460: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00010470: 332e 3939 3631 3238 322c 302c 302c 332e  3.9961282,0,0,3.
-00010480: 3939 3631 3238 322c 2d34 3838 2e35 3330  9961282,-488.530
-00010490: 3834 2c2d 3431 382e 3735 3037 3529 223e  84,-418.75075)">
-000104a0: 0a20 2020 2020 203c 7265 6374 0a20 2020  .      <rect.   
-000104b0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-000104c0: 6c3a 2362 3362 3362 333b 6669 6c6c 2d6f  l:#b3b3b3;fill-o
-000104d0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-000104e0: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
-000104f0: 683a 303b 7374 726f 6b65 2d6d 6974 6572  h:0;stroke-miter
-00010500: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00010510: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00010520: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-00010530: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-00010540: 3a31 220a 2020 2020 2020 2020 2069 643d  :1".         id=
-00010550: 2272 6563 7431 3530 3734 2d30 2d39 2d32  "rect15074-0-9-2
-00010560: 2d39 2d34 2d32 2d35 2d38 220a 2020 2020  -9-4-2-5-8".    
-00010570: 2020 2020 2077 6964 7468 3d22 342e 3233       width="4.23
-00010580: 3333 3332 3622 0a20 2020 2020 2020 2020  33326".         
-00010590: 6865 6967 6874 3d22 342e 3233 3333 3332  height="4.233332
-000105a0: 3622 0a20 2020 2020 2020 2020 783d 2231  6".         x="1
-000105b0: 3533 2e39 3734 3137 220a 2020 2020 2020  53.97417".      
-000105c0: 2020 2079 3d22 3134 332e 3835 3034 220a     y="143.8504".
-000105d0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-000105e0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-000105f0: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
-00010600: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-00010610: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
-00010620: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-00010630: 7374 796c 653d 2266 696c 6c3a 2333 6534  style="fill:#3e4
-00010640: 6237 373b 6669 6c6c 2d6f 7061 6369 7479  b77;fill-opacity
-00010650: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00010660: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-00010670: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00010680: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00010690: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-000106a0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-000106b0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-000106c0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-000106d0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-000106e0: 643d 226d 2031 3534 2e31 3532 3636 2c31  d="m 154.15266,1
-000106f0: 3435 2e32 3530 3038 2031 2e34 3337 3438  45.25008 1.43748
-00010700: 2c2d 302e 3036 3533 2030 2e39 3434 3437  ,-0.0653 0.94447
-00010710: 2c2d 312e 3035 3133 3820 6320 2d31 2e31  ,-1.05138 c -1.1
-00010720: 3839 3833 2c30 2e38 3030 3138 202d 312e  8983,0.80018 -1.
-00010730: 3735 3832 372c 302e 3932 3836 202d 322e  75827,0.9286 -2.
-00010740: 3338 3139 352c 312e 3131 3637 3220 7a22  38195,1.11672 z"
-00010750: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00010760: 7468 3134 3534 372d 312d 372d 382d 352d  th14547-1-7-8-5-
-00010770: 302d 332d 342d 3222 0a20 2020 2020 2020  0-3-4-2".       
-00010780: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00010790: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-000107a0: 3022 0a20 2020 2020 2020 2020 736f 6469  0".         sodi
-000107b0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-000107c0: 6363 6363 220a 2020 2020 2020 2020 2069  cccc".         i
-000107d0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-000107e0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-000107f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-00010800: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-00010810: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
-00010820: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00010830: 6c3a 2330 3630 3530 383b 6669 6c6c 2d6f  l:#060508;fill-o
-00010840: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00010850: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00010860: 6964 7468 3a30 3b73 7472 6f6b 652d 6c69  idth:0;stroke-li
-00010870: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00010880: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00010890: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-000108a0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-000108b0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000108c0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000108d0: 2020 2020 2020 643d 226d 2031 3535 2e35        d="m 155.5
-000108e0: 3930 3134 2c31 3435 2e31 3834 3738 2032  9014,145.18478 2
-000108f0: 2e32 3932 3835 2c30 2e34 3339 3532 2063  .29285,0.43952 c
-00010900: 202d 302e 3635 3034 342c 2d30 2e33 3433   -0.65044,-0.343
-00010910: 3835 202d 312e 3032 3731 2c2d 302e 3839  85 -1.0271,-0.89
-00010920: 3633 202d 312e 3334 3833 382c 2d31 2e34  63 -1.34838,-1.4
-00010930: 3930 3934 207a 220a 2020 2020 2020 2020  9094 z".        
-00010940: 2069 643d 2270 6174 6831 3435 3531 2d30   id="path14551-0
-00010950: 2d33 2d39 2d39 2d34 2d39 2d30 2d34 220a  -3-9-9-4-9-0-4".
-00010960: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00010970: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00010980: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-00010990: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-000109a0: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
-000109b0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-000109c0: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-000109d0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000109e0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-000109f0: 3330 3022 202f 3e0a 2020 2020 2020 3c70  300" />.      <p
-00010a00: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
-00010a10: 6c65 3d22 6669 6c6c 3a23 3237 3337 3733  le="fill:#273773
-00010a20: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00010a30: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00010a40: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
-00010a50: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00010a60: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00010a70: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-00010a80: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00010a90: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00010aa0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00010ab0: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
-00010ac0: 6d20 3135 342e 3135 3236 362c 3134 352e  m 154.15266,145.
-00010ad0: 3235 3030 3820 6320 302e 3331 3633 322c  25008 c 0.31632,
-00010ae0: 302e 3138 3134 3720 302e 3636 3530 392c  0.18147 0.66509,
-00010af0: 302e 3333 3739 3720 302e 3738 3430 382c  0.33797 0.78408,
-00010b00: 302e 3637 3132 3220 6c20 302e 3635 3334  0.67122 l 0.6534
-00010b10: 2c2d 302e 3733 3635 3620 7a22 0a20 2020  ,-0.73656 z".   
-00010b20: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00010b30: 3535 332d 332d 322d 322d 312d 332d 382d  553-3-2-2-1-3-8-
-00010b40: 392d 3122 0a20 2020 2020 2020 2020 696e  9-1".         in
-00010b50: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00010b60: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00010b70: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-00010b80: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-00010b90: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00010ba0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-00010bb0: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
-00010bc0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-00010bd0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-00010be0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00010bf0: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
-00010c00: 3432 3637 323b 6669 6c6c 2d6f 7061 6369  42672;fill-opaci
-00010c10: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00010c20: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00010c30: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
-00010c40: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00010c50: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00010c60: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00010c70: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00010c80: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00010c90: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00010ca0: 2020 643d 226d 2031 3534 2e39 3336 3734    d="m 154.93674
-00010cb0: 2c31 3435 2e39 3231 3320 322e 3934 3632  ,145.9213 2.9462
-00010cc0: 352c 2d30 2e32 3937 202d 322e 3239 3238  5,-0.297 -2.2928
-00010cd0: 352c 2d30 2e34 3339 3536 207a 220a 2020  5,-0.43956 z".  
-00010ce0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00010cf0: 3435 3535 2d34 2d31 2d36 2d37 2d32 2d32  4555-4-1-6-7-2-2
-00010d00: 2d33 2d39 220a 2020 2020 2020 2020 2069  -3-9".         i
-00010d10: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-00010d20: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-00010d30: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00010d40: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-00010d50: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
-00010d60: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-00010d70: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
-00010d80: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-00010d90: 7374 796c 653d 2266 696c 6c3a 2335 3436  style="fill:#546
-00010da0: 3638 633b 6669 6c6c 2d6f 7061 6369 7479  68c;fill-opacity
-00010db0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00010dc0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-00010dd0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00010de0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00010df0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00010e00: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00010e10: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00010e20: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00010e30: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00010e40: 643d 226d 2031 3534 2e39 3336 3734 2c31  d="m 154.93674,1
-00010e50: 3435 2e39 3231 3320 6320 302e 3033 3832  45.9213 c 0.0382
-00010e60: 2c30 2e33 3239 3338 202d 302e 3039 342c  ,0.32938 -0.094,
-00010e70: 302e 3533 3730 3320 2d30 2e31 3534 3434  0.53703 -0.15444
-00010e80: 2c30 2e37 3935 3937 206c 2033 2e31 3030  ,0.79597 l 3.100
-00010e90: 3639 2c2d 312e 3039 3239 3720 7a22 0a20  69,-1.09297 z". 
-00010ea0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00010eb0: 3134 3535 392d 332d 342d 322d 342d 342d  14559-3-4-2-4-4-
-00010ec0: 332d 352d 3622 0a20 2020 2020 2020 2020  3-5-6".         
-00010ed0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00010ee0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00010ef0: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-00010f00: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00010f10: 6363 220a 2020 2020 2020 2020 2069 6e6b  cc".         ink
-00010f20: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00010f30: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
-00010f40: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00010f50: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00010f60: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
-00010f70: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00010f80: 2330 3831 3036 393b 6669 6c6c 2d6f 7061  #081069;fill-opa
-00010f90: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00010fa0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00010fb0: 7468 3a30 3b73 7472 6f6b 652d 6c69 6e65  th:0;stroke-line
-00010fc0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00010fd0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00010fe0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00010ff0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00011000: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00011010: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00011020: 2020 2020 643d 226d 2031 3534 2e37 3832      d="m 154.782
-00011030: 332c 3134 362e 3731 3732 3720 312e 3238  3,146.71727 1.28
-00011040: 3330 352c 302e 3139 3030 3820 312e 3831  305,0.19008 1.81
-00011050: 3736 342c 2d31 2e32 3833 3035 207a 220a  764,-1.28305 z".
-00011060: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00011070: 6831 3435 3631 2d39 2d32 2d32 2d38 2d30  h14561-9-2-2-8-0
-00011080: 2d31 2d37 2d33 220a 2020 2020 2020 2020  -1-7-3".        
-00011090: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-000110a0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-000110b0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-000110c0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-000110d0: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
-000110e0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-000110f0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-00011100: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00011110: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-00011120: 3730 6532 623b 6669 6c6c 2d6f 7061 6369  70e2b;fill-opaci
-00011130: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00011140: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00011150: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
-00011160: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00011170: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00011180: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00011190: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000111a0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-000111b0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-000111c0: 2020 643d 226d 2031 3536 2e30 3635 3335    d="m 156.06535
-000111d0: 2c31 3436 2e39 3037 3335 2030 2e37 3534  ,146.90735 0.754
-000111e0: 3338 2c30 2e39 3931 3938 202d 302e 3237  38,0.99198 -0.27
-000111f0: 3931 382c 2d31 2e33 3336 3520 7a22 0a20  918,-1.3365 z". 
-00011200: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00011210: 3134 3536 332d 312d 302d 362d 382d 372d  14563-1-0-6-8-7-
-00011220: 322d 322d 3122 0a20 2020 2020 2020 2020  2-2-1".         
-00011230: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00011240: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00011250: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00011260: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00011270: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00011280: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00011290: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-000112a0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-000112b0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3037   style="fill:#07
-000112c0: 3065 3262 3b66 696c 6c2d 6f70 6163 6974  0e2b;fill-opacit
-000112d0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-000112e0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-000112f0: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
-00011300: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00011310: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00011320: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00011330: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00011340: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00011350: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-00011360: 2064 3d22 6d20 3135 362e 3036 3533 352c   d="m 156.06535,
-00011370: 3134 362e 3930 3733 3520 302e 3735 3433  146.90735 0.7543
-00011380: 382c 302e 3939 3139 3820 6320 302e 3134  8,0.99198 c 0.14
-00011390: 3435 322c 2d31 2e32 3031 3436 2030 2e36  452,-1.20146 0.6
-000113a0: 3533 3132 2c2d 312e 3633 3433 2031 2e30  5312,-1.6343 1.0
-000113b0: 3633 3236 2c2d 322e 3237 3530 3320 7a22  6326,-2.27503 z"
-000113c0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-000113d0: 7468 3134 3536 352d 392d 352d 392d 372d  th14565-9-5-9-7-
-000113e0: 372d 332d 342d 3422 0a20 2020 2020 2020  7-3-4-4".       
-000113f0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00011400: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00011410: 3022 0a20 2020 2020 2020 2020 736f 6469  0".         sodi
-00011420: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-00011430: 6363 6363 220a 2020 2020 2020 2020 2069  cccc".         i
-00011440: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00011450: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00011460: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-00011470: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-00011480: 0a20 2020 2020 203c 6369 7263 6c65 0a20  .      <circle. 
-00011490: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-000114a0: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
-000114b0: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-000114c0: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-000114d0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
-000114e0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-000114f0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00011500: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00011510: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00011520: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00011530: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00011540: 6831 3435 3637 2d36 2d31 2d39 2d37 2d37  h14567-6-1-9-7-7
-00011550: 2d35 2d39 2d34 220a 2020 2020 2020 2020  -5-9-4".        
-00011560: 2063 783d 2231 3534 2e31 3833 3138 220a   cx="154.18318".
-00011570: 2020 2020 2020 2020 2063 793d 2231 3435           cy="145
-00011580: 2e32 3531 3632 220a 2020 2020 2020 2020  .25162".        
-00011590: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000115a0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-000115b0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-000115c0: 706f 7274 2d79 6470 693d 2233 3030 220a  port-ydpi="300".
-000115d0: 2020 2020 2020 2020 2072 3d22 302e 3037           r="0.07
-000115e0: 3430 3637 3737 3922 202f 3e0a 2020 2020  4067779" />.    
-000115f0: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00011600: 2020 2072 3d22 302e 3037 3430 3637 3737     r="0.07406777
-00011610: 3922 0a20 2020 2020 2020 2020 7374 796c  9".         styl
-00011620: 653d 2266 696c 6c3a 2332 3533 6137 643b  e="fill:#253a7d;
-00011630: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00011640: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00011650: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-00011660: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00011670: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00011680: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00011690: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-000116a0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000116b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000116c0: 3536 372d 332d 3933 2d31 2d36 2d39 2d33  567-3-93-1-6-9-3
-000116d0: 2d37 2d38 2d35 220a 2020 2020 2020 2020  -7-8-5".        
-000116e0: 2063 783d 2231 3534 2e37 3730 3422 0a20   cx="154.7704". 
-000116f0: 2020 2020 2020 2020 6379 3d22 3134 362e          cy="146.
-00011700: 3730 3134 3822 0a20 2020 2020 2020 2020  70148".         
-00011710: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00011720: 726d 2d63 656e 7465 722d 783d 2234 2e36  rm-center-x="4.6
-00011730: 3433 3235 3636 220a 2020 2020 2020 2020  432566".        
-00011740: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00011750: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d39  orm-center-y="-9
-00011760: 2e39 3738 3036 3231 220a 2020 2020 2020  .9780621".      
-00011770: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-00011780: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
-00011790: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000117a0: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-000117b0: 2220 2f3e 0a20 2020 2020 203c 6369 7263  " />.      <circ
-000117c0: 6c65 0a20 2020 2020 2020 2020 723d 2230  le.         r="0
-000117d0: 2e30 3734 3036 3737 3739 220a 2020 2020  .074067779".    
-000117e0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000117f0: 3a23 6162 6161 3963 3b66 696c 6c2d 6f70  :#abaa9c;fill-op
-00011800: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00011810: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00011820: 6474 683a 303b 7374 726f 6b65 2d6d 6974  dth:0;stroke-mit
-00011830: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00011840: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00011850: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-00011860: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-00011870: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
-00011880: 643d 2270 6174 6831 3435 3637 2d33 2d39  d="path14567-3-9
-00011890: 2d30 2d39 2d38 2d32 2d38 2d30 2d35 2d33  -0-9-8-2-8-0-5-3
-000118a0: 220a 2020 2020 2020 2020 2063 783d 2231  ".         cx="1
-000118b0: 3536 2e30 3833 3422 0a20 2020 2020 2020  56.0834".       
-000118c0: 2020 6379 3d22 3134 362e 3930 3334 3722    cy="146.90347"
-000118d0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000118e0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-000118f0: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
-00011900: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00011910: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-00011920: 6e74 6572 2d79 3d22 2d39 2e39 3738 3036  nter-y="-9.97806
-00011930: 3231 220a 2020 2020 2020 2020 2069 6e6b  21".         ink
-00011940: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00011950: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
-00011960: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00011970: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00011980: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
-00011990: 2020 2020 2020 723d 2230 2e31 3134 3331        r="0.11431
-000119a0: 3332 3422 0a20 2020 2020 2020 2020 7374  324".         st
-000119b0: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
-000119c0: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
-000119d0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-000119e0: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-000119f0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00011a00: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00011a10: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00011a20: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00011a30: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00011a40: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00011a50: 3134 3536 372d 332d 322d 352d 342d 332d  14567-3-2-5-4-3-
-00011a60: 382d 302d 372d 372d 3522 0a20 2020 2020  8-0-7-7-5".     
-00011a70: 2020 2020 6378 3d22 3135 352e 3630 3033      cx="155.6003
-00011a80: 3622 0a20 2020 2020 2020 2020 6379 3d22  6".         cy="
-00011a90: 3134 352e 3136 3839 3122 0a20 2020 2020  145.16891".     
-00011aa0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-00011ab0: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
-00011ac0: 2237 2e31 3636 3231 3136 220a 2020 2020  "7.1662116".    
-00011ad0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-00011ae0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-00011af0: 3d22 2d31 352e 3339 3937 3531 220a 2020  ="-15.399751".  
-00011b00: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00011b10: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-00011b20: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00011b30: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-00011b40: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-00011b50: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
-00011b60: 723d 2230 2e30 3734 3036 3737 3739 220a  r="0.074067779".
-00011b70: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00011b80: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
-00011b90: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
-00011ba0: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
-00011bb0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-00011bc0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00011bd0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00011be0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00011bf0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00011c00: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00011c10: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00011c20: 7468 3134 3536 372d 322d 382d 362d 372d  th14567-2-8-6-7-
-00011c30: 382d 322d 322d 362d 392d 3622 0a20 2020  8-2-2-6-9-6".   
-00011c40: 2020 2020 2020 6378 3d22 3135 342e 3933        cx="154.93
-00011c50: 3732 3722 0a20 2020 2020 2020 2020 6379  727".         cy
-00011c60: 3d22 3134 352e 3931 3130 3422 0a20 2020  ="145.91104".   
-00011c70: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00011c80: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00011c90: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00011ca0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00011cb0: 3330 3022 202f 3e0a 2020 2020 2020 3c63  300" />.      <c
-00011cc0: 6972 636c 650a 2020 2020 2020 2020 2072  ircle.         r
-00011cd0: 3d22 302e 3134 3037 3931 3935 220a 2020  ="0.14079195".  
-00011ce0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00011cf0: 6c6c 3a23 6564 6630 6663 3b66 696c 6c2d  ll:#edf0fc;fill-
-00011d00: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
-00011d10: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-00011d20: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-00011d30: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00011d40: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00011d50: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00011d60: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00011d70: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00011d80: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00011d90: 3134 3536 372d 322d 372d 302d 392d 302d  14567-2-7-0-9-0-
-00011da0: 352d 312d 312d 332d 3722 0a20 2020 2020  5-1-1-3-7".     
-00011db0: 2020 2020 6378 3d22 3135 372e 3835 3734      cx="157.8574
-00011dc0: 3822 0a20 2020 2020 2020 2020 6379 3d22  8".         cy="
-00011dd0: 3134 352e 3634 3331 3722 0a20 2020 2020  145.64317".     
-00011de0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00011df0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00011e00: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00011e10: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00011e20: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00011e30: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00011e40: 3d22 6669 6c6c 3a6e 6f6e 653b 6669 6c6c  ="fill:none;fill
-00011e50: 2d72 756c 653a 6576 656e 6f64 643b 7374  -rule:evenodd;st
-00011e60: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00011e70: 6f6b 652d 7769 6474 683a 302e 3133 3232  oke-width:0.1322
-00011e80: 3932 3b73 7472 6f6b 652d 6c69 6e65 6361  92;stroke-lineca
-00011e90: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00011ea0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00011eb0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00011ec0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00011ed0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00011ee0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00011ef0: 2020 643d 226d 2031 3534 2e31 3532 3636    d="m 154.15266
-00011f00: 2c31 3435 2e32 3530 3038 2063 2030 2e38  ,145.25008 c 0.8
-00011f10: 3839 3438 2c2d 302e 3138 3132 3320 312e  8948,-0.18123 1.
-00011f20: 3634 3634 332c 2d30 2e36 3237 3532 2032  64643,-0.62752 2
-00011f30: 2e33 3831 3935 2c2d 312e 3131 3636 3820  .38195,-1.11668 
-00011f40: 302e 3333 3234 362c 302e 3630 3432 3120  0.33246,0.60421 
-00011f50: 302e 3635 322c 312e 3232 3032 3720 312e  0.652,1.22027 1.
-00011f60: 3334 3833 382c 312e 3439 3039 202d 302e  34838,1.4909 -0.
-00011f70: 3432 3232 352c 302e 3537 3536 3520 2d30  42225,0.57565 -0
-00011f80: 2e38 3432 3537 2c31 2e31 3536 3531 202d  .84257,1.15651 -
-00011f90: 312e 3036 3332 362c 322e 3237 3530 3320  1.06326,2.27503 
-00011fa0: 6c20 2d30 2e37 3534 3338 2c2d 302e 3939  l -0.75438,-0.99
-00011fb0: 3139 3820 2d31 2e32 3833 3035 2c2d 302e  198 -1.28305,-0.
-00011fc0: 3139 3030 3820 6320 302e 3133 3739 362c  19008 c 0.13796,
-00011fd0: 2d30 2e33 3038 3536 2030 2e32 3033 3335  -0.30856 0.20335
-00011fe0: 2c2d 302e 3538 3038 3420 302e 3135 3434  ,-0.58084 0.1544
-00011ff0: 342c 2d30 2e37 3935 3937 202d 302e 3230  4,-0.79597 -0.20
-00012000: 3137 342c 2d30 2e32 3533 3535 202d 302e  174,-0.25355 -0.
-00012010: 3435 3736 362c 2d30 2e34 3830 3031 202d  45766,-0.48001 -
-00012020: 302e 3738 3430 382c 2d30 2e36 3731 3232  0.78408,-0.67122
-00012030: 207a 220a 2020 2020 2020 2020 2069 643d   z".         id=
-00012040: 2270 6174 6831 3330 332d 372d 3822 0a20  "path1303-7-8". 
-00012050: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-00012060: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-00012070: 6363 6363 2220 2f3e 0a20 2020 203c 2f67  cccc" />.    </g
-00012080: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
+0000bdb0: 2020 2020 643d 226d 2033 3139 2e31 3334      d="m 319.134
+0000bdc0: 3735 2c34 3430 2e31 3139 3734 2032 312e  75,440.11974 21.
+0000bdd0: 3733 3230 322c 2d30 2e39 3837 3832 2031  73202,-0.98782 1
+0000bde0: 342e 3237 3834 372c 2d31 352e 3839 3439  4.27847,-15.8949
+0000bdf0: 2063 202d 3137 2e39 3837 3835 2c31 322e   c -17.98785,12.
+0000be00: 3039 3731 3420 2d32 362e 3538 3136 382c  09714 -26.58168,
+0000be10: 3134 2e30 3338 3538 202d 3336 2e30 3130  14.03858 -36.010
+0000be20: 3439 2c31 362e 3838 3237 3220 7a22 0a20  49,16.88272 z". 
+0000be30: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000be40: 3534 372d 312d 372d 3822 0a20 2020 2020  547-1-7-8".     
+0000be50: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000be60: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000be70: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+0000be80: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+0000be90: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
+0000bea0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000beb0: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000bec0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000bed0: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000bee0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000bef0: 653d 2266 696c 6c3a 2331 6332 6336 383b  e="fill:#1c2c68;
+0000bf00: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000bf10: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000bf20: 726f 6b65 2d77 6964 7468 3a30 2e37 3438  roke-width:0.748
+0000bf30: 3939 373b 7374 726f 6b65 2d6c 696e 6563  997;stroke-linec
+0000bf40: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000bf50: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000bf60: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000bf70: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000bf80: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000bf90: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000bfa0: 2064 3d22 6d20 3334 302e 3836 3637 372c   d="m 340.86677,
+0000bfb0: 3433 392e 3133 3139 3220 392e 3432 3931  439.13192 9.4291
+0000bfc0: 372c 322e 3135 3532 3420 342e 3834 3933  7,2.15524 4.8493
+0000bfd0: 2c2d 3138 2e30 3530 3134 207a 220a 2020  ,-18.05014 z".  
+0000bfe0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000bff0: 3439 2d31 2d30 2d31 220a 2020 2020 2020  49-1-0-1".      
+0000c000: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000c010: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000c020: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000c030: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000c040: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000c050: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000c060: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+0000c070: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+0000c080: 2266 696c 6c3a 2330 3630 3530 383b 6669  "fill:#060508;fi
+0000c090: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000c0a0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000c0b0: 6b65 2d77 6964 7468 3a30 2e37 3438 3939  ke-width:0.74899
+0000c0c0: 373b 7374 726f 6b65 2d6c 696e 6563 6170  7;stroke-linecap
+0000c0d0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+0000c0e0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+0000c0f0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000c100: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000c110: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+0000c120: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+0000c130: 3d22 6d20 3335 302e 3239 3539 342c 3434  ="m 350.29594,44
+0000c140: 312e 3238 3731 3620 3235 2e32 3334 3238  1.28716 25.23428
+0000c150: 2c34 2e34 3930 3039 2063 202d 392e 3833  ,4.49009 c -9.83
+0000c160: 3333 362c 2d35 2e31 3938 3437 202d 3135  336,-5.19847 -15
+0000c170: 2e35 3237 3731 2c2d 3133 2e35 3530 3436  .52771,-13.55046
+0000c180: 202d 3230 2e33 3834 3938 2c2d 3232 2e35   -20.38498,-22.5
+0000c190: 3430 3233 207a 220a 2020 2020 2020 2069  4023 z".       i
+0000c1a0: 643d 2270 6174 6831 3435 3531 2d30 2d33  d="path14551-0-3
+0000c1b0: 2d39 220a 2020 2020 2020 2069 6e6b 7363  -9".       inksc
+0000c1c0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+0000c1d0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+0000c1e0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+0000c1f0: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
+0000c200: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000c210: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+0000c220: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000c230: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+0000c240: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+0000c250: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+0000c260: 3a23 3237 3337 3733 3b66 696c 6c2d 6f70  :#273773;fill-op
+0000c270: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+0000c280: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000c290: 6474 683a 302e 3734 3839 3937 3b73 7472  dth:0.748997;str
+0000c2a0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+0000c2b0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+0000c2c0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+0000c2d0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+0000c2e0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+0000c2f0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000c300: 3122 0a20 2020 2020 2020 643d 226d 2033  1".       d="m 3
+0000c310: 3139 2e31 3334 3735 2c34 3430 2e31 3139  19.13475,440.119
+0000c320: 3734 2063 2034 2e37 3832 3139 2c32 2e37  74 c 4.78219,2.7
+0000c330: 3433 3337 2031 302e 3035 3438 352c 352e  4337 10.05485,5.
+0000c340: 3130 3934 3520 3131 2e38 3533 3832 2c31  10945 11.85382,1
+0000c350: 302e 3134 3736 206c 2039 2e38 3738 322c  0.1476 l 9.8782,
+0000c360: 2d31 312e 3133 3534 3220 7a22 0a20 2020  -11.13542 z".   
+0000c370: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+0000c380: 332d 332d 322d 3222 0a20 2020 2020 2020  3-3-2-2".       
+0000c390: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+0000c3a0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+0000c3b0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+0000c3c0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+0000c3d0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000c3e0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000c3f0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000c400: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000c410: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+0000c420: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+0000c430: 2266 696c 6c3a 2331 3432 3637 323b 6669  "fill:#142672;fi
+0000c440: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000c450: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000c460: 6b65 2d77 6964 7468 3a30 2e37 3438 3939  ke-width:0.74899
+0000c470: 373b 7374 726f 6b65 2d6c 696e 6563 6170  7;stroke-linecap
+0000c480: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+0000c490: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+0000c4a0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000c4b0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000c4c0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+0000c4d0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+0000c4e0: 3d22 6d20 3333 302e 3938 3835 372c 3435  ="m 330.98857,45
+0000c4f0: 302e 3236 3733 3420 3434 2e35 3431 3635  0.26734 44.54165
+0000c500: 2c2d 342e 3439 3030 3920 2d33 342e 3636  ,-4.49009 -34.66
+0000c510: 3334 352c 2d36 2e36 3435 3333 207a 220a  345,-6.64533 z".
+0000c520: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000c530: 3435 3535 2d34 2d31 2d36 220a 2020 2020  4555-4-1-6".    
+0000c540: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000c550: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000c560: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
+0000c570: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000c580: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000c590: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000c5a0: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000c5b0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000c5c0: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
+0000c5d0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000c5e0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000c5f0: 726f 6b65 2d77 6964 7468 3a30 2e37 3438  roke-width:0.748
+0000c600: 3939 373b 7374 726f 6b65 2d6c 696e 6563  997;stroke-linec
+0000c610: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000c620: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000c630: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000c640: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000c650: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000c660: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000c670: 2064 3d22 6d20 3333 302e 3938 3835 372c   d="m 330.98857,
+0000c680: 3435 302e 3236 3733 3420 3235 2e36 3833  450.26734 25.683
+0000c690: 332c 322e 3639 3430 3520 3138 2e38 3538  3,2.69405 18.858
+0000c6a0: 3335 2c2d 372e 3138 3431 3420 7a22 0a20  35,-7.18414 z". 
+0000c6b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000c6c0: 3535 372d 302d 372d 3322 0a20 2020 2020  557-0-7-3".     
+0000c6d0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000c6e0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000c6f0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000c700: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000c710: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000c720: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000c730: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+0000c740: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+0000c750: 3d22 6669 6c6c 3a23 3232 3334 3765 3b66  ="fill:#22347e;f
+0000c760: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000c770: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000c780: 6f6b 652d 7769 6474 683a 302e 3734 3839  oke-width:0.7489
+0000c790: 3937 3b73 7472 6f6b 652d 6c69 6e65 6361  97;stroke-lineca
+0000c7a0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+0000c7b0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+0000c7c0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000c7d0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000c7e0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+0000c7f0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000c800: 643d 226d 2033 3330 2e39 3838 3537 2c34  d="m 330.98857,4
+0000c810: 3530 2e32 3637 3334 2063 2030 2e35 3737  50.26734 c 0.577
+0000c820: 3533 2c34 2e39 3739 3536 202d 312e 3432  53,4.97956 -1.42
+0000c830: 3135 312c 382e 3131 3837 3320 2d32 2e33  151,8.11873 -2.3
+0000c840: 3334 3834 2c31 322e 3033 3334 3220 6c20  3484,12.03342 l 
+0000c850: 3238 2e30 3138 3134 2c2d 392e 3333 3933  28.01814,-9.3393
+0000c860: 3720 7a22 0a20 2020 2020 2020 6964 3d22  7 z".       id="
+0000c870: 7061 7468 3134 3535 392d 332d 342d 3222  path14559-3-4-2"
+0000c880: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000c890: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+0000c8a0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+0000c8b0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+0000c8c0: 6573 3d22 6363 6363 220a 2020 2020 2020  es="cccc".      
+0000c8d0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000c8e0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+0000c8f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000c900: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+0000c910: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+0000c920: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+0000c930: 3831 3036 393b 6669 6c6c 2d6f 7061 6369  81069;fill-opaci
+0000c940: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000c950: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000c960: 3a30 2e37 3438 3939 373b 7374 726f 6b65  :0.748997;stroke
+0000c970: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+0000c980: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+0000c990: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+0000c9a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000c9b0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000c9c0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000c9d0: 2020 2020 2020 2064 3d22 6d20 3332 382e         d="m 328.
+0000c9e0: 3635 3337 332c 3436 322e 3330 3037 3620  65373,462.30076 
+0000c9f0: 3139 2e33 3937 3137 2c32 2e38 3733 3636  19.39717,2.87366
+0000ca00: 2032 372e 3437 3933 322c 2d31 392e 3339   27.47932,-19.39
+0000ca10: 3731 3720 7a22 0a20 2020 2020 2020 6964  717 z".       id
+0000ca20: 3d22 7061 7468 3134 3536 312d 392d 322d  ="path14561-9-2-
+0000ca30: 3222 0a20 2020 2020 2020 696e 6b73 6361  2".       inksca
+0000ca40: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+0000ca50: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+0000ca60: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000ca70: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+0000ca80: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000ca90: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+0000caa0: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+0000cab0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000cac0: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
+0000cad0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+0000cae0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+0000caf0: 683a 302e 3734 3839 3937 3b73 7472 6f6b  h:0.748997;strok
+0000cb00: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+0000cb10: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+0000cb20: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+0000cb30: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000cb40: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000cb50: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000cb60: 0a20 2020 2020 2020 643d 226d 2033 3438  .       d="m 348
+0000cb70: 2e30 3530 392c 3436 352e 3137 3434 3220  .0509,465.17442 
+0000cb80: 3131 2e34 3034 3831 2c31 342e 3939 3638  11.40481,14.9968
+0000cb90: 3920 2d34 2e32 3230 3637 2c2d 3230 2e32  9 -4.22067,-20.2
+0000cba0: 3035 3339 207a 220a 2020 2020 2020 2069  0539 z".       i
+0000cbb0: 643d 2270 6174 6831 3435 3633 2d31 2d30  d="path14563-1-0
+0000cbc0: 2d36 220a 2020 2020 2020 2069 6e6b 7363  -6".       inksc
+0000cbd0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+0000cbe0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+0000cbf0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000cc00: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+0000cc10: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000cc20: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+0000cc30: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+0000cc40: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000cc50: 2332 3833 6438 373b 6669 6c6c 2d6f 7061  #283d87;fill-opa
+0000cc60: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+0000cc70: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+0000cc80: 7468 3a30 2e37 3438 3939 373b 7374 726f  th:0.748997;stro
+0000cc90: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+0000cca0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+0000ccb0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+0000ccc0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+0000ccd0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+0000cce0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000ccf0: 220a 2020 2020 2020 2064 3d22 6d20 3335  ".       d="m 35
+0000cd00: 352e 3233 3530 342c 3435 392e 3936 3539  5.23504,459.9659
+0000cd10: 3220 342e 3232 3036 372c 3230 2e32 3035  2 4.22067,20.205
+0000cd20: 3339 2063 2032 2e31 3834 3936 2c2d 3138  39 c 2.18496,-18
+0000cd30: 2e31 3633 3720 392e 3837 3430 342c 2d32  .1637 9.87404,-2
+0000cd40: 342e 3730 3735 3720 3136 2e30 3734 3531  4.70757 16.07451
+0000cd50: 2c2d 3334 2e33 3934 3036 207a 220a 2020  ,-34.39406 z".  
+0000cd60: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000cd70: 3635 2d39 2d35 2d39 220a 2020 2020 2020  65-9-5-9".      
+0000cd80: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000cd90: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000cda0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
+0000cdb0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
+0000cdc0: 6322 0a20 2020 2020 2020 696e 6b73 6361  c".       inksca
+0000cdd0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000cde0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000cdf0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000ce00: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+0000ce10: 6972 636c 650a 2020 2020 2020 2073 7479  ircle.       sty
+0000ce20: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
+0000ce30: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
+0000ce40: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
+0000ce50: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+0000ce60: 7468 3a30 2e37 3438 3939 373b 7374 726f  th:0.748997;stro
+0000ce70: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000ce80: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000ce90: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+0000cea0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+0000ceb0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+0000cec0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+0000ced0: 2d36 2d31 2d39 220a 2020 2020 2020 2063  -6-1-9".       c
+0000cee0: 783d 2233 3139 2e35 3935 3938 220a 2020  x="319.59598".  
+0000cef0: 2020 2020 2063 793d 2234 3430 2e31 3432       cy="440.142
+0000cf00: 3739 220a 2020 2020 2020 2069 6e6b 7363  79".       inksc
+0000cf10: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000cf20: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000cf30: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000cf40: 693d 2233 3030 220a 2020 2020 2020 2072  i="300".       r
+0000cf50: 3d22 312e 3131 3937 3634 3922 202f 3e0a  ="1.1197649" />.
+0000cf60: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
+0000cf70: 2020 2072 3d22 312e 3131 3937 3634 3922     r="1.1197649"
+0000cf80: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+0000cf90: 696c 6c3a 2332 3533 6137 643b 6669 6c6c  ill:#253a7d;fill
+0000cfa0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+0000cfb0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+0000cfc0: 2d77 6964 7468 3a30 2e37 3438 3939 373b  -width:0.748997;
+0000cfd0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+0000cfe0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+0000cff0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+0000d000: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+0000d010: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000d020: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000d030: 3435 3637 2d33 2d39 332d 312d 3622 0a20  4567-3-93-1-6". 
+0000d040: 2020 2020 2020 6378 3d22 3332 382e 3437        cx="328.47
+0000d050: 3335 3422 0a20 2020 2020 2020 6379 3d22  354".       cy="
+0000d060: 3436 322e 3036 3138 3922 0a20 2020 2020  462.06189".     
+0000d070: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+0000d080: 666f 726d 2d63 656e 7465 722d 783d 2234  form-center-x="4
+0000d090: 2e36 3433 3235 3636 220a 2020 2020 2020  .6432566".      
+0000d0a0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+0000d0b0: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d39  orm-center-y="-9
+0000d0c0: 2e39 3738 3036 3231 220a 2020 2020 2020  .9780621".      
+0000d0d0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000d0e0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+0000d0f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000d100: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+0000d110: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
+0000d120: 2020 2020 723d 2231 2e31 3139 3736 3439      r="1.1197649
+0000d130: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+0000d140: 6669 6c6c 3a23 3235 3361 3764 3b66 696c  fill:#253a7d;fil
+0000d150: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000d160: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000d170: 652d 7769 6474 683a 302e 3734 3839 3937  e-width:0.748997
+0000d180: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000d190: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000d1a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000d1b0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+0000d1c0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000d1d0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000d1e0: 3134 3536 372d 332d 372d 332d 302d 3922  14567-3-7-3-0-9"
+0000d1f0: 0a20 2020 2020 2020 6378 3d22 3335 342e  .       cx="354.
+0000d200: 3936 3233 3722 0a20 2020 2020 2020 6379  96237".       cy
+0000d210: 3d22 3435 332e 3033 3331 3122 0a20 2020  ="453.03311".   
+0000d220: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+0000d230: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
+0000d240: 2234 2e36 3433 3235 3636 220a 2020 2020  "4.6432566".    
+0000d250: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+0000d260: 7366 6f72 6d2d 6365 6e74 6572 2d79 3d22  sform-center-y="
+0000d270: 2d39 2e39 3738 3036 3231 220a 2020 2020  -9.9780621".    
+0000d280: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000d290: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+0000d2a0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000d2b0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+0000d2c0: 2f3e 0a20 2020 203c 6369 7263 6c65 0a20  />.    <circle. 
+0000d2d0: 2020 2020 2020 723d 2231 2e31 3139 3736        r="1.11976
+0000d2e0: 3439 220a 2020 2020 2020 2073 7479 6c65  49".       style
+0000d2f0: 3d22 6669 6c6c 3a23 6138 6139 6161 3b66  ="fill:#a8a9aa;f
+0000d300: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000d310: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000d320: 6f6b 652d 7769 6474 683a 302e 3734 3839  oke-width:0.7489
+0000d330: 3937 3b73 7472 6f6b 652d 6d69 7465 726c  97;stroke-miterl
+0000d340: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+0000d350: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+0000d360: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+0000d370: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000d380: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+0000d390: 7468 3134 3536 372d 332d 352d 382d 382d  th14567-3-5-8-8-
+0000d3a0: 3522 0a20 2020 2020 2020 6378 3d22 3335  5".       cx="35
+0000d3b0: 352e 3232 3739 3422 0a20 2020 2020 2020  5.22794".       
+0000d3c0: 6379 3d22 3435 392e 3830 3436 3922 0a20  cy="459.80469". 
+0000d3d0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+0000d3e0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+0000d3f0: 783d 2234 2e36 3433 3235 3636 220a 2020  x="4.6432566".  
+0000d400: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+0000d410: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+0000d420: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
+0000d430: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000d440: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000d450: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000d460: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000d470: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
+0000d480: 0a20 2020 2020 2020 723d 2231 2e31 3139  .       r="1.119
+0000d490: 3736 3439 220a 2020 2020 2020 2073 7479  7649".       sty
+0000d4a0: 6c65 3d22 6669 6c6c 3a23 6162 6161 3963  le="fill:#abaa9c
+0000d4b0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000d4c0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000d4d0: 7472 6f6b 652d 7769 6474 683a 302e 3734  troke-width:0.74
+0000d4e0: 3839 3937 3b73 7472 6f6b 652d 6d69 7465  8997;stroke-mite
+0000d4f0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000d500: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000d510: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+0000d520: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+0000d530: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
+0000d540: 7061 7468 3134 3536 372d 332d 392d 302d  path14567-3-9-0-
+0000d550: 392d 3822 0a20 2020 2020 2020 6378 3d22  9-8".       cx="
+0000d560: 3334 382e 3332 3335 3822 0a20 2020 2020  348.32358".     
+0000d570: 2020 6379 3d22 3436 352e 3131 3537 3222    cy="465.11572"
+0000d580: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000d590: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+0000d5a0: 722d 783d 2234 2e36 3433 3235 3636 220a  r-x="4.6432566".
+0000d5b0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000d5c0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+0000d5d0: 2d79 3d22 2d39 2e39 3738 3036 3231 220a  -y="-9.9780621".
+0000d5e0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000d5f0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+0000d600: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000d610: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+0000d620: 3030 2220 2f3e 0a20 2020 203c 6369 7263  00" />.    <circ
+0000d630: 6c65 0a20 2020 2020 2020 723d 2231 2e37  le.       r="1.7
+0000d640: 3238 3230 3032 220a 2020 2020 2020 2073  282002".       s
+0000d650: 7479 6c65 3d22 6669 6c6c 3a23 3131 3230  tyle="fill:#1120
+0000d660: 3636 3b66 696c 6c2d 6f70 6163 6974 793a  66;fill-opacity:
+0000d670: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+0000d680: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+0000d690: 3734 3839 3937 3b73 7472 6f6b 652d 6d69  748997;stroke-mi
+0000d6a0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+0000d6b0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+0000d6c0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+0000d6d0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+0000d6e0: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
+0000d6f0: 3d22 7061 7468 3134 3536 372d 332d 322d  ="path14567-3-2-
+0000d700: 352d 342d 3322 0a20 2020 2020 2020 6378  5-4-3".       cx
+0000d710: 3d22 3334 312e 3032 3038 3722 0a20 2020  ="341.02087".   
+0000d720: 2020 2020 6379 3d22 3433 382e 3839 3234      cy="438.8924
+0000d730: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000d740: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000d750: 7465 722d 783d 2237 2e31 3636 3231 3136  ter-x="7.1662116
+0000d760: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000d770: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000d780: 6572 2d79 3d22 2d31 352e 3339 3937 3531  er-y="-15.399751
+0000d790: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000d7a0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000d7b0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000d7c0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000d7d0: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
+0000d7e0: 7263 6c65 0a20 2020 2020 2020 723d 2231  rcle.       r="1
+0000d7f0: 2e31 3139 3736 3439 220a 2020 2020 2020  .1197649".      
+0000d800: 2073 7479 6c65 3d22 6669 6c6c 3a23 6564   style="fill:#ed
+0000d810: 6630 6663 3b66 696c 6c2d 6f70 6163 6974  f0fc;fill-opacit
+0000d820: 793a 302e 3939 3034 3436 3b73 7472 6f6b  y:0.990446;strok
+0000d830: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+0000d840: 2d77 6964 7468 3a30 2e37 3438 3939 373b  -width:0.748997;
+0000d850: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+0000d860: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+0000d870: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+0000d880: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+0000d890: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000d8a0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000d8b0: 3435 3637 2d32 2d36 2d30 2d30 220a 2020  4567-2-6-0-0".  
+0000d8c0: 2020 2020 2063 783d 2233 3530 2e33 3831       cx="350.381
+0000d8d0: 3539 220a 2020 2020 2020 2063 793d 2234  59".       cy="4
+0000d8e0: 3430 2e38 3137 3732 220a 2020 2020 2020  40.81772".      
+0000d8f0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000d900: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+0000d910: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000d920: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+0000d930: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
+0000d940: 2020 2020 723d 2231 2e31 3139 3736 3439      r="1.1197649
+0000d950: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+0000d960: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
+0000d970: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
+0000d980: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
+0000d990: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+0000d9a0: 2e37 3438 3939 373b 7374 726f 6b65 2d6d  .748997;stroke-m
+0000d9b0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000d9c0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000d9d0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+0000d9e0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+0000d9f0: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
+0000da00: 643d 2270 6174 6831 3435 3637 2d32 2d38  d="path14567-2-8
+0000da10: 2d36 2d37 2d38 220a 2020 2020 2020 2063  -6-7-8".       c
+0000da20: 783d 2233 3330 2e39 3936 3238 220a 2020  x="330.99628".  
+0000da30: 2020 2020 2063 793d 2234 3530 2e31 3132       cy="450.112
+0000da40: 3033 220a 2020 2020 2020 2069 6e6b 7363  03".       inksc
+0000da50: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000da60: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000da70: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000da80: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000da90: 6369 7263 6c65 0a20 2020 2020 2020 723d  circle.       r=
+0000daa0: 2232 2e31 3238 3530 3836 220a 2020 2020  "2.1285086".    
+0000dab0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000dac0: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
+0000dad0: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+0000dae0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000daf0: 6b65 2d77 6964 7468 3a31 2e34 3233 3733  ke-width:1.42373
+0000db00: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000db10: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000db20: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000db30: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+0000db40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000db50: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000db60: 3134 3536 372d 322d 372d 302d 392d 3022  14567-2-7-0-9-0"
+0000db70: 0a20 2020 2020 2020 6378 3d22 3337 352e  .       cx="375.
+0000db80: 3134 3433 3522 0a20 2020 2020 2020 6379  14435".       cy
+0000db90: 3d22 3434 362e 3036 3233 3822 0a20 2020  ="446.06238".   
+0000dba0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000dbb0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+0000dbc0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000dbd0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+0000dbe0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+0000dbf0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+0000dc00: 3a23 3365 3462 3737 3b66 696c 6c2d 6f70  :#3e4b77;fill-op
+0000dc10: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+0000dc20: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000dc30: 6474 683a 302e 3834 3530 3235 3b73 7472  dth:0.845025;str
+0000dc40: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+0000dc50: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+0000dc60: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+0000dc70: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+0000dc80: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+0000dc90: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000dca0: 3122 0a20 2020 2020 2020 643d 226d 2034  1".       d="m 4
+0000dcb0: 3038 2e31 3636 322c 3434 312e 3631 3733  08.1662,441.6173
+0000dcc0: 2031 362e 3334 3535 2c2d 302e 3734 3239   16.3455,-0.7429
+0000dcd0: 3820 3130 2e37 3339 342c 2d31 312e 3935  8 10.7394,-11.95
+0000dce0: 3531 3820 6320 2d31 332e 3532 3933 372c  518 c -13.52937,
+0000dcf0: 392e 3039 3837 3320 2d31 392e 3939 3331  9.09873 -19.9931
+0000dd00: 322c 3130 2e35 3538 3938 202d 3237 2e30  2,10.55898 -27.0
+0000dd10: 3834 392c 3132 2e36 3938 3136 207a 220a  849,12.69816 z".
+0000dd20: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000dd30: 3435 3437 2d31 2d37 2d38 2d33 220a 2020  4547-1-7-8-3".  
+0000dd40: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+0000dd50: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+0000dd60: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
+0000dd70: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+0000dd80: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
+0000dd90: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+0000dda0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+0000ddb0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+0000ddc0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+0000ddd0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+0000dde0: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
+0000ddf0: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
+0000de00: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+0000de10: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+0000de20: 3834 3530 3235 3b73 7472 6f6b 652d 6c69  845025;stroke-li
+0000de30: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+0000de40: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+0000de50: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000de60: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000de70: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000de80: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000de90: 2020 2020 643d 226d 2034 3234 2e35 3131      d="m 424.511
+0000dea0: 372c 3434 302e 3837 3433 3220 372e 3039  7,440.87432 7.09
+0000deb0: 3230 352c 312e 3632 3130 3420 332e 3634  205,1.62104 3.64
+0000dec0: 3733 352c 2d31 332e 3537 3632 3220 7a22  735,-13.57622 z"
+0000ded0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000dee0: 3134 3534 392d 312d 302d 312d 3622 0a20  14549-1-0-1-6". 
+0000def0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+0000df00: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+0000df10: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
+0000df20: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+0000df30: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+0000df40: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+0000df50: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+0000df60: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+0000df70: 7479 6c65 3d22 6669 6c6c 3a23 3036 3035  tyle="fill:#0605
+0000df80: 3038 3b66 696c 6c2d 6f70 6163 6974 793a  08;fill-opacity:
+0000df90: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+0000dfa0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+0000dfb0: 3834 3530 3235 3b73 7472 6f6b 652d 6c69  845025;stroke-li
+0000dfc0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+0000dfd0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+0000dfe0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000dff0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000e000: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000e010: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000e020: 2020 2020 643d 226d 2034 3331 2e36 3033      d="m 431.603
+0000e030: 3735 2c34 3432 2e34 3935 3336 2031 382e  75,442.49536 18.
+0000e040: 3937 3937 2c33 2e33 3737 3138 2063 202d  9797,3.37718 c -
+0000e050: 372e 3339 3630 372c 2d33 2e39 3039 3938  7.39607,-3.90998
+0000e060: 202d 3131 2e36 3739 2c2d 3130 2e31 3931   -11.679,-10.191
+0000e070: 3833 202d 3135 2e33 3332 3335 2c2d 3136  83 -15.33235,-16
+0000e080: 2e39 3533 3420 7a22 0a20 2020 2020 2020  .9534 z".       
+0000e090: 6964 3d22 7061 7468 3134 3535 312d 302d  id="path14551-0-
+0000e0a0: 332d 392d 3722 0a20 2020 2020 2020 696e  3-9-7".       in
+0000e0b0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+0000e0c0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+0000e0d0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+0000e0e0: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
+0000e0f0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000e100: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+0000e110: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000e120: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+0000e130: 3030 2220 2f3e 0a20 2020 203c 7061 7468  00" />.    <path
+0000e140: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+0000e150: 696c 6c3a 2332 3733 3737 333b 6669 6c6c  ill:#273773;fill
+0000e160: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+0000e170: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+0000e180: 2d77 6964 7468 3a30 2e38 3435 3032 353b  -width:0.845025;
+0000e190: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+0000e1a0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+0000e1b0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+0000e1c0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000e1d0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000e1e0: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+0000e1f0: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+0000e200: 6d20 3430 382e 3136 3632 2c34 3431 2e36  m 408.1662,441.6
+0000e210: 3137 3320 6320 332e 3539 3638 372c 322e  173 c 3.59687,2.
+0000e220: 3036 3334 2037 2e35 3632 3635 2c33 2e38  0634 7.56265,3.8
+0000e230: 3433 3032 2038 2e39 3135 3733 2c37 2e36  4302 8.91573,7.6
+0000e240: 3332 3420 6c20 372e 3432 3937 372c 2d38  324 l 7.42977,-8
+0000e250: 2e33 3735 3338 207a 220a 2020 2020 2020  .37538 z".      
+0000e260: 2069 643d 2270 6174 6831 3435 3533 2d33   id="path14553-3
+0000e270: 2d32 2d32 2d35 220a 2020 2020 2020 2069  -2-2-5".       i
+0000e280: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+0000e290: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+0000e2a0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+0000e2b0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+0000e2c0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000e2d0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+0000e2e0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000e2f0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+0000e300: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
+0000e310: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+0000e320: 6669 6c6c 3a23 3134 3236 3732 3b66 696c  fill:#142672;fil
+0000e330: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000e340: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000e350: 652d 7769 6474 683a 302e 3834 3530 3235  e-width:0.845025
+0000e360: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+0000e370: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+0000e380: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+0000e390: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+0000e3a0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+0000e3b0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+0000e3c0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+0000e3d0: 226d 2034 3137 2e30 3831 3933 2c34 3439  "m 417.08193,449
+0000e3e0: 2e32 3439 3720 3333 2e35 3031 3532 2c2d  .2497 33.50152,-
+0000e3f0: 332e 3337 3731 3620 2d32 362e 3037 3137  3.37716 -26.0717
+0000e400: 352c 2d34 2e39 3938 3232 207a 220a 2020  5,-4.99822 z".  
+0000e410: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000e420: 3535 2d34 2d31 2d36 2d33 220a 2020 2020  55-4-1-6-3".    
+0000e430: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000e440: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000e450: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
+0000e460: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000e470: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000e480: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000e490: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000e4a0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000e4b0: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
+0000e4c0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000e4d0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000e4e0: 726f 6b65 2d77 6964 7468 3a30 2e38 3435  roke-width:0.845
+0000e4f0: 3032 353b 7374 726f 6b65 2d6c 696e 6563  025;stroke-linec
+0000e500: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000e510: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000e520: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000e530: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000e540: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000e550: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000e560: 2064 3d22 6d20 3431 372e 3038 3139 332c   d="m 417.08193,
+0000e570: 3434 392e 3234 3937 2031 392e 3331 3734  449.2497 19.3174
+0000e580: 312c 322e 3032 3633 3120 3134 2e31 3834  1,2.02631 14.184
+0000e590: 3131 2c2d 352e 3430 3334 3720 7a22 0a20  11,-5.40347 z". 
+0000e5a0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000e5b0: 3535 372d 302d 372d 332d 3522 0a20 2020  557-0-7-3-5".   
+0000e5c0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+0000e5d0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+0000e5e0: 3d22 3022 0a20 2020 2020 2020 696e 6b73  ="0".       inks
+0000e5f0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000e600: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000e610: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000e620: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000e630: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+0000e640: 6c65 3d22 6669 6c6c 3a23 3232 3334 3765  le="fill:#22347e
+0000e650: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000e660: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000e670: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
+0000e680: 3530 3235 3b73 7472 6f6b 652d 6c69 6e65  5025;stroke-line
+0000e690: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+0000e6a0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+0000e6b0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000e6c0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000e6d0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000e6e0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000e6f0: 2020 643d 226d 2034 3137 2e30 3831 3933    d="m 417.08193
+0000e700: 2c34 3439 2e32 3439 3720 6320 302e 3433  ,449.2497 c 0.43
+0000e710: 3433 382c 332e 3734 3533 3320 2d31 2e30  438,3.74533 -1.0
+0000e720: 3639 3138 2c36 2e31 3036 3433 202d 312e  6918,6.10643 -1.
+0000e730: 3735 3631 332c 392e 3035 3038 3220 6c20  75613,9.05082 l 
+0000e740: 3231 2e30 3733 3534 2c2d 372e 3032 3435  21.07354,-7.0245
+0000e750: 3120 7a22 0a20 2020 2020 2020 6964 3d22  1 z".       id="
+0000e760: 7061 7468 3134 3535 392d 332d 342d 322d  path14559-3-4-2-
+0000e770: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000e780: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+0000e790: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+0000e7a0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+0000e7b0: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
+0000e7c0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000e7d0: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+0000e7e0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000e7f0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+0000e800: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+0000e810: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000e820: 2330 3831 3036 393b 6669 6c6c 2d6f 7061  #081069;fill-opa
+0000e830: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+0000e840: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+0000e850: 7468 3a30 2e38 3435 3032 353b 7374 726f  th:0.845025;stro
+0000e860: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+0000e870: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+0000e880: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+0000e890: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+0000e8a0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+0000e8b0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000e8c0: 220a 2020 2020 2020 2064 3d22 6d20 3431  ".       d="m 41
+0000e8d0: 352e 3332 3538 2c34 3538 2e33 3030 3532  5.3258,458.30052
+0000e8e0: 2031 342e 3538 3933 372c 322e 3136 3133   14.58937,2.1613
+0000e8f0: 3920 3230 2e36 3638 3238 2c2d 3134 2e35  9 20.66828,-14.5
+0000e900: 3839 3337 207a 220a 2020 2020 2020 2069  8937 z".       i
+0000e910: 643d 2270 6174 6831 3435 3631 2d39 2d32  d="path14561-9-2
+0000e920: 2d32 2d32 220a 2020 2020 2020 2069 6e6b  -2-2".       ink
+0000e930: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+0000e940: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+0000e950: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000e960: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000e970: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000e980: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000e990: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+0000e9a0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000e9b0: 6c3a 2330 3730 6532 623b 6669 6c6c 2d6f  l:#070e2b;fill-o
+0000e9c0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+0000e9d0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+0000e9e0: 6964 7468 3a30 2e38 3435 3032 353b 7374  idth:0.845025;st
+0000e9f0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+0000ea00: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+0000ea10: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+0000ea20: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000ea30: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000ea40: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+0000ea50: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+0000ea60: 3432 392e 3931 3531 372c 3436 302e 3436  429.91517,460.46
+0000ea70: 3139 3120 382e 3537 3830 312c 3131 2e32  191 8.57801,11.2
+0000ea80: 3739 3734 202d 332e 3137 3435 342c 2d31  7974 -3.17454,-1
+0000ea90: 352e 3139 3732 3620 7a22 0a20 2020 2020  5.19726 z".     
+0000eaa0: 2020 6964 3d22 7061 7468 3134 3536 332d    id="path14563-
+0000eab0: 312d 302d 362d 3922 0a20 2020 2020 2020  1-0-6-9".       
+0000eac0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+0000ead0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+0000eae0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000eaf0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+0000eb00: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000eb10: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+0000eb20: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
+0000eb30: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+0000eb40: 6669 6c6c 3a23 3238 3364 3837 3b66 696c  fill:#283d87;fil
+0000eb50: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000eb60: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000eb70: 652d 7769 6474 683a 302e 3834 3530 3235  e-width:0.845025
+0000eb80: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+0000eb90: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+0000eba0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+0000ebb0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+0000ebc0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+0000ebd0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+0000ebe0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+0000ebf0: 226d 2034 3335 2e33 3138 3634 2c34 3536  "m 435.31864,456
+0000ec00: 2e35 3434 3339 2033 2e31 3734 3534 2c31  .54439 3.17454,1
+0000ec10: 352e 3139 3732 3620 6320 312e 3634 3333  5.19726 c 1.6433
+0000ec20: 392c 2d31 332e 3636 3136 3220 372e 3432  9,-13.66162 7.42
+0000ec30: 3636 352c 2d31 382e 3538 3335 3320 3132  665,-18.58353 12
+0000ec40: 2e30 3930 3237 2c2d 3235 2e38 3639 3131  .09027,-25.86911
+0000ec50: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
+0000ec60: 6174 6831 3435 3635 2d39 2d35 2d39 2d31  ath14565-9-5-9-1
+0000ec70: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000ec80: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+0000ec90: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+0000eca0: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+0000ecb0: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
+0000ecc0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000ecd0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+0000ece0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000ecf0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+0000ed00: 3e0a 2020 2020 3c65 6c6c 6970 7365 0a20  >.    <ellipse. 
+0000ed10: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000ed20: 6c3a 2330 3730 6532 623b 6669 6c6c 2d6f  l:#070e2b;fill-o
+0000ed30: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
+0000ed40: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000ed50: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
+0000ed60: 3530 3235 3b73 7472 6f6b 652d 6d69 7465  5025;stroke-mite
+0000ed70: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000ed80: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000ed90: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+0000eda0: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+0000edb0: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
+0000edc0: 7061 7468 3134 3536 372d 362d 312d 392d  path14567-6-1-9-
+0000edd0: 3222 0a20 2020 2020 2020 6378 3d22 3430  2".       cx="40
+0000ede0: 382e 3531 3330 3922 0a20 2020 2020 2020  8.51309".       
+0000edf0: 6379 3d22 3434 312e 3633 3436 3122 0a20  cy="441.63461". 
+0000ee00: 2020 2020 2020 7278 3d22 302e 3834 3232        rx="0.8422
+0000ee10: 3139 3035 220a 2020 2020 2020 2072 793d  1905".       ry=
+0000ee20: 2230 2e38 3432 3231 3931 3122 0a20 2020  "0.84221911".   
+0000ee30: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000ee40: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+0000ee50: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000ee60: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+0000ee70: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
+0000ee80: 2020 2020 2020 2072 3d22 302e 3834 3232         r="0.8422
+0000ee90: 3139 3131 220a 2020 2020 2020 2073 7479  1911".       sty
+0000eea0: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
+0000eeb0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000eec0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000eed0: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
+0000eee0: 3530 3235 3b73 7472 6f6b 652d 6d69 7465  5025;stroke-mite
+0000eef0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000ef00: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000ef10: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+0000ef20: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+0000ef30: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
+0000ef40: 7061 7468 3134 3536 372d 332d 3933 2d31  path14567-3-93-1
+0000ef50: 2d36 2d37 220a 2020 2020 2020 2063 783d  -6-7".       cx=
+0000ef60: 2234 3135 2e31 3930 3238 220a 2020 2020  "415.19028".    
+0000ef70: 2020 2063 793d 2234 3538 2e31 3230 3835     cy="458.12085
+0000ef80: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000ef90: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000efa0: 6572 2d78 3d22 332e 3439 3233 3732 3322  er-x="3.4923723"
+0000efb0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000efc0: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+0000efd0: 722d 793d 222d 372e 3530 3438 3839 3722  r-y="-7.5048897"
+0000efe0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000eff0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+0000f000: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000f010: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+0000f020: 3330 3022 202f 3e0a 2020 2020 3c63 6972  300" />.    <cir
+0000f030: 636c 650a 2020 2020 2020 2072 3d22 302e  cle.       r="0.
+0000f040: 3834 3232 3139 3131 220a 2020 2020 2020  84221911".      
+0000f050: 2073 7479 6c65 3d22 6669 6c6c 3a23 3235   style="fill:#25
+0000f060: 3361 3764 3b66 696c 6c2d 6f70 6163 6974  3a7d;fill-opacit
+0000f070: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+0000f080: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+0000f090: 302e 3834 3530 3235 3b73 7472 6f6b 652d  0.845025;stroke-
+0000f0a0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000f0b0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000f0c0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+0000f0d0: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+0000f0e0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000f0f0: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
+0000f100: 372d 332d 302d 392d 3022 0a20 2020 2020  7-3-0-9-0".     
+0000f110: 2020 6378 3d22 3433 352e 3131 3335 3622    cx="435.11356"
+0000f120: 0a20 2020 2020 2020 6379 3d22 3435 312e  .       cy="451.
+0000f130: 3332 3939 3322 0a20 2020 2020 2020 696e  32993".       in
+0000f140: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
+0000f150: 2d63 656e 7465 722d 783d 2233 2e34 3932  -center-x="3.492
+0000f160: 3337 3136 220a 2020 2020 2020 2069 6e6b  3716".       ink
+0000f170: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
+0000f180: 6365 6e74 6572 2d79 3d22 2d37 2e35 3034  center-y="-7.504
+0000f190: 3839 3131 220a 2020 2020 2020 2069 6e6b  8911".       ink
+0000f1a0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+0000f1b0: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
+0000f1c0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+0000f1d0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+0000f1e0: 203c 6369 7263 6c65 0a20 2020 2020 2020   <circle.       
+0000f1f0: 723d 2230 2e38 3432 3231 3931 3122 0a20  r="0.84221911". 
+0000f200: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000f210: 6c3a 2361 3861 3961 613b 6669 6c6c 2d6f  l:#a8a9aa;fill-o
+0000f220: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+0000f230: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+0000f240: 6964 7468 3a30 2e38 3435 3032 353b 7374  idth:0.845025;st
+0000f250: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000f260: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000f270: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+0000f280: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+0000f290: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+0000f2a0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000f2b0: 3637 2d33 2d35 2d38 2d38 2d35 2d39 220a  67-3-5-8-8-5-9".
+0000f2c0: 2020 2020 2020 2063 783d 2234 3335 2e33         cx="435.3
+0000f2d0: 3133 3239 220a 2020 2020 2020 2063 793d  1329".       cy=
+0000f2e0: 2234 3536 2e34 3233 3122 0a20 2020 2020  "456.4231".     
+0000f2f0: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+0000f300: 666f 726d 2d63 656e 7465 722d 783d 2233  form-center-x="3
+0000f310: 2e34 3932 3337 3036 220a 2020 2020 2020  .4923706".      
+0000f320: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+0000f330: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d37  orm-center-y="-7
+0000f340: 2e35 3034 3839 3538 220a 2020 2020 2020  .5048958".      
+0000f350: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000f360: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+0000f370: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000f380: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+0000f390: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
+0000f3a0: 2020 2020 723d 2230 2e38 3432 3231 3931      r="0.8422191
+0000f3b0: 3122 0a20 2020 2020 2020 7374 796c 653d  1".       style=
+0000f3c0: 2266 696c 6c3a 2361 6261 6139 633b 6669  "fill:#abaa9c;fi
+0000f3d0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000f3e0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000f3f0: 6b65 2d77 6964 7468 3a30 2e38 3435 3032  ke-width:0.84502
+0000f400: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+0000f410: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000f420: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000f430: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+0000f440: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000f450: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000f460: 6831 3435 3637 2d33 2d39 2d30 2d39 2d38  h14567-3-9-0-9-8
+0000f470: 2d33 220a 2020 2020 2020 2063 783d 2234  -3".       cx="4
+0000f480: 3330 2e31 3230 3234 220a 2020 2020 2020  30.12024".      
+0000f490: 2063 793d 2234 3630 2e34 3137 3736 220a   cy="460.41776".
+0000f4a0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000f4b0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+0000f4c0: 2d78 3d22 332e 3439 3233 3731 3522 0a20  -x="3.4923715". 
+0000f4d0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+0000f4e0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+0000f4f0: 793d 222d 372e 3530 3438 3930 3722 0a20  y="-7.5048907". 
+0000f500: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000f510: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+0000f520: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000f530: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+0000f540: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
+0000f550: 650a 2020 2020 2020 2072 3d22 312e 3239  e.       r="1.29
+0000f560: 3938 3437 3122 0a20 2020 2020 2020 7374  98471".       st
+0000f570: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
+0000f580: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
+0000f590: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+0000f5a0: 7374 726f 6b65 2d77 6964 7468 3a30 2e38  stroke-width:0.8
+0000f5b0: 3435 3032 353b 7374 726f 6b65 2d6d 6974  45025;stroke-mit
+0000f5c0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+0000f5d0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+0000f5e0: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+0000f5f0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+0000f600: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+0000f610: 2270 6174 6831 3435 3637 2d33 2d32 2d35  "path14567-3-2-5
+0000f620: 2d34 2d33 2d36 220a 2020 2020 2020 2063  -4-3-6".       c
+0000f630: 783d 2234 3234 2e36 3237 3539 220a 2020  x="424.62759".  
+0000f640: 2020 2020 2063 793d 2234 3430 2e36 3934       cy="440.694
+0000f650: 3231 220a 2020 2020 2020 2069 6e6b 7363  21".       inksc
+0000f660: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+0000f670: 6e74 6572 2d78 3d22 352e 3338 3939 3932  nter-x="5.389992
+0000f680: 3422 0a20 2020 2020 2020 696e 6b73 6361  4".       inksca
+0000f690: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000f6a0: 7465 722d 793d 222d 3131 2e35 3832 3735  ter-y="-11.58275
+0000f6b0: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
+0000f6c0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000f6d0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000f6e0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000f6f0: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+0000f700: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
+0000f710: 302e 3834 3232 3139 3131 220a 2020 2020  0.84221911".    
+0000f720: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000f730: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
+0000f740: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+0000f750: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000f760: 6b65 2d77 6964 7468 3a30 2e38 3435 3032  ke-width:0.84502
+0000f770: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+0000f780: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000f790: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000f7a0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+0000f7b0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000f7c0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000f7d0: 6831 3435 3637 2d32 2d36 2d30 2d30 2d30  h14567-2-6-0-0-0
+0000f7e0: 220a 2020 2020 2020 2063 783d 2234 3331  ".       cx="431
+0000f7f0: 2e36 3638 3138 220a 2020 2020 2020 2063  .66818".       c
+0000f800: 793d 2234 3432 2e31 3432 3234 220a 2020  y="442.14224".  
+0000f810: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000f820: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000f830: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000f840: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000f850: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
+0000f860: 0a20 2020 2020 2020 723d 2230 2e38 3432  .       r="0.842
+0000f870: 3231 3931 3122 0a20 2020 2020 2020 7374  21911".       st
+0000f880: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
+0000f890: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
+0000f8a0: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+0000f8b0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000f8c0: 6474 683a 302e 3834 3530 3235 3b73 7472  dth:0.845025;str
+0000f8d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000f8e0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000f8f0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+0000f900: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+0000f910: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000f920: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+0000f930: 372d 322d 382d 362d 372d 382d 3622 0a20  7-2-8-6-7-8-6". 
+0000f940: 2020 2020 2020 6378 3d22 3431 372e 3038        cx="417.08
+0000f950: 3737 3422 0a20 2020 2020 2020 6379 3d22  774".       cy="
+0000f960: 3434 392e 3133 3238 3722 0a20 2020 2020  449.13287".     
+0000f970: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000f980: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+0000f990: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000f9a0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+0000f9b0: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
+0000f9c0: 2020 2020 2072 3d22 312e 3630 3039 3334       r="1.600934
+0000f9d0: 3722 0a20 2020 2020 2020 7374 796c 653d  7".       style=
+0000f9e0: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
+0000f9f0: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
+0000fa00: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
+0000fa10: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+0000fa20: 312e 3630 3632 353b 7374 726f 6b65 2d6d  1.60625;stroke-m
+0000fa30: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000fa40: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000fa50: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+0000fa60: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+0000fa70: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
+0000fa80: 643d 2270 6174 6831 3435 3637 2d32 2d37  d="path14567-2-7
+0000fa90: 2d30 2d39 2d30 2d32 220a 2020 2020 2020  -0-9-0-2".      
+0000faa0: 2063 783d 2234 3530 2e32 3933 3138 220a   cx="450.29318".
+0000fab0: 2020 2020 2020 2063 793d 2234 3436 2e30         cy="446.0
+0000fac0: 3836 3938 220a 2020 2020 2020 2069 6e6b  8698".       ink
+0000fad0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+0000fae0: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
+0000faf0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+0000fb00: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+0000fb10: 203c 670a 2020 2020 2020 2069 643d 2267   <g.       id="g
+0000fb20: 3133 3831 220a 2020 2020 2020 2074 7261  1381".       tra
+0000fb30: 6e73 666f 726d 3d22 6d61 7472 6978 2837  nsform="matrix(7
+0000fb40: 2e35 3531 3733 3834 2c30 2c30 2c37 2e35  .5517384,0,0,7.5
+0000fb50: 3531 3733 3834 2c2d 3639 332e 3835 3333  517384,-693.8533
+0000fb60: 352c 2d38 3235 2e30 3338 3539 2922 3e0a  5,-825.03859)">.
+0000fb70: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+0000fb80: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+0000fb90: 3a23 3365 3462 3737 3b66 696c 6c2d 6f70  :#3e4b77;fill-op
+0000fba0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+0000fbb0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000fbc0: 6474 683a 303b 7374 726f 6b65 2d6c 696e  dth:0;stroke-lin
+0000fbd0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+0000fbe0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+0000fbf0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+0000fc00: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+0000fc10: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+0000fc20: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+0000fc30: 2020 2020 2064 3d22 6d20 3135 342e 3135       d="m 154.15
+0000fc40: 3236 362c 3134 352e 3235 3030 3820 312e  266,145.25008 1.
+0000fc50: 3433 3734 382c 2d30 2e30 3635 3320 302e  43748,-0.0653 0.
+0000fc60: 3934 3434 372c 2d31 2e30 3531 3338 2063  94447,-1.05138 c
+0000fc70: 202d 312e 3138 3938 332c 302e 3830 3031   -1.18983,0.8001
+0000fc80: 3820 2d31 2e37 3538 3237 2c30 2e39 3238  8 -1.75827,0.928
+0000fc90: 3620 2d32 2e33 3831 3935 2c31 2e31 3136  6 -2.38195,1.116
+0000fca0: 3732 207a 220a 2020 2020 2020 2020 2069  72 z".         i
+0000fcb0: 643d 2270 6174 6831 3435 3437 2d31 2d37  d="path14547-1-7
+0000fcc0: 2d38 2d35 2d30 2d33 2d34 220a 2020 2020  -8-5-0-3-4".    
+0000fcd0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+0000fce0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+0000fcf0: 653d 2230 220a 2020 2020 2020 2020 2073  e="0".         s
+0000fd00: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+0000fd10: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
+0000fd20: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000fd30: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+0000fd40: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000fd50: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+0000fd60: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+0000fd70: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+0000fd80: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
+0000fd90: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000fda0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000fdb0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
+0000fdc0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+0000fdd0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+0000fde0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+0000fdf0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000fe00: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000fe10: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000fe20: 2020 2020 2020 2020 2064 3d22 6d20 3135           d="m 15
+0000fe30: 352e 3539 3031 342c 3134 352e 3138 3437  5.59014,145.1847
+0000fe40: 3820 322e 3239 3238 352c 302e 3433 3935  8 2.29285,0.4395
+0000fe50: 3220 6320 2d30 2e36 3530 3434 2c2d 302e  2 c -0.65044,-0.
+0000fe60: 3334 3338 3520 2d31 2e30 3237 312c 2d30  34385 -1.0271,-0
+0000fe70: 2e38 3936 3320 2d31 2e33 3438 3338 2c2d  .8963 -1.34838,-
+0000fe80: 312e 3439 3039 3420 7a22 0a20 2020 2020  1.49094 z".     
+0000fe90: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+0000fea0: 312d 302d 332d 392d 392d 342d 392d 3022  1-0-3-9-9-4-9-0"
+0000feb0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+0000fec0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+0000fed0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+0000fee0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+0000fef0: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
+0000ff00: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000ff10: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+0000ff20: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000ff30: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000ff40: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
+0000ff50: 7061 7468 0a20 2020 2020 2020 2020 7374  path.         st
+0000ff60: 796c 653d 2266 696c 6c3a 2332 3733 3737  yle="fill:#27377
+0000ff70: 333b 6669 6c6c 2d6f 7061 6369 7479 3a31  3;fill-opacity:1
+0000ff80: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+0000ff90: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
+0000ffa0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+0000ffb0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+0000ffc0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+0000ffd0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000ffe0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000fff0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00010000: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+00010010: 226d 2031 3534 2e31 3532 3636 2c31 3435  "m 154.15266,145
+00010020: 2e32 3530 3038 2063 2030 2e33 3136 3332  .25008 c 0.31632
+00010030: 2c30 2e31 3831 3437 2030 2e36 3635 3039  ,0.18147 0.66509
+00010040: 2c30 2e33 3337 3937 2030 2e37 3834 3038  ,0.33797 0.78408
+00010050: 2c30 2e36 3731 3232 206c 2030 2e36 3533  ,0.67122 l 0.653
+00010060: 342c 2d30 2e37 3336 3536 207a 220a 2020  4,-0.73656 z".  
+00010070: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00010080: 3435 3533 2d33 2d32 2d32 2d31 2d33 2d38  4553-3-2-2-1-3-8
+00010090: 2d39 220a 2020 2020 2020 2020 2069 6e6b  -9".         ink
+000100a0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+000100b0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+000100c0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000100d0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+000100e0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+000100f0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+00010100: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
+00010110: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+00010120: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+00010130: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00010140: 2073 7479 6c65 3d22 6669 6c6c 3a23 3134   style="fill:#14
+00010150: 3236 3732 3b66 696c 6c2d 6f70 6163 6974  2672;fill-opacit
+00010160: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00010170: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00010180: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
+00010190: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+000101a0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+000101b0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+000101c0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000101d0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+000101e0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+000101f0: 2064 3d22 6d20 3135 342e 3933 3637 342c   d="m 154.93674,
+00010200: 3134 352e 3932 3133 2032 2e39 3436 3235  145.9213 2.94625
+00010210: 2c2d 302e 3239 3720 2d32 2e32 3932 3835  ,-0.297 -2.29285
+00010220: 2c2d 302e 3433 3935 3620 7a22 0a20 2020  ,-0.43956 z".   
+00010230: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00010240: 3535 352d 342d 312d 362d 372d 322d 322d  555-4-1-6-7-2-2-
+00010250: 3322 0a20 2020 2020 2020 2020 696e 6b73  3".         inks
+00010260: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00010270: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+00010280: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00010290: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+000102a0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+000102b0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+000102c0: 3330 3022 202f 3e0a 2020 2020 2020 3c70  300" />.      <p
+000102d0: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
+000102e0: 6c65 3d22 6669 6c6c 3a23 3534 3636 3863  le="fill:#54668c
+000102f0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00010300: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00010310: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
+00010320: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00010330: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00010340: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+00010350: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00010360: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00010370: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+00010380: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+00010390: 6d20 3135 342e 3933 3637 342c 3134 352e  m 154.93674,145.
+000103a0: 3932 3133 2063 2030 2e30 3338 322c 302e  9213 c 0.0382,0.
+000103b0: 3332 3933 3820 2d30 2e30 3934 2c30 2e35  32938 -0.094,0.5
+000103c0: 3337 3033 202d 302e 3135 3434 342c 302e  3703 -0.15444,0.
+000103d0: 3739 3539 3720 6c20 332e 3130 3036 392c  79597 l 3.10069,
+000103e0: 2d31 2e30 3932 3937 207a 220a 2020 2020  -1.09297 z".    
+000103f0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00010400: 3539 2d33 2d34 2d32 2d34 2d34 2d33 2d35  59-3-4-2-4-4-3-5
+00010410: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00010420: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00010430: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00010440: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00010450: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
+00010460: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00010470: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00010480: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+00010490: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+000104a0: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
+000104b0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+000104c0: 7479 6c65 3d22 6669 6c6c 3a23 3038 3130  tyle="fill:#0810
+000104d0: 3639 3b66 696c 6c2d 6f70 6163 6974 793a  69;fill-opacity:
+000104e0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+000104f0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+00010500: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00010510: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00010520: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00010530: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00010540: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00010550: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00010560: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00010570: 3d22 6d20 3135 342e 3738 3233 2c31 3436  ="m 154.7823,146
+00010580: 2e37 3137 3237 2031 2e32 3833 3035 2c30  .71727 1.28305,0
+00010590: 2e31 3930 3038 2031 2e38 3137 3634 2c2d  .19008 1.81764,-
+000105a0: 312e 3238 3330 3520 7a22 0a20 2020 2020  1.28305 z".     
+000105b0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+000105c0: 312d 392d 322d 322d 382d 302d 312d 3722  1-9-2-2-8-0-1-7"
+000105d0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+000105e0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+000105f0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+00010600: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00010610: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00010620: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00010630: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00010640: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
+00010650: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00010660: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
+00010670: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00010680: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00010690: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
+000106a0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+000106b0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000106c0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+000106d0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+000106e0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+000106f0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00010700: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
+00010710: 3135 362e 3036 3533 352c 3134 362e 3930  156.06535,146.90
+00010720: 3733 3520 302e 3735 3433 382c 302e 3939  735 0.75438,0.99
+00010730: 3139 3820 2d30 2e32 3739 3138 2c2d 312e  198 -0.27918,-1.
+00010740: 3333 3635 207a 220a 2020 2020 2020 2020  3365 z".        
+00010750: 2069 643d 2270 6174 6831 3435 3633 2d31   id="path14563-1
+00010760: 2d30 2d36 2d38 2d37 2d32 2d32 220a 2020  -0-6-8-7-2-2".  
+00010770: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00010780: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00010790: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+000107a0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+000107b0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+000107c0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+000107d0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+000107e0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+000107f0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00010800: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
+00010810: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00010820: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00010830: 2d77 6964 7468 3a30 3b73 7472 6f6b 652d  -width:0;stroke-
+00010840: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00010850: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00010860: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+00010870: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00010880: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00010890: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+000108a0: 2020 2020 2020 2020 643d 226d 2031 3536          d="m 156
+000108b0: 2e30 3635 3335 2c31 3436 2e39 3037 3335  .06535,146.90735
+000108c0: 2030 2e37 3534 3338 2c30 2e39 3931 3938   0.75438,0.99198
+000108d0: 2063 2030 2e31 3434 3532 2c2d 312e 3230   c 0.14452,-1.20
+000108e0: 3134 3620 302e 3635 3331 322c 2d31 2e36  146 0.65312,-1.6
+000108f0: 3334 3320 312e 3036 3332 362c 2d32 2e32  343 1.06326,-2.2
+00010900: 3735 3033 207a 220a 2020 2020 2020 2020  7503 z".        
+00010910: 2069 643d 2270 6174 6831 3435 3635 2d39   id="path14565-9
+00010920: 2d35 2d39 2d37 2d37 2d33 2d34 220a 2020  -5-9-7-7-3-4".  
+00010930: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00010940: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00010950: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+00010960: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+00010970: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
+00010980: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00010990: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+000109a0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+000109b0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+000109c0: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
+000109d0: 636c 650a 2020 2020 2020 2020 2073 7479  cle.         sty
+000109e0: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
+000109f0: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
+00010a00: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
+00010a10: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00010a20: 7468 3a30 3b73 7472 6f6b 652d 6d69 7465  th:0;stroke-mite
+00010a30: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00010a40: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00010a50: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+00010a60: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+00010a70: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
+00010a80: 3d22 7061 7468 3134 3536 372d 362d 312d  ="path14567-6-1-
+00010a90: 392d 372d 372d 352d 3922 0a20 2020 2020  9-7-7-5-9".     
+00010aa0: 2020 2020 6378 3d22 3135 342e 3138 3331      cx="154.1831
+00010ab0: 3822 0a20 2020 2020 2020 2020 6379 3d22  8".         cy="
+00010ac0: 3134 352e 3235 3136 3222 0a20 2020 2020  145.25162".     
+00010ad0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00010ae0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00010af0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00010b00: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00010b10: 3022 0a20 2020 2020 2020 2020 723d 2230  0".         r="0
+00010b20: 2e30 3734 3036 3737 3739 2220 2f3e 0a20  .074067779" />. 
+00010b30: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
+00010b40: 2020 2020 2020 723d 2230 2e30 3734 3036        r="0.07406
+00010b50: 3737 3739 220a 2020 2020 2020 2020 2073  7779".         s
+00010b60: 7479 6c65 3d22 6669 6c6c 3a23 3235 3361  tyle="fill:#253a
+00010b70: 3764 3b66 696c 6c2d 6f70 6163 6974 793a  7d;fill-opacity:
+00010b80: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00010b90: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+00010ba0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00010bb0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00010bc0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00010bd0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00010be0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00010bf0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00010c00: 6831 3435 3637 2d33 2d39 332d 312d 362d  h14567-3-93-1-6-
+00010c10: 392d 332d 372d 3822 0a20 2020 2020 2020  9-3-7-8".       
+00010c20: 2020 6378 3d22 3135 342e 3737 3034 220a    cx="154.7704".
+00010c30: 2020 2020 2020 2020 2063 793d 2231 3436           cy="146
+00010c40: 2e37 3031 3438 220a 2020 2020 2020 2020  .70148".        
+00010c50: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00010c60: 6f72 6d2d 6365 6e74 6572 2d78 3d22 342e  orm-center-x="4.
+00010c70: 3634 3332 3536 3622 0a20 2020 2020 2020  6432566".       
+00010c80: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00010c90: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
+00010ca0: 392e 3937 3830 3632 3122 0a20 2020 2020  9.9780621".     
+00010cb0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00010cc0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00010cd0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00010ce0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00010cf0: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
+00010d00: 636c 650a 2020 2020 2020 2020 2072 3d22  cle.         r="
+00010d10: 302e 3037 3430 3637 3737 3922 0a20 2020  0.074067779".   
+00010d20: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00010d30: 6c3a 2361 6261 6139 633b 6669 6c6c 2d6f  l:#abaa9c;fill-o
+00010d40: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00010d50: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00010d60: 6964 7468 3a30 3b73 7472 6f6b 652d 6d69  idth:0;stroke-mi
+00010d70: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00010d80: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00010d90: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+00010da0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+00010db0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00010dc0: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
+00010dd0: 392d 302d 392d 382d 322d 382d 302d 3522  9-0-9-8-2-8-0-5"
+00010de0: 0a20 2020 2020 2020 2020 6378 3d22 3135  .         cx="15
+00010df0: 362e 3038 3334 220a 2020 2020 2020 2020  6.0834".        
+00010e00: 2063 793d 2231 3436 2e39 3033 3437 220a   cy="146.90347".
+00010e10: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00010e20: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+00010e30: 6572 2d78 3d22 342e 3634 3332 3536 3622  er-x="4.6432566"
+00010e40: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00010e50: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+00010e60: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
+00010e70: 3122 0a20 2020 2020 2020 2020 696e 6b73  1".         inks
+00010e80: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+00010e90: 3d22 3330 3022 0a20 2020 2020 2020 2020  ="300".         
+00010ea0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00010eb0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+00010ec0: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
+00010ed0: 2020 2020 2072 3d22 302e 3131 3433 3133       r="0.114313
+00010ee0: 3234 220a 2020 2020 2020 2020 2073 7479  24".         sty
+00010ef0: 6c65 3d22 6669 6c6c 3a23 3131 3230 3636  le="fill:#112066
+00010f00: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00010f10: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00010f20: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
+00010f30: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00010f40: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00010f50: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+00010f60: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+00010f70: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00010f80: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00010f90: 3435 3637 2d33 2d32 2d35 2d34 2d33 2d38  4567-3-2-5-4-3-8
+00010fa0: 2d30 2d37 2d37 220a 2020 2020 2020 2020  -0-7-7".        
+00010fb0: 2063 783d 2231 3535 2e36 3030 3336 220a   cx="155.60036".
+00010fc0: 2020 2020 2020 2020 2063 793d 2231 3435           cy="145
+00010fd0: 2e31 3638 3931 220a 2020 2020 2020 2020  .16891".        
+00010fe0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00010ff0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 372e  orm-center-x="7.
+00011000: 3136 3632 3131 3622 0a20 2020 2020 2020  1662116".       
+00011010: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00011020: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
+00011030: 3135 2e33 3939 3735 3122 0a20 2020 2020  15.399751".     
+00011040: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00011050: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00011060: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00011070: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00011080: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
+00011090: 636c 650a 2020 2020 2020 2020 2072 3d22  cle.         r="
+000110a0: 302e 3037 3430 3637 3737 3922 0a20 2020  0.074067779".   
+000110b0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+000110c0: 6c3a 2365 6466 3066 633b 6669 6c6c 2d6f  l:#edf0fc;fill-o
+000110d0: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
+000110e0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+000110f0: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
+00011100: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00011110: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00011120: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+00011130: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+00011140: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00011150: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00011160: 3435 3637 2d32 2d38 2d36 2d37 2d38 2d32  4567-2-8-6-7-8-2
+00011170: 2d32 2d36 2d39 220a 2020 2020 2020 2020  -2-6-9".        
+00011180: 2063 783d 2231 3534 2e39 3337 3237 220a   cx="154.93727".
+00011190: 2020 2020 2020 2020 2063 793d 2231 3435           cy="145
+000111a0: 2e39 3131 3034 220a 2020 2020 2020 2020  .91104".        
+000111b0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+000111c0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+000111d0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+000111e0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+000111f0: 2f3e 0a20 2020 2020 203c 6369 7263 6c65  />.      <circle
+00011200: 0a20 2020 2020 2020 2020 723d 2230 2e31  .         r="0.1
+00011210: 3430 3739 3139 3522 0a20 2020 2020 2020  4079195".       
+00011220: 2020 7374 796c 653d 2266 696c 6c3a 2365    style="fill:#e
+00011230: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
+00011240: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
+00011250: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00011260: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
+00011270: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00011280: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00011290: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+000112a0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+000112b0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+000112c0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+000112d0: 2d32 2d37 2d30 2d39 2d30 2d35 2d31 2d31  -2-7-0-9-0-5-1-1
+000112e0: 2d33 220a 2020 2020 2020 2020 2063 783d  -3".         cx=
+000112f0: 2231 3537 2e38 3537 3438 220a 2020 2020  "157.85748".    
+00011300: 2020 2020 2063 793d 2231 3435 2e36 3433       cy="145.643
+00011310: 3137 220a 2020 2020 2020 2020 2069 6e6b  17".         ink
+00011320: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+00011330: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
+00011340: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00011350: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00011360: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
+00011370: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00011380: 6e6f 6e65 3b66 696c 6c2d 7275 6c65 3a65  none;fill-rule:e
+00011390: 7665 6e6f 6464 3b73 7472 6f6b 653a 2366  venodd;stroke:#f
+000113a0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+000113b0: 7468 3a30 2e31 3332 3239 323b 7374 726f  th:0.132292;stro
+000113c0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+000113d0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000113e0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+000113f0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00011400: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00011410: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00011420: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
+00011430: 3135 342e 3135 3236 362c 3134 352e 3235  154.15266,145.25
+00011440: 3030 3820 6320 302e 3838 3934 382c 2d30  008 c 0.88948,-0
+00011450: 2e31 3831 3233 2031 2e36 3436 3433 2c2d  .18123 1.64643,-
+00011460: 302e 3632 3735 3220 322e 3338 3139 352c  0.62752 2.38195,
+00011470: 2d31 2e31 3136 3638 2030 2e33 3332 3436  -1.11668 0.33246
+00011480: 2c30 2e36 3034 3231 2030 2e36 3532 2c31  ,0.60421 0.652,1
+00011490: 2e32 3230 3237 2031 2e33 3438 3338 2c31  .22027 1.34838,1
+000114a0: 2e34 3930 3920 2d30 2e34 3232 3235 2c30  .4909 -0.42225,0
+000114b0: 2e35 3735 3635 202d 302e 3834 3235 372c  .57565 -0.84257,
+000114c0: 312e 3135 3635 3120 2d31 2e30 3633 3236  1.15651 -1.06326
+000114d0: 2c32 2e32 3735 3033 206c 202d 302e 3735  ,2.27503 l -0.75
+000114e0: 3433 382c 2d30 2e39 3931 3938 202d 312e  438,-0.99198 -1.
+000114f0: 3238 3330 352c 2d30 2e31 3930 3038 2063  28305,-0.19008 c
+00011500: 2030 2e31 3337 3936 2c2d 302e 3330 3835   0.13796,-0.3085
+00011510: 3620 302e 3230 3333 352c 2d30 2e35 3830  6 0.20335,-0.580
+00011520: 3834 2030 2e31 3534 3434 2c2d 302e 3739  84 0.15444,-0.79
+00011530: 3539 3720 2d30 2e32 3031 3734 2c2d 302e  597 -0.20174,-0.
+00011540: 3235 3335 3520 2d30 2e34 3537 3636 2c2d  25355 -0.45766,-
+00011550: 302e 3438 3030 3120 2d30 2e37 3834 3038  0.48001 -0.78408
+00011560: 2c2d 302e 3637 3132 3220 7a22 0a20 2020  ,-0.67122 z".   
+00011570: 2020 2020 2020 6964 3d22 7061 7468 3133        id="path13
+00011580: 3033 2d37 220a 2020 2020 2020 2020 2073  03-7".         s
+00011590: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+000115a0: 733d 2263 6363 6363 6363 6322 202f 3e0a  s="cccccccc" />.
+000115b0: 2020 2020 3c2f 673e 0a20 2020 203c 7061      </g>.    <pa
+000115c0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+000115d0: 2266 696c 6c3a 2333 6534 6237 373b 6669  "fill:#3e4b77;fi
+000115e0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000115f0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00011600: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
+00011610: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00011620: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00011630: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00011640: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00011650: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00011660: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00011670: 0a20 2020 2020 2020 643d 226d 2034 3731  .       d="m 471
+00011680: 2e35 3934 3531 2c33 3331 2e33 3733 3533  .59451,331.37353
+00011690: 2035 2e34 3332 3939 2c2d 302e 3234 3638   5.43299,-0.2468
+000116a0: 2033 2e35 3639 3635 2c2d 332e 3937 3337   3.56965,-3.9737
+000116b0: 3220 6320 2d34 2e34 3936 3939 2c33 2e30  2 c -4.49699,3.0
+000116c0: 3234 3320 2d36 2e36 3435 3433 2c33 2e35  243 -6.64543,3.5
+000116d0: 3039 3637 202d 392e 3030 3236 342c 342e  0967 -9.00264,4.
+000116e0: 3232 3036 3720 7a22 0a20 2020 2020 2020  22067 z".       
+000116f0: 6964 3d22 7061 7468 3134 3534 372d 312d  id="path14547-1-
+00011700: 372d 382d 352d 302d 3322 0a20 2020 2020  7-8-5-0-3".     
+00011710: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00011720: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00011730: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+00011740: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00011750: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
+00011760: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+00011770: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+00011780: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+00011790: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+000117a0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+000117b0: 653d 2266 696c 6c3a 2330 3630 3530 383b  e="fill:#060508;
+000117c0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+000117d0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+000117e0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
+000117f0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00011800: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00011810: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+00011820: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00011830: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00011840: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00011850: 3122 0a20 2020 2020 2020 643d 226d 2034  1".       d="m 4
+00011860: 3737 2e30 3237 352c 3333 312e 3132 3637  77.0275,331.1267
+00011870: 3320 382e 3636 3538 392c 312e 3636 3131  3 8.66589,1.6611
+00011880: 3820 6320 2d32 2e34 3538 3335 2c2d 312e  8 c -2.45835,-1.
+00011890: 3239 3935 3920 2d33 2e38 3831 3935 2c2d  29959 -3.88195,-
+000118a0: 332e 3338 3735 3920 2d35 2e30 3936 3234  3.38759 -5.09624
+000118b0: 2c2d 352e 3633 3530 3520 7a22 0a20 2020  ,-5.63505 z".   
+000118c0: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+000118d0: 312d 302d 332d 392d 392d 342d 3922 0a20  1-0-3-9-9-4-9". 
+000118e0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+000118f0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00011900: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
+00011910: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+00011920: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
+00011930: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00011940: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+00011950: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00011960: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00011970: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00011980: 7374 796c 653d 2266 696c 6c3a 2332 3733  style="fill:#273
+00011990: 3737 333b 6669 6c6c 2d6f 7061 6369 7479  773;fill-opacity
+000119a0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+000119b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+000119c0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+000119d0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000119e0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+000119f0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00011a00: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00011a10: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00011a20: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+00011a30: 226d 2034 3731 2e35 3934 3531 2c33 3331  "m 471.59451,331
+00011a40: 2e33 3733 3533 2063 2031 2e31 3935 3534  .37353 c 1.19554
+00011a50: 2c30 2e36 3835 3837 2032 2e35 3133 3732  ,0.68587 2.51372
+00011a60: 2c31 2e32 3737 3337 2032 2e39 3633 3435  ,1.27737 2.96345
+00011a70: 2c32 2e35 3336 3920 6c20 322e 3436 3935  ,2.5369 l 2.4695
+00011a80: 342c 2d32 2e37 3833 3835 207a 220a 2020  4,-2.78385 z".  
+00011a90: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00011aa0: 3533 2d33 2d32 2d32 2d31 2d33 2d38 220a  53-3-2-2-1-3-8".
+00011ab0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00011ac0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00011ad0: 7572 653d 2230 220a 2020 2020 2020 2073  ure="0".       s
+00011ae0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00011af0: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
+00011b00: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00011b10: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+00011b20: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00011b30: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+00011b40: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00011b50: 2073 7479 6c65 3d22 6669 6c6c 3a23 3134   style="fill:#14
+00011b60: 3236 3732 3b66 696c 6c2d 6f70 6163 6974  2672;fill-opacit
+00011b70: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00011b80: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00011b90: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
+00011ba0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00011bb0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00011bc0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00011bd0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00011be0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00011bf0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00011c00: 3d22 6d20 3437 342e 3535 3739 362c 3333  ="m 474.55796,33
+00011c10: 332e 3931 3034 3320 3131 2e31 3335 3433  3.91043 11.13543
+00011c20: 2c2d 312e 3132 3235 3220 2d38 2e36 3635  ,-1.12252 -8.665
+00011c30: 3839 2c2d 312e 3636 3133 3320 7a22 0a20  89,-1.66133 z". 
+00011c40: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00011c50: 3535 352d 342d 312d 362d 372d 322d 3222  555-4-1-6-7-2-2"
+00011c60: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00011c70: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00011c80: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+00011c90: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00011ca0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+00011cb0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00011cc0: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+00011cd0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00011ce0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3534   style="fill:#54
+00011cf0: 3636 3863 3b66 696c 6c2d 6f70 6163 6974  668c;fill-opacit
+00011d00: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00011d10: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00011d20: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
+00011d30: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00011d40: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00011d50: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00011d60: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00011d70: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00011d80: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00011d90: 3d22 6d20 3437 342e 3535 3739 362c 3333  ="m 474.55796,33
+00011da0: 332e 3931 3034 3320 6320 302e 3134 3433  3.91043 c 0.1443
+00011db0: 382c 312e 3234 3439 202d 302e 3335 3532  8,1.2449 -0.3552
+00011dc0: 382c 322e 3032 3937 3220 2d30 2e35 3833  8,2.02972 -0.583
+00011dd0: 3731 2c33 2e30 3038 3339 206c 2031 312e  71,3.00839 l 11.
+00011de0: 3731 3931 342c 2d34 2e31 3330 3931 207a  71914,-4.13091 z
+00011df0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00011e00: 6831 3435 3539 2d33 2d34 2d32 2d34 2d34  h14559-3-4-2-4-4
+00011e10: 2d33 220a 2020 2020 2020 2069 6e6b 7363  -3".       inksc
+00011e20: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00011e30: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00011e40: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00011e50: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
+00011e60: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00011e70: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00011e80: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00011e90: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00011ea0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00011eb0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00011ec0: 3a23 3038 3130 3639 3b66 696c 6c2d 6f70  :#081069;fill-op
+00011ed0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00011ee0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00011ef0: 6474 683a 303b 7374 726f 6b65 2d6c 696e  dth:0;stroke-lin
+00011f00: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00011f10: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00011f20: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00011f30: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00011f40: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00011f50: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00011f60: 2020 2064 3d22 6d20 3437 332e 3937 3432     d="m 473.9742
+00011f70: 352c 3333 362e 3931 3838 3220 342e 3834  5,336.91882 4.84
+00011f80: 3933 322c 302e 3731 3834 3120 362e 3836  932,0.71841 6.86
+00011f90: 3938 322c 2d34 2e38 3439 3332 207a 220a  982,-4.84932 z".
+00011fa0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00011fb0: 3435 3631 2d39 2d32 2d32 2d38 2d30 2d31  4561-9-2-2-8-0-1
+00011fc0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00011fd0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00011fe0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+00011ff0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00012000: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+00012010: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+00012020: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+00012030: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00012040: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+00012050: 3730 6532 623b 6669 6c6c 2d6f 7061 6369  70e2b;fill-opaci
+00012060: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00012070: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00012080: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
+00012090: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+000120a0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+000120b0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+000120c0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+000120d0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+000120e0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+000120f0: 643d 226d 2034 3738 2e38 3233 3537 2c33  d="m 478.82357,3
+00012100: 3337 2e36 3337 3233 2032 2e38 3531 322c  37.63723 2.8512,
+00012110: 332e 3734 3932 3220 2d31 2e30 3535 3137  3.74922 -1.05517
+00012120: 2c2d 352e 3035 3133 3420 7a22 0a20 2020  ,-5.05134 z".   
+00012130: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00012140: 332d 312d 302d 362d 382d 372d 3222 0a20  3-1-0-6-8-7-2". 
+00012150: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00012160: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00012170: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
+00012180: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+00012190: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+000121a0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+000121b0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+000121c0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+000121d0: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
+000121e0: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
+000121f0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00012200: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+00012210: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00012220: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00012230: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00012240: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00012250: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00012260: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00012270: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+00012280: 6d20 3437 382e 3832 3335 372c 3333 372e  m 478.82357,337.
+00012290: 3633 3732 3320 322e 3835 3132 2c33 2e37  63723 2.8512,3.7
+000122a0: 3439 3232 2063 2030 2e35 3436 3232 2c2d  4922 c 0.54622,-
+000122b0: 342e 3534 3039 3620 322e 3436 3834 392c  4.54096 2.46849,
+000122c0: 2d36 2e31 3736 3839 2034 2e30 3138 3632  -6.17689 4.01862
+000122d0: 2c2d 382e 3539 3835 3420 7a22 0a20 2020  ,-8.59854 z".   
+000122e0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+000122f0: 352d 392d 352d 392d 372d 372d 3322 0a20  5-9-5-9-7-7-3". 
+00012300: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00012310: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00012320: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
+00012330: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+00012340: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
+00012350: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00012360: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+00012370: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00012380: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00012390: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
+000123a0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+000123b0: 3730 6532 623b 6669 6c6c 2d6f 7061 6369  70e2b;fill-opaci
+000123c0: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
+000123d0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+000123e0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
+000123f0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00012400: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00012410: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+00012420: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+00012430: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00012440: 2069 643d 2270 6174 6831 3435 3637 2d36   id="path14567-6
+00012450: 2d31 2d39 2d37 2d37 2d35 220a 2020 2020  -1-9-7-7-5".    
+00012460: 2020 2063 783d 2234 3731 2e37 3039 3834     cx="471.70984
+00012470: 220a 2020 2020 2020 2063 793d 2233 3331  ".       cy="331
+00012480: 2e33 3739 3333 220a 2020 2020 2020 2069  .37933".       i
+00012490: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+000124a0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+000124b0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+000124c0: 2d79 6470 693d 2233 3030 220a 2020 2020  -ydpi="300".    
+000124d0: 2020 2072 3d22 302e 3237 3939 3431 3222     r="0.2799412"
+000124e0: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
+000124f0: 2020 2020 2020 2072 3d22 302e 3237 3939         r="0.2799
+00012500: 3431 3222 0a20 2020 2020 2020 7374 796c  412".       styl
+00012510: 653d 2266 696c 6c3a 2332 3533 6137 643b  e="fill:#253a7d;
+00012520: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00012530: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00012540: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
+00012550: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00012560: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00012570: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+00012580: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+00012590: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000125a0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+000125b0: 372d 332d 3933 2d31 2d36 2d39 2d33 2d37  7-3-93-1-6-9-3-7
+000125c0: 220a 2020 2020 2020 2063 783d 2234 3733  ".       cx="473
+000125d0: 2e39 3239 3236 220a 2020 2020 2020 2063  .92926".       c
+000125e0: 793d 2233 3336 2e38 3539 3133 220a 2020  y="336.85913".  
+000125f0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+00012600: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
+00012610: 3d22 342e 3634 3332 3536 3622 0a20 2020  ="4.6432566".   
+00012620: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+00012630: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
+00012640: 222d 392e 3937 3830 3632 3122 0a20 2020  "-9.9780621".   
+00012650: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00012660: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00012670: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00012680: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00012690: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
+000126a0: 2020 2020 2020 2072 3d22 302e 3237 3939         r="0.2799
+000126b0: 3431 3222 0a20 2020 2020 2020 7374 796c  412".       styl
+000126c0: 653d 2266 696c 6c3a 2361 6261 6139 633b  e="fill:#abaa9c;
+000126d0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+000126e0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+000126f0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
+00012700: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00012710: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00012720: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+00012730: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+00012740: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00012750: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00012760: 372d 332d 392d 302d 392d 382d 322d 382d  7-3-9-0-9-8-2-8-
+00012770: 3022 0a20 2020 2020 2020 6378 3d22 3437  0".       cx="47
+00012780: 382e 3839 3137 3822 0a20 2020 2020 2020  8.89178".       
+00012790: 6379 3d22 3333 372e 3632 3235 3922 0a20  cy="337.62259". 
+000127a0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+000127b0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+000127c0: 783d 2234 2e36 3433 3235 3636 220a 2020  x="4.6432566".  
+000127d0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+000127e0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+000127f0: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
+00012800: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00012810: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00012820: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00012830: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+00012840: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
+00012850: 0a20 2020 2020 2020 723d 2230 2e34 3332  .       r="0.432
+00012860: 3035 3030 3522 0a20 2020 2020 2020 7374  05005".       st
+00012870: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
+00012880: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
+00012890: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000128a0: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
+000128b0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+000128c0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+000128d0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+000128e0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+000128f0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00012900: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00012910: 3536 372d 332d 322d 352d 342d 332d 382d  567-3-2-5-4-3-8-
+00012920: 302d 3722 0a20 2020 2020 2020 6378 3d22  0-7".       cx="
+00012930: 3437 372e 3036 3631 220a 2020 2020 2020  477.0661".      
+00012940: 2063 793d 2233 3331 2e30 3636 3737 220a   cy="331.06677".
+00012950: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00012960: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+00012970: 2d78 3d22 372e 3136 3632 3131 3622 0a20  -x="7.1662116". 
+00012980: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+00012990: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+000129a0: 793d 222d 3135 2e33 3939 3735 3122 0a20  y="-15.399751". 
+000129b0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+000129c0: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+000129d0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000129e0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+000129f0: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
+00012a00: 650a 2020 2020 2020 2072 3d22 302e 3237  e.       r="0.27
+00012a10: 3939 3431 3222 0a20 2020 2020 2020 7374  99412".       st
+00012a20: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
+00012a30: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
+00012a40: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+00012a50: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00012a60: 6474 683a 303b 7374 726f 6b65 2d6d 6974  dth:0;stroke-mit
+00012a70: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00012a80: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00012a90: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00012aa0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00012ab0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+00012ac0: 2270 6174 6831 3435 3637 2d32 2d38 2d36  "path14567-2-8-6
+00012ad0: 2d37 2d38 2d32 2d32 2d36 220a 2020 2020  -7-8-2-2-6".    
+00012ae0: 2020 2063 783d 2234 3734 2e35 3539 3937     cx="474.55997
+00012af0: 220a 2020 2020 2020 2063 793d 2233 3333  ".       cy="333
+00012b00: 2e38 3731 3637 220a 2020 2020 2020 2069  .87167".       i
+00012b10: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00012b20: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+00012b30: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00012b40: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00012b50: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
+00012b60: 2020 723d 2230 2e35 3332 3132 3730 3822    r="0.53212708"
+00012b70: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+00012b80: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
+00012b90: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
+00012ba0: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
+00012bb0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+00012bc0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00012bd0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00012be0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00012bf0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00012c00: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00012c10: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00012c20: 3435 3637 2d32 2d37 2d30 2d39 2d30 2d35  4567-2-7-0-9-0-5
+00012c30: 2d31 2d31 220a 2020 2020 2020 2063 783d  -1-1".       cx=
+00012c40: 2234 3835 2e35 3936 3938 220a 2020 2020  "485.59698".    
+00012c50: 2020 2063 793d 2233 3332 2e38 3539 3235     cy="332.85925
+00012c60: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00012c70: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+00012c80: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+00012c90: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+00012ca0: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+00012cb0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+00012cc0: 2266 696c 6c3a 6e6f 6e65 3b66 696c 6c2d  "fill:none;fill-
+00012cd0: 7275 6c65 3a65 7665 6e6f 6464 3b73 7472  rule:evenodd;str
+00012ce0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00012cf0: 6b65 2d77 6964 7468 3a30 2e35 3030 3030  ke-width:0.50000
+00012d00: 313b 7374 726f 6b65 2d6c 696e 6563 6170  1;stroke-linecap
+00012d10: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00012d20: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00012d30: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00012d40: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00012d50: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00012d60: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00012d70: 3d22 6d20 3437 312e 3539 3435 312c 3333  ="m 471.59451,33
+00012d80: 312e 3337 3335 3320 6320 332e 3336 3138  1.37353 c 3.3618
+00012d90: 312c 2d30 2e36 3834 3936 2036 2e32 3232  1,-0.68496 6.222
+00012da0: 3732 2c2d 322e 3337 3137 3320 392e 3030  72,-2.37173 9.00
+00012db0: 3236 342c 2d34 2e32 3230 3532 2031 2e32  264,-4.22052 1.2
+00012dc0: 3536 3534 2c32 2e32 3833 3633 2032 2e34  5654,2.28363 2.4
+00012dd0: 3634 3236 2c34 2e36 3132 3034 2035 2e30  6426,4.61204 5.0
+00012de0: 3936 3234 2c35 2e36 3334 3920 2d31 2e35  9624,5.6349 -1.5
+00012df0: 3935 392c 322e 3137 3536 3820 2d33 2e31  959,2.17568 -3.1
+00012e00: 3834 3531 2c34 2e33 3731 3036 202d 342e  8451,4.37106 -4.
+00012e10: 3031 3836 322c 382e 3539 3835 3420 6c20  01862,8.59854 l 
+00012e20: 2d32 2e38 3531 322c 2d33 2e37 3439 3232  -2.8512,-3.74922
+00012e30: 202d 342e 3834 3933 322c 2d30 2e37 3138   -4.84932,-0.718
+00012e40: 3431 2063 2030 2e35 3231 3432 2c2d 312e  41 c 0.52142,-1.
+00012e50: 3136 3632 3120 302e 3736 3835 372c 2d32  16621 0.76857,-2
+00012e60: 2e31 3935 3320 302e 3538 3337 312c 2d33  .1953 0.58371,-3
+00012e70: 2e30 3038 3339 202d 302e 3736 3234 382c  .00839 -0.76248,
+00012e80: 2d30 2e39 3538 3320 2d31 2e37 3239 3734  -0.9583 -1.72974
+00012e90: 2c2d 312e 3831 3432 3120 2d32 2e39 3633  ,-1.81421 -2.963
+00012ea0: 3435 2c2d 322e 3533 3639 207a 220a 2020  45,-2.5369 z".  
+00012eb0: 2020 2020 2069 643d 2270 6174 6831 3330       id="path130
+00012ec0: 3322 0a20 2020 2020 2020 736f 6469 706f  3".       sodipo
+00012ed0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00012ee0: 6363 6363 6363 2220 2f3e 0a20 203c 2f67  cccccc" />.  </g
+00012ef0: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
```

### Comparing `saenopy-0.8.0/saenopy/load.py` & `saenopy-0.9.0/saenopy/unused/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,530 +1,529 @@
-import numpy as np
-__name2__ = __name__
-__name__ = "saenopy"
-from .solver import Solver
-
-
-def load_gmsh(filename):
-    nodes = None
-    tetrahedra = None
-    entities = {}
-
-    def read_node_block(file_iter):
-        line = next(file_iter)
-        entityDim, entityTag, parametric, numNodesInBlock = line.split()
-        first_index = 0
-        last_index = 1
-        indices = np.zeros(int(numNodesInBlock), dtype=int)
-        for i in range(int(numNodesInBlock)):
-            line = next(file_iter)
-            if i == 0:
-                first_index = int(line)
-            if i == int(numNodesInBlock)-1:
-                last_index = int(line)+1
-            indices[i] = int(line)
-            pass
-        if file_iter.nodes is None:
-            file_iter.nodes = np.zeros((int(last_index), 3))
-        if file_iter.nodes.shape[0] < last_index:
-            file_iter.nodes = np.concatenate((file_iter.nodes, np.zeros((last_index-file_iter.nodes.shape[0], 3))))
-        data = np.zeros((int(numNodesInBlock), 3))
-        for i in range(int(numNodesInBlock)):
-            line = next(file_iter)
-            if 1:#entityDim != "0" and entityDim != "1" and en:
-                data[i, :] = [float(s) for s in line.split()]
-        file_iter.nodes[indices, :] = data
-        return entityDim+"_"+entityTag, data, first_index
-
-    def read_nodes(file_iter):
-        if version_major == "4":
-            line = next(file_iter).split()
-            try:
-                numEntityBlocks, numNodes, minNodeTag, maxNodeTag = line
-            except ValueError:
-                numEntityBlocks, numNodes = line
-            for i in range(int(numEntityBlocks)):
-                tag, data, first_index = read_node_block(file_iter)
-                entities[tag]["nodes"] = data
-                entities[tag]["first_index"] = first_index
-        if version_major == "2":
-            global nodes
-            numNodes = int(next(file_iter))
-            file_iter.nodes = np.zeros((int(numNodes), int(3)))
-            for i in range(numNodes):
-                line = next(file_iter)
-                id, x, y, z = line.split()
-                file_iter.nodes[int(id)-1, :] = [float(x), float(y), float(z)]
-            return file_iter.nodes
-
-    def read_elements_block(file_iter):
-        line = next(file_iter)
-        entityDim, entityTag, elementType, numElementsInBlock = line.split()
-        nodes_per_type = {"1": 2, "2": 3, "3": 4, "4":4, "5":8, "6":6, "7":5, "8":3, "9":6, "10":9, "11":10, "12":27, "13":18, "14":14, "15": 1}
-        if elementType in nodes_per_type.keys():
-            data = np.zeros((int(numElementsInBlock), nodes_per_type[elementType]), dtype=int)
-            for i in range(int(numElementsInBlock)):
-                line = next(file_iter)
-                #if elementType == "5":
-                #    print("e", line)
-                data[i, :] = [int(s) for s in line.split()[1:]]
-            #if elementType == "4":
-            #    print(data, data.min(), data.max(), np.unique(data).shape)
-        else:
-            for i in range(int(numElementsInBlock)):
-                line = next(file_iter)
-            data = None
-        return entityDim+"_"+entityTag, data
-
-    def read_elements(file_iter):
-        if version_major == "4":
-            numEntityBlocks, numNodes, minNodeTag, maxNodeTag = next(file_iter).split()
-            for i in range(int(numEntityBlocks)):
-                tag, data = read_elements_block(file_iter)
-                #if entities[tag]["first_index"]:
-                #    data -= entities[tag]["first_index"]+1
-                entities[tag]["elements"] = data
-        if version_major == "2":
-            numElements = int(next(file_iter))
-            data = np.zeros((int(numElements), 4), dtype=int)
-            for i in range(numElements):
-                line = next(file_iter)
-                line = line.split()
-                id = line[0]
-                # only use thetrahedra
-                if line[1] == "4":
-                    a, b, c, d = line[-4:]
-                    data[int(id)-1, :] = [int(a), int(b), int(c), int(d)]
-            return data
-
-    def read_entities(file_iter):
-        numPoints, numCurves, numSurfaces, numVolumes = next(file_iter).split()
-        for i in range(int(numPoints)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["0_"+tag] = dict(type="point")
-        for i in range(int(numCurves)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["1_"+tag] = dict(type="curve")
-        for i in range(int(numSurfaces)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["2_"+tag] = dict(type="surface")
-        for i in range(int(numVolumes)):
-            line = next(file_iter)
-            data = line.split()
-            volumeTag, minX, minY, minZ, maxX, maxY, maxZ = data[:7]
-            numPhysicalTags = int(data[7])
-            phys_tags = []
-            for t in data[7:numPhysicalTags]:
-                phys_tags.append(int(t))
-            numBoundngSurfaces = int(data[7+numPhysicalTags])
-            surf_tags = []
-            for t in data[7+numPhysicalTags:7+numPhysicalTags+numBoundngSurfaces]:
-                surf_tags.append(int(t))
-            entities["3_"+volumeTag] = dict(type="volume", minX=float(minX), minY=float(maxY), minZ=float(minZ),
-                                                           maxX=float(maxX), maxY=float(maxY), maxZ=float(maxZ),
-                                                           physical_tags=phys_tags, surface_tags=surf_tags)
-
-    # def get the version and type
-    with open(filename, "rb") as fp:
-        file_iter = iter(fp)
-        for line in file_iter:
-            if line.startswith(b"$MeshFormat"):
-                line = next(file_iter)
-                version, file_type, data_size = line.split()
-                try:
-                    version_major, version_minor = version.split(b".")
-                except ValueError:
-                    version_major = version
-                    version_minor = "0"
-                if int(file_type) == 1:
-                    raise IOError("Gmesh reader does not support binary format")
-                if int(version_major) != 4 and int(version_major) != 2:
-                    raise IOError("Gmesh file version %s not supported" % version)
-
-    with open(filename, "r") as fp:
-        file_iter = iter(fp)
-        file_iter.nodes = None
-        for line in file_iter:
-            if line.startswith("$MeshFormat"):
-                line = next(file_iter)
-                version, file_type, data_size = line.split()
-                try:
-                    version_major, version_minor = version.split(".")
-                except ValueError:
-                    version_major = version
-                    version_minor = "0"
-            if line.startswith("$Entities"):
-                read_entities(file_iter)
-            if line.startswith("$Nodes"):
-                nodes = read_nodes(file_iter)
-            if line.startswith("$Elements"):
-                tetrahedra = read_elements(file_iter)
-        nodes = file_iter.nodes
-
-    for entityId in entities:
-        entity = entities[entityId]
-        #print("---- entity ----", entityId, entity["type"], len(entity["elements"]))
-        #print(entities[entityId])
-        if entity["type"] == "volume":
-            #nodes = entity["nodes"]
-            tetrahedra = entity["elements"]
-            print(tetrahedra.min(), tetrahedra.max())
-            #print("volumne", tetrahedra, entity)
-    #print(entities.keys())
-    #print(nodes[0])
-    #print(nodes[1])
-    #print(nodes[2])
-    #print(nodes[3])
-
-    if tetrahedra.shape[1] == 4:
-        from .solver import Solver
-        M = Solver()
-        tetrahedra -= 1
-        unique_indices = np.unique(tetrahedra[tetrahedra[:, 0] != -1])
-        index_lookup = np.ones(max([tetrahedra.max() + 1, unique_indices.max() + 1]), dtype=int) * np.nan
-        index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
-        M.setNodes(nodes)#[unique_indices, :])
-        M.setTetrahedra(tetrahedra)#index_lookup[tetrahedra])
-    else:
-        from .FiniteBodyForcesHex import FiniteBodyForces
-        M = FiniteBodyForces()
-        unique_indices = np.unique(tetrahedra)
-        index_lookup = np.ones(max([tetrahedra.max()+1, unique_indices.max()+1]), dtype=int)*np.nan
-        index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
-        M.setNodes(nodes[unique_indices, :])
-        M.setHexahedra(index_lookup[tetrahedra])
-
-    return M
-
-def ensure_array_length(arr, length):
-    if arr is None:
-        return np.zeros((length, 3))
-    if arr.shape[0] < length:
-        additional_arr = np.zeros((length - arr.shape[0], 3))
-        return np.concatenate((arr, additional_arr))
-    return arr
-
-class special_file_iter:
-    def __init__(self, fp):
-        self.iter = iter(fp)
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        l = next(self.iter)
-        return l.strip()
-
-    def get_next_n_lines(self, n):
-        for i in range(n):
-            yield next(self.iter)
-
-def gmsh_get_version(filename):
-    with open(filename, "r") as fp:
-        file_iter = special_file_iter(fp)
-        file_iter.nodes = None
-        for line in file_iter:
-            if line == "$MeshFormat":
-                line = next(file_iter)
-                version, file_type, data_size = line.split()
-                try:
-                    version_major, version_minor = version.split(".")
-                except ValueError:
-                    version_major = version
-                    version_minor = "0"
-    return version_major, version_minor
-
-def load_gmsh4(filename):
-    nodes = None
-    tetrahedra = None
-    entities = {}
-
-    def read_node_block(file_iter):
-        line = next(file_iter)
-        # print("read_node_block", line)
-        entityTag, entityDim, parametric, numNodesInBlock = line.split()
-        data = np.loadtxt(file_iter.get_next_n_lines(int(numNodesInBlock)), dtype=float).reshape(-1, 4)
-        # the first part contains the indices
-        indices = data[:, 0].astype(int)
-        # the second the point data
-        data = data[:, 1:]
-        # print(indices.min(), indices.max(), indices.shape, data.shape)
-        file_iter.nodes = ensure_array_length(file_iter.nodes, indices.max() + 1)
-        file_iter.nodes[indices, :] = data
-        return entityDim + "_" + entityTag, data, indices[0]
-
-    def read_nodes(file_iter):
-        line = next(file_iter).split()
-        try:
-            numEntityBlocks, numNodes, minNodeTag, maxNodeTag = line
-        except ValueError:
-            numEntityBlocks, numNodes = line
-
-        # iterate over all node blocks
-        for i in range(int(numEntityBlocks)):
-            tag, data, first_index = read_node_block(file_iter)
-            entities[tag]["nodes"] = data
-            entities[tag]["first_index"] = first_index
-
-    def read_elements_block(file_iter):
-        line = next(file_iter)
-        # print("read_elements_block", line)
-        entityTag, entityDim, elementType, numElementsInBlock = line.split()
-        nodes_per_type = {"1": 2, "2": 3, "3": 4, "4": 4, "5": 8, "6": 6, "7": 5, "8": 3, "9": 6, "10": 9, "11": 10,
-                          "12": 27, "13": 18, "14": 14, "15": 1}
-        if elementType in nodes_per_type.keys():
-            n = nodes_per_type[elementType]
-            data = np.loadtxt(file_iter.get_next_n_lines(int(numElementsInBlock)), dtype=int).reshape(-1, n + 1)[:, 1:]
-            # if elementType == "4":
-            #    print("44444", data, data.min(), data.max(), np.unique(data).shape, file_iter.nodes.shape)
-        else:
-            # ignore data
-            _ = [l for l in file_iter.get_next_n_lines(int(numElementsInBlock))]
-            data = None
-        return entityDim + "_" + entityTag, data
-
-    def read_elements(file_iter):
-        line = next(file_iter)
-        numEntityBlocks, numNodes = line.split()
-        for i in range(int(numEntityBlocks)):
-            tag, data = read_elements_block(file_iter)
-            entities[tag]["elements"] = data
-
-    def read_entities(file_iter):
-        numPoints, numCurves, numSurfaces, numVolumes = next(file_iter).split()
-        for i in range(int(numPoints)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["0_" + tag] = dict(type="point")
-        for i in range(int(numCurves)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["1_" + tag] = dict(type="curve")
-        for i in range(int(numSurfaces)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["2_" + tag] = dict(type="surface")
-        for i in range(int(numVolumes)):
-            line = next(file_iter)
-            data = line.split()
-            volumeTag, minX, minY, minZ, maxX, maxY, maxZ = data[:7]
-            numPhysicalTags = int(data[7])
-            phys_tags = []
-            for t in data[7:numPhysicalTags]:
-                phys_tags.append(int(t))
-            numBoundngSurfaces = int(data[7 + numPhysicalTags])
-            surf_tags = []
-            for t in data[7 + numPhysicalTags:7 + numPhysicalTags + numBoundngSurfaces]:
-                surf_tags.append(int(t))
-            entities["3_" + volumeTag] = dict(type="volume", minX=float(minX), minY=float(maxY), minZ=float(minZ),
-                                              maxX=float(maxX), maxY=float(maxY), maxZ=float(maxZ),
-                                              physical_tags=phys_tags, surface_tags=surf_tags)
-
-    with open(filename, "r") as fp:
-        file_iter = special_file_iter(fp)
-        file_iter.nodes = None
-        for line in file_iter:
-            if line == "$MeshFormat":
-                line = next(file_iter)
-                version, file_type, data_size = line.split()
-                try:
-                    version_major, version_minor = version.split(".")
-                except ValueError:
-                    version_major = version
-                    version_minor = "0"
-            if line == "$Entities":
-                read_entities(file_iter)
-            if line == "$Nodes":
-                nodes = read_nodes(file_iter)
-            if line == "$Elements":
-                tetrahedra = read_elements(file_iter)
-        nodes = file_iter.nodes
-
-    for entityId in entities:
-        entity = entities[entityId]
-        # print("---- entity ----", entityId, entity["type"], len(entity["elements"]))
-        # print(entities[entityId])
-        if entity["type"] == "volume":
-            # nodes = entity["nodes"]
-            tetrahedra = entity["elements"]
-            # print(tetrahedra.min(), tetrahedra.max())
-            # print("volumne", tetrahedra, entity)
-
-    return tetrahedra, nodes
-
-
-def load_gmsh(filename):
-    nodes = None
-    tetrahedra = None
-    entities = {}
-
-    def read_node_block(file_iter):
-        line = next(file_iter)
-        #print("read_node_block", line)
-        entityDim, entityTag, parametric, numNodesInBlock = line.split()
-        # the first part contains the indices
-        indices = np.loadtxt(file_iter.get_next_n_lines(int(numNodesInBlock)), dtype=int).reshape(-1)
-        # the second the point data
-        data = np.loadtxt(file_iter.get_next_n_lines(int(numNodesInBlock)), dtype=float)[..., :3].reshape(-1, 3)
-        #print(indices.min(), indices.max(), indices.shape, data.shape)
-        file_iter.nodes = ensure_array_length(file_iter.nodes, indices.max()+1)
-        file_iter.nodes[indices, :] = data
-        return entityDim+"_"+entityTag, data, indices[0]
-
-    def read_nodes(file_iter):
-        if version_major == "4":
-            line = next(file_iter).split()
-            try:
-                numEntityBlocks, numNodes, minNodeTag, maxNodeTag = line
-            except ValueError:
-                numEntityBlocks, numNodes = line
-
-            # iterate over all node blocks
-            for i in range(int(numEntityBlocks)):
-                tag, data, first_index = read_node_block(file_iter)
-                entities[tag]["nodes"] = data
-                entities[tag]["first_index"] = first_index
-        if version_major == "2":
-            global nodes
-            numNodes = int(next(file_iter))
-            file_iter.nodes = np.zeros((int(numNodes), int(3)))
-            for i in range(numNodes):
-                line = next(file_iter)
-                id, x, y, z = line.split()
-                file_iter.nodes[int(id)-1, :] = [float(x), float(y), float(z)]
-            return file_iter.nodes
-
-    def read_elements_block(file_iter):
-        line = next(file_iter)
-        #print("read_elements_block", line)
-        entityDim, entityTag, elementType, numElementsInBlock = line.split()
-        nodes_per_type = {"1": 2, "2": 3, "3": 4, "4":4, "5":8, "6":6, "7":5, "8":3, "9":6, "10":9, "11":10, "12":27, "13":18, "14":14, "15": 1}
-        if elementType in nodes_per_type.keys():
-            n = nodes_per_type[elementType]
-            data = np.loadtxt(file_iter.get_next_n_lines(int(numElementsInBlock)), dtype=int).reshape(-1, n+1)[:, 1:]
-            #if elementType == "4":
-            #    print("44444", data, data.min(), data.max(), np.unique(data).shape, file_iter.nodes.shape)
-        else:
-            # ignore data
-            _ = [l for l in file_iter.get_next_n_lines(int(numElementsInBlock))]
-            data = None
-        return entityDim+"_"+entityTag, data
-
-    def read_elements(file_iter):
-        if version_major == "4":
-            numEntityBlocks, numNodes, minNodeTag, maxNodeTag = next(file_iter).split()
-            for i in range(int(numEntityBlocks)):
-                tag, data = read_elements_block(file_iter)
-                entities[tag]["elements"] = data
-
-        if version_major == "2":
-            numElements = int(next(file_iter))
-            data = np.zeros((int(numElements), 4), dtype=int)
-            for i in range(numElements):
-                line = next(file_iter)
-                line = line.split()
-                id = line[0]
-                # only use thetrahedra
-                if line[1] == "4":
-                    a, b, c, d = line[-4:]
-                    data[int(id)-1, :] = [int(a), int(b), int(c), int(d)]
-            return data
-
-    def read_entities(file_iter):
-        numPoints, numCurves, numSurfaces, numVolumes = next(file_iter).split()
-        for i in range(int(numPoints)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["0_"+tag] = dict(type="point")
-        for i in range(int(numCurves)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["1_"+tag] = dict(type="curve")
-        for i in range(int(numSurfaces)):
-            line = next(file_iter)
-            tag, _ = line.split(maxsplit=1)
-            entities["2_"+tag] = dict(type="surface")
-        for i in range(int(numVolumes)):
-            line = next(file_iter)
-            data = line.split()
-            volumeTag, minX, minY, minZ, maxX, maxY, maxZ = data[:7]
-            numPhysicalTags = int(data[7])
-            phys_tags = []
-            for t in data[7:numPhysicalTags]:
-                phys_tags.append(int(t))
-            numBoundngSurfaces = int(data[7+numPhysicalTags])
-            surf_tags = []
-            for t in data[7+numPhysicalTags:7+numPhysicalTags+numBoundngSurfaces]:
-                surf_tags.append(int(t))
-            entities["3_"+volumeTag] = dict(type="volume", minX=float(minX), minY=float(maxY), minZ=float(minZ),
-                                                           maxX=float(maxX), maxY=float(maxY), maxZ=float(maxZ),
-                                                           physical_tags=phys_tags, surface_tags=surf_tags)
-
-    version_major, version_minor = gmsh_get_version(filename)
-
-    if version_major == "4" and version_minor == "0":
-        tetrahedra, nodes = load_gmsh4(filename)
-    else:
-        with open(filename, "r") as fp:
-            file_iter = special_file_iter(fp)
-            file_iter.nodes = None
-            for line in file_iter:
-                if line == "$MeshFormat":
-                    line = next(file_iter)
-                    version, file_type, data_size = line.split()
-                    try:
-                        version_major, version_minor = version.split(".")
-                    except ValueError:
-                        version_major = version
-                        version_minor = "0"
-                if line == "$Entities":
-                    read_entities(file_iter)
-                if line == "$Nodes":
-                    nodes = read_nodes(file_iter)
-                if line == "$Elements":
-                    tetrahedra = read_elements(file_iter)
-            nodes = file_iter.nodes
-
-        for entityId in entities:
-            entity = entities[entityId]
-            #print("---- entity ----", entityId, entity["type"], len(entity["elements"]))
-            #print(entities[entityId])
-            if entity["type"] == "volume":
-                #nodes = entity["nodes"]
-                tetrahedra = entity["elements"]
-                #print(tetrahedra.min(), tetrahedra.max())
-                #print("volumne", tetrahedra, entity)
-
-    if tetrahedra.shape[1] == 4:
-        from .solver import Solver
-        M = Solver()
-        #tetrahedra -= 1
-        #unique_indices = np.unique(tetrahedra)
-        #print(nodes.shape, tetrahedra.shape, tetrahedra.min(), tetrahedra.max())
-        #print(nodes[0])
-        #nodes[tetrahedra]
-        #index_lookup = np.ones(max([tetrahedra.max() + 1, unique_indices.max() + 1]), dtype=int) * np.nan
-        #index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
-        if 0:
-            M.setNodes(nodes[unique_indices, :])
-            M.setTetrahedra(index_lookup[tetrahedra])
-        else:
-            M.setNodes(nodes)
-            M.setTetrahedra(tetrahedra)
-    else:
-        from .FiniteBodyForcesHex import FiniteBodyForces
-        M = FiniteBodyForces()
-        unique_indices = np.unique(tetrahedra)
-        index_lookup = np.ones(max([tetrahedra.max()+1, unique_indices.max()+1]), dtype=int)*np.nan
-        index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
-        M.setNodes(nodes[unique_indices, :])
-        M.setHexahedra(index_lookup[tetrahedra])
-
-    return M
-
-
-if __name2__ == "__main__":
-    #load_gmsh(r"D:\Repositories\saenopy\david\mesh_rheology\plateplate_d20h1_s0.09.msh")
-    load_gmsh(r"D:\Repositories\saenopy\david\mesh_rheology\plateplate_d20h1_s0.05.msh")
+import numpy as np
+__name2__ = __name__
+__name__ = "saenopy"
+
+
+def load_gmsh(filename):
+    nodes = None
+    tetrahedra = None
+    entities = {}
+
+    def read_node_block(file_iter):
+        line = next(file_iter)
+        entityDim, entityTag, parametric, numNodesInBlock = line.split()
+        first_index = 0
+        last_index = 1
+        indices = np.zeros(int(numNodesInBlock), dtype=int)
+        for i in range(int(numNodesInBlock)):
+            line = next(file_iter)
+            if i == 0:
+                first_index = int(line)
+            if i == int(numNodesInBlock)-1:
+                last_index = int(line)+1
+            indices[i] = int(line)
+            pass
+        if file_iter.nodes is None:
+            file_iter.nodes = np.zeros((int(last_index), 3))
+        if file_iter.nodes.shape[0] < last_index:
+            file_iter.nodes = np.concatenate((file_iter.nodes, np.zeros((last_index-file_iter.nodes.shape[0], 3))))
+        data = np.zeros((int(numNodesInBlock), 3))
+        for i in range(int(numNodesInBlock)):
+            line = next(file_iter)
+            if 1:#entityDim != "0" and entityDim != "1" and en:
+                data[i, :] = [float(s) for s in line.split()]
+        file_iter.nodes[indices, :] = data
+        return entityDim+"_"+entityTag, data, first_index
+
+    def read_nodes(file_iter):
+        if version_major == "4":
+            line = next(file_iter).split()
+            try:
+                numEntityBlocks, numNodes, minNodeTag, maxNodeTag = line
+            except ValueError:
+                numEntityBlocks, numNodes = line
+            for i in range(int(numEntityBlocks)):
+                tag, data, first_index = read_node_block(file_iter)
+                entities[tag]["nodes"] = data
+                entities[tag]["first_index"] = first_index
+        if version_major == "2":
+            global nodes
+            numNodes = int(next(file_iter))
+            file_iter.nodes = np.zeros((int(numNodes), int(3)))
+            for i in range(numNodes):
+                line = next(file_iter)
+                id, x, y, z = line.split()
+                file_iter.nodes[int(id)-1, :] = [float(x), float(y), float(z)]
+            return file_iter.nodes
+
+    def read_elements_block(file_iter):
+        line = next(file_iter)
+        entityDim, entityTag, elementType, numElementsInBlock = line.split()
+        nodes_per_type = {"1": 2, "2": 3, "3": 4, "4":4, "5":8, "6":6, "7":5, "8":3, "9":6, "10":9, "11":10, "12":27, "13":18, "14":14, "15": 1}
+        if elementType in nodes_per_type.keys():
+            data = np.zeros((int(numElementsInBlock), nodes_per_type[elementType]), dtype=int)
+            for i in range(int(numElementsInBlock)):
+                line = next(file_iter)
+                #if elementType == "5":
+                #    print("e", line)
+                data[i, :] = [int(s) for s in line.split()[1:]]
+            #if elementType == "4":
+            #    print(data, data.min(), data.max(), np.unique(data).shape)
+        else:
+            for i in range(int(numElementsInBlock)):
+                line = next(file_iter)
+            data = None
+        return entityDim+"_"+entityTag, data
+
+    def read_elements(file_iter):
+        if version_major == "4":
+            numEntityBlocks, numNodes, minNodeTag, maxNodeTag = next(file_iter).split()
+            for i in range(int(numEntityBlocks)):
+                tag, data = read_elements_block(file_iter)
+                #if entities[tag]["first_index"]:
+                #    data -= entities[tag]["first_index"]+1
+                entities[tag]["elements"] = data
+        if version_major == "2":
+            numElements = int(next(file_iter))
+            data = np.zeros((int(numElements), 4), dtype=int)
+            for i in range(numElements):
+                line = next(file_iter)
+                line = line.split()
+                id = line[0]
+                # only use thetrahedra
+                if line[1] == "4":
+                    a, b, c, d = line[-4:]
+                    data[int(id)-1, :] = [int(a), int(b), int(c), int(d)]
+            return data
+
+    def read_entities(file_iter):
+        numPoints, numCurves, numSurfaces, numVolumes = next(file_iter).split()
+        for i in range(int(numPoints)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["0_"+tag] = dict(type="point")
+        for i in range(int(numCurves)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["1_"+tag] = dict(type="curve")
+        for i in range(int(numSurfaces)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["2_"+tag] = dict(type="surface")
+        for i in range(int(numVolumes)):
+            line = next(file_iter)
+            data = line.split()
+            volumeTag, minX, minY, minZ, maxX, maxY, maxZ = data[:7]
+            numPhysicalTags = int(data[7])
+            phys_tags = []
+            for t in data[7:numPhysicalTags]:
+                phys_tags.append(int(t))
+            numBoundngSurfaces = int(data[7+numPhysicalTags])
+            surf_tags = []
+            for t in data[7+numPhysicalTags:7+numPhysicalTags+numBoundngSurfaces]:
+                surf_tags.append(int(t))
+            entities["3_"+volumeTag] = dict(type="volume", minX=float(minX), minY=float(maxY), minZ=float(minZ),
+                                                           maxX=float(maxX), maxY=float(maxY), maxZ=float(maxZ),
+                                                           physical_tags=phys_tags, surface_tags=surf_tags)
+
+    # def get the version and type
+    with open(filename, "rb") as fp:
+        file_iter = iter(fp)
+        for line in file_iter:
+            if line.startswith(b"$MeshFormat"):
+                line = next(file_iter)
+                version, file_type, data_size = line.split()
+                try:
+                    version_major, version_minor = version.split(b".")
+                except ValueError:
+                    version_major = version
+                    version_minor = "0"
+                if int(file_type) == 1:
+                    raise IOError("Gmesh reader does not support binary format")
+                if int(version_major) != 4 and int(version_major) != 2:
+                    raise IOError("Gmesh file version %s not supported" % version)
+
+    with open(filename, "r") as fp:
+        file_iter = iter(fp)
+        file_iter.nodes = None
+        for line in file_iter:
+            if line.startswith("$MeshFormat"):
+                line = next(file_iter)
+                version, file_type, data_size = line.split()
+                try:
+                    version_major, version_minor = version.split(".")
+                except ValueError:
+                    version_major = version
+                    version_minor = "0"
+            if line.startswith("$Entities"):
+                read_entities(file_iter)
+            if line.startswith("$Nodes"):
+                nodes = read_nodes(file_iter)
+            if line.startswith("$Elements"):
+                tetrahedra = read_elements(file_iter)
+        nodes = file_iter.nodes
+
+    for entityId in entities:
+        entity = entities[entityId]
+        #print("---- entity ----", entityId, entity["type"], len(entity["elements"]))
+        #print(entities[entityId])
+        if entity["type"] == "volume":
+            #nodes = entity["nodes"]
+            tetrahedra = entity["elements"]
+            print(tetrahedra.min(), tetrahedra.max())
+            #print("volumne", tetrahedra, entity)
+    #print(entities.keys())
+    #print(nodes[0])
+    #print(nodes[1])
+    #print(nodes[2])
+    #print(nodes[3])
+
+    if tetrahedra.shape[1] == 4:
+        from .solver import Solver
+        M = Solver()
+        tetrahedra -= 1
+        unique_indices = np.unique(tetrahedra[tetrahedra[:, 0] != -1])
+        index_lookup = np.ones(max([tetrahedra.max() + 1, unique_indices.max() + 1]), dtype=int) * np.nan
+        index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
+        M.setNodes(nodes)#[unique_indices, :])
+        M.setTetrahedra(tetrahedra)#index_lookup[tetrahedra])
+    else:
+        from .FiniteBodyForcesHex import FiniteBodyForces
+        M = FiniteBodyForces()
+        unique_indices = np.unique(tetrahedra)
+        index_lookup = np.ones(max([tetrahedra.max()+1, unique_indices.max()+1]), dtype=int)*np.nan
+        index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
+        M.setNodes(nodes[unique_indices, :])
+        M.setHexahedra(index_lookup[tetrahedra])
+
+    return M
+
+def ensure_array_length(arr, length):
+    if arr is None:
+        return np.zeros((length, 3))
+    if arr.shape[0] < length:
+        additional_arr = np.zeros((length - arr.shape[0], 3))
+        return np.concatenate((arr, additional_arr))
+    return arr
+
+class special_file_iter:
+    def __init__(self, fp):
+        self.iter = iter(fp)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        l = next(self.iter)
+        return l.strip()
+
+    def get_next_n_lines(self, n):
+        for i in range(n):
+            yield next(self.iter)
+
+def gmsh_get_version(filename):
+    with open(filename, "r") as fp:
+        file_iter = special_file_iter(fp)
+        file_iter.nodes = None
+        for line in file_iter:
+            if line == "$MeshFormat":
+                line = next(file_iter)
+                version, file_type, data_size = line.split()
+                try:
+                    version_major, version_minor = version.split(".")
+                except ValueError:
+                    version_major = version
+                    version_minor = "0"
+    return version_major, version_minor
+
+def load_gmsh4(filename):
+    nodes = None
+    tetrahedra = None
+    entities = {}
+
+    def read_node_block(file_iter):
+        line = next(file_iter)
+        # print("read_node_block", line)
+        entityTag, entityDim, parametric, numNodesInBlock = line.split()
+        data = np.loadtxt(file_iter.get_next_n_lines(int(numNodesInBlock)), dtype=float).reshape(-1, 4)
+        # the first part contains the indices
+        indices = data[:, 0].astype(int)
+        # the second the point data
+        data = data[:, 1:]
+        # print(indices.min(), indices.max(), indices.shape, data.shape)
+        file_iter.nodes = ensure_array_length(file_iter.nodes, indices.max() + 1)
+        file_iter.nodes[indices, :] = data
+        return entityDim + "_" + entityTag, data, indices[0]
+
+    def read_nodes(file_iter):
+        line = next(file_iter).split()
+        try:
+            numEntityBlocks, numNodes, minNodeTag, maxNodeTag = line
+        except ValueError:
+            numEntityBlocks, numNodes = line
+
+        # iterate over all node blocks
+        for i in range(int(numEntityBlocks)):
+            tag, data, first_index = read_node_block(file_iter)
+            entities[tag]["nodes"] = data
+            entities[tag]["first_index"] = first_index
+
+    def read_elements_block(file_iter):
+        line = next(file_iter)
+        # print("read_elements_block", line)
+        entityTag, entityDim, elementType, numElementsInBlock = line.split()
+        nodes_per_type = {"1": 2, "2": 3, "3": 4, "4": 4, "5": 8, "6": 6, "7": 5, "8": 3, "9": 6, "10": 9, "11": 10,
+                          "12": 27, "13": 18, "14": 14, "15": 1}
+        if elementType in nodes_per_type.keys():
+            n = nodes_per_type[elementType]
+            data = np.loadtxt(file_iter.get_next_n_lines(int(numElementsInBlock)), dtype=int).reshape(-1, n + 1)[:, 1:]
+            # if elementType == "4":
+            #    print("44444", data, data.min(), data.max(), np.unique(data).shape, file_iter.nodes.shape)
+        else:
+            # ignore data
+            _ = [l for l in file_iter.get_next_n_lines(int(numElementsInBlock))]
+            data = None
+        return entityDim + "_" + entityTag, data
+
+    def read_elements(file_iter):
+        line = next(file_iter)
+        numEntityBlocks, numNodes = line.split()
+        for i in range(int(numEntityBlocks)):
+            tag, data = read_elements_block(file_iter)
+            entities[tag]["elements"] = data
+
+    def read_entities(file_iter):
+        numPoints, numCurves, numSurfaces, numVolumes = next(file_iter).split()
+        for i in range(int(numPoints)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["0_" + tag] = dict(type="point")
+        for i in range(int(numCurves)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["1_" + tag] = dict(type="curve")
+        for i in range(int(numSurfaces)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["2_" + tag] = dict(type="surface")
+        for i in range(int(numVolumes)):
+            line = next(file_iter)
+            data = line.split()
+            volumeTag, minX, minY, minZ, maxX, maxY, maxZ = data[:7]
+            numPhysicalTags = int(data[7])
+            phys_tags = []
+            for t in data[7:numPhysicalTags]:
+                phys_tags.append(int(t))
+            numBoundngSurfaces = int(data[7 + numPhysicalTags])
+            surf_tags = []
+            for t in data[7 + numPhysicalTags:7 + numPhysicalTags + numBoundngSurfaces]:
+                surf_tags.append(int(t))
+            entities["3_" + volumeTag] = dict(type="volume", minX=float(minX), minY=float(maxY), minZ=float(minZ),
+                                              maxX=float(maxX), maxY=float(maxY), maxZ=float(maxZ),
+                                              physical_tags=phys_tags, surface_tags=surf_tags)
+
+    with open(filename, "r") as fp:
+        file_iter = special_file_iter(fp)
+        file_iter.nodes = None
+        for line in file_iter:
+            if line == "$MeshFormat":
+                line = next(file_iter)
+                version, file_type, data_size = line.split()
+                try:
+                    version_major, version_minor = version.split(".")
+                except ValueError:
+                    version_major = version
+                    version_minor = "0"
+            if line == "$Entities":
+                read_entities(file_iter)
+            if line == "$Nodes":
+                nodes = read_nodes(file_iter)
+            if line == "$Elements":
+                tetrahedra = read_elements(file_iter)
+        nodes = file_iter.nodes
+
+    for entityId in entities:
+        entity = entities[entityId]
+        # print("---- entity ----", entityId, entity["type"], len(entity["elements"]))
+        # print(entities[entityId])
+        if entity["type"] == "volume":
+            # nodes = entity["nodes"]
+            tetrahedra = entity["elements"]
+            # print(tetrahedra.min(), tetrahedra.max())
+            # print("volumne", tetrahedra, entity)
+
+    return tetrahedra, nodes
+
+
+def load_gmsh(filename):
+    nodes = None
+    tetrahedra = None
+    entities = {}
+
+    def read_node_block(file_iter):
+        line = next(file_iter)
+        #print("read_node_block", line)
+        entityDim, entityTag, parametric, numNodesInBlock = line.split()
+        # the first part contains the indices
+        indices = np.loadtxt(file_iter.get_next_n_lines(int(numNodesInBlock)), dtype=int).reshape(-1)
+        # the second the point data
+        data = np.loadtxt(file_iter.get_next_n_lines(int(numNodesInBlock)), dtype=float)[..., :3].reshape(-1, 3)
+        #print(indices.min(), indices.max(), indices.shape, data.shape)
+        file_iter.nodes = ensure_array_length(file_iter.nodes, indices.max()+1)
+        file_iter.nodes[indices, :] = data
+        return entityDim+"_"+entityTag, data, indices[0]
+
+    def read_nodes(file_iter):
+        if version_major == "4":
+            line = next(file_iter).split()
+            try:
+                numEntityBlocks, numNodes, minNodeTag, maxNodeTag = line
+            except ValueError:
+                numEntityBlocks, numNodes = line
+
+            # iterate over all node blocks
+            for i in range(int(numEntityBlocks)):
+                tag, data, first_index = read_node_block(file_iter)
+                entities[tag]["nodes"] = data
+                entities[tag]["first_index"] = first_index
+        if version_major == "2":
+            global nodes
+            numNodes = int(next(file_iter))
+            file_iter.nodes = np.zeros((int(numNodes), int(3)))
+            for i in range(numNodes):
+                line = next(file_iter)
+                id, x, y, z = line.split()
+                file_iter.nodes[int(id)-1, :] = [float(x), float(y), float(z)]
+            return file_iter.nodes
+
+    def read_elements_block(file_iter):
+        line = next(file_iter)
+        #print("read_elements_block", line)
+        entityDim, entityTag, elementType, numElementsInBlock = line.split()
+        nodes_per_type = {"1": 2, "2": 3, "3": 4, "4":4, "5":8, "6":6, "7":5, "8":3, "9":6, "10":9, "11":10, "12":27, "13":18, "14":14, "15": 1}
+        if elementType in nodes_per_type.keys():
+            n = nodes_per_type[elementType]
+            data = np.loadtxt(file_iter.get_next_n_lines(int(numElementsInBlock)), dtype=int).reshape(-1, n+1)[:, 1:]
+            #if elementType == "4":
+            #    print("44444", data, data.min(), data.max(), np.unique(data).shape, file_iter.nodes.shape)
+        else:
+            # ignore data
+            _ = [l for l in file_iter.get_next_n_lines(int(numElementsInBlock))]
+            data = None
+        return entityDim+"_"+entityTag, data
+
+    def read_elements(file_iter):
+        if version_major == "4":
+            numEntityBlocks, numNodes, minNodeTag, maxNodeTag = next(file_iter).split()
+            for i in range(int(numEntityBlocks)):
+                tag, data = read_elements_block(file_iter)
+                entities[tag]["elements"] = data
+
+        if version_major == "2":
+            numElements = int(next(file_iter))
+            data = np.zeros((int(numElements), 4), dtype=int)
+            for i in range(numElements):
+                line = next(file_iter)
+                line = line.split()
+                id = line[0]
+                # only use thetrahedra
+                if line[1] == "4":
+                    a, b, c, d = line[-4:]
+                    data[int(id)-1, :] = [int(a), int(b), int(c), int(d)]
+            return data
+
+    def read_entities(file_iter):
+        numPoints, numCurves, numSurfaces, numVolumes = next(file_iter).split()
+        for i in range(int(numPoints)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["0_"+tag] = dict(type="point")
+        for i in range(int(numCurves)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["1_"+tag] = dict(type="curve")
+        for i in range(int(numSurfaces)):
+            line = next(file_iter)
+            tag, _ = line.split(maxsplit=1)
+            entities["2_"+tag] = dict(type="surface")
+        for i in range(int(numVolumes)):
+            line = next(file_iter)
+            data = line.split()
+            volumeTag, minX, minY, minZ, maxX, maxY, maxZ = data[:7]
+            numPhysicalTags = int(data[7])
+            phys_tags = []
+            for t in data[7:numPhysicalTags]:
+                phys_tags.append(int(t))
+            numBoundngSurfaces = int(data[7+numPhysicalTags])
+            surf_tags = []
+            for t in data[7+numPhysicalTags:7+numPhysicalTags+numBoundngSurfaces]:
+                surf_tags.append(int(t))
+            entities["3_"+volumeTag] = dict(type="volume", minX=float(minX), minY=float(maxY), minZ=float(minZ),
+                                                           maxX=float(maxX), maxY=float(maxY), maxZ=float(maxZ),
+                                                           physical_tags=phys_tags, surface_tags=surf_tags)
+
+    version_major, version_minor = gmsh_get_version(filename)
+
+    if version_major == "4" and version_minor == "0":
+        tetrahedra, nodes = load_gmsh4(filename)
+    else:
+        with open(filename, "r") as fp:
+            file_iter = special_file_iter(fp)
+            file_iter.nodes = None
+            for line in file_iter:
+                if line == "$MeshFormat":
+                    line = next(file_iter)
+                    version, file_type, data_size = line.split()
+                    try:
+                        version_major, version_minor = version.split(".")
+                    except ValueError:
+                        version_major = version
+                        version_minor = "0"
+                if line == "$Entities":
+                    read_entities(file_iter)
+                if line == "$Nodes":
+                    nodes = read_nodes(file_iter)
+                if line == "$Elements":
+                    tetrahedra = read_elements(file_iter)
+            nodes = file_iter.nodes
+
+        for entityId in entities:
+            entity = entities[entityId]
+            #print("---- entity ----", entityId, entity["type"], len(entity["elements"]))
+            #print(entities[entityId])
+            if entity["type"] == "volume":
+                #nodes = entity["nodes"]
+                tetrahedra = entity["elements"]
+                #print(tetrahedra.min(), tetrahedra.max())
+                #print("volumne", tetrahedra, entity)
+
+    if tetrahedra.shape[1] == 4:
+        from .solver import Solver
+        M = Solver()
+        #tetrahedra -= 1
+        #unique_indices = np.unique(tetrahedra)
+        #print(nodes.shape, tetrahedra.shape, tetrahedra.min(), tetrahedra.max())
+        #print(nodes[0])
+        #nodes[tetrahedra]
+        #index_lookup = np.ones(max([tetrahedra.max() + 1, unique_indices.max() + 1]), dtype=int) * np.nan
+        #index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
+        if 0:
+            M.setNodes(nodes[unique_indices, :])
+            M.setTetrahedra(index_lookup[tetrahedra])
+        else:
+            M.setNodes(nodes)
+            M.setTetrahedra(tetrahedra)
+    else:
+        from .FiniteBodyForcesHex import FiniteBodyForces
+        M = FiniteBodyForces()
+        unique_indices = np.unique(tetrahedra)
+        index_lookup = np.ones(max([tetrahedra.max()+1, unique_indices.max()+1]), dtype=int)*np.nan
+        index_lookup[unique_indices] = np.arange(len(unique_indices), dtype=int)
+        M.setNodes(nodes[unique_indices, :])
+        M.setHexahedra(index_lookup[tetrahedra])
+
+    return M
+
+
+if __name2__ == "__main__":
+    #load_gmsh(r"D:\Repositories\saenopy\david\mesh_rheology\plateplate_d20h1_s0.09.msh")
+    load_gmsh(r"D:\Repositories\saenopy\david\mesh_rheology\plateplate_d20h1_s0.05.msh")
```

### Comparing `saenopy-0.8.0/saenopy/macro.py` & `saenopy-0.9.0/saenopy/macro.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/materials.py` & `saenopy-0.9.0/saenopy/materials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from numba import njit
 import numba
-from saenopy.loadHelpers import Saveable
+from saenopy.saveable import Saveable
 
 
 def saveEpsilon(epsilon, fname, CFG):
     """
     Save the material function to a file, e.g. for further plotting.
     """
     imax = int(np.ceil((CFG["EPSMAX"] + 1.0) / CFG["EPSSTEP"]))
@@ -121,15 +121,15 @@
         return ["SemiAffineFiberMaterial", self.k, self.d0, self.lambda_s, self.ds]
 
     def __init__(self, k, d0=None, lambda_s=None, ds=None):
         # parameters
         self.k = k
         self.d0 = d0 if d0 is not None and d0 >= 0 else None    
         # buckling None (constant stiffness) and buckling zero (drop in stiffness) is not the same 
-        if d0 is not None and self.d0 < 1e-30:  # approximate the zero case
+        if self.d0 is not None and self.d0 < 1e-30:  # approximate the zero case
             self.d0 = 1e-30
         self.lambda_s = lambda_s if lambda_s is not None and lambda_s >= 0 else None
         self.ds = ds if ds is not None and ds >= 0 else None
         self.parameters = dict(k=k, d0=d0, lambda_s=lambda_s, ds=ds)
 
     def stiffness(self, s):
         self._check_parameters_valid()
```

### Comparing `saenopy-0.8.0/saenopy/meshViewer.py` & `saenopy-0.9.0/saenopy/unused/meshViewer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,345 +1,345 @@
-import numpy as np
-import base64
-
-def MeshViewer(R, L, F, U, f1, f2):
-    source = """
-    <!--<div id="info"><a href="http://threejs.org" target="_blank" rel="noopener">three.js</a> - dashed lines example</div>-->
-    <div id="container"></div>
-    
-    <script src="https://threejs.org/build/three.js"></script>
-    
-    <script src="https://threejs.org/examples/js/WebGL.js"></script>
-    <script src="https://threejs.org/examples/js/libs/stats.min.js"></script>
-    <script src="https://threejs.org/examples/js/libs/dat.gui.min.js"></script>
-    
-    <script src="https://threejs.org/examples/js/controls/OrbitControls.js"></script>
-    
-    <style>
-    
-    .dg li {
-        background: #f7f7f7 !important;
-    }
-    .dg {
-       color: #111;
-       text-shadow: none;
-    }
-    .dg.main .close-button {
-        background: none;
-    }
-    .dg.main .close-button:hover {
-       background: none;
-    }
-    .dg .cr.boolean {
-        border-left: 1px solid #cfcfcf;
-    }
-    .dg .cr.number {
-        border-left: 1px solid #cfcfcf;
-    }
-    .dg .c input[type=text] {
-        background: #fffefe00;
-        outline: none;
-        color: #111 !important;
-    }
-    .dg .c input[type=text]:hover {
-        background: #fffefe00;
-        outline: none;
-        color: #111 !important;
-    }
-    .dg .c .slider {
-        background: #d6d6d6;
-        cursor: ew-resize;
-        border-radius: 5px;
-    }
-    .dg .c .slider:hover {
-        background: #d6d6d6;
-    }
-    .dg .c .slider-fg {
-        background: #747575;
-        border-radius: 5px;
-    }
-    .dg .c .slider:hover .slider-fg {
-       background: #42a5f5;
-    }
-    .dg li:not(.folder) {
-        border: 1px solid #cfcfcf;
-        border-radius: 2px;
-    }
-    
-    </style>
-    
-    <script>
-    
-    function NewArray(type, base64) {
-        var binary_string =  window.atob(base64);
-        var len = binary_string.length;
-        var bytes = new Uint8Array( len );
-        for (var i = 0; i < len; i++)        {
-            bytes[i] = binary_string.charCodeAt(i);
-        }
-        return new type(bytes.buffer);
-    }
-    
-        //if ( WEBGL.isWebGLAvailable() === false ) {
-        //    document.body.appendChild( WEBGL.getWebGLErrorMessage() );
-        //}
-    
-        var renderer, scene, camera, stats, controls;
-        var objects = [];
-        var gui;
-    
-        factor_mesh = %f;
-        factor_force = %f;
-    
-        var WIDTH = window.innerWidth, HEIGHT = window.innerHeight;
-    
-        init();
-        animate();
-    
-        function init() {
-    
-            camera = new THREE.PerspectiveCamera( 60, WIDTH / HEIGHT, 1, 200 );
-            camera.position.z = 150;
-    
-            scene = new THREE.Scene();
-            scene.background = new THREE.Color( 0xFFFFFF);//0x111111 );
-            scene.fog = new THREE.Fog( 0xFFFFFF, 50, 200);
-    
-            renderer = new THREE.WebGLRenderer( { antialias: true } );
-            renderer.setPixelRatio( window.devicePixelRatio );
-            renderer.setSize( WIDTH, HEIGHT );
-    
-            var container = document.getElementById( 'container' );
-            container.appendChild( renderer.domElement );
-    
-            //stats = new Stats();
-            //container.appendChild( stats.dom );
-    
-            //
-            addMesh(%s, %s, %s, %s)
-            window.addEventListener( 'resize', onWindowResize, false );
-    
-            controls = new THREE.OrbitControls( camera, renderer.domElement );
-            //controls.minDistance = 10;
-            //controls.maxDistance = 500;
-            initGui();
-    
-        }
-    
-    
-        function addMesh(points1, lines1, F1, U1) {
-            points = points1;
-            lines = lines1;
-            F = F1;
-            U = U1;
-    
-            for(var i=0; i < points.length; i++) {
-                points[i] *= factor_mesh;
-                U[i] *= factor_mesh;
-            }
-    
-            //var h = size * 0.5;
-    
-            var geometry = new THREE.BufferGeometry();
-            var position = [];
-            //console.log(points.length, tets.length);
-        
-            for(var t=0; t < lines1.length/2; t++) {
-                        var t1 = lines1[t*2+0];
-                        var t2 = lines1[t*2+1];
-                        for(var x=0; x < 3; x++)
-                            position.push(points[t1*3+x]);
-                        for(var x=0; x < 3; x++)
-                            position.push(points[t2*3+x]);
-                //console.log(t);
-            }
-            console.log("ready");
-    
-            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
-    
-            //var geometryCube = cube( 50 );
-    
-            //var lineSegments = new THREE.LineSegments( geometry, new THREE.LineDashedMaterial( { color: 0xffaa00, dashSize: 3, gapSize: 1 } ) );
-            mesh_lines = new THREE.LineSegments( geometry, new THREE.LineBasicMaterial( { color: 0xffaa00, linewidth: 0.5, transparent: true, opacity: 0.5} ) );
-            mesh_lines.computeLineDistances();
-    
-            objects.push( mesh_lines );
-            scene.add( mesh_lines );
-    
-            var geometry = new THREE.BufferGeometry();
-            var position = [];
-            var force_tips = [];
-    
-            for(var i=0; i < U.length/3; i++) {
-                f_abs = Math.sqrt(F[i*3+0]**2 + F[i*3+1]**2 + F[i*3+2]**2);
-                factor = factor_force*factor_mesh;//1/f_abs/3000 * f_abs * 100000;
-                for(var x=0; x < 3; x++)
-                    position.push((points[i*3+x]));
-                for(var x=0; x < 3; x++) {
-                    position.push(points[i * 3 + x] + F[i * 3 + x] * factor);
-                    force_tips.push(points[i * 3 + x] + F[i * 3 + x] * factor);
-                }
-            }
-    
-            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
-    
-            force_mat = new THREE.LineBasicMaterial( { color: 0xaa0000, linewidth: 3,} );
-            force_lines = new THREE.LineSegments( geometry, force_mat );
-            force_lines.computeLineDistances();
-    
-            objects.push( force_lines );
-            scene.add( force_lines );
-    
-            var sprite = new THREE.TextureLoader().load( 'https://threejs.org/examples/textures/sprites/disc.png' );
-    
-            var geometry = new THREE.BufferGeometry();
-            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( points, 3 ) );
-            mesh_points = new THREE.Points( geometry, new THREE.PointsMaterial( { size: 8, sizeAttenuation: false, color: 0xffaa00, map: sprite, alphaTest: 0.5, transparent: true } ) );
-            scene.add( mesh_points );
-    
-            var geometry = new THREE.BufferGeometry();
-            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( force_tips, 3 ) );
-            force_points = new THREE.Points( geometry, new THREE.PointsMaterial( { size: 10, sizeAttenuation: false, color: 0xaa0000, map: sprite, alphaTest: 0.5, transparent: true } ) );
-            scene.add( force_points );
-    
-            // Displacements
-    
-            var geometry = new THREE.BufferGeometry();
-            var position = [];
-            var displacement_tips = [];
-    
-            for(var i=0; i < U.length/3; i++) {
-                for(var x=0; x < 3; x++)
-                    position.push((points[i*3+x]));
-                for(var x=0; x < 3; x++) {
-                    position.push(points[i * 3 + x] + U[i * 3 + x]);
-                    displacement_tips.push(points[i * 3 + x] + U[i * 3 + x]);
-                }
-            }
-    
-            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
-            displacement_mat = new THREE.LineBasicMaterial( { color: 0x00aa00, linewidth: 2,} );
-            displacement_lines = new THREE.LineSegments( geometry, displacement_mat );
-            displacement_lines.computeLineDistances();
-    
-            objects.push( displacement_lines );
-            scene.add( displacement_lines );
-    
-            var geometry = new THREE.BufferGeometry();
-            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( displacement_tips, 3 ) );
-            displacement_points = new THREE.Points( geometry, new THREE.PointsMaterial( { size: 10, sizeAttenuation: false, color: 0x00aa00, map: sprite, alphaTest: 0.5, transparent: true } ) );
-            scene.add( displacement_points );
-        }
-    
-        function onWindowResize() {
-            camera.aspect = window.innerWidth / window.innerHeight;
-            camera.updateProjectionMatrix();
-            renderer.setSize( window.innerWidth, window.innerHeight );
-        }
-    
-        function animate() {
-            requestAnimationFrame( animate );
-    
-            render();
-            renderer.render( scene, camera );
-            //stats.update();
-    
-        }
-    
-        function render() {
-    
-            var time = Date.now() * 0.001;
-    
-            scene.traverse( function ( object ) {
-    
-                //if ( object.isLine ) {
-    
-                    //object.rotation.y = 0.25 * time;
-                    //object.rotation.y = 0.25 * time;
-    
-                //}
-    
-            } );
-    
-            renderer.render( scene, camera );
-    
-        }
-    
-        function initGui() {
-            gui = new dat.GUI();
-            var param = {
-                'mesh': true,
-                'forces': true,
-                'force scale': 1,
-                'displacements': true,
-                'view_range' : 200,
-            };
-            gui.add( param, 'mesh' ).onChange( function ( val ) {
-                mesh_lines.visible = val;
-                mesh_points.visible = val;
-            } );
-            gui.add( param, 'forces' ).onChange( function ( val ) {
-                force_lines.visible = val;
-                force_points.visible = val;
-            } );
-    
-            gui.add( param, 'force scale', 1, 8, 0.1 ).onChange( function ( val ) {
-                var position = [];
-                var force_tips = [];
-    
-                for(var i=0; i < U.length/3; i++) {
-                    f_abs = Math.sqrt(F[i * 3 + 0] ** 2 + F[i * 3 + 1] ** 2 + F[i * 3 + 2] ** 2);
-                    factor = factor_force * factor_mesh * val;//1/f_abs/3000 * f_abs * 100000;
-                    for (var x = 0; x < 3; x++)
-                        position.push((points[i * 3 + x]));
-                    for (var x = 0; x < 3; x++) {
-                        position.push(points[i * 3 + x] + F[i * 3 + x] * factor);
-                        force_tips.push(points[i * 3 + x] + F[i * 3 + x] * factor);
-                    }
-                }
-                force_lines.geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
-                force_points.geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( force_tips, 3 ) );
-            } );
-    
-            gui.add( param, 'displacements' ).onChange( function ( val ) {
-                displacement_lines.visible = val;
-                displacement_points.visible = val;
-            } );
-    
-            gui.add( param, 'view_range', 10, 300, 1 ).onChange( function ( val ) {
-                scene.fog.far = val;
-            } );
-        }
-    
-    </script>
-    """
-    source = source.replace("'", "\"")
-
-    def wrap(array):
-        if array.dtype == "float32":
-            data_type = "Float32Array"
-        elif array.dtype == "float64":
-            data_type = "Float64Array"
-        elif array.dtype == "int8":
-            data_type = "Int8Array"
-        elif array.dtype == "uint8":
-            data_type = "Uint8Array"
-        elif array.dtype == "int16":
-            data_type = "Int16Array"
-        elif array.dtype == "uint16":
-            data_type = "Uint16Array"
-        elif array.dtype == "int32":
-            data_type = "Int32Array"
-        elif array.dtype == "uint32":
-            data_type = "Uint32Array"
-        elif array.dtype == "int64":
-            data_type = "BigInt64Array"
-        elif array.dtype == "uint64":
-            data_type = "BigUint64Array"
-        else:
-            raise TypeError(array.dtype)
-        return "NewArray("+data_type+", \""+repr(base64.b64encode(array))[2:-1]+"\")"
-
-    here = source % (f1, f2, wrap(R-np.mean(R, axis=0)), wrap(L), wrap(F), wrap(U))
-    from IPython.core.display import HTML, display
-    code = "<h1></h1><iframe srcdoc='{0}' scrolling=no style='border:none; width: 100%; height: 600px'></iframe>".format(here)
-    display(HTML(code))
+import numpy as np
+import base64
+
+def MeshViewer(R, L, F, U, f1, f2):
+    source = """
+    <!--<div id="info"><a href="http://threejs.org" target="_blank" rel="noopener">three.js</a> - dashed lines example</div>-->
+    <div id="container"></div>
+    
+    <script src="https://threejs.org/build/three.js"></script>
+    
+    <script src="https://threejs.org/examples/js/WebGL.js"></script>
+    <script src="https://threejs.org/examples/js/libs/stats.min.js"></script>
+    <script src="https://threejs.org/examples/js/libs/dat.gui.min.js"></script>
+    
+    <script src="https://threejs.org/examples/js/controls/OrbitControls.js"></script>
+    
+    <style>
+    
+    .dg li {
+        background: #f7f7f7 !important;
+    }
+    .dg {
+       color: #111;
+       text-shadow: none;
+    }
+    .dg.main .close-button {
+        background: none;
+    }
+    .dg.main .close-button:hover {
+       background: none;
+    }
+    .dg .cr.boolean {
+        border-left: 1px solid #cfcfcf;
+    }
+    .dg .cr.number {
+        border-left: 1px solid #cfcfcf;
+    }
+    .dg .c input[type=text] {
+        background: #fffefe00;
+        outline: none;
+        color: #111 !important;
+    }
+    .dg .c input[type=text]:hover {
+        background: #fffefe00;
+        outline: none;
+        color: #111 !important;
+    }
+    .dg .c .slider {
+        background: #d6d6d6;
+        cursor: ew-resize;
+        border-radius: 5px;
+    }
+    .dg .c .slider:hover {
+        background: #d6d6d6;
+    }
+    .dg .c .slider-fg {
+        background: #747575;
+        border-radius: 5px;
+    }
+    .dg .c .slider:hover .slider-fg {
+       background: #42a5f5;
+    }
+    .dg li:not(.folder) {
+        border: 1px solid #cfcfcf;
+        border-radius: 2px;
+    }
+    
+    </style>
+    
+    <script>
+    
+    function NewArray(type, base64) {
+        var binary_string =  window.atob(base64);
+        var len = binary_string.length;
+        var bytes = new Uint8Array( len );
+        for (var i = 0; i < len; i++)        {
+            bytes[i] = binary_string.charCodeAt(i);
+        }
+        return new type(bytes.buffer);
+    }
+    
+        //if ( WEBGL.isWebGLAvailable() === false ) {
+        //    document.body.appendChild( WEBGL.getWebGLErrorMessage() );
+        //}
+    
+        var renderer, scene, camera, stats, controls;
+        var objects = [];
+        var gui;
+    
+        factor_mesh = %f;
+        factor_force = %f;
+    
+        var WIDTH = window.innerWidth, HEIGHT = window.innerHeight;
+    
+        init();
+        animate();
+    
+        function init() {
+    
+            camera = new THREE.PerspectiveCamera( 60, WIDTH / HEIGHT, 1, 200 );
+            camera.position.z = 150;
+    
+            scene = new THREE.Scene();
+            scene.background = new THREE.Color( 0xFFFFFF);//0x111111 );
+            scene.fog = new THREE.Fog( 0xFFFFFF, 50, 200);
+    
+            renderer = new THREE.WebGLRenderer( { antialias: true } );
+            renderer.setPixelRatio( window.devicePixelRatio );
+            renderer.setSize( WIDTH, HEIGHT );
+    
+            var container = document.getElementById( 'container' );
+            container.appendChild( renderer.domElement );
+    
+            //stats = new Stats();
+            //container.appendChild( stats.dom );
+    
+            //
+            addMesh(%s, %s, %s, %s)
+            window.addEventListener( 'resize', onWindowResize, false );
+    
+            controls = new THREE.OrbitControls( camera, renderer.domElement );
+            //controls.minDistance = 10;
+            //controls.maxDistance = 500;
+            initGui();
+    
+        }
+    
+    
+        function addMesh(points1, lines1, F1, U1) {
+            points = points1;
+            lines = lines1;
+            F = F1;
+            U = U1;
+    
+            for(var i=0; i < points.length; i++) {
+                points[i] *= factor_mesh;
+                U[i] *= factor_mesh;
+            }
+    
+            //var h = size * 0.5;
+    
+            var geometry = new THREE.BufferGeometry();
+            var position = [];
+            //console.log(points.length, tets.length);
+        
+            for(var t=0; t < lines1.length/2; t++) {
+                        var t1 = lines1[t*2+0];
+                        var t2 = lines1[t*2+1];
+                        for(var x=0; x < 3; x++)
+                            position.push(points[t1*3+x]);
+                        for(var x=0; x < 3; x++)
+                            position.push(points[t2*3+x]);
+                //console.log(t);
+            }
+            console.log("ready");
+    
+            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
+    
+            //var geometryCube = cube( 50 );
+    
+            //var lineSegments = new THREE.LineSegments( geometry, new THREE.LineDashedMaterial( { color: 0xffaa00, dashSize: 3, gapSize: 1 } ) );
+            mesh_lines = new THREE.LineSegments( geometry, new THREE.LineBasicMaterial( { color: 0xffaa00, linewidth: 0.5, transparent: true, opacity: 0.5} ) );
+            mesh_lines.computeLineDistances();
+    
+            objects.push( mesh_lines );
+            scene.add( mesh_lines );
+    
+            var geometry = new THREE.BufferGeometry();
+            var position = [];
+            var force_tips = [];
+    
+            for(var i=0; i < U.length/3; i++) {
+                f_abs = Math.sqrt(F[i*3+0]**2 + F[i*3+1]**2 + F[i*3+2]**2);
+                factor = factor_force*factor_mesh;//1/f_abs/3000 * f_abs * 100000;
+                for(var x=0; x < 3; x++)
+                    position.push((points[i*3+x]));
+                for(var x=0; x < 3; x++) {
+                    position.push(points[i * 3 + x] + F[i * 3 + x] * factor);
+                    force_tips.push(points[i * 3 + x] + F[i * 3 + x] * factor);
+                }
+            }
+    
+            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
+    
+            force_mat = new THREE.LineBasicMaterial( { color: 0xaa0000, linewidth: 3,} );
+            force_lines = new THREE.LineSegments( geometry, force_mat );
+            force_lines.computeLineDistances();
+    
+            objects.push( force_lines );
+            scene.add( force_lines );
+    
+            var sprite = new THREE.TextureLoader().load( 'https://threejs.org/examples/textures/sprites/disc.png' );
+    
+            var geometry = new THREE.BufferGeometry();
+            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( points, 3 ) );
+            mesh_points = new THREE.Points( geometry, new THREE.PointsMaterial( { size: 8, sizeAttenuation: false, color: 0xffaa00, map: sprite, alphaTest: 0.5, transparent: true } ) );
+            scene.add( mesh_points );
+    
+            var geometry = new THREE.BufferGeometry();
+            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( force_tips, 3 ) );
+            force_points = new THREE.Points( geometry, new THREE.PointsMaterial( { size: 10, sizeAttenuation: false, color: 0xaa0000, map: sprite, alphaTest: 0.5, transparent: true } ) );
+            scene.add( force_points );
+    
+            // Displacements
+    
+            var geometry = new THREE.BufferGeometry();
+            var position = [];
+            var displacement_tips = [];
+    
+            for(var i=0; i < U.length/3; i++) {
+                for(var x=0; x < 3; x++)
+                    position.push((points[i*3+x]));
+                for(var x=0; x < 3; x++) {
+                    position.push(points[i * 3 + x] + U[i * 3 + x]);
+                    displacement_tips.push(points[i * 3 + x] + U[i * 3 + x]);
+                }
+            }
+    
+            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
+            displacement_mat = new THREE.LineBasicMaterial( { color: 0x00aa00, linewidth: 2,} );
+            displacement_lines = new THREE.LineSegments( geometry, displacement_mat );
+            displacement_lines.computeLineDistances();
+    
+            objects.push( displacement_lines );
+            scene.add( displacement_lines );
+    
+            var geometry = new THREE.BufferGeometry();
+            geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( displacement_tips, 3 ) );
+            displacement_points = new THREE.Points( geometry, new THREE.PointsMaterial( { size: 10, sizeAttenuation: false, color: 0x00aa00, map: sprite, alphaTest: 0.5, transparent: true } ) );
+            scene.add( displacement_points );
+        }
+    
+        function onWindowResize() {
+            camera.aspect = window.innerWidth / window.innerHeight;
+            camera.updateProjectionMatrix();
+            renderer.setSize( window.innerWidth, window.innerHeight );
+        }
+    
+        function animate() {
+            requestAnimationFrame( animate );
+    
+            render();
+            renderer.render( scene, camera );
+            //stats.update();
+    
+        }
+    
+        function render() {
+    
+            var time = Date.now() * 0.001;
+    
+            scene.traverse( function ( object ) {
+    
+                //if ( object.isLine ) {
+    
+                    //object.rotation.y = 0.25 * time;
+                    //object.rotation.y = 0.25 * time;
+    
+                //}
+    
+            } );
+    
+            renderer.render( scene, camera );
+    
+        }
+    
+        function initGui() {
+            gui = new dat.GUI();
+            var param = {
+                'mesh': true,
+                'forces': true,
+                'force scale': 1,
+                'displacements': true,
+                'view_range' : 200,
+            };
+            gui.add( param, 'mesh' ).onChange( function ( val ) {
+                mesh_lines.visible = val;
+                mesh_points.visible = val;
+            } );
+            gui.add( param, 'forces' ).onChange( function ( val ) {
+                force_lines.visible = val;
+                force_points.visible = val;
+            } );
+    
+            gui.add( param, 'force scale', 1, 8, 0.1 ).onChange( function ( val ) {
+                var position = [];
+                var force_tips = [];
+    
+                for(var i=0; i < U.length/3; i++) {
+                    f_abs = Math.sqrt(F[i * 3 + 0] ** 2 + F[i * 3 + 1] ** 2 + F[i * 3 + 2] ** 2);
+                    factor = factor_force * factor_mesh * val;//1/f_abs/3000 * f_abs * 100000;
+                    for (var x = 0; x < 3; x++)
+                        position.push((points[i * 3 + x]));
+                    for (var x = 0; x < 3; x++) {
+                        position.push(points[i * 3 + x] + F[i * 3 + x] * factor);
+                        force_tips.push(points[i * 3 + x] + F[i * 3 + x] * factor);
+                    }
+                }
+                force_lines.geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( position, 3 ) );
+                force_points.geometry.addAttribute( 'position', new THREE.Float32BufferAttribute( force_tips, 3 ) );
+            } );
+    
+            gui.add( param, 'displacements' ).onChange( function ( val ) {
+                displacement_lines.visible = val;
+                displacement_points.visible = val;
+            } );
+    
+            gui.add( param, 'view_range', 10, 300, 1 ).onChange( function ( val ) {
+                scene.fog.far = val;
+            } );
+        }
+    
+    </script>
+    """
+    source = source.replace("'", "\"")
+
+    def wrap(array):
+        if array.dtype == "float32":
+            data_type = "Float32Array"
+        elif array.dtype == "float64":
+            data_type = "Float64Array"
+        elif array.dtype == "int8":
+            data_type = "Int8Array"
+        elif array.dtype == "uint8":
+            data_type = "Uint8Array"
+        elif array.dtype == "int16":
+            data_type = "Int16Array"
+        elif array.dtype == "uint16":
+            data_type = "Uint16Array"
+        elif array.dtype == "int32":
+            data_type = "Int32Array"
+        elif array.dtype == "uint32":
+            data_type = "Uint32Array"
+        elif array.dtype == "int64":
+            data_type = "BigInt64Array"
+        elif array.dtype == "uint64":
+            data_type = "BigUint64Array"
+        else:
+            raise TypeError(array.dtype)
+        return "NewArray("+data_type+", \""+repr(base64.b64encode(array))[2:-1]+"\")"
+
+    here = source % (f1, f2, wrap(R-np.mean(R, axis=0)), wrap(L), wrap(F), wrap(U))
+    from IPython.core.display import HTML, display
+    code = "<h1></h1><iframe srcdoc='{0}' scrolling=no style='border:none; width: 100%; height: 600px'></iframe>".format(here)
+    display(HTML(code))
```

### Comparing `saenopy-0.8.0/saenopy/multigridHelper.py` & `saenopy-0.9.0/saenopy/multigridHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import numpy as np
 import pandas as pd
 import time
+from typing import Union
+from nptyping import NDArray, Shape, Float, Int, Bool
 
 
-def createMesh(count=None, element_width=None, box_width=None, tesselation_mode="6"):
+def createMesh(count: int = None, element_width: float = None, box_width: float = None, tesselation_mode: str = "6") \
+        -> (NDArray[Shape["N_c, 3"], Float], NDArray[Shape["N_t, 4"], Int]):
     if isinstance(box_width, (int, float)):
         box_width = [box_width, box_width, box_width]
 
     if isinstance(element_width, (int, float)):
         element_width = [element_width, element_width, element_width]
 
     if isinstance(count, (int, float)):
@@ -595,24 +598,26 @@
     sum_region = (M.R[right, 1] < np.max(M.R[right, 1])) & \
                  (M.R[right, 2] < np.max(M.R[right, 2]))
 
     stress = -np.sum(M.f[right, 0][sum_region], axis=0) / A
     print("strain", lambd, "stress", stress, "duration", time.time() - t)
     return stress
 
-def getBorder(R, width=0.5e-6):
+
+def getBorder(R: NDArray[Shape["N_c, 3"], Float], width=0.5e-6) \
+               -> NDArray[Shape["N_c"], Bool]:
     minR = np.min(R, axis=0)
     maxR = np.max(R, axis=0)
 
     border = (R[:, 0] < minR[0] + width) | (R[:, 0] > maxR[0] - width) | \
              (R[:, 1] < minR[1] + width) | (R[:, 1] > maxR[1] - width) | \
              (R[:, 2] < minR[2] + width) | (R[:, 2] > maxR[2] - width)
     return border
 
-def getBoxMeshSurface(T):
+def getBoxMeshSurface(T: NDArray[Shape["N_t, 4"], Int]) -> NDArray[Shape["N_surface"], Int]:
     node_uses = pd.Series(T.ravel()).value_counts().sort_index()
     surface = node_uses != 20
     return surface
 
 
 def plotMesh(R, T, ax=None):
     if ax is None:
@@ -639,16 +644,18 @@
     max_width = np.max(width)
     center = (maxR-minR)/2+minR
 
     ax.set_xlim(center[0]-max_width/2, center[0]+max_width/2)
     ax.set_ylim(center[1]-max_width/2, center[1]+max_width/2)
     ax.set_zlim(center[2]-max_width/2, center[2]+max_width/2)
 
-def removeNodes(R, T, remove_indices):
+
+def removeNodes(R: NDArray[Shape["N_c, 3"], Float], T: NDArray[Shape["N_t, 4"], Int], remove_indices) \
+        -> (NDArray[Shape["N_c, 3"], Float], NDArray[Shape["N_t, 4"], Int]):
     """ removes the nodes with the provided indices from the mesh """
     R2 = R[~remove_indices].copy()
     indices_keep = np.arange(0, len(R))[~remove_indices]
     new_indices = np.zeros(len(R))*np.nan
     new_indices[indices_keep] = np.arange(0, len(R2))
     T2 = new_indices[T]
-    T2 = T2[~np.isnan(np.sum(T2,axis=1))].astype(np.int)
+    T2 = T2[~np.isnan(np.sum(T2,axis=1))].astype(int)
     return R2, T2
```

### Comparing `saenopy-0.8.0/saenopy/numbaOverload.py` & `saenopy-0.9.0/saenopy/numbaOverload.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/save.py` & `saenopy-0.9.0/saenopy/unused/save.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-import base64
-import numpy as np
-import os
-
-
-def ensure_file_extension(filename, ext):
-    basename, file_ext = os.path.splitext(filename)
-    if file_ext != ext:
-        return filename + ext
-    return filename
-
-
-def save_vtp(filename, M):
-    """
-    Export a mesh to the .vtp file format which can be opened in ParaView.
-
-    Parameters
-    ----------
-    filename : str
-        The file where to store the mesh.
-    mesh : :py:class:`~.FiniteBodyForces.FiniteBodyForces`
-        The mesh to save.
-    """
-    xml = """<?xml version="1.0"?>
-<VTKFile type="PolyData" version="0.1" byte_order="LittleEndian" header_type="UInt64">
-<PolyData>
-    <Piece NumberOfPoints="%d" NumberOfVerts="0" NumberOfLines="%d" NumberOfStrips="0" NumberOfPolys="0">
-        <CellData></CellData>
-        <Points>
-            <DataArray Name="Points" NumberOfComponents="3" type="Float32" format="binary">
-            %s
-            </DataArray>
-        </Points>
-        <Verts>
-        </Verts>
-        <Lines>
-            <DataArray type="UInt32" Name="connectivity" format="binary">
-             %s
-            </DataArray>
-            <DataArray type="UInt32" Name="offsets" format="binary">
-             %s
-            </DataArray>
-        </Lines>
-        <Strips></Strips>
-        <Polys></Polys>
-        <PointData>
-            <DataArray Name="Displacement" NumberOfComponents="3" type="Float32" format="binary">
-                %s
-            </DataArray>
-            <DataArray Name="Force" NumberOfComponents="3" type="Float32" format="binary">
-                %s
-            </DataArray>
-        </PointData>
-    </Piece>
-</PolyData>
-</VTKFile>
-"""
-    line_pairs = set()
-    for tet in M.T:
-        for i in range(4):
-            for j in range(4):
-                t1, t2 = tet[i], tet[j]
-                if t1 >= t2:
-                    continue
-                line_pairs.add((t1, t2))
-
-    line_pairs = np.array(list(line_pairs)).ravel()
-    n_lines = len(line_pairs) // 2
-
-    def to_ascii(a):
-        return " ".join(str(i) for i in a.ravel())
-
-    def to_binary(a):
-        byts = base64.b64encode(np.array(a.nbytes, np.uint64).tobytes() + a.tobytes())
-        return repr(byts)[2:-1]
-
-    xml = xml % (
-    M.R.shape[0], n_lines, to_binary(M.R.astype("float32")), to_binary(line_pairs.astype("uint32")), to_binary((np.arange(n_lines) * 2 + 2).astype("uint32")), to_binary(M.U.astype("float32")),
-    to_binary(M.f.astype("float32")))
-    with open(ensure_file_extension(filename, ".vtp"), "w") as fp:
-        fp.write(xml)
-
-def save_vtu(filename, M):
-    xml="""<?xml version="1.0"?>
-<VTKFile type="UnstructuredGrid" version="0.1" byte_order="LittleEndian" header_type="UInt64">
-    <UnstructuredGrid>
-        <Piece NumberOfPoints="%d" NumberOfCells="%s">
-            <Points>
-                <DataArray Name="Points" NumberOfComponents="3" type="Float32" format="binary">
-                %s
-                </DataArray>
-            </Points>
-            
-            <PointData>
-                <DataArray Name="Displacement" NumberOfComponents="3" type="Float32" format="binary">
-                    %s
-                </DataArray>
-                <DataArray Name="Force" NumberOfComponents="3" type="Float32" format="binary">
-                    %s
-                </DataArray>
-            </PointData>
-            
-            <Cells>
-                <DataArray type="UInt32" Name="connectivity" format="binary">
-                    %s
-                </DataArray>
-                <DataArray type="UInt32" Name="offsets" format="binary">
-                    %s
-                </DataArray>
-                <DataArray type="UInt8" Name="types" format="binary">
-                    %s
-                </DataArray>
-            </Cells>
-        </Piece>
-  </UnstructuredGrid>
-</VTKFile>
-"""
-    def to_ascii(a):
-        return " ".join(str(i) for i in a.ravel())
-
-    def to_binary(a):
-        byts = base64.b64encode(np.array(a.nbytes, np.uint64).tobytes() + a.tobytes())
-        return repr(byts)[2:-1]
-
-    T = M.T
-    n_tets = M.T.shape[0]
-
-    xml = xml % (
-        M.R.shape[0], M.T.shape[0], to_binary(M.R.astype("float32")),
-        to_binary(M.U.astype("float32")),
-        to_binary(M.f.astype("float32")),
-        to_binary(T.astype("uint32")),
-        to_binary((np.arange(n_tets) * 4 + 4).astype("uint32")),
-        to_binary((np.ones(n_tets, dtype=np.uint8) * 10).astype("uint8")),
-    )
-    with open(ensure_file_extension(filename, ".vtu"), "w") as fp:
-        fp.write(xml)
-
-def save_gmsh(filename, M):
-    """
-    Export a mesh to the .msh file format which can be opened in GMsh.
-
-    Parameters
-    ----------
-    filename : str
-        The file where to store the mesh.
-    mesh : :py:class:`~.FiniteBodyForces.FiniteBodyForces`
-        The mesh to save.
-    """
-    nodes = M.R
-    num_nodes = nodes.shape[0]
-    tets = M.T+1
-    num_tets = tets.shape[0]
-
-    with open(ensure_file_extension(filename, ".msh"), "w") as fp:
-        fp.write("$MeshFormat\n")
-        fp.write("4.2 0 8\n")
-        fp.write("$EndMeshFormat\n")
-        fp.write("$Nodes\n")
-        fp.write("1 %d 1 %d\n" % (num_nodes, num_nodes))
-        fp.write("3 1 0 %d\n" % num_nodes)
-        for i in range(num_nodes):
-            fp.write(str(i+1)+"\n")
-        for node in nodes:
-            fp.write(" ".join(str(i) for i in node)+"\n")
-        fp.write("$EndNodes\n")
-        fp.write("$Elements\n")
-        fp.write("1 %d 1 %d\n" % (num_tets, num_tets))
-        fp.write("3 1 4 %d\n" % num_tets)
-        for i, tet in enumerate(tets):
-            fp.write(str(i)+" "+" ".join(str(i) for i in tet)+"\n")
-        fp.write("$EndElements\n")
+import base64
+import numpy as np
+import os
+
+
+def ensure_file_extension(filename, ext):
+    basename, file_ext = os.path.splitext(filename)
+    if file_ext != ext:
+        return filename + ext
+    return filename
+
+
+def save_vtp(filename, M):
+    """
+    Export a mesh to the .vtp file format which can be opened in ParaView.
+
+    Parameters
+    ----------
+    filename : str
+        The file where to store the mesh.
+    mesh : :py:class:`~.FiniteBodyForces.FiniteBodyForces`
+        The mesh to save.
+    """
+    xml = """<?xml version="1.0"?>
+<VTKFile type="PolyData" version="0.1" byte_order="LittleEndian" header_type="UInt64">
+<PolyData>
+    <Piece NumberOfPoints="%d" NumberOfVerts="0" NumberOfLines="%d" NumberOfStrips="0" NumberOfPolys="0">
+        <CellData></CellData>
+        <Points>
+            <DataArray Name="Points" NumberOfComponents="3" type="Float32" format="binary">
+            %s
+            </DataArray>
+        </Points>
+        <Verts>
+        </Verts>
+        <Lines>
+            <DataArray type="UInt32" Name="connectivity" format="binary">
+             %s
+            </DataArray>
+            <DataArray type="UInt32" Name="offsets" format="binary">
+             %s
+            </DataArray>
+        </Lines>
+        <Strips></Strips>
+        <Polys></Polys>
+        <PointData>
+            <DataArray Name="Displacement" NumberOfComponents="3" type="Float32" format="binary">
+                %s
+            </DataArray>
+            <DataArray Name="Force" NumberOfComponents="3" type="Float32" format="binary">
+                %s
+            </DataArray>
+        </PointData>
+    </Piece>
+</PolyData>
+</VTKFile>
+"""
+    line_pairs = set()
+    for tet in M.T:
+        for i in range(4):
+            for j in range(4):
+                t1, t2 = tet[i], tet[j]
+                if t1 >= t2:
+                    continue
+                line_pairs.add((t1, t2))
+
+    line_pairs = np.array(list(line_pairs)).ravel()
+    n_lines = len(line_pairs) // 2
+
+    def to_ascii(a):
+        return " ".join(str(i) for i in a.ravel())
+
+    def to_binary(a):
+        byts = base64.b64encode(np.array(a.nbytes, np.uint64).tobytes() + a.tobytes())
+        return repr(byts)[2:-1]
+
+    xml = xml % (
+    M.R.shape[0], n_lines, to_binary(M.R.astype("float32")), to_binary(line_pairs.astype("uint32")), to_binary((np.arange(n_lines) * 2 + 2).astype("uint32")), to_binary(M.U.astype("float32")),
+    to_binary(M.f.astype("float32")))
+    with open(ensure_file_extension(filename, ".vtp"), "w") as fp:
+        fp.write(xml)
+
+def save_vtu(filename, M):
+    xml="""<?xml version="1.0"?>
+<VTKFile type="UnstructuredGrid" version="0.1" byte_order="LittleEndian" header_type="UInt64">
+    <UnstructuredGrid>
+        <Piece NumberOfPoints="%d" NumberOfCells="%s">
+            <Points>
+                <DataArray Name="Points" NumberOfComponents="3" type="Float32" format="binary">
+                %s
+                </DataArray>
+            </Points>
+            
+            <PointData>
+                <DataArray Name="Displacement" NumberOfComponents="3" type="Float32" format="binary">
+                    %s
+                </DataArray>
+                <DataArray Name="Force" NumberOfComponents="3" type="Float32" format="binary">
+                    %s
+                </DataArray>
+            </PointData>
+            
+            <Cells>
+                <DataArray type="UInt32" Name="connectivity" format="binary">
+                    %s
+                </DataArray>
+                <DataArray type="UInt32" Name="offsets" format="binary">
+                    %s
+                </DataArray>
+                <DataArray type="UInt8" Name="types" format="binary">
+                    %s
+                </DataArray>
+            </Cells>
+        </Piece>
+  </UnstructuredGrid>
+</VTKFile>
+"""
+    def to_ascii(a):
+        return " ".join(str(i) for i in a.ravel())
+
+    def to_binary(a):
+        byts = base64.b64encode(np.array(a.nbytes, np.uint64).tobytes() + a.tobytes())
+        return repr(byts)[2:-1]
+
+    T = M.T
+    n_tets = M.T.shape[0]
+
+    xml = xml % (
+        M.R.shape[0], M.T.shape[0], to_binary(M.R.astype("float32")),
+        to_binary(M.U.astype("float32")),
+        to_binary(M.f.astype("float32")),
+        to_binary(T.astype("uint32")),
+        to_binary((np.arange(n_tets) * 4 + 4).astype("uint32")),
+        to_binary((np.ones(n_tets, dtype=np.uint8) * 10).astype("uint8")),
+    )
+    with open(ensure_file_extension(filename, ".vtu"), "w") as fp:
+        fp.write(xml)
+
+def save_gmsh(filename, M):
+    """
+    Export a mesh to the .msh file format which can be opened in GMsh.
+
+    Parameters
+    ----------
+    filename : str
+        The file where to store the mesh.
+    mesh : :py:class:`~.FiniteBodyForces.FiniteBodyForces`
+        The mesh to save.
+    """
+    nodes = M.R
+    num_nodes = nodes.shape[0]
+    tets = M.T+1
+    num_tets = tets.shape[0]
+
+    with open(ensure_file_extension(filename, ".msh"), "w") as fp:
+        fp.write("$MeshFormat\n")
+        fp.write("4.2 0 8\n")
+        fp.write("$EndMeshFormat\n")
+        fp.write("$Nodes\n")
+        fp.write("1 %d 1 %d\n" % (num_nodes, num_nodes))
+        fp.write("3 1 0 %d\n" % num_nodes)
+        for i in range(num_nodes):
+            fp.write(str(i+1)+"\n")
+        for node in nodes:
+            fp.write(" ".join(str(i) for i in node)+"\n")
+        fp.write("$EndNodes\n")
+        fp.write("$Elements\n")
+        fp.write("1 %d 1 %d\n" % (num_tets, num_tets))
+        fp.write("3 1 4 %d\n" % num_tets)
+        for i, tet in enumerate(tets):
+            fp.write(str(i)+" "+" ".join(str(i) for i in tet)+"\n")
+        fp.write("$EndElements\n")
```

### Comparing `saenopy-0.8.0/saenopy/solver.py` & `saenopy-0.9.0/saenopy/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import os
 import sys
 import time
 
 import numpy as np
 import scipy.sparse as ssp
 
-from numba import jit, njit
+from numba import njit
 from typing import Union
+from nptyping import NDArray, Shape, Float, Int, Bool
 
-from saenopy.multigridHelper import getLinesTetrahedra, getLinesTetrahedra2
+from saenopy.multigridHelper import getLinesTetrahedra2
 from saenopy.buildBeams import buildBeams
 from saenopy.materials import Material, SemiAffineFiberMaterial
 from saenopy.conjugateGradient import cg
-from saenopy.loadHelpers import Saveable
+from saenopy.saveable import Saveable
 from typing import List
-from pathlib import Path
-import natsort
-from saenopy.getDeformations import getStack, Stack, format_glob
+
 
 class Mesh(Saveable):
     __save_parameters__ = ['R', 'T', 'node_vars']
-    R = None  # the 3D positions of the vertices, dimension: N_c x 3
-    T = None  # the tetrahedra' 4 corner vertices (defined by index), dimensions: N_T x 4
+    R: NDArray[Shape["N_c, 3"], Float] = None  # the 3D positions of the vertices, dimension: N_c x 3
+    T: NDArray[Shape["N_t, 4"], Int] = None  # the tetrahedra' 4 corner vertices (defined by index), dimensions: N_T x 4
 
-    node_vars = None
+    node_vars: dict = None
 
-    def __init__(self, R=None, T=None, node_vars=None):
+    def __init__(self,
+                 R: NDArray[Shape["N_c, 3"], Float] = None,
+                 T: NDArray[Shape["N_t, 4"], Int] = None,
+                 node_vars: dict = None):
         if R is not None:
             self.setNodes(R)
         if T is not None:
             self.setTetrahedra(T)
         self.node_vars = {}
         if node_vars is not None:
             for name, data in node_vars.items():
                 self.setNodeVar(name, data)
 
-    def setNodes(self, data: np.ndarray):
+    def setNodes(self, data: NDArray[Shape["N_c, 3"], Float]):
         """
         Provide mesh coordinates.
 
         Parameters
         ----------
         data : ndarray
             The coordinates of the vertices. Dimensions Nx3
@@ -48,16 +50,15 @@
         data = np.asarray(data)
         assert len(data.shape) == 2, "Mesh node data needs to be Nx3."
         assert data.shape[1] == 3, "Mesh vertices need to have 3 spacial coordinate."
 
         # store the loaded node coordinates
         self.R = data.astype(np.float64)
 
-
-    def setTetrahedra(self, data: np.ndarray):
+    def setTetrahedra(self, data: NDArray[Shape["N_t, 4"], Int]):
         """
         Provide mesh connectivity. Nodes have to be connected by tetrahedra. Each tetraherdon consts of the indices of
         the 4 vertices which it connects.
 
         Parameters
         ----------
         data : ndarray
@@ -67,65 +68,65 @@
         data = np.asarray(data)
         assert len(data.shape) == 2, "Mesh tetrahedra needs to be Nx4."
         assert data.shape[1] == 4, "Mesh tetrahedra need to have 4 corners."
         assert 0 <= data.min(), "Mesh tetrahedron node indices are not allowed to be negative."
         assert data.max() < self.R.shape[0], "Mesh tetrahedron node indices cannot be bigger than the number of vertices."
 
         # store the tetrahedron data (needs to be int indices)
-        self.T = data.astype(np.int)
+        self.T = data.astype(int)
 
-    def setNodeVar(self, name, data):
+    def setNodeVar(self, name: str, data: Union[NDArray[Shape["N_c"], Float], NDArray[Shape["N_c, 3"], Float]]):
         data = np.asarray(data)
         assert len(data.shape) == 1 or len(data.shape) == 2, "Node var needs to be scalar or vectorial"
         if len(data.shape) == 2:
             assert data.shape[1] == 3, "Vectrial node var needs to have 3 dimensionts"
         assert data.shape[0] == self.R.shape[0], "Node var has to have the same number of nodes than the mesh"
         self.node_vars[name] = data
 
-    def getNodeVar(self, name):
+    def getNodeVar(self, name: str) -> Union[NDArray[Shape["N_c"], Float], NDArray[Shape["N_c, 3"], Float]]:
         return self.node_vars[name]
 
-    def hasNodeVar(self, name):
+    def hasNodeVar(self, name: str):
         return name in self.node_vars
 
 
 class Solver(Saveable):
     __save_parameters__ = ["R", "T", "U", "f", "U_fixed", "U_target", "U_target_mask", "f_target", "E_glo", "var", "regularisation_results",
                       "reg_mask", "regularisation_parameters", "material_model"]
 
-    R = None  # the 3D positions of the vertices, dimension: N_c x 3
-    T = None  # the tetrahedra' 4 corner vertices (defined by index), dimensions: N_T x 4
-    E = None  # the energy stored in each tetrahedron, dimensions: N_T
-    V = None  # the volume of each tetrahedron, dimensions: N_T
-    var = None  # a bool if a node is movable
+    R: NDArray[Shape["N_c, 3"], Float] = None  # the 3D positions of the vertices, dimension: N_c x 3
+    T: NDArray[Shape["N_t, 4"], Int] = None  # the tetrahedra' 4 corner vertices (defined by index), dimensions: N_T x 4
+    E: NDArray[Shape["N_t"], Float] = None  # the energy stored in each tetrahedron, dimensions: N_T
+    V: NDArray[Shape["N_t"], Float] = None  # the volume of each tetrahedron, dimensions: N_T
+    var: NDArray[Shape["N_c"], Bool] = None  # a bool if a node is movable
 
-    Phi = None  # the shape tensor of each tetrahedron, dimensions: N_T x 4 x 3
+    Phi: NDArray[Shape["N_t, 4, 3"], Float] = None  # the shape tensor of each tetrahedron, dimensions: N_T x 4 x 3
     Phi_valid = False
-    U = None  # the displacements of each node, dimensions: N_c x 3
-    U_fixed = None
-    U_target = None
-    U_target_mask = None
-    reg_mask = None
-
-    f = None  # the global forces on each node, dimensions: N_c x 3
-    f_target = None  # the external forces on each node, dimensions: N_c x 3
-    K_glo = None  # the global stiffness tensor, dimensions: N_c x N_c x 3 x 3
+    U: NDArray[Shape["N_c, 3"], Float] = None  # the displacements of each node, dimensions: N_c x 3
+    U_fixed: NDArray[Shape["N_c, 3"], Float] = None
+    U_target: NDArray[Shape["N_c, 3"], Float] = None
+    U_target_mask: NDArray[Shape["N_c"], Bool] = None
+    reg_mask: NDArray[Shape["N_c"], Bool] = None
+
+    f: NDArray[Shape["N_c, 3"], Float] = None  # the global forces on each node, dimensions: N_c x 3
+    f_target: NDArray[Shape["N_c, 3"], Float] = None  # the external forces on each node, dimensions: N_c x 3
+    K_glo: NDArray[Shape["N_c, N_c, 3, 3"], Float] = None  # the global stiffness tensor, dimensions: N_c x N_c x 3 x 3
 
     Laplace = None
 
-    E_glo = 0  # the global energy
+    E_glo: float = 0  # the global energy
 
     # a list of all vertices are connected via a tetrahedron, stored as pairs: dimensions: N_connections x 2
-    connections = None
+    connections: NDArray[Shape["N_con, 2"], Int] = None
     connections_valid = False
 
     N_T = 0  # the number of tetrahedra
     N_c = 0  # the number of vertices
 
-    s = None  # the beams, dimensions N_b x 3
+    s: NDArray[Shape["N_b, 3"], Float] = None  # the beams, dimensions N_b x 3
     N_b = 0  # the number of beams
 
     material_model: SemiAffineFiberMaterial = None  # the function specifying the material model
     material_parameters = None
 
     verbose = False
 
@@ -134,15 +135,15 @@
     preprocessing = [
         "load_stack": ["1_*.tif", "2_*.tif", voxel_sixe],
         "3D_piv": [overlap, windowsize, signoise, drifcorrection],
         "iterpolate_mesh": [],
     ]
     '''
 
-    def setNodes(self, data: np.ndarray):
+    def setNodes(self, data: NDArray[Shape["N_c, 3"], Float]):
         """
         Provide mesh coordinates.
 
         Parameters
         ----------
         data : ndarray
             The coordinates of the vertices. Dimensions Nx3
@@ -161,15 +162,16 @@
         self.N_c = data.shape[0]
 
         self.var = np.ones(self.N_c, dtype=bool)
         self.U = np.zeros((self.N_c, 3))
         self.f = np.zeros((self.N_c, 3))
         self.f_target = np.zeros((self.N_c, 3))
 
-    def setBoundaryCondition(self, displacements: np.ndarray = None, forces: np.ndarray = None):
+    def setBoundaryCondition(self, displacements: NDArray[Shape["N_c, 3"], Float] = None,
+                             forces: NDArray[Shape["N_c, 3"], Float] = None):
         """
         Provide the boundary condition for the mesh, to be used with :py:meth:`~.Solver.solve_nonregularized`.
 
         Parameters
         ----------
         displacements : ndarray, optional
             If the displacement of a node is not nan, it is treated as a Dirichlet boundary condition and the
@@ -193,49 +195,49 @@
         if forces is None:
             self.f_target = np.zeros((self.N_c, 3))
         else:
             self._setExternalForces(forces)
             # if no displacements where given, take the variable nodes from the nans in the force list
             if displacements is None:
                 self.var = ~np.any(np.isnan(forces), axis=1)
-            # if not, check if the the fixed displacements have no force
+            # if not, check if the fixed displacements have no force
             elif np.all(np.isnan(self.f_target[~self.var])) is False:
                 print("WARNING: Forces for fixed vertices were specified. These boundary conditions cannot be"
                       "fulfilled", file=sys.stderr)
 
-    def setInitialDisplacements(self, displacements: np.ndarray):
+    def setInitialDisplacements(self, displacements: NDArray[Shape["N_c, 3"], Float]):
         """
         Provide initial displacements of the nodes. For fixed nodes these displacements are ignored.
 
         Parameters
         ----------
         displacements : ndarray
             The list of displacements. Dimensions Nx3
         """
         # check the input
         displacements = np.asarray(displacements)
         assert displacements.shape == (self.N_c, 3)
         self.U[self.var] = displacements[self.var].astype(np.float64)
 
-    def _setExternalForces(self, forces: np.ndarray):
+    def _setExternalForces(self, forces: NDArray[Shape["N_c, 3"], Float]):
         """
         Provide external forces that act on the vertices. The forces can also be set with
         :py:meth:`~.Solver.setNodes` directly with the vertices.
 
         Parameters
         ----------
         forces : ndarray
             The list of forces. Dimensions Nx3
         """
         # check the input
         forces = np.asarray(forces)
         assert forces.shape == (self.N_c, 3)
         self.f_target = forces.astype(np.float64)
 
-    def setTetrahedra(self, data: np.ndarray):
+    def setTetrahedra(self, data: NDArray[Shape["N_t, 4"], Int]):
         """
         Provide mesh connectivity. Nodes have to be connected by tetrahedra. Each tetraherdon consts of the indices of
         the 4 vertices which it connects.
 
         Parameters
         ----------
         data : ndarray
@@ -276,15 +278,15 @@
         material : :py:class:`~.materials.Material`
              The material, must be of a subclass of Material.
         """
         self.material_model = material
         if generate_lookup is True:
             self.material_model_look_up = self.material_model.generate_look_up_table()
 
-    def setBeams(self, beams: Union[int, np.ndarray] = 300):
+    def setBeams(self, beams: Union[int, NDArray[Shape["N_b, 3"], Float]] = 300):
         """
         Sets the beams for the calculation over the whole solid angle.
 
         Parameters
         ----------
         beams : int, ndarray
             Either an integer which defines in how many beams to discretize the whole solid angle or an ndarray providing
@@ -294,15 +296,15 @@
             beams = buildBeams(beams)
         self.s = beams
         self.N_b = beams.shape[0]
 
     def _computeConnections(self):
         # current scipy versions do not have the sputils anymore
         try:
-            from scipy.sparse import get_index_dtype
+            from scipy.sparse._sputils import get_index_dtype
         except ImportError:
             from scipy.sparse.sputils import get_index_dtype
 
         # calculate the indices for "update_f_glo"
         y, x = np.meshgrid(np.arange(3), self.T.ravel())
         self.force_distribute_coordinates = (x.ravel(), y.ravel())
 
@@ -417,15 +419,15 @@
         # store the stiffness matrix K in self.K_glo
         # transform from N_T x 4 x 4 x 3 x 3 -> N_v * 3 x N_v * 3
         self.K_glo = ssp.coo_matrix((K_glo.ravel()[self.filter_in], self.stiffness_distribute_coordinates2),
                                 shape=(self.N_c*3, self.N_c*3)).tocsr()
         if self.verbose:
             print("updating forces and stiffness matrix finished %.2fs" % (time.time() - t_start))
 
-    def getMaxTetStiffness(self):
+    def getMaxTetStiffness(self) -> NDArray[Shape["N_t"], Float]:
         """
         Calculates the stiffness matrix K_ij, the force F_i and the energy E of each node.
         """
         t_start = time.time()
         batchsize = 10000
 
         tetrahedra_stiffness = np.zeros(self.T.shape[0])
@@ -441,15 +443,15 @@
 
             epsbarbar_b = self.material_model.stiffness(s - 1)
 
             tetrahedra_stiffness[t] = np.max(epsbarbar_b, axis=1)
 
         return tetrahedra_stiffness
 
-    def _get_s_bar(self, t: np.ndarray):
+    def _get_s_bar(self, t: slice) -> NDArray[Shape["N_t, 3, N_b"], Float]:
         # get the displacements of all corners of the tetrahedron (N_Tx3x4)
         # u_tim  (t in [0, N_T], i in {x,y,z}, m in {1,2,3,4})
         # F is the linear map from T (the undeformed tetrahedron) to T' (the deformed tetrahedron)
         # F_tij = d_ij + u_tmi * Phi_tmj  (t in [0, N_T], i,j in {x,y,z}, m in {1,2,3,4})
         F = np.eye(3) + np.einsum("tmi,tmj->tij", self.U[self.T[t]], self.Phi[t])
 
         # multiply the F tensor with the beam
@@ -533,24 +535,26 @@
         if self.Phi_valid is False:
             self._computePhi()
 
         # if the connections are not valid, calculate them
         if self.connections_valid is False:
             self._computeConnections()
 
-    def solve_boundarycondition(self, stepper: float = 0.066, i_max: int = 300, rel_conv_crit: float = 0.01, relrecname: str = None, verbose: bool = False, callback: callable = None):
+    def solve_boundarycondition(self, stepper: float = 0.066, i_max: int = 300, i_min: int = 12, rel_conv_crit: float = 0.01, relrecname: str = None, verbose: bool = False, callback: callable = None):
         """
         Solve the displacement of the free nodes constraint to the boundary conditions.
 
         Parameters
         ----------
         stepper : float, optional
             How much of the displacement of each conjugate gradient step to apply. Default 0.066
         i_max : int, optional
             The maximal number of iterations for the relaxation. Default 300
+        i_min : int, optional
+            The minimal number of iterations for the relaxation. Minimum value is 6. Default is 12
         rel_conv_crit : float, optional
             If the relative standard deviation of the last 6 energy values is below this threshold, finish the iteration.
             Default 0.01
         relrecname : string, optional
             If a filename is provided, for every iteration the displacement of the conjugate gradient step, the global
             energy and the residuum are stored in this file.
         verbose : bool, optional
@@ -591,17 +595,17 @@
 
             # log and store values (if a target file was provided)
             relrec.append([du, self.E_glo, ff])
             if relrecname is not None:
                 np.savetxt(relrecname, relrec)
             if callback is not None:
                 callback(self, relrec)
-
-            # if we have passed 6 iterations calculate average and std
-            if i > 6:
+                
+            # if we have passed i_min iterations we calculate average and std of the last 6 iteration
+            if i > i_min:
                 # calculate the average energy over the last 6 iterations
                 last_Es = np.array(relrec)[:-6:-1, 1]
                 Emean = np.mean(last_Es)
                 Estd = np.std(last_Es)
 
                 # if the iterations converge, stop the iteration
                 # coefficient of variation below "rel_conv_crit"
@@ -636,15 +640,15 @@
         du = np.sum(uu[self.var] ** 2) * stepper * stepper
 
         # return the total applied displacement
         return du
 
     """ regularization """
 
-    def setTargetDisplacements(self, displacement: np.ndarray, reg_mask: np.ndarray=None):
+    def setTargetDisplacements(self, displacement: NDArray[Shape["N_c, 3"], Float], reg_mask: NDArray[Shape["N_c"], Bool] = None):
         """
         Provide the displacements that should be fitted by the regularization.
 
         Parameters
         ----------
         displacement : ndarray
             If the displacement of a node is not nan, it is
@@ -745,29 +749,31 @@
             print("L = |u-uf|^2 + lambda*|w*f|^2 = ", L)
 
         relrec.append((L, uuf2, ff))
 
         if relrecname is not None:
             np.savetxt(relrecname, relrec)
 
-    def solve_regularized(self, stepper: float =0.33, solver_precision: float =1e-18, i_max: int = 100,
-                          rel_conv_crit: float = 0.01, alpha: float = 1e10, method: str = "huber", relrecname: str = None,
-                          verbose: bool = False, callback: callable = None):
+    def solve_regularized(self, stepper: float = 0.33, solver_precision: float = 1e-18, i_max: int = 300,
+                          i_min: int = 12, rel_conv_crit: float = 0.01, alpha: float = 1e10, method: str = "huber",
+                          relrecname: str = None, verbose: bool = False, callback: callable = None):
         """
         Fit the provided displacements. Displacements can be provided with
         :py:meth:`~.Solver.setTargetDisplacements`.
 
         Parameters
         ----------
         stepper : float, optional
              How much of the displacement of each conjugate gradient step to apply. Default 0.33
         solver_precision : float, optional
             The tolerance for the conjugate gradient step. Will be multiplied by the number of nodes. Default 1e-18.
         i_max : int, optional
-            The maximal number of iterations for the regularisation. Default 100
+            The maximal number of iterations for the regularisation. Default 300
+        i_min : int, optional
+            The minimal number of iterations for the relaxation. Minimum value is 6. Default is 12.
         rel_conv_crit :  float, optional
             If the relative standard deviation of the last 6 energy values is below this threshold, finish the iteration.
             Default 0.01
         alpha :  float, optional
             The regularisation parameter. How much to weight the suppression of forces against the fitting of the measured
             displacement. Default 3e9
         method :  string, optional
@@ -810,15 +816,15 @@
             print("going to update glo f and K")
         self._updateGloFAndK()
 
         # log and store values (if a target file was provided)
         relrec = []
         self.relrec = relrec
         if callback is not None:
-            callback(self, relrec)
+            callback(self, relrec, 0, i_max)
         self._recordRegularizationStatus(relrec, alpha, relrecname)
 
         if self.verbose:
             print("check before relax !")
         # start the iteration
         for i in range(i_max):
             # compute the weight matrix
@@ -837,31 +843,31 @@
             if self.verbose:
                 print("Round", i+1, " |du|=", uu)
 
             # log and store values (if a target file was provided)
             self._recordRegularizationStatus(relrec, alpha, relrecname)
 
             if callback is not None:
-                callback(self, relrec)
+                callback(self, relrec, i, i_max)
 
-            # if we have passed 6 iterations calculate average and std
-            if i > 6:
+            # if we have passed i_min iterations we calculate average and std of the last 6 iteration
+            if i > i_min:
                 # calculate the average energy over the last 6 iterations
                 last_Ls = np.array(relrec)[:-6:-1, 1]
                 Lmean = np.mean(last_Ls)
-                Lstd = np.std(last_Ls) / np.sqrt(5)  # the original formula just had /N instead of /sqrt(N)
+                Lstd = np.std(last_Ls)       #  Use Coefficient of Variation; in saeno there was the additional factor  "/ np.sqrt(5)" behind 
 
                 # if the iterations converge, stop the iteration
                 if Lstd / Lmean < rel_conv_crit:
                     break
 
         self.regularisation_results = relrec
         return relrec
 
-    def _solve_regularization_CG(self, stepper: float =0.33, solver_precision: float = 1e-18):
+    def _solve_regularization_CG(self, stepper: float = 0.33, solver_precision: float = 1e-18):
         """
         Solve the displacements from the current stiffness tensor using conjugate gradient.
         """
 
         # solve the conjugate gradient which solves the equation A x = b for x
         # where A is (I - KAK) (K: stiffness matrix, A: weight matrix) and b is (u_meas - u - KAf)
         uu = cg(self.A, self.b.flatten(), maxiter=25*int(pow(self.N_c, 0.33333)+0.5), tol=self.N_c * solver_precision).reshape((self.N_c, 3))
@@ -1007,15 +1013,15 @@
 
     #     results["E_GLO"] = self.E_glo
 
     #     results["POLARITY"] = fmax / contractility
 
     #     return results
 
-    def getPolarity(self):
+    def getPolarity(self) -> float:
 
         inner = self.reg_mask
         f = self.f[inner]
         R = self.R[inner]
 
         fsum = np.sum(f, axis=0)
 
@@ -1209,21 +1215,21 @@
         tri.set_alpha(alpha)
         tri.set_edgecolor(edge_color)
         axes.add_collection3d(tri)
         axes.plot(points[:, 0], points[:, 1], points[:, 2], 'ko')
         axes.set_aspect('equal')
 
     def viewMesh(self, f1: float, f2: float):
-        from .meshViewer import MeshViewer
+        from saenopy.unused.meshViewer import MeshViewer
 
         L = getLinesTetrahedra2(self.T)
 
         return MeshViewer(self.R, L, self.f, self.U, f1, f2)
 
-    def getCenter(self, mode="force", border=None):
+    def getCenter(self, mode="force", border=None) -> NDArray[Shape["3"], Float]:
         f = self.f
         R = self.R
         U = self.U
 
         if self.reg_mask is not None:
             f = self.f * self.reg_mask[:, None]
 
@@ -1280,15 +1286,15 @@
         RR = R - Rcms
         RRnorm = RR/ np.linalg.norm(RR, axis=1)[:,None]
         fnorm = f / np.linalg.norm(f, axis=1)[:,None]
         f2 = np.sum(RRnorm * fnorm, axis=1)[:,None] * f
         f3 = np.cross(RRnorm, f)
         return f2, f3
 
-    def force_ratio_outer_to_inner(self, width_outer = 5e-6):
+    def force_ratio_outer_to_inner(self, width_outer=5e-6):
         """
         Divides the Cubus in an outer and inner part, where the outer part
         is defined as everything closer than width_outer (default ist 14 um)
         to the edge of the stack.
 
         Then computes the ratio of the mean forces in the outer part divided by
         the mean forces within the inner part.
@@ -1336,15 +1342,15 @@
             sumz = np.nansum(np.abs(self.U_target[:,2]))
             # calculate the fraction of the z-component
             ratioz = sumz / (sumx+sumy+sumz)
         except:
             ratioz = np.nan
         return ratioz
 
-    def getContractility(self, center_mode="force", r_max=None):
+    def getContractility(self, center_mode="force", r_max=None) -> str:
         f = self.f
         R = self.R
 
         if self.reg_mask is not None:
             f = self.f * self.reg_mask[:, None]
 
         # get center of force field
@@ -1360,20 +1366,21 @@
         #mag = np.linalg.norm(f, axis=1)
 
         RRnorm = RR / np.linalg.norm(RR, axis=1)[:, None]
         contractility = np.nansum(np.einsum("ki,ki->k", RRnorm, f))
         return contractility
 
 
-    def getContractilityIgnoreBorder(self, width_outer = 5e-6, center_mode="force" ):
+    def getContractilityIgnoreBorder(self, width_outer=5e-6, center_mode="force") -> float:
         """
-        Computes the contractilty value while ignoring all force vectors that
+        Computes the contractility value while ignoring all force vectors that
         are located within at the borders (outer shell with width_outer).
         For Drift/Rotation we often find high forces here.
         """
+        f_org = self.f.copy()
         f = self.f
         R = self.R
         # exclude counter forces
         if self.reg_mask is not None:
             f = self.f * self.reg_mask[:, None]
         # mask the data points in the outer layer (closer to the outer border than
         # width_outer and for the inner shell the remaining inner volume
@@ -1384,28 +1391,31 @@
         f[outer_layer] = np.nan
         # get center of complete force field and set as origin
         Rcms_all = self.getCenter(mode=center_mode)
         RR = R - Rcms_all
 
         RRnorm = RR / np.linalg.norm(RR, axis=1)[:, None]
         contractility = np.nansum(np.einsum("ki,ki->k", RRnorm, f))
+        
+        # go back to original forcefield
+        self.f = f_org        
 
         return contractility
 
     def getContractilityUnbiasedEpicenter(self,  r_max=None):
         """
-        Computes a contractilty value, that uses an unbiased center approach.
-        Instsead of computing the center from all force vectors, which will bias the
-        the location (as a result of optimization), here we split the image stack into +x,-x halfspaces
-        +y,-y halfspaces and +z,-z halfspaces around the intitially found center.
-        Then we compute the center of the force vectors within this halfsphere and
-        compute the contractility of the force components in the opposing halfspacce
-        onto this center (e.g. -x halfspace values uses the center from +x halfsphere).
+        Computes a contractility value, that uses an unbiased center approach.
+        Instead of computing the center from all force vectors, which will bias
+        the location (as a result of optimization), here we split the image stack into +x,-x half-spaces
+        +y,-y half-spaces and +z,-z half-spaces around the initially found center.
+        Then we compute the center of the force vectors within this half-sphere and
+        compute the contractility of the force components in the opposing half-space
+        onto this center (e.g. -x halfspace values uses the center from +x half-sphere).
         We then add up the derived contractility values from -x and +x components (same for -+y and -+z)
-        and  compute the final unbiased contractilty as mean value of all 3 dimension.
+        and  compute the final unbiased contractility as mean value of all 3 dimension.
 
         returns the unbiased contractility value
         """
 
         ### first get the initial center of the whole force field withe
         ## the biased Center method
         f = self.f
@@ -1756,196 +1766,72 @@
 
         plotter.link_views()
         if camera_position is not None:
             plotter.camera_position = camera_position
         campos = plotter.show(screenshot=export)
         return plotter, campos
 
-
-class Result(Saveable):
-    __save_parameters__ = ['stack', 'time_delta', 'piv_parameter', 'mesh_piv',
-                           'interpolate_parameter', 'solve_parameter', 'solver',
-                           '___save_name__', '___save_version__']
-    ___save_name__ = "Result"
-    ___save_version__ = "1.0"
-    output: str = None
-    state: False
-
-    stack: List[Stack] = None
-
-    piv_parameter: dict = None
-    mesh_piv: List[Mesh] = None
-
-    interpolate_parameter: dict = None
-    solve_parameter: dict = None
-    solver: List[Solver] = None
-
-    def __init__(self, output=None, stack=None, time_delta=None, **kwargs):
-        self.output = str(output)
-
-        self.stack = stack
-        if stack == None:
-            self.stack = []
-
-        self.state = False
-        self.time_delta = time_delta
-
-        self.mesh_piv = [None] * (len(self.stack) - 1)
-        self.solver = [None] * (len(self.mesh_piv))
-
-        super().__init__(**kwargs)
-
-    def save(self):
-        Path(self.output).parent.mkdir(exist_ok=True, parents=True)
-        super().save(self.output)
-
-    def on_load(self, filename):
-        self.output = str(Path(filename))
-
-    def __repr__(self):
-        def filename_to_string(filename):
-            if isinstance(filename, list):
-                return str(Path(common_start(filename) + "{z}" + common_end(filename)))
-            return str(Path(filename))
-        folders = [filename_to_string(stack.filename) for stack in self.stack]
-        base_folder = common_start(folders)
-        base_folder = os.sep.join(base_folder.split(os.sep)[:-1])
-        indent = "    "
-        text = "Result(" + "\n"
-        text += indent + "output = " + self.output + "\n"
-        text += indent + "stacks = [" + "\n"
-        text += indent + indent + "base_folder = " + base_folder + "\n"
-        for stack, filename in zip(self.stack, folders):
-            text += indent + indent + filename[len(base_folder):] + " " + str(stack.voxel_size) + "\n"
-        text += indent + "]" + "\n"
-        if self.piv_parameter:
-            text += indent + "piv_parameter = " + str(self.piv_parameter) + "\n"
-        if self.interpolate_parameter:
-            text += indent + "interpolate_parameter = " + str(self.interpolate_parameter) + "\n"
-        if self.solve_parameter:
-            text += indent + "solve_parameter = " + str(self.solve_parameter) + "\n"
-        text += ")" + "\n"
-        return text
-
-
+# needs to stay here instead of top to prevent circular import
+from saenopy.result_file import Result
 
 def save(filename: str, M: Solver):
     M.save(filename)
 
 
-def load(filename: str) -> Solver:
+def load_solver(filename: str) -> Solver:
     return Solver.load(filename)
 
 
+def load(filename: str) -> Result:
+    return Result.load(filename)
 
-from pathlib import Path
-import os
-def get_stacks(filename, output_path, voxel_size, time_delta=None, exist_overwrite_callback=None):
-    results = []
-    if isinstance(filename, (list, tuple)):
-        results1, output_base = format_glob(filename[0])
-        results2, _ = format_glob(filename[1])
-
-        for (r1, d1), (r2, d2) in zip(results1.groupby("template").max().iterrows(),
-                                      results2.groupby("template").max().iterrows()):
-            output = Path(output_path) / os.path.relpath(r1, output_base)
-            output = output.parent / output.stem
-            output = Path(str(output).replace("*", "") + ".npz")
-
-            r1 = r1.format(z="*")
-            r2 = r2.format(z="*")
-
-            if output.exists() and exist_overwrite_callback is not None:
-                mode = exist_overwrite_callback(output)
-                if mode == 0:
-                    break
-                if mode == "read":
-                    print('exists', output)
-                    data = Result.load(output)
-                    results.append(data)
-                    continue
-
-            data = Result(
-                output=output,
-                stack=[Stack(r1, voxel_size), Stack(r2, voxel_size)],
-            )
-            data.save()
-            results.append(data)
-    else:
-        results1, output_base = format_glob(filename)
-        if time_delta is None:
-            raise ValueError("A time series needs a time_delta, None was given.")
-
-        for template, d in results1.groupby("template"):
-            output = Path(output_path) / os.path.relpath(d.iloc[0].template, output_base)
-            output = output.parent / output.stem
-            output = Path(str(output).replace("*", "") + ".npz")
-
-            if output.exists() and exist_overwrite_callback is not None:
-                mode = exist_overwrite_callback(output)
-                if mode == 0:
-                    break
-                if mode == "read":
-                    print('exists', output)
-                    data = Result.load(output)
-                    results.append(data)
-                    continue
-
-            stacks = []
-            for t, d0 in d.groupby("t"):
-                d0 = d0.sort_values(by='z', key=natsort.natsort_keygen())
-                stacks.append(Stack(d0.filename, voxel_size))
-
-            data = Result(
-                output=output,
-                stack=stacks,
-                time_delta=time_delta,
-            )
-            data.save()
-            results.append(data)
-    return results
-
-def common_start(values):
-    if len(values) != 0:
-        start = values[0]
-        while start:
-            if all(value.startswith(start) for value in values):
-                return start
-            start = start[:-1]
-    return ""
-
-def common_end(values):
-    if len(values) != 0:
-        end = values[0]
-        while end:
-            if all(value.endswith(end) for value in values):
-                return end
-            end = end[1:]
-    return ""
+
+def load_results(filename: str) -> List[Result]:
+    import glob
+    return [Result.load(file) for file in glob.glob(filename, recursive=True)]
 
 
-def substract_reference_state(mesh_piv, mode):
+def subtract_reference_state(mesh_piv, mode):
     U = [M.getNodeVar("U_measured") for M in mesh_piv]
     # correct for the median position
     if len(U) > 2:
         xpos2 = np.cumsum(U, axis=0)  # mittlere position
         if mode == "first":
             xpos2 -= xpos2[0]
         elif mode == "median":
             xpos2 -= np.nanmedian(xpos2, axis=0)  # aktuelle abweichung von
         elif mode == "last":
             xpos2 -= xpos2[-1]
+        elif mode == "next":
+            xpos2 = U
     else:
         xpos2 = U
     return xpos2
 
 
-def interpolate_mesh(M, xpos2, params):
+def interpolate_mesh(M: Solver, xpos2: np.ndarray, params: dict) -> Solver:
     import saenopy
     from saenopy.multigridHelper import getScaledMesh, getNodesWithOneFace
+    
+    if params["mesh_size_same"]:
+        x, y, z = (M.R.max(axis=0) - M.R.min(axis=0))*1e6
+        params["mesh_size_x"] = x
+        params["mesh_size_y"] = y
+        params["mesh_size_z"] = z
+    if params["mesh_size_x"] < params["element_size"]*2 or \
+       params["mesh_size_y"] < params["element_size"]*2 or \
+       params["mesh_size_z"] < params["element_size"]*2:
+        raise ValueError("Mesh size needs to be at least twice the element size.")
+
+    # no thinning if no values are set
+    if "inner_region" not in params:
+        params["inner_region"] = x
+    if "thinning_factor" not in params:    
+        params["thinning_factor"] = 0
+    
     points, cells = saenopy.multigridHelper.getScaledMesh(params["element_size"] * 1e-6,
                                                           params["inner_region"] * 1e-6,
                                                           np.array([params["mesh_size_x"], params["mesh_size_y"],
                                                                     params["mesh_size_z"]]) * 1e-6 / 2,
                                                           [0, 0, 0], params["thinning_factor"])
 
     R = (M.R - np.min(M.R, axis=0)) - (np.max(M.R, axis=0) - np.min(M.R, axis=0)) / 2
```

### Comparing `saenopy-0.8.0/saenopy/stack3DHelper.py` & `saenopy-0.9.0/saenopy/unused/stack3DHelper.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.8.0/saenopy/tfjit.py` & `saenopy-0.9.0/saenopy/unused/tfjit.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-import dis
-import inspect
-import numpy as np
-import tensorflow as tf
-import time
-import tqdm
-
-import types
-
-def rename_code_object(func, new_name):
-    code = func.__code__
-    return types.FunctionType(
-        types.CodeType(
-            code.co_argcount, code.co_nlocals,
-            code.co_stacksize, code.co_flags,
-            code.co_code, code.co_consts,
-            code.co_names, code.co_varnames,
-            code.co_filename, new_name,
-            code.co_firstlineno, code.co_lnotab,
-            code.co_freevars, code.co_cellvars),
-        func.__globals__, new_name, func.__defaults__, func.__closure__)
-
-class TensorFlowTheanoFunction(object):
-    def __init__(self, inputs, outputs, name=None):
-        self._inputs = inputs
-        self._outputs = outputs
-
-    def __call__(self, *args, **kwargs):
-        feeds = {}
-        for (argpos, arg) in enumerate(args):
-            feeds[self._inputs[argpos]] = arg
-        return tf.get_default_session().run(self._outputs, feeds)
-
-class ProperlyWrapFunc(TensorFlowTheanoFunction):
-
-    def __init__(self, inputs, outputs, name):
-        super(ProperlyWrapFunc, self).__init__(inputs, outputs)
-        renamed = rename_code_object(super(ProperlyWrapFunc, self).__call__, name)
-        self.__class__ = type(name, (ProperlyWrapFunc,), {'__call__': renamed})
-
-sess = tf.InteractiveSession()
-
-def x(a, b):
-    for i in range(10):
-        c = b+10
-    return np.dot(a+5, c)
-
-#for ins in dis.get_instructions(x.__code__):
-#    print(ins)
-#exit()
-def translateFunction(func, tf_args, np_args, tf_kwargs):
-    target_func = None
-    if func == int:
-        target_func = int
-    if func == np.einsum:
-        target_func = tf.einsum
-    if func == np.eye:
-        target_func = tf.eye
-        tf_kwargs["dtype"] = tf.float64
-    if func == np.floor:
-        target_func = tf.floor
-    if getattr(func, "tf_jit", False) is True:
-        #if getattr(func, "tensor_run", None) is not None:
-        return getattr(func, "build_graph")(tf_args, np_args)
-    if target_func is None:
-        return func(*tf_args, **tf_kwargs)
-        raise ValueError("Cannot compile func", func)
-    return target_func(*tf_args, **tf_kwargs)
-
-def print_me(target):
-    try:
-        return "("+str(target.shape)+")"
-    except:
-        return str(target)
-
-def tfjit():
-    def processFunc(__func_to_compile__):
-        signature = inspect.signature(__func_to_compile__)
-        parameter_names = [str(param) for param in signature.parameters]
-        self = []
-        def compile_func(*args, **kwargs):
-            if compile_func.tensor_run is not None:
-                print("*args", len(args), [print_me(a) for a in args])
-                try:
-                    return compile_func.tensor_run(*args, **kwargs)
-                except ValueError:
-                    pass
-            tensor_inputs = []
-            numpy_inputs = []
-            for name, value in zip(parameter_names, args):
-                numpy_inputs.append(value)
-                if isinstance(value, np.ndarray):
-                    value = tf.placeholder(dtype=tf.float64, shape=value.shape, name=name)
-                    tensor_inputs.append(value)
-                locals()[name] = value
-
-            def build_graph(tensor_inputs, numpy_inputs):
-                tensor_locals = {name: value for name, value in zip(parameter_names, tensor_inputs)}
-                numpy_locals = {name: value for name, value in zip(parameter_names, numpy_inputs)}
-                stack_tf = []
-                stack_np = []
-
-                print("Compile", compile_func.numpy_run.__name__)
-                for ins in tqdm.tqdm(dis.get_instructions(compile_func.numpy_run.__code__)):
-                    if len(stack_tf):
-                        print(stack_tf[-1])
-                    print(ins)
-                    if ins.opname == "LOAD_FAST":
-                        tensor_var = tensor_locals[ins.argval]
-                        if getattr(tensor_var, "__replace_with__", None) is not None:
-                            tensor_var = getattr(tensor_var, "__replace_with__")
-                        stack_tf.append(tensor_var)
-                        stack_np.append(numpy_locals[ins.argval])
-                        continue
-                    if ins.opname == "STORE_FAST":
-                        tensor_locals[ins.argval] = tf.identity(stack_tf[-1], name=ins.argval)
-                        stack_tf[-1] = tensor_locals[ins.argval]
-                        stack_np[-1] = numpy_locals[ins.argval] = stack_np[-1]
-                        continue
-                    if ins.opname == "CALL_FUNCTION" or ins.opname == "CALL_METHOD":# or ins.opname == "CALL_FUNCTION_EX":
-                        tf_args = []
-                        #if ins.opname == "CALL_FUNCTION_EX":
-                        #    for el in stack_tf.pop():
-                        #        tf_args.append(el)
-                        #    tf_args = tf_args[::-1]
-                        for i in range(ins.arg):
-                            tf_args.append(stack_tf.pop())
-                        tf_f = stack_tf.pop()
-                        if isinstance(tf_f, tuple):
-                            tf_args.extend(tf_f[1:][::-1])
-                            tf_f = tf_f[0]
-
-                        np_args = []
-                        #if ins.opname == "CALL_FUNCTION_EX":
-                        #    for el in np_args.pop():
-                        #        np_args.append(el)
-                        #    np_args = np_args[::-1]
-                        for i in range(ins.arg):
-                            np_args.append(stack_np.pop())
-                        np_f = stack_np.pop()
-
-                        #print("Call function", np_f)
-                        #print("Call function", [print_me(t) for t in np_args[::-1]])
-                        stack_np.append(np_f(*np_args[::-1]))
-                        #print("Call function", tf_args[::-1])
-                        stack_tf.append(translateFunction(tf_f, tf_args[::-1], np_args[::-1], {}))
-                        continue
-                    for stack in [stack_tf, stack_np]:
-                        if ins.opname == "LOAD_GLOBAL":
-                            if ins.argval == "int":
-                                stack.append(int)
-                            else:
-                                stack.append(globals()[ins.argval])
-                            continue
-                        if ins.opname == "LOAD_METHOD":
-                            if isinstance(stack[-1], tf.Tensor) and ins.argval == "astype":
-                                stack[-1] = (tf.cast, stack[-1])
-                            elif isinstance(stack[-1], tf.Tensor) and ins.argval == "flatten":
-                                stack[-1] = (tf.reshape, stack[-1], [-1])
-                            elif isinstance(stack[-1], tf.Tensor) and ins.argval == "reshape":
-                                stack[-1] = (tf.reshape, stack[-1])
-                            else:
-                                stack[-1] = getattr(stack[-1], ins.argval)
-                            continue
-                        if ins.opname == "LOAD_ATTR":
-                            if isinstance(stack[-1], tf.Tensor) and ins.argval == "reshape":
-                                stack[-1] = lambda *args: tf.reshape(stack[-1], *args)
-                            else:
-                                stack[-1] = getattr(stack[-1], ins.argval)
-                            continue
-                        if ins.opname == "LOAD_DEREF":
-                            index = compile_func.numpy_run.__code__.co_freevars.index(ins.argval)
-                            var = compile_func.numpy_run.__closure__[index].cell_contents
-                            if stack == stack_tf and isinstance(var, np.ndarray):
-                                var = tf.Variable(var, name=ins.argval, dtype=var.dtype)
-                                sess.run(var.initializer)
-                            stack.append(var)
-                            continue
-
-                        if ins.opname == "LOAD_CONST":
-                            stack.append(ins.argval)
-                            continue
-                        if ins.opname == "BINARY_ADD":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            stack.append(TOS1 + TOS)
-                            continue
-                        if ins.opname == "BINARY_SUBTRACT":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            stack.append(TOS1 - TOS)
-                            continue
-                        if ins.opname == "BINARY_MULTIPLY":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            stack.append(TOS1 * TOS)
-                            continue
-                        if ins.opname == "BINARY_TRUE_DIVIDE":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            stack.append(TOS1 / TOS)
-                            continue
-                        if ins.opname == "COMPARE_OP":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            if ins.argval == ">":
-                                stack.append(TOS1 > TOS)
-                                continue
-                        if ins.opname == "STORE_SUBSCR":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            TOS2 = stack.pop()
-                            #print("STORE_SUBSCR", TOS1, TOS, TOS2)
-                            if TOS.dtype == "bool" and isinstance(TOS, tf.Tensor):
-                                w = tf.where(TOS, tf.ones_like(TOS1) * TOS2, TOS1)
-                                TOS1.__replace_with__ = w
-                                #TOS1.assign(tf.where(TOS, tf.zeros_like(a)))
-                            else:
-                                TOS1[TOS] = TOS2
-                            #stack.append()
-                            continue
-                        if ins.opname == "BINARY_SUBSCR":
-                            TOS = stack.pop()
-                            TOS1 = stack.pop()
-                            #print("BINARY_SUBSCR", TOS1, TOS)
-                            if isinstance(TOS1, tf.Tensor) or isinstance(TOS, tf.Tensor):
-                                #print("Gather")
-                                stack.append(tf.gather(TOS1, TOS))
-                            else:
-                                #print("No gather", type(TOS1), isinstance(TOS1, tf.Tensor))
-                                stack.append(TOS1[TOS])
-                            continue
-                        if ins.opname == "BUILD_TUPLE":
-                            args = []
-                            for i in range(ins.arg):
-                                args.append(stack.pop())
-                            stack.append(tuple(args[::-1]))
-                            continue
-                        if ins.opname == "RETURN_VALUE":
-                            #print("Return value", stack)
-                            return stack[-1]
-                            break
-                        #print(ins)
-                        raise
-
-            return_value = build_graph(tensor_inputs, numpy_inputs)
-
-            #print("compiling with", tensor_inputs, return_value)
-            __compiled_tensorflow_func__ = TensorFlowTheanoFunction(tensor_inputs, return_value, __func_to_compile__.__name__)
-            compile_func.tensor_run = __compiled_tensorflow_func__
-            compile_func.build_graph = build_graph
-            writer = tf.summary.FileWriter(".", sess.graph)
-            return __compiled_tensorflow_func__(*numpy_inputs)
-
-        compile_func.tensor_run = None
-        compile_func.numpy_run = __func_to_compile__
-        compile_func.tf_jit = True
-        return compile_func
-    return processFunc
+import dis
+import inspect
+import numpy as np
+import tensorflow as tf
+import time
+import tqdm
+
+import types
+
+def rename_code_object(func, new_name):
+    code = func.__code__
+    return types.FunctionType(
+        types.CodeType(
+            code.co_argcount, code.co_nlocals,
+            code.co_stacksize, code.co_flags,
+            code.co_code, code.co_consts,
+            code.co_names, code.co_varnames,
+            code.co_filename, new_name,
+            code.co_firstlineno, code.co_lnotab,
+            code.co_freevars, code.co_cellvars),
+        func.__globals__, new_name, func.__defaults__, func.__closure__)
+
+class TensorFlowTheanoFunction(object):
+    def __init__(self, inputs, outputs, name=None):
+        self._inputs = inputs
+        self._outputs = outputs
+
+    def __call__(self, *args, **kwargs):
+        feeds = {}
+        for (argpos, arg) in enumerate(args):
+            feeds[self._inputs[argpos]] = arg
+        return tf.get_default_session().run(self._outputs, feeds)
+
+class ProperlyWrapFunc(TensorFlowTheanoFunction):
+
+    def __init__(self, inputs, outputs, name):
+        super(ProperlyWrapFunc, self).__init__(inputs, outputs)
+        renamed = rename_code_object(super(ProperlyWrapFunc, self).__call__, name)
+        self.__class__ = type(name, (ProperlyWrapFunc,), {'__call__': renamed})
+
+sess = tf.InteractiveSession()
+
+def x(a, b):
+    for i in range(10):
+        c = b+10
+    return np.dot(a+5, c)
+
+#for ins in dis.get_instructions(x.__code__):
+#    print(ins)
+#exit()
+def translateFunction(func, tf_args, np_args, tf_kwargs):
+    target_func = None
+    if func == int:
+        target_func = int
+    if func == np.einsum:
+        target_func = tf.einsum
+    if func == np.eye:
+        target_func = tf.eye
+        tf_kwargs["dtype"] = tf.float64
+    if func == np.floor:
+        target_func = tf.floor
+    if getattr(func, "tf_jit", False) is True:
+        #if getattr(func, "tensor_run", None) is not None:
+        return getattr(func, "build_graph")(tf_args, np_args)
+    if target_func is None:
+        return func(*tf_args, **tf_kwargs)
+        raise ValueError("Cannot compile func", func)
+    return target_func(*tf_args, **tf_kwargs)
+
+def print_me(target):
+    try:
+        return "("+str(target.shape)+")"
+    except:
+        return str(target)
+
+def tfjit():
+    def processFunc(__func_to_compile__):
+        signature = inspect.signature(__func_to_compile__)
+        parameter_names = [str(param) for param in signature.parameters]
+        self = []
+        def compile_func(*args, **kwargs):
+            if compile_func.tensor_run is not None:
+                print("*args", len(args), [print_me(a) for a in args])
+                try:
+                    return compile_func.tensor_run(*args, **kwargs)
+                except ValueError:
+                    pass
+            tensor_inputs = []
+            numpy_inputs = []
+            for name, value in zip(parameter_names, args):
+                numpy_inputs.append(value)
+                if isinstance(value, np.ndarray):
+                    value = tf.placeholder(dtype=tf.float64, shape=value.shape, name=name)
+                    tensor_inputs.append(value)
+                locals()[name] = value
+
+            def build_graph(tensor_inputs, numpy_inputs):
+                tensor_locals = {name: value for name, value in zip(parameter_names, tensor_inputs)}
+                numpy_locals = {name: value for name, value in zip(parameter_names, numpy_inputs)}
+                stack_tf = []
+                stack_np = []
+
+                print("Compile", compile_func.numpy_run.__name__)
+                for ins in tqdm.tqdm(dis.get_instructions(compile_func.numpy_run.__code__)):
+                    if len(stack_tf):
+                        print(stack_tf[-1])
+                    print(ins)
+                    if ins.opname == "LOAD_FAST":
+                        tensor_var = tensor_locals[ins.argval]
+                        if getattr(tensor_var, "__replace_with__", None) is not None:
+                            tensor_var = getattr(tensor_var, "__replace_with__")
+                        stack_tf.append(tensor_var)
+                        stack_np.append(numpy_locals[ins.argval])
+                        continue
+                    if ins.opname == "STORE_FAST":
+                        tensor_locals[ins.argval] = tf.identity(stack_tf[-1], name=ins.argval)
+                        stack_tf[-1] = tensor_locals[ins.argval]
+                        stack_np[-1] = numpy_locals[ins.argval] = stack_np[-1]
+                        continue
+                    if ins.opname == "CALL_FUNCTION" or ins.opname == "CALL_METHOD":# or ins.opname == "CALL_FUNCTION_EX":
+                        tf_args = []
+                        #if ins.opname == "CALL_FUNCTION_EX":
+                        #    for el in stack_tf.pop():
+                        #        tf_args.append(el)
+                        #    tf_args = tf_args[::-1]
+                        for i in range(ins.arg):
+                            tf_args.append(stack_tf.pop())
+                        tf_f = stack_tf.pop()
+                        if isinstance(tf_f, tuple):
+                            tf_args.extend(tf_f[1:][::-1])
+                            tf_f = tf_f[0]
+
+                        np_args = []
+                        #if ins.opname == "CALL_FUNCTION_EX":
+                        #    for el in np_args.pop():
+                        #        np_args.append(el)
+                        #    np_args = np_args[::-1]
+                        for i in range(ins.arg):
+                            np_args.append(stack_np.pop())
+                        np_f = stack_np.pop()
+
+                        #print("Call function", np_f)
+                        #print("Call function", [print_me(t) for t in np_args[::-1]])
+                        stack_np.append(np_f(*np_args[::-1]))
+                        #print("Call function", tf_args[::-1])
+                        stack_tf.append(translateFunction(tf_f, tf_args[::-1], np_args[::-1], {}))
+                        continue
+                    for stack in [stack_tf, stack_np]:
+                        if ins.opname == "LOAD_GLOBAL":
+                            if ins.argval == "int":
+                                stack.append(int)
+                            else:
+                                stack.append(globals()[ins.argval])
+                            continue
+                        if ins.opname == "LOAD_METHOD":
+                            if isinstance(stack[-1], tf.Tensor) and ins.argval == "astype":
+                                stack[-1] = (tf.cast, stack[-1])
+                            elif isinstance(stack[-1], tf.Tensor) and ins.argval == "flatten":
+                                stack[-1] = (tf.reshape, stack[-1], [-1])
+                            elif isinstance(stack[-1], tf.Tensor) and ins.argval == "reshape":
+                                stack[-1] = (tf.reshape, stack[-1])
+                            else:
+                                stack[-1] = getattr(stack[-1], ins.argval)
+                            continue
+                        if ins.opname == "LOAD_ATTR":
+                            if isinstance(stack[-1], tf.Tensor) and ins.argval == "reshape":
+                                stack[-1] = lambda *args: tf.reshape(stack[-1], *args)
+                            else:
+                                stack[-1] = getattr(stack[-1], ins.argval)
+                            continue
+                        if ins.opname == "LOAD_DEREF":
+                            index = compile_func.numpy_run.__code__.co_freevars.index(ins.argval)
+                            var = compile_func.numpy_run.__closure__[index].cell_contents
+                            if stack == stack_tf and isinstance(var, np.ndarray):
+                                var = tf.Variable(var, name=ins.argval, dtype=var.dtype)
+                                sess.run(var.initializer)
+                            stack.append(var)
+                            continue
+
+                        if ins.opname == "LOAD_CONST":
+                            stack.append(ins.argval)
+                            continue
+                        if ins.opname == "BINARY_ADD":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            stack.append(TOS1 + TOS)
+                            continue
+                        if ins.opname == "BINARY_SUBTRACT":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            stack.append(TOS1 - TOS)
+                            continue
+                        if ins.opname == "BINARY_MULTIPLY":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            stack.append(TOS1 * TOS)
+                            continue
+                        if ins.opname == "BINARY_TRUE_DIVIDE":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            stack.append(TOS1 / TOS)
+                            continue
+                        if ins.opname == "COMPARE_OP":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            if ins.argval == ">":
+                                stack.append(TOS1 > TOS)
+                                continue
+                        if ins.opname == "STORE_SUBSCR":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            TOS2 = stack.pop()
+                            #print("STORE_SUBSCR", TOS1, TOS, TOS2)
+                            if TOS.dtype == "bool" and isinstance(TOS, tf.Tensor):
+                                w = tf.where(TOS, tf.ones_like(TOS1) * TOS2, TOS1)
+                                TOS1.__replace_with__ = w
+                                #TOS1.assign(tf.where(TOS, tf.zeros_like(a)))
+                            else:
+                                TOS1[TOS] = TOS2
+                            #stack.append()
+                            continue
+                        if ins.opname == "BINARY_SUBSCR":
+                            TOS = stack.pop()
+                            TOS1 = stack.pop()
+                            #print("BINARY_SUBSCR", TOS1, TOS)
+                            if isinstance(TOS1, tf.Tensor) or isinstance(TOS, tf.Tensor):
+                                #print("Gather")
+                                stack.append(tf.gather(TOS1, TOS))
+                            else:
+                                #print("No gather", type(TOS1), isinstance(TOS1, tf.Tensor))
+                                stack.append(TOS1[TOS])
+                            continue
+                        if ins.opname == "BUILD_TUPLE":
+                            args = []
+                            for i in range(ins.arg):
+                                args.append(stack.pop())
+                            stack.append(tuple(args[::-1]))
+                            continue
+                        if ins.opname == "RETURN_VALUE":
+                            #print("Return value", stack)
+                            return stack[-1]
+                            break
+                        #print(ins)
+                        raise
+
+            return_value = build_graph(tensor_inputs, numpy_inputs)
+
+            #print("compiling with", tensor_inputs, return_value)
+            __compiled_tensorflow_func__ = TensorFlowTheanoFunction(tensor_inputs, return_value, __func_to_compile__.__name__)
+            compile_func.tensor_run = __compiled_tensorflow_func__
+            compile_func.build_graph = build_graph
+            writer = tf.summary.FileWriter(".", sess.graph)
+            return __compiled_tensorflow_func__(*numpy_inputs)
+
+        compile_func.tensor_run = None
+        compile_func.numpy_run = __func_to_compile__
+        compile_func.tf_jit = True
+        return compile_func
+    return processFunc
```

### Comparing `saenopy-0.8.0/PKG-INFO` & `saenopy-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: saenopy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Semi-elastic fiber optimisation in python.
 License: MIT
 Author: rgerum
 Author-email: 14153051+rgerum@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: imagecodecs (>=2022.9.26,<2023.0.0)
 Requires-Dist: jointforces (>=1.0.1,<2.0.0)
 Requires-Dist: natsort (>=8.2.0,<9.0.0)
-Requires-Dist: nbsphinx (>=0.8.10,<0.9.0); extra == "docs"
+Requires-Dist: nbsphinx (>=0.8.10,<0.9.0) ; extra == "docs"
+Requires-Dist: nptyping (>=2.4.1,<3.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: openpiv (>=0.24.2,<0.25.0)
 Requires-Dist: pyqt5 (>=5.15.7,<6.0.0)
 Requires-Dist: pyvista (>=0.37.0,<0.38.0)
 Requires-Dist: pyvistaqt (>=0.9.0,<0.10.0)
 Requires-Dist: qimage2ndarray (>=1.9.0,<2.0.0)
 Requires-Dist: qtawesome (>=1.2.1,<2.0.0)
+Requires-Dist: qtrangeslider (>=0.1.5,<0.2.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
-Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0); extra == "docs"
+Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
+Requires-Dist: sphinx-gallery (>=0.11.1,<0.12.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 SAENOPY
 =======
 
 [![DOC](https://readthedocs.org/projects/saenopy/badge/)](https://saenopy.readthedocs.io)
@@ -38,13 +44,20 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center">
   <img src="saenopy/img/Logo.png" />
 </p>
 
 
+SAENOPY is a free open source 3D traction force microscopy software. Its material model is especially well suited for
+tissue-mimicking and typically highly non-linear biopolymer matrices such as collagen, fibrin, or Matrigel. 
 
-SAENOPY a python implementation of the SAENO - Semi-affine Elastic Network Optimizer, originally developed by Julian
- Steinwachs.
+It features a python package to use in scripts and an extensive graphical user interface.
+
+Check out our [Documentation](https://saenopy.readthedocs.io) on how to install and use it or our preprint:
+
+*Dynamic traction force measurements of migrating immune cells in 3D matrices*
+David Böhringer, Mar Cóndor, Lars Bischof, Tina Czerwinski, Andreas Bauer, Caroline Voskens, Silvia Budday, 
+Christoph Mark, Ben Fabry, Richard Gerum
+**bioRxiv 2022.11.16.516758**; doi: https://doi.org/10.1101/2022.11.16.516758
 
-[Documentation](https://saenopy.readthedocs.io)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

