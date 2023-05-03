# Comparing `tmp/tgwrap-0.5.5.tar.gz` & `tmp/tgwrap-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.5.5.tar", max compression
+gzip compressed data, was "tgwrap-0.5.6.tar", max compression
```

## Comparing `tgwrap-0.5.5.tar` & `tgwrap-0.5.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.5.5/LICENSE
--rw-r--r--   0        0        0     6036 2023-05-01 07:14:37.572053 tgwrap-0.5.5/README.md
--rw-r--r--   0        0        0      879 2023-05-01 11:05:14.565545 tgwrap-0.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.5.5/tgwrap/__init__.py
--rwxr-xr-x   0        0        0    24310 2023-04-25 12:36:41.404857 tgwrap-0.5.5/tgwrap/cli.py
--rwxr-xr-x   0        0        0    45811 2023-05-01 07:58:40.590824 tgwrap-0.5.5/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.5.5/tgwrap/printer.py
--rw-r--r--   0        0        0     4435 2023-01-17 14:04:36.314955 tgwrap-0.5.5/tgwrap/terrasafe.py
--rw-r--r--   0        0        0     7123 1970-01-01 00:00:00.000000 tgwrap-0.5.5/setup.py
--rw-r--r--   0        0        0     7075 1970-01-01 00:00:00.000000 tgwrap-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.5.6/LICENSE
+-rw-r--r--   0        0        0     6530 2023-05-02 09:53:07.369821 tgwrap-0.5.6/README.md
+-rw-r--r--   0        0        0      879 2023-05-03 04:49:24.472348 tgwrap-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.5.6/tgwrap/__init__.py
+-rwxr-xr-x   0        0        0    24647 2023-05-02 09:54:39.822466 tgwrap-0.5.6/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    46856 2023-05-02 09:53:48.224890 tgwrap-0.5.6/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.5.6/tgwrap/printer.py
+-rw-r--r--   0        0        0     4435 2023-01-17 14:04:36.314955 tgwrap-0.5.6/tgwrap/terrasafe.py
+-rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 tgwrap-0.5.6/setup.py
+-rw-r--r--   0        0        0     7569 1970-01-01 00:00:00.000000 tgwrap-0.5.6/PKG-INFO
```

### Comparing `tgwrap-0.5.5/LICENSE` & `tgwrap-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.5/README.md` & `tgwrap-0.5.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -138,12 +138,23 @@
     source: shared-integration/intsvc01
     target: integration/is01
     exclude_modules:  # a list of modules that will always be excluded, can be omitted
       - my-specific-module
   is02:
     source: shared-integration/intsvc01
     target: integration/is02
+
+# global configuration files that are deployed as well
+# note that these files are typically applicable to all landing zones and stages!
+# this might lead to unexpected behaviour
+# note that you can exclude syncing these files with a command line switch
+global_config_files:
+  root-terragrunt:
+    source: ../../terragrunt.hcl # relative to base_path
+    target: ../../terragrunt.hcl # can be omitted, then it is same as source path
+  terrasafe-config:
+    source: ../../terrasafe-config.json
 ```
 
 ## Development
 
 In order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.
```

### Comparing `tgwrap-0.5.5/pyproject.toml` & `tgwrap-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.5.5"
+version = "0.5.6"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.5.5/tgwrap/cli.py` & `tgwrap-0.5.6/tgwrap/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -581,14 +581,18 @@
     help="Version tag, use 'latest' to, well, get the latest version.",
     required=True, default='latest', show_default=True,
     )
 @click.option('--target-stage', '-t',
     help='Stage to deploy to',
     type=click.Choice(STAGES, case_sensitive=True), required=True,
     )
