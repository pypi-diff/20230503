# Comparing `tmp/masci-tools-0.9.0a0.tar.gz` & `tmp/masci-tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masci-tools-0.9.0a0.tar", last modified: Fri Mar 25 10:55:27 2022, max compression
+gzip compressed data, was "masci-tools-0.9.1.tar", last modified: Tue Apr  5 08:04:29 2022, max compression
```

## Comparing `masci-tools-0.9.0a0.tar` & `masci-tools-0.9.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     3769 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     3130 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1898 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.github/workflows/fleur-release.yml
--rw-r--r--   0        0        0     2838 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.gitignore
--rw-r--r--   0        0        0     2854 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.readthedocs.yml
--rw-r--r--   0        0        0     4853 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/.zenodo.json
--rw-r--r--   0        0        0      298 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/AUTHORS.txt
--rw-r--r--   0        0        0    26472 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     1267 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/LICENSE.txt
--rw-r--r--   0        0        0     2925 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/README.md
--rw-r--r--   0        0        0      354 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/codecov.yml
--rw-r--r--   0        0        0     5612 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/docs/Makefile
--rw-r--r--   0        0        0      187 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/docs/source/_static/theme_overrides.css
--rw-r--r--   0        0        0    13394 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/docs/source/conf.py
--rw-r--r--   0        0        0     6806 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/docs/source/devel_guide/fleur_parser.rst
--rw-r--r--   0        0        0      156 2022-03-25 10:55:23.333321 masci-tools-0.9.0a0/docs/source/devel_guide/index.rst
--rw-r--r--   0        0        0     6408 2022-03-25 10:55:23.337321 masci-tools-0.9.0a0/docs/source/devel_guide/plot_data.rst
--rw-r--r--   0        0        0    19222 2022-03-25 10:55:23.337321 masci-tools-0.9.0a0/docs/source/devel_guide/plotting.rst
--rw-r--r--   0        0        0   372758 2022-03-25 10:55:23.337321 masci-tools-0.9.0a0/docs/source/images/bandstructure_simple_non_spinpol.png
--rw-r--r--   0        0        0   581631 2022-03-25 10:55:23.341321 masci-tools-0.9.0a0/docs/source/images/bandstructure_simple_spinpol.png
--rw-r--r--   0        0        0   602284 2022-03-25 10:55:23.345321 masci-tools-0.9.0a0/docs/source/images/bandstructure_weighted_non_spinpol.png
--rw-r--r--   0        0        0   961340 2022-03-25 10:55:23.353322 masci-tools-0.9.0a0/docs/source/images/bandstructure_weighted_spinpol.png
--rw-r--r--   0        0        0   491343 2022-03-25 10:55:23.357322 masci-tools-0.9.0a0/docs/source/images/dos_non_spinpol_multiplied.png
--rw-r--r--   0        0        0   541938 2022-03-25 10:55:23.361322 masci-tools-0.9.0a0/docs/source/images/dos_non_spinpol_selection.png
--rw-r--r--   0        0        0   470378 2022-03-25 10:55:23.365322 masci-tools-0.9.0a0/docs/source/images/dos_non_spinpol_standard.png
--rw-r--r--   0        0        0   474437 2022-03-25 10:55:23.365322 masci-tools-0.9.0a0/docs/source/images/dos_spinpol_selection.png
--rw-r--r--   0        0        0   458299 2022-03-25 10:55:23.369322 masci-tools-0.9.0a0/docs/source/images/dos_spinpol_standard.png
--rw-r--r--   0        0        0   268777 2022-03-25 10:55:23.373322 masci-tools-0.9.0a0/docs/source/images/scatter_multi.png
--rw-r--r--   0        0        0   245355 2022-03-25 10:55:23.373322 masci-tools-0.9.0a0/docs/source/images/scatter_multi_global_params.png
--rw-r--r--   0        0        0   247105 2022-03-25 10:55:23.373322 masci-tools-0.9.0a0/docs/source/images/scatter_multi_specific_params.png
--rw-r--r--   0        0        0   165633 2022-03-25 10:55:23.377323 masci-tools-0.9.0a0/docs/source/images/scatterplot_defaults.png
--rw-r--r--   0        0        0   194101 2022-03-25 10:55:23.377323 masci-tools-0.9.0a0/docs/source/images/scatterplot_labels.png
--rw-r--r--   0        0        0   173314 2022-03-25 10:55:23.377323 masci-tools-0.9.0a0/docs/source/images/scatterplot_limits.png
--rw-r--r--   0        0        0   162022 2022-03-25 10:55:23.377323 masci-tools-0.9.0a0/docs/source/images/scatterplot_params.png
--rw-r--r--   0        0        0   171655 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/images/scatterplot_scale.png
--rw-r--r--   0        0        0   170193 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/images/scatterplot_standard.png
--rw-r--r--   0        0        0     2201 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/index.rst
--rw-r--r--   0        0        0     3110 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/module_guide/code.rst
--rw-r--r--   0        0        0      135 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/module_guide/mg_index.rst
--rw-r--r--   0        0        0     2009 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/module_guide/tools.rst
--rw-r--r--   0        0        0       79 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/reference/_changelog.md
--rw-r--r--   0        0        0       71 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/reference/index.rst
--rw-r--r--   0        0        0     9368 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/user_guide/fleur_parser.rst
--rw-r--r--   0        0        0     9785 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/user_guide/fleur_plots.rst
--rw-r--r--   0        0        0    10210 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/user_guide/fleurxmlmodifier.rst
--rw-r--r--   0        0        0     9511 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/user_guide/hdf5_parser.rst
--rw-r--r--   0        0        0      175 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0    14842 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/docs/source/user_guide/plotting.rst
--rw-r--r--   0        0        0     1511 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/__init__.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/__init__.py
--rw-r--r--   0        0        0      109 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/commands/__init__.py
--rw-r--r--   0        0        0     9339 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/commands/fleur_schema.py
--rw-r--r--   0        0        0    11028 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/commands/parse.py
--rw-r--r--   0        0        0     3061 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/commands/plot.py
--rw-r--r--   0        0        0      566 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/commands/root.py
--rw-r--r--   0        0        0      219 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/commands/tools.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/parameters/__init__.py
--rw-r--r--   0        0        0     1769 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/parameters/slice.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/utils/__init__.py
--rw-r--r--   0        0        0     9387 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/cmdline/utils/echo.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/__init__.py
--rw-r--r--   0        0        0     1919 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/cif2inp_ase.py
--rw-r--r--   0        0        0    24342 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/common_functions.py
--rw-r--r--   0        0        0    27518 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/fleur_inpgen.py
--rw-r--r--   0        0        0    53247 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/fleurxmlmodifier.py
--rw-r--r--   0        0        0     4415 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/hdf5_util.py
--rw-r--r--   0        0        0     9707 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/io_fleurxml.py
--rw-r--r--   0        0        0     8227 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/io_nmmpmat.py
--rw-r--r--   0        0        0   101099 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/kkr_params.py
--rw-r--r--   0        0        0     3209 2022-03-25 10:55:23.381323 masci-tools-0.9.0a0/masci_tools/io/kkr_read_shapefun_info.py
--rw-r--r--   0        0        0     7318 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/modify_potential.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/__init__.py
--rw-r--r--   0        0        0     1203 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/__init__.py
--rw-r--r--   0        0        0    21984 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/default_parse_tasks.py
--rw-r--r--   0        0        0    11542 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/fleur_inpxml_parser.py
--rw-r--r--   0        0        0    17894 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/fleur_outxml_parser.py
--rw-r--r--   0        0        0      276 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/fleur_schema/__init__.py
--rw-r--r--   0        0        0    10789 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/outxml_conversions.py
--rw-r--r--   0        0        0     2470 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/task_migrations.py
--rw-r--r--   0        0        0    33493 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.27/FleurInputSchema.xsd
--rw-r--r--   0        0        0    42415 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.28/FleurInputSchema.xsd
--rw-r--r--   0        0        0    47113 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.29/FleurInputSchema.xsd
--rw-r--r--   0        0        0    27264 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.29/FleurOutputSchema.xsd
--rw-r--r--   0        0        0    47945 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.30/FleurInputSchema.xsd
--rw-r--r--   0        0        0    27264 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.30/FleurOutputSchema.xsd
--rw-r--r--   0        0        0    48072 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.31/FleurInputSchema.xsd
--rw-r--r--   0        0        0    27264 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.31/FleurOutputSchema.xsd
--rw-r--r--   0        0        0    58368 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.32/FleurInputSchema.xsd
--rw-r--r--   0        0        0    59060 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.33/FleurInputSchema.xsd
--rw-r--r--   0        0        0    30973 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.33/FleurOutputSchema.xsd
--rw-r--r--   0        0        0    59653 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.34/FleurInputSchema.xsd
--rwxr-xr-x   0        0        0    31737 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.34/FleurOutputSchema.xsd
--rw-r--r--   0        0        0    59415 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.35/FleurInputSchema.xsd
--rw-r--r--   0        0        0    37578 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.35/FleurOutputSchema.xsd
--rw-r--r--   0        0        0     1417 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/__init__.py
--rw-r--r--   0        0        0    54308 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/fleur_schema_parser_functions.py
--rw-r--r--   0        0        0    13216 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/inpschema_todict.py
--rw-r--r--   0        0        0    12047 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/outschema_todict.py
--rw-r--r--   0        0        0    51789 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/schema_dict.py
--rw-r--r--   0        0        0      286 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/__init__.py
--rw-r--r--   0        0        0    11457 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/reader.py
--rw-r--r--   0        0        0    15084 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/recipes.py
--rw-r--r--   0        0        0    27416 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/transforms.py
--rw-r--r--   0        0        0    25156 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/kkrimp_parser_functions.py
--rw-r--r--   0        0        0    36179 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/kkrparser_functions.py
--rw-r--r--   0        0        0     1430 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/__init__.py
--rw-r--r--   0        0        0    10855 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/recipes.py
--rw-r--r--   0        0        0     6083 2022-03-25 10:55:23.385323 masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/tabulator.py
--rw-r--r--   0        0        0     6365 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/transformers.py
--rw-r--r--   0        0        0    13529 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/io/parsers/voroparser_functions.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/testing/__init__.py
--rw-r--r--   0        0        0     7216 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/testing/bokeh.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/__init__.py
--rw-r--r--   0        0        0    97586 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/banddos_analysis_1.mlapp
--rw-r--r--   0        0        0   249802 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/banddos_analysis_1.mlappinstall
--rw-r--r--   0        0        0     2937 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/banddos_analysis_1.prj
--rw-r--r--   0        0        0    39947 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/cf_calculation.py
--rw-r--r--   0        0        0     6998 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_031_033.json
--rw-r--r--   0        0        0     6998 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_031_to_034.json
--rw-r--r--   0        0        0     7218 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_033_to_031.json
--rw-r--r--   0        0        0      316 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_033_to_034.json
--rw-r--r--   0        0        0    43064 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/fleur_inpxml_converter.py
--rw-r--r--   0        0        0     4665 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/greensf_calculations.py
--rw-r--r--   0        0        0     1834 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/greensf_visualization.py
--rw-r--r--   0        0        0    41027 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/greensfunction.py
--rw-r--r--   0        0        0    41894 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/matlabfrag.m
--rw-r--r--   0        0        0     4071 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/mlf2pdf.m
--rw-r--r--   0        0        0     5829 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/molecule3D.m
--rw-r--r--   0        0        0     2819 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/plotting.m
--rw-r--r--   0        0        0     3249 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/saving_pdf.m
--rw-r--r--   0        0        0     2137 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/tools/saving_txt.m
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/__init__.py
--rw-r--r--   0        0        0     9840 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/case_insensitive_dict.py
--rw-r--r--   0        0        0    69616 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/chemical_elements.py
--rw-r--r--   0        0        0    37717 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/constants.py
--rw-r--r--   0        0        0     4347 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/econfig.py
--rw-r--r--   0        0        0    10384 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/fleur_calculate_expression.py
--rwxr-xr-x   0        0        0    13334 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/kkr_rms_tracker.py
--rw-r--r--   0        0        0     9622 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/lockable_containers.py
--rw-r--r--   0        0        0     2962 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/logging_util.py
--rw-r--r--   0        0        0     3726 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/math_util.py
--rwxr-xr-x   0        0        0    16716 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/modifypotential.py
--rw-r--r--   0        0        0    21505 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/parse_tasks.py
--rw-r--r--   0        0        0     5475 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/parse_tasks_decorators.py
--rw-r--r--   0        0        0      276 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/parse_utils.py
--rwxr-xr-x   0        0        0     1788 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/plot_shapfun.py
--rw-r--r--   0        0        0    17928 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/python_util.py
--rw-r--r--   0        0        0    56663 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/schema_dict_util.py
--rw-r--r--   0        0        0     1134 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/typing.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/xml/__init__.py
--rw-r--r--   0        0        0     2754 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/xml/collect_xml_setters.py
--rw-r--r--   0        0        0    17722 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/xml/common_functions.py
--rw-r--r--   0        0        0    23598 2022-03-25 10:55:23.389323 masci-tools-0.9.0a0/masci_tools/util/xml/converters.py
--rw-r--r--   0        0        0    58048 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/util/xml/xml_getters.py
--rw-r--r--   0        0        0    16961 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_basic.py
--rw-r--r--   0        0        0    67992 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_names.py
--rw-r--r--   0        0        0    15412 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_nmmpmat.py
--rw-r--r--   0        0        0    33138 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_xpaths.py
--rw-r--r--   0        0        0    16757 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/util/xml/xpathbuilder.py
--rw-r--r--   0        0        0        0 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/__init__.py
--rw-r--r--   0        0        0    84719 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/bokeh_plots.py
--rw-r--r--   0        0        0    23044 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/bokeh_plotter.py
--rw-r--r--   0        0        0    17599 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/common.py
--rw-r--r--   0        0        0    35201 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/data.py
--rw-r--r--   0        0        0    26839 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/fleur.py
--rw-r--r--   0        0        0     4081 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_FS_qdos.py
--rw-r--r--   0        0        0     8765 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_bandstruc_qdos.py
--rw-r--r--   0        0        0    14449 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_dos.py
--rw-r--r--   0        0        0     3582 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_shapefun.py
--rw-r--r--   0        0        0    27097 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/matplotlib_plotter.py
--rw-r--r--   0        0        0    31957 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/parameters.py
--rw-r--r--   0        0        0   129659 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/masci_tools/vis/plot_methods.py
--rw-r--r--   0        0        0     1589 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/open_source_licenses.txt
--rw-r--r--   0        0        0     4844 2022-03-25 10:55:23.393323 masci-tools-0.9.0a0/pyproject.toml
--rw-r--r--   0        0        0     5585 1970-01-01 00:00:00.000000 masci-tools-0.9.0a0/PKG-INFO
+-rw-r--r--   0        0        0     3769 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     3130 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1898 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.github/workflows/fleur-release.yml
+-rw-r--r--   0        0        0     2838 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.gitignore
+-rw-r--r--   0        0        0     2854 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0     4853 2022-04-05 08:04:25.832226 masci-tools-0.9.1/.zenodo.json
+-rw-r--r--   0        0        0      298 2022-04-05 08:04:25.832226 masci-tools-0.9.1/AUTHORS.txt
+-rw-r--r--   0        0        0    27203 2022-04-05 08:04:25.832226 masci-tools-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1267 2022-04-05 08:04:25.832226 masci-tools-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     2925 2022-04-05 08:04:25.832226 masci-tools-0.9.1/README.md
+-rw-r--r--   0        0        0      354 2022-04-05 08:04:25.832226 masci-tools-0.9.1/codecov.yml
+-rw-r--r--   0        0        0     5612 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      187 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/source/_static/theme_overrides.css
+-rw-r--r--   0        0        0    13394 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/source/conf.py
+-rw-r--r--   0        0        0     6806 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/source/devel_guide/fleur_parser.rst
+-rw-r--r--   0        0        0      156 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/source/devel_guide/index.rst
+-rw-r--r--   0        0        0     6408 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/source/devel_guide/plot_data.rst
+-rw-r--r--   0        0        0    19222 2022-04-05 08:04:25.832226 masci-tools-0.9.1/docs/source/devel_guide/plotting.rst
+-rw-r--r--   0        0        0   372758 2022-04-05 08:04:25.836226 masci-tools-0.9.1/docs/source/images/bandstructure_simple_non_spinpol.png
+-rw-r--r--   0        0        0   581631 2022-04-05 08:04:25.840226 masci-tools-0.9.1/docs/source/images/bandstructure_simple_spinpol.png
+-rw-r--r--   0        0        0   602284 2022-04-05 08:04:25.840226 masci-tools-0.9.1/docs/source/images/bandstructure_weighted_non_spinpol.png
+-rw-r--r--   0        0        0   961340 2022-04-05 08:04:25.848226 masci-tools-0.9.1/docs/source/images/bandstructure_weighted_spinpol.png
+-rw-r--r--   0        0        0   491343 2022-04-05 08:04:25.852226 masci-tools-0.9.1/docs/source/images/dos_non_spinpol_multiplied.png
+-rw-r--r--   0        0        0   541938 2022-04-05 08:04:25.856226 masci-tools-0.9.1/docs/source/images/dos_non_spinpol_selection.png
+-rw-r--r--   0        0        0   470378 2022-04-05 08:04:25.856226 masci-tools-0.9.1/docs/source/images/dos_non_spinpol_standard.png
+-rw-r--r--   0        0        0   474437 2022-04-05 08:04:25.860226 masci-tools-0.9.1/docs/source/images/dos_spinpol_selection.png
+-rw-r--r--   0        0        0   458299 2022-04-05 08:04:25.864226 masci-tools-0.9.1/docs/source/images/dos_spinpol_standard.png
+-rw-r--r--   0        0        0   268777 2022-04-05 08:04:25.864226 masci-tools-0.9.1/docs/source/images/scatter_multi.png
+-rw-r--r--   0        0        0   245355 2022-04-05 08:04:25.864226 masci-tools-0.9.1/docs/source/images/scatter_multi_global_params.png
+-rw-r--r--   0        0        0   247105 2022-04-05 08:04:25.868226 masci-tools-0.9.1/docs/source/images/scatter_multi_specific_params.png
+-rw-r--r--   0        0        0   165633 2022-04-05 08:04:25.868226 masci-tools-0.9.1/docs/source/images/scatterplot_defaults.png
+-rw-r--r--   0        0        0   194101 2022-04-05 08:04:25.868226 masci-tools-0.9.1/docs/source/images/scatterplot_labels.png
+-rw-r--r--   0        0        0   173314 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/images/scatterplot_limits.png
+-rw-r--r--   0        0        0   162022 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/images/scatterplot_params.png
+-rw-r--r--   0        0        0   171655 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/images/scatterplot_scale.png
+-rw-r--r--   0        0        0   170193 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/images/scatterplot_standard.png
+-rw-r--r--   0        0        0     2201 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/index.rst
+-rw-r--r--   0        0        0     3110 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/module_guide/code.rst
+-rw-r--r--   0        0        0      135 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/module_guide/mg_index.rst
+-rw-r--r--   0        0        0     2009 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/module_guide/tools.rst
+-rw-r--r--   0        0        0       79 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/reference/_changelog.md
+-rw-r--r--   0        0        0       71 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/reference/index.rst
+-rw-r--r--   0        0        0     9368 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/user_guide/fleur_parser.rst
+-rw-r--r--   0        0        0     9785 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/user_guide/fleur_plots.rst
+-rw-r--r--   0        0        0    10210 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/user_guide/fleurxmlmodifier.rst
+-rw-r--r--   0        0        0     9511 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/user_guide/hdf5_parser.rst
+-rw-r--r--   0        0        0      175 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0    14842 2022-04-05 08:04:25.872226 masci-tools-0.9.1/docs/source/user_guide/plotting.rst
+-rw-r--r--   0        0        0     1505 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/__init__.py
+-rw-r--r--   0        0        0      109 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/commands/__init__.py
+-rw-r--r--   0        0        0     9339 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/commands/fleur_schema.py
+-rw-r--r--   0        0        0    11028 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/commands/parse.py
+-rw-r--r--   0        0        0     3061 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/commands/plot.py
+-rw-r--r--   0        0        0      566 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/commands/root.py
+-rw-r--r--   0        0        0      219 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/commands/tools.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.872226 masci-tools-0.9.1/masci_tools/cmdline/parameters/__init__.py
+-rw-r--r--   0        0        0     1769 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/cmdline/parameters/slice.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/cmdline/utils/__init__.py
+-rw-r--r--   0        0        0     9387 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/cmdline/utils/echo.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/__init__.py
+-rw-r--r--   0        0        0     1919 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/cif2inp_ase.py
+-rw-r--r--   0        0        0    24342 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/common_functions.py
+-rw-r--r--   0        0        0    27518 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/fleur_inpgen.py
+-rw-r--r--   0        0        0    53247 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/fleurxmlmodifier.py
+-rw-r--r--   0        0        0     4415 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/hdf5_util.py
+-rw-r--r--   0        0        0     9707 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/io_fleurxml.py
+-rw-r--r--   0        0        0     8227 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/io_nmmpmat.py
+-rw-r--r--   0        0        0   101099 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/kkr_params.py
+-rw-r--r--   0        0        0     3209 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/kkr_read_shapefun_info.py
+-rw-r--r--   0        0        0     7318 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/modify_potential.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/__init__.py
+-rw-r--r--   0        0        0     1203 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/__init__.py
+-rw-r--r--   0        0        0    21984 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/default_parse_tasks.py
+-rw-r--r--   0        0        0    11542 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/fleur_inpxml_parser.py
+-rw-r--r--   0        0        0    17894 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/fleur_outxml_parser.py
+-rw-r--r--   0        0        0      276 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/fleur_schema/__init__.py
+-rw-r--r--   0        0        0    10789 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/outxml_conversions.py
+-rw-r--r--   0        0        0     2470 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur/task_migrations.py
+-rw-r--r--   0        0        0    33493 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.27/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    42415 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.28/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    47113 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.29/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    27264 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.29/FleurOutputSchema.xsd
+-rw-r--r--   0        0        0    47945 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.30/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    27264 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.30/FleurOutputSchema.xsd
+-rw-r--r--   0        0        0    48072 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.31/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    27264 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.31/FleurOutputSchema.xsd
+-rw-r--r--   0        0        0    58368 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.32/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    59060 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.33/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    30973 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.33/FleurOutputSchema.xsd
+-rw-r--r--   0        0        0    59653 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.34/FleurInputSchema.xsd
+-rwxr-xr-x   0        0        0    31737 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.34/FleurOutputSchema.xsd
+-rw-r--r--   0        0        0    59415 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.35/FleurInputSchema.xsd
+-rw-r--r--   0        0        0    37578 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.35/FleurOutputSchema.xsd
+-rw-r--r--   0        0        0     1417 2022-04-05 08:04:25.876226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/__init__.py
+-rw-r--r--   0        0        0    55854 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/fleur_schema_parser_functions.py
+-rw-r--r--   0        0        0    13216 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/inpschema_todict.py
+-rw-r--r--   0        0        0    12047 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/outschema_todict.py
+-rw-r--r--   0        0        0    51789 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/schema_dict.py
+-rw-r--r--   0        0        0      286 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/hdf5/__init__.py
+-rw-r--r--   0        0        0    11504 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/hdf5/reader.py
+-rw-r--r--   0        0        0    15084 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/hdf5/recipes.py
+-rw-r--r--   0        0        0    27416 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/hdf5/transforms.py
+-rw-r--r--   0        0        0    25156 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/kkrimp_parser_functions.py
+-rw-r--r--   0        0        0    36179 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/kkrparser_functions.py
+-rw-r--r--   0        0        0     1430 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/tabulator/__init__.py
+-rw-r--r--   0        0        0    10855 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/tabulator/recipes.py
+-rw-r--r--   0        0        0     6083 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/tabulator/tabulator.py
+-rw-r--r--   0        0        0     6365 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/tabulator/transformers.py
+-rw-r--r--   0        0        0    13529 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/io/parsers/voroparser_functions.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/testing/__init__.py
+-rw-r--r--   0        0        0     7227 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/testing/bokeh.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/__init__.py
+-rw-r--r--   0        0        0    97586 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/banddos_analysis_1.mlapp
+-rw-r--r--   0        0        0   249802 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/banddos_analysis_1.mlappinstall
+-rw-r--r--   0        0        0     2937 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/banddos_analysis_1.prj
+-rw-r--r--   0        0        0    39999 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/cf_calculation.py
+-rw-r--r--   0        0        0     6998 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/conversions/conversion_031_033.json
+-rw-r--r--   0        0        0     6998 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/conversions/conversion_031_to_034.json
+-rw-r--r--   0        0        0     7218 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/conversions/conversion_033_to_031.json
+-rw-r--r--   0        0        0      316 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/conversions/conversion_033_to_034.json
+-rw-r--r--   0        0        0    43667 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/fleur_inpxml_converter.py
+-rw-r--r--   0        0        0     4665 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/greensf_calculations.py
+-rw-r--r--   0        0        0     1834 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/greensf_visualization.py
+-rw-r--r--   0        0        0    41027 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/greensfunction.py
+-rw-r--r--   0        0        0    41894 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/matlabfrag.m
+-rw-r--r--   0        0        0     4071 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/mlf2pdf.m
+-rw-r--r--   0        0        0     5829 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/molecule3D.m
+-rw-r--r--   0        0        0     2819 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/plotting.m
+-rw-r--r--   0        0        0     3249 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/saving_pdf.m
+-rw-r--r--   0        0        0     2137 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/tools/saving_txt.m
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/util/__init__.py
+-rw-r--r--   0        0        0     9840 2022-04-05 08:04:25.880226 masci-tools-0.9.1/masci_tools/util/case_insensitive_dict.py
+-rw-r--r--   0        0        0    69616 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/chemical_elements.py
+-rw-r--r--   0        0        0    37717 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/constants.py
+-rw-r--r--   0        0        0     4347 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/econfig.py
+-rw-r--r--   0        0        0    10384 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/fleur_calculate_expression.py
+-rwxr-xr-x   0        0        0    13334 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/kkr_rms_tracker.py
+-rw-r--r--   0        0        0     9622 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/lockable_containers.py
+-rw-r--r--   0        0        0     2962 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/logging_util.py
+-rw-r--r--   0        0        0     3726 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/math_util.py
+-rwxr-xr-x   0        0        0    16716 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/modifypotential.py
+-rw-r--r--   0        0        0    21505 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/parse_tasks.py
+-rw-r--r--   0        0        0     5475 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/parse_tasks_decorators.py
+-rw-r--r--   0        0        0      276 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/parse_utils.py
+-rwxr-xr-x   0        0        0     1788 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/plot_shapfun.py
+-rw-r--r--   0        0        0    17928 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/python_util.py
+-rw-r--r--   0        0        0    56663 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/schema_dict_util.py
+-rw-r--r--   0        0        0     1137 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/typing.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/__init__.py
+-rw-r--r--   0        0        0     2754 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/collect_xml_setters.py
+-rw-r--r--   0        0        0    17703 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/common_functions.py
+-rw-r--r--   0        0        0    23529 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/converters.py
+-rw-r--r--   0        0        0    58048 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/xml_getters.py
+-rw-r--r--   0        0        0    16961 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/xml_setters_basic.py
+-rw-r--r--   0        0        0    67992 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/xml_setters_names.py
+-rw-r--r--   0        0        0    15412 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/xml_setters_nmmpmat.py
+-rw-r--r--   0        0        0    33138 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/xml_setters_xpaths.py
+-rw-r--r--   0        0        0    16757 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/util/xml/xpathbuilder.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/__init__.py
+-rw-r--r--   0        0        0    84719 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/bokeh_plots.py
+-rw-r--r--   0        0        0    23044 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/bokeh_plotter.py
+-rw-r--r--   0        0        0    17599 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/common.py
+-rw-r--r--   0        0        0    35201 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/data.py
+-rw-r--r--   0        0        0    26839 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/fleur.py
+-rw-r--r--   0        0        0     4081 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/kkr_plot_FS_qdos.py
+-rw-r--r--   0        0        0     8765 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/kkr_plot_bandstruc_qdos.py
+-rw-r--r--   0        0        0    14449 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/kkr_plot_dos.py
+-rw-r--r--   0        0        0     3582 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/kkr_plot_shapefun.py
+-rw-r--r--   0        0        0    27097 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/matplotlib_plotter.py
+-rw-r--r--   0        0        0    31957 2022-04-05 08:04:25.884226 masci-tools-0.9.1/masci_tools/vis/parameters.py
+-rw-r--r--   0        0        0   129659 2022-04-05 08:04:25.888226 masci-tools-0.9.1/masci_tools/vis/plot_methods.py
+-rw-r--r--   0        0        0     1589 2022-04-05 08:04:25.888226 masci-tools-0.9.1/open_source_licenses.txt
+-rw-r--r--   0        0        0     4838 2022-04-05 08:04:25.888226 masci-tools-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5583 1970-01-01 00:00:00.000000 masci-tools-0.9.1/PKG-INFO
```

### Comparing `masci-tools-0.9.0a0/.github/workflows/cd.yml` & `masci-tools-0.9.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/.github/workflows/ci.yml` & `masci-tools-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/.github/workflows/fleur-release.yml` & `masci-tools-0.9.1/.github/workflows/fleur-release.yml`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/.gitignore` & `masci-tools-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/.pre-commit-config.yaml` & `masci-tools-0.9.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   -   id: flynt
       args: [
           '--line-length=120',
           '--fail-on-change',
       ]
 
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v2.31.1
     hooks:
     -   id: pyupgrade
         args: [
             '--py37-plus'
         ]
 
 - repo: local
```

