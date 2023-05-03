# Comparing `tmp/python-dotenv-vault-0.4.1a0.tar.gz` & `tmp/python-dotenv-vault-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.4.1a0.tar", last modified: Sat Jan 28 08:04:37 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.5.0.tar", last modified: Wed May  3 17:59:17 2023, max compression
```

## Comparing `python-dotenv-vault-0.4.1a0.tar` & `python-dotenv-vault-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:04:37.248338 python-dotenv-vault-0.4.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-01-28 08:04:37.248338 python-dotenv-vault-0.4.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-01-28 08:04:27.000000 python-dotenv-vault-0.4.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-28 08:04:37.248338 python-dotenv-vault-0.4.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-01-28 08:04:27.000000 python-dotenv-vault-0.4.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:04:37.248338 python-dotenv-vault-0.4.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:04:37.248338 python-dotenv-vault-0.4.1a0/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-28 08:04:27.000000 python-dotenv-vault-0.4.1a0/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-28 08:04:27.000000 python-dotenv-vault-0.4.1a0/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-28 08:04:27.000000 python-dotenv-vault-0.4.1a0/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-01-28 08:04:27.000000 python-dotenv-vault-0.4.1a0/src/dotenv_vault/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:04:37.248338 python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-01-28 08:04:37.000000 python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-28 08:04:37.000000 python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 08:04:37.000000 python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-28 08:04:37.000000 python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-28 08:04:37.000000 python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.767441 python-dotenv-vault-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.4.1a0/PKG-INFO` & `python-dotenv-vault-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,147 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.4.1a0
+Version: 0.5.0
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
 
-# python-dotenv-vault
+# python-dotenv-vault [![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
 
 <img src="https://raw.githubusercontent.com/motdotla/dotenv/master/dotenv.svg" alt="dotenv-vault" align="right" width="200" />
 
