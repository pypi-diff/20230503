# Comparing `tmp/tuxsuite-1.8.0.tar.gz` & `tmp/tuxsuite-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxsuite-1.8.0.tar", last modified: Thu Feb 16 06:22:41 2023, max compression
+gzip compressed data, was "tuxsuite-1.9.0.tar", last modified: Mon Feb 27 07:39:06 2023, max compression
```

## Comparing `tuxsuite-1.8.0.tar` & `tuxsuite-1.9.0.tar`

### file list

```diff
@@ -1,143 +1,145 @@
--rw-r--r--   0        0        0       66 2023-02-16 06:22:38.989627 tuxsuite-1.8.0/.ackrc
--rw-r--r--   0        0        0       96 2023-02-16 06:22:38.989627 tuxsuite-1.8.0/.flake8
--rw-r--r--   0        0        0       88 2023-02-16 06:22:38.989627 tuxsuite-1.8.0/.gitignore
--rw-r--r--   0        0        0     2075 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      431 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/.gitlab/issue_templates/bug.md
--rw-r--r--   0        0        0      498 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/.gitlab/issue_templates/feature_request.md
--rw-r--r--   0        0        0      322 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/Dockerfile
--rw-r--r--   0        0        0      828 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/Dockerfile.ci-debian
--rw-r--r--   0        0        0      528 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1054 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/LICENSE
--rw-r--r--   0        0        0      754 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/Makefile
--rw-r--r--   0        0        0    11062 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/README.md
--rw-r--r--   0        0        0      150 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/debian/changelog
--rw-r--r--   0        0        0     1201 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/debian/control
--rw-r--r--   0        0        0      100 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/debian/gbp.conf
--rw-r--r--   0        0        0      594 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/debian/rules
--rw-r--r--   0        0        0       12 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/debian/source/format
--rw-r--r--   0        0        0       10 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/docs/.gitignore
--rw-r--r--   0        0        0     3487 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/docs/code-of-conduct.md
--rw-r--r--   0        0        0      133 2023-02-16 06:22:38.990627 tuxsuite-1.8.0/docs/extra.css
--rw-r--r--   0        0        0     5472 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/images/tuxbuild_icon.svg
--rw-r--r--   0        0        0     3642 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/images/tuxsuite.svg
--rw-r--r--   0        0        0     5438 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/images/tuxsuite_icon.svg
--rw-r--r--   0        0        0     5422 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/images/tuxtest_icon.svg
--rw-r--r--   0        0        0    10515 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/plan/examples.md
--rw-r--r--   0        0        0     2736 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/plan/index.md
--rw-r--r--   0        0        0     3966 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/plan/specifications.md
--rw-r--r--   0        0        0      739 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/plan/subcommands.md
--rw-r--r--   0        0        0     1451 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/python-api.md
--rw-r--r--   0        0        0      486 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/results/arguments/from-json.md
--rw-r--r--   0        0        0      916 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/results/arguments/json-out.md
--rw-r--r--   0        0        0     6674 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/results/examples.md
--rw-r--r--   0        0        0      796 2023-02-16 06:22:38.991627 tuxsuite-1.8.0/docs/results/features/results.md
--rw-r--r--   0        0        0     3033 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/additional-arguments.md
--rw-r--r--   0        0        0     1905 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/architectures-toolchains.md
--rw-r--r--   0        0        0      760 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/build-name.md
--rw-r--r--   0        0        0     3137 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/build-status.md
--rw-r--r--   0        0        0      845 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/environment-variables.md
--rw-r--r--   0        0        0      921 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/git-ref-sha.md
--rw-r--r--   0        0        0      358 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/git-repo.md
--rw-r--r--   0        0        0     1451 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/kconfig.md
--rw-r--r--   0        0        0      937 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/make-targets.md
--rw-r--r--   0        0        0      611 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/make-variables.md
--rw-r--r--   0        0        0    60863 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/metadata.md
--rw-r--r--   0        0        0     4965 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/patch-series.md
--rw-r--r--   0        0        0     1378 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/subcommands.md
--rw-r--r--   0        0        0      638 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/target-architectures.md
--rw-r--r--   0        0        0     1226 2023-02-16 06:22:38.992627 tuxsuite-1.8.0/docs/tuxbuild/toolchains.md
--rw-r--r--   0        0        0      709 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxbuild/tuxmake.md
--rw-r--r--   0        0        0      672 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/arguments/device.md
--rw-r--r--   0        0        0      233 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/arguments/kernel.md
--rw-r--r--   0        0        0      349 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/arguments/no-wait.md
--rw-r--r--   0        0        0      888 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/arguments/tests.md
--rw-r--r--   0        0        0      485 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/arguments/timeouts.md
--rw-r--r--   0        0        0      738 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/features/devices.md
--rw-r--r--   0        0        0      960 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/features/status-result.md
--rw-r--r--   0        0        0     1629 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/docs/tuxtest/subcommands.md
--rw-r--r--   0        0        0      130 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/Makefile
--rw-r--r--   0        0        0      401 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/bitbake/demo.json
--rw-r--r--   0        0        0      154 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/bitbake/kas.json
--rw-r--r--   0        0        0      313 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/bitbake/ledge-rpb.json
--rw-r--r--   0        0        0      933 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/bitbake/lkft.json
--rw-r--r--   0        0        0      537 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/bitbake/lt-qcom.json
--rw-r--r--   0        0        0      277 2023-02-16 06:22:38.993627 tuxsuite-1.8.0/examples/bitbake/mbed.json
--rw-r--r--   0        0        0    62921 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/mbed.yaml
--rw-r--r--   0        0        0      386 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/oe-rpb.json
--rw-r--r--   0        0        0      402 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/oniro.json
--rw-r--r--   0        0        0     3670 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/poky-kirkstone-plan.yaml
--rw-r--r--   0        0        0     2853 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/poky-next.yaml
--rw-r--r--   0        0        0      386 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/qcom-rpb-dunfell.json
--rw-r--r--   0        0        0      384 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/qcom-rpb-honister.json
--rw-r--r--   0        0        0      581 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/sample_bake_plan.yaml
--rw-r--r--   0        0        0      723 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/template.json
--rw-r--r--   0        0        0      295 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/bitbake/yocto.json
--rw-r--r--   0        0        0    10107 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/linux-test-plan.yaml
--rw-r--r--   0        0        0     1727 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/examples/planv1.yaml
--rw-r--r--   0        0        0     2469 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/mkdocs.yml
--rw-r--r--   0        0        0      508 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      173 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/requirements-dev.txt
--rw-r--r--   0        0        0        5 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/requirements.txt
--rwxr-xr-x   0        0        0      124 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/run
--rwxr-xr-x   0        0        0      224 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/scripts/markdownlint
--rwxr-xr-x   0        0        0      158 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/scripts/readme2index.sh
--rwxr-xr-x   0        0        0     1618 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/scripts/release
--rwxr-xr-x   0        0        0      438 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/scripts/validate-pre-release.sh
--rw-r--r--   0        0        0        0 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/test/__init__.py
--rwxr-xr-x   0        0        0    14786 2023-02-16 06:22:38.994627 tuxsuite-1.8.0/test/api_v1.py
--rw-r--r--   0        0        0     8993 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/conftest.py
--rwxr-xr-x   0        0        0      593 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/integration/test_api_server
--rwxr-xr-x   0        0        0      146 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/integration/test_call_via_python_module
--rw-r--r--   0        0        0     2738 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/integration/test_helper.sh
--rwxr-xr-x   0        0        0     1599 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/integration/test_tuxsuite_build
--rw-r--r--   0        0        0      405 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/templates/build.html
--rw-r--r--   0        0        0      196 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/templates/index.html
--rw-r--r--   0        0        0      400 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/templates/layout.html
--rw-r--r--   0        0        0      483 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/test_api_v1.py
--rw-r--r--   0        0        0    39175 2023-02-16 06:22:38.995627 tuxsuite-1.8.0/test/test_build.py
--rw-r--r--   0        0        0    51112 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli.py
--rw-r--r--   0        0        0    14407 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli_build_subcommands.py
--rw-r--r--   0        0        0     4648 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli_group_subcommands.py
--rw-r--r--   0        0        0    47302 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli_plan_subcommands.py
--rw-r--r--   0        0        0     2973 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli_project_subcommands.py
--rw-r--r--   0        0        0    18930 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli_test_subcommands.py
--rw-r--r--   0        0        0     3364 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_cli_utils.py
--rw-r--r--   0        0        0     6103 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_config.py
--rw-r--r--   0        0        0     1269 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_download.py
--rw-r--r--   0        0        0     2581 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_gitutils.py
--rw-r--r--   0        0        0      271 2023-02-16 06:22:38.996628 tuxsuite-1.8.0/test/test_main.py
--rw-r--r--   0        0        0    34993 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/test/test_plan.py
--rw-r--r--   0        0        0     1129 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/test/test_requests.py
--rw-r--r--   0        0        0      524 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/test/test_tuxsuite.py
--rw-r--r--   0        0        0      733 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite.rst
--rw-r--r--   0        0        0     1923 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite.spec
--rw-r--r--   0        0        0     9734 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/__init__.py
--rw-r--r--   0        0        0      122 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/__main__.py
--rw-r--r--   0        0        0    45589 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/build.py
--rw-r--r--   0        0        0     4845 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/__init__.py
--rw-r--r--   0        0        0     4707 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/bake.py
--rw-r--r--   0        0        0    14997 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/build.py
--rw-r--r--   0        0        0      617 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/colors.py
--rw-r--r--   0        0        0     1899 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/common.py
--rw-r--r--   0        0        0      477 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/config.py
--rw-r--r--   0        0        0     3812 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/group.py
--rw-r--r--   0        0        0      181 2023-02-16 06:22:38.997628 tuxsuite-1.8.0/tuxsuite/cli/icons.py
--rw-r--r--   0        0        0     7185 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/models.py
--rw-r--r--   0        0        0    16619 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/plan.py
--rw-r--r--   0        0        0     1894 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/project.py
--rw-r--r--   0        0        0      695 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/requests.py
--rw-r--r--   0        0        0     7557 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/results.py
--rw-r--r--   0        0        0    14332 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/test.py
--rw-r--r--   0        0        0    10145 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/utils.py
--rw-r--r--   0        0        0       45 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/version.py
--rw-r--r--   0        0        0      259 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/cli/yaml.py
--rw-r--r--   0        0        0     9104 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/config.py
--rw-r--r--   0        0        0      795 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/download.py
--rw-r--r--   0        0        0     1067 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/exceptions.py
--rw-r--r--   0        0        0     1569 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/gitutils.py
--rw-r--r--   0        0        0     1703 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/requests.py
--rw-r--r--   0        0        0     1860 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/schema.py
--rw-r--r--   0        0        0     1185 2023-02-16 06:22:38.998628 tuxsuite-1.8.0/tuxsuite/utils.py
--rw-r--r--   0        0        0    35838 2023-02-16 06:22:39.001628 tuxsuite-1.8.0/tuxsuite_logo.png
--rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 tuxsuite-1.8.0/setup.py
--rw-r--r--   0        0        0      192 1970-01-01 00:00:00.000000 tuxsuite-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/.ackrc
+-rw-r--r--   0        0        0       96 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/.flake8
+-rw-r--r--   0        0        0       88 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/.gitignore
+-rw-r--r--   0        0        0     2075 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      431 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/.gitlab/issue_templates/bug.md
+-rw-r--r--   0        0        0      498 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/.gitlab/issue_templates/feature_request.md
+-rw-r--r--   0        0        0      322 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/Dockerfile
+-rw-r--r--   0        0        0      828 2023-02-27 07:39:03.726854 tuxsuite-1.9.0/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      528 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1054 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/LICENSE
+-rw-r--r--   0        0        0      754 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/Makefile
+-rw-r--r--   0        0        0    11062 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/README.md
+-rw-r--r--   0        0        0      150 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/debian/changelog
+-rw-r--r--   0        0        0     1201 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/debian/control
+-rw-r--r--   0        0        0      100 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/debian/gbp.conf
+-rw-r--r--   0        0        0      594 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/debian/rules
+-rw-r--r--   0        0        0       12 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/debian/source/format
+-rw-r--r--   0        0        0       10 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/.gitignore
+-rw-r--r--   0        0        0     4198 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/callbacks.md
+-rw-r--r--   0        0        0     3487 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/code-of-conduct.md
+-rw-r--r--   0        0        0      133 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/extra.css
+-rw-r--r--   0        0        0     5472 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/images/tuxbuild_icon.svg
+-rw-r--r--   0        0        0     3642 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/images/tuxsuite.svg
+-rw-r--r--   0        0        0     5438 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/images/tuxsuite_icon.svg
+-rw-r--r--   0        0        0     5422 2023-02-27 07:39:03.727854 tuxsuite-1.9.0/docs/images/tuxtest_icon.svg
+-rw-r--r--   0        0        0    10515 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/plan/examples.md
+-rw-r--r--   0        0        0     2736 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/plan/index.md
+-rw-r--r--   0        0        0     3966 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/plan/specifications.md
+-rw-r--r--   0        0        0      739 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/plan/subcommands.md
+-rw-r--r--   0        0        0     1451 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/python-api.md
+-rw-r--r--   0        0        0      486 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/results/arguments/from-json.md
+-rw-r--r--   0        0        0      916 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/results/arguments/json-out.md
+-rw-r--r--   0        0        0     6674 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/results/examples.md
+-rw-r--r--   0        0        0      796 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/results/features/results.md
+-rw-r--r--   0        0        0     3307 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/additional-arguments.md
+-rw-r--r--   0        0        0     1905 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/architectures-toolchains.md
+-rw-r--r--   0        0        0      760 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/build-name.md
+-rw-r--r--   0        0        0     3137 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/build-status.md
+-rw-r--r--   0        0        0      845 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/environment-variables.md
+-rw-r--r--   0        0        0      921 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/git-ref-sha.md
+-rw-r--r--   0        0        0      358 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/git-repo.md
+-rw-r--r--   0        0        0     1451 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/kconfig.md
+-rw-r--r--   0        0        0      937 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/make-targets.md
+-rw-r--r--   0        0        0      611 2023-02-27 07:39:03.728854 tuxsuite-1.9.0/docs/tuxbuild/make-variables.md
+-rw-r--r--   0        0        0    60863 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxbuild/metadata.md
+-rw-r--r--   0        0        0     4965 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxbuild/patch-series.md
+-rw-r--r--   0        0        0     1378 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxbuild/subcommands.md
+-rw-r--r--   0        0        0      638 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxbuild/target-architectures.md
+-rw-r--r--   0        0        0     1226 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxbuild/toolchains.md
+-rw-r--r--   0        0        0      709 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxbuild/tuxmake.md
+-rw-r--r--   0        0        0      298 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/arguments/additional-arguments.md
+-rw-r--r--   0        0        0      672 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/arguments/device.md
+-rw-r--r--   0        0        0      233 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/arguments/kernel.md
+-rw-r--r--   0        0        0      349 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/arguments/no-wait.md
+-rw-r--r--   0        0        0      888 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/arguments/tests.md
+-rw-r--r--   0        0        0      485 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/arguments/timeouts.md
+-rw-r--r--   0        0        0      738 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/features/devices.md
+-rw-r--r--   0        0        0      960 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/features/status-result.md
+-rw-r--r--   0        0        0     1629 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/docs/tuxtest/subcommands.md
+-rw-r--r--   0        0        0      130 2023-02-27 07:39:03.729854 tuxsuite-1.9.0/examples/Makefile
+-rw-r--r--   0        0        0      401 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/demo.json
+-rw-r--r--   0        0        0      154 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/kas.json
+-rw-r--r--   0        0        0      313 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/ledge-rpb.json
+-rw-r--r--   0        0        0      933 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/lkft.json
+-rw-r--r--   0        0        0      537 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/lt-qcom.json
+-rw-r--r--   0        0        0      277 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/mbed.json
+-rw-r--r--   0        0        0    62921 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/mbed.yaml
+-rw-r--r--   0        0        0      386 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/oe-rpb.json
+-rw-r--r--   0        0        0      402 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/oniro.json
+-rw-r--r--   0        0        0     3670 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/poky-kirkstone-plan.yaml
+-rw-r--r--   0        0        0     2853 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/poky-next.yaml
+-rw-r--r--   0        0        0      386 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/qcom-rpb-dunfell.json
+-rw-r--r--   0        0        0      384 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/qcom-rpb-honister.json
+-rw-r--r--   0        0        0      581 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/sample_bake_plan.yaml
+-rw-r--r--   0        0        0      723 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/template.json
+-rw-r--r--   0        0        0      295 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/bitbake/yocto.json
+-rw-r--r--   0        0        0    10107 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/linux-test-plan.yaml
+-rw-r--r--   0        0        0     1727 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/examples/planv1.yaml
+-rw-r--r--   0        0        0     2569 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/mkdocs.yml
+-rw-r--r--   0        0        0      508 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      173 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/requirements-dev.txt
+-rw-r--r--   0        0        0        5 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/requirements.txt
+-rwxr-xr-x   0        0        0      124 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/run
+-rwxr-xr-x   0        0        0      218 2023-02-27 07:39:03.730854 tuxsuite-1.9.0/scripts/markdownlint
+-rwxr-xr-x   0        0        0      158 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/scripts/readme2index.sh
+-rwxr-xr-x   0        0        0     1618 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/scripts/release
+-rwxr-xr-x   0        0        0      438 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/scripts/validate-pre-release.sh
+-rw-r--r--   0        0        0        0 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/__init__.py
+-rwxr-xr-x   0        0        0    14786 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/api_v1.py
+-rw-r--r--   0        0        0     8993 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/conftest.py
+-rwxr-xr-x   0        0        0      593 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/integration/test_api_server
+-rwxr-xr-x   0        0        0      146 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/integration/test_call_via_python_module
+-rw-r--r--   0        0        0     2738 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/integration/test_helper.sh
+-rwxr-xr-x   0        0        0     1599 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/integration/test_tuxsuite_build
+-rw-r--r--   0        0        0      405 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/templates/build.html
+-rw-r--r--   0        0        0      196 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/templates/index.html
+-rw-r--r--   0        0        0      400 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/templates/layout.html
+-rw-r--r--   0        0        0      483 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/test_api_v1.py
+-rw-r--r--   0        0        0    39239 2023-02-27 07:39:03.731854 tuxsuite-1.9.0/test/test_build.py
+-rw-r--r--   0        0        0    51355 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli.py
+-rw-r--r--   0        0        0    14407 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli_build_subcommands.py
+-rw-r--r--   0        0        0     4648 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli_group_subcommands.py
+-rw-r--r--   0        0        0    47302 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli_plan_subcommands.py
+-rw-r--r--   0        0        0     2973 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli_project_subcommands.py
+-rw-r--r--   0        0        0    18930 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli_test_subcommands.py
+-rw-r--r--   0        0        0     3364 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_cli_utils.py
+-rw-r--r--   0        0        0     6103 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_config.py
+-rw-r--r--   0        0        0     1269 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_download.py
+-rw-r--r--   0        0        0     2581 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_gitutils.py
+-rw-r--r--   0        0        0      271 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_main.py
+-rw-r--r--   0        0        0    34993 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_plan.py
+-rw-r--r--   0        0        0     1129 2023-02-27 07:39:03.732854 tuxsuite-1.9.0/test/test_requests.py
+-rw-r--r--   0        0        0      524 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/test/test_tuxsuite.py
+-rw-r--r--   0        0        0      733 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite.rst
+-rw-r--r--   0        0        0     1923 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite.spec
+-rw-r--r--   0        0        0     9734 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/__init__.py
+-rw-r--r--   0        0        0      122 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/__main__.py
+-rw-r--r--   0        0        0    45980 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/build.py
+-rw-r--r--   0        0        0     4845 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/__init__.py
+-rw-r--r--   0        0        0     5013 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/bake.py
+-rw-r--r--   0        0        0    15337 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/build.py
+-rw-r--r--   0        0        0      617 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/colors.py
+-rw-r--r--   0        0        0     1921 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/common.py
+-rw-r--r--   0        0        0      477 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/config.py
+-rw-r--r--   0        0        0     3812 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/group.py
+-rw-r--r--   0        0        0      181 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/icons.py
+-rw-r--r--   0        0        0     7185 2023-02-27 07:39:03.733854 tuxsuite-1.9.0/tuxsuite/cli/models.py
+-rw-r--r--   0        0        0    16619 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/plan.py
+-rw-r--r--   0        0        0     1894 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/project.py
+-rw-r--r--   0        0        0      695 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/requests.py
+-rw-r--r--   0        0        0     7557 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/results.py
+-rw-r--r--   0        0        0    14641 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/test.py
+-rw-r--r--   0        0        0    10321 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/utils.py
+-rw-r--r--   0        0        0       45 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/version.py
+-rw-r--r--   0        0        0      259 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/cli/yaml.py
+-rw-r--r--   0        0        0     9104 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/config.py
+-rw-r--r--   0        0        0      795 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/download.py
+-rw-r--r--   0        0        0     1067 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/exceptions.py
+-rw-r--r--   0        0        0     1569 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/gitutils.py
+-rw-r--r--   0        0        0     1703 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/requests.py
+-rw-r--r--   0        0        0     1860 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/schema.py
+-rw-r--r--   0        0        0     1185 2023-02-27 07:39:03.734854 tuxsuite-1.9.0/tuxsuite/utils.py
+-rw-r--r--   0        0        0    35838 2023-02-27 07:39:03.735854 tuxsuite-1.9.0/tuxsuite_logo.png
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 tuxsuite-1.9.0/setup.py
+-rw-r--r--   0        0        0      192 1970-01-01 00:00:00.000000 tuxsuite-1.9.0/PKG-INFO
```

### Comparing `tuxsuite-1.8.0/.gitlab-ci.yml` & `tuxsuite-1.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/Dockerfile.ci-debian` & `tuxsuite-1.9.0/Dockerfile.ci-debian`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/Dockerfile.ci-fedora` & `tuxsuite-1.9.0/Dockerfile.ci-fedora`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/LICENSE` & `tuxsuite-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/Makefile` & `tuxsuite-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/README.md` & `tuxsuite-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/debian/control` & `tuxsuite-1.9.0/debian/control`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/debian/rules` & `tuxsuite-1.9.0/debian/rules`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/code-of-conduct.md` & `tuxsuite-1.9.0/docs/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/images/tuxbuild_icon.svg` & `tuxsuite-1.9.0/docs/images/tuxbuild_icon.svg`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/images/tuxsuite.svg` & `tuxsuite-1.9.0/docs/images/tuxsuite.svg`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/images/tuxsuite_icon.svg` & `tuxsuite-1.9.0/docs/images/tuxsuite_icon.svg`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/images/tuxtest_icon.svg` & `tuxsuite-1.9.0/docs/images/tuxtest_icon.svg`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/plan/examples.md` & `tuxsuite-1.9.0/docs/plan/examples.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/plan/index.md` & `tuxsuite-1.9.0/docs/plan/index.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/plan/specifications.md` & `tuxsuite-1.9.0/docs/plan/specifications.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/plan/subcommands.md` & `tuxsuite-1.9.0/docs/plan/subcommands.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/python-api.md` & `tuxsuite-1.9.0/docs/python-api.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/results/arguments/json-out.md` & `tuxsuite-1.9.0/docs/results/arguments/json-out.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/results/examples.md` & `tuxsuite-1.9.0/docs/results/examples.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/results/features/results.md` & `tuxsuite-1.9.0/docs/results/features/results.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/additional-arguments.md` & `tuxsuite-1.9.0/docs/tuxbuild/additional-arguments.md`

 * *Files 12% similar despite different names*

```diff
@@ -82,7 +82,15 @@
 the artifacts of a build that uses private storage, as shown below:
 
 ```sh
 curl -L -H 'Authorization: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx' \
 'https://storage.tuxsuite.com/private/demo/demo/builds/2Klp3IebV45CIMnC7BnfTGbIAGV/build.log' \
 -o /tmp/build.log
 ```
