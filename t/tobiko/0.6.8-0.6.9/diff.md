# Comparing `tmp/tobiko-0.6.8.tar.gz` & `tmp/tobiko-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tobiko-0.6.8.tar", last modified: Thu Mar 30 08:14:31 2023, max compression
+gzip compressed data, was "tobiko-0.6.9.tar", last modified: Wed May  3 08:00:34 2023, max compression
```

## Comparing `tobiko-0.6.8.tar` & `tobiko-0.6.9.tar`

### file list

```diff
@@ -1,919 +1,960 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.529365 tobiko-0.6.8/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-03-30 08:13:54.000000 tobiko-0.6.8/.ansible-lint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-03-30 08:13:54.000000 tobiko-0.6.8/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-03-30 08:13:54.000000 tobiko-0.6.8/.dockerignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1834 2023-03-30 08:13:54.000000 tobiko-0.6.8/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27759 2023-03-30 08:13:54.000000 tobiko-0.6.8/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-03-30 08:13:54.000000 tobiko-0.6.8/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2023-03-30 08:14:31.000000 tobiko-0.6.8/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    96754 2023-03-30 08:14:31.000000 tobiko-0.6.8/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2023-03-30 08:13:54.000000 tobiko-0.6.8/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-03-30 08:13:54.000000 tobiko-0.6.8/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5607 2023-03-30 08:14:31.529365 tobiko-0.6.8/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-03-30 08:13:54.000000 tobiko-0.6.8/Pipfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3881 2023-03-30 08:13:54.000000 tobiko-0.6.8/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-03-30 08:13:54.000000 tobiko-0.6.8/ansible.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2023-03-30 08:13:54.000000 tobiko-0.6.8/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.445365 tobiko-0.6.8/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/readthedocs_requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.445365 tobiko-0.6.8/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.445365 tobiko-0.6.8/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11492 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/_static/tobiko.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11492 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/_static/tobiko.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4082 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/content.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.445365 tobiko-0.6.8/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6527 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/contributor/Vagrantfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11779 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/contributor/contributor.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2500 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/contributor/reviewer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1980 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/contributor/setup_tobiko_workstation.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.445365 tobiko-0.6.8/doc/source/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/etc/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/etc/tobiko.conf.gen
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/etc/tobiko.conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/doc/source/miscellaneous/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/miscellaneous/from-tempest-to-tobiko.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/miscellaneous/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4156 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_conf_credentials.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_conf_explanation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_conf_logging.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_conf_venv_with_tox.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_install_venv.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_run_faults.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_run_scenario.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_run_specific_tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_run_workflow.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_skip_resources_creation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/_test_cases_report_files.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/quick-start.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2023-03-30 08:13:54.000000 tobiko-0.6.8/doc/source/user/run-test-cases.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-03-30 08:13:54.000000 tobiko-0.6.8/docker-compose.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-03-30 08:13:54.000000 tobiko-0.6.8/etc/README.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11492 2023-03-30 08:13:54.000000 tobiko-0.6.8/etc/tobiko.conf.example
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-03-30 08:13:54.000000 tobiko-0.6.8/extra-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/plugin.spec
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/infrared_plugin/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-before-run/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-before-run/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-before-run/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-before-run/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-before-run/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-deploy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-deploy/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-deploy/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-deploy/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-deploy/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-init/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-init/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-init/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-jenkins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-jenkins/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-jenkins/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.449365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-jenkins/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-jenkins/vars/jenkins.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2928 2023-03-30 08:13:54.000000 tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-03-30 08:13:54.000000 tobiko-0.6.8/linters-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-03-30 08:13:54.000000 tobiko-0.6.8/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-03-30 08:13:54.000000 tobiko-0.6.8/mypy.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/playbooks/docker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/docker/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/docker/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/docker/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/playbooks/infrared/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/infrared/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/infrared/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/playbooks/tripleo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/tripleo/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/tripleo/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/tripleo/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/playbooks/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-03-30 08:13:54.000000 tobiko-0.6.8/playbooks/unit/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-03-30 08:13:54.000000 tobiko-0.6.8/pytest.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.425365 tobiko-0.6.8/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/notes/Added-parser-for-`ss`-command-ac426b522eb8adbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/notes/Added-support-for-metalsmith-00b9f808c1030236.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6127 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-03-30 08:13:54.000000 tobiko-0.6.8/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2023-03-30 08:13:54.000000 tobiko-0.6.8/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.433365 tobiko-0.6.8/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/roles/multi-node-setup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/multi-node-setup/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/roles/multi-node-setup/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/multi-node-setup/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/roles/multi-node-setup/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/multi-node-setup/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.453365 tobiko-0.6.8/roles/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4773 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tests/Vagrantfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tests/ansible.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2980 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tests/provision.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tests/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tests/templates/hosts.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tests/templates/ssh_config.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1786 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tests/test_infrared_plugin.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-bindep/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-bindep/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-bindep/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-bindep/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-bindep/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-bindep/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-bindep/tasks/ensure-bindep.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-bindep/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-check-collected-files/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-check-collected-files/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-check-collected-files/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-check-collected-files/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-check-collected-files/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-cleanup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-cleanup/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-cleanup/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-cleanup/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-cleanup/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-collect/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-collect/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-collect/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-collect/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-collect/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-collect/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-collect/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-collect-report/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-collect-report/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-collect-report/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-collect-report/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-collect-report/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-common/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-common/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2063 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-common/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-compile-python/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3604 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/Vagrantfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/ansible.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-compile-python/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/defaults/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/resolv_conf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-compile-python/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/tasks/setup_pip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3264 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/tasks/setup_python.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-compile-python/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/tests/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1975 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-compile-python/tests/test_py38.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-configure/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-configure/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-configure/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-configure/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-configure/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-configure/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-configure/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-copy-resolv-conf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-copy-resolv-conf/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-copy-resolv-conf/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-copy-resolv-conf/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-copy-resolv-conf/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.457365 tobiko-0.6.8/roles/tobiko-devstack/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-devstack/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-devstack/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/deploy-devstack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/deploy-tobiko.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/ensure-stack-user.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/install-bindeps.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/run-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-devstack/tasks/run-unstack.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-docker-compose/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-docker-compose/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-docker-compose/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-docker-compose/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-docker-compose/tasks/build.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-docker-compose/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-docker-compose/tasks/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-download-images/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-download-images/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-download-images/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-download-images/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-download-images/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-ensure-docker-compose/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-docker-compose/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-docker-compose/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-docker-compose/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-docker-compose/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-ensure-python3/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-python3/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-python3/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3899 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/files/get_python_info.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-python3/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/ensure-python3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1860 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/install.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/platform.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-CentOS-7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-Fedora-31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-Fedora.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-MacOSX.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-RedHat-7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-RedHat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-Ubuntu-18.04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/py3-Ubuntu.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-python3/vars/rhosp-RedHat-7.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-ensure-ssh-keys/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-ssh-keys/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-ssh-keys/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-ssh-keys/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-ssh-keys/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-ensure-tox/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.461365 tobiko-0.6.8/roles/tobiko-ensure-tox/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-tox/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-ensure-tox/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-tox/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-ensure-tox/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-tox/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-ensure-tox/tasks/tox.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.429365 tobiko-0.6.8/roles/tobiko-fixup-stuff/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-fixup-stuff/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-fixup-stuff/tasks/centos.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-fixup-stuff/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.433365 tobiko-0.6.8/roles/tobiko-inventory/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-inventory/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-inventory/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-inventory/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-inventory/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/templates/test_inventory.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-inventory/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/vars/test-inventory-CentOS-7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/vars/test-inventory-Fedora.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/vars/test-inventory-RedHat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-inventory/vars/test-inventory-Ubuntu.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.433365 tobiko-0.6.8/roles/tobiko-redhat-subscription/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-redhat-subscription/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-redhat-subscription/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-redhat-subscription/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-redhat-subscription/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.433365 tobiko-0.6.8/roles/tobiko-run/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-run/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-run/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.465365 tobiko-0.6.8/roles/tobiko-run/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/tasks/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/roles/tobiko-run/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-designate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-faults.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-heat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-nova.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-octavia.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-ovn-migration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-designate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-faults.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-heat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-nova.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-octavia.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources-ovn-migration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-create-resources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-default.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-designate-faults.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-faults-iha.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-faults-neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-faults.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-functional.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-gate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-minimal.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-octavia-faults.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-sanity-shiftstack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-sanity.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-unit.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.433365 tobiko-0.6.8/roles/tobiko-tox/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/roles/tobiko-tox/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-tox/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/roles/tobiko-tox/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-tox/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/roles/tobiko-tox/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-tox/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-tox/tasks/tox.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.433365 tobiko-0.6.8/roles/tobiko-zuul/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/roles/tobiko-zuul/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-zuul/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/roles/tobiko-zuul/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-03-30 08:13:54.000000 tobiko-0.6.8/roles/tobiko-zuul/vars/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-03-30 08:14:31.529365 tobiko-0.6.8/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2023-03-30 08:13:54.000000 tobiko-0.6.8/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-30 08:13:54.000000 tobiko-0.6.8/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/tobiko/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5793 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.473365 tobiko-0.6.8/tobiko/actors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/actors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9703 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/actors/_actor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2660 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/actors/_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5351 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/actors/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/actors/_request.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.473365 tobiko-0.6.8/tobiko/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16453 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_background.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4054 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_cached.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12491 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_case.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_deprecation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4278 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_detail.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5031 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19992 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_ini.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6879 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_operation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1922 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_os.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10255 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4153 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_select.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5571 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_shelves.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5553 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_skip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1818 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2806 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/common/_yaml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12789 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.473365 tobiko-0.6.8/tobiko/docker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/docker/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8778 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/docker/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/docker/_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4463 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/docker/_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/docker/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.477365 tobiko-0.6.8/tobiko/http/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/http/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/http/_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/http/_session.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.477365 tobiko-0.6.8/tobiko/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2375 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.477365 tobiko-0.6.8/tobiko/openstack/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/designate/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/designate/_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/designate/_zone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.477365 tobiko-0.6.8/tobiko/openstack/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/glance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/glance/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18476 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/glance/_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/glance/_io.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/glance/_lzma.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2978 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/glance/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.477365 tobiko-0.6.8/tobiko/openstack/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/heat/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/heat/_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27203 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/heat/_stack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4394 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/heat/_template.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.477365 tobiko-0.6.8/tobiko/openstack/ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/ironic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/ironic/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5396 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/ironic/_node.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.481365 tobiko-0.6.8/tobiko/openstack/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6280 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8837 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/_clouds_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14543 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/_credentials.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6988 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/keystone/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.481365 tobiko-0.6.8/tobiko/openstack/metalsmith/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/metalsmith/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2623 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/metalsmith/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/metalsmith/_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.481365 tobiko-0.6.8/tobiko/openstack/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6276 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6150 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4283 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_cidr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2231 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3701 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8807 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5033 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_quota_set.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_security_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5313 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/neutron/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.481365 tobiko-0.6.8/tobiko/openstack/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3687 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16960 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8975 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_cloud_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2574 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_hypervisor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_key_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5343 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_quota_set.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4183 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2686 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/nova/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.485365 tobiko-0.6.8/tobiko/openstack/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3113 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9191 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_amphora.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2730 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3678 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/_waiters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/octavia/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.485365 tobiko-0.6.8/tobiko/openstack/openstackclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2971 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_security_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_security_group_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1769 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/openstackclient/_subnet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.485365 tobiko-0.6.8/tobiko/openstack/stacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6259 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2821 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_centos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_cirros.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_designate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_fedora.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_hot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_l3ha.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31677 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19596 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9994 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_octavia.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2907 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_redhat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7495 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_ubuntu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/_vlan.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.485365 tobiko-0.6.8/tobiko/openstack/stacks/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/designate/zone.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.485365 tobiko-0.6.8/tobiko/openstack/stacks/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/neutron/external_network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/neutron/floating_ip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/neutron/network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/neutron/qos.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/neutron/router_interface.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/neutron/security_groups.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.489365 tobiko-0.6.8/tobiko/openstack/stacks/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/nova/flavor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/nova/key_pair.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/nova/multi_ip_test_stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5474 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/nova/server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/nova/server_group.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.489365 tobiko-0.6.8/tobiko/openstack/stacks/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3880 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/octavia/listener.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/octavia/load_balancer.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/octavia/member.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2046 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/stacks/octavia/pool.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.489365 tobiko-0.6.8/tobiko/openstack/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1864 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27700 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/tests/_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3309 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/tests/_nova.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.489365 tobiko-0.6.8/tobiko/openstack/topology/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3103 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5902 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_assert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6753 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6669 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_sh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28521 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/openstack/topology/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.489365 tobiko-0.6.8/tobiko/podman/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6856 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.489365 tobiko-0.6.8/tobiko/podman/_podman1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11357 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7078 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/podman/_podman1/libs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/_containers_attach.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3178 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/_containers_start.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6547 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4791 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/pods.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/system.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6354 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/libs/tunnel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_podman1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/podman/_shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/run/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5967 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/_discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/_find.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2287 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/_result.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3728 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/_run.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/run/_worker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/shell/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/shell/ansible/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ansible/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17125 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ansible/_playbook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ansible/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/shell/curl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/curl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3850 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/curl/_execute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14215 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/curl/_process.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/shell/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/files/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8343 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/files/_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2947 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/find.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2829 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/grep.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ifconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4758 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ip.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.493365 tobiko-0.6.8/tobiko/shell/iperf3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/iperf3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/iperf3/_assert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/iperf3/_execute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2954 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/iperf3/_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2056 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/iperf3/_parameters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/iperf3/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.497365 tobiko-0.6.8/tobiko/shell/ping/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/_assert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13196 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9280 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/_parameters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18909 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/_ping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6405 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/_statistics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ping/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.497365 tobiko-0.6.8/tobiko/shell/sh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5045 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2087 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_cmdline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2211 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18921 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7070 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_execute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2343 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5482 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_io.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5682 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_mkdirs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_mktemp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3606 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_nameservers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_path.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20435 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7874 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_ps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7215 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_reboot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9926 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9679 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_systemctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_uptime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1455 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_wc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/_which.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/sh/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10527 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ss.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/shell/ssh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27583 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2620 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7540 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10857 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/_forward.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4449 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/_key_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/_skip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3472 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/ssh/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/shell/tcpdump/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/tcpdump/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/tcpdump/_assert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/tcpdump/_execute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/tcpdump/_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shell/tcpdump/_parameters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/shiftstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2598 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/_clouds_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2124 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1490 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/_skip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1531 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3440 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/shiftstack/stacks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7473 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/conftest.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/tests/faults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/tests/faults/containers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/containers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15417 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/containers/container_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4553 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/containers/test_container_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4893 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/containers/test_container_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/tests/faults/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30246 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/ha/cloud_disruptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10445 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/ha/test_cloud_recovery.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/tests/faults/iha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/iha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/iha/test_cloud_recovery.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.501365 tobiko-0.6.8/tobiko/tests/faults/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34270 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/neutron/test_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/neutron/test_raft.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/faults/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/octavia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10398 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/octavia/test_faults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10345 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/faults/octavia/test_services.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3567 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/common/test_background.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/docker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/docker/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/docker/test_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/openstack/hot/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/hot/my_stack.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4572 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4656 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_subnet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_centos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5737 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_cirros.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1784 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_fedora.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8603 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_red_hat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_ubuntu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_vlan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_designate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_glance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5937 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6822 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8622 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_octavia.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10147 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/test_topology.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.505365 tobiko-0.6.8/tobiko/tests/functional/openstack/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/openstack/tests/test_nova.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.509365 tobiko-0.6.8/tobiko/tests/functional/podman/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/podman/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/podman/test_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.509365 tobiko-0.6.8/tobiko/tests/functional/run/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/run/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/run/test_discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1534 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/run/test_find.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/run/test_run.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.509365 tobiko-0.6.8/tobiko/tests/functional/shell/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.509365 tobiko-0.6.8/tobiko/tests/functional/shell/sh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8392 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7929 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_execute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5999 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_ps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4369 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_reboot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1573 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_systemctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3293 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_wc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3339 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_which.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5398 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/test_curl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/test_ifconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7892 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/test_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/test_mktemp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/test_nameservers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8419 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shell/test_ping.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.509365 tobiko-0.6.8/tobiko/tests/functional/shiftstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shiftstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shiftstack/test_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shiftstack/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/shiftstack/test_stacks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.509365 tobiko-0.6.8/tobiko/tests/functional/tripleo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/requirements/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/requirements/openstack-cloud.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.437365 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.437365 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/roles/ping/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/roles/ping/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/roles/ping/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/test_debug_vars.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/test_overcloud_openstack_auth.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/test_ping_hosts.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/test_undercloud_current_dir.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/playbooks/vars/some-vars.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3172 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/test_ansible.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10507 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/test_overcloud.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/test_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7040 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/functional/tripleo/test_undercloud.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/cloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/cloud/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2468 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/cloud/test_nodes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/containers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/containers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13884 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/containers/test_containers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/ha/test_overcloud.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/neutron/test_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12046 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/neutron/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1088 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/neutron/test_nodes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/nova/test_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/nova/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/requirements.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.437365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.437365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/files/demo.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/scripts/pods_ready.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1412 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/check_demo_app.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/debug_machines.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/recreate_ocp_project.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/validate_node.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5801 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/verification.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/vars/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/verify-shiftstack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/sanity/shiftstack/test_shiftstack.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.513365 tobiko-0.6.8/tobiko/tests/scenario/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3679 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/designate/test_zone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.517365 tobiko-0.6.8/tobiko/tests/scenario/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12528 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5300 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8526 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4398 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12581 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12959 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/neutron/test_trunk.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.517365 tobiko-0.6.8/tobiko/tests/scenario/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8873 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/nova/test_server.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.517365 tobiko-0.6.8/tobiko/tests/scenario/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/octavia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7115 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/octavia/test_traffic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.517365 tobiko-0.6.8/tobiko/tests/scenario/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/scenario/playbooks/test_floatingip.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.517365 tobiko-0.6.8/tobiko/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/_case.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/_patch.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/actors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3591 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/actors/test_actor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/actors/test_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/_case.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/_keystone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/designate/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/designate/test_zone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/heat/my-stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/heat/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12132 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/heat/test_stack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/heat/test_template.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3556 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11783 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/test_credentials.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/test_session.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/metalsmith/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/metalsmith/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/metalsmith/test_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/neutron/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/neutron/test_extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2509 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/nova/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/nova/test_cloud_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/nova/test_server.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/octavia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3968 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/octavia/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/test_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/openstack/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2211 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/openstack/tests/test_neutron.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.521365 tobiko-0.6.8/tobiko/tests/unit/shell/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/shell/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.525365 tobiko-0.6.8/tobiko/tests/unit/shell/sh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/shell/sh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5171 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/shell/sh/test_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3721 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/shell/sh/test_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/shell/sh/test_io.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/shell/test_ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8281 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_cached.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7457 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_case.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4874 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_conftest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8709 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18362 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_ini.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4554 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4508 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_operation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13294 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6512 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_select.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8912 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_skip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4911 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/test_version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.525365 tobiko-0.6.8/tobiko/tests/unit/tripleo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/tripleo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tests/unit/tripleo/test_config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.525365 tobiko-0.6.8/tobiko/tripleo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/_ansible.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15041 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/_overcloud.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/_rhosp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11473 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8737 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/_undercloud.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4005 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28716 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9527 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16545 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/pacemaker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10914 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/processes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/tripleo/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11492 2023-03-30 08:13:54.000000 tobiko-0.6.8/tobiko.conf.example
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.469365 tobiko-0.6.8/tobiko.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5607 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26680 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-03-30 08:14:31.000000 tobiko-0.6.8/tobiko.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.525365 tobiko-0.6.8/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3641 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/abandon_old_reviews.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4618 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1199 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/get_version.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      249 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/install-bindeps.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2108 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/install.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5646 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/run_tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4354 2023-03-30 08:13:54.000000 tobiko-0.6.8/tools/setup_infrared.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10828 2023-03-30 08:13:54.000000 tobiko-0.6.8/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15024 2023-03-30 08:13:54.000000 tobiko-0.6.8/upper-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-30 08:14:31.529365 tobiko-0.6.8/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2023-03-30 08:13:54.000000 tobiko-0.6.8/zuul.d/docker.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3575 2023-03-30 08:13:54.000000 tobiko-0.6.8/zuul.d/infrared.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1697 2023-03-30 08:13:54.000000 tobiko-0.6.8/zuul.d/others.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2023-03-30 08:13:54.000000 tobiko-0.6.8/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.889661 tobiko-0.6.9/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-05-03 08:00:07.000000 tobiko-0.6.9/.ansible-lint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-05-03 08:00:07.000000 tobiko-0.6.9/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-05-03 08:00:07.000000 tobiko-0.6.9/.dockerignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1834 2023-05-03 08:00:07.000000 tobiko-0.6.9/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27759 2023-05-03 08:00:07.000000 tobiko-0.6.9/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-05-03 08:00:07.000000 tobiko-0.6.9/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1697 2023-05-03 08:00:34.000000 tobiko-0.6.9/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97735 2023-05-03 08:00:34.000000 tobiko-0.6.9/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2023-05-03 08:00:07.000000 tobiko-0.6.9/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-05-03 08:00:07.000000 tobiko-0.6.9/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5607 2023-05-03 08:00:34.889661 tobiko-0.6.9/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-05-03 08:00:07.000000 tobiko-0.6.9/Pipfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3881 2023-05-03 08:00:07.000000 tobiko-0.6.9/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-03 08:00:07.000000 tobiko-0.6.9/ansible.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2023-05-03 08:00:07.000000 tobiko-0.6.9/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.746501 tobiko-0.6.9/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/readthedocs_requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.746501 tobiko-0.6.9/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.746501 tobiko-0.6.9/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13956 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/_static/tobiko.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13956 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/_static/tobiko.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/content.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.746501 tobiko-0.6.9/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6527 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/contributor/Vagrantfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11779 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/contributor/contributor.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2500 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/contributor/reviewer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1980 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/contributor/setup_tobiko_workstation.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.746501 tobiko-0.6.9/doc/source/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/etc/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/etc/tobiko.conf.gen
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/etc/tobiko.conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.746501 tobiko-0.6.9/doc/source/miscellaneous/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/miscellaneous/from-tempest-to-tobiko.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/miscellaneous/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.750477 tobiko-0.6.9/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.750477 tobiko-0.6.9/doc/source/reference/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/actors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/docker.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/http.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.750477 tobiko-0.6.9/doc/source/reference/modules/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/designate.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/glance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/heat.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/ironic.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/keystone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/metalsmith.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/neutron.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/nova.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/octavia.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/openstackclient.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/stacks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/openstack/topology.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/podman.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/run.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.754454 tobiko-0.6.9/doc/source/reference/modules/shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/ansible.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/curl.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/files.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/iperf3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/ping.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/sh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/ssh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shell/tcpdump.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/shiftstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tobiko.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.754454 tobiko-0.6.9/doc/source/reference/modules/tripleo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tripleo/containers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tripleo/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tripleo/nova.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tripleo/pacemaker.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tripleo/processes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/reference/modules/tripleo/services.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4156 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_conf_credentials.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_conf_explanation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_conf_logging.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_conf_venv_with_tox.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_install_venv.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_run_faults.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_run_scenario.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_run_specific_tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_run_workflow.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_skip_resources_creation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/_test_cases_report_files.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/quick-start.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2023-05-03 08:00:07.000000 tobiko-0.6.9/doc/source/user/run-test-cases.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-05-03 08:00:07.000000 tobiko-0.6.9/docker-compose.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-05-03 08:00:07.000000 tobiko-0.6.9/etc/README.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13956 2023-05-03 08:00:07.000000 tobiko-0.6.9/etc/tobiko.conf.example
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-03 08:00:07.000000 tobiko-0.6.9/extra-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/plugin.spec
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/infrared_plugin/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-before-run/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-before-run/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-before-run/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-before-run/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-before-run/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-deploy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-deploy/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-deploy/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-deploy/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-deploy/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-init/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-init/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-init/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-jenkins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-jenkins/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-jenkins/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-jenkins/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-jenkins/vars/jenkins.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.758431 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2928 2023-05-03 08:00:07.000000 tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-05-03 08:00:07.000000 tobiko-0.6.9/linters-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-05-03 08:00:07.000000 tobiko-0.6.9/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-03 08:00:07.000000 tobiko-0.6.9/mypy.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/playbooks/docker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/docker/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/docker/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/docker/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/playbooks/infrared/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/infrared/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/infrared/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/playbooks/tripleo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/tripleo/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/tripleo/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/tripleo/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/playbooks/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-03 08:00:07.000000 tobiko-0.6.9/playbooks/unit/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2023-05-03 08:00:07.000000 tobiko-0.6.9/pytest.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.718664 tobiko-0.6.9/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/notes/Added-parser-for-`ss`-command-ac426b522eb8adbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/notes/Added-support-for-metalsmith-00b9f808c1030236.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6127 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-03 08:00:07.000000 tobiko-0.6.9/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-05-03 08:00:07.000000 tobiko-0.6.9/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/roles/multi-node-setup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/multi-node-setup/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/roles/multi-node-setup/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/multi-node-setup/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.762407 tobiko-0.6.9/roles/multi-node-setup/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/multi-node-setup/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4773 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tests/Vagrantfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tests/ansible.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2980 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tests/provision.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tests/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tests/templates/hosts.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tests/templates/ssh_config.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1786 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tests/test_infrared_plugin.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-bindep/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-bindep/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-bindep/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-bindep/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-bindep/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-bindep/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-bindep/tasks/ensure-bindep.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-bindep/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-check-collected-files/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-check-collected-files/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-check-collected-files/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-check-collected-files/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-check-collected-files/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-cleanup/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-cleanup/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-cleanup/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-cleanup/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-cleanup/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-collect/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-collect/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-collect/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-collect/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-collect/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-collect/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-collect/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-collect-report/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-collect-report/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-collect-report/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-collect-report/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-collect-report/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-common/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.766384 tobiko-0.6.9/roles/tobiko-common/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2063 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-common/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-compile-python/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3604 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/Vagrantfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/ansible.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-compile-python/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/defaults/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/resolv_conf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-compile-python/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/tasks/setup_pip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3264 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/tasks/setup_python.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-compile-python/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/tests/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1975 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-compile-python/tests/test_py38.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-configure/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-configure/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-configure/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-configure/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-configure/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-configure/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-configure/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-copy-resolv-conf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-copy-resolv-conf/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-copy-resolv-conf/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-copy-resolv-conf/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-copy-resolv-conf/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-devstack/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.770361 tobiko-0.6.9/roles/tobiko-devstack/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-devstack/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/deploy-devstack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/deploy-tobiko.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/ensure-stack-user.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/install-bindeps.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/run-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-devstack/tasks/run-unstack.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.722641 tobiko-0.6.9/roles/tobiko-docker-compose/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-docker-compose/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-docker-compose/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-docker-compose/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-docker-compose/tasks/build.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-docker-compose/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-docker-compose/tasks/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-download-images/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-download-images/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-download-images/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-download-images/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-download-images/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-ensure-docker-compose/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-ensure-docker-compose/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-docker-compose/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-ensure-docker-compose/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-docker-compose/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-ensure-python3/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-ensure-python3/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-ensure-python3/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3899 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/files/get_python_info.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-ensure-python3/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.774337 tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/ensure-python3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/install.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/platform.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-CentOS-7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-Fedora-31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-Fedora.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-MacOSX.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-RedHat-7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-RedHat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-Ubuntu-18.04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/py3-Ubuntu.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-python3/vars/rhosp-RedHat-7.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-ensure-ssh-keys/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-ensure-ssh-keys/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-ssh-keys/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-ensure-ssh-keys/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-ssh-keys/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-ensure-tox/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-ensure-tox/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-tox/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-ensure-tox/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-tox/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-ensure-tox/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-tox/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-ensure-tox/tasks/tox.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-fixup-stuff/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-fixup-stuff/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-fixup-stuff/tasks/centos.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-fixup-stuff/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-inventory/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-inventory/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-inventory/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-inventory/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-inventory/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/templates/test_inventory.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-inventory/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/vars/test-inventory-CentOS-7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/vars/test-inventory-Fedora.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/vars/test-inventory-RedHat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-inventory/vars/test-inventory-Ubuntu.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-redhat-subscription/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-redhat-subscription/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-redhat-subscription/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-redhat-subscription/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-redhat-subscription/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-run/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.778314 tobiko-0.6.9/roles/tobiko-run/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.782291 tobiko-0.6.9/roles/tobiko-run/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.782291 tobiko-0.6.9/roles/tobiko-run/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/tasks/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/roles/tobiko-run/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-designate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-faults.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-heat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-nova.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-octavia.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-ovn-migration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-designate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-faults.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-heat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-nova.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-octavia.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources-ovn-migration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-create-resources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-default.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-faults-iha.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-faults-neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-faults.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-functional.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-gate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-minimal.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-octavia-faults.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-sanity-shiftstack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-sanity.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-unit.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.726617 tobiko-0.6.9/roles/tobiko-tox/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/roles/tobiko-tox/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-tox/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/roles/tobiko-tox/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-tox/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/roles/tobiko-tox/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-tox/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-tox/tasks/tox.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.730594 tobiko-0.6.9/roles/tobiko-zuul/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/roles/tobiko-zuul/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-zuul/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/roles/tobiko-zuul/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-05-03 08:00:07.000000 tobiko-0.6.9/roles/tobiko-zuul/vars/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-05-03 08:00:34.889661 tobiko-0.6.9/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2023-05-03 08:00:07.000000 tobiko-0.6.9/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-03 08:00:07.000000 tobiko-0.6.9/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.786267 tobiko-0.6.9/tobiko/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5793 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.790244 tobiko-0.6.9/tobiko/actors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/actors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9703 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/actors/_actor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2660 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/actors/_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5351 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/actors/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/actors/_request.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.794221 tobiko-0.6.9/tobiko/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16453 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_background.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4054 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_cached.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12491 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_case.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_deprecation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4278 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_detail.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5034 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19992 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_ini.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6879 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_operation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1922 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_os.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10255 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4153 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_select.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5571 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_shelves.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5553 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_skip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1818 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2806 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/common/_yaml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12929 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.794221 tobiko-0.6.9/tobiko/docker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/docker/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8778 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/docker/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/docker/_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4463 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/docker/_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/docker/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.794221 tobiko-0.6.9/tobiko/http/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/http/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/http/_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/http/_session.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.794221 tobiko-0.6.9/tobiko/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2375 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.798197 tobiko-0.6.9/tobiko/openstack/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/designate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/designate/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/designate/_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/designate/_zone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.798197 tobiko-0.6.9/tobiko/openstack/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/glance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/glance/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18476 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/glance/_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/glance/_io.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/glance/_lzma.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2978 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/glance/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.798197 tobiko-0.6.9/tobiko/openstack/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/heat/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/heat/_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27203 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/heat/_stack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4394 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/heat/_template.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.798197 tobiko-0.6.9/tobiko/openstack/ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/ironic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/ironic/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5396 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/ironic/_node.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.802174 tobiko-0.6.9/tobiko/openstack/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6280 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8837 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/_clouds_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14543 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/_credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6988 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/keystone/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.802174 tobiko-0.6.9/tobiko/openstack/metalsmith/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/metalsmith/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2623 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/metalsmith/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/metalsmith/_instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.802174 tobiko-0.6.9/tobiko/openstack/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6512 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6150 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2231 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3701 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8807 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5033 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_quota_set.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_security_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4967 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3309 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/_subnet_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3580 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/neutron/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.806151 tobiko-0.6.9/tobiko/openstack/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3687 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16960 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8975 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_cloud_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2574 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_hypervisor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_key_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5343 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_quota_set.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4183 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/nova/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.806151 tobiko-0.6.9/tobiko/openstack/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3113 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9191 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_amphora.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2730 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3678 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/_waiters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/octavia/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.810127 tobiko-0.6.9/tobiko/openstack/openstackclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2971 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_security_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_security_group_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1769 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstackclient/_subnet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.810127 tobiko-0.6.9/tobiko/openstack/openstacksdkclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstacksdkclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/openstacksdkclient/_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.814104 tobiko-0.6.9/tobiko/openstack/stacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6259 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2821 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_centos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_cirros.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_designate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_fedora.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_hot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_l3ha.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36155 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19596 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9994 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_octavia.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2907 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_redhat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7484 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_ubuntu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/_vlan.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.814104 tobiko-0.6.9/tobiko/openstack/stacks/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/designate/zone.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.814104 tobiko-0.6.9/tobiko/openstack/stacks/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/neutron/external_network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/neutron/floating_ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4496 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/neutron/network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/neutron/qos.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/neutron/router_interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/neutron/security_groups.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.814104 tobiko-0.6.9/tobiko/openstack/stacks/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/nova/flavor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/nova/key_pair.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/nova/multi_ip_test_stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5474 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/nova/server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/nova/server_group.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.818081 tobiko-0.6.9/tobiko/openstack/stacks/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3880 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/octavia/listener.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/octavia/load_balancer.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/octavia/member.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2046 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/stacks/octavia/pool.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.818081 tobiko-0.6.9/tobiko/openstack/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1864 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29438 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/tests/_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3309 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/tests/_nova.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.822058 tobiko-0.6.9/tobiko/openstack/topology/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3103 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5902 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_assert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6753 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6669 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_sh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28520 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/openstack/topology/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.822058 tobiko-0.6.9/tobiko/podman/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6856 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.822058 tobiko-0.6.9/tobiko/podman/_podman1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11357 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7078 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.826034 tobiko-0.6.9/tobiko/podman/_podman1/libs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/_containers_attach.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3178 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/_containers_start.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6547 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4791 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/pods.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/system.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6354 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/libs/tunnel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_podman1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/podman/_shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.826034 tobiko-0.6.9/tobiko/run/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5967 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/_discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/_find.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2287 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/_result.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3728 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/_run.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/run/_worker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.830011 tobiko-0.6.9/tobiko/shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.830011 tobiko-0.6.9/tobiko/shell/ansible/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ansible/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17125 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ansible/_playbook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ansible/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.830011 tobiko-0.6.9/tobiko/shell/curl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/curl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3850 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/curl/_execute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14215 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/curl/_process.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.830011 tobiko-0.6.9/tobiko/shell/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/files/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8343 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/files/_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2947 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/find.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2829 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/grep.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ifconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4758 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.830011 tobiko-0.6.9/tobiko/shell/iperf3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/iperf3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/iperf3/_assert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/iperf3/_execute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2954 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/iperf3/_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2056 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/iperf3/_parameters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/iperf3/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.837964 tobiko-0.6.9/tobiko/shell/ping/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/_assert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13196 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9357 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/_parameters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18924 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/_ping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6405 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/_statistics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ping/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.841941 tobiko-0.6.9/tobiko/shell/sh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5045 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2087 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_cmdline.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2211 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18921 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7070 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_execute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2343 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5482 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_io.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5682 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_mkdirs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_mktemp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3606 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_nameservers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_path.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20439 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7874 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_ps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7215 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_reboot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9926 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_ssh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9679 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_systemctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_uptime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1455 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_wc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/_which.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/sh/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10488 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ss.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.841941 tobiko-0.6.9/tobiko/shell/ssh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27583 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2620 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7540 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10857 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/_forward.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4449 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/_key_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/_skip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3472 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/ssh/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.841941 tobiko-0.6.9/tobiko/shell/tcpdump/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/tcpdump/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/tcpdump/_assert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/tcpdump/_execute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/tcpdump/_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shell/tcpdump/_parameters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/shiftstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2598 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/_clouds_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2124 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1490 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/_skip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1531 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3440 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/shiftstack/stacks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7473 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/conftest.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/tests/faults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/tests/faults/containers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/containers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15417 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/containers/container_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4553 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/containers/test_container_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4893 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/containers/test_container_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/tests/faults/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30525 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/ha/cloud_disruptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11043 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/ha/test_cloud_recovery.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/tests/faults/iha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/iha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/iha/test_cloud_recovery.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.845918 tobiko-0.6.9/tobiko/tests/faults/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34292 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/neutron/test_agents.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/neutron/test_raft.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.849894 tobiko-0.6.9/tobiko/tests/faults/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/octavia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10398 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/octavia/test_faults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10345 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/faults/octavia/test_services.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.849894 tobiko-0.6.9/tobiko/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.849894 tobiko-0.6.9/tobiko/tests/functional/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3567 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/common/test_background.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.849894 tobiko-0.6.9/tobiko/tests/functional/docker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/docker/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/docker/test_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.849894 tobiko-0.6.9/tobiko/tests/functional/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.849894 tobiko-0.6.9/tobiko/tests/functional/openstack/hot/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/hot/my_stack.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.853871 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4572 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4930 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4503 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_subnet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.853871 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_centos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5737 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_cirros.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1784 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_fedora.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9450 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_red_hat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_ubuntu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_vlan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_designate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_glance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5937 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6822 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8622 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_octavia.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10147 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/test_topology.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.853871 tobiko-0.6.9/tobiko/tests/functional/openstack/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/openstack/tests/test_nova.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.853871 tobiko-0.6.9/tobiko/tests/functional/podman/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/podman/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/podman/test_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.853871 tobiko-0.6.9/tobiko/tests/functional/run/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/run/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/run/test_discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1534 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/run/test_find.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/run/test_run.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.857848 tobiko-0.6.9/tobiko/tests/functional/shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.857848 tobiko-0.6.9/tobiko/tests/functional/shell/sh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8392 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7929 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_execute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5999 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_ps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4369 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_reboot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1573 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_systemctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3293 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_wc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3339 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_which.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5398 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/test_curl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/test_ifconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7892 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/test_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/test_mktemp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/test_nameservers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8419 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shell/test_ping.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.857848 tobiko-0.6.9/tobiko/tests/functional/shiftstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shiftstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shiftstack/test_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shiftstack/test_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/shiftstack/test_stacks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.857848 tobiko-0.6.9/tobiko/tests/functional/tripleo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/requirements/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/requirements/openstack-cloud.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.734571 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.734571 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/roles/ping/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/roles/ping/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/roles/ping/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/test_debug_vars.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/test_overcloud_openstack_auth.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/test_ping_hosts.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/test_undercloud_current_dir.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/playbooks/vars/some-vars.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3172 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/test_ansible.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10507 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/test_overcloud.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/test_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7040 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/functional/tripleo/test_undercloud.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/sanity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/sanity/cloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/cloud/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2468 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/cloud/test_nodes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/sanity/containers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/containers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13884 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/containers/test_containers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/sanity/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/ha/test_overcloud.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/sanity/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/neutron/test_agents.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12046 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/neutron/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1088 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/neutron/test_nodes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.861824 tobiko-0.6.9/tobiko/tests/sanity/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/nova/test_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/nova/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/requirements.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.738547 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.738547 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/files/demo.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/scripts/pods_ready.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1412 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/check_demo_app.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/debug_machines.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/recreate_ocp_project.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/validate_node.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5801 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/verification.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/vars/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/verify-shiftstack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/sanity/shiftstack/test_shiftstack.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.865801 tobiko-0.6.9/tobiko/tests/scenario/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/designate/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3653 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/designate/test_zone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.869778 tobiko-0.6.9/tobiko/tests/scenario/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12740 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5300 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8526 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4398 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12581 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13012 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/neutron/test_trunk.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.869778 tobiko-0.6.9/tobiko/tests/scenario/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8873 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/nova/test_server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.869778 tobiko-0.6.9/tobiko/tests/scenario/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/octavia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7115 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/octavia/test_traffic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.869778 tobiko-0.6.9/tobiko/tests/scenario/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/scenario/playbooks/test_floatingip.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.873754 tobiko-0.6.9/tobiko/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/_case.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/_patch.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.873754 tobiko-0.6.9/tobiko/tests/unit/actors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3591 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/actors/test_actor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/actors/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.877731 tobiko-0.6.9/tobiko/tests/unit/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/_case.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/_keystone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.877731 tobiko-0.6.9/tobiko/tests/unit/openstack/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/designate/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/designate/test_zone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.877731 tobiko-0.6.9/tobiko/tests/unit/openstack/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/heat/my-stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/heat/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12132 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/heat/test_stack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/heat/test_template.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.877731 tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3556 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11783 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/test_credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/test_session.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.881708 tobiko-0.6.9/tobiko/tests/unit/openstack/metalsmith/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/metalsmith/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/metalsmith/test_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.881708 tobiko-0.6.9/tobiko/tests/unit/openstack/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/neutron/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/neutron/test_extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.881708 tobiko-0.6.9/tobiko/tests/unit/openstack/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2509 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/nova/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/nova/test_cloud_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/nova/test_server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.881708 tobiko-0.6.9/tobiko/tests/unit/openstack/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/octavia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3968 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/octavia/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/test_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.881708 tobiko-0.6.9/tobiko/tests/unit/openstack/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2211 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/openstack/tests/test_neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.881708 tobiko-0.6.9/tobiko/tests/unit/shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/shell/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.885684 tobiko-0.6.9/tobiko/tests/unit/shell/sh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/shell/sh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5171 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/shell/sh/test_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3721 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/shell/sh/test_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/shell/sh/test_io.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/shell/test_ssh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8281 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_cached.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7457 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_case.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4874 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_conftest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8709 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18362 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_ini.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4554 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4508 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_operation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13294 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6512 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_select.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8912 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_skip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4911 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/test_version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.885684 tobiko-0.6.9/tobiko/tests/unit/tripleo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/tripleo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tests/unit/tripleo/test_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.885684 tobiko-0.6.9/tobiko/tripleo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/_ansible.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15041 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/_overcloud.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/_rhosp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11473 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8737 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/_undercloud.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4005 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28716 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9527 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16545 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/pacemaker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10913 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/processes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/tripleo/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13956 2023-05-03 08:00:07.000000 tobiko-0.6.9/tobiko.conf.example
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.790244 tobiko-0.6.9/tobiko.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5607 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28370 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-05-03 08:00:34.000000 tobiko-0.6.9/tobiko.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.889661 tobiko-0.6.9/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3641 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/abandon_old_reviews.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4618 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1199 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/get_version.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      249 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/install-bindeps.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2108 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/install.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5646 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/run_tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4354 2023-05-03 08:00:07.000000 tobiko-0.6.9/tools/setup_infrared.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10966 2023-05-03 08:00:07.000000 tobiko-0.6.9/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15024 2023-05-03 08:00:07.000000 tobiko-0.6.9/upper-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-03 08:00:34.889661 tobiko-0.6.9/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2023-05-03 08:00:07.000000 tobiko-0.6.9/zuul.d/docker.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3575 2023-05-03 08:00:07.000000 tobiko-0.6.9/zuul.d/infrared.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2023-05-03 08:00:07.000000 tobiko-0.6.9/zuul.d/others.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2023-05-03 08:00:07.000000 tobiko-0.6.9/zuul.d/project.yaml
```

### Comparing `tobiko-0.6.8/.dockerignore` & `tobiko-0.6.9/.dockerignore`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/.pre-commit-config.yaml` & `tobiko-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/.pylintrc` & `tobiko-0.6.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/AUTHORS` & `tobiko-0.6.9/AUTHORS`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 Nir Magnezi <nmagnezi@redhat.com>
 Omer <oschwart@redhat.com>
 Pini Komarov <pkomarov@redhat.com>
 Rafael Folco <rfolco@redhat.com>
 Roee Agiman <ragiman@redhat.com>
 Roman Safronov <rsafrono@redhat.com>
 Slawek Kaplonski <skaplons@redhat.com>
