# Comparing `tmp/ansys-templates-0.6.0.tar.gz` & `tmp/ansys-templates-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-templates-0.6.0.tar", last modified: Tue Apr 18 16:04:14 2023, max compression
+gzip compressed data, was "ansys-templates-0.7.0.tar", last modified: Wed May  3 06:16:19 2023, max compression
```

## Comparing `ansys-templates-0.6.0.tar` & `ansys-templates-0.7.0.tar`

### file list

```diff
@@ -1,194 +1,252 @@
--rw-r--r--   0        0        0     1091 2023-04-18 16:04:01.152234 ansys-templates-0.6.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9732 2023-04-18 16:04:01.152234 ansys-templates-0.6.0/README.rst
--rw-r--r--   0        0        0     3132 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2271 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3563 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3558 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3729 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2779 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      282 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4078 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3414 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       81 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2377 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1087 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3238 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2903 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3070 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3055 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2831 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1110 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3398 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2619 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6537 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1010 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1035 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3170 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0      994 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     2840 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      283 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     4828 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3060 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     8371 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3351 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3825 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    34868 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       52 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      916 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0     9913 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0   749872 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png
--rw-r--r--   0        0        0      121 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
--rw-r--r--   0        0        0     2030 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py
--rw-r--r--   0        0        0     4695 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py
--rw-r--r--   0        0        0     5241 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
--rw-r--r--   0        0        0      593 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py
--rw-r--r--   0        0        0       20 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11220 1970-01-01 00:00:00.000000 ansys-templates-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0    10173 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/README.rst
+-rw-r--r--   0        0        0     3132 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2331 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3680 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3738 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3729 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      282 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4078 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-05-03 06:16:04.903525 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1444 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     4461 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      283 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     4821 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3052 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     7565 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3351 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     4375 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38829 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       47 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       46 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       47 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      959 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0    10360 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    10623 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      916 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0     9913 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0      756 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
+-rw-r--r--   0        0        0      585 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/colorscale.py
+-rw-r--r--   0        0        0    16026 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_page.py
+-rw-r--r--   0        0        0     2533 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/design_table_page.py
+-rw-r--r--   0        0        0     5572 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/project_summary_page.py
+-rw-r--r--   0        0        0      647 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/result_files_page.py
+-rw-r--r--   0        0        0      870 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/scenery_page.py
+-rw-r--r--   0        0        0     1596 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/status_overview_page.py
+-rw-r--r--   0        0        0     4962 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/summary_page.py
+-rw-r--r--   0        0        0    12146 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/visualization_page.py
+-rw-r--r--   0        0        0     5165 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
+-rw-r--r--   0        0        0    11886 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/problem_setup_page.py
+-rw-r--r--   0        0        0       20 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1429 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2903 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3070 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-05-03 06:16:04.907526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3055 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2831 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1110 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2619 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1010 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1035 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      994 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     2840 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      283 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     4828 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3060 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     8363 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3351 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3729 2023-05-03 06:16:04.911526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    34868 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       52 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      916 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0     9913 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0   749872 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png
+-rw-r--r--   0        0        0      121 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
+-rw-r--r--   0        0        0     2030 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py
+-rw-r--r--   0        0        0     4695 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py
+-rw-r--r--   0        0        0     5241 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
+-rw-r--r--   0        0        0      593 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py
+-rw-r--r--   0        0        0       20 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-05-03 06:16:04.915526 ansys-templates-0.7.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11661 1970-01-01 00:00:00.000000 ansys-templates-0.7.0/PKG-INFO
```

### Comparing `ansys-templates-0.6.0/LICENSES/MIT.txt` & `ansys-templates-0.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/README.rst` & `ansys-templates-0.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
 
 Available templates
 -------------------
 Available templates in ``ansys-templates`` are:
 
 - ``doc-project``: Create a documentation project using Sphinx.
+- ``osl-solution``: Create an optiSLang Solution based on the Solution Application Framework.
 - ``pybasic``: Create a basic Python Package.
 - ``pyansys``: Create a PyAnsys Python Package project.
 - ``pyansys-advanced``: Create an advanced PyAnsys Python Package project.
 - ``pyansys-openapi-client``: Create an OpenAPI Client Package project.
 - ``pyace``: Create a Python project for any method developers.
 - ``pyace-flask``: Create a Flask project initialized for any developer.
 - ``pyace-grpc``: Create gRPC project initialized for any developer.
@@ -138,15 +139,16 @@
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-flask             |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-grpc              |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | solution                |                       |  ``X``          |  ``X``  |  ``X``   |  ``X``         |         |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
-
+| osl-solution            |                       |  ``X``          |  ``X``  |  ``X``   |  ``X``         |         |
++-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 
 Demo branches
 -------------
 To have a better idea on how each template will look once it gets rendered, see
 its corresponding demonstration branch.
 
 * Demo branch for `doc-project`_
@@ -156,20 +158,22 @@
 * Demo branch for `pyansys-advanced using poetry`_
 * Demo branch for `pyansys-advanced using setuptools`_
 * Demo branch for `pyace`_
 * Demo branch for `pyace-fast`_
 * Demo branch for `pyace-flask`_
 * Demo branch for `pyace-grpc`_
 * Demo branch for `solution`_