+
+## callback
+
+`--callback` is an optional argument which POSTs JSON data that has
+the status of the build, at the end of the build to the given URL. The
+URL should be a valid http(s) link that accepts POST data.
+
+[See Callbacks Reference, for more details](../callbacks.md)
```

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/architectures-toolchains.md` & `tuxsuite-1.9.0/docs/tuxbuild/architectures-toolchains.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/build-name.md` & `tuxsuite-1.9.0/docs/tuxbuild/build-name.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/build-status.md` & `tuxsuite-1.9.0/docs/tuxbuild/build-status.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/environment-variables.md` & `tuxsuite-1.9.0/docs/tuxbuild/environment-variables.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/git-ref-sha.md` & `tuxsuite-1.9.0/docs/tuxbuild/git-ref-sha.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/kconfig.md` & `tuxsuite-1.9.0/docs/tuxbuild/kconfig.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/make-targets.md` & `tuxsuite-1.9.0/docs/tuxbuild/make-targets.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/make-variables.md` & `tuxsuite-1.9.0/docs/tuxbuild/make-variables.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/metadata.md` & `tuxsuite-1.9.0/docs/tuxbuild/metadata.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/patch-series.md` & `tuxsuite-1.9.0/docs/tuxbuild/patch-series.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/subcommands.md` & `tuxsuite-1.9.0/docs/tuxbuild/subcommands.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/target-architectures.md` & `tuxsuite-1.9.0/docs/tuxbuild/target-architectures.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/toolchains.md` & `tuxsuite-1.9.0/docs/tuxbuild/toolchains.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxbuild/tuxmake.md` & `tuxsuite-1.9.0/docs/tuxbuild/tuxmake.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxtest/arguments/device.md` & `tuxsuite-1.9.0/docs/tuxtest/arguments/device.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxtest/arguments/tests.md` & `tuxsuite-1.9.0/docs/tuxtest/arguments/tests.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxtest/features/devices.md` & `tuxsuite-1.9.0/docs/tuxtest/features/devices.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxtest/features/status-result.md` & `tuxsuite-1.9.0/docs/tuxtest/features/status-result.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/docs/tuxtest/subcommands.md` & `tuxsuite-1.9.0/docs/tuxtest/subcommands.md`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/lkft.json` & `tuxsuite-1.9.0/examples/bitbake/lkft.json`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/lt-qcom.json` & `tuxsuite-1.9.0/examples/bitbake/lt-qcom.json`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/mbed.yaml` & `tuxsuite-1.9.0/examples/bitbake/mbed.yaml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/poky-kirkstone-plan.yaml` & `tuxsuite-1.9.0/examples/bitbake/poky-kirkstone-plan.yaml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/poky-next.yaml` & `tuxsuite-1.9.0/examples/bitbake/poky-next.yaml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/sample_bake_plan.yaml` & `tuxsuite-1.9.0/examples/bitbake/sample_bake_plan.yaml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/bitbake/template.json` & `tuxsuite-1.9.0/examples/bitbake/template.json`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/linux-test-plan.yaml` & `tuxsuite-1.9.0/examples/linux-test-plan.yaml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/examples/planv1.yaml` & `tuxsuite-1.9.0/examples/planv1.yaml`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/mkdocs.yml` & `tuxsuite-1.9.0/mkdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -63,20 +63,22 @@
     - Required Arguments:
       - Device: tuxtest/arguments/device.md
       - kernel: tuxtest/arguments/kernel.md
     - Optional Arguments:
       - Tests: tuxtest/arguments/tests.md
       - Timeouts: tuxtest/arguments/timeouts.md
       - No Wait: tuxtest/arguments/no-wait.md