+Stephen Finucane <stephenfin@redhat.com>
 Sławek Kapłoński <skaplons@redhat.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Tobias Urdin <tobias.urdin@binero.com>
 Wes Hayutin <weshayutin@gmail.com>
 abregman <abregman@redhat.com>
 dabarzil <dabarzil@redhat.com>
 gaobin <gaobin@inspur.com>
```

### Comparing `tobiko-0.6.8/ChangeLog` & `tobiko-0.6.9/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,41 @@
 CHANGES
 =======
 
+0.6.9
+-----
+
+* Add new tox env and workflow for ovn\_migration sanity tests
+* Don't run some of the stateless SG tests in ovn migration workflow
+* Unskip UbuntuExternalPortTest tests on upstream jobs
+* Workaround to avoid connectivity problems from ubuntu VM instances
+* Create only one Sec Group per fixture
+* Use Subnet pools to avoid cidr concurrency issues
+* Fix faults tests when External LB is configured
+* Do not upgrade virtualenv to the latest version
+* Refactor test\_alive\_agents\_are\_consistent\_along\_time
+* Fix neutron requests that are sent by background processes
+* Add designate upstream job
+* Fix captured exceptions and add some logs to test\_ovsdb\_transation
+* Catch some exceptions when novaclient.list\_services is run
+* Update github host key
+* Remove designate\_faults testenv
+* Fix basic Designate scenario test
+* Make sphinx to generate Tobiko API docs based on docstrings
+* Update latest stable tag to 0.6.8
+
 0.6.8
 -----
 
 * Drop lib-validations dependency
 * Refactor pcs commands execution
 * Add designate IR plugin files
 * Add test case to test ovn leadership change
 * Fix get\_overcloud\_ssh\_username
+* Add openstacksdk config options method
 * Remove internal Red Hat URLs
 * Obtain overcloud ssh username based on RHOSP release
 * nit: fixed RetryAttempt details
 * [Stateless SG] Add test to check there's no SG entries in conntrack
 * Update latest stable tag to 0.6.7
 
 0.6.7
```

### Comparing `tobiko-0.6.8/Dockerfile` & `tobiko-0.6.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/LICENSE` & `tobiko-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/PKG-INFO` & `tobiko-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tobiko
-Version: 0.6.8
+Version: 0.6.9
 Summary: OpenStack Testing Upgrades Library
 Home-page: https://tobiko.readthedocs.io/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======
         Tobiko
```

### Comparing `tobiko-0.6.8/README.rst` & `tobiko-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/bindep.txt` & `tobiko-0.6.9/bindep.txt`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/Makefile` & `tobiko-0.6.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/_static/tobiko.conf.sample` & `tobiko-0.6.9/doc/source/_static/tobiko.conf.sample`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 [DEFAULT]
 
 
+[ansible]
+
+#
+# From tobiko
+#
+
+# Default Ansible inventory files (list value)
+#inventory_files = /etc/ansible/hosts
+
+# Default Ansible playbook verbosity (integer value)
+#verbosity = <None>
+
+
 [centos]
 
 #
 # From tobiko
 #
 
 # Default centos image name (string value)
@@ -27,14 +40,18 @@
 
 # Default centos password (string value)
 #password = <None>
 
 # Default centos SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [centos7]
 
 #
 # From tobiko
 #
 
@@ -58,14 +75,18 @@
 
 # Default centos7 password (string value)
 #password = <None>
 
 # Default centos7 SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [cirros]
 
 #
 # From tobiko
 #
 