+* Demo branch for `osl-solution`_
 
 
 .. _doc-project: https://github.com/ansys/ansys-templates/tree/demo/doc-project
 .. _pybasic: https://github.com/ansys/ansys-templates/tree/demo/pybasic
 .. _pyansys: https://github.com/ansys/ansys-templates/tree/demo/pyansys
 .. _pyansys-advanced using flit: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-flit
 .. _pyansys-advanced using poetry: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-poetry
 .. _pyansys-advanced using setuptools: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-setuptools
 .. _pyace: https://github.com/ansys/ansys-templates/tree/demo/pyace-pkg
 .. _pyace-fast: https://github.com/ansys/ansys-templates/tree/demo/pyace-fast
 .. _pyace-flask: https://github.com/ansys/ansys-templates/tree/demo/pyace-flask
 .. _pyace-grpc: https://github.com/ansys/ansys-templates/tree/demo/pyace-grpc
 .. _solution: https://github.com/ansys/ansys-templates/tree/demo/solution
+.. _osl-solution: https://github.com/ansys/ansys-templates/tree/demo/solution
```

### Comparing `ansys-templates-0.6.0/pyproject.toml` & `ansys-templates-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "0.6.0"
+version = "0.7.0"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -58,17 +58,17 @@
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
 ]
 doc = [
-    "ansys-sphinx-theme==0.9.7",
+    "ansys-sphinx-theme==0.9.8",
     "numpydoc==1.5.0",
-    "sphinx==5.3.0",
+    "sphinx==6.2.1",
     "sphinx-copybutton==0.5.2",
 ]
 
 [tool.flit.module]
 name = "ansys.templates"
 
 [project.scripts]
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/__init__.py` & `ansys-templates-0.7.0/src/ansys/templates/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 except ModuleNotFoundError:
     import importlib_metadata
 
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 AVAILABLE_TEMPLATES_AND_DESCRIPTION = {
     "doc-project": "Create a documentation project using Sphinx.",
+    "osl-solution": "Create an oSL solution based on SAF.",
     "pybasic": "Create a basic Python Package.",
     "pyansys": "Create a PyAnsys Python Package project.",
     "pyansys-advanced": "Create an advanced PyAnsys Python Package project.",
     "pyansys-openapi_client": "Create an OpenAPI Client Package project.",
     "pyace": "Create a Python project for any method developers.",
     "pyace-flask": "Create a Flask project initialized for any developer.",
     "pyace-grpc": "Create gRPC project initialized for any developer.",
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/__main__.py` & `ansys-templates-0.7.0/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/cli.py` & `ansys-templates-0.7.0/src/ansys/templates/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,7 +122,12 @@
     """Create gRPC project initialized for any developer."""
     create_project("pyace-grpc")
 
 @new.command()
 def solution():
     """Create a Solution based on the Solution Application Framework."""
     create_project("solution")
+
+@new.command()
+def osl_solution():
+    """Create an oSL solution based on SAF."""
+    create_project("osl-solution")
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/licenses/LICENSE_MIT` & `ansys-templates-0.7.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/paths.py` & `ansys-templates-0.7.0/src/ansys/templates/paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,21 @@
 
 PYTHON_TEMPLATES_PYACE_FAST_PATH = PYTHON_TEMPLATES_PATH / "pyace_fastapi"
 """Path to the FastAPI based Python Project template."""
 
 PYTHON_TEMPLATES_SOLUTION_PATH = PYTHON_TEMPLATES_PATH / "solution"
 """Path to the Solution template."""
 
+PYTHON_TEMPLATES_OSL_SOLUTION_PATH = PYTHON_TEMPLATES_PATH / "osl_solution"
+"""Path to the optiSLang Solution template."""
+
 TEMPLATE_PATH_FINDER = {
     "common": PYTHON_TEMPLATES_COMMON_PATH,
     "doc-project": PYTHON_TEMPLATES_DOC_PROJECT,
+    "osl-solution": PYTHON_TEMPLATES_OSL_SOLUTION_PATH,
     "pybasic": PYTHON_TEMPLATES_PYBASIC_PATH,
     "pyansys": PYTHON_TEMPLATES_PYANSYS_PATH,
     "pyansys-advanced": PYTHON_TEMPLATES_PYANSYS_ADVANCED_PATH,
     "pyansys-openapi-client": PYTHON_TEMPLATES_PYANSYS_OPENAPI_CLIENT_PATH,
     "pyace": PYTHON_TEMPLATES_PYACE_PATH,
     "pyace-grpc": PYTHON_TEMPLATES_PYACE_GRPC_PATH,
     "pyace-flask": PYTHON_TEMPLATES_PYACE_FLASK_PATH,
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys-templates-0.7.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys-templates-0.7.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys-templates-0.7.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.7.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys-templates-0.7.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/cookiecutter.json` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'__requires_python'": "'3.8'"}*

```diff
@@ -7,15 +7,15 @@
     "__logo_color": "black",
     "__max_linelength": "120",
     "__pkg_name": "ansys-solutions-{{ cookiecutter.solution_name.lower().replace('_', '-') }}",
     "__pkg_namespace": "ansys.solutions.{{ cookiecutter.__project_name_slug }}",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.project_name.lower().replace('_', '-') }}",
     "__repository_url": "",
