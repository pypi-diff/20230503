# Comparing `tmp/pyvista-0.38.5.tar.gz` & `tmp/pyvista-0.38.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-0.38.5.tar", last modified: Fri Mar 17 20:03:05 2023, max compression
+gzip compressed data, was "pyvista-0.38.6.tar", last modified: Wed May  3 12:47:52 2023, max compression
```

## Comparing `pyvista-0.38.5.tar` & `pyvista-0.38.6.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.385543 pyvista-0.38.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-03-17 19:48:32.000000 pyvista-0.38.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-03-17 19:48:32.000000 pyvista-0.38.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-03-17 19:48:32.000000 pyvista-0.38.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11759 2023-03-17 20:03:05.385543 pyvista-0.38.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-03-17 19:48:32.000000 pyvista-0.38.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4361 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.353543 pyvista-0.38.5/pyvista/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2229 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    24325 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/_vtk.py
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.357543 pyvista-0.38.5/pyvista/core/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/cell.py
--rw-r--r--   0 runner    (1001) docker     (122)     5196 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/celltype.py
--rw-r--r--   0 runner    (1001) docker     (122)    39744 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/composite.py
--rw-r--r--   0 runner    (1001) docker     (122)    21356 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    90436 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    43891 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/datasetattributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1417 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.357543 pyvista-0.38.5/pyvista/core/filters/
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6488 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/composite.py
--rw-r--r--   0 runner    (1001) docker     (122)   205728 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/data_set.py
--rw-r--r--   0 runner    (1001) docker     (122)   130158 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/poly_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/rectilinear_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     7258 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/structured_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    29260 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/uniform_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/filters/unstructured_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    27593 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    15741 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    99228 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/core/pyvista_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.357543 pyvista-0.38.5/pyvista/demos/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16005 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/demos/demos.py
--rw-r--r--   0 runner    (1001) docker     (122)     7047 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/demos/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.365543 pyvista-0.38.5/pyvista/examples/
--rw-r--r--   0 runner    (1001) docker     (122)   463087 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/2k_earth_daymap.jpg
--rwxr-xr-x   0 runner    (1001) docker     (122)      193 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    74547 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/airplane.ply
--rw-r--r--   0 runner    (1001) docker     (122)    17941 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/ant.ply
--rw-r--r--   0 runner    (1001) docker     (122)    21542 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)   522284 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/channels.vti
--rw-r--r--   0 runner    (1001) docker     (122)   136310 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/downloads.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11939 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (122)    37447 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/globe.vtk
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/gltf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/hexbeam.vtk
--rw-r--r--   0 runner    (1001) docker     (122)    20128 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/nut.ply
--rw-r--r--   0 runner    (1001) docker     (122)    27105 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/planets.py
--rw-r--r--   0 runner    (1001) docker     (122)   228473 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/rectilinear.vtk
--rw-r--r--   0 runner    (1001) docker     (122)    16237 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/sphere.ply
--rw-r--r--   0 runner    (1001) docker     (122)    14094 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/uniform.vtk
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/examples/vrml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.365543 pyvista-0.38.5/pyvista/ext/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16150 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/ext/coverage.py
--rw-r--r--   0 runner    (1001) docker     (122)    18361 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/ext/plot_directive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.365543 pyvista-0.38.5/pyvista/jupyter/
--rw-r--r--   0 runner    (1001) docker     (122)     7467 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/jupyter/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/jupyter/pv_ipygany.py
--rw-r--r--   0 runner    (1001) docker     (122)    22749 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/jupyter/pv_pythreejs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.373543 pyvista-0.38.5/pyvista/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)    32810 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/_property.py
--rw-r--r--   0 runner    (1001) docker     (122)    12811 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/actor_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)    14627 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/background_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)    26773 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/camera.py
--rw-r--r--   0 runner    (1001) docker     (122)   143967 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/charts.py
--rw-r--r--   0 runner    (1001) docker     (122)    39881 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)    28561 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/composite_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    25828 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/export_vtkjs.py
--rw-r--r--   0 runner    (1001) docker     (122)    13613 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    40969 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/lights.py
--rw-r--r--   0 runner    (1001) docker     (122)    35180 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    35551 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/opts.py
--rw-r--r--   0 runner    (1001) docker     (122)    45425 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/picking.py
--rw-r--r--   0 runner    (1001) docker     (122)   249068 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/prop3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/render_passes.py
--rw-r--r--   0 runner    (1001) docker     (122)    37427 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/render_window_interactor.py
--rw-r--r--   0 runner    (1001) docker     (122)   119380 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)    21769 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    19505 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/scalar_bars.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)    18705 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     1636 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/volume.py
--rw-r--r--   0 runner    (1001) docker     (122)    12557 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/volume_property.py
--rw-r--r--   0 runner    (1001) docker     (122)    83778 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    86848 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.373543 pyvista-0.38.5/pyvista/trame/
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/trame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11691 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/trame/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (122)    17768 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/trame/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     7282 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/trame/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.377543 pyvista-0.38.5/pyvista/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11449 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/cell_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    13992 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12939 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     8721 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    19325 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)    46203 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    49454 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    36348 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/parametric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    71624 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5933 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/transformations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-03-17 19:48:33.000000 pyvista-0.38.5/pyvista/utilities/xvfb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.353543 pyvista-0.38.5/pyvista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11759 2023-03-17 20:03:05.000000 pyvista-0.38.5/pyvista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4317 2023-03-17 20:03:05.000000 pyvista-0.38.5/pyvista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 20:03:05.000000 pyvista-0.38.5/pyvista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-03-17 20:03:05.000000 pyvista-0.38.5/pyvista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-17 20:03:05.000000 pyvista-0.38.5/pyvista.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-17 20:03:05.385543 pyvista-0.38.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-03-17 19:48:33.000000 pyvista-0.38.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:03:05.385543 pyvista-0.38.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9856 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (122)     9049 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (122)    38514 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_charts.py
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)    27072 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_dataobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    50850 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    21038 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_datasetattributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (122)   100362 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     9972 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    50389 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    12704 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_imaging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)    10294 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_lights.py
--rw-r--r--   0 runner    (1001) docker     (122)     6232 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_meshio.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     6771 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     3544 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_parametric_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_picking.py
--rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (122)     6899 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_pointset.py
--rw-r--r--   0 runner    (1001) docker     (122)    30357 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_polydata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_pyvista_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_render_pass.py
--rw-r--r--   0 runner    (1001) docker     (122)     6380 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_render_window_interactor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_scalar_bars.py
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_scraper.py
--rw-r--r--   0 runner    (1001) docker     (122)    17936 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_tinypages.py
--rw-r--r--   0 runner    (1001) docker     (122)    30477 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-03-17 19:48:33.000000 pyvista-0.38.5/tests/test_volume_property.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.667746 pyvista-0.38.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-05-03 12:33:54.000000 pyvista-0.38.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-05-03 12:33:54.000000 pyvista-0.38.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-03 12:33:54.000000 pyvista-0.38.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11759 2023-05-03 12:47:52.667746 pyvista-0.38.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-05-03 12:33:54.000000 pyvista-0.38.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4361 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.643745 pyvista-0.38.6/pyvista/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2229 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24325 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.643745 pyvista-0.38.6/pyvista/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/cell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5196 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/celltype.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39744 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21356 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    90436 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43891 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/datasetattributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1417 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.647745 pyvista-0.38.6/pyvista/core/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6488 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)   205728 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)   130158 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/poly_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/rectilinear_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7258 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/structured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29260 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/uniform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/filters/unstructured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27593 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15741 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    99228 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/core/pyvista_ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.647745 pyvista-0.38.6/pyvista/demos/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16005 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/demos/demos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7047 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/demos/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.651745 pyvista-0.38.6/pyvista/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)   463087 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/2k_earth_daymap.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      193 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74547 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/airplane.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    17941 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/ant.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    21542 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)   522284 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/channels.vti
+-rw-r--r--   0 runner    (1001) docker     (122)   136310 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/downloads.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11939 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37447 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/globe.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/hexbeam.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)    20128 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/nut.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    27105 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/planets.py
+-rw-r--r--   0 runner    (1001) docker     (122)   228473 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/rectilinear.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)    16237 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/sphere.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    14094 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/uniform.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/examples/vrml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.651745 pyvista-0.38.6/pyvista/ext/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16150 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/ext/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18361 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/ext/plot_directive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.651745 pyvista-0.38.6/pyvista/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (122)     7467 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/jupyter/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/jupyter/pv_ipygany.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22749 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/jupyter/pv_pythreejs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.659746 pyvista-0.38.6/pyvista/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32810 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12811 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/actor_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14627 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/background_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26773 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)   143967 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/charts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39881 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28561 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/composite_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25828 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/export_vtkjs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13613 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40969 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/lights.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35180 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35551 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/opts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45425 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/picking.py
+-rw-r--r--   0 runner    (1001) docker     (122)   249445 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/prop3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/render_passes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37427 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/render_window_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (122)   119380 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21769 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19505 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/scalar_bars.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18705 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1636 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12557 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/volume_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83778 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    86848 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.659746 pyvista-0.38.6/pyvista/trame/
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/trame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11691 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/trame/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17768 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/trame/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7282 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/trame/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.663746 pyvista-0.38.6/pyvista/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11449 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/cell_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13992 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12939 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8721 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19325 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46203 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49454 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36348 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/parametric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71624 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5933 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-03 12:33:55.000000 pyvista-0.38.6/pyvista/utilities/xvfb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.643745 pyvista-0.38.6/pyvista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11759 2023-05-03 12:47:52.000000 pyvista-0.38.6/pyvista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4317 2023-05-03 12:47:52.000000 pyvista-0.38.6/pyvista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 12:47:52.000000 pyvista-0.38.6/pyvista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-05-03 12:47:52.000000 pyvista-0.38.6/pyvista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-03 12:47:52.000000 pyvista-0.38.6/pyvista.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 12:47:52.667746 pyvista-0.38.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-03 12:33:55.000000 pyvista-0.38.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 12:47:52.667746 pyvista-0.38.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9856 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9049 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38514 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_charts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27072 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50850 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21038 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_datasetattributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (122)   100362 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9972 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50389 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12704 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10294 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_lights.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6232 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_meshio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6771 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3544 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_parametric_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_picking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6899 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_pointset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30357 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_polydata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_pyvista_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_render_pass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6380 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_render_window_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_scalar_bars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17936 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_tinypages.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30477 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-03 12:33:55.000000 pyvista-0.38.6/tests/test_volume_property.py
```

### Comparing `pyvista-0.38.5/AUTHORS.rst` & `pyvista-0.38.6/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/LICENSE` & `pyvista-0.38.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/PKG-INFO` & `pyvista-0.38.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.38.5
+Version: 0.38.6
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.38.5/README.rst` & `pyvista-0.38.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyproject.toml` & `pyvista-0.38.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/__init__.py` & `pyvista-0.38.6/pyvista/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/_typing.py` & `pyvista-0.38.6/pyvista/_typing.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/_vtk.py` & `pyvista-0.38.6/pyvista/_vtk.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/__init__.py` & `pyvista-0.38.6/pyvista/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/cell.py` & `pyvista-0.38.6/pyvista/core/cell.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/celltype.py` & `pyvista-0.38.6/pyvista/core/celltype.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/composite.py` & `pyvista-0.38.6/pyvista/core/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/dataobject.py` & `pyvista-0.38.6/pyvista/core/dataobject.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/dataset.py` & `pyvista-0.38.6/pyvista/core/dataset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/datasetattributes.py` & `pyvista-0.38.6/pyvista/core/datasetattributes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/errors.py` & `pyvista-0.38.6/pyvista/core/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/__init__.py` & `pyvista-0.38.6/pyvista/core/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/composite.py` & `pyvista-0.38.6/pyvista/core/filters/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/data_set.py` & `pyvista-0.38.6/pyvista/core/filters/data_set.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/poly_data.py` & `pyvista-0.38.6/pyvista/core/filters/poly_data.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/rectilinear_grid.py` & `pyvista-0.38.6/pyvista/core/filters/rectilinear_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/structured_grid.py` & `pyvista-0.38.6/pyvista/core/filters/structured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/uniform_grid.py` & `pyvista-0.38.6/pyvista/core/filters/uniform_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/filters/unstructured_grid.py` & `pyvista-0.38.6/pyvista/core/filters/unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/grid.py` & `pyvista-0.38.6/pyvista/core/grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/objects.py` & `pyvista-0.38.6/pyvista/core/objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/pointset.py` & `pyvista-0.38.6/pyvista/core/pointset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/core/pyvista_ndarray.py` & `pyvista-0.38.6/pyvista/core/pyvista_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/demos/demos.py` & `pyvista-0.38.6/pyvista/demos/demos.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/demos/logo.py` & `pyvista-0.38.6/pyvista/demos/logo.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/errors.py` & `pyvista-0.38.6/pyvista/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/2k_earth_daymap.jpg` & `pyvista-0.38.6/pyvista/examples/2k_earth_daymap.jpg`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/airplane.ply` & `pyvista-0.38.6/pyvista/examples/airplane.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/ant.ply` & `pyvista-0.38.6/pyvista/examples/ant.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/cells.py` & `pyvista-0.38.6/pyvista/examples/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/channels.vti` & `pyvista-0.38.6/pyvista/examples/channels.vti`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/downloads.py` & `pyvista-0.38.6/pyvista/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/examples.py` & `pyvista-0.38.6/pyvista/examples/examples.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/globe.vtk` & `pyvista-0.38.6/pyvista/examples/globe.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/gltf.py` & `pyvista-0.38.6/pyvista/examples/gltf.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/hexbeam.vtk` & `pyvista-0.38.6/pyvista/examples/hexbeam.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/nut.ply` & `pyvista-0.38.6/pyvista/examples/nut.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/planets.py` & `pyvista-0.38.6/pyvista/examples/planets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/rectilinear.vtk` & `pyvista-0.38.6/pyvista/examples/rectilinear.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/sphere.ply` & `pyvista-0.38.6/pyvista/examples/sphere.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/uniform.vtk` & `pyvista-0.38.6/pyvista/examples/uniform.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/examples/vrml.py` & `pyvista-0.38.6/pyvista/examples/vrml.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/ext/coverage.py` & `pyvista-0.38.6/pyvista/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/ext/plot_directive.py` & `pyvista-0.38.6/pyvista/ext/plot_directive.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/jupyter/__init__.py` & `pyvista-0.38.6/pyvista/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/jupyter/notebook.py` & `pyvista-0.38.6/pyvista/jupyter/notebook.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/jupyter/pv_ipygany.py` & `pyvista-0.38.6/pyvista/jupyter/pv_ipygany.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/jupyter/pv_pythreejs.py` & `pyvista-0.38.6/pyvista/jupyter/pv_pythreejs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/__init__.py` & `pyvista-0.38.6/pyvista/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/_plotting.py` & `pyvista-0.38.6/pyvista/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/_property.py` & `pyvista-0.38.6/pyvista/plotting/_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/actor.py` & `pyvista-0.38.6/pyvista/plotting/actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/actor_properties.py` & `pyvista-0.38.6/pyvista/plotting/actor_properties.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/axes.py` & `pyvista-0.38.6/pyvista/plotting/axes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/axes_actor.py` & `pyvista-0.38.6/pyvista/plotting/axes_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/background_renderer.py` & `pyvista-0.38.6/pyvista/plotting/background_renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/camera.py` & `pyvista-0.38.6/pyvista/plotting/camera.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/charts.py` & `pyvista-0.38.6/pyvista/plotting/charts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/colors.py` & `pyvista-0.38.6/pyvista/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/composite_mapper.py` & `pyvista-0.38.6/pyvista/plotting/composite_mapper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/export_vtkjs.py` & `pyvista-0.38.6/pyvista/plotting/export_vtkjs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/helpers.py` & `pyvista-0.38.6/pyvista/plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/lights.py` & `pyvista-0.38.6/pyvista/plotting/lights.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/lookup_table.py` & `pyvista-0.38.6/pyvista/plotting/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/mapper.py` & `pyvista-0.38.6/pyvista/plotting/mapper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/opts.py` & `pyvista-0.38.6/pyvista/plotting/opts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/picking.py` & `pyvista-0.38.6/pyvista/plotting/picking.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/plotting.py` & `pyvista-0.38.6/pyvista/plotting/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -4827,30 +4827,37 @@
         >>> import pyvista
         >>> pl = pyvista.Plotter()
         >>> pl.open_gif('movie.gif', fps=8, palettesize=64)  # doctest:+SKIP
 
         See :ref:`gif_movie_example` for a full example using this method.
 
         """
-        from imageio import get_writer
+        try:
+            from imageio import __version__, get_writer
+        except ModuleNotFoundError:  # pragma: no cover
+            raise ModuleNotFoundError(
+                'Install imageio to use `open_gif` with:\n\n   pip install imageio'
+            ) from None
 
         if filename[-3:] != 'gif':
             raise ValueError('Unsupported filetype.  Must end in .gif')
         if isinstance(pyvista.FIGURE_PATH, str) and not os.path.isabs(filename):
             filename = os.path.join(pyvista.FIGURE_PATH, filename)
         self._gif_filename = os.path.abspath(filename)
-        self.mwriter = get_writer(
-            filename,
-            mode='I',
-            loop=loop,
-            fps=fps,
-            palettesize=palettesize,
-            subrectangles=subrectangles,
-            **kwargs,
-        )
+
+        kwargs['mode'] = 'I'
+        kwargs['loop'] = loop
+        kwargs['palettesize'] = palettesize
+        kwargs['subrectangles'] = subrectangles
+        if scooby.meets_version(__version__, '2.28.1'):
+            kwargs['duration'] = 1000 * 1 / fps
+        else:  # pragma: no cover
+            kwargs['fps'] = fps
+
+        self.mwriter = get_writer(filename, **kwargs)
 
     def write_frame(self):
         """Write a single frame to the movie file.
 
         Examples
         --------
         >>> import pyvista