@@ -89,14 +110,28 @@
 
 # Default cirros password (string value)
 #password = <None>
 
 # Default cirros SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
+
+[common]
+
+#
+# From tobiko
+#
+
+# Default directory where to look for shelves. (string value)
+#shelves_dir = ~/.tobiko/cache/shelves
+
 
 [fedora]
 
 #
 # From tobiko
 #
 
@@ -120,14 +155,18 @@
 
 # Default fedora password (string value)
 #password = <None>
 
 # Default fedora SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [glance]
 
 #
 # From tobiko
 #
 
@@ -211,14 +250,17 @@
 
 # Trust ID for trust scoping. (string value)
 #trust_id = <None>
 
 # Cloud name used pick authentication parameters from clouds.* (string value)
 #cloud_name = <None>
 
+# Host login from where to search for clouds file (list value)
+#clouds_file_hosts = localhost
+
 # Directories where to look for clouds files (list value)
 #clouds_file_dirs = .,~/.config/openstack,/etc/openstack
 
 # Clouds file names (list value)
 #clouds_file_names = clouds.yaml,clouds.yml,clouds.json
 
 
@@ -285,29 +327,35 @@
 [nova]
 
 #
 # From tobiko
 #
 
 # Default SSH key to login to server instances (string value)
-#key_file = ~/.ssh/id_rsa
+#key_file = ~/.ssh/id_ecdsa
+
+# Default SSH key type to login to server instances (string value)
+#key_type = ecdsa
 
 
 [octavia]
 
 #
 # From tobiko
 #
 
 # Interval to check for status changes, in seconds. (integer value)
 #check_interval = 5
 
 # Timeout, in seconds, to wait for a status change. (integer value)
 #check_timeout = 360
 
+# The user we should use when we SSH the amphora. (string value)
+#amphora_user = cloud-user
+
 
 [ping]
 
 #
 # From tobiko
 #
 
@@ -358,14 +406,18 @@
 
 # Default rhel password (string value)
 #password = <None>
 
 # Default rhel SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [shell]
 
 #
 # From tobiko
 #
 
@@ -373,14 +425,33 @@
 #command = /bin/sh -c
 
 # Default sudo command used for executing commands as superuser or another user (string
 # value)
 #sudo = sudo
 
 
+[shiftstack]
+
+#
+# From tobiko
+#
+
+# local clouds file path (string value)
+#local_clouds_file_path = .tobiko/shifstack/clouds.yaml
+
+# remote clouds file path on undercloud-0 host (string value)
+#remote_clouds_file_path = ~/clouds.yaml
+
+# Keystone credentials cloud name (string value)
+#cloud_name = shiftstack
+
+# Path to the RC file used to populate OS_* environment variables (list value)
+#rcfile = ./shiftstackrc
+
+
 [ssh]
 
 #
 # From tobiko
 #
 
 # Logout debugging messages of paramiko library (boolean value)
@@ -394,16 +465,16 @@
 
 # Default SSH username (string value)
 #username = <None>
 
 # Default user SSH configuration files (list value)
 #config_files = ssh_config,.ssh/config
 
-# Default SSH private key file(s) (list value)
-#key_file = ~/.ssh/id_rsa,.ssh/id
+# Default SSH private key file(s) wildcard (list value)
+#key_file = .ssh/id,~/.ssh/id_dsa,~/.ssh/id_rsa,~/.ssh/id_ecdsa,~/.ssh/id_ed25519
 
 # Set to False to disable connecting to the SSH agent (boolean value)
 #allow_agent = false
 
 # Set to True to turn on compression (boolean value)
 #compress = false
 
@@ -483,39 +554,57 @@
 # TCP port of SSH server on undercloud host (integer value)
 #undercloud_ssh_port = <None>
 
 # Username with access to stackrc and overcloudrc files (string value)
 #undercloud_ssh_username = stack
 
 # SSH key filename used to login to Undercloud node (string value)
-#undercloud_ssh_key_filename = ~/.ssh/id_rsa
+#undercloud_ssh_key_filename = <None>
 
 # Undercloud RC filename (list value)
 #undercloud_rcfile = ~/stackrc
 
+# undercloud cloud name to be used for loading credentials from the undercloud clouds
+# files (string value)
+#undercloud_cloud_name = undercloud
+
 # TCP port of SSH server on overcloud hosts (integer value)
 #overcloud_ssh_port = <None>
 
 # Default username used to connect to overcloud nodes (string value)
-#overcloud_ssh_username = heat-admin
+#overcloud_ssh_username = <None>
 
 # SSH key filename used to login to Overcloud nodes (string value)
 #overcloud_ssh_key_filename = ~/.ssh/id_overcloud
 
 # Overcloud RC filenames (list value)
 #overcloud_rcfile = ~/overcloudrc,~/qe-Cloud-0rc
 
+# overcloud cloud name to be used for loading credentials from the overcloud clouds
+# files (string value)
+#overcloud_cloud_name = overcloud
+
 # Default IP address version to be used to connect to overcloud nodes  (integer value)
 #overcloud_ip_version = <None>
 
 # Name of network used to connect to overcloud nodes (string value)
 #overcloud_network_name = <None>
 
+# Dictionary with the node groups corresponding to different hostname prefixes (dict
+# value)
+#overcloud_groups_dict = cmp:compute,ctrl:controller
+
 # path to where to export tripleo inventory file (string value)
-#inventory_file = tripleo-hosts.yaml
+#inventory_file = .ansible/inventory/tripleo.yaml
+
+# OSP env was done with an external load balancer (boolean value)
+#has_external_load_balancer = false
+
+# whether Ceph RGW is deployed (boolean value)
+#ceph_rgw = false
 
 
 [ubuntu]
 
 #
 # From tobiko
 #
@@ -539,7 +628,11 @@
 #username = <None>
 
 # Default ubuntu password (string value)
 #password = <None>
 
 # Default ubuntu SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
+
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
```

### Comparing `tobiko-0.6.8/doc/source/_static/tobiko.conf.txt` & `tobiko-0.6.9/doc/source/_static/tobiko.conf.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 [DEFAULT]
 
 
+[ansible]
+
+#
+# From tobiko
+#
+
+# Default Ansible inventory files (list value)
+#inventory_files = /etc/ansible/hosts
+
+# Default Ansible playbook verbosity (integer value)
+#verbosity = <None>
+
+
 [centos]
 
 #
 # From tobiko
 #
 
 # Default centos image name (string value)
@@ -27,14 +40,18 @@
 
 # Default centos password (string value)
 #password = <None>
 
 # Default centos SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [centos7]
 
 #
 # From tobiko
 #
 
@@ -58,14 +75,18 @@
 
 # Default centos7 password (string value)
 #password = <None>
 
 # Default centos7 SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [cirros]
 
 #
 # From tobiko
 #
 
@@ -89,14 +110,28 @@
 
 # Default cirros password (string value)
 #password = <None>
 
 # Default cirros SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
+
+[common]
+
+#
+# From tobiko
+#
+
+# Default directory where to look for shelves. (string value)
+#shelves_dir = ~/.tobiko/cache/shelves
+
 
 [fedora]
 
 #
 # From tobiko
 #
 
@@ -120,14 +155,18 @@
 
 # Default fedora password (string value)
 #password = <None>
 
 # Default fedora SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [glance]
 
 #
 # From tobiko
 #
 
@@ -211,14 +250,17 @@
 
 # Trust ID for trust scoping. (string value)
 #trust_id = <None>
 
 # Cloud name used pick authentication parameters from clouds.* (string value)
 #cloud_name = <None>
 
+# Host login from where to search for clouds file (list value)
+#clouds_file_hosts = localhost
+
 # Directories where to look for clouds files (list value)
 #clouds_file_dirs = .,~/.config/openstack,/etc/openstack
 
 # Clouds file names (list value)
 #clouds_file_names = clouds.yaml,clouds.yml,clouds.json
 
 
@@ -285,29 +327,35 @@
 [nova]
 
 #
 # From tobiko
 #
 
 # Default SSH key to login to server instances (string value)
-#key_file = ~/.ssh/id_rsa
+#key_file = ~/.ssh/id_ecdsa
+
+# Default SSH key type to login to server instances (string value)
+#key_type = ecdsa
 
 
 [octavia]
 
 #
 # From tobiko
 #
 
 # Interval to check for status changes, in seconds. (integer value)
 #check_interval = 5
 
 # Timeout, in seconds, to wait for a status change. (integer value)
 #check_timeout = 360
 
+# The user we should use when we SSH the amphora. (string value)
+#amphora_user = cloud-user
+
 
 [ping]
 
 #
 # From tobiko
 #
 
@@ -358,14 +406,18 @@
 
 # Default rhel password (string value)
 #password = <None>
 
 # Default rhel SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [shell]
 
 #
 # From tobiko
 #
 
@@ -373,14 +425,33 @@
 #command = /bin/sh -c
 
 # Default sudo command used for executing commands as superuser or another user (string
 # value)
 #sudo = sudo
 
 
+[shiftstack]
+
+#
+# From tobiko
+#
+
+# local clouds file path (string value)
+#local_clouds_file_path = .tobiko/shifstack/clouds.yaml
+
+# remote clouds file path on undercloud-0 host (string value)
+#remote_clouds_file_path = ~/clouds.yaml
+
+# Keystone credentials cloud name (string value)
+#cloud_name = shiftstack
+
+# Path to the RC file used to populate OS_* environment variables (list value)
+#rcfile = ./shiftstackrc
+
+
 [ssh]
 
 #
 # From tobiko
 #
 
 # Logout debugging messages of paramiko library (boolean value)
@@ -394,16 +465,16 @@
 
 # Default SSH username (string value)
 #username = <None>
 
 # Default user SSH configuration files (list value)
 #config_files = ssh_config,.ssh/config
 
-# Default SSH private key file(s) (list value)
-#key_file = ~/.ssh/id_rsa,.ssh/id
+# Default SSH private key file(s) wildcard (list value)
+#key_file = .ssh/id,~/.ssh/id_dsa,~/.ssh/id_rsa,~/.ssh/id_ecdsa,~/.ssh/id_ed25519
 
 # Set to False to disable connecting to the SSH agent (boolean value)
 #allow_agent = false
 
 # Set to True to turn on compression (boolean value)
 #compress = false
 
@@ -483,39 +554,57 @@
 # TCP port of SSH server on undercloud host (integer value)
 #undercloud_ssh_port = <None>
 
 # Username with access to stackrc and overcloudrc files (string value)
 #undercloud_ssh_username = stack
 
 # SSH key filename used to login to Undercloud node (string value)
-#undercloud_ssh_key_filename = ~/.ssh/id_rsa
+#undercloud_ssh_key_filename = <None>
 
 # Undercloud RC filename (list value)
 #undercloud_rcfile = ~/stackrc
 
+# undercloud cloud name to be used for loading credentials from the undercloud clouds
+# files (string value)
+#undercloud_cloud_name = undercloud
+
 # TCP port of SSH server on overcloud hosts (integer value)
 #overcloud_ssh_port = <None>
 
 # Default username used to connect to overcloud nodes (string value)
-#overcloud_ssh_username = heat-admin
+#overcloud_ssh_username = <None>
 
 # SSH key filename used to login to Overcloud nodes (string value)
 #overcloud_ssh_key_filename = ~/.ssh/id_overcloud
 
 # Overcloud RC filenames (list value)
 #overcloud_rcfile = ~/overcloudrc,~/qe-Cloud-0rc
 
+# overcloud cloud name to be used for loading credentials from the overcloud clouds
+# files (string value)
+#overcloud_cloud_name = overcloud
+
 # Default IP address version to be used to connect to overcloud nodes  (integer value)
 #overcloud_ip_version = <None>
 
 # Name of network used to connect to overcloud nodes (string value)
 #overcloud_network_name = <None>
 
+# Dictionary with the node groups corresponding to different hostname prefixes (dict
+# value)
+#overcloud_groups_dict = cmp:compute,ctrl:controller
+
 # path to where to export tripleo inventory file (string value)
-#inventory_file = tripleo-hosts.yaml
+#inventory_file = .ansible/inventory/tripleo.yaml
+
+# OSP env was done with an external load balancer (boolean value)
+#has_external_load_balancer = false
+
+# whether Ceph RGW is deployed (boolean value)
+#ceph_rgw = false
 
 
 [ubuntu]
 
 #
 # From tobiko
 #
@@ -539,7 +628,11 @@
 #username = <None>
 
 # Default ubuntu password (string value)
 #password = <None>
 
 # Default ubuntu SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
+
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
```

### Comparing `tobiko-0.6.8/doc/source/conf.py` & `tobiko-0.6.9/doc/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.coverage',
     'sphinx.ext.ifconfig',
     'sphinx.ext.graphviz',
     'sphinx.ext.todo',
+    'sphinx.ext.napoleon',
     'oslo_config.sphinxext',
     'oslo_config.sphinxconfiggen',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
 
@@ -123,7 +124,17 @@
 html_static_path = [f'{TOBIKO_DOC_DIR}/_static']
 
 # -- Options for oslo_config.sphinxconfiggen ---------------------------------
 
 config_generator_config_file = [
     (f'etc/tobiko.conf.gen', f"{TOBIKO_DOC_DIR}/_static/tobiko")
 ]
+
+def autodoc_skip_member(app, what, name, obj, skip, options):
+    # NOTE(slaweq): skip all external modules, like fixtures from the autodoc
+    if "tobiko" not in str(obj):
+        return True
+    # for tobiko modules, lets do what autodoc already decided to do
+    return skip
+
+def setup(app):
+    app.connect('autodoc-skip-member', autodoc_skip_member)
```

### Comparing `tobiko-0.6.8/doc/source/content.rst` & `tobiko-0.6.9/doc/source/content.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/contributor/Vagrantfile` & `tobiko-0.6.9/doc/source/contributor/Vagrantfile`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/contributor/contributor.rst` & `tobiko-0.6.9/doc/source/contributor/contributor.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/contributor/index.rst` & `tobiko-0.6.9/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/contributor/reviewer.rst` & `tobiko-0.6.9/doc/source/contributor/reviewer.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/contributor/setup_tobiko_workstation.rst` & `tobiko-0.6.9/doc/source/contributor/setup_tobiko_workstation.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/etc/tobiko.conf.rst` & `tobiko-0.6.9/doc/source/etc/tobiko.conf.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/miscellaneous/from-tempest-to-tobiko.rst` & `tobiko-0.6.9/doc/source/miscellaneous/from-tempest-to-tobiko.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/miscellaneous/index.rst` & `tobiko-0.6.9/doc/source/miscellaneous/index.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/reference/index.rst` & `tobiko-0.6.9/tobiko/shell/sh/_mktemp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-..
-      Licensed under the Apache License, Version 2.0 (the "License"); you may
-      not use this file except in compliance with the License. You may obtain
-      a copy of the License at
-
-          http://www.apache.org/licenses/LICENSE-2.0
-
-      Unless required by applicable law or agreed to in writing, software
-      distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-      WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-      License for the specific language governing permissions and limitations
-      under the License.
-
-      Convention for heading levels in Neutron lib devref:
-      =======  Heading 0 (reserved for the title in a document)
-      -------  Heading 1
-      ~~~~~~~  Heading 2
-      +++++++  Heading 3
-      '''''''  Heading 4
-      (Avoid deeper levels because they do not render well.)
-
-================================
-Tobiko Framework Reference Guide
-================================
-
-.. toctree::
-   :maxdepth: 1
-
-* :ref:`genindex`
-* :ref:`search`
+# Copyright (c) 2021 Red Hat, Inc.
+#
+# All Rights Reserved.
+#
+#    Licensed under the Apache License, Version 2.0 (the "License"); you may
+#    not use this file except in compliance with the License. You may obtain
+#    a copy of the License at
+#
+#         http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#    License for the specific language governing permissions and limitations
+#    under the License.
+from __future__ import absolute_import
+
+import tobiko
+from tobiko.shell import ssh
+from tobiko.shell.sh import _execute
+
+
+def make_temp_dir(ssh_client: ssh.SSHClientType = None,
+                  sudo: bool = None) \
+        -> str:
+    test_case = tobiko.get_test_case()
+    dir_name: str = _execute.execute('mktemp -d',
+                                     ssh_client=ssh_client,
+                                     sudo=sudo).stdout.strip()
+    test_case.addCleanup(_execute.execute,
+                         f'rm -fR "{dir_name}"',
+                         ssh_client=ssh_client,
+                         sudo=sudo)
+    return dir_name
```

### Comparing `tobiko-0.6.8/doc/source/user/_conf_credentials.rst` & `tobiko-0.6.9/doc/source/user/_conf_credentials.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_conf_logging.rst` & `tobiko-0.6.9/doc/source/user/_conf_logging.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_install_venv.rst` & `tobiko-0.6.9/doc/source/user/_install_venv.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_run_faults.rst` & `tobiko-0.6.9/doc/source/user/_run_faults.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_run_scenario.rst` & `tobiko-0.6.9/doc/source/user/_run_scenario.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_run_specific_tests.rst` & `tobiko-0.6.9/doc/source/user/_run_specific_tests.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_run_workflow.rst` & `tobiko-0.6.9/doc/source/user/_run_workflow.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_skip_resources_creation.rst` & `tobiko-0.6.9/doc/source/user/_skip_resources_creation.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/_test_cases_report_files.rst` & `tobiko-0.6.9/doc/source/user/_test_cases_report_files.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/config.rst` & `tobiko-0.6.9/doc/source/user/config.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/install.rst` & `tobiko-0.6.9/doc/source/user/install.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/quick-start.rst` & `tobiko-0.6.9/doc/source/user/quick-start.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/doc/source/user/run-test-cases.rst` & `tobiko-0.6.9/doc/source/user/run-test-cases.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/docker-compose.yml` & `tobiko-0.6.9/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/etc/tobiko.conf.example` & `tobiko-0.6.9/etc/tobiko.conf.example`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 [DEFAULT]
 
 
+[ansible]
+
+#
+# From tobiko
+#
+
+# Default Ansible inventory files (list value)
+#inventory_files = /etc/ansible/hosts
+
+# Default Ansible playbook verbosity (integer value)
+#verbosity = <None>
+
+
 [centos]
 
 #
 # From tobiko
 #
 
 # Default centos image name (string value)
@@ -27,14 +40,18 @@
 
 # Default centos password (string value)
 #password = <None>
 
 # Default centos SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [centos7]
 
 #
 # From tobiko
 #
 
@@ -58,14 +75,18 @@
 
 # Default centos7 password (string value)
 #password = <None>
 
 # Default centos7 SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [cirros]
 
 #
 # From tobiko
 #
 
@@ -89,14 +110,28 @@
 
 # Default cirros password (string value)
 #password = <None>
 
 # Default cirros SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
+
+[common]
+
+#
+# From tobiko
+#
+
+# Default directory where to look for shelves. (string value)
+#shelves_dir = ~/.tobiko/cache/shelves
+
 
 [fedora]
 
 #
 # From tobiko
 #
 
@@ -120,14 +155,18 @@
 
 # Default fedora password (string value)
 #password = <None>
 
 # Default fedora SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [glance]
 
 #
 # From tobiko
 #
 
@@ -211,14 +250,17 @@
 
 # Trust ID for trust scoping. (string value)
 #trust_id = <None>
 
 # Cloud name used pick authentication parameters from clouds.* (string value)
 #cloud_name = <None>
 
+# Host login from where to search for clouds file (list value)
+#clouds_file_hosts = localhost
+
 # Directories where to look for clouds files (list value)
 #clouds_file_dirs = .,~/.config/openstack,/etc/openstack
 
 # Clouds file names (list value)
 #clouds_file_names = clouds.yaml,clouds.yml,clouds.json
 
 
@@ -285,29 +327,35 @@
 [nova]
 
 #
 # From tobiko
 #
 
 # Default SSH key to login to server instances (string value)
-#key_file = ~/.ssh/id_rsa
+#key_file = ~/.ssh/id_ecdsa
+
+# Default SSH key type to login to server instances (string value)
+#key_type = ecdsa
 
 
 [octavia]
 
 #
 # From tobiko
 #
 
 # Interval to check for status changes, in seconds. (integer value)
 #check_interval = 5
 
 # Timeout, in seconds, to wait for a status change. (integer value)
 #check_timeout = 360
 
+# The user we should use when we SSH the amphora. (string value)
+#amphora_user = cloud-user
+
 
 [ping]
 
 #
 # From tobiko
 #
 
@@ -358,14 +406,18 @@
 
 # Default rhel password (string value)
 #password = <None>
 
 # Default rhel SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [shell]
 
 #
 # From tobiko
 #
 
@@ -373,14 +425,33 @@
 #command = /bin/sh -c
 
 # Default sudo command used for executing commands as superuser or another user (string
 # value)
 #sudo = sudo
 
 
+[shiftstack]
+
+#
+# From tobiko
+#
+
+# local clouds file path (string value)
+#local_clouds_file_path = .tobiko/shifstack/clouds.yaml
+
+# remote clouds file path on undercloud-0 host (string value)
+#remote_clouds_file_path = ~/clouds.yaml
+
+# Keystone credentials cloud name (string value)
+#cloud_name = shiftstack
+
+# Path to the RC file used to populate OS_* environment variables (list value)
+#rcfile = ./shiftstackrc
+
+
 [ssh]
 
 #
 # From tobiko
 #
 
 # Logout debugging messages of paramiko library (boolean value)
@@ -394,16 +465,16 @@
 
 # Default SSH username (string value)
 #username = <None>
 
 # Default user SSH configuration files (list value)
 #config_files = ssh_config,.ssh/config
 
-# Default SSH private key file(s) (list value)
-#key_file = ~/.ssh/id_rsa,.ssh/id
+# Default SSH private key file(s) wildcard (list value)
+#key_file = .ssh/id,~/.ssh/id_dsa,~/.ssh/id_rsa,~/.ssh/id_ecdsa,~/.ssh/id_ed25519
 
 # Set to False to disable connecting to the SSH agent (boolean value)
 #allow_agent = false
 
 # Set to True to turn on compression (boolean value)
 #compress = false
 
@@ -483,39 +554,57 @@
 # TCP port of SSH server on undercloud host (integer value)
 #undercloud_ssh_port = <None>
 
 # Username with access to stackrc and overcloudrc files (string value)
 #undercloud_ssh_username = stack
 
 # SSH key filename used to login to Undercloud node (string value)
-#undercloud_ssh_key_filename = ~/.ssh/id_rsa
+#undercloud_ssh_key_filename = <None>
 
 # Undercloud RC filename (list value)
 #undercloud_rcfile = ~/stackrc
 
+# undercloud cloud name to be used for loading credentials from the undercloud clouds
+# files (string value)
+#undercloud_cloud_name = undercloud
+
 # TCP port of SSH server on overcloud hosts (integer value)
 #overcloud_ssh_port = <None>
 
 # Default username used to connect to overcloud nodes (string value)
-#overcloud_ssh_username = heat-admin
+#overcloud_ssh_username = <None>
 
 # SSH key filename used to login to Overcloud nodes (string value)
 #overcloud_ssh_key_filename = ~/.ssh/id_overcloud
 
 # Overcloud RC filenames (list value)
 #overcloud_rcfile = ~/overcloudrc,~/qe-Cloud-0rc
 
+# overcloud cloud name to be used for loading credentials from the overcloud clouds
+# files (string value)
+#overcloud_cloud_name = overcloud
+
 # Default IP address version to be used to connect to overcloud nodes  (integer value)
 #overcloud_ip_version = <None>
 
 # Name of network used to connect to overcloud nodes (string value)
 #overcloud_network_name = <None>
 