-    "__requires_python": "3.7",
+    "__requires_python": "3.8",
     "__short_description": "",
     "__solution_definition_name": "{{ cookiecutter.__solution_name_slug.title() }}Solution",
     "__solution_name_slug": "{{ cookiecutter.solution_name.lower().replace('-', '_') }}",
     "__template_name": "solution",
     "__version": "0.1.dev0",
     "_copy_without_render": [
         "*.html"
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,14 @@
 
   .. code:: bash
 
     python -m codespell .
 
 
 Testing
-=======
 
 **Unit tests** and **Integration tests** are executed via the ``pytest`` framework.
 
 To run the unit tests:
 
   .. code:: bash
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,20 @@
 
 # Main dependencies
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
 ansys-saf-glow = {version = "^0.2.0", source = "solutions-private-pypi" }
 ansys-saf-portal = {version = "^0.1.6", source = "solutions-private-pypi"}
-toml = {version = "^0.10.0"} # supports python versions until 3.9
 {% if cookiecutter.with_dash_ui == "yes" %}
 dash = {version = "^2.6"}
 dash_bootstrap_components = {version = "^1.2"}
 dash-extensions = {version = "^0.1"}
 dash-iconify = {version = "^0.1"}
 dash-uploader = {version = "^0.6"}
-packaging = {version = "^23"}
 {% endif %}
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 [tool.poetry.group.doc.dependencies]
 ansys-sphinx-theme = {version = "^0.8.0"}
```

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys-templates-0.7.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys-templates-0.7.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/testing.py` & `ansys-templates-0.7.0/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/src/ansys/templates/utils.py` & `ansys-templates-0.7.0/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.6.0/PKG-INFO` & `ansys-templates-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 0.6.0
+Version: 0.7.0
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: click>=7.0,<8.0.0
 Requires-Dist: cookiecutter>=2.1.0
 Requires-Dist: isort>=5.10.1
-Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: sphinx==5.3.0 ; extra == "doc"
+Requires-Dist: sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
 Project-URL: Source, https://github.com/ansys-templates/ansys-templates
 Project-URL: Tracker, https://github.com/ansys/ansys-templates/issues
@@ -133,14 +133,15 @@
 
 
 Available templates
 -------------------
 Available templates in ``ansys-templates`` are:
 
 - ``doc-project``: Create a documentation project using Sphinx.
+- ``osl-solution``: Create an optiSLang Solution based on the Solution Application Framework.
 - ``pybasic``: Create a basic Python Package.
 - ``pyansys``: Create a PyAnsys Python Package project.
 - ``pyansys-advanced``: Create an advanced PyAnsys Python Package project.
 - ``pyansys-openapi-client``: Create an OpenAPI Client Package project.
 - ``pyace``: Create a Python project for any method developers.
 - ``pyace-flask``: Create a Flask project initialized for any developer.
 - ``pyace-grpc``: Create gRPC project initialized for any developer.
@@ -172,15 +173,16 @@
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-flask             |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-grpc              |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | solution                |                       |  ``X``          |  ``X``  |  ``X``   |  ``X``         |         |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
-
+| osl-solution            |                       |  ``X``          |  ``X``  |  ``X``   |  ``X``         |         |
++-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 
 Demo branches
 -------------
 To have a better idea on how each template will look once it gets rendered, see
 its corresponding demonstration branch.
 
 * Demo branch for `doc-project`_
@@ -190,21 +192,23 @@
 * Demo branch for `pyansys-advanced using poetry`_
 * Demo branch for `pyansys-advanced using setuptools`_
 * Demo branch for `pyace`_
 * Demo branch for `pyace-fast`_
 * Demo branch for `pyace-flask`_
 * Demo branch for `pyace-grpc`_
 * Demo branch for `solution`_
+* Demo branch for `osl-solution`_
 
 
 .. _doc-project: https://github.com/ansys/ansys-templates/tree/demo/doc-project
 .. _pybasic: https://github.com/ansys/ansys-templates/tree/demo/pybasic
 .. _pyansys: https://github.com/ansys/ansys-templates/tree/demo/pyansys
 .. _pyansys-advanced using flit: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-flit
 .. _pyansys-advanced using poetry: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-poetry
 .. _pyansys-advanced using setuptools: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-setuptools
 .. _pyace: https://github.com/ansys/ansys-templates/tree/demo/pyace-pkg
 .. _pyace-fast: https://github.com/ansys/ansys-templates/tree/demo/pyace-fast
 .. _pyace-flask: https://github.com/ansys/ansys-templates/tree/demo/pyace-flask
 .. _pyace-grpc: https://github.com/ansys/ansys-templates/tree/demo/pyace-grpc
 .. _solution: https://github.com/ansys/ansys-templates/tree/demo/solution
+.. _osl-solution: https://github.com/ansys/ansys-templates/tree/demo/solution
```

