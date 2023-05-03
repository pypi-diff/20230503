# Comparing `tmp/sleplet-1.4.0.tar.gz` & `tmp/sleplet-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.4.0.tar", last modified: Thu Apr 20 16:42:51 2023, max compression
+gzip compressed data, was "sleplet-1.4.1.tar", last modified: Wed May  3 13:58:27 2023, max compression
```

## Comparing `sleplet-1.4.0.tar` & `sleplet-1.4.1.tar`

### file list

```diff
@@ -1,210 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.982827 sleplet-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.950825 sleplet-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.954825 sleplet-1.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.954825 sleplet-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/licence.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/paper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 16:42:35.000000 sleplet-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 16:42:35.000000 sleplet-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 16:42:35.000000 sleplet-1.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-20 16:42:35.000000 sleplet-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-20 16:42:35.000000 sleplet-1.4.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-20 16:42:51.982827 sleplet-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-20 16:42:35.000000 sleplet-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/DOCUMENTATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/config.mako
--rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.950825 sleplet-1.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/examples/arbitrary/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/_denoising_slepian_wavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/_slepian_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/examples/arbitrary/africa/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/denoising_slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/eigenvalues_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/slepian_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/tiling_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/eigenvalues_combined.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/examples/arbitrary/south_america/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/eigenvalues_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/tiling_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/denoising_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/mesh_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/mesh_slepian_eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/mesh_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/produce_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/_denoising_axisym.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/denoising_axisym_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/denoising_axisym_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/denoising_axisym_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/translation_normalisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/wavelet_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/polar_cap/
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/eigenfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/fried_egg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/simons_5_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/simons_5_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/slepian_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/wavelets/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/wavelets/axisymmetric_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/wavelets/axisymmetric_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/paper/
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-04-20 16:42:35.000000 sleplet-1.4.0/paper/arxiv.tex
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-20 16:42:35.000000 sleplet-1.4.0/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-20 16:42:35.000000 sleplet-1.4.0/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-20 16:42:35.000000 sleplet-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:42:51.982827 sleplet-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.950825 sleplet-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.966826 sleplet-1.4.0/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.970827 sleplet-1.4.0/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.970827 sleplet-1.4.0/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.974827 sleplet-1.4.0/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/directional_spin_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.978827 sleplet-1.4.0/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.978827 sleplet-1.4.0/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.982827 sleplet-1.4.0/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.970827 sleplet-1.4.0/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.982827 sleplet-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_arbitrary_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_loading_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_wavelets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.286598 sleplet-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.250598 sleplet-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.258598 sleplet-1.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.262598 sleplet-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/licence.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/paper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 13:58:16.000000 sleplet-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-03 13:58:16.000000 sleplet-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-03 13:58:16.000000 sleplet-1.4.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-03 13:58:16.000000 sleplet-1.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-03 13:58:16.000000 sleplet-1.4.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 13:58:27.282598 sleplet-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-03 13:58:16.000000 sleplet-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.262598 sleplet-1.4.1/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/DOCUMENTATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/config.mako
+-rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.254598 sleplet-1.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/arbitrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/_denoising_slepian_wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/_slepian_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/arbitrary/africa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/denoising_slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/eigenvalues_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/slepian_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/tiling_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/eigenvalues_combined.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/arbitrary/south_america/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/eigenvalues_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/tiling_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/denoising_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/mesh_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/mesh_slepian_eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/mesh_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/produce_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/_denoising_axisym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/denoising_axisym_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/denoising_axisym_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/denoising_axisym_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/translation_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/wavelet_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/examples/polar_cap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/eigenfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/fried_egg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/simons_5_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/simons_5_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/slepian_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/examples/wavelets/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/wavelets/axisymmetric_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/wavelets/axisymmetric_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-03 13:58:16.000000 sleplet-1.4.1/paper/arxiv.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-03 13:58:16.000000 sleplet-1.4.1/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-03 13:58:16.000000 sleplet-1.4.1/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-03 13:58:16.000000 sleplet-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 13:58:16.000000 sleplet-1.4.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:58:27.286598 sleplet-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.254598 sleplet-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.274598 sleplet-1.4.1/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.274598 sleplet-1.4.1/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.278598 sleplet-1.4.1/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/directional_spin_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.274598 sleplet-1.4.1/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_arbitrary_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_loading_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_wavelets.py
```

### Comparing `sleplet-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `sleplet-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `sleplet-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/.github/workflows/deploy.yml` & `sleplet-1.4.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/.github/workflows/documentation.yml` & `sleplet-1.4.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/.github/workflows/examples.yml` & `sleplet-1.4.1/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/.github/workflows/linting.yml` & `sleplet-1.4.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/.github/workflows/test.yml` & `sleplet-1.4.1/.github/workflows/test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -35,7 +35,10 @@
           cache-dependency-path: "pyproject.toml"
 
       - name: Install dependencies
         run: python -m pip install tox tox-gh-actions
 
       - name: Test with tox
         run: tox