+# Dictionary with the node groups corresponding to different hostname prefixes (dict
+# value)
+#overcloud_groups_dict = cmp:compute,ctrl:controller
+
 # path to where to export tripleo inventory file (string value)
-#inventory_file = tripleo-hosts.yaml
+#inventory_file = .ansible/inventory/tripleo.yaml
+
+# OSP env was done with an external load balancer (boolean value)
+#has_external_load_balancer = false
+
+# whether Ceph RGW is deployed (boolean value)
+#ceph_rgw = false
 
 
 [ubuntu]
 
 #
 # From tobiko
 #
@@ -539,7 +628,11 @@
 #username = <None>
 
 # Default ubuntu password (string value)
 #password = <None>
 
 # Default ubuntu SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
+
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
```

### Comparing `tobiko-0.6.8/infrared_plugin/Dockerfile` & `tobiko-0.6.9/infrared_plugin/Dockerfile`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/infrared_plugin/plugin.spec` & `tobiko-0.6.9/infrared_plugin/plugin.spec`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-before-run/tasks/main.yaml` & `tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-before-run/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-deploy/tasks/main.yaml` & `tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-deploy/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-init/tasks/main.yaml` & `tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-init/tasks/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 - name: "get Tobiko files"
   include_role: name=tobiko-ir-deploy
   vars:
     deploy_dir: '{{ tobiko_src_dir | realpath }}'
     deploy_git_repo: '{{ tobiko_git_repo }}'
-    deploy_git_refspec: "{{ tobiko_git_refspec | default('0.6.7') }}"
+    deploy_git_refspec: "{{ tobiko_git_refspec | default('0.6.8') }}"
     deploy_git_remote: "{{ tobiko_git_remote | default('') }}"
   when: create_tobiko_dir is changed
 
 
 - name: "find roles in directory '{{ tobiko_src_dir | realpath }}/roles'"
   find:
     paths:
```

### Comparing `tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/defaults/main.yaml` & `tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/infrared_plugin/roles/tobiko-ir-run/tasks/main.yaml` & `tobiko-0.6.9/infrared_plugin/roles/tobiko-ir-run/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/lower-constraints.txt` & `tobiko-0.6.9/lower-constraints.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Jinja2==2.11.2
 keystoneauth1==4.3.0
 metalsmith==1.6.2
 mock==3.0.5
 netaddr==0.8.0
 neutron-lib==2.7.0
 openstacksdk==0.31.2
+oslo.concurrency==3.26.0
 oslo.config==8.4.0
 oslo.log==4.4.0
 packaging==20.4
 paramiko==2.9.2
 pbr==5.5.1
 psutil==5.8.0
 pytest===6.2.5
```

### Comparing `tobiko-0.6.8/playbooks/tripleo/run.yaml` & `tobiko-0.6.9/playbooks/tripleo/run.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/releasenotes/source/conf.py` & `tobiko-0.6.9/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/requirements.txt` & `tobiko-0.6.9/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 fixtures>=3.0.0                 # Apache-2.0/BSD
 Jinja2>=2.11.2                  # BSD
 keystoneauth1>=4.3.0            # Apache-2.0
 metalsmith>=1.6.2               # Apache-2.0
 netaddr>=0.8.0                  # BSD
 neutron-lib>=2.7.0              # Apache-2.0
 openstacksdk>=0.31.2            # Apache-2.0
+oslo.concurrency>=3.26.0        # Apache-2.0
 oslo.config>=8.4.0              # Apache-2.0
 oslo.log>=4.4.0                 # Apache-2.0
 packaging>=20.4                 # Apache-2.0
 paramiko>=2.9.2                 # LGPLv2.1
 pbr>=5.5.1                      # Apache-2.0
 psutil>=5.8.0                   # BSD
 python-dateutil>=2.8.0          # Apache-2.0
```

### Comparing `tobiko-0.6.8/roles/multi-node-setup/README.rst` & `tobiko-0.6.9/roles/multi-node-setup/README.rst`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/multi-node-setup/tasks/main.yaml` & `tobiko-0.6.9/roles/multi-node-setup/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tests/Vagrantfile` & `tobiko-0.6.9/roles/tests/Vagrantfile`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tests/provision.yaml` & `tobiko-0.6.9/roles/tests/provision.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tests/test_infrared_plugin.yaml` & `tobiko-0.6.9/roles/tests/test_infrared_plugin.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-bindep/tasks/ensure-bindep.yaml` & `tobiko-0.6.9/roles/tobiko-bindep/tasks/ensure-bindep.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-bindep/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-bindep/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-check-collected-files/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-check-collected-files/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-cleanup/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-cleanup/tasks/main.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,30 @@
         xargs -r timeout 180 openstack stack delete -y --wait
   register: result
   retries: 5
   delay: 5
   until: result.rc == 0
   ignore_errors: yes
 
+- name: "cleanup subnet pools created by Tobiko tests"
+  shell: |
+    source {{ stackrc_file }}
+    openstack subnet pool list -f value -c 'Name' | \
+        grep "^tobiko\." | \
+        xargs -r openstack subnet pool delete
+  ignore_errors: yes
+
+- name: "cleanup Security Groups created by Tobiko tests"
+  shell: |
+    source {{ stackrc_file }}
+    openstack security group list -f value -c 'Name' | \
+        grep "^tobiko\." | \
+        xargs -r openstack security group delete
+  ignore_errors: yes
+
 - name: "cleanup Glance images created by Tobiko tests"
   shell: |
     source {{ stackrc_file }}
     openstack image list -f value -c 'Name' | \
         grep "^tobiko\." | \
         xargs -r openstack image delete
   ignore_errors: yes
```

### Comparing `tobiko-0.6.8/roles/tobiko-collect/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-collect/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-collect-report/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-collect-report/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-common/defaults/main.yaml` & `tobiko-0.6.9/roles/tobiko-common/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-compile-python/Vagrantfile` & `tobiko-0.6.9/roles/tobiko-compile-python/Vagrantfile`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-compile-python/defaults/main.yaml` & `tobiko-0.6.9/roles/tobiko-compile-python/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-compile-python/tasks/setup_pip.yaml` & `tobiko-0.6.9/roles/tobiko-compile-python/tasks/setup_pip.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-compile-python/tasks/setup_python.yaml` & `tobiko-0.6.9/roles/tobiko-compile-python/tasks/setup_python.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-compile-python/tests/test_py38.yaml` & `tobiko-0.6.9/roles/tobiko-compile-python/tests/test_py38.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-configure/defaults/main.yaml` & `tobiko-0.6.9/roles/tobiko-configure/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-configure/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-configure/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-devstack/tasks/deploy-devstack.yaml` & `tobiko-0.6.9/roles/tobiko-devstack/tasks/deploy-devstack.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-devstack/tasks/deploy-tobiko.yaml` & `tobiko-0.6.9/roles/tobiko-devstack/tasks/deploy-tobiko.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-devstack/tasks/ensure-stack-user.yaml` & `tobiko-0.6.9/roles/tobiko-devstack/tasks/ensure-stack-user.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-devstack/tasks/run-unstack.yaml` & `tobiko-0.6.9/roles/tobiko-devstack/tasks/run-unstack.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-docker-compose/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-docker-compose/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-python3/defaults/main.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-python3/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-python3/files/get_python_info.py` & `tobiko-0.6.9/roles/tobiko-ensure-python3/files/get_python_info.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/ensure-python3.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/ensure-python3.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/install.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/install.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,13 @@
   register: upgrade_python_packages
   changed_when:
     "'Successfully installed' in upgrade_python_packages.stdout"
   loop:
     - pip
     - setuptools
     - wheel
-    - virtualenv
 
 
 - name: "show python_info facts"
   debug:
     msg:
       python_info: '{{ python_info }}'
```

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-python3/tasks/platform.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-python3/tasks/platform.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-ssh-keys/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-ssh-keys/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-ensure-tox/tasks/tox.yaml` & `tobiko-0.6.9/roles/tobiko-ensure-tox/tasks/tox.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-inventory/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-inventory/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-run/tasks/main.yaml` & `tobiko-0.6.9/roles/tobiko-run/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-run/tasks/run.yaml` & `tobiko-0.6.9/roles/tobiko-run/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-check-resources-faults.yaml` & `tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-check-resources-faults.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-designate-faults.yaml` & `tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-faults.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 ---
 
 test_workflow_steps:
-  - tox_description: 'create Designate resources'
-    tox_envlist: designate
-    tox_step_name: create_designate_resources
+  - tox_description: 'run sanity test cases before creating resources'
+    tox_envlist: sanity
+    tox_step_name: before
     tox_environment:
       TOBIKO_PREVENT_CREATE: no
 
-  - tox_description: 'run Designate disruptive test cases'
-    tox_envlist: designate_faults
-    tox_step_name: verify_designate_faults
+  - tox_description: 'create workload resources'
+    tox_envlist: scenario
+    tox_step_name: create_resources
+    tox_environment:
+      TOBIKO_PREVENT_CREATE: no
+
+  - tox_description: 'run disruptive test cases'
+    tox_envlist: faults
+    tox_step_name: faults
+    tox_environment:
+      TOBIKO_PREVENT_CREATE: no
+    pytest_maxfail: 1
+
+  - tox_description: 'run sanity test cases after disruptive tests'
+    tox_envlist: sanity
+    tox_step_name: after
+    tox_environment:
+      TOBIKO_PREVENT_CREATE: no
 
-  - tox_description: 'verify Designate resources'
-    tox_envlist: designate
-    tox_step_name: verify_designate_resources
+  - tox_description: 'verify workload resources'
+    tox_envlist: scenario
+    tox_step_name: verify_resources
     tox_environment:
       TOBIKO_PREVENT_CREATE: yes
```

### Comparing `tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-faults-neutron.yaml` & `tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-faults-neutron.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-faults.yaml` & `tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-gate.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 ---
 
 test_workflow_steps:
-  - tox_description: 'run sanity test cases before creating resources'
-    tox_envlist: sanity
-    tox_step_name: before
-    tox_environment:
-      TOBIKO_PREVENT_CREATE: no
-
   - tox_description: 'create workload resources'
     tox_envlist: scenario
     tox_step_name: create_resources
     tox_environment:
       TOBIKO_PREVENT_CREATE: no
+    test_flaky: true
+
+  - tox_description: 'run sanity test cases before disruptive test cases'
+    tox_envlist: sanity
+    tox_step_name: before_faults
+    tox_environment:
+      TOBIKO_PREVENT_CREATE: no
+    test_flaky: true
 
   - tox_description: 'run disruptive test cases'
     tox_envlist: faults
     tox_step_name: faults
     tox_environment:
       TOBIKO_PREVENT_CREATE: no
-    pytest_maxfail: 1
+    test_flaky: true
 
-  - tox_description: 'run sanity test cases after disruptive tests'
+  - tox_description: 'run sanity test cases after disruptive test cases'
     tox_envlist: sanity
-    tox_step_name: after
+    tox_step_name: after_faults
     tox_environment:
       TOBIKO_PREVENT_CREATE: no
+    test_flaky: true
 
   - tox_description: 'verify workload resources'
     tox_envlist: scenario
     tox_step_name: verify_resources
     tox_environment:
       TOBIKO_PREVENT_CREATE: yes
