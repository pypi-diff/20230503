# Comparing `tmp/dipdup-6.5.5.tar.gz` & `tmp/dipdup-6.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-6.5.5.tar", max compression
+gzip compressed data, was "dipdup-6.5.6.tar", max compression
```

## Comparing `dipdup-6.5.5.tar` & `dipdup-6.5.6.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0     1067 2023-04-17 23:05:28.327453 dipdup-6.5.5/LICENSE
--rw-r--r--   0        0        0     2787 2023-04-17 23:05:28.327453 dipdup-6.5.5/README.md
--rw-r--r--   0        0        0     2778 2023-04-17 23:05:28.355454 dipdup-6.5.5/pyproject.toml
--rw-r--r--   0        0        0      213 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/__init__.py
--rw-r--r--   0        0        0      106 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/__main__.py
--rw-r--r--   0        0        0      585 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/baking_bad.py
--rw-r--r--   0        0        0    18507 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/cli.py
--rw-r--r--   0        0        0    22289 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/codegen.py
--rw-r--r--   0        0        0    69778 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/config.py
--rw-r--r--   0        0        0    25902 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/context.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/coinbase/__init__.py
--rw-r--r--   0        0        0     2387 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/coinbase/datasource.py
--rw-r--r--   0        0        0     1309 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/coinbase/models.py
--rw-r--r--   0        0        0     6291 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/datasource.py
--rw-r--r--   0        0        0     2420 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/factory.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/ipfs/__init__.py
--rw-r--r--   0        0        0      688 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/ipfs/datasource.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/metadata/__init__.py
--rw-r--r--   0        0        0     1773 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/metadata/datasource.py
--rw-r--r--   0        0        0      155 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/metadata/enums.py
--rw-r--r--   0        0        0     2172 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/subscription.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/tzkt/__init__.py
--rw-r--r--   0        0        0    46886 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/tzkt/datasource.py
--rw-r--r--   0        0        0     9895 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/datasources/tzkt/models.py
--rw-r--r--   0        0        0    24980 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     2013 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/enums.py
--rw-r--r--   0        0        0     2192 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/env.py
--rw-r--r--   0        0        0     9500 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     2734 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/fetcher.py
--rw-r--r--   0        0        0    25590 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/hasura.py
--rw-r--r--   0        0        0     9795 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/http.py
--rw-r--r--   0        0        0     7414 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/__init__.py
--rw-r--r--   0        0        0     3033 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/fetcher.py
--rw-r--r--   0        0        0     7103 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/index.py
--rw-r--r--   0        0        0     2131 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/matcher.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/__init__.py
--rw-r--r--   0        0        0     1402 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/fetcher.py
--rw-r--r--   0        0        0     5324 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/index.py
--rw-r--r--   0        0        0     3297 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/matcher.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/head/__init__.py
--rw-r--r--   0        0        0     2320 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/head/index.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/__init__.py
--rw-r--r--   0        0        0    19397 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/fetcher.py
--rw-r--r--   0        0        0    13344 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/index.py
--rw-r--r--   0        0        0     7386 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/matcher.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/__init__.py
--rw-r--r--   0        0        0     1357 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/fetcher.py
--rw-r--r--   0        0        0     5377 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/index.py
--rw-r--r--   0        0        0     1791 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/matcher.py
--rwxr-xr-x   0        0        0     8269 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/install.py
--rw-r--r--   0        0        0    22523 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/models.py
--rw-r--r--   0        0        0    10978 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/project.py
--rw-r--r--   0        0        0      203 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0     2097 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0      431 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/Dockerfile.j2
--rw-r--r--   0        0        0      474 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      489 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/dipdup.dev.yml.j2
--rw-r--r--   0        0        0      481 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/dipdup.prod.yml.j2
--rw-r--r--   0        0        0     2907 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/docker-compose.swarm.yml.j2
--rw-r--r--   0        0        0     1341 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/docker-compose.yml.j2
--rw-r--r--   0        0        0       37 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/replay.json.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0      197 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
--rw-r--r--   0        0        0      128 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/blank/dipdup.yml.j2
--rw-r--r--   0        0        0       95 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-auction.json
--rw-r--r--   0        0        0       98 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-big-maps.json
--rw-r--r--   0        0        0       83 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-dao.json
--rw-r--r--   0        0        0       83 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-dex.json
--rw-r--r--   0        0        0       95 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-domains.json
--rw-r--r--   0        0        0       92 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-events.json
--rw-r--r--   0        0        0      101 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-factories.json
--rw-r--r--   0        0        0       86 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-head.json
--rw-r--r--   0        0        0      119 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-nft-marketplace.json
--rw-r--r--   0        0        0       83 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-raw.json
--rw-r--r--   0        0        0      119 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-token-transfers.json
--rw-r--r--   0        0        0       89 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-token.json
--rw-r--r--   0        0        0     1116 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      918 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1624 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      853 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1524 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      779 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      847 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1713 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      840 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      702 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_dao/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      416 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     4878 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0     1842 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1769 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      587 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1642 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1689 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1039 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      960 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1868 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1795 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      581 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1636 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1655 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1160 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      956 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      948 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      900 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      564 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      536 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1475 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      819 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      592 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_events/dipdup.yml.j2
--rw-r--r--   0        0        0      976 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      716 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
--rw-r--r--   0        0        0      416 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      333 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_head/dipdup.yml.j2
--rw-r--r--   0        0        0     1230 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      586 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1018 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      949 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      866 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1382 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      486 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      350 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      235 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      787 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      453 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      647 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      945 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      456 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      550 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      822 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     1226 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_default/Makefile.j2
--rw-r--r--   0        0        0     1032 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_default/pyproject.toml.j2
--rw-r--r--   0        0        0      923 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_none/Makefile.j2
--rw-r--r--   0        0        0      552 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_none/pyproject.toml.j2
--rw-r--r--   0        0        0     4008 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/py.typed
--rw-r--r--   0        0        0     4845 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     6041 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0      227 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0      157 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/templates/models.py.j2
--rw-r--r--   0        0        0     3029 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/transactions.py
--rw-r--r--   0        0        0     4631 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/__init__.py
--rw-r--r--   0        0        0     1824 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/codegen.py
--rw-r--r--   0        0        0    11813 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/database.py
--rw-r--r--   0        0        0     2044 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/sys.py
--rw-r--r--   0        0        0     4513 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/yaml.py
--rw-r--r--   0        0        0     4690 1970-01-01 00:00:00.000000 dipdup-6.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-02 23:14:20.261844 dipdup-6.5.6/LICENSE
+-rw-r--r--   0        0        0     3937 2023-05-02 23:14:20.261844 dipdup-6.5.6/README.md
+-rw-r--r--   0        0        0     2778 2023-05-02 23:14:20.289845 dipdup-6.5.6/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      585 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/baking_bad.py
+-rw-r--r--   0        0        0    18507 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/cli.py
+-rw-r--r--   0        0        0    22289 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/codegen.py
+-rw-r--r--   0        0        0    69884 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/config.py
+-rw-r--r--   0        0        0    25902 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/context.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/coinbase/__init__.py
+-rw-r--r--   0        0        0     2387 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/coinbase/datasource.py
+-rw-r--r--   0        0        0     1309 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/coinbase/models.py
+-rw-r--r--   0        0        0     6291 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/datasource.py
+-rw-r--r--   0        0        0     2420 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/factory.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/ipfs/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/ipfs/datasource.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/metadata/__init__.py
+-rw-r--r--   0        0        0     1773 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/metadata/datasource.py
+-rw-r--r--   0        0        0      161 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/metadata/enums.py
+-rw-r--r--   0        0        0     2172 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/subscription.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/tzkt/__init__.py
+-rw-r--r--   0        0        0    46886 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/tzkt/datasource.py
+-rw-r--r--   0        0        0     9895 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/tzkt/models.py
+-rw-r--r--   0        0        0    24980 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     2013 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/enums.py
+-rw-r--r--   0        0        0     2192 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/env.py
+-rw-r--r--   0        0        0     9500 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     2734 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0    25590 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/hasura.py
+-rw-r--r--   0        0        0     9793 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/http.py
+-rw-r--r--   0        0        0     7414 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/__init__.py
+-rw-r--r--   0        0        0     3033 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/fetcher.py
+-rw-r--r--   0        0        0     7103 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/index.py
+-rw-r--r--   0        0        0     2131 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/matcher.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/__init__.py
+-rw-r--r--   0        0        0     1402 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/fetcher.py
+-rw-r--r--   0        0        0     5324 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/index.py
+-rw-r--r--   0        0        0     3297 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/matcher.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/head/__init__.py
+-rw-r--r--   0        0        0     2320 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/head/index.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/__init__.py
+-rw-r--r--   0        0        0    19397 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/fetcher.py
+-rw-r--r--   0        0        0    13344 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/index.py
+-rw-r--r--   0        0        0     7386 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/matcher.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/fetcher.py
+-rw-r--r--   0        0        0     5377 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/index.py
+-rw-r--r--   0        0        0     1791 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/matcher.py
+-rwxr-xr-x   0        0        0     8269 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/install.py
+-rw-r--r--   0        0        0    22523 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/models.py
+-rw-r--r--   0        0        0    10978 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/project.py
+-rw-r--r--   0        0        0      203 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0     2097 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0      431 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/Dockerfile.j2
+-rw-r--r--   0        0        0      474 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      489 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/dipdup.dev.yml.j2
+-rw-r--r--   0        0        0      481 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/dipdup.prod.yml.j2
+-rw-r--r--   0        0        0     2907 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/docker-compose.swarm.yml.j2
+-rw-r--r--   0        0        0     1341 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/docker-compose.yml.j2
+-rw-r--r--   0        0        0       37 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/replay.json.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0      197 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
+-rw-r--r--   0        0        0      128 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/blank/dipdup.yml.j2
+-rw-r--r--   0        0        0       95 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-auction.json
+-rw-r--r--   0        0        0       98 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-big-maps.json
+-rw-r--r--   0        0        0       83 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-dao.json
+-rw-r--r--   0        0        0       83 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-dex.json
+-rw-r--r--   0        0        0       95 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-domains.json
+-rw-r--r--   0        0        0       92 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-events.json
+-rw-r--r--   0        0        0      101 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-factories.json
+-rw-r--r--   0        0        0       86 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-head.json
+-rw-r--r--   0        0        0      119 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-nft-marketplace.json
+-rw-r--r--   0        0        0       83 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-raw.json
+-rw-r--r--   0        0        0      119 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-token-transfers.json
+-rw-r--r--   0        0        0       89 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-token.json
+-rw-r--r--   0        0        0     1116 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      918 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1624 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      853 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1524 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      779 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      847 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1713 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      840 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      702 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      416 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     4878 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0     1842 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1769 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      587 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1642 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1689 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1039 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      960 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1868 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1795 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      581 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1636 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1655 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1160 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      956 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      948 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      900 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      564 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      536 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1475 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      819 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      592 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_events/dipdup.yml.j2
+-rw-r--r--   0        0        0      976 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      716 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
+-rw-r--r--   0        0        0      416 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      333 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_head/dipdup.yml.j2
+-rw-r--r--   0        0        0     1230 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      586 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1018 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      949 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      866 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1382 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      486 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      350 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      235 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      787 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      453 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      647 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      945 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      456 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      550 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      822 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     1226 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_default/Makefile.j2
+-rw-r--r--   0        0        0     1032 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_default/pyproject.toml.j2
+-rw-r--r--   0        0        0      923 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_none/Makefile.j2
+-rw-r--r--   0        0        0      552 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_none/pyproject.toml.j2
+-rw-r--r--   0        0        0     4008 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/py.typed
+-rw-r--r--   0        0        0     4845 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     6041 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0      227 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0      157 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/templates/models.py.j2
+-rw-r--r--   0        0        0     3029 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     4631 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/utils/__init__.py
+-rw-r--r--   0        0        0     1824 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/utils/codegen.py
+-rw-r--r--   0        0        0    11813 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/utils/database.py
+-rw-r--r--   0        0        0     2044 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/utils/sys.py
+-rw-r--r--   0        0        0     4513 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/yaml.py
+-rw-r--r--   0        0        0     5840 1970-01-01 00:00:00.000000 dipdup-6.5.6/PKG-INFO
```

### Comparing `dipdup-6.5.5/LICENSE` & `dipdup-6.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/pyproject.toml` & `dipdup-6.5.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "6.5.5"
+version = "6.5.6"
 license = "MIT"
 authors = [
     "Lev Gorodetskiy <dipdup@drsr.io>",
     "Michael Zaikin <mz@baking-bad.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/dipdup-io/dipdup"
@@ -27,25 +27,25 @@
     { include = "dipdup", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 
 asyncpg = "0.27.0"
-datamodel-code-generator = "0.18.0"
+datamodel-code-generator = "0.18.1"
 pydantic = "1.10.7"
 tortoise-orm = "0.19.3"
 
 aiohttp = "^3.8.1"
 aiolimiter = "^1.0.0"
 anyio = "^3.3.2"
 APScheduler = "^3.8.0"
 asyncclick = "^8.0.1"
 orjson = "^3.6.6"
-prometheus-client = "^0.14.1"
+prometheus-client = "^0.16.0"
 pyhumps = "^3.0.2"
 pysignalr = "0.2.0"
 python-dotenv = "^0.19.0"
 "ruamel.yaml" = "^0.17.2"
 sentry-sdk = "^1.4.3"
 sqlparse = "^0.4.2"
 tabulate = "^0.9.0"
```

### Comparing `dipdup-6.5.5/src/dipdup/baking_bad.py` & `dipdup-6.5.6/src/dipdup/baking_bad.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/cli.py` & `dipdup-6.5.6/src/dipdup/cli.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/codegen.py` & `dipdup-6.5.6/src/dipdup/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/config.py` & `dipdup-6.5.6/src/dipdup/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from __future__ import annotations
 
 import hashlib
 import importlib
 import json
 import logging.config
 import re
-import sys
 from abc import ABC
 from abc import abstractmethod
 from collections import Counter
 from contextlib import suppress
 from dataclasses import field
 from pathlib import Path
 from pydoc import locate
@@ -200,16 +199,16 @@
     replay_path: str | None = None
 
 
 @dataclass
 class ResolvedHTTPConfig:
     """HTTP client configuration with defaults"""
 
-    retry_count: int = sys.maxsize
-    retry_sleep: float = 0.0
+    retry_count: int = 10
+    retry_sleep: float = 1.0
     retry_multiplier: float = 1.0
     ratelimit_rate: int = 0
     ratelimit_period: int = 0
     ratelimit_sleep: float = 5.0
     connection_limit: int = 100
     connection_timeout: int = 60
     batch_size: int = 1000
@@ -1279,14 +1278,17 @@
     first_level: int = 0
     last_level: int = 0
 
     def import_objects(self, package: str) -> None:
         for handler_config in self.handlers:
             handler_config.initialize_callback_fn(package)
 
+            if isinstance(handler_config, EventHandlerConfig):
+                handler_config.initialize_event_type(package)
+
 
 ResolvedIndexConfigU = (
     OperationIndexConfig
     | BigMapIndexConfig
     | HeadIndexConfig
     | TokenTransferIndexConfig
     | EventIndexConfig
```

### Comparing `dipdup-6.5.5/src/dipdup/context.py` & `dipdup-6.5.6/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/coinbase/datasource.py` & `dipdup-6.5.6/src/dipdup/datasources/coinbase/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/coinbase/models.py` & `dipdup-6.5.6/src/dipdup/datasources/coinbase/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/datasource.py` & `dipdup-6.5.6/src/dipdup/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/factory.py` & `dipdup-6.5.6/src/dipdup/datasources/factory.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/ipfs/datasource.py` & `dipdup-6.5.6/src/dipdup/datasources/ipfs/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/metadata/datasource.py` & `dipdup-6.5.6/src/dipdup/datasources/metadata/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/subscription.py` & `dipdup-6.5.6/src/dipdup/datasources/subscription.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/tzkt/datasource.py` & `dipdup-6.5.6/src/dipdup/datasources/tzkt/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/datasources/tzkt/models.py` & `dipdup-6.5.6/src/dipdup/datasources/tzkt/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/dipdup.py` & `dipdup-6.5.6/src/dipdup/dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/enums.py` & `dipdup-6.5.6/src/dipdup/enums.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/env.py` & `dipdup-6.5.6/src/dipdup/env.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/exceptions.py` & `dipdup-6.5.6/src/dipdup/exceptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/fetcher.py` & `dipdup-6.5.6/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/hasura.py` & `dipdup-6.5.6/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/http.py` & `dipdup-6.5.6/src/dipdup/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     async def __aenter__(self) -> None:
         """Create underlying aiohttp session"""
         self.__session = aiohttp.ClientSession(
             base_url=self._url,
             json_serialize=lambda *a, **kw: orjson.dumps(*a, **kw).decode(),
             connector=aiohttp.TCPConnector(limit=self._config.connection_limit),
-            timeout=aiohttp.ClientTimeout(connect=self._config.connection_timeout),
+            timeout=aiohttp.ClientTimeout(total=self._config.connection_timeout),
         )
 
     async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: Any) -> None:
         """Close underlying aiohttp session"""
         self._logger.debug('Closing gateway session (%s)', self._url)
         if not self.__session:
             raise FrameworkException('Session is not initialized')
```

### Comparing `dipdup-6.5.5/src/dipdup/index.py` & `dipdup-6.5.6/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/big_map/fetcher.py` & `dipdup-6.5.6/src/dipdup/indexes/big_map/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/big_map/index.py` & `dipdup-6.5.6/src/dipdup/indexes/big_map/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/big_map/matcher.py` & `dipdup-6.5.6/src/dipdup/indexes/big_map/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/event/fetcher.py` & `dipdup-6.5.6/src/dipdup/indexes/event/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/event/index.py` & `dipdup-6.5.6/src/dipdup/indexes/event/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/event/matcher.py` & `dipdup-6.5.6/src/dipdup/indexes/event/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/head/index.py` & `dipdup-6.5.6/src/dipdup/indexes/head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/operation/fetcher.py` & `dipdup-6.5.6/src/dipdup/indexes/operation/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/operation/index.py` & `dipdup-6.5.6/src/dipdup/indexes/operation/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/operation/matcher.py` & `dipdup-6.5.6/src/dipdup/indexes/operation/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/token_transfer/fetcher.py` & `dipdup-6.5.6/src/dipdup/indexes/token_transfer/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/token_transfer/index.py` & `dipdup-6.5.6/src/dipdup/indexes/token_transfer/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/indexes/token_transfer/matcher.py` & `dipdup-6.5.6/src/dipdup/indexes/token_transfer/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/install.py` & `dipdup-6.5.6/src/dipdup/install.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/models.py` & `dipdup-6.5.6/src/dipdup/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/project.py` & `dipdup-6.5.6/src/dipdup/project.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/base/.gitignore.j2` & `dipdup-6.5.6/src/dipdup/projects/base/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/base/docker-compose.swarm.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/base/docker-compose.swarm.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/base/docker-compose.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/base/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_auction/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_auction/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dao/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dao/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_domains/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_domains/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_events/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_events/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_factories/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_factories/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_token/dipdup.yml.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_token/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2` & `dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/linters_default/Makefile.j2` & `dipdup-6.5.6/src/dipdup/projects/linters_default/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/linters_default/pyproject.toml.j2` & `dipdup-6.5.6/src/dipdup/projects/linters_default/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/linters_none/Makefile.j2` & `dipdup-6.5.6/src/dipdup/projects/linters_none/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/projects/linters_none/pyproject.toml.j2` & `dipdup-6.5.6/src/dipdup/projects/linters_none/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/prometheus.py` & `dipdup-6.5.6/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/scheduler.py` & `dipdup-6.5.6/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/sentry.py` & `dipdup-6.5.6/src/dipdup/sentry.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/sql/truncate_schema.sql` & `dipdup-6.5.6/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/transactions.py` & `dipdup-6.5.6/src/dipdup/transactions.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/utils/__init__.py` & `dipdup-6.5.6/src/dipdup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/utils/codegen.py` & `dipdup-6.5.6/src/dipdup/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/utils/database.py` & `dipdup-6.5.6/src/dipdup/utils/database.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/utils/sys.py` & `dipdup-6.5.6/src/dipdup/utils/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.5/src/dipdup/yaml.py` & `dipdup-6.5.6/src/dipdup/yaml.py`

 * *Files identical despite different names*