+
+      - name: Coverage
+        uses: coverallsapp/github-action@v2
```

### Comparing `sleplet-1.4.0/.pre-commit-config.yaml` & `sleplet-1.4.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.264
     hooks:
       - id: ruff
   - repo: https://github.com/Lucas-C/pre-commit-hooks
     rev: v1.5.1
     hooks:
       - id: forbid-tabs
   - repo: https://github.com/pappasam/toml-sort
@@ -13,15 +13,15 @@
       - id: toml-sort-fix
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.1.1
     hooks:
       - id: mypy
         additional_dependencies: [numpy, pydantic]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-case-conflict
       - id: check-docstring-first
```

### Comparing `sleplet-1.4.0/CITATION.cff` & `sleplet-1.4.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/CONTRIBUTING.md` & `sleplet-1.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/LICENCE.md` & `sleplet-1.4.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/PKG-INFO` & `sleplet-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.0
+Version: 1.4.1
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
         
@@ -56,18 +56,19 @@
 Provides-Extra: readme
 License-File: LICENCE.md
 
 # SLEPLET
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
-[![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
+[![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
```

### Comparing `sleplet-1.4.0/README.md` & `sleplet-1.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # SLEPLET
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
-[![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
+[![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
```

### Comparing `sleplet-1.4.0/documentation/DOCUMENTATION.md` & `sleplet-1.4.1/documentation/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/documentation/config.mako` & `sleplet-1.4.1/documentation/config.mako`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png` & `sleplet-1.4.1/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png` & `sleplet-1.4.1/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/_denoising_slepian_wavelet.py` & `sleplet-1.4.1/examples/arbitrary/_denoising_slepian_wavelet.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/_slepian_wavelet_covariance.py` & `sleplet-1.4.1/examples/arbitrary/_slepian_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/denoising_slepian_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/denoising_slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/eigenvalues_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/eigenvalues_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/slepian_reconstruction_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/slepian_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/tiling_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/tiling_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/africa/wavelet_reconstruction_africa.py` & `sleplet-1.4.1/examples/arbitrary/africa/wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/eigenvalues_combined.py` & `sleplet-1.4.1/examples/arbitrary/eigenvalues_combined.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/eigenvalues_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/eigenvalues_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/slepian_reconstruction_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/slepian_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/tiling_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/tiling_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py` & `sleplet-1.4.1/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/mesh/denoising_slepian_mesh.py` & `sleplet-1.4.1/examples/mesh/denoising_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/mesh/mesh_region.py` & `sleplet-1.4.1/examples/mesh/mesh_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/mesh/mesh_slepian_eigenvalues.py` & `sleplet-1.4.1/examples/mesh/mesh_slepian_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/mesh/mesh_tiling.py` & `sleplet-1.4.1/examples/mesh/mesh_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/misc/_denoising_axisym.py` & `sleplet-1.4.1/examples/misc/_denoising_axisym.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/misc/denoising_axisym_africa.py` & `sleplet-1.4.1/examples/misc/denoising_axisym_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/misc/denoising_axisym_earth.py` & `sleplet-1.4.1/examples/misc/denoising_axisym_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/misc/denoising_axisym_south_america.py` & `sleplet-1.4.1/examples/misc/denoising_axisym_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/misc/translation_normalisation.py` & `sleplet-1.4.1/examples/misc/translation_normalisation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/misc/wavelet_transform.py` & `sleplet-1.4.1/examples/misc/wavelet_transform.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/eigenfunctions.py` & `sleplet-1.4.1/examples/polar_cap/eigenfunctions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/eigenvalues.py` & `sleplet-1.4.1/examples/polar_cap/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/fried_egg.py` & `sleplet-1.4.1/examples/polar_cap/fried_egg.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/simons_5_1.py` & `sleplet-1.4.1/examples/polar_cap/simons_5_1.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/simons_5_3.py` & `sleplet-1.4.1/examples/polar_cap/simons_5_3.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/slepian_coefficients.py` & `sleplet-1.4.1/examples/polar_cap/slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/polar_cap/slepian_error.py` & `sleplet-1.4.1/examples/polar_cap/slepian_error.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/wavelets/axisymmetric_tiling.py` & `sleplet-1.4.1/examples/wavelets/axisymmetric_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/examples/wavelets/axisymmetric_wavelet_covariance.py` & `sleplet-1.4.1/examples/wavelets/axisymmetric_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/paper/arxiv.tex` & `sleplet-1.4.1/paper/arxiv.tex`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/paper/paper.bib` & `sleplet-1.4.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/paper/paper.md` & `sleplet-1.4.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/pyproject.toml` & `sleplet-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 legacy_tox_ini = """
     [gh-actions]
     python =
         3.10: py310
 
     [testenv]
     commands =
-        pytest --cov --slow
+        pytest --cov --cov-report=lcov --slow
     deps =
         pytest-cov
         pytest-skip-slow
 
     [tox]
     env_list =
         py310
```

### Comparing `sleplet-1.4.0/src/sleplet/__init__.py` & `sleplet-1.4.1/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_bool_methods.py` & `sleplet-1.4.1/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_class_lists.py` & `sleplet-1.4.1/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_convolution_methods.py` & `sleplet-1.4.1/src/sleplet/_convolution_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.4.1/src/sleplet/_data/create_earth_flm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D100
 import numpy as np
 import pyssht as ssht
 from numpy import typing as npt
 from scipy import io as sio
 
 import sleplet._data.setup_pooch
 import sleplet._smoothing
```

### Comparing `sleplet-1.4.0/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.4.1/src/sleplet/_data/create_wmap_flm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D100
 import numpy as np
 import pyssht as ssht
 from numpy import typing as npt
 from numpy.random import default_rng
 from scipy import io as sio
 
 import sleplet._data.setup_pooch
```

### Comparing `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_data/setup_pooch.py` & `sleplet-1.4.1/src/sleplet/_data/setup_pooch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D100
 import logging
 import os
 
 import pooch
 from platformdirs import user_data_path
 
 _logger = logging.getLogger(__name__)
```

### Comparing `sleplet-1.4.0/src/sleplet/_integration_methods.py` & `sleplet-1.4.1/src/sleplet/_integration_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_mask_methods.py` & `sleplet-1.4.1/src/sleplet/_mask_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_mesh_methods.py` & `sleplet-1.4.1/src/sleplet/_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_parallel_methods.py` & `sleplet-1.4.1/src/sleplet/_parallel_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_plotly_methods.py` & `sleplet-1.4.1/src/sleplet/_plotly_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.4.1/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D100
 import logging
 from argparse import ArgumentParser, Namespace
 
 import sleplet._class_lists
 import sleplet._string_methods
 import sleplet.meshes.mesh
 import sleplet.meshes.mesh_coefficients
@@ -99,15 +100,15 @@
         field,
         amplitude=amplitude,
         normalise=normalise,
         region=hasattr(f, "mesh_slepian"),
     ).execute()
 
 
-def main() -> None:
+def main() -> None:  # noqa: D103
     args = read_args()
     _logger.info(f"mesh: '{args.function}', plotting method: '{args.method}'")
 
     # function to plot
     mesh = sleplet.meshes.mesh.Mesh(args.function, zoom=args.zoom)
     f = sleplet._class_lists.MESH_COEFFICIENTS[
         sleplet._string_methods.convert_classes_list_to_snake_case(
```

### Comparing `sleplet-1.4.0/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.4.1/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D100
 import logging
 from argparse import ArgumentParser, Namespace
 
 import numpy as np
 import pyssht as ssht
 from numpy import typing as npt
 
@@ -341,15 +342,15 @@
     )
     coefficients = f.convolve(g_coefficients, coefficients, shannon=shannon)
 
     filename += f"_convolved_{g.name}"
     return coefficients, filename
 
 
-def main() -> None:
+def main() -> None:  # noqa: D103
     args = read_args()
 
     mask = sleplet._mask_methods.create_default_region() if args.region else None
 
     f = sleplet._class_lists.COEFFICIENTS[
         sleplet._string_methods.convert_classes_list_to_snake_case(
             sleplet._class_lists.COEFFICIENTS,
```

### Comparing `sleplet-1.4.0/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.4.1/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_smoothing.py` & `sleplet-1.4.1/src/sleplet/_smoothing.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/_string_methods.py` & `sleplet-1.4.1/src/sleplet/_string_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/__init__.py` & `sleplet-1.4.1/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/africa.py` & `sleplet-1.4.1/src/sleplet/functions/africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/coefficients.py` & `sleplet-1.4.1/src/sleplet/functions/coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/dirac_delta.py` & `sleplet-1.4.1/src/sleplet/functions/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/directional_spin_wavelets.py` & `sleplet-1.4.1/src/sleplet/functions/directional_spin_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/earth.py` & `sleplet-1.4.1/src/sleplet/functions/earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.4.1/src/sleplet/functions/elongated_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/flm.py` & `sleplet-1.4.1/src/sleplet/functions/flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/fp.py` & `sleplet-1.4.1/src/sleplet/functions/fp.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/gaussian.py` & `sleplet-1.4.1/src/sleplet/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.4.1/src/sleplet/functions/harmonic_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/identity.py` & `sleplet-1.4.1/src/sleplet/functions/identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/noise_earth.py` & `sleplet-1.4.1/src/sleplet/functions/noise_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/ridgelets.py` & `sleplet-1.4.1/src/sleplet/functions/ridgelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian.py` & `sleplet-1.4.1/src/sleplet/functions/slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_africa.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_identity.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_noise_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.4.1/src/sleplet/functions/slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/south_america.py` & `sleplet-1.4.1/src/sleplet/functions/south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.4.1/src/sleplet/functions/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.4.1/src/sleplet/functions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/functions/wmap.py` & `sleplet-1.4.1/src/sleplet/functions/wmap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/harmonic_methods.py` & `sleplet-1.4.1/src/sleplet/harmonic_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/__init__.py` & `sleplet-1.4.1/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.4.1/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_field.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/noise.py` & `sleplet-1.4.1/src/sleplet/noise.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/plot_methods.py` & `sleplet-1.4.1/src/sleplet/plot_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.4.1/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.4.1/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.4.1/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian/region.py` & `sleplet-1.4.1/src/sleplet/slepian/region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.4.1/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.4.1/src/sleplet/slepian/slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.4.1/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.4.1/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/slepian_methods.py` & `sleplet-1.4.1/src/sleplet/slepian_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet/wavelet_methods.py` & `sleplet-1.4.1/src/sleplet/wavelet_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.4.1/src/sleplet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.0
+Version: 1.4.1
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
         
@@ -56,18 +56,19 @@
 Provides-Extra: readme
 License-File: LICENCE.md
 
 # SLEPLET
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
-[![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
+[![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
```

### Comparing `sleplet-1.4.0/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.4.1/src/sleplet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 CITATION.cff
 CONTRIBUTING.md
 LICENCE.md
 README.md
 pyproject.toml
+renovate.json
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/documentation.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
 .github/workflows/deploy.yml
 .github/workflows/documentation.yml
 .github/workflows/examples.yml
```

### Comparing `sleplet-1.4.0/tests/conftest.py` & `sleplet-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_arbitrary_region.py` & `sleplet-1.4.1/tests/test_arbitrary_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_arrays.py` & `sleplet-1.4.1/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_bool.py` & `sleplet-1.4.1/tests/test_bool.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_convolution.py` & `sleplet-1.4.1/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_decomposition.py` & `sleplet-1.4.1/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_harmonic.py` & `sleplet-1.4.1/tests/test_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_loading_pooch.py` & `sleplet-1.4.1/tests/test_loading_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_mesh.py` & `sleplet-1.4.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_plot.py` & `sleplet-1.4.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_region.py` & `sleplet-1.4.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_slepian_mesh.py` & `sleplet-1.4.1/tests/test_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_strings.py` & `sleplet-1.4.1/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_translation.py` & `sleplet-1.4.1/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.0/tests/test_wavelets.py` & `sleplet-1.4.1/tests/test_wavelets.py`

 * *Files identical despite different names*