+    test_flaky: true
```

### Comparing `tobiko-0.6.8/roles/tobiko-run/vars/test-workflow-unit.yaml` & `tobiko-0.6.9/roles/tobiko-run/vars/test-workflow-unit.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-tox/defaults/main.yaml` & `tobiko-0.6.9/roles/tobiko-tox/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/roles/tobiko-tox/tasks/tox.yaml` & `tobiko-0.6.9/roles/tobiko-tox/tasks/tox.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/setup.cfg` & `tobiko-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/setup.py` & `tobiko-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/__init__.py` & `tobiko-0.6.9/tobiko/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/actors/__init__.py` & `tobiko-0.6.9/tobiko/actors/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/actors/_actor.py` & `tobiko-0.6.9/tobiko/actors/_actor.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/actors/_manager.py` & `tobiko-0.6.9/tobiko/actors/_manager.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/actors/_proxy.py` & `tobiko-0.6.9/tobiko/actors/_proxy.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/actors/_request.py` & `tobiko-0.6.9/tobiko/actors/_request.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_background.py` & `tobiko-0.6.9/tobiko/common/_background.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_cached.py` & `tobiko-0.6.9/tobiko/common/_cached.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_case.py` & `tobiko-0.6.9/tobiko/common/_case.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_config.py` & `tobiko-0.6.9/tobiko/common/_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_deprecation.py` & `tobiko-0.6.9/tobiko/common/_deprecation.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_detail.py` & `tobiko-0.6.9/tobiko/common/_detail.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_exception.py` & `tobiko-0.6.9/tobiko/common/_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 LOG = log.getLogger(__name__)
 
 
 class TobikoException(Exception):
     """Base Tobiko Exception.
 
     To use this class, inherit from it and define attribute 'message' string.
-    If **properties parameters is given, then it will format message string
+    If ``properties`` parameters is given, then it will format message string
     using properties as key-word arguments.
 
-    Example:
+    Example::
 
         class MyException(TobikoException):
             message = "This exception occurred because of {reason}"
 
         try:
             raise MyException(reason="something went wrong")
         except MyException as ex:
```

### Comparing `tobiko-0.6.8/tobiko/common/_fixture.py` & `tobiko-0.6.9/tobiko/common/_fixture.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_ini.py` & `tobiko-0.6.9/tobiko/common/_ini.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_loader.py` & `tobiko-0.6.9/tobiko/common/_loader.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_logging.py` & `tobiko-0.6.9/tobiko/common/_logging.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_operation.py` & `tobiko-0.6.9/tobiko/common/_operation.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_os.py` & `tobiko-0.6.9/tobiko/common/_os.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_retry.py` & `tobiko-0.6.9/tobiko/common/_retry.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_select.py` & `tobiko-0.6.9/tobiko/common/_select.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_shelves.py` & `tobiko-0.6.9/tobiko/common/_shelves.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_skip.py` & `tobiko-0.6.9/tobiko/common/_skip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_time.py` & `tobiko-0.6.9/tobiko/common/_time.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_utils.py` & `tobiko-0.6.9/tobiko/common/_utils.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_version.py` & `tobiko-0.6.9/tobiko/common/_version.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/common/_yaml.py` & `tobiko-0.6.9/tobiko/common/_yaml.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/config.py` & `tobiko-0.6.9/tobiko/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,18 @@
                        "runner execution"))]
 
 COMMON_GROUP_NAME = 'common'
 
 COMMON_OPTIONS = [
     cfg.StrOpt('shelves_dir',
                default='~/.tobiko/cache/shelves',
-               help=("Default directory where to look for shelves.")),
+               help="Directory where to look for shelves."),
+    cfg.StrOpt('lock_dir',
+               default='~/.tobiko/cache/lock',
+               help="Directory where lock persistent files will be saved"),
 ]
 
 
 def workspace_config_files(project=None, prog=None):
     project = project or 'tobiko'
     filenames = []
     if prog is not None:
```

### Comparing `tobiko-0.6.8/tobiko/docker/__init__.py` & `tobiko-0.6.9/tobiko/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/docker/_client.py` & `tobiko-0.6.9/tobiko/docker/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/docker/_exception.py` & `tobiko-0.6.9/tobiko/docker/_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/docker/_shell.py` & `tobiko-0.6.9/tobiko/docker/_shell.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/docker/config.py` & `tobiko-0.6.9/tobiko/docker/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/http/__init__.py` & `tobiko-0.6.9/tobiko/http/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/http/_connection.py` & `tobiko-0.6.9/tobiko/http/_connection.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/http/_session.py` & `tobiko-0.6.9/tobiko/http/_session.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/_client.py` & `tobiko-0.6.9/tobiko/openstack/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/designate/__init__.py` & `tobiko-0.6.9/tobiko/openstack/designate/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/designate/_client.py` & `tobiko-0.6.9/tobiko/openstack/designate/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/designate/_constants.py` & `tobiko-0.6.9/tobiko/openstack/designate/_constants.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/designate/_zone.py` & `tobiko-0.6.9/tobiko/openstack/designate/_zone.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/glance/__init__.py` & `tobiko-0.6.9/tobiko/openstack/glance/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/glance/_client.py` & `tobiko-0.6.9/tobiko/openstack/glance/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/glance/_image.py` & `tobiko-0.6.9/tobiko/openstack/glance/_image.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/glance/_io.py` & `tobiko-0.6.9/tobiko/openstack/glance/_io.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/glance/_lzma.py` & `tobiko-0.6.9/tobiko/openstack/glance/_lzma.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/glance/config.py` & `tobiko-0.6.9/tobiko/openstack/glance/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/heat/__init__.py` & `tobiko-0.6.9/tobiko/openstack/heat/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/heat/_client.py` & `tobiko-0.6.9/tobiko/openstack/heat/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/heat/_resource.py` & `tobiko-0.6.9/tobiko/openstack/heat/_resource.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/heat/_stack.py` & `tobiko-0.6.9/tobiko/openstack/heat/_stack.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/heat/_template.py` & `tobiko-0.6.9/tobiko/openstack/heat/_template.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/ironic/__init__.py` & `tobiko-0.6.9/tobiko/openstack/ironic/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/ironic/_client.py` & `tobiko-0.6.9/tobiko/openstack/ironic/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/ironic/_node.py` & `tobiko-0.6.9/tobiko/openstack/ironic/_node.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/__init__.py` & `tobiko-0.6.9/tobiko/openstack/keystone/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/_client.py` & `tobiko-0.6.9/tobiko/openstack/keystone/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/_clouds_file.py` & `tobiko-0.6.9/tobiko/openstack/keystone/_clouds_file.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/_credentials.py` & `tobiko-0.6.9/tobiko/openstack/keystone/_credentials.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/_resource.py` & `tobiko-0.6.9/tobiko/openstack/keystone/_resource.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/_services.py` & `tobiko-0.6.9/tobiko/openstack/keystone/_services.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/_session.py` & `tobiko-0.6.9/tobiko/openstack/keystone/_session.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/keystone/config.py` & `tobiko-0.6.9/tobiko/openstack/keystone/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/metalsmith/__init__.py` & `tobiko-0.6.9/tobiko/openstack/metalsmith/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/metalsmith/_client.py` & `tobiko-0.6.9/tobiko/openstack/metalsmith/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/metalsmith/_instance.py` & `tobiko-0.6.9/tobiko/openstack/metalsmith/_instance.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/__init__.py` & `tobiko-0.6.9/tobiko/openstack/neutron/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 from __future__ import absolute_import
 
 from tobiko.openstack.neutron import _agent
 from tobiko.openstack.neutron import _client
-from tobiko.openstack.neutron import _cidr
 from tobiko.openstack.neutron import _extension
 from tobiko.openstack.neutron import _floating_ip
 from tobiko.openstack.neutron import _port
 from tobiko.openstack.neutron import _quota_set
 from tobiko.openstack.neutron import _network
 from tobiko.openstack.neutron import _router
 from tobiko.openstack.neutron import _security_group
 from tobiko.openstack.neutron import _subnet
+from tobiko.openstack.neutron import _subnet_pool
 
 
 SERVER = 'neutron-server'
 METADATA_IPv4 = '169.254.169.254'
 DHCP_AGENT = _agent.DHCP_AGENT
 L3_AGENT = _agent.L3_AGENT
 METADATA_AGENT = _agent.METADATA_AGENT
@@ -61,18 +61,14 @@
 ServiceUnavailable = _client.ServiceUnavailable
 NeutronClient = _client.NeutronClient
 NeutronClientException = _client.NeutronClientException
 NeutronClientType = _client.NeutronClientType
 neutron_client = _client.neutron_client
 get_neutron_client = _client.get_neutron_client
 
-new_ipv4_cidr = _cidr.new_ipv4_cidr
-new_ipv6_cidr = _cidr.new_ipv6_cidr
-list_subnet_cidrs = _cidr.list_subnet_cidrs
-
 get_networking_extensions = _extension.get_networking_extensions
 missing_networking_extensions = _extension.missing_networking_extensions
 has_networking_extensions = _extension.has_networking_extensions
 skip_if_missing_networking_extensions = (
     _extension.skip_if_missing_networking_extensions)
 
 create_floating_ip = _floating_ip.create_floating_ip
@@ -136,14 +132,22 @@
 get_subnet_id = _subnet.get_subnet_id
 find_subnet = _subnet.find_subnet
 list_subnets = _subnet.list_subnets
 SubnetType = _subnet.SubnetType
 SubnetIdType = _subnet.SubnetIdType
 NoSuchSubnet = _subnet.NoSuchSubnet
 
+SubnetPoolType = _subnet_pool.SubnetPoolType
+SubnetPoolIdType = _subnet_pool.SubnetPoolIdType
+NoSuchSubnetPool = _subnet_pool.NoSuchSubnetPool
+get_subnet_pool = _subnet_pool.get_subnet_pool
+create_subnet_pool = _subnet_pool.create_subnet_pool
+delete_subnet_pool = _subnet_pool.delete_subnet_pool
+find_subnet_pool = _subnet_pool.find_subnet_pool
+
 list_security_groups = _security_group.list_security_groups
 get_security_group = _security_group.get_security_group
 get_default_security_group = _security_group.get_default_security_group
 create_security_group = _security_group.create_security_group
 update_security_group = _security_group.update_security_group
 delete_security_group = _security_group.delete_security_group
 create_security_group_rule = _security_group.create_security_group_rule
```

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_agent.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_agent.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_client.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_extension.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_extension.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_floating_ip.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_floating_ip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_network.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_network.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_port.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_port.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_quota_set.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_quota_set.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_router.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_router.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_security_group.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_security_group.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/_subnet.py` & `tobiko-0.6.9/tobiko/openstack/neutron/_subnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import typing
 
 import netaddr
 
 import tobiko
 from tobiko.openstack.neutron import _client
 from tobiko.openstack.neutron import _network
-from tobiko.openstack.neutron import _cidr
 
 
 SubnetType = typing.Dict[str, typing.Any]
 SubnetIdType = typing.Union[str, SubnetType]
 
 
 def get_subnet_id(subnet: SubnetIdType) -> str:
@@ -46,33 +45,24 @@
         raise NoSuchSubnet(id=subnet_id) from ex
 
 
 def create_subnet(client: _client.NeutronClientType = None,
                   network: _network.NetworkIdType = None,
                   add_cleanup=True,
                   ip_version=4,
-                  cidr: str = None,
                   **params) -> SubnetType:
     if 'network_id' not in params:
         if network is None:
             from tobiko.openstack import stacks
             network_id = tobiko.setup_fixture(
                 stacks.NetworkStackFixture).network_id
         else:
             network_id = _network.get_network_id(network)
         params['network_id'] = network_id
     params['ip_version'] = ip_version
-    if cidr is None:
-        if ip_version == 4:
-            cidr = _cidr.new_ipv4_cidr()
-        elif ip_version == 6:
-            cidr = _cidr.new_ipv6_cidr()
-        else:
-            raise ValueError(f'Invalid ip version: {ip_version}')
-    params['cidr'] = cidr
     subnet = _client.neutron_client(client).create_subnet(
         body={'subnet': params})['subnet']
     if add_cleanup:
         tobiko.add_cleanup(cleanup_subnet, subnet=subnet, client=client)
     return subnet
```

### Comparing `tobiko-0.6.8/tobiko/openstack/neutron/config.py` & `tobiko-0.6.9/tobiko/openstack/neutron/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,22 @@
     cfg.StrOpt('ipv4_cidr',
                default='10.100.0.0/16',
                help="The CIDR block to allocate IPv4 subnets from"),
     cfg.IntOpt('ipv4_prefixlen',
                default=24,
                help="The mask bits for IPv4 subnets"),
     cfg.ListOpt('ipv4_dns_nameservers',
-                default=None,
+                # This value is a workaround to avoid UbuntuExternalPortTest
+                # failures - with certain ubuntu images, routes to the
+                # nameservers were added to a VLAN interface, breaking
+                # connectivity from the VMs to the external network.
+                default=["8.8.8.8"],
                 help="List of nameservers IPv4 addresses"),
     cfg.StrOpt('ipv6_cidr',
-               default='2001:db8::/48',
+               default='fc00::/48',
                help="The CIDR block to allocate IPv6 subnets from"),
     cfg.IntOpt('ipv6_prefixlen',
                default=64,
                help="The mask bits for IPv6 subnets"),
     cfg.ListOpt('ipv6_dns_nameservers',
                 default=None,
                 help="List of nameservers IPv6 addresses"),
```

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/__init__.py` & `tobiko-0.6.9/tobiko/openstack/nova/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_client.py` & `tobiko-0.6.9/tobiko/openstack/nova/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_cloud_init.py` & `tobiko-0.6.9/tobiko/openstack/nova/_cloud_init.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_hypervisor.py` & `tobiko-0.6.9/tobiko/openstack/nova/_hypervisor.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_key_file.py` & `tobiko-0.6.9/tobiko/openstack/nova/_key_file.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_quota_set.py` & `tobiko-0.6.9/tobiko/openstack/nova/_quota_set.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_server.py` & `tobiko-0.6.9/tobiko/openstack/nova/_server.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/_service.py` & `tobiko-0.6.9/tobiko/openstack/nova/_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 from __future__ import absolute_import
 
 import json
 import typing
 
+from keystoneauth1 import exceptions as ks_exceptions
+from novaclient import exceptions as nc_exceptions
 from oslo_log import log
 
 import tobiko
 from tobiko.openstack.nova import _client
 
 
 LOG = log.getLogger(__name__)
@@ -44,15 +46,21 @@
 
 
 def wait_for_services_up(retry: typing.Optional[tobiko.Retry] = None,
                          **list_services_params):
     for attempt in tobiko.retry(other_retry=retry,
                                 default_timeout=300.,
                                 default_interval=5.):
-        services = _client.list_services(**list_services_params)
+        try:
+            services = _client.list_services(**list_services_params)
+        except (ks_exceptions.connection.ConnectFailure,
+                nc_exceptions.ClientException):
+            # Re-raises this exception in case this is the last attempt
+            attempt.check_limits()
+            continue
         LOG.debug(f"Found {len(services)} Nova services")
         try:
             if not services:
                 raise NovaServicesNotfound(
                     attributes=json.dumps(list_services_params))
 
             heathy_services = services.with_attributes(state='up')
@@ -66,11 +74,10 @@
                 details = services_details(failed_services)
                 LOG.info(f"Failed Nova services:\n{details}")
                 raise NovaServicesFailed(details=details)
             LOG.info('All nova services are up!')
             break  # all Nova services are healthy
 
         except NovaServiceException:
-            # Re-raises this exception in case this is the last retry
-            # attempt
+            # Re-raises this exception in case this is the last attempt
             attempt.check_limits()
             continue
```

### Comparing `tobiko-0.6.8/tobiko/openstack/nova/config.py` & `tobiko-0.6.9/tobiko/openstack/nova/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/__init__.py` & `tobiko-0.6.9/tobiko/openstack/octavia/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_amphora.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_amphora.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_client.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_constants.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_constants.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_exceptions.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_exceptions.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_load_balancer.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_load_balancer.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_validators.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_validators.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/_waiters.py` & `tobiko-0.6.9/tobiko/openstack/octavia/_waiters.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/octavia/config.py` & `tobiko-0.6.9/tobiko/openstack/octavia/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/__init__.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_client.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_exception.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_log.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_log.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_network.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_network.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_port.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_port.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_security_group.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_security_group.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_security_group_rule.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_security_group_rule.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/openstackclient/_subnet.py` & `tobiko-0.6.9/tobiko/openstack/openstackclient/_subnet.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/__init__.py` & `tobiko-0.6.9/tobiko/openstack/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_centos.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_centos.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_cirros.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_cirros.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_designate.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_designate.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_fedora.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_fedora.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_hot.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_hot.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_l3ha.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_l3ha.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_neutron.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_neutron.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 from __future__ import absolute_import
 
 import json
+import os
 import typing
 
 import netaddr
+from oslo_concurrency import lockutils
 from oslo_log import log
 
 import tobiko
 from tobiko import config
 from tobiko.openstack import heat
 from tobiko.openstack import neutron
 from tobiko.openstack.stacks import _hot
 from tobiko.shell import ip
 from tobiko.shell import sh
 from tobiko.shell import ssh
 
 
 CONF = config.CONF
 LOG = log.getLogger(__name__)
+LOCK_DIR = os.path.expanduser(CONF.tobiko.common.lock_dir)
 
 
 class ExternalNetworkStackFixture(heat.HeatStackFixture):
 
     template = _hot.heat_template_file('neutron/external_network.yaml')
 
     @property
@@ -268,47 +271,144 @@
     return create_router_interface_func(router=router,
                                         subnet=subnet,
                                         network=network,
                                         client=client,
                                         add_cleanup=add_cleanup)
 
 
+@neutron.skip_if_missing_networking_extensions('subnet_allocation')
+class SubnetPoolFixture(tobiko.SharedFixture):
+    """Neutron Subnet Pool Fixture.
+
+    A subnet pool is a dependency of network fixtures with either IPv4 or
+    IPv6 subnets (or both). The CIDRs for those subnets are obtained from this
+    resource.
+    NOTE: this fixture does not represent a heat stack, but it is under the
+    stacks module until a decision is taken on where this kind of fixtures are
+    located
+    """
+
+    name: typing.Optional[str] = None
+    prefixes: list = [CONF.tobiko.neutron.ipv4_cidr]
+    default_prefixlen: int = CONF.tobiko.neutron.ipv4_prefixlen
+    _subnet_pool: typing.Optional[neutron.SubnetPoolType] = None
+
+    def __init__(self,
+                 name: typing.Optional[str] = None,
+                 prefixes: typing.Optional[list] = None,
+                 default_prefixlen: typing.Optional[int] = None):
+        self.name = name or self.fixture_name
+        if prefixes:
+            self.prefixes = prefixes
+        if default_prefixlen:
+            self.default_prefixlen = default_prefixlen
+        super().__init__()
+
+    @property
+    def ip_version(self):
+        valid_versions = (4, 6)
+        for valid_version in valid_versions:
+            if len(self.prefixes) > 0 and all(
+                    netaddr.IPNetwork(prefix).version == valid_version
+                    for prefix in self.prefixes):
+                return valid_version
+        # return None when neither IPv4 nor IPv6 (or when both)
+        return None
+
+    def setup_fixture(self):
+        if config.get_bool_env('TOBIKO_PREVENT_CREATE'):
+            LOG.debug("SubnetPoolFixture should have been already created: %r",
+                      self.subnet_pool)
+        else:
+            self.try_create_subnet_pool()
+
+        if self.subnet_pool:
+            tobiko.addme_to_shared_resource(__name__, self.name)
+
+    @lockutils.synchronized(
+        'create_subnet_pool', external=True, lock_path=LOCK_DIR)
+    def try_create_subnet_pool(self):
+        if not self.subnet_pool:
+            self._subnet_pool = neutron.create_subnet_pool(
+                name=self.name, prefixes=self.prefixes,
+                default_prefixlen=self.default_prefixlen, add_cleanup=False)
+
+    def cleanup_fixture(self):
+        n_tests_using_resource = len(tobiko.removeme_from_shared_resource(
+             __name__, self.name))
+        if n_tests_using_resource == 0:
+            self._cleanup_subnet_pool()
+        else:
+            LOG.info('Subnet Pool %r not deleted because %d tests '
+                     'are using it still.',
+                     self.name, n_tests_using_resource)
+
+    def _cleanup_subnet_pool(self):
+        sp_id = self.subnet_pool_id
+        if sp_id:
+            self._subnet_pool = None
+            LOG.debug('Deleting Subnet Pool %r (%r)...',
+                      self.name, sp_id)
+            neutron.delete_subnet_pool(sp_id)
+            LOG.debug('Subnet Pool %r (%r) deleted.', self.name, sp_id)
+
+    @property
+    def subnet_pool_id(self):
+        if self.subnet_pool:
+            return self._subnet_pool['id']
+
+    @property
+    def subnet_pool(self):
+        if not self._subnet_pool:
+            try:
+                self._subnet_pool = neutron.find_subnet_pool(name=self.name)
+            except neutron.NoSuchSubnetPool:
+                LOG.debug("Subnet Pool %r not found.", self.name)
+                self._subnet_pool = None
+        return self._subnet_pool
+
+
+class SubnetPoolIPv6Fixture(SubnetPoolFixture):
+    prefixes: list = [CONF.tobiko.neutron.ipv6_cidr]
+    default_prefixlen: int = CONF.tobiko.neutron.ipv6_prefixlen
+
+
 @neutron.skip_if_missing_networking_extensions('port-security')
 class NetworkStackFixture(heat.HeatStackFixture):
     """Heat stack for creating internal network with a router to external"""
+    subnet_pools_ipv4_stack = (tobiko.required_fixture(SubnetPoolFixture)
+                               if bool(CONF.tobiko.neutron.ipv4_cidr)
+                               else None)
+    subnet_pools_ipv6_stack = (tobiko.required_fixture(SubnetPoolIPv6Fixture)
+                               if bool(CONF.tobiko.neutron.ipv6_cidr)
+                               else None)
 
     #: Heat template file
     template = _hot.heat_template_file('neutron/network.yaml')
 
     #: Enable port security by default for new network ports
     port_security_enabled = True
 
     @property
     def has_ipv4(self):
         """Whenever to setup IPv4 subnet"""
         return bool(CONF.tobiko.neutron.ipv4_cidr)
 
     @property
-    def ipv4_cidr(self):
-        if self.has_ipv4:
-            return neutron.new_ipv4_cidr(seed=self.fixture_name)
-        else:
-            return None
-
-    @property
     def has_ipv6(self):
         """Whenever to setup IPv6 subnet"""
         return bool(CONF.tobiko.neutron.ipv6_cidr)
 
     @property
-    def ipv6_cidr(self):
-        if self.has_ipv6:
-            return neutron.new_ipv6_cidr(seed=self.fixture_name)
-        else:
-            return None
+    def subnet_pool_ipv4_id(self):
+        return self.subnet_pools_ipv4_stack.subnet_pool_id
+
+    @property
+    def subnet_pool_ipv6_id(self):
+        return self.subnet_pools_ipv6_stack.subnet_pool_id
 
     @property
     def network_value_specs(self):
         """Extra network creation parameters"""
         return {}
 
     gateway_stack = tobiko.required_fixture(RouterStackFixture)
@@ -533,25 +633,36 @@
         if description:
             self.description = description
         if rules:
             self.rules = rules
         super(StatelessSecurityGroupFixture, self).__init__()
 
     def setup_fixture(self):
+        if config.get_bool_env('TOBIKO_PREVENT_CREATE'):
+            LOG.debug("StatelessSecurityGroupFixture should have been already "
+                      "created: %r", self.security_group)
+        else:
+            self.try_create_security_group()
+
+        if self.security_group:
+            tobiko.addme_to_shared_resource(__name__, self.name)
+
+    @lockutils.synchronized(
+        'create_security_group', external=True, lock_path=LOCK_DIR)
+    def try_create_security_group(self):
         if not self.security_group:
             self._security_group = neutron.create_security_group(
                 name=self.name, description=self.description,
                 add_cleanup=False, stateful=False)
-        if self.security_group:
+            # add rules once the SG was created
             for rule in self.rules:
                 neutron.create_security_group_rule(
                     self._security_group['id'],
                     add_cleanup=False,
                     **rule)
-            tobiko.addme_to_shared_resource(__name__, self.name)
 
     def cleanup_fixture(self):
         n_tests_using_stack = len(tobiko.removeme_from_shared_resource(
              __name__, self.name))
         if n_tests_using_stack == 0:
             self._cleanup_security_group()
         else:
@@ -572,19 +683,20 @@
     def security_group_id(self):
         if self.security_group:
             return self._security_group['id']
 
     @property
     def security_group(self):
         if not self._security_group:
-            try:
-                self._security_group = neutron.get_security_group(self.name)
-            except neutron.NotFound:
+            sgs = neutron.list_security_groups(name=self.name)
+            if len(sgs) == 0:
                 LOG.debug("Security group %r not found.", self.name)
                 self._security_group = None
+            else:
+                self._security_group = sgs.unique
         return self._security_group
 
 
 def list_external_networks(name: str = None) -> \
         tobiko.Selection[neutron.NetworkType]:
     networks = tobiko.Selection[neutron.NetworkType]()
     if name is not None:
```

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_nova.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_octavia.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_octavia.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_qos.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_qos.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_redhat.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_redhat.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_ubuntu.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_ubuntu.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,23 +56,25 @@
 
 class UbuntuImageFixture(UbuntuMinimalImageFixture,
                          glance.CustomizedGlanceImageFixture):
     """Ubuntu server image running an HTTP server
 
     The server has additional installed packages compared to
     the minimal one:
-      - iperf3
-      - ping
-      - ncat
-      - nginx
-      - vlan
+
+    - iperf3
+    - ping
+    - ncat
+    - nginx
+    - vlan
 
     The image will also have below running services:
-      - nginx HTTP server listening on TCP port 80
-      - iperf3 server listening on TCP port 5201
+
+    - nginx HTTP server listening on TCP port 80
+    - iperf3 server listening on TCP port 5201
     """
 
     def __init__(self,
                  ethernet_devide: str = None,
                  **kwargs):
         super().__init__(**kwargs)
         self._ethernet_device = ethernet_devide
@@ -185,16 +187,17 @@
 
 
 class UbuntuServerStackFixture(UbuntuMinimalServerStackFixture,
                                _vlan.VlanServerStackFixture):
     """Ubuntu server running an HTTP server
 
     The server has additional commands compared to the minimal one:
-      iperf3
-      ping
+
+    - iperf3
+    - ping
     """
 
     #: Glance image used to create a Nova server instance
     image_fixture = tobiko.required_fixture(UbuntuImageFixture)
 
     # I expect Ubuntu based servers to be slow to boot
     is_reachable_timeout = 900.
```

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/_vlan.py` & `tobiko-0.6.9/tobiko/openstack/stacks/_vlan.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/designate/zone.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/designate/zone.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/neutron/external_network.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/neutron/external_network.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/neutron/floating_ip.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/neutron/floating_ip.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/neutron/network.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/neutron/network.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -23,25 +23,21 @@
     default: false
 
   has_ipv6:
     description: Whenever to create IPv6 subnet
     type: boolean
     default: false
 
-  ipv4_cidr:
-    description: IPv4 subnet CIDR to be assigned to new network
+  subnet_pool_ipv4_id:
+    description: IPv4 Subnet Pool ID
     type: string
-    constraints:
-      - custom_constraint: net_cidr
 
-  ipv6_cidr:
-    description: IPv6 subnet CIDR to be assigned to new network
+  subnet_pool_ipv6_id:
+    description: IPv6 Subnet Pool ID
     type: string
-    constraints:
-      - custom_constraint: net_cidr
 
   ipv4_dns_nameservers:
     description: IPv4 nameservers IP addresses
     type: comma_delimited_list
     default: ''
 
   ipv6_dns_nameservers:
@@ -121,24 +117,24 @@
 
   _ipv4_subnet:
     type: OS::Neutron::Subnet
     condition: has_ipv4
     properties:
       network: {get_resource: _network}
       ip_version: 4
-      cidr: {get_param: ipv4_cidr}
+      subnetpool: {get_param: subnet_pool_ipv4_id}
       dns_nameservers: {get_param: ipv4_dns_nameservers}
 
   _ipv6_subnet:
     type: OS::Neutron::Subnet
     condition: has_ipv6
     properties:
       network: {get_resource: _network}
       ip_version: 6
-      cidr: {get_param: ipv6_cidr}
+      subnetpool: {get_param: subnet_pool_ipv6_id}
       dns_nameservers: {get_param: ipv6_dns_nameservers}
       ipv6_address_mode: {get_param: ipv6_address_mode}
       ipv6_ra_mode: {get_param: ipv6_ra_mode}
 
   _gateway:
     type: OS::Neutron::Router
     condition: has_gateway
```

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/neutron/qos.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/neutron/qos.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/neutron/router_interface.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/neutron/router_interface.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/neutron/security_groups.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/neutron/security_groups.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/nova/flavor.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/nova/flavor.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/nova/key_pair.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/nova/key_pair.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/nova/multi_ip_test_stack.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/nova/multi_ip_test_stack.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/nova/server.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/nova/server.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/nova/server_group.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/nova/server_group.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/octavia/listener.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/octavia/listener.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/octavia/load_balancer.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/octavia/load_balancer.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/octavia/member.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/octavia/member.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/stacks/octavia/pool.yaml` & `tobiko-0.6.9/tobiko/openstack/stacks/octavia/pool.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/tests/__init__.py` & `tobiko-0.6.9/tobiko/openstack/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/tests/_neutron.py` & `tobiko-0.6.9/tobiko/openstack/tests/_neutron.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,47 +93,66 @@
         break
     else:
         raise RuntimeError("Retry loop broken")
 
     return agents
 
 
-def test_alive_agents_are_consistent_along_time(previous_alive_agents=None):
-    test_case = tobiko.get_test_case()
-    if previous_alive_agents is None:
-        # the following dict of agents is obtained when:
-        # - the list_agents request is replied with 200
-        # - the list is not empty
-        # - no agents are dead
-        alive_agents = {agent['id']: agent
-                        for agent in test_neutron_agents_are_alive()}
-    else:
-        alive_agents = previous_alive_agents
+def test_alive_agents_are_consistent_along_time(retry_timeout=180.,
+                                                retry_interval=5.,
+                                                consistent_sleep=5.,
+                                                consistent_count=5,):
+    # the following dict of agents is obtained when:
+    # - the list_agents request is replied with 200
+    # - the list is not empty
+    # - no agents are dead
+    alive_agents = {agent['id']: agent
+                    for agent in test_neutron_agents_are_alive()}
+
+    for attempt_out in tobiko.retry(timeout=retry_timeout,
+                                    interval=retry_interval):
+        LOG.debug('trying to obtain a consistent list of alive neutron agents '
+                  f'for {consistent_count} times')
+        for attempt_in in tobiko.retry(sleep_time=consistent_sleep,
+                                       count=consistent_count):
+            try:
+                agents = neutron.list_agents()
+            except (neutron.ServiceUnavailable,
+                    neutron.NeutronClientException,
+                    exceptions.connection.ConnectFailure):
+                LOG.exception('Error obtaining the list of neutron agents')
+                # go to the outer loop, if its timeout didn't expire yet
+                # the alive_agents reference is the previous list
+                break
+            actual = {agent['id']: agent for agent in agents}
 
-    for attempt in tobiko.retry(sleep_time=5., count=5):
-        agents = neutron.list_agents()
-        actual = {agent['id']: agent
-                  for agent in agents}
-
-        # any dead agents? If yes, fail now
-        dead_agents = agents.with_items(alive=False)
-        test_case.assertEqual(
-            [], dead_agents, "Some neutron agents died")
-
-        if len(actual) > len(alive_agents):
-            LOG.debug('Some new agents appeared! It seems not all the agents '
-                      'had been started yet, so let\'s restart this check')
-            return test_alive_agents_are_consistent_along_time(actual)
-
-        # any agent disappeared? If yes, fail now
-        test_case.assertEqual(
-            set(alive_agents), set(actual), 'Some agents disappeared')
+            # any dead agents? If yes, go to the outer loop
+            # the alive_agents reference is the previous list
+            dead_agents = agents.with_items(alive=False)
+            if len(dead_agents) > 0:
+                LOG.warn(f'Some dead agents have been found: {dead_agents}')
+                break
 
-        if attempt.is_last:
-            break
+            # go to the outer loop if the set of agents changed
+            # the alive_agents reference is the new list
+            if set(actual) != set(alive_agents):
+                alive_agents = actual
+                LOG.warn("The list of agents has changed")
+                break
+
+            LOG.debug("The new list of agents matched the previous list "
+                      "%d times", attempt_in.number + 1)
+
+            if attempt_in.is_last:
+                LOG.info(f"the list of agents obtained for {consistent_count} "
+                         "times was consistent - the test passes")
+                return
+
+        if attempt_out.is_last:
+            tobiko.fail("No consistent neutron agent results obtained")
 
 
 def ovn_dbs_vip_bindings(test_case):
     ovn_conn_str = get_ovn_db_connections()
     # ovn db sockets might be centrillized or distributed
     # that depends on the openstack version under test
     sockets_centrallized = topology.verify_osp_version('14.0', lower=True)
@@ -607,44 +626,53 @@
         {}, interfaces,
         f"OVS interface(s) found on OpenStack nodes: {interfaces}")
 
 
 def cleanup_ports_network(port_count):
     # This function cleans up the ports and the created network
     for _ in range(port_count):
+        port_name = f'tobiko_ovn_leader_test_port-{_}'
         try:
-            port = neutron.find_port(name=f'tobiko_ovn_leader_test_port-{_}')
+            port = neutron.find_port(name=port_name)
             neutron.delete_port(port=port['id'])
-        except neutron.NoSuchPort:
-            LOG.debug("No Such port found")
+            LOG.debug("Port deleted: %s", port_name)
+        except (neutron.NoSuchPort, tobiko.ObjectNotFound):
+            LOG.debug("No Such port found: %s", port_name)
     network = neutron.find_network(name='tobiko_ovn_leader_test_network')
     neutron.delete_network(network=network)
 
 
 def check_port_created(port_count):
     # This function checks the number of ports created
     test_case = tobiko.get_test_case()
     port_count_created = 0
     for _ in range(port_count):
+        port_name = f'tobiko_ovn_leader_test_port-{_}'
         try:
-            port = neutron.find_port(name=f'tobiko_ovn_leader_test_port-{_}')
+            port = neutron.find_port(name=port_name)
             if port:
                 port_count_created += 1
-        except neutron.NoSuchPort:
-            LOG.debug("No Such port found")
+                LOG.debug("Port found: %s", port_name)
+        except (neutron.NoSuchPort, tobiko.ObjectNotFound):
+            LOG.debug("No Such port found: %s", port_name)
     test_case.assertEqual(port_count_created, port_count)
 
 
 def create_multiple_port_network(port_count):
     # This function is run in threading mode
-    session = keystone.get_keystone_session()
+    session = keystone.get_keystone_session(shared=False)
     client = neutron.get_neutron_client(session=session)
     network = neutron.create_network(client=client, add_cleanup=False,
                                      name='tobiko_ovn_leader_test_network')
     for _ in range(port_count):
+        # different clients are needed for the requests that are sent in
+        # parallel processes running in background
+        # with a common client, an SSLError exception is raised
+        session = keystone.get_keystone_session(shared=False)
+        client = neutron.get_neutron_client(session=session)
         # Multiple requests are sent in background mode to save time
         # and not to wait till the control returns
         sh.start_background_process(bg_function=neutron.create_port,
                                     bg_process_name=f"create_port-{_}",
                                     client=client, network=network,
                                     add_cleanup=False,
                                     name=f'tobiko_ovn_leader_test_port-{_}')
```

### Comparing `tobiko-0.6.8/tobiko/openstack/tests/_nova.py` & `tobiko-0.6.9/tobiko/openstack/tests/_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/__init__.py` & `tobiko-0.6.9/tobiko/openstack/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_address.py` & `tobiko-0.6.9/tobiko/openstack/topology/_address.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_assert.py` & `tobiko-0.6.9/tobiko/openstack/topology/_assert.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_config.py` & `tobiko-0.6.9/tobiko/openstack/topology/_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_connection.py` & `tobiko-0.6.9/tobiko/openstack/topology/_connection.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_exception.py` & `tobiko-0.6.9/tobiko/openstack/topology/_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_namespace.py` & `tobiko-0.6.9/tobiko/openstack/topology/_namespace.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_neutron.py` & `tobiko-0.6.9/tobiko/openstack/topology/_neutron.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_sh.py` & `tobiko-0.6.9/tobiko/openstack/topology/_sh.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/_topology.py` & `tobiko-0.6.9/tobiko/openstack/topology/_topology.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,15 +721,15 @@
 
 def verify_osp_version(required_version, higher=False, lower=False):
     try:
         current_version = get_openstack_version()
     except Exception:
         current_version = None
     if current_version is None:
-        return False
+        return True
 
     required_version_parsed = version.parse(required_version)
     current_version_parsed = version.parse(current_version)
 
     if higher and lower:
         raise RuntimeError
     elif not higher and not lower:  # this means equal
```

### Comparing `tobiko-0.6.8/tobiko/openstack/topology/config.py` & `tobiko-0.6.9/tobiko/openstack/topology/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/__init__.py` & `tobiko-0.6.9/tobiko/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_client.py` & `tobiko-0.6.9/tobiko/podman/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_exception.py` & `tobiko-0.6.9/tobiko/podman/_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/LICENSE` & `tobiko-0.6.9/tobiko/podman/_podman1/LICENSE`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/README.md` & `tobiko-0.6.9/tobiko/podman/_podman1/README.md`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/__init__.py` & `tobiko-0.6.9/tobiko/podman/_podman1/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/client.py` & `tobiko-0.6.9/tobiko/podman/_podman1/client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/__init__.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/_containers_attach.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/_containers_attach.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/_containers_start.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/_containers_start.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/containers.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/containers.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/errors.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/errors.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/images.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/images.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/pods.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/pods.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/system.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/system.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_podman1/libs/tunnel.py` & `tobiko-0.6.9/tobiko/podman/_podman1/libs/tunnel.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/podman/_shell.py` & `tobiko-0.6.9/tobiko/podman/_shell.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/__init__.py` & `tobiko-0.6.9/tobiko/run/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/_config.py` & `tobiko-0.6.9/tobiko/run/_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/_discover.py` & `tobiko-0.6.9/tobiko/run/_discover.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/_find.py` & `tobiko-0.6.9/tobiko/run/_find.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/_result.py` & `tobiko-0.6.9/tobiko/run/_result.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/_run.py` & `tobiko-0.6.9/tobiko/run/_run.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/run/_worker.py` & `tobiko-0.6.9/tobiko/run/_worker.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ansible/__init__.py` & `tobiko-0.6.9/tobiko/shell/ansible/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ansible/_playbook.py` & `tobiko-0.6.9/tobiko/shell/ansible/_playbook.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ansible/config.py` & `tobiko-0.6.9/tobiko/shell/ansible/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/curl/__init__.py` & `tobiko-0.6.9/tobiko/shell/curl/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/curl/_execute.py` & `tobiko-0.6.9/tobiko/shell/curl/_execute.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/curl/_process.py` & `tobiko-0.6.9/tobiko/shell/curl/_process.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/files/__init__.py` & `tobiko-0.6.9/tobiko/shell/files/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/files/_logs.py` & `tobiko-0.6.9/tobiko/shell/files/_logs.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/find.py` & `tobiko-0.6.9/tobiko/shell/find.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/grep.py` & `tobiko-0.6.9/tobiko/shell/grep.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ifconfig.py` & `tobiko-0.6.9/tobiko/shell/ifconfig.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ip.py` & `tobiko-0.6.9/tobiko/shell/ip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/iperf3/__init__.py` & `tobiko-0.6.9/tobiko/shell/iperf3/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/iperf3/_assert.py` & `tobiko-0.6.9/tobiko/shell/iperf3/_assert.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/iperf3/_execute.py` & `tobiko-0.6.9/tobiko/shell/iperf3/_execute.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/iperf3/_interface.py` & `tobiko-0.6.9/tobiko/shell/iperf3/_interface.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/iperf3/_parameters.py` & `tobiko-0.6.9/tobiko/shell/iperf3/_parameters.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/iperf3/config.py` & `tobiko-0.6.9/tobiko/shell/iperf3/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ping/__init__.py` & `tobiko-0.6.9/tobiko/shell/ping/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ping/_assert.py` & `tobiko-0.6.9/tobiko/shell/ping/_assert.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ping/_exception.py` & `tobiko-0.6.9/tobiko/shell/ping/_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ping/_interface.py` & `tobiko-0.6.9/tobiko/shell/ping/_interface.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ping/_parameters.py` & `tobiko-0.6.9/tobiko/shell/ping/_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,55 +67,45 @@
                     fragmentation=None,
                     host: typing.Optional[PingAddressType] = None,
                     interval=None, ip_version=None, packet_size=None,
                     source=None, timeout=None, network_namespace=None):
     """Validate parameters and initialize a new PingParameters instance
 
     :param default: (PingParameters or None) instance from where to take