+      - Additional Arguments: tuxtest/arguments/additional-arguments.md
   - Sub-commands: tuxtest/subcommands.md
 - Results:
   - Features:
     - Results: results/features/results.md
   - Arguments:
     - JSON Output: results/arguments/json-out.md
     - From JSON: results/arguments/from-json.md
   - Examples: results/examples.md
 
 - Reference:
   - Python API: python-api.md
+  - Callbacks: callbacks.md
 - Community:
   - Code of Conduct: code-of-conduct.md
```

### Comparing `tuxsuite-1.8.0/scripts/release` & `tuxsuite-1.9.0/scripts/release`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/api_v1.py` & `tuxsuite-1.9.0/test/api_v1.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/conftest.py` & `tuxsuite-1.9.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/integration/test_api_server` & `tuxsuite-1.9.0/test/integration/test_api_server`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/integration/test_helper.sh` & `tuxsuite-1.9.0/test/integration/test_helper.sh`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/integration/test_tuxsuite_build` & `tuxsuite-1.9.0/test/integration/test_tuxsuite_build`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_build.py` & `tuxsuite-1.9.0/test/test_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
             "local_conf": [],
             "targets": [
                 "rpb-console-image rpb-console-image-test rpb-desktop-image rpb-desktop-image-test"
             ],
             "name": "",
             "no_cache": False,
             "is_public": True,