-[![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
-
 Extends the proven & trusted foundation of [python-dotenv](https://github.com/theskumar/python-dotenv), with a `.env.vault` file.
 
-The extended standard lets you sync your `.env` files – quickly & securely. Stop sharing them over insecure channels like Slack and email, and never lose an important `.env` file again.
+The extended standard lets you load encrypted secrets from your `.env.vault` file in production (and other) environments. Brought to you by the same people that pioneered [dotenv-nodejs](https://github.com/motdotla/dotenv).
+
+* [🌱 Install](#-install)
+* [🏗️ Usage (.env)](#%EF%B8%8F-usage)
+* [🚀 Deploying (.env.vault) 🆕](#-deploying)
+* [🌴 Multiple Environments](#-manage-multiple-environments)
+* [❓ FAQ](#-faq)
+* [⏱️ Changelog](./CHANGELOG.md)
 
-## Installation
+## 🌱 Install
 
 ```shell
 pip install python-dotenv-vault
 ```
 
+## 🏗️ Usage
+
+Development usage works just like [python-dotenv](https://github.com/theskumar/python-dotenv).
+
+Add your application configuration to your `.env` file in the root of your project:
+
+```shell
+S3_BUCKET=YOURS3BUCKET
+SECRET_KEY=YOURSECRETKEYGOESHERE
+```
+
 As early as possible in your application bootstrap process, load .env:
 
 ```python
 from dotenv_vault import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 # Code of your application, which uses environment variables (e.g. from `os.environ` or
 # `os.getenv`) as if they came from the actual environment.
 ```
 
-## Usage
-
-### `.env`
-
-Basic usage works just like [python-dotenv](https://github.com/theskumar/python-dotenv).
-
-Add your application configuration to your `.env` file in the root of your project:
-
-```shell
-S3_BUCKET=YOURS3BUCKET
-SECRET_KEY=YOURSECRETKEYGOESHERE
-```
-
 When your application loads, these variables will be available in `os.environ` or `os.getenv`:
 
 ```python
 s3_bucket = os.getenv("S3_BUCKET")
 print(s3_bucket)
 ```
 
-### `.env.vault`
-
-The `.env.vault` extends `.env`. It facilitates syncing your .env file across machines, team members, and environments.
+## 🚀 Deploying
 
-Usage is similar to git. In the same directory as your `.env` file, run the command:
+Encrypt your environment variables by doing:
 
 ```shell
-$ npx dotenv-vault new
+npx dotenv-vault local build
 ```
 
-Follow those instructions and then run:
+This will create an encrypted `.env.vault` file along with a `.env.keys` file containing the encryption keys. Set the `DOTENV_KEY` environment variable by copying and pasting the key value from the `.env.keys` file onto your server or cloud provider. For example in heroku:
 
 ```shell
-$ npx dotenv-vault login
+heroku config:set DOTENV_KEY=<key string from .env.keys>
 ```
 
-Then run push and pull:
+Commit your .env.vault file safely to code and deploy. Your .env.vault fill be decrypted on boot, its environment variables injected, and your app work as expected.
 
-```shell
-$ npx dotenv-vault push
-$ npx dotenv-vault pull
-```
+Note that when the `DOTENV_KEY` environment variable is set, environment settings will *always* be loaded from the `.env.vault` file in the project root. For development use, you can leave the `DOTENV_KEY` environment variable unset and fall back on the `dotenv` behaviour of loading from `.env` or a specified set of files (see [here in the `dotenv` README](https://github.com/bkeepers/dotenv#usage) for the details).
 
-That's it!
+## 🌴 Manage Multiple Environments
 
-You just synced your `.env` file. Commit your `.env.vault` file to code, and tell your teammates to run `npx dotenv-vault pull`.
+You have two options for managing multiple environments - locally managed or vault managed - both use [dotenv-vault](https://github.com/dotenv-org/dotenv-vault).
 
-[Learn more](https://www.dotenv.org/docs/tutorials/sync)
+Locally managed never makes a remote API call. It is completely managed on your machine. Vault managed adds conveniences like backing up your .env file, secure sharing across your team, access permissions, and version history. Choose what works best for you.
 
-## Multiple Environments
+#### 💻 Locally Managed
 
-Run the command:
+Create a `.env.production` file in the root of your project and put your production values there.
 
 ```shell
-$ npx dotenv-vault open production
+# .env.production
+S3_BUCKET="PRODUCTION_S3BUCKET"
+SECRET_KEY="PRODUCTION_SECRETKEYGOESHERE"
 ```
 
-It will open up an interface to manage your production environment variables.
-
-[Learn more](https://www.dotenv.org/docs/tutorials/environments)
-
-## Integrate Anywhere™
-
-Build your encrypted `.env.vault`:
+Rebuild your `.env.vault` file.
 
 ```shell
-$ npx dotenv-vault build
+npx dotenv-vault local build
 ```
 
-Safely commit and push your changes:
+View your `.env.keys` file. There is a production `DOTENV_KEY` that pairs with the `DOTENV_VAULT_PRODUCTION` cipher in your `.env.vault` file.
 
-```shell
-$ git commit -am "Updated .env.vault"
-$ git push
-```
+Set the production `DOTENV_KEY` on your server, recommit your `.env.vault` file to code, and deploy. That's it!
 
-Obtain your `DOTENV_KEY`:
+Your .env.vault fill be decrypted on boot, its production environment variables injected, and your app work as expected.
 
-```shell
-$ npx dotenv-vault keys
-```
+#### 🔐 Vault Managed
 
-Set `DOTENV_KEY` on your infrastructure. For example, on Heroku:
+Sync your .env file. Run the push command and follow the instructions. [learn more](/docs/sync/quickstart)
 
-```shell
-$ heroku config:set DOTENV_KEY="dotenv://:key_1234@dotenv.org/vault/.env.vault?environment=production"
+```
+$ npx dotenv-vault push
 ```
 
-All set! When your app boots, it will recognize a `DOTENV_KEY` is set, decrypt the `.env.vault` file, and load the variables to `ENV`.
+Manage multiple environments with the included UI. [learn more](/docs/tutorials/environments)
 
-Made a change to your production envs? Run `npx dotenv-vault build`, commit that safely to code, and deploy. It's simple and safe like that.
+```
+$ npx dotenv-vault open
+```
 
-[Learn more](https://www.dotenv.org/docs/tutorials/integrations)
+Build your `.env.vault` file with multiple environments.
 
-## Dotenv.org
+```
+$ npx dotenv-vault build
+```
 
-You need a [Dotenv Account](https://dotenv.org) to use Dotenv Vault. It is free to use with premium features.
+Access your `DOTENV_KEY`.
 
-![](https://api.checklyhq.com/v1/badges/checks/c2fee99a-38e7-414e-89b8-9766ceeb1927?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/4f557967-1ed1-486a-b762-39a63781d752?style=flat&theme=dark&responseTime=true)
-<br>
-![](https://api.checklyhq.com/v1/badges/checks/804eb6fa-6599-4688-a649-7ff3c39a64b9?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/6a94504e-e936-4f07-bc0b-e08fee2734b3?style=flat&theme=dark&responseTime=true)
-<br>
-![](https://api.checklyhq.com/v1/badges/checks/06ac4f4e-3e0e-4501-9987-580b4d2a6b06?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/0ffc1e55-7ef0-4c2c-8acc-b6311871f41c?style=flat&theme=dark&responseTime=true)
+```
+$ npx dotenv-vault keys
+```
 
-Visit [health.dotenv.org](https://health.dotenv.org) for more information.
+Set the production `DOTENV_KEY` on your server, recommit your `.env.vault` file to code, and deploy. That's it!
 
-## FAQ
+## ❓ FAQ
 
 #### What happens if `DOTENV_KEY` is not set?
 
-Dotenv Vault gracefully falls back to [dotenv](https://github.com/bkeepers/dotenv) when `DOTENV_KEY` is not set. This is the default for development so that you can focus on editing your `.env` file and save the `build` command until you are ready to deploy those environment variables changes.
+Dotenv Vault gracefully falls back to [python-dotenv](https://github.com/theskumar/python-dotenv) when `DOTENV_KEY` is not set. This is the default for development so that you can focus on editing your `.env` file and save the `build` command until you are ready to deploy those environment variables changes.
 
 #### Should I commit my `.env` file?
 
 No. We **strongly** recommend against committing your `.env` file to version control. It should only include environment-specific values such as database passwords or API keys. Your production database should have a different password than your development database.
 
 #### Should I commit my `.env.vault` file?
 
@@ -179,15 +167,31 @@
 
 MIT
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
-## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.2.0...master)
+## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.0...master)
+
+## 0.5.0
+
+### Added
+
+ - Reorganise and simplify code
+ - Make API correspond more closely to `python-dotenv`
+ - Improve error handling
+ - Add tests and CI
+ - Upgrade to `build` for release build
+ 
+## 0.4.1
+
+### Added
+
+- expand cryptography library version range for better support
 
 ## 0.4.0
 
 ### Added
 
 - Added feature to allow custom .env.vault path
```

### Comparing `python-dotenv-vault-0.4.1a0/README.md` & `python-dotenv-vault-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,136 @@
-# python-dotenv-vault
+# python-dotenv-vault [![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
 
 <img src="https://raw.githubusercontent.com/motdotla/dotenv/master/dotenv.svg" alt="dotenv-vault" align="right" width="200" />
 
-[![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
-
 Extends the proven & trusted foundation of [python-dotenv](https://github.com/theskumar/python-dotenv), with a `.env.vault` file.
 
-The extended standard lets you sync your `.env` files – quickly & securely. Stop sharing them over insecure channels like Slack and email, and never lose an important `.env` file again.
+The extended standard lets you load encrypted secrets from your `.env.vault` file in production (and other) environments. Brought to you by the same people that pioneered [dotenv-nodejs](https://github.com/motdotla/dotenv).
+
+* [🌱 Install](#-install)
+* [🏗️ Usage (.env)](#%EF%B8%8F-usage)
+* [🚀 Deploying (.env.vault) 🆕](#-deploying)
+* [🌴 Multiple Environments](#-manage-multiple-environments)
+* [❓ FAQ](#-faq)
+* [⏱️ Changelog](./CHANGELOG.md)
 
-## Installation
+## 🌱 Install
 
 ```shell
 pip install python-dotenv-vault
 ```
 
+## 🏗️ Usage
+
+Development usage works just like [python-dotenv](https://github.com/theskumar/python-dotenv).
+
+Add your application configuration to your `.env` file in the root of your project:
+
+```shell
+S3_BUCKET=YOURS3BUCKET
+SECRET_KEY=YOURSECRETKEYGOESHERE
+```
+
 As early as possible in your application bootstrap process, load .env:
 
 ```python
 from dotenv_vault import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 # Code of your application, which uses environment variables (e.g. from `os.environ` or
 # `os.getenv`) as if they came from the actual environment.
 ```
 
-## Usage
-
-### `.env`
-
-Basic usage works just like [python-dotenv](https://github.com/theskumar/python-dotenv).
-
-Add your application configuration to your `.env` file in the root of your project:
-
-```shell
-S3_BUCKET=YOURS3BUCKET
-SECRET_KEY=YOURSECRETKEYGOESHERE
-```
-
 When your application loads, these variables will be available in `os.environ` or `os.getenv`:
 
 ```python
 s3_bucket = os.getenv("S3_BUCKET")
 print(s3_bucket)
 ```
 
-### `.env.vault`
+## 🚀 Deploying
 
-The `.env.vault` extends `.env`. It facilitates syncing your .env file across machines, team members, and environments.
-
-Usage is similar to git. In the same directory as your `.env` file, run the command:
+Encrypt your environment variables by doing:
 
 ```shell
-$ npx dotenv-vault new
+npx dotenv-vault local build
 ```
 
-Follow those instructions and then run:
+This will create an encrypted `.env.vault` file along with a `.env.keys` file containing the encryption keys. Set the `DOTENV_KEY` environment variable by copying and pasting the key value from the `.env.keys` file onto your server or cloud provider. For example in heroku:
 
 ```shell
-$ npx dotenv-vault login
+heroku config:set DOTENV_KEY=<key string from .env.keys>
 ```
 
-Then run push and pull:
+Commit your .env.vault file safely to code and deploy. Your .env.vault fill be decrypted on boot, its environment variables injected, and your app work as expected.
 
-```shell
-$ npx dotenv-vault push
-$ npx dotenv-vault pull
-```
+Note that when the `DOTENV_KEY` environment variable is set, environment settings will *always* be loaded from the `.env.vault` file in the project root. For development use, you can leave the `DOTENV_KEY` environment variable unset and fall back on the `dotenv` behaviour of loading from `.env` or a specified set of files (see [here in the `dotenv` README](https://github.com/bkeepers/dotenv#usage) for the details).
 
-That's it!
+## 🌴 Manage Multiple Environments
 
-You just synced your `.env` file. Commit your `.env.vault` file to code, and tell your teammates to run `npx dotenv-vault pull`.
+You have two options for managing multiple environments - locally managed or vault managed - both use [dotenv-vault](https://github.com/dotenv-org/dotenv-vault).
 
-[Learn more](https://www.dotenv.org/docs/tutorials/sync)
+Locally managed never makes a remote API call. It is completely managed on your machine. Vault managed adds conveniences like backing up your .env file, secure sharing across your team, access permissions, and version history. Choose what works best for you.
 
-## Multiple Environments
+#### 💻 Locally Managed
 
-Run the command:
+Create a `.env.production` file in the root of your project and put your production values there.
 
 ```shell
-$ npx dotenv-vault open production
+# .env.production
+S3_BUCKET="PRODUCTION_S3BUCKET"
+SECRET_KEY="PRODUCTION_SECRETKEYGOESHERE"
 ```
 
-It will open up an interface to manage your production environment variables.
-
-[Learn more](https://www.dotenv.org/docs/tutorials/environments)
-
-## Integrate Anywhere™
-
-Build your encrypted `.env.vault`:
+Rebuild your `.env.vault` file.
 
 ```shell
-$ npx dotenv-vault build
+npx dotenv-vault local build
 ```
 
-Safely commit and push your changes:
+View your `.env.keys` file. There is a production `DOTENV_KEY` that pairs with the `DOTENV_VAULT_PRODUCTION` cipher in your `.env.vault` file.
 
-```shell
-$ git commit -am "Updated .env.vault"
-$ git push
-```
+Set the production `DOTENV_KEY` on your server, recommit your `.env.vault` file to code, and deploy. That's it!
 
-Obtain your `DOTENV_KEY`:
+Your .env.vault fill be decrypted on boot, its production environment variables injected, and your app work as expected.
 
-```shell
-$ npx dotenv-vault keys
-```
+#### 🔐 Vault Managed
 
-Set `DOTENV_KEY` on your infrastructure. For example, on Heroku:
+Sync your .env file. Run the push command and follow the instructions. [learn more](/docs/sync/quickstart)
 
-```shell
-$ heroku config:set DOTENV_KEY="dotenv://:key_1234@dotenv.org/vault/.env.vault?environment=production"
+```
+$ npx dotenv-vault push
 ```
 
-All set! When your app boots, it will recognize a `DOTENV_KEY` is set, decrypt the `.env.vault` file, and load the variables to `ENV`.
+Manage multiple environments with the included UI. [learn more](/docs/tutorials/environments)
 
-Made a change to your production envs? Run `npx dotenv-vault build`, commit that safely to code, and deploy. It's simple and safe like that.
+```
+$ npx dotenv-vault open
+```
 
-[Learn more](https://www.dotenv.org/docs/tutorials/integrations)
+Build your `.env.vault` file with multiple environments.
 
-## Dotenv.org
+```
+$ npx dotenv-vault build
+```
 
-You need a [Dotenv Account](https://dotenv.org) to use Dotenv Vault. It is free to use with premium features.
+Access your `DOTENV_KEY`.
 
-![](https://api.checklyhq.com/v1/badges/checks/c2fee99a-38e7-414e-89b8-9766ceeb1927?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/4f557967-1ed1-486a-b762-39a63781d752?style=flat&theme=dark&responseTime=true)
-<br>
-![](https://api.checklyhq.com/v1/badges/checks/804eb6fa-6599-4688-a649-7ff3c39a64b9?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/6a94504e-e936-4f07-bc0b-e08fee2734b3?style=flat&theme=dark&responseTime=true)
-<br>
-![](https://api.checklyhq.com/v1/badges/checks/06ac4f4e-3e0e-4501-9987-580b4d2a6b06?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/0ffc1e55-7ef0-4c2c-8acc-b6311871f41c?style=flat&theme=dark&responseTime=true)
+```
+$ npx dotenv-vault keys
+```
 
-Visit [health.dotenv.org](https://health.dotenv.org) for more information.
+Set the production `DOTENV_KEY` on your server, recommit your `.env.vault` file to code, and deploy. That's it!
 
-## FAQ
+## ❓ FAQ
 
 #### What happens if `DOTENV_KEY` is not set?
 
-Dotenv Vault gracefully falls back to [dotenv](https://github.com/bkeepers/dotenv) when `DOTENV_KEY` is not set. This is the default for development so that you can focus on editing your `.env` file and save the `build` command until you are ready to deploy those environment variables changes.
+Dotenv Vault gracefully falls back to [python-dotenv](https://github.com/theskumar/python-dotenv) when `DOTENV_KEY` is not set. This is the default for development so that you can focus on editing your `.env` file and save the `build` command until you are ready to deploy those environment variables changes.
 
 #### Should I commit my `.env` file?
 
 No. We **strongly** recommend against committing your `.env` file to version control. It should only include environment-specific values such as database passwords or API keys. Your production database should have a different password than your development database.
 
 #### Should I commit my `.env.vault` file?
```

### Comparing `python-dotenv-vault-0.4.1a0/setup.py` & `python-dotenv-vault-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.4.1a0/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,147 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.4.1a0
+Version: 0.5.0
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
 
-# python-dotenv-vault
+# python-dotenv-vault [![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
 
 <img src="https://raw.githubusercontent.com/motdotla/dotenv/master/dotenv.svg" alt="dotenv-vault" align="right" width="200" />
 
-[![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
-
 Extends the proven & trusted foundation of [python-dotenv](https://github.com/theskumar/python-dotenv), with a `.env.vault` file.
 
-The extended standard lets you sync your `.env` files – quickly & securely. Stop sharing them over insecure channels like Slack and email, and never lose an important `.env` file again.
+The extended standard lets you load encrypted secrets from your `.env.vault` file in production (and other) environments. Brought to you by the same people that pioneered [dotenv-nodejs](https://github.com/motdotla/dotenv).
+
+* [🌱 Install](#-install)
+* [🏗️ Usage (.env)](#%EF%B8%8F-usage)
+* [🚀 Deploying (.env.vault) 🆕](#-deploying)
+* [🌴 Multiple Environments](#-manage-multiple-environments)
+* [❓ FAQ](#-faq)
+* [⏱️ Changelog](./CHANGELOG.md)
 
-## Installation
+## 🌱 Install
 
 ```shell
 pip install python-dotenv-vault
 ```
 
+## 🏗️ Usage
+
+Development usage works just like [python-dotenv](https://github.com/theskumar/python-dotenv).
+
+Add your application configuration to your `.env` file in the root of your project:
+
+```shell
+S3_BUCKET=YOURS3BUCKET
+SECRET_KEY=YOURSECRETKEYGOESHERE
+```
+
 As early as possible in your application bootstrap process, load .env:
 
 ```python
 from dotenv_vault import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 # Code of your application, which uses environment variables (e.g. from `os.environ` or
 # `os.getenv`) as if they came from the actual environment.
 ```
 
-## Usage
-
-### `.env`
-
-Basic usage works just like [python-dotenv](https://github.com/theskumar/python-dotenv).
-
-Add your application configuration to your `.env` file in the root of your project:
-
-```shell
-S3_BUCKET=YOURS3BUCKET
-SECRET_KEY=YOURSECRETKEYGOESHERE
-```
-
 When your application loads, these variables will be available in `os.environ` or `os.getenv`:
 
 ```python
 s3_bucket = os.getenv("S3_BUCKET")
 print(s3_bucket)
 ```
 
-### `.env.vault`
-
-The `.env.vault` extends `.env`. It facilitates syncing your .env file across machines, team members, and environments.
+## 🚀 Deploying
 
-Usage is similar to git. In the same directory as your `.env` file, run the command:
+Encrypt your environment variables by doing:
 
 ```shell
-$ npx dotenv-vault new
+npx dotenv-vault local build
 ```
 
-Follow those instructions and then run:
+This will create an encrypted `.env.vault` file along with a `.env.keys` file containing the encryption keys. Set the `DOTENV_KEY` environment variable by copying and pasting the key value from the `.env.keys` file onto your server or cloud provider. For example in heroku:
 
 ```shell
-$ npx dotenv-vault login
+heroku config:set DOTENV_KEY=<key string from .env.keys>
 ```
 
-Then run push and pull:
+Commit your .env.vault file safely to code and deploy. Your .env.vault fill be decrypted on boot, its environment variables injected, and your app work as expected.
 
-```shell
-$ npx dotenv-vault push
-$ npx dotenv-vault pull
-```
+Note that when the `DOTENV_KEY` environment variable is set, environment settings will *always* be loaded from the `.env.vault` file in the project root. For development use, you can leave the `DOTENV_KEY` environment variable unset and fall back on the `dotenv` behaviour of loading from `.env` or a specified set of files (see [here in the `dotenv` README](https://github.com/bkeepers/dotenv#usage) for the details).
 
-That's it!
+## 🌴 Manage Multiple Environments
 
-You just synced your `.env` file. Commit your `.env.vault` file to code, and tell your teammates to run `npx dotenv-vault pull`.
+You have two options for managing multiple environments - locally managed or vault managed - both use [dotenv-vault](https://github.com/dotenv-org/dotenv-vault).
 
-[Learn more](https://www.dotenv.org/docs/tutorials/sync)
+Locally managed never makes a remote API call. It is completely managed on your machine. Vault managed adds conveniences like backing up your .env file, secure sharing across your team, access permissions, and version history. Choose what works best for you.
 
-## Multiple Environments
+#### 💻 Locally Managed
 
-Run the command:
+Create a `.env.production` file in the root of your project and put your production values there.
 
 ```shell
-$ npx dotenv-vault open production
+# .env.production
+S3_BUCKET="PRODUCTION_S3BUCKET"
+SECRET_KEY="PRODUCTION_SECRETKEYGOESHERE"
 ```
 
-It will open up an interface to manage your production environment variables.
-
-[Learn more](https://www.dotenv.org/docs/tutorials/environments)
-
-## Integrate Anywhere™
-
-Build your encrypted `.env.vault`:
+Rebuild your `.env.vault` file.
 
 ```shell
-$ npx dotenv-vault build
+npx dotenv-vault local build
 ```
 
-Safely commit and push your changes:
+View your `.env.keys` file. There is a production `DOTENV_KEY` that pairs with the `DOTENV_VAULT_PRODUCTION` cipher in your `.env.vault` file.
 
-```shell
-$ git commit -am "Updated .env.vault"
-$ git push
-```
+Set the production `DOTENV_KEY` on your server, recommit your `.env.vault` file to code, and deploy. That's it!
 
-Obtain your `DOTENV_KEY`:
+Your .env.vault fill be decrypted on boot, its production environment variables injected, and your app work as expected.
 
-```shell
-$ npx dotenv-vault keys
-```
+#### 🔐 Vault Managed
 
-Set `DOTENV_KEY` on your infrastructure. For example, on Heroku:
+Sync your .env file. Run the push command and follow the instructions. [learn more](/docs/sync/quickstart)
 
-```shell
-$ heroku config:set DOTENV_KEY="dotenv://:key_1234@dotenv.org/vault/.env.vault?environment=production"
+```
+$ npx dotenv-vault push
 ```
 
-All set! When your app boots, it will recognize a `DOTENV_KEY` is set, decrypt the `.env.vault` file, and load the variables to `ENV`.
+Manage multiple environments with the included UI. [learn more](/docs/tutorials/environments)
 
-Made a change to your production envs? Run `npx dotenv-vault build`, commit that safely to code, and deploy. It's simple and safe like that.
+```
+$ npx dotenv-vault open
+```
 
-[Learn more](https://www.dotenv.org/docs/tutorials/integrations)
+Build your `.env.vault` file with multiple environments.
 
-## Dotenv.org
+```
+$ npx dotenv-vault build
+```
 
-You need a [Dotenv Account](https://dotenv.org) to use Dotenv Vault. It is free to use with premium features.
+Access your `DOTENV_KEY`.
 
-![](https://api.checklyhq.com/v1/badges/checks/c2fee99a-38e7-414e-89b8-9766ceeb1927?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/4f557967-1ed1-486a-b762-39a63781d752?style=flat&theme=dark&responseTime=true)
-<br>
-![](https://api.checklyhq.com/v1/badges/checks/804eb6fa-6599-4688-a649-7ff3c39a64b9?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/6a94504e-e936-4f07-bc0b-e08fee2734b3?style=flat&theme=dark&responseTime=true)
-<br>
-![](https://api.checklyhq.com/v1/badges/checks/06ac4f4e-3e0e-4501-9987-580b4d2a6b06?style=flat&theme=dark&responseTime=true)
-![](https://api.checklyhq.com/v1/badges/checks/0ffc1e55-7ef0-4c2c-8acc-b6311871f41c?style=flat&theme=dark&responseTime=true)
+```
+$ npx dotenv-vault keys
+```
 
-Visit [health.dotenv.org](https://health.dotenv.org) for more information.
+Set the production `DOTENV_KEY` on your server, recommit your `.env.vault` file to code, and deploy. That's it!
 
-## FAQ
+## ❓ FAQ
 
 #### What happens if `DOTENV_KEY` is not set?
 
-Dotenv Vault gracefully falls back to [dotenv](https://github.com/bkeepers/dotenv) when `DOTENV_KEY` is not set. This is the default for development so that you can focus on editing your `.env` file and save the `build` command until you are ready to deploy those environment variables changes.
+Dotenv Vault gracefully falls back to [python-dotenv](https://github.com/theskumar/python-dotenv) when `DOTENV_KEY` is not set. This is the default for development so that you can focus on editing your `.env` file and save the `build` command until you are ready to deploy those environment variables changes.
 
 #### Should I commit my `.env` file?
 
 No. We **strongly** recommend against committing your `.env` file to version control. It should only include environment-specific values such as database passwords or API keys. Your production database should have a different password than your development database.
 
 #### Should I commit my `.env.vault` file?
 
@@ -179,15 +167,31 @@
 
 MIT
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
-## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.2.0...master)
+## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.0...master)
+
+## 0.5.0
+
+### Added
+
+ - Reorganise and simplify code
+ - Make API correspond more closely to `python-dotenv`
+ - Improve error handling
+ - Add tests and CI
+ - Upgrade to `build` for release build
+ 
+## 0.4.1
+
+### Added
+
+- expand cryptography library version range for better support
 
 ## 0.4.0
 
 ### Added
 
 - Added feature to allow custom .env.vault path
```