-    default values when other value is not provided. If None (that is the
-    default value) it will copy default parameters from
-    DEFAULT_PING_PARAMETERS
-
+        default values when other value is not provided. If None (that is the
+        default value) it will copy default parameters from
+        DEFAULT_PING_PARAMETERS
     :param count: (int or None) number of ping ICMP message expecting to be
-    received before having a success. Default value can be configured using
-    'count' option in [ping] config section.
-
+        received before having a success. Default value can be configured using
+        'count' option in [ping] config section.
     :param host: (str or None) IP address or host name to send ICMP
-    messages to. It is required to format a valid ping command, therefore
-    no default value exists for this parameter.
-
+        messages to. It is required to format a valid ping command, therefore
+        no default value exists for this parameter.
     :param deadline: (int or None) positive number representing the maximum
-    number of seconds ping command can send ICMP messages before stop
-    executing. Default value can be configured using 'deadline' option
-    in [ping] config section.
-
+        number of seconds ping command can send ICMP messages before stop
+        executing. Default value can be configured using 'deadline' option in
+        [ping] config section.
     :param fragmentation: (bool or None) when False this would tell ping
-    to forbid ICMP messages fragmentation. Default value can be configured
-    using 'fragmentation' option in [ping] config section. Fragmentation can't
-    be disabled when using ping provided by BusyBox (IE with CirrOS images).
-
+        to forbid ICMP messages fragmentation. Default value can be configured
+        using 'fragmentation' option in [ping] config section. Fragmentation
+        can't be disabled when using ping provided by BusyBox (IE with CirrOS
+        images).
     :param interval: (int or None) interval of time before sending following
-    ICMP message. Default value can be configured using 'interval' option
-    in [ping] config section.
-
+        ICMP message. Default value can be configured using 'interval' option
+        in [ping] config section.
     :param ip_version: (4, 6 or None) If not None it makes sure it will
-    use specified IP version for sending ICMP packages.
-
+        use specified IP version for sending ICMP packages.
     :param packet_size: (int or None) if not None, it specifies the total ICMP
-    message size (headers + payload).
-
+        message size (headers + payload).
     :param source: (str or None) IP address or interface name from where
-    to send ICMP message.
-
+        to send ICMP message.
     :param timeout: (int or None) time in seconds after which ping operation
-    would raise PingFailed exception.
-
+        would raise PingFailed exception.
     :raises TypeError: in case some parameter cannot be converted to right
-    expected type
-
+        expected type
     :raises ValueError: in case some parameter has an unexpected value
     """
 
     if default is None:
         default = default_ping_parameters()
 
     return PingParameters(
```

### Comparing `tobiko-0.6.8/tobiko/shell/ping/_ping.py` & `tobiko-0.6.9/tobiko/shell/ping/_ping.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 
 def ping(host: PingHostType, until=TRANSMITTED, check: bool = True,
          **ping_params) -> _statistics.PingStatistics:
     """Send ICMP messages to host address until timeout
 
     :param host: destination host address
-    :param **ping_params: parameters to be forwarded to get_statistics()
+    :param ping_params: parameters to be forwarded to :mod:`get_statistics`
         function
     :returns: PingStatistics
     """
     return get_statistics(host=host, until=until, check=check, **ping_params)
 
 
 def ping_until_delivered(host, **ping_params):
@@ -148,15 +148,15 @@
 
     Send 'count' ICMP messages
 
     ICMP messages are considered delivered when they have been
     transmitted without being counted as errors.
 
     :param host: destination host address
-    :param **ping_params: parameters to be forwarded to get_statistics()
+    :param ping_params: parameters to be forwarded to :mod:`get_statistics`
         function
     :returns: PingStatistics
     :raises: PingFailed in case timeout expires before delivering all
         expected count messages
     """
     return ping(host=host, until=DELIVERED, **ping_params)
 
@@ -167,15 +167,15 @@
     Send ICMP messages until it fails to deliver 'count' messages
 
     ICMP messages are considered undelivered when they have been
     transmitted and they have been counted as error in ping statistics (for
     example because of errors into the route to remote address).
 
     :param host: destination host address
-    :param **ping_params: parameters to be forwarded to get_statistics()
+    :param ping_params: parameters to be forwarded to :mod:`get_statistics`
         function
     :returns: PingStatistics
     :raises: PingFailed in case timeout expires before failing delivering
         expected 'count' of messages
     """
     return ping(host=host, until=UNDELIVERED, **ping_params)
 
@@ -185,15 +185,15 @@
 
     Send ICMP messages until it receives 'count' messages back
 
     ICMP messages are considered received when they have been
     transmitted without any routing errors and they are received back
 
     :param host: destination host address
-    :param **ping_params: parameters to be forwarded to get_statistics()
+    :param ping_params: parameters to be forwarded to :mod:`get_statistics`
         function
     :returns: PingStatistics
     :raises: PingFailed in case timeout expires before receiving all
         expected 'count' of messages
     """
     return ping(host=host, until=RECEIVED, **ping_params)
 
@@ -204,15 +204,15 @@
     Send ICMP messages until it fails to receive 'count' messages back.
 
     ICMP messages are considered unreceived when they have been
     transmitted without any routing error but they failed to be received
     back (for example because of network filtering).
 
     :param host: destination host address
-    :param **ping_params: parameters to be forwarded to get_statistics()
+    :param ping_params: parameters to be forwarded to :mod:`get_statistics`
         function
     :returns: PingStatistics
     :raises: PingFailed in case timeout expires before failed receiving
         expected 'count' of messages
     """
     return ping(host=host, until=UNRECEIVED, **ping_params)
```

### Comparing `tobiko-0.6.8/tobiko/shell/ping/_statistics.py` & `tobiko-0.6.9/tobiko/shell/ping/_statistics.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ping/config.py` & `tobiko-0.6.9/tobiko/shell/ping/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/__init__.py` & `tobiko-0.6.9/tobiko/shell/sh/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_cmdline.py` & `tobiko-0.6.9/tobiko/shell/sh/_cmdline.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_command.py` & `tobiko-0.6.9/tobiko/shell/sh/_command.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_connection.py` & `tobiko-0.6.9/tobiko/shell/sh/_connection.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_exception.py` & `tobiko-0.6.9/tobiko/shell/sh/_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_execute.py` & `tobiko-0.6.9/tobiko/shell/sh/_execute.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_hostname.py` & `tobiko-0.6.9/tobiko/shell/sh/_hostname.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_io.py` & `tobiko-0.6.9/tobiko/shell/sh/_io.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_local.py` & `tobiko-0.6.9/tobiko/shell/sh/_local.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_mkdirs.py` & `tobiko-0.6.9/tobiko/shell/sh/_mkdirs.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_mktemp.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/designate/test_zone.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-# Copyright (c) 2021 Red Hat, Inc.
-#
-# All Rights Reserved.
+# Copyright 2022 Red Hat
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 from __future__ import absolute_import
 
-import tobiko
-from tobiko.shell import ssh
-from tobiko.shell.sh import _execute
+from tobiko.openstack import designate
+from tobiko.tests.unit import openstack
+
+
+class DesignateZoneTest(openstack.OpenstackTest):
 
+    def test_designate_zone_id_with_str(self):
+        self.assertEqual('some-id',
+                         designate.designate_zone_id('some-id'))
 
-def make_temp_dir(ssh_client: ssh.SSHClientType = None,
-                  sudo: bool = None) \
-        -> str:
-    test_case = tobiko.get_test_case()
-    dir_name: str = _execute.execute('mktemp -d',
-                                     ssh_client=ssh_client,
-                                     sudo=sudo).stdout.strip()
-    test_case.addCleanup(_execute.execute,
-                         f'rm -fR "{dir_name}"',
-                         ssh_client=ssh_client,
-                         sudo=sudo)
-    return dir_name
+    def test_designate_zone_id_with_dict(self):
+        self.assertEqual('some-id',
+                         designate.designate_zone_id({'id': 'some-id'}))
```

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_nameservers.py` & `tobiko-0.6.9/tobiko/shell/sh/_nameservers.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_path.py` & `tobiko-0.6.9/tobiko/shell/sh/_path.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_process.py` & `tobiko-0.6.9/tobiko/shell/sh/_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,22 +539,24 @@
     return bg_process_name_pid_list
 
 
 def check_or_start_background_process(bg_function=None,
                                       bg_process_name=None,
                                       check_function=None,
                                       **kwargs):
-    """ Check if process exists, if so restart the process,
-        execute some check logic i.e. a check function.
-        if the process by name isn't running,
-        start a new separate process i.e a background function
-        params:
-            bg_process_name= process name
-            bg_function: function name
-            check_function: function name """
+    """Start or restart a process.
+
+    Check if a process exists, if so restart the process, execute some check
+    logic i.e. a check function. if the process by name isn't running, start a
+    new separate process i.e a background function
+
+    :param bg_process_name: process name
+    :param bg_function: function name
+    :param check_function: function name
+    """
 
     procs_running_list = get_bg_procs_pids(bg_process_name)
     if procs_running_list:
         # in any case test is still running, check for failures:
         # execute process check i.e. go over process results file
         # truncate the log file and restart the background process
         LOG.info(f'running a check function: {check_function} '
```

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_ps.py` & `tobiko-0.6.9/tobiko/shell/sh/_ps.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_reboot.py` & `tobiko-0.6.9/tobiko/shell/sh/_reboot.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_ssh.py` & `tobiko-0.6.9/tobiko/shell/sh/_ssh.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_systemctl.py` & `tobiko-0.6.9/tobiko/shell/sh/_systemctl.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_uptime.py` & `tobiko-0.6.9/tobiko/shell/sh/_uptime.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_wc.py` & `tobiko-0.6.9/tobiko/shell/sh/_wc.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/_which.py` & `tobiko-0.6.9/tobiko/shell/sh/_which.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/sh/config.py` & `tobiko-0.6.9/tobiko/shell/sh/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ss.py` & `tobiko-0.6.9/tobiko/shell/ss.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,23 +91,24 @@
 
 class SockData(dict):
     """A single socket information parsed from output of ss command line tool
 
     Output of ss command line tool should be parsed and stored in the dict
     with keys are items of the SockHeader object. In most of the cases it
     should contain the following keys:
-      - protocol (optional)
-      - state (optional)
-      - recv_q
-      - send_q
-      - local_addr (IP or filename)
-      - local_port
-      - remote_addr (IP or filename)
-      - remote_port
-      - process (list of processes names)
+
+    - protocol (optional)
+    - state (optional)
+    - recv_q
+    - send_q
+    - local_addr (IP or filename)
+    - local_port
+    - remote_addr (IP or filename)
+    - remote_port
+    - process (list of processes names)
     """
 
 
 LOG = log.getLogger(__name__)
 
 
 def _ss(params: str = '',
@@ -236,23 +237,24 @@
 def tcp_listening(address: str = '',
                   port: str = '',
                   **exec_params) -> typing.List[SockData]:
     """List of tcp sockets in listening state
 
     Information can be filtered by local address and port and will be returned
     as a list of SockData object where the following keys should exist:
-      - protocol (optional)
-      - state (optional)
-      - recv_q
-      - send_q
-      - local_addr (netaddr.IPAddress object)
-      - local_port
-      - remote_addr (netaddr.IPAddress object)
-      - remote_port
-      - process (list of processes names)
+
+    - protocol (optional)
+    - state (optional)
+    - recv_q
+    - send_q
+    - local_addr (netaddr.IPAddress object)
+    - local_port
+    - remote_addr (netaddr.IPAddress object)
+    - remote_port
+    - process (list of processes names)
     """
     params = '-t state listening'
     ss_fields = SockHeader('Recv-Q Send-Q Local Address:Port'
                            'Peer Address:Port Process')
     if port:
         params += ' sport {}'.format(port)
     if address:
@@ -287,23 +289,24 @@
 
 def unix_listening(file_name: str = '',
                    **exec_params) -> typing.List[SockData]:
     """List of unix sockets in listening state
 
     Information can be filtered by file name and will be returned as a list of
     SockData object where the following keys should exist:
-      - protocol (optional)
-      - state (optional)
-      - recv_q
-      - send_q
-      - local_addr (filename string)
-      - local_port (should be *)
-      - remote_addr (filename string - should be *)
-      - remote_port (should be *)
-      - process (list of processes names)
+
+    - protocol (optional)
+    - state (optional)
+    - recv_q
+    - send_q
+    - local_addr (filename string)
+    - local_port (should be ``*``)
+    - remote_addr (filename string - should be ``*``)
+    - remote_port (should be ``*``)
+    - process (list of processes names)
     """
     params = '-x state listening'
     ss_fields = SockHeader('Netid Recv-Q Send-Q Local Address:Port'
                            'Peer Address:Port Process')
     ss_fields.extend_ports()
     if file_name:
         params += ' src {}'.format(file_name)
```

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/__init__.py` & `tobiko-0.6.9/tobiko/shell/ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/_client.py` & `tobiko-0.6.9/tobiko/shell/ssh/_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/_command.py` & `tobiko-0.6.9/tobiko/shell/ssh/_command.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/_config.py` & `tobiko-0.6.9/tobiko/shell/ssh/_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/_forward.py` & `tobiko-0.6.9/tobiko/shell/ssh/_forward.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/_key_file.py` & `tobiko-0.6.9/tobiko/shell/ssh/_key_file.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/_skip.py` & `tobiko-0.6.9/tobiko/shell/ssh/_skip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/ssh/config.py` & `tobiko-0.6.9/tobiko/shell/ssh/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/tcpdump/__init__.py` & `tobiko-0.6.9/tobiko/shell/tcpdump/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/tcpdump/_assert.py` & `tobiko-0.6.9/tobiko/shell/tcpdump/_assert.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/tcpdump/_execute.py` & `tobiko-0.6.9/tobiko/shell/tcpdump/_execute.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/tcpdump/_interface.py` & `tobiko-0.6.9/tobiko/shell/tcpdump/_interface.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shell/tcpdump/_parameters.py` & `tobiko-0.6.9/tobiko/shell/tcpdump/_parameters.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/__init__.py` & `tobiko-0.6.9/tobiko/shiftstack/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/_clouds_file.py` & `tobiko-0.6.9/tobiko/shiftstack/_clouds_file.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/_heat.py` & `tobiko-0.6.9/tobiko/shiftstack/_heat.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/_keystone.py` & `tobiko-0.6.9/tobiko/shiftstack/_keystone.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/_neutron.py` & `tobiko-0.6.9/tobiko/shiftstack/_neutron.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/_nova.py` & `tobiko-0.6.9/tobiko/shiftstack/_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/_skip.py` & `tobiko-0.6.9/tobiko/shiftstack/_skip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/config.py` & `tobiko-0.6.9/tobiko/shiftstack/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/shiftstack/stacks.py` & `tobiko-0.6.9/tobiko/shiftstack/stacks.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/base.py` & `tobiko-0.6.9/tobiko/tests/base.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/conftest.py` & `tobiko-0.6.9/tobiko/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/containers/container_ops.py` & `tobiko-0.6.9/tobiko/tests/faults/containers/container_ops.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/containers/test_container_config.py` & `tobiko-0.6.9/tobiko/tests/faults/containers/test_container_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/containers/test_container_log.py` & `tobiko-0.6.9/tobiko/tests/faults/containers/test_container_log.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/ha/cloud_disruptions.py` & `tobiko-0.6.9/tobiko/tests/faults/ha/cloud_disruptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import time
 import urllib.parse
 
 import netaddr
 from oslo_log import log
 
 import tobiko
+from tobiko import config
 from tobiko.openstack import glance
 from tobiko.openstack import keystone
 from tobiko.openstack import neutron
 from tobiko.openstack import stacks
 from tobiko.openstack import tests
 from tobiko.openstack import topology
 from tobiko.tests.faults.ha import test_cloud_recovery
@@ -38,14 +39,16 @@
 from tobiko.shell import sh
 from tobiko.tripleo import containers
 from tobiko.tripleo import nova
 from tobiko.tripleo import pacemaker
 from tobiko.tripleo import topology as tripleo_topology
 from tobiko import tripleo
 
+
+CONF = config.CONF
 LOG = log.getLogger(__name__)
 
 network_disruption = """
  sudo iptables-save > ~/working.iptables.rules &&
  sudo iptables -I INPUT 1 -m state --state RELATED,ESTABLISHED -j ACCEPT &&
  sudo iptables -I INPUT 2 -p tcp -m state --state NEW -m tcp --dport 22 -j \
  ACCEPT &&
