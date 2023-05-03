# Comparing `tmp/slack-watchman-3.0.9.tar.gz` & `tmp/slack-watchman-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slack-watchman-3.0.9.tar", last modified: Sat Oct 31 19:47:42 2020, max compression
+gzip compressed data, was "slack-watchman-4.0.0.tar", last modified: Wed May  3 19:18:55 2023, max compression
```

## Comparing `slack-watchman-3.0.9.tar` & `slack-watchman-4.0.0.tar`

### file list

```diff
@@ -1,68 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-31 19:47:42.396689 slack-watchman-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (116)      114 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9411 2020-10-31 19:47:42.396689 slack-watchman-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7084 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-31 19:47:42.396689 slack-watchman-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1307 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-31 19:47:42.388689 slack-watchman-3.0.9/slack_watchman/
--rw-r--r--   0 runner    (1001) docker     (116)     1136 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/__about__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15671 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      264 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     5733 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-31 19:47:42.396689 slack-watchman-3.0.9/slack_watchman/rules/
--rw-r--r--   0 runner    (1001) docker     (116)      496 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/access_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      356 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/archive_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      466 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/aws_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      590 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/azure_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      651 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/azure_service_account_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      603 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/bank_cards.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      513 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/bearer_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      408 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/budget_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      371 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/certificate_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      508 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/client_secrets.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      435 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/cloudflare_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      329 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/config_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      438 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/cusip_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      411 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/cv_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      512 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/date_of_birth.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      487 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/drivers_licence_uk.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      403 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/excel_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      355 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/executable_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      510 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/facebook_access_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      569 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/facebook_secret_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      508 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/gcp_service_account_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      550 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/gcp_service_accounts_text.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      542 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/github_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      504 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/google_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      487 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/heroku_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      574 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/iban_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      783 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/interesting_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      473 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/itin_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      450 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/mailchimp_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      488 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/mailgun_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      457 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/mastercard_datacash.yml
--rw-r--r--   0 runner    (1001) docker     (116)      572 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/ni_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      435 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/passport_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      563 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/passwords.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      551 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/paypal_braintree.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      380 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/powerpoint_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      629 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/private_keys.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      539 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/private_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      507 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/s3_config_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      445 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/shodan_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      453 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/slack_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      538 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/slack_webhooks.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      498 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/ssn_us.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      534 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/stripe_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      429 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/twilio_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      775 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/twitter_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      381 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/rules/word_files.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    12923 2020-10-31 19:47:29.000000 slack-watchman-3.0.9/slack_watchman/slack_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-31 19:47:42.388689 slack-watchman-3.0.9/slack_watchman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9411 2020-10-31 19:47:42.000000 slack-watchman-3.0.9/slack_watchman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2419 2020-10-31 19:47:42.000000 slack-watchman-3.0.9/slack_watchman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-31 19:47:42.000000 slack-watchman-3.0.9/slack_watchman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-10-31 19:47:42.000000 slack-watchman-3.0.9/slack_watchman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       35 2020-10-31 19:47:42.000000 slack-watchman-3.0.9/slack_watchman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-10-31 19:47:42.000000 slack-watchman-3.0.9/slack_watchman.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.444386 slack-watchman-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.448386 slack-watchman-4.0.0/src/slack_watchman/
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/src/slack_watchman/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/signature_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/slack_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/sw_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.452387 slack-watchman-4.0.0/src/slack_watchman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/top_level.txt
```

### Comparing `slack-watchman-3.0.9/PKG-INFO` & `slack-watchman-4.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,190 @@
-Metadata-Version: 2.1
-Name: slack-watchman
-Version: 3.0.9
-Summary: Monitoring your Slack workspaces for sensitive information
-Home-page: https://github.com/PaperMtn/slack-watchman
-Author: PaperMtn
-Author-email: papermtn@protonmail.com
-License: GPL-3.0
-Description: <img src="https://i.imgur.com/RsZPaC9.png" width="550">
-        
-        # Slack Watchman
-        ![Python 2.7 and 3 compatible](https://img.shields.io/pypi/pyversions/slack-watchman)
-        ![PyPI version](https://img.shields.io/pypi/v/slack-watchman.svg)
-        ![License: MIT](https://img.shields.io/pypi/l/slack-watchman.svg)
-        
-        Monitoring your Slack workspaces for sensitive information
-        
-        ## About Slack Watchman
-        Slack Watchman is an application that uses the Slack API to look for potentially sensitive data exposed in your Slack workspaces.
-        
-        More information about Slack Watchman can be found [on my blog](https://papermtn.co.uk/slack-watchman-monitoring-slack-workspaces-for-sensitive-information/).
-        
-        ### Features
-        Slack Watchman looks for:
-        
-        - API Keys, Tokens & Service Accounts
-          - AWS, Azure, GCP, Google API, Slack (keys & webhooks), Twitter, Facebook, GitHub
-          - Generic Private keys
-          - Access Tokens, Bearer Tokens, Client Secrets, Private Tokens
-        - Files
-            - Certificate files
-            - Potentially interesting/malicious/sensitive files (.docm, .xlsm, .zip etc.)
-            - Executable files
-            - Keychain files
-            - Config files for popular services (Terraform, Jenkins, OpenVPN and more)
-        - Personal Data
-            - Leaked passwords
-            - Passport numbers, Dates of birth, Social security numbers, National insurance numbers, Drivers licence numbers (UK), Individual Taxpayer Identification Number
-        - Financial data
-            - Paypal Braintree tokens, Bank card details, IBAN numbers, CUSIP numbers
-        
-        It also gives the following, which can be used for general auditing:
-        - User data
-            - All users & all admins
-        - Channel data
-            - All channels, including externally shared channels
-        
-        #### Time based searching
-        You can run Slack Watchman to look for results going back as far as:
-        - 24 hours
-        - 7 days
-        - 30 days
-        - All time
-        
-        This means after one deep scan, you can schedule Slack Watchman to run regularly and only return results from your chosen timeframe.
-        
-        ### Rules
-        Slack Watchman uses custom YAML rules to detect matches in Slack.
-        
-        They follow this format:
-        
-        ```yaml
-        ---
-        filename:
-        enabled: [true|false]
-        meta:
-          name:
-          author:
-          date:
-          description: #what the search should find
-          severity: #rating out of 100
-        category: #[files|tokens|financial|pii]
-        scope:
-        - #[files|messages]
-        file_types: #optional list for use with file searching
-        test_cases:
-          match_cases:
-          - #test case that should match the regex*
-          fail_cases:
-          - #test case that should not match the regex*
-        strings:
-        - #search query to use in Slack*
-        pattern: #Regex pattern to filter out false positives*
-        ```
-        There are Python tests to ensure rules are formatted properly and that the Regex patterns work in the `tests` dir
-        
-        More information about rules, and how you can add your own, is in the file `docs/rules.md`.
-        
-        ### Logging
-        
-        Slack Watchman gives the following logging options:
-        - CSV
-        - Log file
-        - Stdout
-        - TCP stream
-        
-        When using CSV logging, searches for rules are returned in separate CSV files, for all other methods of logging, results are output in JSON format, perfect for ingesting into a SIEM or other log analysis platform.
-        
-        For file and TCP stream logging, configuration options need to be passed via `.conf` file or environment variable. See the file `docs/logging.md` for instructions on how to set it up.
-        
-        If no logging option is given, Slack Watchman defaults to CSV logging.
-        
-        ## Requirements
-        ### Slack API token
-        To run Slack Watchman, you will need a Slack API OAuth access token. You can do this by creating a simple [Slack App](https://api.slack.com/apps).
-        
-        The app needs to have the following **User Token Scopes** added:
-        ```
-        channels:read
-        files:read
-        groups:read
-        im:read
-        links:read
-        mpim:read
-        remote_files:read
-        search:read
-        team:read
-        users:read
-        users:read.email
-        ```
-        **Note**: User tokens act on behalf of the user who authorises them, so I would suggest you create this app and authorise it using a service account, otherwise the app will have access to your private channels and chats.
-        
-        #### Providing token
-        Slack Watchman will first try to get the the Slack token from the environment variable `SLACK_WATCHMAN_TOKEN`, if this fails it will load the token from .conf file (see below).
-        
-        ### .conf file
-        Configuration options can be passed in a file named `watchman.conf` which must be stored in your home directory. The file should follow the YAML format, and should look like below:
-        ```yaml
-        slack_watchman:
-          token: xoxp-xxxxxxxx
-          logging:
-            file_logging:
-              path:
-            json_tcp:
-              host:
-              port:
-        ```
-        Slack Watchman will look for this file at runtime, and use the configuration options from here. If you are not using the advanced logging features, leave them blank.
-        
-        If you are having issues with your .conf file, run it through a YAML linter.
-        
-        An example file is in `docs/example.conf`
-        
-        ## Installation
-        Install via pip
-        
-        `pip install slack-watchman`
-        
-        ## Usage
-        Slack Watchman will be installed as a global command, use as follows:
-        ```
-        usage: slack-watchman [-h] --timeframe {d,w,m,a}
-                              [--output {csv,file,stdout,stream}] [--version] [--all]
-                              [--users] [--channels] [--pii] [--financial] [--tokens]
-                              [--files] [--custom CUSTOM]
-        
-        Monitoring your Slack workspaces for sensitive information
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --output {csv,file,stdout,stream}
-                                Where to send results
-          --version             show program's version number and exit
-          --all                 Find everything
-          --users               Find all users
-          --channels            Find all channels
-          --pii                 Find personal data: Passwords, DOB, passport details,
-                                drivers licence, ITIN, SSN
-          --financial           Find financial data: Card details, PayPal Braintree
-                                tokens, IBAN numbers, CUSIP numbers
-          --tokens              Find tokens: Private keys, AWS, GCP, Google API,
-                                Slack, Slack webhooks, Facebook, Twitter, GitHub
-          --files               Find files: Certificates, interesting/malicious files
-          --custom              Search for user defined custom search queries that you
-                                have created rules for
-        
-        required arguments:
-          --timeframe {d,w,m,a}
-                                How far back to search: d = 24 hours w = 7 days, m =
-                                30 days, a = all time
-          ```
-        
-        You can run Slack Watchman to look for everything, and output to default CSV:
-        
-        `slack-watchman --timeframe a --all`
-        
-        Or arguments can be grouped together to search more granularly. This will look for tokens and files for the last 30 days, and output the results to a TCP stream:
-        
-        `slack-watchman --timeframe m --tokens --files --output stream`
-        
-        ## Other Watchman apps
-        You may be interested in some of the other apps in the Watchman family:
-        - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
-        - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
-        
-        ## License
-        The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack.
-        
-Keywords: audit slack slack-watchman watchman blue-team red-team threat-hunting
-Platform: UNKNOWN
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+<img src="https://i.imgur.com/jeU9F0a.png" width="550">
+
+# Slack Watchman
+![Python 2.7 and 3 compatible](https://img.shields.io/pypi/pyversions/slack-watchman)
+![PyPI version](https://img.shields.io/pypi/v/slack-watchman.svg)
+![License: MIT](https://img.shields.io/pypi/l/slack-watchman.svg)
+
+Monitoring and enumerating Slack for exposed secrets
+
+## About Slack Watchman
+Slack Watchman is an application that uses the Slack API to find potentially sensitive data exposed in a Slack workspace, and to enumerate other useful information for red, blue and purple teams.
+
+More information about Slack Watchman can be found [on my blog](https://papermtn.co.uk/slack-watchman-monitoring-slack-workspaces-for-sensitive-information/).
+
+### Features
+Slack Watchman looks for:
+
+- API Keys, Tokens & Service Accounts
+  - AWS, Azure, GCP, Google API, Slack (keys & webhooks), Twitter, Facebook, GitHub and more
+  - Generic Private keys
+  - Access Tokens, Bearer Tokens, Client Secrets, Private Tokens
+- Files
+    - Certificate files
+    - Potentially interesting/malicious/sensitive files (.docm, .xlsm, .zip etc.)
+    - Executable files
+    - Keychain files
+    - Config files for popular services (Terraform, Jenkins, OpenVPN and more)
+- Personal Data
+    - Leaked passwords
+    - Passport numbers, Dates of birth, Social security numbers, National insurance numbers and more
+- Financial data
+    - Paypal Braintree tokens, Bank card details, IBAN numbers, CUSIP numbers and more
+
+It also enumerates the following:
+- User data
+    - All users & all admins
+- Channel data
+    - All channels, including externally shared channels
+
+#### Time based searching
+You can run Slack Watchman to look for results going back as far as:
+- 24 hours
+- 7 days
+- 30 days
+- All time
+
+This means after one deep scan, you can schedule Slack Watchman to run regularly and only return results from your chosen timeframe.
+
+### Signatures
+Slack Watchman uses custom YAML signatures to detect matches in Slack. These signatures are pulled from the central [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures). Slack Watchman automatically updates its signature base at runtime to ensure its using the latest signatures to detect secrets.
+
+### Logging
+
+Slack Watchman gives the following logging options:
+- Terminal-friendly Stdout
+- JSON to Stdout
+
+Slack Watchman defaults to terminal-friendly stdout logging if no option is given. This is designed to be easier for humans to read.
+
+JSON logging is also available, which is perfect for ingesting into a SIEM or other log analysis platforms.
+
+JSON formatted logging can be easily redirected to a file as below:
+```commandline
+slack-watchman --timeframe a --all --output json >> slack_watchman_log.json 
+```
+
+## Authentication Requirements
+### Slack API token
+To run Slack Watchman, you will need a Slack API OAuth access token. You can do this by creating a simple [Slack App](https://api.slack.com/apps).
+
+The app needs to have the following **User Token Scopes** added:
+```
+channels:read
+files:read
+groups:read
+im:read
+links:read
+mpim:read
+remote_files:read
+search:read
+team:read
+users:read
+users:read.email
+```
+**Note**: User tokens act on behalf of the user who authorises them, so I would suggest you create this app and authorise it using a service account, otherwise the app will have access to your private channels and chats.
+
+### Cookie Authentication
+Alternatively, Slack Watchman can also authenticate to Slack using a user `d` cookie, which is stored in the browser of each user logged into a workspace.
+
+To use cookie authentication, you will need to provide the `d` cookie, and the URL of the target workspace. Then you will need to use the `--cookie` flag when running Slack Watchman
+
+More information on cookie authentication can be found [on my blog](https://papermtn.co.uk/category/tools/slack-watchman/)
+#### Providing tokens
+Slack Watchman will first try to get the Slack token (plus the cookie token and URL if selected) from the environment variables 
+- `SLACK_WATCHMAN_TOKEN`
+- `SLACK_WATCHMAN_COOKIE`
+- `SLACK_WATCHMAN_URL`
+
+If this fails it will try to load the token(s) from `.conf` file (see below).
+
+#### .conf file
+Configuration options can be passed in a file named `watchman.conf` which must be stored in your home directory. The file should follow the YAML format, and should look like below:
+```yaml
+slack_watchman:
+  token: xoxp-xxxxxxxx
+  cookie: xoxd-%2xxxxx
+  url: https://xxxxx.slack.com
+```
+Slack Watchman will look for this file at runtime, and use the configuration options from here. If you are not using cookie auth, leave `cookie` and `url` blank.
+
+If you are having issues with your .conf file, run it through a YAML linter.
+
+An example file is in `docs/example.conf`
+
+**Note**: Cookie and URL values are optional, and not required if not using cookie authentication.
+
+## Installation
+You can install the latest stable version via pip:
+
+```commandline
+python3 -m pip install slack-watchman
+```
+
+Or build from source yourself:
+
+Download the release source files, then from the top level repository run:
+```commandline
+python3 -m pip build
+python3 -m pip install --force-reinstall dist/*.whl
+```
+
+## Docker Image
+
+Slack Watchman is also available from the Docker hub as a Docker image:
+
+`docker pull papermountain/slack-watchman:latest`
+
+You can then run Slack Watchman in a container, making sure you pass the required environment variables:
+
+```commandline
+// help
+docker run --rm papermountain/slack-watchman -h
+
+// scan all
+docker run --rm -e SLACK_WATCHMAN_TOKEN=xoxp... papermountain/slack-watchman --timeframe a --all --output json
+docker run --rm --env-file .env papermountain/slack-watchman --timeframe a --all --output stdout
+```
+
+## Usage
+Slack Watchman will be installed as a global command, use as follows:
+```commandline
+usage: slack-watchman [-h] --timeframe {d,w,m,a} [--output {json,stdout}] [--version] [--all] [--users] [--channels] [--pii] [--secrets]
+                      [--debug] [--verbose] [--cookie]
+
+Monitoring and enumerating Slack for exposed secrets
+
+options:
+  -h, --help            show this help message and exit
+  --output {json,stdout}, -o {json,stdout}
+                        Where to send results
+  --version, -v         show program's version number and exit
+  --all, -a             Find secrets and PII
+  --users, -u           Enumerate users and output them to .csv
+  --channels, -c        Enumerate channels and output them to .csv
+  --pii, -p             Find personal data: DOB, passport details, drivers licence, ITIN, SSN etc.
+  --secrets, -s         Find exposed secrets: credentials, tokens etc.
+  --debug, -d           Turn on debug level logging
+  --verbose, -V         Turn on more verbose output for JSON logging. This includes more fields, but is larger
+  --cookie              Use cookie auth using Slack d cookie. REQUIRES either SLACK_WATCHMAN_COOKIE and SLACK_WATCHMAN_URL environment
+                        variables set, or both values set in watchman.conf
+
+required arguments:
+  --timeframe {d,w,m,a}, -t {d,w,m,a}
+                        How far back to search: d = 24 hours w = 7 days, m = 30 days, a = all time
+  ```
+
+You can run Slack Watchman to look for everything, and output to default stdout:
+
+```commandline
+slack-watchman --timeframe a --all
+```
+
+## Other Watchman apps
+You may be interested in the other apps in the Watchman family:
+- [Slack Watchman for Enterprise Grid](https://github.com/PaperMtn/slack-watchman-enterprise-grid)
+- [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
+- [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
+
+## License
+The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
```

### Comparing `slack-watchman-3.0.9/slack_watchman/__about__.py` & `slack-watchman-4.0.0/src/slack_watchman/__version__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Slack Watchman
-# Copyright (C) 2020  PaperMtn
+# Copyright (C) 2023  PaperMtn
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -21,14 +21,15 @@
     '__version__',
     '__author__',
     '__email__',
     '__license__',
 ]
 
 __title__ = 'Slack Watchman'
-__summary__ = 'Monitoring your Slack workspaces for sensitive information'
-__uri__ = 'https://github.com/PaperMtn/slack-watchman'
-__version__ = '3.0.9'
+__version__ = '4.0.0'
+__summary__ = 'Monitoring and enumerating Slack for exposed secrets'
 __author__ = 'PaperMtn'
 __email__ = 'papermtn@protonmail.com'
 __license__ = 'GPL-3.0'
-__copyright__ = '2020 {}'.format(__author__)
+__uri__ = 'https://github.com/PaperMtn/slack-watchman'
+__copyright__ = f'2023 {__author__}'
+
```