```

### Comparing `pyvista-0.38.5/pyvista/plotting/prop3d.py` & `pyvista-0.38.6/pyvista/plotting/prop3d.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/render_passes.py` & `pyvista-0.38.6/pyvista/plotting/render_passes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/render_window_interactor.py` & `pyvista-0.38.6/pyvista/plotting/render_window_interactor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/renderer.py` & `pyvista-0.38.6/pyvista/plotting/renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/renderers.py` & `pyvista-0.38.6/pyvista/plotting/renderers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/scalar_bars.py` & `pyvista-0.38.6/pyvista/plotting/scalar_bars.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/tools.py` & `pyvista-0.38.6/pyvista/plotting/tools.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/volume.py` & `pyvista-0.38.6/pyvista/plotting/volume.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/volume_property.py` & `pyvista-0.38.6/pyvista/plotting/volume_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/plotting/widgets.py` & `pyvista-0.38.6/pyvista/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/themes.py` & `pyvista-0.38.6/pyvista/themes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/trame/__init__.py` & `pyvista-0.38.6/pyvista/trame/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/trame/jupyter.py` & `pyvista-0.38.6/pyvista/trame/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/trame/ui.py` & `pyvista-0.38.6/pyvista/trame/ui.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/trame/views.py` & `pyvista-0.38.6/pyvista/trame/views.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/__init__.py` & `pyvista-0.38.6/pyvista/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/algorithms.py` & `pyvista-0.38.6/pyvista/utilities/algorithms.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/arrays.py` & `pyvista-0.38.6/pyvista/utilities/arrays.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/cell_type_helper.py` & `pyvista-0.38.6/pyvista/utilities/cell_type_helper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/cells.py` & `pyvista-0.38.6/pyvista/utilities/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/common.py` & `pyvista-0.38.6/pyvista/utilities/common.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/docs.py` & `pyvista-0.38.6/pyvista/utilities/docs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/errors.py` & `pyvista-0.38.6/pyvista/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/features.py` & `pyvista-0.38.6/pyvista/utilities/features.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/fileio.py` & `pyvista-0.38.6/pyvista/utilities/fileio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/geometric_objects.py` & `pyvista-0.38.6/pyvista/utilities/geometric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/helpers.py` & `pyvista-0.38.6/pyvista/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/misc.py` & `pyvista-0.38.6/pyvista/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/parametric_objects.py` & `pyvista-0.38.6/pyvista/utilities/parametric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/reader.py` & `pyvista-0.38.6/pyvista/utilities/reader.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/regression.py` & `pyvista-0.38.6/pyvista/utilities/regression.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/sphinx_gallery.py` & `pyvista-0.38.6/pyvista/utilities/sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/transformations.py` & `pyvista-0.38.6/pyvista/utilities/transformations.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/wrappers.py` & `pyvista-0.38.6/pyvista/utilities/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista/utilities/xvfb.py` & `pyvista-0.38.6/pyvista/utilities/xvfb.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/pyvista.egg-info/PKG-INFO` & `pyvista-0.38.6/pyvista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.38.5
+Version: 0.38.6
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.38.5/pyvista.egg-info/SOURCES.txt` & `pyvista-0.38.6/pyvista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_actor.py` & `pyvista-0.38.6/tests/test_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_axes.py` & `pyvista-0.38.6/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_camera.py` & `pyvista-0.38.6/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_cells.py` & `pyvista-0.38.6/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_charts.py` & `pyvista-0.38.6/tests/test_charts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_colors.py` & `pyvista-0.38.6/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_composite.py` & `pyvista-0.38.6/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_dataobject.py` & `pyvista-0.38.6/tests/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_dataset.py` & `pyvista-0.38.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_datasetattributes.py` & `pyvista-0.38.6/tests/test_datasetattributes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_demos.py` & `pyvista-0.38.6/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_export.py` & `pyvista-0.38.6/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_filters.py` & `pyvista-0.38.6/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_geometric_objects.py` & `pyvista-0.38.6/tests/test_geometric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_grid.py` & `pyvista-0.38.6/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_helpers.py` & `pyvista-0.38.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_imaging.py` & `pyvista-0.38.6/tests/test_imaging.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_init.py` & `pyvista-0.38.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_lights.py` & `pyvista-0.38.6/tests/test_lights.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_lookup_table.py` & `pyvista-0.38.6/tests/test_lookup_table.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_meshio.py` & `pyvista-0.38.6/tests/test_meshio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_objects.py` & `pyvista-0.38.6/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_parametric_geometry.py` & `pyvista-0.38.6/tests/test_parametric_geometry.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_picking.py` & `pyvista-0.38.6/tests/test_picking.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_plotter.py` & `pyvista-0.38.6/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_pointset.py` & `pyvista-0.38.6/tests/test_pointset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_polydata.py` & `pyvista-0.38.6/tests/test_polydata.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_property.py` & `pyvista-0.38.6/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_pyvista_ndarray.py` & `pyvista-0.38.6/tests/test_pyvista_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_regression.py` & `pyvista-0.38.6/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_render_pass.py` & `pyvista-0.38.6/tests/test_render_pass.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_render_window_interactor.py` & `pyvista-0.38.6/tests/test_render_window_interactor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_renderer.py` & `pyvista-0.38.6/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_scalar_bars.py` & `pyvista-0.38.6/tests/test_scalar_bars.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_scraper.py` & `pyvista-0.38.6/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_theme.py` & `pyvista-0.38.6/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_tinypages.py` & `pyvista-0.38.6/tests/test_tinypages.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_utilities.py` & `pyvista-0.38.6/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.38.5/tests/test_volume_property.py` & `pyvista-0.38.6/tests/test_volume_property.py`

 * *Files identical despite different names*