@@ -545,51 +548,62 @@
     delete /var/lib/mysql/grastate.dat in a random node,
     check that bootstrap is done from a node with grastate"""
     if tripleo_topology.is_composable_roles_env():
         nodes = topology.list_openstack_nodes(group='database')
     else:
         nodes = topology.list_openstack_nodes(group='controller')
     node = random.choice(nodes)
-    LOG.info(f'disable {pacemaker.HAPROXY_RESOURCE}')
-    if f"resource '{pacemaker.HAPROXY_RESOURCE}' is not running on any node" \
-            not in pacemaker.run_pcs_resource_operation(
-                pacemaker.HAPROXY_RESOURCE,
-                pacemaker.DISABLE,
-                node.ssh_client,
-                operation_wait=30):
-        raise PcsDisableException()
-    LOG.info('shut down {} on all servers: {}'.format(
-        pacemaker.GALERA_RESOURCE, nodes))
-    if f"resource '{pacemaker.GALERA_RESOURCE}' is not running on any node" \
-            not in pacemaker.run_pcs_resource_operation(
-                pacemaker.GALERA_RESOURCE,
+
+    pcs_haproxy = pacemaker.HAPROXY_RESOURCE
+    pcs_galera = pacemaker.GALERA_RESOURCE
+
+    if not CONF.tobiko.tripleo.has_external_load_balancer:
+        LOG.info(f'disable {pcs_haproxy}')
+        if f"resource '{pcs_haproxy}' is not running on any node" not in \
+                pacemaker.run_pcs_resource_operation(
+                    pcs_haproxy,
+                    pacemaker.DISABLE,
+                    node.ssh_client,
+                    operation_wait=30):
+            raise PcsDisableException()
+    else:
+        LOG.debug(f'With Ext LB setups, {pcs_haproxy} is not deployed')
+
+    LOG.info('shut down {} on all servers: {}'.format(pcs_galera, nodes))
+    if f"resource '{pcs_galera}' is not running on any node" not in \
+            pacemaker.run_pcs_resource_operation(
+                pcs_galera,
                 pacemaker.DISABLE,
                 node.ssh_client):
         raise PcsDisableException()
     LOG.info('remove grastate: {} on server: {}'.format(remove_grastate,
                                                         node.name))
     sh.execute(remove_grastate, ssh_client=node.ssh_client)
 
-    LOG.info('enable back {} on all servers: {}'.format(
-        pacemaker.GALERA_RESOURCE, nodes))
+    LOG.info('enable back {} on all servers: {}'.format(pcs_galera, nodes))
     if topology.verify_osp_version('17.0', lower=True):
         promoted = "master"
     else:
         promoted = "promoted"
-    if f"resource '{pacemaker.GALERA_RESOURCE}' is {promoted} on node" not in \
+    if f"resource '{pcs_galera}' is {promoted} on node" not in \
             pacemaker.run_pcs_resource_operation(
-                pacemaker.GALERA_RESOURCE, pacemaker.ENABLE, node.ssh_client,
+                pcs_galera, pacemaker.ENABLE, node.ssh_client,
                 operation_wait=90):
         raise PcsEnableException()
-    LOG.info(f'enable {pacemaker.HAPROXY_RESOURCE}')
-    if f"resource '{pacemaker.HAPROXY_RESOURCE}' is running on node" not in \
-            pacemaker.run_pcs_resource_operation(pacemaker.HAPROXY_RESOURCE,
-                                                 pacemaker.ENABLE,
-                                                 node.ssh_client):
-        raise PcsEnableException()
+
+    if not CONF.tobiko.tripleo.has_external_load_balancer:
+        LOG.info(f'enable {pcs_haproxy}')
+        if f"resource '{pcs_haproxy}' is running on node" not in \
+                pacemaker.run_pcs_resource_operation(pcs_haproxy,
+                                                     pacemaker.ENABLE,
+                                                     node.ssh_client):
+            raise PcsEnableException()
+    else:
+        LOG.debug(f'With Ext LB setups, {pcs_haproxy} is not deployed')
+
     # gcomm:// without args means that bootstrap is done from this node
     bootstrap = sh.execute(check_bootstrap, ssh_client=node.ssh_client).stdout
     if re.search('wsrep-cluster-address=gcomm://', bootstrap) is None:
         raise GaleraBoostrapException()
     lastDate = re.findall(r"\w{,3}\s*\w{,3}\s*\d{,2}\s*\d{,2}:\d{,2}:\d{,2}\s*"
                           r"\d{4}", bootstrap)[-1]
     return node, lastDate
```

### Comparing `tobiko-0.6.8/tobiko/tests/faults/ha/test_cloud_recovery.py` & `tobiko-0.6.9/tobiko/tests/faults/ha/test_cloud_recovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,33 @@
 import typing
 
 import pytest
 from oslo_log import log
 import testtools
 
 import tobiko
+from tobiko import config
 from tobiko.openstack import neutron
 from tobiko.openstack import nova as nova_osp
 from tobiko.openstack import topology
 from tobiko.openstack import tests
 from tobiko.tests.faults.ha import cloud_disruptions
 from tobiko.tripleo import pacemaker
 from tobiko.tripleo import processes
 from tobiko.tripleo import containers
 from tobiko.tripleo import nova
 from tobiko.tripleo import overcloud
 from tobiko.tripleo import undercloud
 
 
+CONF = config.CONF
 LOG = log.getLogger(__name__)
+SKIP_MESSAGE_EXTLB = ('Tests requiring a main VIP should be skipped when an '
+                      'external load balancer is used')
+has_external_lb = CONF.tobiko.tripleo.has_external_load_balancer
 
 
 def overcloud_health_checks(passive_checks_only=False,
                             skip_mac_table_size_test=False):
     # this method will be changed in future commit
     check_pacemaker_resources_health()
     check_overcloud_processes_health()
@@ -165,49 +170,55 @@
                 continue
             vm_id = vm['id']
             try:
                 nova_osp.delete_server(vm_id)
             except nova_osp.ServerNotFoundError:
                 LOG.debug(f"Server {vm_id} not found")
 
+    @testtools.skipIf(has_external_lb, SKIP_MESSAGE_EXTLB)
     def test_z99_reboot_controller_galera_main_vip(self):
         # This test case may fail at times if RHBZ#2124877 is not resolved
         # but that bug is due to a race condition,
         # so it is not reproducible 100% times
         OvercloudHealthCheck.run_before(passive_checks_only=True)
         multi_ip_test_fixture, ports_before_stack_creation = \
             cloud_disruptions.reboot_controller_galera_main_vip()
         OvercloudHealthCheck.run_after(passive_checks_only=True)
         self.vms_detailed_info = cloud_disruptions.get_vms_detailed_info(
             multi_ip_test_fixture)
         cloud_disruptions.check_no_duplicate_ips(
             self.vms_detailed_info, ports_before_stack_creation)
 
+    @testtools.skipIf(has_external_lb, SKIP_MESSAGE_EXTLB)
     def test_z99_reboot_controller_main_vip(self):
         OvercloudHealthCheck.run_before()
         cloud_disruptions.reset_controller_main_vip()
         OvercloudHealthCheck.run_after()
 
+    @testtools.skipIf(has_external_lb, SKIP_MESSAGE_EXTLB)
     def test_z99_reboot_controller_non_main_vip(self):
         OvercloudHealthCheck.run_before()
         cloud_disruptions.reset_controllers_non_main_vip()
         OvercloudHealthCheck.run_after()
 
+    @testtools.skipIf(has_external_lb, SKIP_MESSAGE_EXTLB)
     def test_z99_crash_controller_main_vip(self):
         OvercloudHealthCheck.run_before()
         cloud_disruptions.crash_controller_main_vip()
         OvercloudHealthCheck.run_after()
 
     @overcloud.skip_unless_kexec_tools_installed
+    @testtools.skipIf(has_external_lb, SKIP_MESSAGE_EXTLB)
     def test_z99_crash_controller_non_main_vip(self):
         OvercloudHealthCheck.run_before()
         cloud_disruptions.crash_controllers_non_main_vip()
         OvercloudHealthCheck.run_after()
 
     @pacemaker.skip_if_fencing_not_deployed
+    @testtools.skipIf(has_external_lb, SKIP_MESSAGE_EXTLB)
     def test_network_disruptor_main_vip(self):
         OvercloudHealthCheck.run_before()
         cloud_disruptions.network_disrupt_controller_main_vip()
         OvercloudHealthCheck.run_after()
         cloud_disruptions.network_undisrupt_controller_main_vip()
 
     # @pacemaker.skip_if_fencing_not_deployed
```

### Comparing `tobiko-0.6.8/tobiko/tests/faults/iha/test_cloud_recovery.py` & `tobiko-0.6.9/tobiko/tests/faults/iha/test_cloud_recovery.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/neutron/test_agents.py` & `tobiko-0.6.9/tobiko/tests/faults/neutron/test_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,15 +525,15 @@
 
     def _is_radvd_process_expected(self):
         stateless_modes = ['slaac', 'dhcpv6-stateless']
         ipv6_ra_mode = self.stack.network_stack.ipv6_subnet_details.get(
             'ipv6_ra_mode')
         ipv6_address_mode = self.stack.network_stack.ipv6_subnet_details.get(
             'ipv6_address_mode')
-        if not self.stack.network_stack.ipv6_cidr:
+        if not self.stack.network_stack.ipv6_subnet_details.get('cidr'):
             return False
         if (ipv6_ra_mode not in stateless_modes or
                 ipv6_address_mode not in stateless_modes):
             return False
         return True
 
     def test_radvd_during_stop_l3_agent(self):
```

### Comparing `tobiko-0.6.8/tobiko/tests/faults/neutron/test_raft.py` & `tobiko-0.6.9/tobiko/tests/faults/neutron/test_raft.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/octavia/test_faults.py` & `tobiko-0.6.9/tobiko/tests/faults/octavia/test_faults.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/faults/octavia/test_services.py` & `tobiko-0.6.9/tobiko/tests/faults/octavia/test_services.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/common/test_background.py` & `tobiko-0.6.9/tobiko/tests/functional/common/test_background.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/docker/test_client.py` & `tobiko-0.6.9/tobiko/tests/functional/docker/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_agent.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_agent.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_floating_ip.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_floating_ip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_network.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_network.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_port.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_port.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/neutron/test_router.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/neutron/test_router.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,17 +91,23 @@
     def test_remove_router_interface_with_port(self):
         interface = self.test_add_router_interface_with_port()
         neutron.remove_router_interface(router=interface['id'],
                                         port=interface['port_id'])
 
     def test_add_router_interface_with_subnet(self):
         network = neutron.create_network(name=self.id())
+        subnet_pool_range = "172.168.111.0/24"
+        subnet_pool_default_prefixlen = 26
+        subnet_pool = neutron.create_subnet_pool(
+            name=self.id(),
+            prefixes=[subnet_pool_range],
+            default_prefixlen=subnet_pool_default_prefixlen)
         subnet = neutron.create_subnet(name=self.id(),
                                        network=network,
-                                       cidr=neutron.new_ipv4_cidr(),
+                                       subnetpool_id=subnet_pool['id'],
                                        ip_version=4)
         router = self.test_create_router()
         interface = neutron.add_router_interface(router=router, subnet=subnet)
         self.assertEqual(subnet['id'], interface['subnet_id'])
         return interface
 
     def test_remove_router_interface_with_subnet(self):
```

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_centos.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_centos.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_cirros.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_cirros.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_fedora.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_fedora.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_neutron.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_neutron.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,41 +159,64 @@
 class RouterInterfaceTest(testtools.TestCase):
 
     router_stack = tobiko.required_fixture(RouterInterfaceTestRouter)
     network_stack = tobiko.required_fixture(RouterInterfaceTestNetwork)
 
     required_fixtures = [router_stack, network_stack]
 
+    subnet_index = 201
+
     @classmethod
     def tearDownClass(cls) -> None:
         for fixture in cls.required_fixtures:
             try:
                 tobiko.cleanup_fixture(fixture.fixture)
             except Exception:
                 LOG.exception(f'Error cleaning up fixture: {fixture.fixture}')
 
+    def _get_subnet_pool(self, ip_version=4):
+        if ip_version == 4:
+            subnet_pool_range = f"172.168.{self.subnet_index}.0/24"
+            subnet_pool_default_prefixlen = 26
+        elif ip_version == 6:
+            subnet_pool_range = f"2003:{self.subnet_index}::/64"
+            subnet_pool_default_prefixlen = 68
+        else:
+            raise ValueError
+
+        subnet_pool = neutron.create_subnet_pool(
+            name=self.id(),
+            prefixes=[subnet_pool_range],
+            default_prefixlen=subnet_pool_default_prefixlen)
+
+        self.subnet_index += 1
+        return subnet_pool
+
     def test_ensure_router_interface_with_subnet(self,
                                                  ip_version=4):
         network = neutron.create_network()
+        subnet_pool = self._get_subnet_pool(ip_version)
         subnet = neutron.create_subnet(network=network,
+                                       subnetpool_id=subnet_pool['id'],
                                        ip_version=ip_version)
         self._test_ensure_router(subnet=subnet)
 
     def test_ensure_router_interface_with_ipv6_subnet(self):
         self.test_ensure_router_interface_with_subnet(ip_version=6)
 
     def test_ensure_router_interface_with_routed_ipv4_subnet(self):
         self._test_ensure_router(subnet=self.network_stack.ipv4_subnet_id)
 
     def test_ensure_router_interface_with_routed_ipv6_subnet(self):
         self._test_ensure_router(subnet=self.network_stack.ipv6_subnet_id)
 
     def test_ensure_router_interface_with_network(self):
         network = neutron.create_network()
-        neutron.create_subnet(network=network)
+        subnet_pool = self._get_subnet_pool()
+        neutron.create_subnet(network=network, subnetpool_id=subnet_pool['id'])
         self._test_ensure_router(network=network)
 
     def test_ensure_router_interface_with_routed_network(self):
         self._test_ensure_router(network=self.network_stack.network_id)
 
     def _test_ensure_router(self,
                             network: neutron.NetworkIdType = None,
```

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_nova.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_red_hat.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_red_hat.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_ubuntu.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_ubuntu.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/stacks/test_vlan.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/stacks/test_vlan.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_designate.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_designate.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_glance.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_glance.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_heat.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_heat.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_keystone.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_keystone.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_nova.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_octavia.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_octavia.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/test_topology.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/test_topology.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/openstack/tests/test_nova.py` & `tobiko-0.6.9/tobiko/tests/functional/openstack/tests/test_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/podman/test_client.py` & `tobiko-0.6.9/tobiko/tests/functional/podman/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/run/test_discover.py` & `tobiko-0.6.9/tobiko/tests/functional/run/test_discover.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/run/test_find.py` & `tobiko-0.6.9/tobiko/tests/functional/run/test_find.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/run/test_run.py` & `tobiko-0.6.9/tobiko/tests/functional/run/test_run.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/_fixtures.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/_fixtures.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_connection.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_connection.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_execute.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_execute.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_hostname.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_hostname.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_process.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_process.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_ps.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_ps.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_reboot.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_reboot.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_systemctl.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_systemctl.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_wc.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_wc.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/sh/test_which.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/sh/test_which.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/test_curl.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/test_curl.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/test_ifconfig.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/test_ifconfig.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/test_ip.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/test_ip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/test_mktemp.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/test_mktemp.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/test_nameservers.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/test_nameservers.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shell/test_ping.py` & `tobiko-0.6.9/tobiko/tests/functional/shell/test_ping.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shiftstack/test_neutron.py` & `tobiko-0.6.9/tobiko/tests/functional/shiftstack/test_neutron.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shiftstack/test_nova.py` & `tobiko-0.6.9/tobiko/tests/functional/shiftstack/test_nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/shiftstack/test_stacks.py` & `tobiko-0.6.9/tobiko/tests/functional/shiftstack/test_stacks.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/tripleo/test_ansible.py` & `tobiko-0.6.9/tobiko/tests/functional/tripleo/test_ansible.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/tripleo/test_containers.py` & `tobiko-0.6.9/tobiko/tests/functional/tripleo/test_containers.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/tripleo/test_overcloud.py` & `tobiko-0.6.9/tobiko/tests/functional/tripleo/test_overcloud.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/tripleo/test_topology.py` & `tobiko-0.6.9/tobiko/tests/functional/tripleo/test_topology.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/functional/tripleo/test_undercloud.py` & `tobiko-0.6.9/tobiko/tests/functional/tripleo/test_undercloud.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/__init__.py` & `tobiko-0.6.9/tobiko/tests/sanity/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/cloud/test_nodes.py` & `tobiko-0.6.9/tobiko/tests/sanity/cloud/test_nodes.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/containers/__init__.py` & `tobiko-0.6.9/tobiko/tests/sanity/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/containers/test_containers.py` & `tobiko-0.6.9/tobiko/tests/sanity/containers/test_containers.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/ha/__init__.py` & `tobiko-0.6.9/tobiko/tests/sanity/ha/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/ha/test_overcloud.py` & `tobiko-0.6.9/tobiko/tests/sanity/ha/test_overcloud.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/neutron/test_agents.py` & `tobiko-0.6.9/tobiko/tests/sanity/neutron/test_agents.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/neutron/test_cli.py` & `tobiko-0.6.9/tobiko/tests/sanity/neutron/test_cli.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/neutron/test_nodes.py` & `tobiko-0.6.9/tobiko/tests/sanity/neutron/test_nodes.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/nova/test_server.py` & `tobiko-0.6.9/tobiko/tests/sanity/nova/test_server.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/nova/test_service.py` & `tobiko-0.6.9/tobiko/tests/sanity/nova/test_service.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/scripts/pods_ready.sh` & `tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/scripts/pods_ready.sh`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/check_demo_app.yml` & `tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/check_demo_app.yml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/debug_machines.yml` & `tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/debug_machines.yml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/recreate_ocp_project.yml` & `tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/recreate_ocp_project.yml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/verification.yml` & `tobiko-0.6.9/tobiko/tests/sanity/shiftstack/playbooks/roles/tests/tasks/verification.yml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/sanity/shiftstack/test_shiftstack.py` & `tobiko-0.6.9/tobiko/tests/sanity/shiftstack/test_shiftstack.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/designate/test_zone.py` & `tobiko-0.6.9/tobiko/tests/scenario/designate/test_zone.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,25 +38,24 @@
     """
 
     zone_stack = tobiko.required_fixture(stacks.DesignateZoneStackFixture)
 
     def setUp(self):
         super(DesignateBasicScenarioTest, self).setUp()
         # Wait for Designate recourses to be active
-        create_recordset = self.zone_stack.recordset_create()
-        LOG.debug(create_recordset)
-
         self.zone_stack.wait_for_active_recordsets()
 
     def test_basic_sanity_scenario(self):
 
         # check that SOA, NS and A recordsets are listed in recordset list
         recordset_list = self.zone_stack.recordset_list
         expected_recordset_types = ["SOA", "NS", "A"]
         actual_recordset_types = [item["type"] for item in recordset_list]
+        expected_recordset_types.sort()
+        actual_recordset_types.sort()
         self.assertEqual(expected_recordset_types, actual_recordset_types)
 
         # list all Controller nodes
         nodes = topology.list_openstack_nodes(group='controller')
         valid_dns_ip_list = []
 
         for node in nodes:
@@ -78,12 +77,12 @@
                     answerA = my_resolver.resolve(
                         'record.tobiko.openstack.stacks._designate.'
                         'designatezonestackfixture.', 'A')
                     LOG.debug(f"{answerSOA},{answerNS},{answerA}"
                               f" is stored for a zone")
                     LOG.debug(f"{dns_ip} is a valid DNS server!")
                     valid_dns_ip_list.append(str(dns_ip))
-                except (dns.resolver.Timeout, dns.resolver.NoNameservers):
+                except (dns.resolver.Timeout, dns.resolver.NXDOMAIN):
                     LOG.warn(f"{dns_ip} is NOT a valid DNS server!")
 
         self.assertEqual(len(valid_dns_ip_list), len(nodes))
         LOG.debug(f"List of valid BIND9 IPs: {valid_dns_ip_list}")
```

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_floating_ip.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_floating_ip.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from tobiko import config
 from tobiko.shell import files
 from tobiko.shell import ping
 from tobiko.shell import sh
 from tobiko.openstack import neutron
 from tobiko.openstack import stacks
 from tobiko.openstack import topology
+from tobiko.tripleo import undercloud
 
 
 CONF = config.CONF
 LOG = log.getLogger(__name__)
 
 
 @pytest.mark.minimal
@@ -238,23 +239,26 @@
 @neutron.skip_if_missing_networking_agents(binary='neutron-l3-agent',
                                            count=2)
 class FloatingIpWithL3HATest(FloatingIPTest):
     #: Resources stack with floating IP and Nova server
     stack = tobiko.required_fixture(stacks.L3haServerStackFixture)
 
 
+@undercloud.skip_if_missing_undercloud
 @topology.skip_unless_osp_version('16.1', higher=True)
 class TestFloatingIPLogging(testtools.TestCase):
 
     stack = tobiko.required_fixture(stacks.NetworkStackFixture)
 
     def setUp(self):
         super(TestFloatingIPLogging, self).setUp()
         self.port = neutron.create_port(network_id=self.stack.network_id)
         self.fip = neutron.create_floating_ip()
+        # TODO(eolivare): adapt the following path to non-tripleo setups and
+        # remove the skip_if_missing_undercloud decorator
         log_filename = '/var/log/containers/neutron/server.log'
         self.log_digger = files.MultihostLogFileDigger(filename=log_filename,
                                                        sudo=True)
         for node in topology.list_openstack_nodes(group='controller'):
             self.log_digger.add_host(hostname=node.hostname,
                                      ssh_client=node.ssh_client)
```

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_network.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_network.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_port.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_port.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_qos.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_qos.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_router.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_router.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_security_groups.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_security_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    under the License.
 from __future__ import absolute_import
 
 import json
 import typing
 
 from oslo_log import log
+import pytest
 import testtools
 
 import tobiko
 from tobiko.openstack import neutron
 from tobiko.openstack import stacks
 from tobiko.openstack import topology
 from tobiko.shell import sh
@@ -281,14 +282,15 @@
 
     @property
     def security_groups(self) -> typing.List[str]:
         """List with Stateless security group"""
         return [self.security_groups_stack.security_group_id]
 
 
+@pytest.mark.skip_during_ovn_migration
 @neutron.skip_if_missing_networking_extensions('stateful-security-group')
 class StatelessSecurityGroupInstanceTest(BaseSecurityGroupTest):
 
     #: Resources stack with Nova server to send messages to
     vm = tobiko.required_fixture(
         CirrosServerWithStatelessSecurityGroupFixture)
```

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/neutron/test_trunk.py` & `tobiko-0.6.9/tobiko/tests/scenario/neutron/test_trunk.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/nova/test_server.py` & `tobiko-0.6.9/tobiko/tests/scenario/nova/test_server.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/octavia/test_traffic.py` & `tobiko-0.6.9/tobiko/tests/scenario/octavia/test_traffic.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/scenario/playbooks/test_floatingip.yaml` & `tobiko-0.6.9/tobiko/tests/scenario/playbooks/test_floatingip.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/__init__.py` & `tobiko-0.6.9/tobiko/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/_case.py` & `tobiko-0.6.9/tobiko/tests/unit/_case.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/_patch.py` & `tobiko-0.6.9/tobiko/tests/unit/_patch.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/actors/test_actor.py` & `tobiko-0.6.9/tobiko/tests/unit/actors/test_actor.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/actors/test_proxy.py` & `tobiko-0.6.9/tobiko/tests/unit/actors/test_proxy.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/__init__.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/_case.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/_case.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/_keystone.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/_keystone.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/designate/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/designate/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/heat/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/heat/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/heat/test_stack.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/heat/test_stack.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/heat/test_template.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/heat/test_template.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/test_credentials.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/test_credentials.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/keystone/test_session.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/keystone/test_session.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/metalsmith/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/metalsmith/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/neutron/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/neutron/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/neutron/test_extension.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/neutron/test_extension.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/nova/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/nova/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/nova/test_cloud_init.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/nova/test_cloud_init.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/nova/test_server.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/nova/test_server.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/octavia/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/octavia/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/test_client.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/test_client.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/openstack/tests/test_neutron.py` & `tobiko-0.6.9/tobiko/tests/unit/openstack/tests/test_neutron.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/shell/sh/test_command.py` & `tobiko-0.6.9/tobiko/tests/unit/shell/sh/test_command.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/shell/sh/test_hostname.py` & `tobiko-0.6.9/tobiko/tests/unit/shell/sh/test_hostname.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/shell/sh/test_io.py` & `tobiko-0.6.9/tobiko/tests/unit/shell/sh/test_io.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/shell/test_ssh.py` & `tobiko-0.6.9/tobiko/tests/unit/shell/test_ssh.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_cached.py` & `tobiko-0.6.9/tobiko/tests/unit/test_cached.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_case.py` & `tobiko-0.6.9/tobiko/tests/unit/test_case.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_config.py` & `tobiko-0.6.9/tobiko/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_conftest.py` & `tobiko-0.6.9/tobiko/tests/unit/test_conftest.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_exception.py` & `tobiko-0.6.9/tobiko/tests/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_fixture.py` & `tobiko-0.6.9/tobiko/tests/unit/test_fixture.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_ini.py` & `tobiko-0.6.9/tobiko/tests/unit/test_ini.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_loader.py` & `tobiko-0.6.9/tobiko/tests/unit/test_loader.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_logging.py` & `tobiko-0.6.9/tobiko/tests/unit/test_logging.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_operation.py` & `tobiko-0.6.9/tobiko/tests/unit/test_operation.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_retry.py` & `tobiko-0.6.9/tobiko/tests/unit/test_retry.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_select.py` & `tobiko-0.6.9/tobiko/tests/unit/test_select.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_skip.py` & `tobiko-0.6.9/tobiko/tests/unit/test_skip.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_time.py` & `tobiko-0.6.9/tobiko/tests/unit/test_time.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_utils.py` & `tobiko-0.6.9/tobiko/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/test_version.py` & `tobiko-0.6.9/tobiko/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tests/unit/tripleo/test_config.py` & `tobiko-0.6.9/tobiko/tests/unit/tripleo/test_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/__init__.py` & `tobiko-0.6.9/tobiko/tripleo/__init__.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/_ansible.py` & `tobiko-0.6.9/tobiko/tripleo/_ansible.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/_config.py` & `tobiko-0.6.9/tobiko/tripleo/_config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/_overcloud.py` & `tobiko-0.6.9/tobiko/tripleo/_overcloud.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/_rhosp.py` & `tobiko-0.6.9/tobiko/tripleo/_rhosp.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/_topology.py` & `tobiko-0.6.9/tobiko/tripleo/_topology.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/_undercloud.py` & `tobiko-0.6.9/tobiko/tripleo/_undercloud.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/config.py` & `tobiko-0.6.9/tobiko/tripleo/config.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/containers.py` & `tobiko-0.6.9/tobiko/tripleo/containers.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/nova.py` & `tobiko-0.6.9/tobiko/tripleo/nova.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/pacemaker.py` & `tobiko-0.6.9/tobiko/tripleo/pacemaker.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/tripleo/processes.py` & `tobiko-0.6.9/tobiko/tripleo/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 class OvercloudProcessesStatus(object):
     """
     class to handle processes checks,
     checks that all of these are running in the overcloud:
     'ovsdb-server','pcsd', 'corosync', 'beam.smp', 'mysqld', 'redis-server',
     'haproxy', 'nova-conductor', 'nova-scheduler', 'neutron-server',
-     'nova-compute', 'glance-api'
+    'nova-compute', 'glance-api'
     """
     def __init__(self):
         self.processes_to_check = ['ovsdb-server', 'pcsd', 'corosync',
                                    'beam.smp', 'mysqld', 'redis-server',
                                    'haproxy', 'nova-conductor',
                                    'nova-scheduler', 'neutron-server',
                                    'nova-compute', 'glance-api']
```