+@click.option('--include-global-config-files/--exclude-global-config-files', '-i/-x',
+    help='Whether or not to include deploying the (in the manifest specified) global config files',
+    is_flag=True, default=True, show_default=True,
+    )
 @click.option('--auto-approve', '-a',
     help='Do not ask for confirmation before applying planned changes (where applicable)',
     is_flag=True, default=False, show_default=True,
     )
 @click.option('--verbose', '-v',
     help='Verbose printing',
     is_flag=True, default=False, show_default=True,
@@ -598,26 +602,27 @@
     is_flag=True, default=False, show_default=True,
     )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.version_option(version=__version__)
 def deploy(
-    manifest_file, version_tag, target_stage,
+    manifest_file, version_tag, target_stage, include_global_config_files,
     auto_approve, verbose, dry_run, working_dir
     ):
     """ [experimental] Deploys the terragrunt config files from a git repository """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.deploy(
         manifest_file=manifest_file,
         version_tag=version_tag,
         target_stage=target_stage,
+        include_global_config_files=include_global_config_files,
         auto_approve=auto_approve,
         dry_run=dry_run,
         working_dir=working_dir,
     )
 
 @main.command(
     name="show-graph",
```

### Comparing `tgwrap-0.5.5/tgwrap/main.py` & `tgwrap-0.5.6/tgwrap/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -862,15 +862,15 @@
             auto_approve=auto_approve,
             dry_run=dry_run,
             clean_up=clean_up,
         )
 
     def deploy(
         self, manifest_file, version_tag, target_stage,
-        auto_approve, dry_run, working_dir, 
+        include_global_config_files, auto_approve, dry_run, working_dir, 
         ):
         """ Deploys the terragrunt config files from a git repository """
 
         DEFAULT_VERSION='latest'
 
         try:
             temp_dir = os.path.join(tempfile.mkdtemp(prefix='tgwrap-'), "tg-source")
@@ -965,14 +965,36 @@
                                 "source": source_path,
                                 "target": target_path,
                                 "excludes": exclude_modules,
                             }
                         else:
                             self.printer.warning(f'Source path of substack does not exist: {source_path}')
 
+            if include_global_config_files:
+                for gc, global_config in manifest.get('global_config_files', {}).items():
+                    self.printer.verbose(f'Found global config : {gc}')
+
+                    source_path = os.path.join(
+                        source_dir, global_config['source']
+                        )
+                    target = global_config.get('target', global_config['source'])
+                    target_path = os.path.join(
+                        working_dir, target,
+                        )
+
+                    if os.path.exists(source_path):
+                        deploy_actions[f'global configs -> {target}'] = {
+                            "source": source_path,
+                            "target": target_path,
+                        }
+                    else:
+                        self.printer.warning(f'Source path of global configs does not exist: {source_path}')
+            else:
+                self.printer.verbose(f'Skipping global configs')
+
             self.printer.header('Modules to deploy:')
             self.printer.normal(f'-> git repository: {manifest["git_repository"]}')
             self.printer.normal(f'-> version tag: {version_tag}')
             self.printer.normal('Modules:')
             for key, value in deploy_actions.items():
                 self.printer.normal(f'--> {key}')
```

### Comparing `tgwrap-0.5.5/tgwrap/printer.py` & `tgwrap-0.5.6/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.5/tgwrap/terrasafe.py` & `tgwrap-0.5.6/tgwrap/terrasafe.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.5/setup.py` & `tgwrap-0.5.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.5.5',
+    'version': '0.5.6',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
-    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.\n\nIt would provide output as follows:\n\n```console\n$ tgwrap analyze -x\n\n...\n\nAnalyse project: inputs\nRun terrasafe: inputs\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n\nAnalyse project: runners\nChanges:\nmodule.vmss.azurerm_key_vault_secret.pwd: delete,create\nmodule.vmss.azurerm_key_vault_secret.user: delete,create\nmodule.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update\n\nRun terrasafe: runners\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
+    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.\n\nIt would provide output as follows:\n\n```console\n$ tgwrap analyze -x\n\n...\n\nAnalyse project: inputs\nRun terrasafe: inputs\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n\nAnalyse project: runners\nChanges:\nmodule.vmss.azurerm_key_vault_secret.pwd: delete,create\nmodule.vmss.azurerm_key_vault_secret.user: delete,create\nmodule.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update\n\nRun terrasafe: runners\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tgwrap-0.5.5/PKG-INFO` & `tgwrap-0.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.5.5
+Version: 0.5.6
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
@@ -165,13 +165,24 @@
     source: shared-integration/intsvc01
     target: integration/is01
     exclude_modules:  # a list of modules that will always be excluded, can be omitted
       - my-specific-module
   is02:
     source: shared-integration/intsvc01
     target: integration/is02
+
+# global configuration files that are deployed as well
+# note that these files are typically applicable to all landing zones and stages!
+# this might lead to unexpected behaviour
+# note that you can exclude syncing these files with a command line switch
+global_config_files:
+  root-terragrunt:
+    source: ../../terragrunt.hcl # relative to base_path
+    target: ../../terragrunt.hcl # can be omitted, then it is same as source path
+  terrasafe-config:
+    source: ../../terrasafe-config.json
 ```
 
 ## Development
 
 In order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.
```