+            "callback": None,
             "bblayers_conf": [],
             "container": bitbake.build_definition.container,
             "manifest_file": None,
             "pinned_manifest": None,
         }
         assert bitbake.generate_build_request() == (expected_data, {})
 
@@ -242,14 +243,15 @@
                 "target": "rpb-console-image rpb-console-image-test rpb-desktop-image rpb-desktop-image-test",
                 "targets": [
                     "rpb-console-image rpb-console-image-test rpb-desktop-image rpb-desktop-image-test"
                 ],
                 "name": "",
                 "no_cache": False,
                 "is_public": True,
+                "callback": None,
                 "artifacts": [],
                 "environment": {},
                 "extraconfigs": [],
                 "local_conf": [],
                 "bblayers_conf": [],
                 "container": bitbake.build_definition.container,
                 "manifests": {},
```

### Comparing `tuxsuite-1.8.0/test/test_cli.py` & `tuxsuite-1.9.0/test/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,15 @@
             make_variables={},
             build_name=None,
             kernel_image=None,
             image_sha=None,
             no_cache=False,
             patch_series=None,
             is_public=True,
+            callback=None,
         )
 
     def test_build_download(self, mocker, monkeypatch, tuxsuite_config):
         build = mocker.patch("tuxsuite.Build")
         download = mocker.patch("tuxsuite.download.download")
         monkeypatch.setattr(
             sys,
@@ -579,14 +580,15 @@
             make_variables={},
             build_name=None,
             kernel_image=None,
             image_sha=None,
             no_cache=False,
             patch_series=None,
             is_public=True,
+            callback=None,
         )
 
     def test_build_no_make_targets(self, mocker, monkeypatch, tuxsuite_config):
         Build = mocker.patch("tuxsuite.Build")
         Build.return_value.build_data = "https://tuxsuite.example.com/abcdef0123456789/"
         monkeypatch.setattr(
             sys,
@@ -616,14 +618,15 @@
             make_variables={},
             build_name=None,
             kernel_image=None,
             image_sha=None,
             no_cache=False,
             patch_series=None,
             is_public=True,
+            callback=None,
         )
 
     def test_build_valid_make_vars(self, mocker, monkeypatch, tuxsuite_config):
         Build = mocker.patch("tuxsuite.Build")
         build = Build.return_value
         monkeypatch.setattr(
             sys,
@@ -693,14 +696,15 @@
             make_variables={},
             build_name=None,
             kernel_image=None,
             image_sha=None,
             no_cache=False,
             patch_series=None,
             is_public=True,
+            callback=None,
         )
 
     def test_build_no_wait(self, mocker, monkeypatch, tuxsuite_config, tmp_path):
         build = mocker.patch("tuxsuite.Build")
         monkeypatch.setattr(
             sys,
             "argv",
@@ -932,14 +936,15 @@
             scp_romfw=None,
             fip=None,
             parameters={},
             tests=[],
             timeouts={},
             boot_args=None,
             wait_for=None,
+            callback=None,
         )
 
         mocker.resetall()
         monkeypatch.setattr(
             sys,
             "argv",
             [
@@ -967,14 +972,15 @@
             scp_romfw=None,
             fip=None,
             parameters={},
             tests=["ltp-smoke"],
             timeouts={},
             boot_args=None,
             wait_for=None,
+            callback=None,
         )
 
         mocker.resetall()
         monkeypatch.setattr(
             sys,
             "argv",
             [
@@ -1001,14 +1007,15 @@
             scp_romfw=None,
             fip=None,
             parameters={},
             tests=["ltp-smoke"],
             timeouts={},
             boot_args=None,
             wait_for="mybuilduid",
+            callback=None,
         )
 
         mocker.resetall()
         monkeypatch.setattr(
             sys,
             "argv",
             [
@@ -1035,14 +1042,15 @@
             scp_romfw=None,
             fip=None,
             parameters={},
             tests=[],
             timeouts={"deploy": 1, "boot": 2},
             boot_args=None,
             wait_for=None,
+            callback=None,
         )
 
         mocker.resetall()
         monkeypatch.setattr(
             sys,
             "argv",
             [
@@ -1077,14 +1085,15 @@
             scp_romfw="scp_romfw.bin",
             fip="fip.bin",
             parameters={"USERDATA": "userdata.tar.xz", "TC_URL": "toolchain.tar.xz"},
             tests=["lldb"],
             timeouts={},
             boot_args=None,
             wait_for=None,
+            callback=None,
         )
 
     def test_test_cli_errors(self, mocker, monkeypatch):
         monkeypatch.setattr(
             sys,
             "argv",
             [
```

### Comparing `tuxsuite-1.8.0/test/test_cli_build_subcommands.py` & `tuxsuite-1.9.0/test/test_cli_build_subcommands.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_cli_group_subcommands.py` & `tuxsuite-1.9.0/test/test_cli_group_subcommands.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_cli_plan_subcommands.py` & `tuxsuite-1.9.0/test/test_cli_plan_subcommands.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_cli_project_subcommands.py` & `tuxsuite-1.9.0/test/test_cli_project_subcommands.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_cli_test_subcommands.py` & `tuxsuite-1.9.0/test/test_cli_test_subcommands.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_cli_utils.py` & `tuxsuite-1.9.0/test/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_config.py` & `tuxsuite-1.9.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_download.py` & `tuxsuite-1.9.0/test/test_download.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_gitutils.py` & `tuxsuite-1.9.0/test/test_gitutils.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_plan.py` & `tuxsuite-1.9.0/test/test_plan.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_requests.py` & `tuxsuite-1.9.0/test/test_requests.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/test/test_tuxsuite.py` & `tuxsuite-1.9.0/test/test_tuxsuite.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite.rst` & `tuxsuite-1.9.0/tuxsuite.rst`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite.spec` & `tuxsuite-1.9.0/tuxsuite.spec`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxsuite
-Version:   1.8.0
+Version:   1.9.0
 Release:   0%{?dist}
 Summary:   TuxSuite, helps with Linux kernel development
 License:   Expat
 URL:       https://tuxsuite.com
 Source0:   %{pypi_source}
```

### Comparing `tuxsuite-1.8.0/tuxsuite/__init__.py` & `tuxsuite-1.9.0/tuxsuite/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 
 """
 This is the tuxsuite module.
 """
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 
 from . import build
 from . import config
 from . import schema, exceptions
 
 from abc import ABC, abstractmethod
```

### Comparing `tuxsuite-1.8.0/tuxsuite/build.py` & `tuxsuite-1.9.0/tuxsuite/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,15 @@
     build_name = attrib(default=None)
     status = attrib(default={})
     uid = attrib(default=None)
     json = attrib(default=False)
     limit = attrib(default=0)
     no_cache = attrib(default=False)
     is_public = attrib(default=True)
+    callback = attrib(default=None)
 
     def __attrs_post_init__(self):
         if isinstance(self.kconfig, str):
             self.kconfig = [self.kconfig]
         self.verify_build_parameters()
         self.client_token = str(uuid.uuid4())
 
@@ -300,14 +301,16 @@
             build_entry["no_cache"] = self.no_cache
         if self.patch_series:
             (
                 build_entry["kernel_patch_file"],
                 kernel_patch,
             ) = handle_patch(self.patch_series)
             patch[build_entry["kernel_patch_file"]] = kernel_patch
+        if self.callback is not None:
+            build_entry["callback"] = self.callback
         return (build_entry, patch)
 
     def verify_build_parameters(self):
         """Pre-check the build arguments"""
         assert self.git_repo, "git_repo is mandatory\n"
         assert self.is_supported_git_url(
             self.git_repo
@@ -570,14 +573,15 @@
                             boot_args=test.get("boot_args"),
                             device=test["device"],
                             dtb=test.get("dtb"),
                             parameters=test.get("parameters", {}),
                             rootfs=test.get("rootfs"),
                             tests=test.get("tests", []),
                             timeouts=test.get("timeouts"),
+                            callback=test.get("callback"),
                             wait_for=build.uid,
                         )
                     )
                 self.builds.append(build)
             else:
                 for test in cfg["tests"]:
                     tests.append(
@@ -599,14 +603,15 @@
                             modules=test.get("modules"),
                             parameters=test.get("parameters", {}),
                             rootfs=test.get("rootfs"),
                             scp_fw=test.get("scp_fw"),
                             scp_romfw=test.get("scp_romfw"),
                             tests=test.get("tests", []),
                             timeouts=test.get("timeouts"),
+                            callback=test.get("callback"),
                         )
                     )
 
         if tests:
             ret = []
             # submit in batches of 500 to prevent tuxapi lambda time out
             for i in range(0, len(tests), 500):
@@ -887,14 +892,15 @@
     modules = attrib(default=None)
     parameters = attrib(default=[])
     rootfs = attrib(default=None)
     scp_fw = attrib(default=None)
     scp_romfw = attrib(default=None)
     tests = attrib(default=[])
     timeouts = attrib(default=[])
+    callback = attrib(default=None)
 
     uid = attrib(default=None)
     wait_for = attrib(default=None)
     status = attrib(default={})
     url = attrib(default=None)
 
     def __str__(self):
@@ -925,14 +931,16 @@
             data["tests"] = self.tests
         if self.timeouts:
             data["timeouts"] = self.timeouts
         if self.boot_args:
             data["boot_args"] = self.boot_args
         if self.wait_for:
             data["waiting_for"] = self.wait_for
+        if self.callback:
+            data["callback"] = self.callback
         if plan is not None:
             data["plan"] = plan
 
         return data
 
     def test(self, plan=None):
         url = self.tuxapi_url + "/v1/groups/{}/projects/{}/tests".format(
@@ -1135,14 +1143,15 @@
         container = attrib(default="ubuntu-20.04")
         manifest_file = attrib(default=None)
         name = attrib(default="")
         no_cache = attrib(default=False)
         extraconfigs = attrib(default=[])
         pinned_manifest = attrib(default=None)
         is_public = attrib(default=True)
+        callback = attrib(default=None)
 
     def __attrs_post_init__(self):
         self.build_definition = self.BuildDefinition(**(self.data))
         # TODO: Temp legacy target fixes, to be removed after we deprecate target
         try:
             if (
                 self.build_definition.targets is None
```

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/__init__.py` & `tuxsuite-1.9.0/tuxsuite/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/bake.py` & `tuxsuite-1.9.0/tuxsuite/cli/bake.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from tuxsuite.cli.requests import post
 from tuxsuite.cli.utils import (
     error,
     file_or_url,
     format_result,
     wait_for_object,
+    is_url,
 )
 
 
 def handle_submit(cmdargs, _, config):
     build_definition = cmdargs.build_definition[0]
     try:
         with open(os.path.abspath(build_definition)) as reader:
@@ -30,14 +31,15 @@
         error("Either local manifest or pinned manifest to be provided, not both")
     else:
         # either one will be present
         data["manifest_file"] = cmdargs.local_manifest
         data["pinned_manifest"] = cmdargs.pinned_manifest
     data["no_cache"] = cmdargs.no_cache
     data["is_public"] = cmdargs.private
+    data["callback"] = cmdargs.callback
 
     try:
         build = tuxsuite.Bitbake(data=data)
     except (AssertionError, tuxsuite.exceptions.TuxSuiteError) as e:
         error(e)
     print(
         "Building targets: {} with bitbake from {} source with distro: {} machine: {} arguments".format(
@@ -148,14 +150,23 @@
     )
     sp.add_argument(
         "-P",
         "--private",
         action="store_false",
         help="Private build",
     )
+    sp.add_argument(
+        "--callback",
+        default=None,
+        help=(
+            "Callback URL. The bake backend will send a POST request to "
+            "this URL with signed data, when bake completes."
+        ),
+        type=is_url,
+    )
 
 
 def setup_parser(parser):
     # "bake submit"
     t = parser.add_parser("submit")
     t.add_argument(
         "build_definition",
```

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/build.py` & `tuxsuite-1.9.0/tuxsuite/cli/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     datediff,
     fetch_next,
     key_value,
     wait_for_object,
     error,
     format_result,
     show_log,
+    is_url,
 )
 
 import json
 import requests
 import sys
 import time
 
@@ -310,14 +311,15 @@
             make_variables=make_variables,
             kernel_image=cmdargs.kernel_image,
             patch_series=cmdargs.patch_series,
             image_sha=cmdargs.image_sha,
             build_name=cmdargs.build_name,
             no_cache=cmdargs.no_cache,
             is_public=cmdargs.private,
+            callback=cmdargs.callback,
         )
 
     except (AssertionError, tuxsuite.exceptions.TuxSuiteError) as e:
         error(e)
     print(
         "Building Linux Kernel {} at {}".format(
             build.git_repo, build.git_ref or build.git_sha
@@ -444,14 +446,24 @@
         help="Target architecture [arc|arm|arm64|hexagon|i386|mips|parisc|powerpc|riscv|s390|sh|sparc|x86_64]",
     )
     sp.add_argument(
         "--image-sha",
         default=None,
         help="Pin the container image sha (64 hexadecimal digits)",
     )
+    sp.add_argument(
+        "--callback",
+        default=None,
+        help=(
+            "Callback URL. The kernel build backend will send a POST "
+            "request to this URL with signed data, when the kernel "
+            "build completes."
+        ),
+        type=is_url,
+    )
 
 
 def setup_parser(parser):
     # "build config <uid>"
     t = parser.add_parser("config")
     t.add_argument("uid")
```

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/colors.py` & `tuxsuite-1.9.0/tuxsuite/cli/colors.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/common.py` & `tuxsuite-1.9.0/tuxsuite/cli/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,10 +62,11 @@
         default=False,
         action="store_true",
         help="Build without using any compilation cache",
     )
     sp.add_argument(
         "-P",
         "--private",
+        default=True,
         action="store_false",
         help="Private build",
     )
```

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/group.py` & `tuxsuite-1.9.0/tuxsuite/cli/group.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/models.py` & `tuxsuite-1.9.0/tuxsuite/cli/models.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/plan.py` & `tuxsuite-1.9.0/tuxsuite/cli/plan.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/project.py` & `tuxsuite-1.9.0/tuxsuite/cli/project.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/requests.py` & `tuxsuite-1.9.0/tuxsuite/cli/requests.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/results.py` & `tuxsuite-1.9.0/tuxsuite/cli/results.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/test.py` & `tuxsuite-1.9.0/tuxsuite/cli/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     LIMIT,
     datediff,
     fetch_next,
     key_value,
     wait_for_object,
     format_result,
     error,
+    is_url,
 )
 from tuxsuite.cli.yaml import yaml_load
 
 import json
 import sys
 import time
 
@@ -309,14 +310,15 @@
             parameters=params,
             rootfs=cmdargs.rootfs,
             scp_fw=cmdargs.scp_fw,
             scp_romfw=cmdargs.scp_romfw,
             tests=tests,
             timeouts=timeouts_d,
             wait_for=cmdargs.wait_for,
+            callback=cmdargs.callback,
         )
     except (AssertionError, tuxsuite.exceptions.TuxSuiteError) as e:
         error(e)
 
     try:
         test.test()
         print("uid: {}".format(test.uid))
@@ -456,14 +458,23 @@
         help="Don't wait for tests to finish",
     )
     sp.add_argument(
         "--json-out",
         help="Write json test status out to a named file path",
         type=argparse.FileType("w", encoding="utf-8"),
     )
+    sp.add_argument(
+        "--callback",
+        default=None,
+        help=(
+            "Callback URL. The test backend will send a POST request "
+            "to this URL with signed data, when the test completes."
+        ),
+        type=is_url,
+    )
 
 
 def setup_parser(parser):
     # "test get <uid>"
     t = parser.add_parser("get")
     t.add_argument("uid")
     t.add_argument("--json", action="store_true")
```

### Comparing `tuxsuite-1.8.0/tuxsuite/cli/utils.py` & `tuxsuite-1.9.0/tuxsuite/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,21 @@
     if urlparse(path).scheme in ["http", "https"]:
         return path
     elif os.path.exists(path):
         return path
     error(f"{path} does not exist or invalid")
 
 
+def is_url(path):
+    """Validate if path is an URL"""
+    if urlparse(path).scheme in ["http", "https"]:
+        return path
+    error(f"{path} is not a valid http(s) url")
+
+
 def wait_for_object(build_object):
     result = True
     for state in build_object.watch():
         print_state(state)
         if state.status in ["error", "fail"] or state.state == "error" and state.final:
             result = False
     return result
```

### Comparing `tuxsuite-1.8.0/tuxsuite/config.py` & `tuxsuite-1.9.0/tuxsuite/config.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/download.py` & `tuxsuite-1.9.0/tuxsuite/download.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/exceptions.py` & `tuxsuite-1.9.0/tuxsuite/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/gitutils.py` & `tuxsuite-1.9.0/tuxsuite/gitutils.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/requests.py` & `tuxsuite-1.9.0/tuxsuite/requests.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/schema.py` & `tuxsuite-1.9.0/tuxsuite/schema.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite/utils.py` & `tuxsuite-1.9.0/tuxsuite/utils.py`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/tuxsuite_logo.png` & `tuxsuite-1.9.0/tuxsuite_logo.png`

 * *Files identical despite different names*

### Comparing `tuxsuite-1.8.0/setup.py` & `tuxsuite-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['attrs', 'Click', 'requests', 'pyyaml', 'voluptuous', 'b4']
 
 entry_points = \
 {'console_scripts': ['tuxsuite = tuxsuite.cli:main']}
 
 setup(name='tuxsuite',
-      version='1.8.0',
+      version='1.9.0',
       description='This is the tuxsuite module.',
       author='Senthil Kumaran',
       author_email='senthil.kumaran@linaro.org',
       url='https://www.tuxsuite.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