### Comparing `tobiko-0.6.8/tobiko/tripleo/services.py` & `tobiko-0.6.9/tobiko/tripleo/services.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko/version.py` & `tobiko-0.6.9/tobiko/version.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tobiko.conf.example` & `tobiko-0.6.9/tobiko.conf.example`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 [DEFAULT]
 
 
+[ansible]
+
+#
+# From tobiko
+#
+
+# Default Ansible inventory files (list value)
+#inventory_files = /etc/ansible/hosts
+
+# Default Ansible playbook verbosity (integer value)
+#verbosity = <None>
+
+
 [centos]
 
 #
 # From tobiko
 #
 
 # Default centos image name (string value)
@@ -27,14 +40,18 @@
 
 # Default centos password (string value)
 #password = <None>
 
 # Default centos SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [centos7]
 
 #
 # From tobiko
 #
 
@@ -58,14 +75,18 @@
 
 # Default centos7 password (string value)
 #password = <None>
 
 # Default centos7 SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [cirros]
 
 #
 # From tobiko
 #
 
@@ -89,14 +110,28 @@
 
 # Default cirros password (string value)
 #password = <None>
 
 # Default cirros SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
+
+[common]
+
+#
+# From tobiko
+#
+
+# Default directory where to look for shelves. (string value)
+#shelves_dir = ~/.tobiko/cache/shelves
+
 
 [fedora]
 
 #
 # From tobiko
 #
 
@@ -120,14 +155,18 @@
 
 # Default fedora password (string value)
 #password = <None>
 
 # Default fedora SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [glance]
 
 #
 # From tobiko
 #
 
@@ -211,14 +250,17 @@
 
 # Trust ID for trust scoping. (string value)
 #trust_id = <None>
 
 # Cloud name used pick authentication parameters from clouds.* (string value)
 #cloud_name = <None>
 
+# Host login from where to search for clouds file (list value)
+#clouds_file_hosts = localhost
+
 # Directories where to look for clouds files (list value)
 #clouds_file_dirs = .,~/.config/openstack,/etc/openstack
 
 # Clouds file names (list value)
 #clouds_file_names = clouds.yaml,clouds.yml,clouds.json
 
 
@@ -285,29 +327,35 @@
 [nova]
 
 #
 # From tobiko
 #
 
 # Default SSH key to login to server instances (string value)
-#key_file = ~/.ssh/id_rsa
+#key_file = ~/.ssh/id_ecdsa
+
+# Default SSH key type to login to server instances (string value)
+#key_type = ecdsa
 
 
 [octavia]
 
 #
 # From tobiko
 #
 
 # Interval to check for status changes, in seconds. (integer value)
 #check_interval = 5
 
 # Timeout, in seconds, to wait for a status change. (integer value)
 #check_timeout = 360
 
+# The user we should use when we SSH the amphora. (string value)
+#amphora_user = cloud-user
+
 
 [ping]
 
 #
 # From tobiko
 #
 
@@ -358,14 +406,18 @@
 
 # Default rhel password (string value)
 #password = <None>
 
 # Default rhel SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
 
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
+
 
 [shell]
 
 #
 # From tobiko
 #
 
@@ -373,14 +425,33 @@
 #command = /bin/sh -c
 
 # Default sudo command used for executing commands as superuser or another user (string
 # value)
 #sudo = sudo
 
 
+[shiftstack]
+
+#
+# From tobiko
+#
+
+# local clouds file path (string value)
+#local_clouds_file_path = .tobiko/shifstack/clouds.yaml
+
+# remote clouds file path on undercloud-0 host (string value)
+#remote_clouds_file_path = ~/clouds.yaml
+
+# Keystone credentials cloud name (string value)
+#cloud_name = shiftstack
+
+# Path to the RC file used to populate OS_* environment variables (list value)
+#rcfile = ./shiftstackrc
+
+
 [ssh]
 
 #
 # From tobiko
 #
 
 # Logout debugging messages of paramiko library (boolean value)
@@ -394,16 +465,16 @@
 
 # Default SSH username (string value)
 #username = <None>
 
 # Default user SSH configuration files (list value)
 #config_files = ssh_config,.ssh/config
 
-# Default SSH private key file(s) (list value)
-#key_file = ~/.ssh/id_rsa,.ssh/id
+# Default SSH private key file(s) wildcard (list value)
+#key_file = .ssh/id,~/.ssh/id_dsa,~/.ssh/id_rsa,~/.ssh/id_ecdsa,~/.ssh/id_ed25519
 
 # Set to False to disable connecting to the SSH agent (boolean value)
 #allow_agent = false
 
 # Set to True to turn on compression (boolean value)
 #compress = false
 
@@ -483,39 +554,57 @@
 # TCP port of SSH server on undercloud host (integer value)
 #undercloud_ssh_port = <None>
 
 # Username with access to stackrc and overcloudrc files (string value)
 #undercloud_ssh_username = stack
 
 # SSH key filename used to login to Undercloud node (string value)
-#undercloud_ssh_key_filename = ~/.ssh/id_rsa
+#undercloud_ssh_key_filename = <None>
 
 # Undercloud RC filename (list value)
 #undercloud_rcfile = ~/stackrc
 
+# undercloud cloud name to be used for loading credentials from the undercloud clouds
+# files (string value)
+#undercloud_cloud_name = undercloud
+
 # TCP port of SSH server on overcloud hosts (integer value)
 #overcloud_ssh_port = <None>
 
 # Default username used to connect to overcloud nodes (string value)
-#overcloud_ssh_username = heat-admin
+#overcloud_ssh_username = <None>
 
 # SSH key filename used to login to Overcloud nodes (string value)
 #overcloud_ssh_key_filename = ~/.ssh/id_overcloud
 
 # Overcloud RC filenames (list value)
 #overcloud_rcfile = ~/overcloudrc,~/qe-Cloud-0rc
 
+# overcloud cloud name to be used for loading credentials from the overcloud clouds
+# files (string value)
+#overcloud_cloud_name = overcloud
+
 # Default IP address version to be used to connect to overcloud nodes  (integer value)
 #overcloud_ip_version = <None>
 
 # Name of network used to connect to overcloud nodes (string value)
 #overcloud_network_name = <None>
 
+# Dictionary with the node groups corresponding to different hostname prefixes (dict
+# value)
+#overcloud_groups_dict = cmp:compute,ctrl:controller
+
 # path to where to export tripleo inventory file (string value)
-#inventory_file = tripleo-hosts.yaml
+#inventory_file = .ansible/inventory/tripleo.yaml
+
+# OSP env was done with an external load balancer (boolean value)
+#has_external_load_balancer = false
+
+# whether Ceph RGW is deployed (boolean value)
+#ceph_rgw = false
 
 
 [ubuntu]
 
 #
 # From tobiko
 #
@@ -539,7 +628,11 @@
 #username = <None>
 
 # Default ubuntu password (string value)
 #password = <None>
 
 # Default ubuntu SSH connection timeout (seconds) (floating point value)
 #connection_timeout = <None>
+
+# Allow to disable SSH auth algorithmsin order to SSH to old servers likeCirrOS ones
+# (dict value)
+#disabled_algorithms = <None>
```

### Comparing `tobiko-0.6.8/tobiko.egg-info/PKG-INFO` & `tobiko-0.6.9/tobiko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tobiko
-Version: 0.6.8
+Version: 0.6.9
 Summary: OpenStack Testing Upgrades Library
 Home-page: https://tobiko.readthedocs.io/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======
         Tobiko
```

### Comparing `tobiko-0.6.8/tobiko.egg-info/SOURCES.txt` & `tobiko-0.6.9/tobiko.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -40,14 +40,49 @@
 doc/source/contributor/setup_tobiko_workstation.rst
 doc/source/etc/index.rst
 doc/source/etc/tobiko.conf.gen
 doc/source/etc/tobiko.conf.rst
 doc/source/miscellaneous/from-tempest-to-tobiko.rst
 doc/source/miscellaneous/index.rst
 doc/source/reference/index.rst
+doc/source/reference/modules/actors.rst
+doc/source/reference/modules/docker.rst
+doc/source/reference/modules/http.rst
+doc/source/reference/modules/podman.rst
+doc/source/reference/modules/run.rst
+doc/source/reference/modules/shiftstack.rst
+doc/source/reference/modules/tobiko.rst
+doc/source/reference/modules/openstack/designate.rst
+doc/source/reference/modules/openstack/glance.rst
+doc/source/reference/modules/openstack/heat.rst
+doc/source/reference/modules/openstack/index.rst
+doc/source/reference/modules/openstack/ironic.rst
+doc/source/reference/modules/openstack/keystone.rst
+doc/source/reference/modules/openstack/metalsmith.rst
+doc/source/reference/modules/openstack/neutron.rst
+doc/source/reference/modules/openstack/nova.rst
+doc/source/reference/modules/openstack/octavia.rst
+doc/source/reference/modules/openstack/openstackclient.rst
+doc/source/reference/modules/openstack/stacks.rst
+doc/source/reference/modules/openstack/topology.rst
+doc/source/reference/modules/shell/ansible.rst
+doc/source/reference/modules/shell/curl.rst
+doc/source/reference/modules/shell/files.rst
+doc/source/reference/modules/shell/index.rst
+doc/source/reference/modules/shell/iperf3.rst
+doc/source/reference/modules/shell/ping.rst
+doc/source/reference/modules/shell/sh.rst
+doc/source/reference/modules/shell/ssh.rst
+doc/source/reference/modules/shell/tcpdump.rst
+doc/source/reference/modules/tripleo/containers.rst
+doc/source/reference/modules/tripleo/index.rst
+doc/source/reference/modules/tripleo/nova.rst
+doc/source/reference/modules/tripleo/pacemaker.rst
+doc/source/reference/modules/tripleo/processes.rst
+doc/source/reference/modules/tripleo/services.rst
 doc/source/user/_conf_credentials.rst
 doc/source/user/_conf_explanation.rst
 doc/source/user/_conf_logging.rst
 doc/source/user/_conf_venv_with_tox.rst
 doc/source/user/_install_venv.rst
 doc/source/user/_run_faults.rst
 doc/source/user/_run_scenario.rst
@@ -199,15 +234,14 @@
 roles/tobiko-run/vars/test-workflow-create-resources-heat.yaml
 roles/tobiko-run/vars/test-workflow-create-resources-neutron.yaml
 roles/tobiko-run/vars/test-workflow-create-resources-nova.yaml
 roles/tobiko-run/vars/test-workflow-create-resources-octavia.yaml
 roles/tobiko-run/vars/test-workflow-create-resources-ovn-migration.yaml
 roles/tobiko-run/vars/test-workflow-create-resources.yaml
 roles/tobiko-run/vars/test-workflow-default.yaml
-roles/tobiko-run/vars/test-workflow-designate-faults.yaml
 roles/tobiko-run/vars/test-workflow-faults-iha.yaml
 roles/tobiko-run/vars/test-workflow-faults-neutron.yaml
 roles/tobiko-run/vars/test-workflow-faults.yaml
 roles/tobiko-run/vars/test-workflow-functional.yaml
 roles/tobiko-run/vars/test-workflow-gate.yaml
 roles/tobiko-run/vars/test-workflow-minimal.yaml
 roles/tobiko-run/vars/test-workflow-octavia-faults.yaml
@@ -295,24 +329,24 @@
 tobiko/openstack/keystone/_session.py
 tobiko/openstack/keystone/config.py
 tobiko/openstack/metalsmith/__init__.py
 tobiko/openstack/metalsmith/_client.py
 tobiko/openstack/metalsmith/_instance.py
 tobiko/openstack/neutron/__init__.py
 tobiko/openstack/neutron/_agent.py
-tobiko/openstack/neutron/_cidr.py
 tobiko/openstack/neutron/_client.py
 tobiko/openstack/neutron/_extension.py
 tobiko/openstack/neutron/_floating_ip.py
 tobiko/openstack/neutron/_network.py
 tobiko/openstack/neutron/_port.py
 tobiko/openstack/neutron/_quota_set.py
 tobiko/openstack/neutron/_router.py
 tobiko/openstack/neutron/_security_group.py
 tobiko/openstack/neutron/_subnet.py
+tobiko/openstack/neutron/_subnet_pool.py
 tobiko/openstack/neutron/config.py
 tobiko/openstack/nova/__init__.py
 tobiko/openstack/nova/_client.py
 tobiko/openstack/nova/_cloud_init.py
 tobiko/openstack/nova/_hypervisor.py
 tobiko/openstack/nova/_key_file.py
 tobiko/openstack/nova/_quota_set.py
@@ -333,14 +367,16 @@
 tobiko/openstack/openstackclient/_exception.py
 tobiko/openstack/openstackclient/_log.py
 tobiko/openstack/openstackclient/_network.py
 tobiko/openstack/openstackclient/_port.py
 tobiko/openstack/openstackclient/_security_group.py
 tobiko/openstack/openstackclient/_security_group_rule.py
 tobiko/openstack/openstackclient/_subnet.py
+tobiko/openstack/openstacksdkclient/__init__.py
+tobiko/openstack/openstacksdkclient/_client.py
 tobiko/openstack/stacks/__init__.py
 tobiko/openstack/stacks/_centos.py
 tobiko/openstack/stacks/_cirros.py
 tobiko/openstack/stacks/_designate.py
 tobiko/openstack/stacks/_fedora.py
 tobiko/openstack/stacks/_hot.py
 tobiko/openstack/stacks/_l3ha.py
```

### Comparing `tobiko-0.6.8/tools/abandon_old_reviews.sh` & `tobiko-0.6.9/tools/abandon_old_reviews.sh`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tools/common.py` & `tobiko-0.6.9/tools/common.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tools/get_version.py` & `tobiko-0.6.9/tools/get_version.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tools/install.py` & `tobiko-0.6.9/tools/install.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tools/run_tests.py` & `tobiko-0.6.9/tools/run_tests.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tools/setup_infrared.py` & `tobiko-0.6.9/tools/setup_infrared.py`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/tox.ini` & `tobiko-0.6.9/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -215,16 +215,16 @@
 [testenv:ovn_migration]
 
 basepython = {[integration]basepython}
 envdir = {[integration]envdir}
 passenv = {[integration]passenv}
 setenv =
     {[testenv:scenario]setenv}
-    RUN_TESTS_EXTRA_ARGS = -m ovn_migration {env:OS_TEST_PATH}
-
+    OS_TEST_PATH = {toxinidir}/tobiko/tests/scenario
+    RUN_TESTS_EXTRA_ARGS = -m "not skip_during_ovn_migration" {env:OS_TEST_PATH}
 
 [testenv:nova]
 
 basepython = {[integration]basepython}
 envdir = {[integration]envdir}
 passenv = {[integration]passenv}
 setenv =
@@ -248,14 +248,24 @@
 envdir = {[integration]envdir}
 passenv = {[integration]passenv}
 setenv =
     {[testenv:sanity]setenv}
     OS_TEST_PATH = {toxinidir}/tobiko/tests/sanity/neutron
 
 
+[testenv:ovn_migration_sanity]
+
+basepython = {[integration]basepython}
+envdir = {[integration]envdir}
+passenv = {[integration]passenv}
+setenv =
+    {[testenv:sanity]setenv}
+    RUN_TESTS_EXTRA_ARGS = -m "ovn_migration and not skip_during_ovn_migration" {env:OS_TEST_PATH}
+
+
 [testenv:shiftstack_sanity]
 
 basepython = {[integration]basepython}
 envdir = {[integration]envdir}
 passenv = {[integration]passenv}
 setenv =
     {[testenv:sanity]setenv}
@@ -280,24 +290,14 @@
 envdir = {[integration]envdir}
 passenv = {[integration]passenv}
 setenv =
     {[testenv:faults]setenv}
     OS_TEST_PATH = {toxinidir}/tobiko/tests/faults/octavia
 
 
-[testenv:designate_faults]
-
-basepython = {[integration]basepython}
-envdir = {[integration]envdir}
-passenv = {[integration]passenv}
-setenv =
-    {[testenv:faults]setenv}
-    OS_TEST_PATH = {toxinidir}/tobiko/tests/faults/designate
-
-
 [testenv:neutron_faults]
 
 basepython = {[integration]basepython}
 envdir = {[integration]envdir}
 passenv = {[integration]passenv}
 setenv =
     {[testenv:faults]setenv}
@@ -383,29 +383,29 @@
 [testenv:linkcheck]
 allowlist_externals = sh
 basepython = {[docs]basepython}
 envdir = {[docs]envdir}
 deps = {[docs]deps}
 commands =
     {[docs]commands}
-    sh -c 'cd {toxinidir}/doc/source && sphinx-build -W -b linkcheck . ../build/linkcheck'
+    sh -c 'cd {toxinidir}/doc/source && sphinx-build -W --keep-going -b linkcheck . ../build/linkcheck'
 usedevelop = true
 skipsdist = true
 skip_install = true
 
 
 [testenv:docs]
 allowlist_externals = sh
 basepython = {[docs]basepython}
 envdir = {[docs]envdir}
 deps = {[docs]deps}
 changedir = doc/source
 commands =
     {[testenv:linkcheck]commands}
-    sphinx-build -W -b html . ../build/html
+    sphinx-build -W --keep-going -b html . ../build/html
 usedevelop = true
 skipsdist = true
 skip_install = true
 
 
 [testenv:releasenotes]
```

### Comparing `tobiko-0.6.8/upper-constraints.txt` & `tobiko-0.6.9/upper-constraints.txt`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/zuul.d/docker.yaml` & `tobiko-0.6.9/zuul.d/docker.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/zuul.d/infrared.yaml` & `tobiko-0.6.9/zuul.d/infrared.yaml`

 * *Files identical despite different names*

### Comparing `tobiko-0.6.8/zuul.d/others.yaml` & `tobiko-0.6.9/zuul.d/others.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 
 - secret:
     name: tobiko_git_mirror_credentials
     data:
       user: git
       host: github.com
-      host_key: github.com ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PHkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETYP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoWf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lGHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==
+      host_key: github.com ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCj7ndNxQowgcQnjshcLrqPEiiphnt+VTTvDP6mHBL9j1aNUkY4Ue1gvwnGLVlOhGeYrnZaMgRK6+PKCUXaDbC7qtbW8gIkhL7aGCsOr/C56SJMy/BCZfxd1nWzAOxSDPgVsmerOBYfNqltV9/hWCqBywINIR+5dIg6JTJ72pcEpEjcYgXkE2YEFXV1JHnsKgbLWNlhScqb2UmyRkQyytRLtL+38TGxkxCflmO+5Z8CSSNY7GidjMIZ7Q4zMjA2n1nGrlTDkzwDCsw+wqFPGQA179cnfGWOWRVruj16z6XyvxvjJwbz0wQZ75XK5tKSb7FNyeIEs4TT4jk+S4dhPeAUC5y+bDYirYgM4GC7uEnztnZyaVWQ7B381AK4Qdrwt51ZqExKbQpTUNn+EjqoTwvqNj4kqx5QUCI0ThS/YkOxJCXmPUWZbhjpCg56i+2aB6CmK2JGhn57K5mj0MNdBXA4/WnwH6XoPWJzK5Nyu2zB3nAZp+S5hpQs+p1vN1/wsjk=
       ssh_key: !encrypted/pkcs1-oaep
         - KVpaJkAEwg5nE1uk1okGMDBvRHc1K6tlwxTri5IX6nNx1Ph9/iKw14AVNNW3/7+Zz5DLP
           KTPxfCGVKEb4lduYctCamS0h7rKEx1/2mSb0CCZLYH9X7vuLL8bHU8ARfzChCzPLb4je2
           iLws6DDEhInbS1EHsq0rHm/iVHBLbeEwD0Oj6qScsOasVfrL6hf/A9RAHaLnOYHw1b3HJ
           MQ6dDMCiX02pZMJrdeKQO+UxloGHnqcIYhPlqodueLCBOPrhztGGXLpjoWYfeMTzzzx1w
           f7JXItdkR1uqtR5xc0oS1y/fB70kweHsB16qqHcxOb7DN037Q7+9bEi3aRHxSTuU+3zOD
           1T8HHvTXBjZQscjVFo70a98QUkPjsox1+akQAnbiblnG0NFDyJ/1YWr8VCphAgGbdjYyv
```

### Comparing `tobiko-0.6.8/zuul.d/project.yaml` & `tobiko-0.6.9/zuul.d/project.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 - project:
     templates:
       - ansible-role-jobs
       - build-openstack-docs-pti
       - build-release-notes-jobs-python3
       - check-requirements
       - devstack-tobiko
+      - devstack-tobiko-designate
       - devstack-tobiko-functional
       - devstack-tobiko-heat
       - devstack-tobiko-minimal
-      - devstack-tobiko-octavia
       - devstack-tobiko-neutron
       - devstack-tobiko-nova
+      - devstack-tobiko-octavia
       - devstack-tobiko-ovs
       - devstack-tobiko-sanity
       - devstack-tobiko-storage
       - docs-on-readthedocs
       - openstack-cover-jobs
       - openstack-python3-yoga-jobs
       - openstack-python3-yoga-jobs-arm64
```