### Comparing `masci-tools-0.9.0a0/.zenodo.json` & `masci-tools-0.9.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/CHANGELOG.md` & `masci-tools-0.9.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
-## latest
-[full changelog](https://github.com/JuDFTteam/masci-tools/compare/v0.8.0...develop)
+## v.0.9.1
+[full changelog](https://github.com/JuDFTteam/masci-tools/compare/v0.9.0...v0.9.1)
+
+### Added
+- Standalone function `masci_tools.tools.fleur_inpxml_converter.convert_inpxml` to allow conversions of `inp.xml` files within a python runtime without needing to go via the commandline
+
+### Bugfixes
+- Fixed bug in bokeh testing fixtures using the wrong folder for fallback versions
+- Fixed bug not correctly converting complex numbers from the Fleur xml files if they have whitespace at beginning/end
+
+## v.0.9.0
+[full changelog](https://github.com/JuDFTteam/masci-tools/compare/v0.8.0...v0.9.0)
 
 ### Added
 - New `bokeh` plot routine for matrix plot of rectangle patches with added texts [[#124]](https://github.com/JuDFTteam/masci-tools/pull/124)
 - Added TS contribution to free energy to output of `outxml_parser`
 
 ### Improvements
 - Several arguments in XML setter functions were renamed for more consistent signatures.
@@ -23,14 +33,15 @@
 - `io_nmmpmat`: Allow negative indices in `read_nmmpmat_block` and raise error for invalid index
 ### Bugfixes
 - Fix for signatures of `set_text`/`set_first_text`. These contained names of attribute setting functions [[#118]](https://github.com/JuDFTteam/masci-tools/pull/118)
 - Fix for validating arguments in `FleurXMLModifier` not accepting an argument named `name` when passed by keyword. [[#118]](https://github.com/JuDFTteam/masci-tools/pull/118)
 - Fixed problems in `masci_tools.testing.bokeh` when adding files for new bokeh versions [[#122]](https://github.com/JuDFTteam/masci-tools/pull/122)
 - Several fixes for `plot_fleur_dos`. Using the `area_plot` or specifying `color` explicitely could mess up the color order [[#132]](https://github.com/JuDFTteam/masci-tools/pull/132)
 - Fixed bug in `validate_nmmpmat` and consequently `FleurXMLModifier` not correctly validating denisty matrix files with certain off-diagonal elements being negative [[#135]](https://github.com/JuDFTteam/masci-tools/pull/135)
+- Fix for `HDF5Reader` for compatibility for file handles in `aiida-core` 2.0. The file handles coming from the file repository have no directly attached extension so the check if the file is a hdf file cannot be performed
 
 ### For developers
 - Fixed upload of pytest-mpl results artifacts to include the whole directory with images and not just the HTML file [[#117]](https://github.com/JuDFTteam/masci-tools/pull/117)
 - Updated typing to newer version of `lxml-stubs` (`0.4.0`) [[#123]](https://github.com/JuDFTteam/masci-tools/pull/123)
 
 ## v.0.8.0
 [full changelog](https://github.com/JuDFTteam/masci-tools/compare/v0.7.2...v0.8.0)
```

### Comparing `masci-tools-0.9.0a0/LICENSE.txt` & `masci-tools-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/README.md` & `masci-tools-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/Makefile` & `masci-tools-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/conf.py` & `masci-tools-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/devel_guide/fleur_parser.rst` & `masci-tools-0.9.1/docs/source/devel_guide/fleur_parser.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/devel_guide/plot_data.rst` & `masci-tools-0.9.1/docs/source/devel_guide/plot_data.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/devel_guide/plotting.rst` & `masci-tools-0.9.1/docs/source/devel_guide/plotting.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/bandstructure_simple_non_spinpol.png` & `masci-tools-0.9.1/docs/source/images/bandstructure_simple_non_spinpol.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/bandstructure_simple_spinpol.png` & `masci-tools-0.9.1/docs/source/images/bandstructure_simple_spinpol.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/bandstructure_weighted_non_spinpol.png` & `masci-tools-0.9.1/docs/source/images/bandstructure_weighted_non_spinpol.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/bandstructure_weighted_spinpol.png` & `masci-tools-0.9.1/docs/source/images/bandstructure_weighted_spinpol.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/dos_non_spinpol_multiplied.png` & `masci-tools-0.9.1/docs/source/images/dos_non_spinpol_multiplied.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/dos_non_spinpol_selection.png` & `masci-tools-0.9.1/docs/source/images/dos_non_spinpol_selection.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/dos_non_spinpol_standard.png` & `masci-tools-0.9.1/docs/source/images/dos_non_spinpol_standard.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/dos_spinpol_selection.png` & `masci-tools-0.9.1/docs/source/images/dos_spinpol_selection.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/dos_spinpol_standard.png` & `masci-tools-0.9.1/docs/source/images/dos_spinpol_standard.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatter_multi.png` & `masci-tools-0.9.1/docs/source/images/scatter_multi.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatter_multi_global_params.png` & `masci-tools-0.9.1/docs/source/images/scatter_multi_global_params.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatter_multi_specific_params.png` & `masci-tools-0.9.1/docs/source/images/scatter_multi_specific_params.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatterplot_defaults.png` & `masci-tools-0.9.1/docs/source/images/scatterplot_defaults.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatterplot_labels.png` & `masci-tools-0.9.1/docs/source/images/scatterplot_labels.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatterplot_limits.png` & `masci-tools-0.9.1/docs/source/images/scatterplot_limits.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatterplot_params.png` & `masci-tools-0.9.1/docs/source/images/scatterplot_params.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatterplot_scale.png` & `masci-tools-0.9.1/docs/source/images/scatterplot_scale.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/images/scatterplot_standard.png` & `masci-tools-0.9.1/docs/source/images/scatterplot_standard.png`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/index.rst` & `masci-tools-0.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/module_guide/code.rst` & `masci-tools-0.9.1/docs/source/module_guide/code.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/module_guide/tools.rst` & `masci-tools-0.9.1/docs/source/module_guide/tools.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/user_guide/fleur_parser.rst` & `masci-tools-0.9.1/docs/source/user_guide/fleur_parser.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/user_guide/fleur_plots.rst` & `masci-tools-0.9.1/docs/source/user_guide/fleur_plots.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/user_guide/fleurxmlmodifier.rst` & `masci-tools-0.9.1/docs/source/user_guide/fleurxmlmodifier.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/user_guide/hdf5_parser.rst` & `masci-tools-0.9.1/docs/source/user_guide/hdf5_parser.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/docs/source/user_guide/plotting.rst` & `masci-tools-0.9.1/docs/source/user_guide/plotting.rst`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/__init__.py` & `masci-tools-0.9.1/masci_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 Plus wrappers of visualisation for aiida-fleur workflow nodes
 """
 import logging
 
 __copyright__ = ('Copyright (c), Forschungszentrum Jülich GmbH, IAS-1/PGI-1, Germany. '
                  'All rights reserved.')
 __license__ = 'MIT license, see LICENSE.txt file.'
-__version__ = '0.9.0alpha0'
+__version__ = '0.9.1'
 __authors__ = 'The JuDFT team. Also see AUTHORS.txt file.'
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `masci-tools-0.9.0a0/masci_tools/cmdline/commands/fleur_schema.py` & `masci-tools-0.9.1/masci_tools/cmdline/commands/fleur_schema.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/cmdline/commands/parse.py` & `masci-tools-0.9.1/masci_tools/cmdline/commands/parse.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/cmdline/commands/plot.py` & `masci-tools-0.9.1/masci_tools/cmdline/commands/plot.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/cmdline/commands/root.py` & `masci-tools-0.9.1/masci_tools/cmdline/commands/root.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/cmdline/parameters/slice.py` & `masci-tools-0.9.1/masci_tools/cmdline/parameters/slice.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/cmdline/utils/echo.py` & `masci-tools-0.9.1/masci_tools/cmdline/utils/echo.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/cif2inp_ase.py` & `masci-tools-0.9.1/masci_tools/io/cif2inp_ase.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/common_functions.py` & `masci-tools-0.9.1/masci_tools/io/common_functions.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/fleur_inpgen.py` & `masci-tools-0.9.1/masci_tools/io/fleur_inpgen.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/fleurxmlmodifier.py` & `masci-tools-0.9.1/masci_tools/io/fleurxmlmodifier.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/hdf5_util.py` & `masci-tools-0.9.1/masci_tools/io/hdf5_util.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/io_fleurxml.py` & `masci-tools-0.9.1/masci_tools/io/io_fleurxml.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/io_nmmpmat.py` & `masci-tools-0.9.1/masci_tools/io/io_nmmpmat.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/kkr_params.py` & `masci-tools-0.9.1/masci_tools/io/kkr_params.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/kkr_read_shapefun_info.py` & `masci-tools-0.9.1/masci_tools/io/kkr_read_shapefun_info.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/modify_potential.py` & `masci-tools-0.9.1/masci_tools/io/modify_potential.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/__init__.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur/__init__.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/default_parse_tasks.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur/default_parse_tasks.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/fleur_inpxml_parser.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur/fleur_inpxml_parser.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/fleur_outxml_parser.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur/fleur_outxml_parser.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/outxml_conversions.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur/outxml_conversions.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur/task_migrations.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur/task_migrations.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.27/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.27/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.28/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.28/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.29/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.29/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.29/FleurOutputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.29/FleurOutputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.30/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.30/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.30/FleurOutputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.30/FleurOutputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.31/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.31/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.31/FleurOutputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.31/FleurOutputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.32/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.32/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.33/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.33/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.33/FleurOutputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.33/FleurOutputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.34/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.34/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.34/FleurOutputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.34/FleurOutputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.35/FleurInputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.35/FleurInputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/0.35/FleurOutputSchema.xsd` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/0.35/FleurOutputSchema.xsd`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/__init__.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/fleur_schema_parser_functions.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/fleur_schema_parser_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,46 +10,54 @@
 #                                                                             #
 ###############################################################################
 """
 functions to extract information about the fleur schema input or output
 """
 from __future__ import annotations
 
+import sys
 from masci_tools.util.case_insensitive_dict import CaseInsensitiveDict, CaseInsensitiveFrozenSet
 from functools import wraps
-from typing import Callable, NamedTuple, Any
+from typing import Callable, NamedTuple, Any, overload
 from lxml import etree
 try:
     from typing import Literal, TypedDict
 except ImportError:
     from typing_extensions import Literal, TypedDict  #type: ignore[misc]
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    from typing_extensions import TypeAlias
 import warnings
 import math
 
 #These types have infinite recursive paths and CANNOT BE PARSED in the path generation
 _RECURSIVE_TYPES = ['CompositeTimerType']
 #Name of the type of an scf iteration in the out schema (At this point the paths are split up)
 _ITERATION_TYPE = 'IterationType'
 _ITERATION_GROUP_TYPE = 'GeneralIterationType'
 _INPUT_TYPE = 'FleurInputType'
 
 # The types defined here should not be reduced further and are associated with one clear base type
 # AngularMomentumNumberType and MainQuantumNumberType are here because they are integers
 # but are implemented as xsd:string with a regex
-BASE_TYPES = {
+BaseType: TypeAlias = Literal['int', 'switch', 'string', 'float', 'float_expression', 'complex']
+
+BASE_TYPES: dict[BaseType, set[str]] = {
     'switch': {'FleurBool'},
     'int': {
         'xsd:nonNegativeInteger', 'xsd:positiveInteger', 'xsd:integer', 'AngularMomentumNumberType',
         'MainQuantumNumberType'
     },
     'float': {'xsd:double'},
     'float_expression': {'FleurDouble'},
     'string': {'xsd:string'},
     'complex': {'FortranComplex'}
 }
+
 NAMESPACES = {'xsd': 'http://www.w3.org/2001/XMLSchema'}
 
 
 def convert_str_version_number(version_str: str) -> tuple[int, int]:
     """
     Convert the version number as a integer for easy comparisons
 
@@ -62,20 +70,25 @@
 
     if len(version_numbers) != 2:
         raise ValueError(f"Version number is malformed: '{version_str}'")
 
     return tuple(int(part) for part in version_numbers)  #type: ignore[return-value]
 
 
-class AttributeType(NamedTuple):
-    """Type for describing the types of attributes/text"""
+class _XSDAttributeType(NamedTuple):
+    """Type for describing the types of attributes/text. Can contain unfinished conversions"""
     base_type: str
     length: int | Literal['unbounded'] | None
 
 
+class AttributeType(_XSDAttributeType):
+    """Type for describing the types of attributes/text"""
+    base_type: Literal['int', 'switch', 'string', 'float', 'float_expression', 'complex']
+
+
 class TagInfo(TypedDict):
     """Dict representing the entries for the tag information.
     """
     attribs: CaseInsensitiveFrozenSet[str]
     optional_attribs: CaseInsensitiveDict[str, str]
     optional: CaseInsensitiveFrozenSet[str]
     several: CaseInsensitiveFrozenSet[str]
@@ -243,18 +256,40 @@
         if stop_non_unique:
             if 'maxOccurs' in parent.attrib:
                 if parent.attrib['maxOccurs'] != '1':
                     return None, None
     return parent, parent_type
 
 
-def _get_base_types(xmlschema_evaluator: etree.XPathDocumentEvaluator,
-                    type_elem: etree._Element,
-                    convert_to_base: bool = True,
-                    basic_types_mapping: dict[str, list[AttributeType]] | None = None) -> list[AttributeType]:
+@overload
+def _get_base_types(xmlschema_evaluator: etree.XPathDocumentEvaluator, type_elem: etree._Element,
+                    basic_types_mapping: dict[str, list[AttributeType]] | None,
+                    convert_to_base: Literal[True]) -> list[AttributeType]:
+    ...
+
+
+@overload
+def _get_base_types(xmlschema_evaluator: etree.XPathDocumentEvaluator, type_elem: etree._Element,
+                    basic_types_mapping: dict[str, list[AttributeType]] | None,
+                    convert_to_base: Literal[False]) -> list[_XSDAttributeType]:
+    ...
+
+
+@overload
+def _get_base_types(xmlschema_evaluator: etree.XPathDocumentEvaluator, type_elem: etree._Element,
+                    basic_types_mapping: dict[str, list[AttributeType]] | None) -> list[AttributeType]:
+    ...
+
+
+def _get_base_types(
+    xmlschema_evaluator: etree.XPathDocumentEvaluator,
+    type_elem: etree._Element,
+    basic_types_mapping: dict[str, list[AttributeType]] | None = None,
+    convert_to_base: bool = True,
+) -> list[AttributeType] | list[_XSDAttributeType]:
     """
     Analyses the given type element to deduce its base_types and length restrictions
 
     :param xmlschema_evaluator: etree.XPathEvaluator for the schema
     :param type_elem: etree element of the type to analyse
     :param convert_to_base: if True all possible types are converted to their base_types using either base_types
                             or basic_types_mapping
@@ -265,15 +300,15 @@
     """
 
     if basic_types_mapping is None:
         basic_types_mapping = {}
 
     length = _get_length(xmlschema_evaluator, type_elem)
 
-    possible_types = set()
+    possible_types: set[_XSDAttributeType | AttributeType] = set()
     for child in type_elem:
         child_type = _normalized_name(child.tag)
 
         types = None
         if child_type in ('restriction', 'extension'):
             types = [str(child.attrib['base'])]
         elif child_type == 'list':
@@ -289,17 +324,17 @@
 
         #Reduce the found types to types that can be converted to base types
         if types is not None:
 
             for found_type in types:
 
                 if _is_base_type(found_type):
-                    possible_types.add(AttributeType(base_type=found_type, length=length))
+                    possible_types.add(_XSDAttributeType(base_type=found_type, length=length))
                 elif found_type in basic_types_mapping:
-                    possible_types.add(AttributeType(base_type=found_type, length=length))
+                    possible_types.add(_XSDAttributeType(base_type=found_type, length=length))
                 else:
                     sub_types = _xpath_eval(xmlschema_evaluator, '//xsd:simpleType[@name=$name]', name=found_type)
                     if len(sub_types) == 0:
                         sub_types = _xpath_eval(xmlschema_evaluator,
                                                 '//xsd:complexType[@name=$name]/xsd:simpleContent',
                                                 name=found_type)
 
@@ -312,15 +347,15 @@
                     new_types = _get_base_types(xmlschema_evaluator,
                                                 sub_types[0],
                                                 convert_to_base=False,
                                                 basic_types_mapping=basic_types_mapping)
 
                     if length != 1:
                         possible_types.update(
-                            AttributeType(base_type=base_type, length=length) for base_type, _ in new_types)
+                            _XSDAttributeType(base_type=base_type, length=length) for base_type, _ in new_types)
                     else:
                         possible_types.update(new_types)
 
     if convert_to_base:
         converted_types = set()
         for found_type, length in possible_types:
             if found_type in basic_types_mapping:
@@ -1198,48 +1233,53 @@
 
     text_tags = CaseInsensitiveFrozenSet(text_tag_list)
     assert len(set(text_tag_list)) == len(text_tags), f'Lost Information: {text_tag_list}'
 
     return text_tags
 
 
-def get_basic_types(xmlschema_evaluator: etree.XPathDocumentEvaluator, **kwargs: Any) -> dict[str, list[AttributeType]]:
+def get_basic_types(xmlschema_evaluator: etree.XPathDocumentEvaluator,
+                    input_basic_types: dict[str, list[AttributeType]] | None = None,
+                    **kwargs: Any) -> dict[str, list[AttributeType]]:
     """
     find all types, which can be traced back directly to a base_type
 
     :param xmlschema_evaluator: etree.XPathEvaluator for the schema
 
     :return: dictionary with type names and their corresponding type_definition
              meaning a dictionary with possible base types and evtl. length restriction
     """
-    basic_type_elems = _xpath_eval(xmlschema_evaluator, '//xsd:simpleType[@name]')
-    complex_type_elems = _xpath_eval(xmlschema_evaluator, '//xsd:complexType/xsd:simpleContent')
+    basic_type_elems: list[etree._Element] = _xpath_eval(xmlschema_evaluator, '//xsd:simpleType[@name]')
+    complex_type_elems: list[etree._Element] = _xpath_eval(xmlschema_evaluator, '//xsd:complexType/xsd:simpleContent')
 
     basic_types = {}
     for type_elem in basic_type_elems + complex_type_elems:
         if 'name' in type_elem.attrib:
-            type_name = type_elem.attrib['name']
+            type_name = str(type_elem.attrib['name'])
         else:
-            type_name = type_elem.getparent().attrib['name']
+            parent = type_elem.getparent()
+            if parent is None:
+                raise ValueError('Could not find parent')
+            type_name = str(parent.attrib['name'])
 
         if _is_base_type(type_name):
             continue  #Already a base type
 
-        types = _get_base_types(xmlschema_evaluator, type_elem, basic_types_mapping=kwargs.get('input_basic_types'))
+        types = _get_base_types(xmlschema_evaluator, type_elem, basic_types_mapping=input_basic_types)
 
         if type_name not in basic_types:
             basic_types[type_name] = types
         else:
             raise ValueError(f'Already defined type {type_name}')
 
     #Append the definitions form the inputschema since including it directly is very messy
-    if 'input_basic_types' in kwargs:
-        if any(key in basic_types for key in kwargs['input_basic_types']):
+    if input_basic_types is not None:
+        if any(key in basic_types for key in input_basic_types):
             raise ValueError('Doubled type definitions from Inputschema')
-        basic_types.update(kwargs['input_basic_types'])
+        basic_types.update(input_basic_types)
 
     return basic_types
 
 
 def get_tag_info(xmlschema_evaluator: etree.XPathDocumentEvaluator, **kwargs: Any) -> dict[str, TagInfo]:
     """
     Get all important information about the tags
```

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/inpschema_todict.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/inpschema_todict.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/outschema_todict.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/outschema_todict.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/fleur_schema/schema_dict.py` & `masci-tools-0.9.1/masci_tools/io/parsers/fleur_schema/schema_dict.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/reader.py` & `masci-tools-0.9.1/masci_tools/io/parsers/hdf5/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
         if isinstance(self._original_file, (io.IOBase, Path)):
             self.filename = self._original_file.name
         elif isinstance(self._original_file, bytes):
             self.filename = os.fsdecode(self._original_file)
         else:
             self.filename = cast(str, self._original_file)
 
-        if not self.filename.endswith('.hdf'):
+        extension = Path(self.filename).suffix
+
+        if extension and extension != '.hdf':
             logger.exception('Wrong File Type for %s: Got %s', self.__class__.__name__, self.filename)
             raise ValueError(f'Wrong File Type for {self.__class__.__name__}: Got {self.filename}')
 
         logger.info('Instantiated %s with file %s', self.__class__.__name__, self.filename)
 
         self._move_to_memory = move_to_memory
```

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/recipes.py` & `masci-tools-0.9.1/masci_tools/io/parsers/hdf5/recipes.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/hdf5/transforms.py` & `masci-tools-0.9.1/masci_tools/io/parsers/hdf5/transforms.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/kkrimp_parser_functions.py` & `masci-tools-0.9.1/masci_tools/io/parsers/kkrimp_parser_functions.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/kkrparser_functions.py` & `masci-tools-0.9.1/masci_tools/io/parsers/kkrparser_functions.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/__init__.py` & `masci-tools-0.9.1/masci_tools/io/parsers/tabulator/__init__.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/recipes.py` & `masci-tools-0.9.1/masci_tools/io/parsers/tabulator/recipes.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/tabulator.py` & `masci-tools-0.9.1/masci_tools/io/parsers/tabulator/tabulator.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/tabulator/transformers.py` & `masci-tools-0.9.1/masci_tools/io/parsers/tabulator/transformers.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/io/parsers/voroparser_functions.py` & `masci-tools-0.9.1/masci_tools/io/parsers/voroparser_functions.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/testing/bokeh.py` & `masci-tools-0.9.1/masci_tools/testing/bokeh.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 filename = basename.name
                 _, _, current_version = basename.parent.name.partition('-')
                 current_version = tuple(int(x) for x in current_version.split('.'))
                 prev_version = previous_bokeh_results(current_version)
 
                 if not pytestconfig.getoption('--add-bokeh-version'):
                     if prev_version is not None:
-                        basename = Path(prev_version) / filename
+                        basename = Path(f'bokeh-{prev_version}') / filename
                         warnings.warn(f'Results for bokeh version {basename.parent} not available.'
                                       f'Using the last available version {prev_version}'
                                       'Use the option --add-bokeh-version to add results for this version')
 
             from bokeh.io import curdoc
 
             curdoc().clear()
```

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/banddos_analysis_1.mlapp` & `masci-tools-0.9.1/masci_tools/tools/banddos_analysis_1.mlapp`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/banddos_analysis_1.mlappinstall` & `masci-tools-0.9.1/masci_tools/tools/banddos_analysis_1.mlappinstall`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/banddos_analysis_1.prj` & `masci-tools-0.9.1/masci_tools/tools/banddos_analysis_1.prj`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/cf_calculation.py` & `masci-tools-0.9.1/masci_tools/tools/cf_calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,18 @@
             warnings.warn('The argument only_m0 is deprecated.', DeprecationWarning)
             self.only_m0 = kwargs['only_m0']
         if 'quiet' in kwargs:
             warnings.warn('The argument quiet is deprecated.', DeprecationWarning)
 
     @property
     def denNorm(self):
-        """DEPRECATED: Use density_normalization instead"""
+        """Returns the density normalization
+
+        DEPRECATED: Use density_normalization instead
+        """
         return self.density_normalization
 
     def stevens_prefactor(self, l: int, m: int) -> float:
         """Gives the lm dependent prefactor for conversion between
         Blm and Alm coefficients
 
         Args:
```

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_031_033.json` & `masci-tools-0.9.1/masci_tools/tools/conversions/conversion_031_033.json`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_031_to_034.json` & `masci-tools-0.9.1/masci_tools/tools/conversions/conversion_031_to_034.json`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/conversions/conversion_033_to_031.json` & `masci-tools-0.9.1/masci_tools/tools/conversions/conversion_033_to_031.json`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/fleur_inpxml_converter.py` & `masci-tools-0.9.1/masci_tools/tools/fleur_inpxml_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -803,60 +803,32 @@
     else:
         order = []
 
     if order:
         parent = _reorder_tags(parent, order)
 
 
-@click.group('inpxml')
-def inpxml():
-    """
-    Tool for converting inp.xml files to different versions
+def convert_inpxml(xmltree: etree._ElementTree, schema_dict: InputSchemaDict, to_version: str) -> etree._ElementTree:
     """
+    Convert the given xmltree to the given file version
 
+    :param xmltree: XML tree to convert
+    :param schema_dict: SchemaDict corresponding to the original file version
+    :param to_version: file version to which to convert
 
-@inpxml.command('convert')
-@click.argument('xml-file', type=click.Path(exists=True))
-@click.argument('to_version', type=str)
-@click.option('--output-file', '-o', type=str, default='inp.xml', help='Name of the output file')
-@click.option('--overwrite', is_flag=True, help='If the flag is given and the file already exists it is overwritten')
-@click.pass_context
-def convert_inpxml(ctx: click.Context, xml_file: FileLike, to_version: str, output_file: str, overwrite: bool) -> None:
-    """
-    Convert the given XML_FILE file to version TO_VERSION
-
-    XML_FILE is the file to convert
-    TO_VERSION is the file version of the finale input file
+    :returns: the XML tree converted to the given file version
     """
-    INCLUDE_NSMAP = {'xi': 'http://www.w3.org/2001/XInclude'}
-    INCLUDE_TAG = etree.QName(INCLUDE_NSMAP['xi'], 'include')
-    FALLBACK_TAG = etree.QName(INCLUDE_NSMAP['xi'], 'fallback')
-
-    xmltree, schema_dict = load_inpxml(xml_file)
     schema_dict_target = InputSchemaDict.fromVersion(to_version)
 
     #We want to leave comments in so we cannot use clear_xml for the xinclude feature
     #Here we just include and write out the complete xml file
     xmltree.xinclude()
-
     from_version = evaluate_attribute(xmltree, schema_dict, 'fleurInputVersion')
 
-    try:
-        conversion = load_conversion(from_version, to_version)
-    except FileNotFoundError:
-        echo.echo_warning(f'No conversion available between versions {from_version} to {to_version}')
-        if click.confirm('Do you want to generate this conversion now'):
-            conversion = ctx.invoke(generate_inp_conversion, from_version=from_version, to_version=to_version)
-        else:
-            echo.echo_critical('Cannot convert')
-
-    if Path(output_file).is_file():
-        if not overwrite:
-            echo.echo_critical(f'The output file {output_file} already exists. Use the overwrite flag to ignore')
-        echo.echo_warning(f'The output file {output_file} already exists. Will be overwritten')
+    conversion = load_conversion(from_version, to_version)
 
     set_attrib_value(xmltree, schema_dict_target, 'fleurInputVersion', to_version)
 
     action: MoveAction | RemoveAction | CreateAction | NormalizedMoveAction
     #Collect the nodes to be moved
     move_tags: list[list[etree._Element]] = []
     for action in conversion['tag']['move']:
@@ -911,33 +883,77 @@
         if action.element is not None:
             nodes: list[etree._Element] = eval_xpath(xmltree, action.path, list_return=True)  #type: ignore
             if nodes:
                 xml_set_attrib_value_no_create(xmltree, action.path, action.name, action.element)
 
     _reorder_tree(xmltree.getroot(), schema_dict_target)
 
+    validate_xml(xmltree, schema_dict_target.xmlschema, error_header='Input file does not validate against the schema')
+
+    #If there was no relax.xml included we need to rewrite the xinclude tag for it
+    INCLUDE_NSMAP = {'xi': 'http://www.w3.org/2001/XInclude'}
+    INCLUDE_TAG = etree.QName(INCLUDE_NSMAP['xi'], 'include')
+    FALLBACK_TAG = etree.QName(INCLUDE_NSMAP['xi'], 'fallback')
+    if not tag_exists(xmltree, schema_dict_target, 'relaxation'):
+        xinclude_elem = etree.Element(INCLUDE_TAG, href='relax.xml', nsmap=INCLUDE_NSMAP)
+        xinclude_elem.append(etree.Element(FALLBACK_TAG))
+        xmltree.getroot().append(xinclude_elem)
+
+    etree.indent(xmltree)
+    return xmltree
+
+
+@click.group('inpxml')
+def inpxml():
+    """
+    Tool for converting inp.xml files to different versions
+    """
+
+
+@inpxml.command('convert')
+@click.argument('xml-file', type=click.Path(exists=True))
+@click.argument('to_version', type=str)
+@click.option('--output-file', '-o', type=str, default='inp.xml', help='Name of the output file')
+@click.option('--overwrite', is_flag=True, help='If the flag is given and the file already exists it is overwritten')
+@click.pass_context
+def cmd_convert_inpxml(ctx: click.Context, xml_file: FileLike, to_version: str, output_file: str,
+                       overwrite: bool) -> None:
+    """
+    Convert the given XML_FILE file to version TO_VERSION
+
+    XML_FILE is the file to convert
+    TO_VERSION is the file version of the finale input file
+    """
+    xmltree, schema_dict = load_inpxml(xml_file)
+    from_version = evaluate_attribute(xmltree, schema_dict, 'fleurInputVersion')
+
     try:
-        validate_xml(xmltree,
-                     schema_dict_target.xmlschema,
-                     error_header='Input file does not validate against the schema')
+        load_conversion(from_version, to_version)
+    except FileNotFoundError:
+        echo.echo_warning(f'No conversion available between versions {from_version} to {to_version}')
+        if click.confirm('Do you want to generate this conversion now'):
+            ctx.invoke(generate_inp_conversion, from_version=from_version, to_version=to_version)
+        else:
+            echo.echo_critical('Cannot convert')
+
+    if Path(output_file).is_file():
+        if not overwrite:
+            echo.echo_critical(f'The output file {output_file} already exists. Use the overwrite flag to ignore')
+        echo.echo_warning(f'The output file {output_file} already exists. Will be overwritten')
+
+    try:
+        convert_inpxml(xmltree, schema_dict, to_version)
         echo.echo_success('The conversion was successful')
         echo.echo_info(
             'It is not guaranteed that a FLEUR calculation will behave in the exact same way as the old input file\n'
             'Please check the file for correctness beforehand')
     except etree.DocumentInvalid as err:
         echo.echo_critical(
             f'inp.xml conversion did not finish successfully. The resulting file violates the XML schema with:\n {err}')
 
-    #If there was no relax.xml included we need to rewrite the xinclude tag for it
-    if not tag_exists(xmltree, schema_dict_target, 'relaxation'):
-        xinclude_elem = etree.Element(INCLUDE_TAG, href='relax.xml', nsmap=INCLUDE_NSMAP)
-        xinclude_elem.append(etree.Element(FALLBACK_TAG))
-        xmltree.getroot().append(xinclude_elem)
-
-    etree.indent(xmltree)
     xmltree.write(output_file, encoding='utf-8', pretty_print=True)
     echo.echo_success(f'Converted file written to {output_file}')
 
 
 @inpxml.command('generate-conversion')
 @click.argument('from_version', type=str)
 @click.argument('to_version', type=str)
```

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/greensf_calculations.py` & `masci-tools-0.9.1/masci_tools/tools/greensf_calculations.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/greensf_visualization.py` & `masci-tools-0.9.1/masci_tools/tools/greensf_visualization.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/greensfunction.py` & `masci-tools-0.9.1/masci_tools/tools/greensfunction.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/matlabfrag.m` & `masci-tools-0.9.1/masci_tools/tools/matlabfrag.m`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/mlf2pdf.m` & `masci-tools-0.9.1/masci_tools/tools/mlf2pdf.m`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/molecule3D.m` & `masci-tools-0.9.1/masci_tools/tools/molecule3D.m`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/plotting.m` & `masci-tools-0.9.1/masci_tools/tools/plotting.m`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/saving_pdf.m` & `masci-tools-0.9.1/masci_tools/tools/saving_pdf.m`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/tools/saving_txt.m` & `masci-tools-0.9.1/masci_tools/tools/saving_txt.m`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/case_insensitive_dict.py` & `masci-tools-0.9.1/masci_tools/util/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/chemical_elements.py` & `masci-tools-0.9.1/masci_tools/util/chemical_elements.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/constants.py` & `masci-tools-0.9.1/masci_tools/util/constants.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/econfig.py` & `masci-tools-0.9.1/masci_tools/util/econfig.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/fleur_calculate_expression.py` & `masci-tools-0.9.1/masci_tools/util/fleur_calculate_expression.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/kkr_rms_tracker.py` & `masci-tools-0.9.1/masci_tools/util/kkr_rms_tracker.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/lockable_containers.py` & `masci-tools-0.9.1/masci_tools/util/lockable_containers.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/logging_util.py` & `masci-tools-0.9.1/masci_tools/util/logging_util.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/math_util.py` & `masci-tools-0.9.1/masci_tools/util/math_util.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/modifypotential.py` & `masci-tools-0.9.1/masci_tools/util/modifypotential.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/parse_tasks.py` & `masci-tools-0.9.1/masci_tools/util/parse_tasks.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/parse_tasks_decorators.py` & `masci-tools-0.9.1/masci_tools/util/parse_tasks_decorators.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/plot_shapfun.py` & `masci-tools-0.9.1/masci_tools/util/plot_shapfun.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/python_util.py` & `masci-tools-0.9.1/masci_tools/util/python_util.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/schema_dict_util.py` & `masci-tools-0.9.1/masci_tools/util/schema_dict_util.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/typing.py` & `masci-tools-0.9.1/masci_tools/util/typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 """
 
 TXPathLike = TypeVar('TXPathLike', bound=XPathLike)
 """
 Type for xpath expressions
 """
 
-FileLike: TypeAlias = 'str | bytes | Path | os.PathLike[Any] | IO[Any]'
+FileLike: TypeAlias = Union[str, bytes, Path, os.PathLike, IO[Any]]
 """
 Type used for functions accepting file-like objects, i.e. handles or file paths
 """
 
-XMLFileLike: TypeAlias = 'etree._ElementTree | etree._Element | FileLike'
+XMLFileLike: TypeAlias = Union[etree._ElementTree, etree._Element, FileLike]
 """
 Type used for functions accepting xml-file-like objects, i.e. handles or file paths
 or already parsed xml objects
 """
 
-XMLLike: TypeAlias = 'etree._Element | etree._ElementTree'
+XMLLike: TypeAlias = Union[etree._Element, etree._ElementTree]
 """
 Type used for functions accepting xml objects from lxml
 """
```

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/collect_xml_setters.py` & `masci-tools-0.9.1/masci_tools/util/xml/collect_xml_setters.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/common_functions.py` & `masci-tools-0.9.1/masci_tools/util/xml/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,16 +376,15 @@
                         of the base_xpath
     """
 
     results_base = set(eval_xpath(node, base_xpath, list_return=True))  #type:ignore
     results_complex = set(eval_xpath(node, complex_xpath, list_return=True))  #type:ignore
 
     if not results_base.issuperset(results_complex):
-        raise ValueError(
-            f"Complex xpath '{str(complex_xpath)}' is not compatible with the base_xpath '{str(base_xpath)}'")
+        raise ValueError(f"Complex xpath '{complex_xpath!r}' is not compatible with the base_xpath '{base_xpath!r}'")
 
 
 def abs_to_rel_xpath(xpath: str, new_root: str) -> str:
     """
     Convert a given xpath to be relative from a tag appearing in the
     original xpath.
```

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/converters.py` & `masci-tools-0.9.1/masci_tools/util/xml/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,16 +173,15 @@
             if logger is None:
                 raise ValueError(f"Could not convert '{text}', no matching definition found")
             logger.warning("Could not convert '%s', no matching definition found", text)
             converted_list.append(text)
             all_success = False
             continue
 
-        types: tuple[BaseType,
-                     ...] = tuple(definition.base_type for definition in text_definitions)  #type: ignore[misc]
+        types = tuple(definition.base_type for definition in text_definitions)
         lengths = {definition.length for definition in text_definitions}
 
         if len(text_definitions) == 1:
             if text_definitions[0].length == 1:
                 split_text = [text]
 
         converted_text, suc = convert_from_xml_single_values(split_text, types, constants=constants, logger=logger)
@@ -256,15 +255,15 @@
                 raise ValueError(f"Could not convert '{val}', no matching definition found")
             logger.warning("Could not convert '%s', no matching definition found", val)
 
             converted_list.append('')
             all_success = False
             continue
 
-        types: tuple[BaseType, ...] = tuple(definition.base_type for definition in text_definitions)  #type:ignore[misc]
+        types = tuple(definition.base_type for definition in text_definitions)
 
         converted_text, suc = convert_to_xml_single_values(val, types, logger=logger, float_format=float_format)
         all_success = all_success and suc
 
         converted_list.append(' '.join(converted_text))
 
     ret_value = converted_list
@@ -501,14 +500,16 @@
     """
     Converts a string of the form (float,float) to a complex number
 
     :param number_str: string to convert
 
     :returns: complex number
     """
+    number_str = number_str.strip()
+
     RE_COMPLEX_NUMBER = r'\([-+]?(?:\d*\.\d+|\d+)\,[-+]?(?:\d*\.\d+|\d+)\)'
     RE_SINGLE_FLOAT = r'[-+]?(?:\d*\.\d+|\d+)'
 
     if re.fullmatch(RE_COMPLEX_NUMBER, number_str) is None:
         raise ValueError(f"String '{number_str}' is not of the format (float,float)")
     real_str, imag_str = re.findall(RE_SINGLE_FLOAT, number_str)
```

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/xml_getters.py` & `masci-tools-0.9.1/masci_tools/util/xml/xml_getters.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_basic.py` & `masci-tools-0.9.1/masci_tools/util/xml/xml_setters_basic.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_names.py` & `masci-tools-0.9.1/masci_tools/util/xml/xml_setters_names.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_nmmpmat.py` & `masci-tools-0.9.1/masci_tools/util/xml/xml_setters_nmmpmat.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/xml_setters_xpaths.py` & `masci-tools-0.9.1/masci_tools/util/xml/xml_setters_xpaths.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/util/xml/xpathbuilder.py` & `masci-tools-0.9.1/masci_tools/util/xml/xpathbuilder.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/bokeh_plots.py` & `masci-tools-0.9.1/masci_tools/vis/bokeh_plots.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/bokeh_plotter.py` & `masci-tools-0.9.1/masci_tools/vis/bokeh_plotter.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/common.py` & `masci-tools-0.9.1/masci_tools/vis/common.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/data.py` & `masci-tools-0.9.1/masci_tools/vis/data.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/fleur.py` & `masci-tools-0.9.1/masci_tools/vis/fleur.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_FS_qdos.py` & `masci-tools-0.9.1/masci_tools/vis/kkr_plot_FS_qdos.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_bandstruc_qdos.py` & `masci-tools-0.9.1/masci_tools/vis/kkr_plot_bandstruc_qdos.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_dos.py` & `masci-tools-0.9.1/masci_tools/vis/kkr_plot_dos.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/kkr_plot_shapefun.py` & `masci-tools-0.9.1/masci_tools/vis/kkr_plot_shapefun.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/matplotlib_plotter.py` & `masci-tools-0.9.1/masci_tools/vis/matplotlib_plotter.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/parameters.py` & `masci-tools-0.9.1/masci_tools/vis/parameters.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/masci_tools/vis/plot_methods.py` & `masci-tools-0.9.1/masci_tools/vis/plot_methods.py`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/open_source_licenses.txt` & `masci-tools-0.9.1/open_source_licenses.txt`

 * *Files identical despite different names*

### Comparing `masci-tools-0.9.0a0/pyproject.toml` & `masci-tools-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 column_limit = 120
 coalesce_brackets = true
 align_closing_bracket_with_visual_indent = true
 split_arguments_when_comma_terminated = true
 indent_dictionary_value = false
 
 [bumpver]
-current_version = "0.9.0alpha0"
+current_version = "0.9.1"
 version_pattern = "MAJOR.MINOR.PATCH[TAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [bumpver.file_patterns]
```

### Comparing `masci-tools-0.9.0a0/PKG-INFO` & `masci-tools-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masci-tools
-Version: 0.9.0a0
+Version: 0.9.1
 Summary: masci-tools is a collection of tools for materials science.
 Keywords: material science,plots,fitting,visualization,aiida,dft,all-electron
 Author-email: The JuDFT team <j.broeder@fz-juelich.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

