# Comparing `tmp/formulaic-0.6.0.tar.gz` & `tmp/formulaic-0.6.1.tar.gz`

## Comparing `formulaic-0.6.0.tar` & `formulaic-0.6.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/README.md
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/benchmark.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/benchmarks.csv
--rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/benchmarks.png
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/plot.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/requirements.txt
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/mkdocs.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/requirements.in
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/requirements.txt
--rw-r--r--   0        0        0    16311 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/changelog.md
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/formulas.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/index.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/installation.md
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/migration.md
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/logo.png
--rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/logo.svg
--rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/logo_with_text.png
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/concepts/index.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/dev/index.md
--rw-r--r--   0        0        0    46139 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/contrasts.ipynb
--rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/formulae.ipynb
--rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/grammar.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/index.md
--rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/integration.ipynb
--rw-r--r--   0        0        0    27260 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/model_specs.ipynb
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/quickstart.ipynb
--rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/splines.ipynb
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/transforms.ipynb
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/_version.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/errors.py
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/formula.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/model_matrix.py
--rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/model_spec.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/sugar.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/arrow.py
--rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/base.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/pandas.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/enums.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/evaluated_factor.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/factor_values.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/scoped_factor.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/scoped_term.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/__init__.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/parser.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/utils.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/algos/__init__.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/algos/tokenize.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/algos/tokens_to_ast.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/__init__.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/ast_node.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/factor.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/formula_parser.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/operator.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/operator_resolver.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/ordered_set.py
--rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/structured.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/term.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/token.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/__init__.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/basis_spline.py
--rw-r--r--   0        0        0    25319 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/contrasts.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/identity.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/patsy_compat.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/poly.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/calculus.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/cast.py
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/constraints.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/context.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/iterators.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/layered_mapping.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/sentinels.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/sparse.py
--rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/stateful_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_formula.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_model_matrix.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_model_spec.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_sugar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/__init__.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/test_arrow.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/test_base.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/test_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_evaluated_factor.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_factor_values.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_scoped_factor.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_scoped_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/test_parser.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/algos/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/algos/test_tokenize.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/algos/test_tokens_to_ast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_ast_node.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_factor.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_formula_parser.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_operator.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_operator_resolver.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_ordered_set.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_structured.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_term.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/__init__.py
--rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_basis_spline.py
--rw-r--r--   0        0        0    28451 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_contrasts.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_identity.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_patsy_compat.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_poly.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_calculus.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_capture_context.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_cast.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_constraints.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_iterators.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_layered_mapping.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_sentinels.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_sparse.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_stateful_transforms.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.0/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.0/README.md
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 formulaic-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 formulaic-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/README.md
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/benchmarks.csv
+-rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/benchmarks.png
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/plot.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/requirements.txt
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/mkdocs.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/requirements.in
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/requirements.txt
+-rw-r--r--   0        0        0    16619 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/changelog.md
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/formulas.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/index.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/installation.md
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/migration.md
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/logo_with_text.png
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/concepts/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/dev/index.md
+-rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/contrasts.ipynb
+-rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/formulae.ipynb
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/grammar.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/index.md
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/integration.ipynb
+-rw-r--r--   0        0        0    27554 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/model_specs.ipynb
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/quickstart.ipynb
+-rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/splines.ipynb
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/transforms.ipynb
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/_version.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/errors.py
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/formula.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/model_matrix.py
+-rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/model_spec.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/sugar.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/__init__.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/arrow.py
+-rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/base.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/pandas.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/enums.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/evaluated_factor.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/factor_values.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/scoped_factor.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/scoped_term.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/__init__.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/parser.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/utils.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/algos/__init__.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/algos/tokenize.py
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/algos/tokens_to_ast.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/__init__.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/ast_node.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/factor.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/formula_parser.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/operator.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/operator_resolver.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/ordered_set.py
+-rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/structured.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/term.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/token.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/__init__.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/basis_spline.py
+-rw-r--r--   0        0        0    25669 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/contrasts.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/identity.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/patsy_compat.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/poly.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/calculus.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/cast.py
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/constraints.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/context.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/iterators.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/layered_mapping.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/sentinels.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/sparse.py
+-rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/stateful_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_formula.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_model_matrix.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_model_spec.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_sugar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/__init__.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/test_arrow.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/test_base.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/test_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_evaluated_factor.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_factor_values.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_scoped_factor.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_scoped_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/test_parser.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/algos/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/algos/test_tokenize.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/algos/test_tokens_to_ast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_ast_node.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_factor.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_formula_parser.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_operator.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_operator_resolver.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_ordered_set.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_structured.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_term.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/__init__.py
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_basis_spline.py
+-rw-r--r--   0        0        0    29100 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_contrasts.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_identity.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_patsy_compat.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_poly.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_calculus.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_capture_context.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_cast.py
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_constraints.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_layered_mapping.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_sentinels.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_sparse.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_stateful_transforms.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.1/README.md
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 formulaic-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 formulaic-0.6.1/PKG-INFO
```

### Comparing `formulaic-0.6.0/benchmarks/README.md` & `formulaic-0.6.1/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/benchmarks/benchmark.py` & `formulaic-0.6.1/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/benchmarks/benchmarks.csv` & `formulaic-0.6.1/benchmarks/benchmarks.csv`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/benchmarks/benchmarks.png` & `formulaic-0.6.1/benchmarks/benchmarks.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/benchmarks/plot.py` & `formulaic-0.6.1/benchmarks/plot.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/mkdocs.yml` & `formulaic-0.6.1/docsite/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/requirements.txt` & `formulaic-0.6.1/docsite/requirements.txt`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/changelog.md` & `formulaic-0.6.1/docsite/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 For changes since the latest tagged release, please refer to the
 [git commit log](https://github.com/matthewwardrop/formulaic/commits/main).
 
 ---
 
+# 0.6.1 (2 May 2023)
+
+This is a minor release with one new feature.
+
+**New features and enhancements:**
+
+* Added support for treating individual categorical features as though they do
+  not span the intercept (useful for intentionally generating over-specified
+  model matrices in e.g. regularized models).
+
 ## 0.6.0 (26 Apr 2023)
 
 This is a major release with some important consistency and completeness
 improvements. It should be treated as *almost* being the first release candidate
 of 1.0.0, which will land after some small amount of further feature extensions
 and documentation improvements. All users are recommended to upgrade.
```

### Comparing `formulaic-0.6.0/docsite/docs/formulas.md` & `formulaic-0.6.1/docsite/docs/formulas.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/index.md` & `formulaic-0.6.1/docsite/docs/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/installation.md` & `formulaic-0.6.1/docsite/docs/installation.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/migration.md` & `formulaic-0.6.1/docsite/docs/migration.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/assets/images/favicon.png` & `formulaic-0.6.1/docsite/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/assets/images/logo.png` & `formulaic-0.6.1/docsite/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/assets/images/logo.svg` & `formulaic-0.6.1/docsite/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/assets/images/logo_with_text.png` & `formulaic-0.6.1/docsite/docs/assets/images/logo_with_text.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/concepts/index.md` & `formulaic-0.6.1/docsite/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/guides/contrasts.ipynb` & `formulaic-0.6.1/docsite/docs/guides/contrasts.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999427236070382%*

 * *Differences: {"'cells'": "{30: {'source': {insert: [(22, 'or `.get_model_matrix()` methods; and can bypass the "*

 * *            "reducing of the rank of a \\n'), (23, 'single categorical term in a formula using "*

 * *            "`C(..., spans_intercept=False)` (this\\n'), (24, 'is especially useful, for example, "*

 * *            "if your model includes regularization and you\\n'), (25, 'would prefer to use the "*

 * *            "over-specified model to ensure fairer shrinkage).\\n')], delete: [22]}}}"}*

```diff
@@ -1349,15 +1349,18 @@
                 "overlapping in vectorspace. If you have two identical numerical vectors called\n",
                 "by two different names in your model matrix, Formulaic will happily build the\n",
                 "model matrix you requested, and you're on your own. This is intentional. While\n",
                 "Formulaic strives to make the model matrix generation process as painless as \n",
                 "possible, it also doesn't want to make more assumptions about the use of the \n",
                 "data than is necessary. Note that you can also disable Formulaic's structural\n",
                 "full-rankness algorithms by passing `ensure_full_rank=False` to `model_matrix()`\n",
-                "or `.get_model_matrix()` methods.\n",
+                "or `.get_model_matrix()` methods; and can bypass the reducing of the rank of a \n",
+                "single categorical term in a formula using `C(..., spans_intercept=False)` (this\n",
+                "is especially useful, for example, if your model includes regularization and you\n",
+                "would prefer to use the over-specified model to ensure fairer shrinkage).\n",
                 "\n",
                 "The algorithm that Formulaic uses was heavily inspired by `patsy`[^1]. The basic\n",
                 "idea is to recognize that all categorical codings span the intercept[^2]; and\n",
                 "then to break that coding up into two pieces: a single column that can be\n",
                 "dropped to avoid spanning the intercept, and the remaining body of the coding\n",
                 "that will always be present. You expand associatively the categorical factors,\n",
                 "and then greedily recombine the components, omitting any that would lead to\n",
```

### Comparing `formulaic-0.6.0/docsite/docs/guides/formulae.ipynb` & `formulaic-0.6.1/docsite/docs/guides/formulae.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/guides/grammar.md` & `formulaic-0.6.1/docsite/docs/guides/grammar.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/guides/integration.ipynb` & `formulaic-0.6.1/docsite/docs/guides/integration.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/guides/model_specs.ipynb` & `formulaic-0.6.1/docsite/docs/guides/model_specs.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995878612803546%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'data': {'text/html': {insert: [(19, '      "*

 * *            "<th>center(a)</th>\\n'), (28, '      <td>-1.0</td>\\n'), (35, '      "*

 * *            "<td>0.0</td>\\n'), (41, '      <td>1.0</td>\\n')], delete: [44, 37, 30, 21]}, "*

 * *            "'text/plain': ['   Intercept  center(a)  b[T.B]  b[T.C]\\n', '0        1.0       "*

 * *            "-1.0       0       0\\n', '1        1.0        0.0       1       0\\n', '2        "*

 * *            "1.0        1.0       0       1']}}}}, 4: {'output […]*

```diff
@@ -140,50 +140,50 @@
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Intercept</th>\n",
+                            "      <th>center(a)</th>\n",
                             "      <th>b[T.B]</th>\n",
                             "      <th>b[T.C]</th>\n",
-                            "      <th>center(a)</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>-1.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>-1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   Intercept  b[T.B]  b[T.C]  center(a)\n",
-                            "0        1.0       0       0       -1.0\n",
-                            "1        1.0       1       0        0.0\n",
-                            "2        1.0       0       1        1.0"
+                            "   Intercept  center(a)  b[T.B]  b[T.C]\n",
+                            "0        1.0       -1.0       0       0\n",
+                            "1        1.0        0.0       1       0\n",
+                            "2        1.0        1.0       0       1"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -200,15 +200,15 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "ModelSpec(formula=1 + b + center(a), materializer='pandas', materializer_params={}, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output='pandas', structure=[EncodedTermStructure(term=1, scoped_terms=[1], columns=['Intercept']), EncodedTermStructure(term=b, scoped_terms=[b-], columns=['b[T.B]', 'b[T.C]']), EncodedTermStructure(term=center(a), scoped_terms=[center(a)], columns=['center(a)'])], transform_state={'center(a)': {'ddof': 1, 'center': 2.0, 'scale': None}}, encoder_state={'b': (<Kind.CATEGORICAL: 'categorical'>, {'categories': ['A', 'B', 'C']}), 'center(a)': (<Kind.NUMERICAL: 'numerical'>, {})})"
+                            "ModelSpec(formula=1 + center(a) + b, materializer='pandas', materializer_params={}, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output='pandas', cluster_by=<ClusterBy.NONE: 'none'>, structure=[EncodedTermStructure(term=1, scoped_terms=[1], columns=['Intercept']), EncodedTermStructure(term=center(a), scoped_terms=[center(a)], columns=['center(a)']), EncodedTermStructure(term=b, scoped_terms=[b-], columns=['b[T.B]', 'b[T.C]'])], transform_state={'center(a)': {'ddof': 1, 'center': 2.0, 'scale': None}}, encoder_state={'center(a)': (<Kind.NUMERICAL: 'numerical'>, {}), 'b': (<Kind.CATEGORICAL: 'categorical'>, {'categories': ['A', 'B', 'C']})})"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -222,24 +222,24 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'column_names': ('Intercept', 'b[T.B]', 'b[T.C]', 'center(a)'),\n",
+                            "{'column_names': ('Intercept', 'center(a)', 'b[T.B]', 'b[T.C]'),\n",
                             " 'column_indices': OrderedDict([('Intercept', 0),\n",
-                            "              ('b[T.B]', 1),\n",
-                            "              ('b[T.C]', 2),\n",
-                            "              ('center(a)', 3)]),\n",
-                            " 'terms': [1, b, center(a)],\n",
-                            " 'term_indices': OrderedDict([(1, [0]), (b, [1, 2]), (center(a), [3])]),\n",
+                            "              ('center(a)', 1),\n",
+                            "              ('b[T.B]', 2),\n",
+                            "              ('b[T.C]', 3)]),\n",
+                            " 'terms': [1, center(a), b],\n",
+                            " 'term_indices': OrderedDict([(1, [0]), (center(a), [1]), (b, [2, 3])]),\n",
                             " 'term_slices': OrderedDict([(1, slice(0, 1, None)),\n",
-                            "              (b, slice(1, 3, None)),\n",
-                            "              (center(a), slice(3, 4, None))])}"
+                            "              (center(a), slice(1, 2, None)),\n",
+                            "              (b, slice(2, 4, None))])}"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -336,17 +336,17 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([[ 1.,  0.,  0., -1.],\n",
-                            "       [ 1.,  1.,  0.,  0.],\n",
-                            "       [ 1.,  0.,  1.,  1.]])"
+                            "array([[ 1., -1.,  0.,  0.],\n",
+                            "       [ 1.,  0.,  1.,  0.],\n",
+                            "       [ 1.,  1.,  0.,  1.]])"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -444,50 +444,50 @@
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Intercept</th>\n",
+                            "      <th>center(a)</th>\n",
                             "      <th>b[T.B]</th>\n",
                             "      <th>b[T.C]</th>\n",
-                            "      <th>center(a)</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>3.0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>3.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>4.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>4.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   Intercept  b[T.B]  b[T.C]  center(a)\n",
-                            "0        1.0       0       0        2.0\n",
-                            "1        1.0       1       0        3.0\n",
-                            "2        1.0       0       0        4.0"
+                            "   Intercept  center(a)  b[T.B]  b[T.C]\n",
+                            "0        1.0        2.0       0       0\n",
+                            "1        1.0        3.0       1       0\n",
+                            "2        1.0        4.0       0       0"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -529,50 +529,50 @@
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Intercept</th>\n",
+                            "      <th>center(a)</th>\n",
                             "      <th>b[T.B]</th>\n",
                             "      <th>b[T.C]</th>\n",
-                            "      <th>center(a)</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>3.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>3.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>4.0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>4.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   Intercept  b[T.B]  b[T.C]  center(a)\n",
-                            "0        1.0       0       0        2.0\n",
-                            "1        1.0       0       0        3.0\n",
-                            "2        1.0       0       0        4.0"
+                            "   Intercept  center(a)  b[T.B]  b[T.C]\n",
+                            "0        1.0        2.0       0       0\n",
+                            "1        1.0        3.0       0       0\n",
+                            "2        1.0        4.0       0       0"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -581,15 +581,15 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Directly constructing `ModelMatrix` instances\n",
+                "## Directly constructing `ModelSpec` instances\n",
                 "\n",
                 "It is possible to directly construct Model Matrices, and to prepopulate them\n",
                 "with various choices (e.g. output types, materializer, etc). You could even, in\n",
                 "principle, populate them with state information (but this is **not**\n",
                 "recommended; it is easy to make mistakes here, and is likely better to encode\n",
                 "these choices into the formula itself where possible). For example:"
             ]
@@ -598,15 +598,15 @@
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "ModelSpec(formula=1 + a + b + c, materializer=None, materializer_params=None, ensure_full_rank=False, na_action=<NAAction.DROP: 'drop'>, output='numpy', structure=None, transform_state={}, encoder_state={})"
+                            "ModelSpec(formula=1 + a + b + c, materializer=None, materializer_params=None, ensure_full_rank=False, na_action=<NAAction.DROP: 'drop'>, output='numpy', cluster_by=<ClusterBy.NONE: 'none'>, structure=None, transform_state={}, encoder_state={})"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -645,15 +645,15 @@
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "ModelSpec(formula=1 + a + b + c, materializer='pandas', materializer_params={}, ensure_full_rank=False, na_action=<NAAction.DROP: 'drop'>, output='numpy', structure=[EncodedTermStructure(term=1, scoped_terms=[1], columns=['Intercept']), EncodedTermStructure(term=a, scoped_terms=[a], columns=['a']), EncodedTermStructure(term=b, scoped_terms=[b], columns=['b']), EncodedTermStructure(term=c, scoped_terms=[c], columns=['c'])], transform_state={}, encoder_state={'a': (<Kind.NUMERICAL: 'numerical'>, {}), 'b': (<Kind.NUMERICAL: 'numerical'>, {}), 'c': (<Kind.NUMERICAL: 'numerical'>, {})})"
+                            "ModelSpec(formula=1 + a + b + c, materializer='pandas', materializer_params={}, ensure_full_rank=False, na_action=<NAAction.DROP: 'drop'>, output='numpy', cluster_by=<ClusterBy.NONE: 'none'>, structure=[EncodedTermStructure(term=1, scoped_terms=[1], columns=['Intercept']), EncodedTermStructure(term=a, scoped_terms=[a], columns=['a']), EncodedTermStructure(term=b, scoped_terms=[b], columns=['b']), EncodedTermStructure(term=c, scoped_terms=[c], columns=['c'])], transform_state={}, encoder_state={'a': (<Kind.NUMERICAL: 'numerical'>, {}), 'b': (<Kind.NUMERICAL: 'numerical'>, {}), 'c': (<Kind.NUMERICAL: 'numerical'>, {})})"
                         ]
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -690,19 +690,19 @@
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "root:\n",
-                            "    ModelSpec(formula=1 + a, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, structure=None, transform_state={}, encoder_state={})\n",
+                            "    ModelSpec(formula=1 + a, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, cluster_by=<ClusterBy.NONE: 'none'>, structure=None, transform_state={}, encoder_state={})\n",
                             ".substructure:\n",
-                            "    ModelSpec(formula=1 + b, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, structure=None, transform_state={}, encoder_state={})\n",
+                            "    ModelSpec(formula=1 + b, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, cluster_by=<ClusterBy.NONE: 'none'>, structure=None, transform_state={}, encoder_state={})\n",
                             ".another_substructure:\n",
-                            "    ModelSpec(formula=1 + c, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, structure=None, transform_state={}, encoder_state={})"
+                            "    ModelSpec(formula=1 + c, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, cluster_by=<ClusterBy.NONE: 'none'>, structure=None, transform_state={}, encoder_state={})"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -717,17 +717,17 @@
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             ".lhs:\n",
-                            "    ModelSpec(formula=y, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, structure=None, transform_state={}, encoder_state={})\n",
+                            "    ModelSpec(formula=y, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, cluster_by=<ClusterBy.NONE: 'none'>, structure=None, transform_state={}, encoder_state={})\n",
                             ".rhs:\n",
-                            "    ModelSpec(formula=a + b, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, structure=None, transform_state={}, encoder_state={})"
+                            "    ModelSpec(formula=a + b, materializer=None, materializer_params=None, ensure_full_rank=True, na_action=<NAAction.DROP: 'drop'>, output=None, cluster_by=<ClusterBy.NONE: 'none'>, structure=None, transform_state={}, encoder_state={})"
                         ]
                     },
                     "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `formulaic-0.6.0/docsite/docs/guides/quickstart.ipynb` & `formulaic-0.6.1/docsite/docs/guides/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/guides/splines.ipynb` & `formulaic-0.6.1/docsite/docs/guides/splines.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/docsite/docs/guides/transforms.ipynb` & `formulaic-0.6.1/docsite/docs/guides/transforms.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/__init__.py` & `formulaic-0.6.1/formulaic/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/errors.py` & `formulaic-0.6.1/formulaic/errors.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/formula.py` & `formulaic-0.6.1/formulaic/formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/model_matrix.py` & `formulaic-0.6.1/formulaic/model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/model_spec.py` & `formulaic-0.6.1/formulaic/model_spec.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/sugar.py` & `formulaic-0.6.1/formulaic/sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/arrow.py` & `formulaic-0.6.1/formulaic/materializers/arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/base.py` & `formulaic-0.6.1/formulaic/materializers/base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/pandas.py` & `formulaic-0.6.1/formulaic/materializers/pandas.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/types/evaluated_factor.py` & `formulaic-0.6.1/formulaic/materializers/types/evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/types/factor_values.py` & `formulaic-0.6.1/formulaic/materializers/types/factor_values.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/types/scoped_factor.py` & `formulaic-0.6.1/formulaic/materializers/types/scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/materializers/types/scoped_term.py` & `formulaic-0.6.1/formulaic/materializers/types/scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/parser.py` & `formulaic-0.6.1/formulaic/parser/parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/utils.py` & `formulaic-0.6.1/formulaic/parser/utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/algos/tokenize.py` & `formulaic-0.6.1/formulaic/parser/algos/tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/algos/tokens_to_ast.py` & `formulaic-0.6.1/formulaic/parser/algos/tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/ast_node.py` & `formulaic-0.6.1/formulaic/parser/types/ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/factor.py` & `formulaic-0.6.1/formulaic/parser/types/factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/formula_parser.py` & `formulaic-0.6.1/formulaic/parser/types/formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/operator.py` & `formulaic-0.6.1/formulaic/parser/types/operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/operator_resolver.py` & `formulaic-0.6.1/formulaic/parser/types/operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/ordered_set.py` & `formulaic-0.6.1/formulaic/parser/types/ordered_set.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/structured.py` & `formulaic-0.6.1/formulaic/parser/types/structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/term.py` & `formulaic-0.6.1/formulaic/parser/types/term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/parser/types/token.py` & `formulaic-0.6.1/formulaic/parser/types/token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/transforms/__init__.py` & `formulaic-0.6.1/formulaic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/transforms/basis_spline.py` & `formulaic-0.6.1/formulaic/transforms/basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/transforms/contrasts.py` & `formulaic-0.6.1/formulaic/transforms/contrasts.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 def C(
     data: Any,
     contrasts: Optional[
         Union[Contrasts, Dict[str, Iterable[Number]], numpy.ndarray]
     ] = None,
     *,
     levels: Optional[Iterable[str]] = None,
+    spans_intercept: bool = True,
 ):
     """
     Mark data as being categorical, and optionally specify the contrasts to be
     used during encoding.
 
     Args:
         data: The data to be marked as categorical.
@@ -42,14 +43,18 @@
             the contrast with a vector of weights for the categories, or a
             numpy array with columns representing the contrasts, and rows
             representing the weights over the categories in the data. If not
             specified, a `Treatment` encoding is assumed.
         levels: The categorical levels associated with `data`. If not present,
             levels are inferred from `data`. Note that extra levels in `data`
             will be treated as null data.
+        spans_intercept: Whether the categorical data being coded should be
+            treated as though it spans the intercept. This should nearly always
+            true, except when you are building a model that explicitly handles
+            this using regularization (or other modeling techniques).
     """
 
     def encoder(
         values: Any,
         reduced_rank: bool,
         drop_rows: List[int],
         encoder_state: Dict[str, Any],
@@ -65,15 +70,15 @@
             _state=encoder_state,
             _spec=model_spec,
         )
 
     return FactorValues(
         data,
         kind="categorical",
-        spans_intercept=True,
+        spans_intercept=spans_intercept,
         encoder=encoder,
     )
 
 
 @stateful_transform
 def encode_contrasts(
     data,
```

### Comparing `formulaic-0.6.0/formulaic/transforms/patsy_compat.py` & `formulaic-0.6.1/formulaic/transforms/patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/transforms/poly.py` & `formulaic-0.6.1/formulaic/transforms/poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/transforms/scale.py` & `formulaic-0.6.1/formulaic/transforms/scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/calculus.py` & `formulaic-0.6.1/formulaic/utils/calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/cast.py` & `formulaic-0.6.1/formulaic/utils/cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/constraints.py` & `formulaic-0.6.1/formulaic/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/context.py` & `formulaic-0.6.1/formulaic/utils/context.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/iterators.py` & `formulaic-0.6.1/formulaic/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/layered_mapping.py` & `formulaic-0.6.1/formulaic/utils/layered_mapping.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/sparse.py` & `formulaic-0.6.1/formulaic/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/formulaic/utils/stateful_transforms.py` & `formulaic-0.6.1/formulaic/utils/stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/test_formula.py` & `formulaic-0.6.1/tests/test_formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/test_model_matrix.py` & `formulaic-0.6.1/tests/test_model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/test_model_spec.py` & `formulaic-0.6.1/tests/test_model_spec.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/test_sugar.py` & `formulaic-0.6.1/tests/test_sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/materializers/test_arrow.py` & `formulaic-0.6.1/tests/materializers/test_arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/materializers/test_base.py` & `formulaic-0.6.1/tests/materializers/test_base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/materializers/test_pandas.py` & `formulaic-0.6.1/tests/materializers/test_pandas.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/materializers/types/test_evaluated_factor.py` & `formulaic-0.6.1/tests/materializers/types/test_evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/materializers/types/test_scoped_factor.py` & `formulaic-0.6.1/tests/materializers/types/test_scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/materializers/types/test_scoped_term.py` & `formulaic-0.6.1/tests/materializers/types/test_scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/test_parser.py` & `formulaic-0.6.1/tests/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/test_utils.py` & `formulaic-0.6.1/tests/parser/test_utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/algos/test_tokenize.py` & `formulaic-0.6.1/tests/parser/algos/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/algos/test_tokens_to_ast.py` & `formulaic-0.6.1/tests/parser/algos/test_tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_ast_node.py` & `formulaic-0.6.1/tests/parser/types/test_ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_factor.py` & `formulaic-0.6.1/tests/parser/types/test_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_formula_parser.py` & `formulaic-0.6.1/tests/parser/types/test_formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_operator.py` & `formulaic-0.6.1/tests/parser/types/test_operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_operator_resolver.py` & `formulaic-0.6.1/tests/parser/types/test_operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_structured.py` & `formulaic-0.6.1/tests/parser/types/test_structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_term.py` & `formulaic-0.6.1/tests/parser/types/test_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/parser/types/test_token.py` & `formulaic-0.6.1/tests/parser/types/test_token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/transforms/test_basis_spline.py` & `formulaic-0.6.1/tests/transforms/test_basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/transforms/test_contrasts.py` & `formulaic-0.6.1/tests/transforms/test_contrasts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 
 import numpy
 import pandas
 import pytest
 import scipy.sparse as spsparse
 
+from formulaic import model_matrix
 from formulaic.errors import DataMismatchWarning
 from formulaic.materializers import FactorValues
 from formulaic.model_spec import ModelSpec
 from formulaic.transforms.contrasts import (
     SumContrasts,
     encode_contrasts,
     ContrastsRegistry as contr,
@@ -845,7 +846,29 @@
             },
             index=[1, 2, 3],
         )
         coefficient_matrix_reduced = contrasts.get_coefficient_matrix(
             ["a", "b", "c"], reduced_rank=True
         )
         assert numpy.allclose(coefficient_matrix_reduced, reference_reduced)
+
+
+def test_full_rankness_opt_out():
+    data = pandas.DataFrame({"A": ["a", "b", "c"]})
+    assert model_matrix("A", data).model_spec.column_names == (
+        "Intercept",
+        "A[T.b]",
+        "A[T.c]",
+    )
+    assert model_matrix("C(A)", data).model_spec.column_names == (
+        "Intercept",
+        "C(A)[T.b]",
+        "C(A)[T.c]",
+    )
+    assert model_matrix(
+        "C(A, spans_intercept=False)", data
+    ).model_spec.column_names == (
+        "Intercept",
+        "C(A, spans_intercept=False)[T.a]",
+        "C(A, spans_intercept=False)[T.b]",
+        "C(A, spans_intercept=False)[T.c]",
+    )
```

### Comparing `formulaic-0.6.0/tests/transforms/test_patsy_compat.py` & `formulaic-0.6.1/tests/transforms/test_patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/transforms/test_poly.py` & `formulaic-0.6.1/tests/transforms/test_poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/transforms/test_scale.py` & `formulaic-0.6.1/tests/transforms/test_scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/utils/test_calculus.py` & `formulaic-0.6.1/tests/utils/test_calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/utils/test_cast.py` & `formulaic-0.6.1/tests/utils/test_cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/utils/test_constraints.py` & `formulaic-0.6.1/tests/utils/test_constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/utils/test_layered_mapping.py` & `formulaic-0.6.1/tests/utils/test_layered_mapping.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/utils/test_sparse.py` & `formulaic-0.6.1/tests/utils/test_sparse.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/tests/utils/test_stateful_transforms.py` & `formulaic-0.6.1/tests/utils/test_stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/.gitignore` & `formulaic-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/LICENSE` & `formulaic-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/README.md` & `formulaic-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/pyproject.toml` & `formulaic-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.0/PKG-INFO` & `formulaic-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formulaic
-Version: 0.6.0
+Version: 0.6.1
 Summary: An implementation of Wilkinson formulas.
 Project-URL: repository, https://github.com/matthewwardrop/formulaic
 Project-URL: documentation, https://matthewwardrop.github.io/formulaic
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

