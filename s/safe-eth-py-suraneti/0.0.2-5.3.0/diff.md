# Comparing `tmp/safe-eth-py_suraneti-0.0.2.tar.gz` & `tmp/safe-eth-py_suraneti-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py_suraneti-0.0.2.tar", last modified: Fri Feb  3 12:23:40 2023, max compression
+gzip compressed data, was "safe-eth-py_suraneti-5.3.0.tar", last modified: Wed May  3 03:03:49 2023, max compression
```

## Comparing `safe-eth-py_suraneti-0.0.2.tar` & `safe-eth-py_suraneti-5.3.0.tar`

### file list

```diff
@@ -1,191 +1,194 @@
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.294530 safe-eth-py_suraneti-0.0.2/
--rw-r--r--   0 suraneti   (501) staff       (20)     1082 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/LICENSE
--rw-r--r--   0 suraneti   (501) staff       (20)       71 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/MANIFEST.in
--rw-r--r--   0 suraneti   (501) staff       (20)     6621 2023-02-03 12:23:40.294753 safe-eth-py_suraneti-0.0.2/PKG-INFO
--rw-r--r--   0 suraneti   (501) staff       (20)     5399 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/README.rst
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.043102 safe-eth-py_suraneti-0.0.2/docs/
--rw-r--r--   0 suraneti   (501) staff       (20)      638 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/Makefile
--rw-r--r--   0 suraneti   (501) staff       (20)      799 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/make.bat
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.067946 safe-eth-py_suraneti-0.0.2/docs/source/
--rw-r--r--   0 suraneti   (501) staff       (20)     1993 2023-02-03 12:14:56.000000 safe-eth-py_suraneti-0.0.2/docs/source/conf.py
--rw-r--r--   0 suraneti   (501) staff       (20)      964 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      183 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      954 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      177 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 suraneti   (501) staff       (20)     1198 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      450 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      936 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      226 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.rst
--rw-r--r--   0 suraneti   (501) staff       (20)     1852 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/gnosis.safe.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      896 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/index.rst
--rw-r--r--   0 suraneti   (501) staff       (20)       55 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/modules.rst
--rw-r--r--   0 suraneti   (501) staff       (20)     8492 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/docs/source/quickstart.rst
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.069353 safe-eth-py_suraneti-0.0.2/gnosis/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.075627 safe-eth-py_suraneti-0.0.2/gnosis/eth/
--rw-r--r--   0 suraneti   (501) staff       (20)     1126 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.080457 safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/
--rw-r--r--   0 suraneti   (501) staff       (20)      657 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4699 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)      194 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6315 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2324 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 suraneti   (501) staff       (20)      625 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/constants.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.124956 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/
--rw-r--r--   0 suraneti   (501) staff       (20)   328664 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 suraneti   (501) staff       (20)    28908 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    26897 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 suraneti   (501) staff       (20)    29068 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 suraneti   (501) staff       (20)    54748 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 suraneti   (501) staff       (20)    89890 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 suraneti   (501) staff       (20)   622260 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 suraneti   (501) staff       (20)   983403 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)  1158944 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)  1347363 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)   119875 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    19886 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 suraneti   (501) staff       (20)    78793 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 suraneti   (501) staff       (20)   136946 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)   288861 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)    18975 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    32495 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    39032 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)     1862 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)     6967 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7351 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 suraneti   (501) staff       (20)    17165 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 suraneti   (501) staff       (20)     2480 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 suraneti   (501) staff       (20)     2242 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 suraneti   (501) staff       (20)     8293 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 suraneti   (501) staff       (20)    11889 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.137206 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1501 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/admin.py
--rw-r--r--   0 suraneti   (501) staff       (20)      269 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/filters.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2400 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/forms.py
--rw-r--r--   0 suraneti   (501) staff       (20)     8445 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/models.py
--rw-r--r--   0 suraneti   (501) staff       (20)     5740 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.143628 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)      547 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/models.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3013 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7414 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6203 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 suraneti   (501) staff       (20)      508 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 suraneti   (501) staff       (20)      320 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/django/validators.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.144327 safe-eth-py_suraneti-0.0.2/gnosis/eth/eip712/
--rw-r--r--   0 suraneti   (501) staff       (20)     6383 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    81674 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/ethereum_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12510 2023-02-03 11:51:13.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/ethereum_network.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1174 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/exceptions.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12130 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/multicall.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.192214 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/
--rw-r--r--   0 suraneti   (501) staff       (20)     1093 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.215670 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    15986 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    30036 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    29731 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    27567 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12387 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/makerdao.py
--rw-r--r--   0 suraneti   (501) staff       (20)    25872 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)      239 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    45208 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 suraneti   (501) staff       (20)    36257 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1464 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2418 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)      161 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.217336 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/helpers/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     5856 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4250 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 suraneti   (501) staff       (20)    32443 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1687 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1454 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6687 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1100 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.223499 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.227503 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)   107062 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1045 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1246 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1357 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.228846 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/eip712/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4220 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2724 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.235258 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    31306 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12057 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 suraneti   (501) staff       (20)   142499 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 suraneti   (501) staff       (20)    92731 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 suraneti   (501) staff       (20)   169556 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.240063 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3130 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1820 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1460 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2043 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3456 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 suraneti   (501) staff       (20)    71068 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7087 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 suraneti   (501) staff       (20)    21070 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7391 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4474 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/utils.py
--rw-r--r--   0 suraneti   (501) staff       (20)      281 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/typing.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6407 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/eth/utils.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.242342 safe-eth-py_suraneti-0.0.2/gnosis/protocol/
--rw-r--r--   0 suraneti   (501) staff       (20)      177 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/protocol/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     8569 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2695 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/protocol/order.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.243687 safe-eth-py_suraneti-0.0.2/gnosis/protocol/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     5899 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/py.typed
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.253151 safe-eth-py_suraneti-0.0.2/gnosis/safe/
--rw-r--r--   0 suraneti   (501) staff       (20)      716 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.256518 safe-eth-py_suraneti-0.0.2/gnosis/safe/api/
--rw-r--r--   0 suraneti   (501) staff       (20)      346 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/api/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1917 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/api/base_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3062 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     9201 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1451 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/exceptions.py
--rw-r--r--   0 suraneti   (501) staff       (20)    11385 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/multi_send.py
--rw-r--r--   0 suraneti   (501) staff       (20)     8070 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/proxy_factory.py
--rw-r--r--   0 suraneti   (501) staff       (20)    42010 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/safe.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12128 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12937 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)     9664 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_signature.py
--rw-r--r--   0 suraneti   (501) staff       (20)    16937 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4181 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/serializers.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2039 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/signatures.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.285096 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.287054 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/api/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4989 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)    10808 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 suraneti   (501) staff       (20)    10515 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6448 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 suraneti   (501) staff       (20)    32576 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 suraneti   (501) staff       (20)    16621 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)    16950 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)    13884 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12923 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3762 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3701 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1967 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.289127 safe-eth-py_suraneti-0.0.2/gnosis/util/
--rw-r--r--   0 suraneti   (501) staff       (20)       83 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/util/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)      442 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/gnosis/util/util.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-02-03 12:23:40.294050 safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/
--rw-r--r--   0 suraneti   (501) staff       (20)     6621 2023-02-03 12:23:39.000000 safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/PKG-INFO
--rw-r--r--   0 suraneti   (501) staff       (20)     5650 2023-02-03 12:23:39.000000 safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/SOURCES.txt
--rw-r--r--   0 suraneti   (501) staff       (20)        1 2023-02-03 12:23:39.000000 safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/dependency_links.txt
--rw-r--r--   0 suraneti   (501) staff       (20)      125 2023-02-03 12:23:39.000000 safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/requires.txt
--rw-r--r--   0 suraneti   (501) staff       (20)        7 2023-02-03 12:23:39.000000 safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/top_level.txt
--rw-r--r--   0 suraneti   (501) staff       (20)     2395 2023-02-03 12:23:40.296001 safe-eth-py_suraneti-0.0.2/setup.cfg
--rw-r--r--   0 suraneti   (501) staff       (20)       69 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-0.0.2/setup.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.123518 safe-eth-py_suraneti-5.3.0/
+-rw-r--r--   0 suraneti   (501) staff       (20)     1082 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/LICENSE
+-rw-r--r--   0 suraneti   (501) staff       (20)       71 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/MANIFEST.in
+-rw-r--r--   0 suraneti   (501) staff       (20)     6663 2023-05-03 03:03:49.123663 safe-eth-py_suraneti-5.3.0/PKG-INFO
+-rw-r--r--   0 suraneti   (501) staff       (20)     5399 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/README.rst
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.014187 safe-eth-py_suraneti-5.3.0/docs/
+-rw-r--r--   0 suraneti   (501) staff       (20)      638 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/Makefile
+-rw-r--r--   0 suraneti   (501) staff       (20)      799 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/make.bat
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.067731 safe-eth-py_suraneti-5.3.0/docs/source/
+-rw-r--r--   0 suraneti   (501) staff       (20)     1984 2023-02-07 07:15:36.000000 safe-eth-py_suraneti-5.3.0/docs/source/conf.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      964 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      183 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      954 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      177 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)     1198 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      450 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      936 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      226 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)     1852 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/gnosis.safe.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)      896 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/index.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)       55 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/modules.rst
+-rw-r--r--   0 suraneti   (501) staff       (20)     8492 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/docs/source/quickstart.rst
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.070216 safe-eth-py_suraneti-5.3.0/gnosis/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/__init__.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.101621 safe-eth-py_suraneti-5.3.0/gnosis/eth/
+-rw-r--r--   0 suraneti   (501) staff       (20)     1064 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/__init__.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.103559 safe-eth-py_suraneti-5.3.0/gnosis/eth/abis/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/abis/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    19012 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/abis/multicall.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.128906 safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/
+-rw-r--r--   0 suraneti   (501) staff       (20)      657 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     4938 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      194 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     6831 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2324 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      625 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/constants.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.324823 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/
+-rw-r--r--   0 suraneti   (501) staff       (20)   328664 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    28908 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    26897 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    29068 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    54748 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    89890 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 suraneti   (501) staff       (20)   622260 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 suraneti   (501) staff       (20)   983403 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 suraneti   (501) staff       (20)  1158944 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)  1347363 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 suraneti   (501) staff       (20)   119875 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    19886 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    78793 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 suraneti   (501) staff       (20)   136946 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)   288861 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    18975 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    32495 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    39032 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 suraneti   (501) staff       (20)     1862 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 suraneti   (501) staff       (20)     6967 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     7351 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    17165 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 suraneti   (501) staff       (20)     2480 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 suraneti   (501) staff       (20)     2242 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 suraneti   (501) staff       (20)     8293 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 suraneti   (501) staff       (20)    11889 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.349509 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1501 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/admin.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      269 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/filters.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2400 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/forms.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     8445 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/models.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     5740 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.365849 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      547 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     3013 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     7414 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     6203 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      508 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      320 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/django/validators.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.367612 safe-eth-py_suraneti-5.3.0/gnosis/eth/eip712/
+-rw-r--r--   0 suraneti   (501) staff       (20)     6538 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    77421 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    20911 2023-05-03 02:59:40.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1104 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/exceptions.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    13603 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/multicall.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.396613 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/
+-rw-r--r--   0 suraneti   (501) staff       (20)     1093 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.424875 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    15986 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    30036 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    29731 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    27567 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    25872 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      239 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    45208 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    36257 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1464 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2398 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      161 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.428194 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     5856 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     4194 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    32144 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1677 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1520 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     7154 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1064 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.461378 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.476715 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)   107062 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1047 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1246 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1357 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.480071 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/eip712/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    13315 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2725 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.972394 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    31306 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    12057 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 suraneti   (501) staff       (20)   793149 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    92795 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 suraneti   (501) staff       (20)   171076 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:48.990595 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2706 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1820 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1460 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2043 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     3461 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    61046 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     7087 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    21070 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     7380 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     4474 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/utils.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      281 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/typing.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     6399 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/eth/utils.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.000018 safe-eth-py_suraneti-5.3.0/gnosis/protocol/
+-rw-r--r--   0 suraneti   (501) staff       (20)      177 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/protocol/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     8642 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2695 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/protocol/order.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.002198 safe-eth-py_suraneti-5.3.0/gnosis/protocol/tests/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     5926 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/py.typed
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.041527 safe-eth-py_suraneti-5.3.0/gnosis/safe/
+-rw-r--r--   0 suraneti   (501) staff       (20)      716 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    24396 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/addresses.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.060408 safe-eth-py_suraneti-5.3.0/gnosis/safe/api/
+-rw-r--r--   0 suraneti   (501) staff       (20)      346 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/api/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1917 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/api/base_api.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     3062 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     9262 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1451 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/exceptions.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    11385 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/multi_send.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     8070 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    41997 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/safe.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    12116 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    12982 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     9885 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_signature.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    16881 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_tx.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     4181 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/serializers.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     2039 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/signatures.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.107700 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.110461 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/api/
+-rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     4989 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    10808 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    10515 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     6448 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    32608 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    16628 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    16965 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    14117 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 suraneti   (501) staff       (20)    12928 2023-05-03 02:51:41.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     3762 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     3701 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 suraneti   (501) staff       (20)     1967 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.117353 safe-eth-py_suraneti-5.3.0/gnosis/util/
+-rw-r--r--   0 suraneti   (501) staff       (20)       83 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/util/__init__.py
+-rw-r--r--   0 suraneti   (501) staff       (20)      442 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/gnosis/util/util.py
+drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 03:03:49.123054 safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/
+-rw-r--r--   0 suraneti   (501) staff       (20)     6663 2023-05-03 03:03:47.000000 safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/PKG-INFO
+-rw-r--r--   0 suraneti   (501) staff       (20)     5696 2023-05-03 03:03:47.000000 safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/SOURCES.txt
+-rw-r--r--   0 suraneti   (501) staff       (20)        1 2023-05-03 03:03:47.000000 safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/dependency_links.txt
+-rw-r--r--   0 suraneti   (501) staff       (20)      219 2023-05-03 03:03:47.000000 safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/requires.txt
+-rw-r--r--   0 suraneti   (501) staff       (20)        7 2023-05-03 03:03:47.000000 safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/top_level.txt
+-rw-r--r--   0 suraneti   (501) staff       (20)     2523 2023-05-03 03:03:49.124821 safe-eth-py_suraneti-5.3.0/setup.cfg
+-rw-r--r--   0 suraneti   (501) staff       (20)       69 2023-02-03 11:50:27.000000 safe-eth-py_suraneti-5.3.0/setup.py
```

### Comparing `safe-eth-py_suraneti-0.0.2/LICENSE` & `safe-eth-py_suraneti-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/PKG-INFO` & `safe-eth-py_suraneti-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: safe-eth-py_suraneti
-Version: 0.0.2
+Version: 5.3.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
-Home-page: 
+Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
 Project-URL: Tracker, https://github.com/safe-global/safe-eth-py/issues
 Keywords: ethereum,web3,django,safe,cowswap,gnosis
```

### Comparing `safe-eth-py_suraneti-0.0.2/README.rst` & `safe-eth-py_suraneti-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/Makefile` & `safe-eth-py_suraneti-5.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/make.bat` & `safe-eth-py_suraneti-5.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/conf.py` & `safe-eth-py_suraneti-5.3.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 
 sys.path.insert(0, os.path.abspath("../../"))
 
 
 # -- Project information -----------------------------------------------------
 
-project = "Safe-eth-py_suraneti"
+project = "Safe-eth-py"
 copyright = "2018-2021, Uxio"
 author = "Uxio"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.clients.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.django.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/gnosis.eth.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/gnosis.safe.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/index.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/docs/source/quickstart.rst` & `safe-eth-py_suraneti-5.3.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/__init__.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     SenderAccountNotFoundInNode,
     TransactionAlreadyImported,
     TransactionQueueLimitReached,
     TxSpeed,
     UnknownAccount,
 )
 from .ethereum_network import EthereumNetwork, EthereumNetworkNotSupported
-from .exceptions import InvalidERC20Info, InvalidERC721Info, ParityTraceDecodeException
+from .exceptions import InvalidERC20Info, InvalidERC721Info
 
 __all__ = [
     "EthereumClient",
     "EthereumClientProvider",
     "EthereumTxSent",
     "FromAddressNotFound",
     "GasLimitExceeded",
@@ -35,9 +35,8 @@
     "TransactionQueueLimitReached",
     "TxSpeed",
     "UnknownAccount",
     "EthereumNetwork",
     "EthereumNetworkNotSupported",
     "InvalidERC20Info",
     "InvalidERC721Info",
-    "ParityTraceDecodeException",
 ]
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/__init__.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/blockscout_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,53 +15,54 @@
 
 class BlockScoutConfigurationProblem(BlockscoutClientException):
     pass
 
 
 class BlockscoutClient:
     NETWORK_WITH_URL = {
-        EthereumNetwork.XDAI: "https://blockscout.com/poa/xdai/",
-        EthereumNetwork.MATIC: "https://polygon-explorer-mainnet.chainstacklabs.com/",
+        EthereumNetwork.GNOSIS: "https://blockscout.com/poa/xdai/",
+        EthereumNetwork.POLYGON: "https://polygon-explorer-mainnet.chainstacklabs.com/",
         EthereumNetwork.MUMBAI: "https://polygon-explorer-mumbai.chainstacklabs.com/",
         EthereumNetwork.ENERGY_WEB_CHAIN: "https://explorer.energyweb.org/",
-        EthereumNetwork.VOLTA: "https://volta-explorer.energyweb.org/",
-        EthereumNetwork.OLYMPUS: "https://explorer.polis.tech",
-        EthereumNetwork.BOBA_NETWORK_BOBABEAM: "https://blockexplorer.bobabeam.boba.network/",
-        EthereumNetwork.BOBA_RINKEBY: "https://blockexplorer.rinkeby.boba.network/",
-        EthereumNetwork.BOBA: "https://blockexplorer.boba.network/",
-        EthereumNetwork.GATHER_DEVNET: "https://devnet-explorer.gather.network/",
-        EthereumNetwork.GATHER_TESTNET: "https://testnet-explorer.gather.network/",
-        EthereumNetwork.GATHER_MAINNET: "https://explorer.gather.network/",
-        EthereumNetwork.METIS_TESTNET: "https://stardust-explorer.metis.io/",
+        EthereumNetwork.ENERGY_WEB_VOLTA_TESTNET: "https://volta-explorer.energyweb.org/",
+        EthereumNetwork.POLIS_MAINNET: "https://explorer.polis.tech",
+        EthereumNetwork.BOBABEAM: "https://blockexplorer.bobabeam.boba.network/",
+        EthereumNetwork.BOBA_NETWORK_RINKEBY_TESTNET: "https://blockexplorer.rinkeby.boba.network/",
+        EthereumNetwork.BOBA_NETWORK: "https://blockexplorer.boba.network/",
+        EthereumNetwork.GATHER_DEVNET_NETWORK: "https://devnet-explorer.gather.network/",
+        EthereumNetwork.GATHER_TESTNET_NETWORK: "https://testnet-explorer.gather.network/",
+        EthereumNetwork.GATHER_MAINNET_NETWORK: "https://explorer.gather.network/",
+        EthereumNetwork.METIS_STARDUST_TESTNET: "https://stardust-explorer.metis.io/",
         EthereumNetwork.METIS_GOERLI_TESTNET: "https://goerli.explorer.metisdevops.link/",
-        EthereumNetwork.METIS: "https://andromeda-explorer.metis.io/",
+        EthereumNetwork.METIS_ANDROMEDA_MAINNET: "https://andromeda-explorer.metis.io/",
         EthereumNetwork.FUSE_MAINNET: "https://explorer.fuse.io/",
-        EthereumNetwork.VELAS_MAINNET: "https://evmexplorer.velas.com/",
-        EthereumNetwork.REI_MAINNET: "https://scan.rei.network/",
-        EthereumNetwork.REI_TESTNET: "https://scan-test.rei.network/",
-        EthereumNetwork.METER: "https://scan.meter.io/",
+        EthereumNetwork.VELAS_EVM_MAINNET: "https://evmexplorer.velas.com/",
+        EthereumNetwork.REI_NETWORK: "https://scan.rei.network/",
+        EthereumNetwork.REI_CHAIN_TESTNET: "https://scan-test.rei.network/",
+        EthereumNetwork.METER_MAINNET: "https://scan.meter.io/",
         EthereumNetwork.METER_TESTNET: "https://scan-warringstakes.meter.io/",
-        EthereumNetwork.GODWOKEN_TESTNET: "https://v1.betanet.gwscan.com/",
-        EthereumNetwork.GODWOKEN: "https://v1.gwscan.com/",
+        EthereumNetwork.GODWOKEN_TESTNET_V1: "https://v1.betanet.gwscan.com/",
+        EthereumNetwork.GODWOKEN_MAINNET: "https://v1.gwscan.com/",
         EthereumNetwork.VENIDIUM_TESTNET: "https://evm-testnet.venidiumexplorer.com/",
-        EthereumNetwork.VENIDIUM: "https://evm.venidiumexplorer.com/",
-        EthereumNetwork.KLAY_BAOBAB: "https://baobab.scope.klaytn.com/",
-        EthereumNetwork.KLAY_CYPRESS: "https://scope.klaytn.com/",
-        EthereumNetwork.ACA: "https://blockscout.acala.network/",
+        EthereumNetwork.VENIDIUM_MAINNET: "https://evm.venidiumexplorer.com/",
+        EthereumNetwork.KLAYTN_TESTNET_BAOBAB: "https://baobab.scope.klaytn.com/",
+        EthereumNetwork.KLAYTN_MAINNET_CYPRESS: "https://scope.klaytn.com/",
+        EthereumNetwork.ACALA_NETWORK: "https://blockscout.acala.network/",
         EthereumNetwork.KARURA_NETWORK_TESTNET: "https://blockscout.karura.network/",
         EthereumNetwork.ACALA_NETWORK_TESTNET: "https://blockscout.mandala.acala.network/",
         EthereumNetwork.ASTAR: "https://blockscout.com/astar/",
-        EthereumNetwork.EVMOS_MAINNET: "https://evm.evmos.org",
+        EthereumNetwork.EVMOS: "https://evm.evmos.org",
         EthereumNetwork.EVMOS_TESTNET: "https://evm.evmos.dev",
-        EthereumNetwork.RABBIT: "https://rabbit.analogscan.com",
+        EthereumNetwork.RABBIT_ANALOG_TESTNET_CHAIN: "https://rabbit.analogscan.com",
         EthereumNetwork.KCC_MAINNET: "https://scan.kcc.io/",
         EthereumNetwork.KCC_TESTNET: "https://scan-testnet.kcc.network/",
-        EthereumNetwork.ARBITRUM: "https://explorer.arbitrum.io",
+        EthereumNetwork.ARBITRUM_ONE: "https://explorer.arbitrum.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://nova-explorer.arbitrum.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://goerli-rollup-explorer.arbitrum.io",
+        EthereumNetwork.CROSSBELL: "https://scan.crossbell.io",
     }
 
     def __init__(self, network: EthereumNetwork):
         self.network = network
         self.base_url = self.NETWORK_WITH_URL.get(network)
         if self.base_url is None:
             raise BlockScoutConfigurationProblem(
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/etherscan_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,48 +24,54 @@
 class EtherscanClient:
     NETWORK_WITH_URL = {
         EthereumNetwork.MAINNET: "https://etherscan.io",
         EthereumNetwork.RINKEBY: "https://rinkeby.etherscan.io",
         EthereumNetwork.ROPSTEN: "https://ropsten.etherscan.io",
         EthereumNetwork.GOERLI: "https://goerli.etherscan.io",
         EthereumNetwork.KOVAN: "https://kovan.etherscan.io",
-        EthereumNetwork.BINANCE: "https://bscscan.com",
-        EthereumNetwork.MATIC: "https://polygonscan.com",
-        EthereumNetwork.OPTIMISTIC: "https://optimistic.etherscan.io",
-        EthereumNetwork.ARBITRUM: "https://arbiscan.io",
+        EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: "https://bscscan.com",
+        EthereumNetwork.POLYGON: "https://polygonscan.com",
+        EthereumNetwork.POLYGON_ZKEVM: "https://zkevm.polygonscan.com",
+        EthereumNetwork.OPTIMISM: "https://optimistic.etherscan.io",
+        EthereumNetwork.ARBITRUM_ONE: "https://arbiscan.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://nova.arbiscan.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://goerli.arbiscan.io",
-        EthereumNetwork.AVALANCHE: "https://snowtrace.io",
-        EthereumNetwork.MOON_MOONBEAM: "https://moonscan.io",
-        EthereumNetwork.MOON_MOONRIVER: "https://moonriver.moonscan.io",
-        EthereumNetwork.MOON_MOONBASE: "https://moonbase.moonscan.io",
-        EthereumNetwork.CRONOS_MAINNET: "https://cronoscan.com",
+        EthereumNetwork.AVALANCHE_C_CHAIN: "https://snowtrace.io",
+        EthereumNetwork.MOONBEAM: "https://moonscan.io",
+        EthereumNetwork.MOONRIVER: "https://moonriver.moonscan.io",
+        EthereumNetwork.MOONBASE_ALPHA: "https://moonbase.moonscan.io",
+        EthereumNetwork.CRONOS_MAINNET_BETA: "https://cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://testnet.cronoscan.com",
-        EthereumNetwork.CELO: "https://celoscan.io",
+        EthereumNetwork.CELO_MAINNET: "https://celoscan.io",
+        EthereumNetwork.BASE_GOERLI_TESTNET: "https://goerli.basescan.org",
+        EthereumNetwork.NEON_EVM_DEVNET: "https://neonscan.org",
     }
 
     NETWORK_WITH_API_URL = {
         EthereumNetwork.MAINNET: "https://api.etherscan.io",
         EthereumNetwork.RINKEBY: "https://api-rinkeby.etherscan.io",
         EthereumNetwork.ROPSTEN: "https://api-ropsten.etherscan.io",
-        EthereumNetwork.GOERLI: "https://api-goerli.etherscan.io/",
+        EthereumNetwork.GOERLI: "https://api-goerli.etherscan.io",
         EthereumNetwork.KOVAN: "https://api-kovan.etherscan.io",
-        EthereumNetwork.BINANCE: "https://api.bscscan.com",
-        EthereumNetwork.MATIC: "https://api.polygonscan.com",
-        EthereumNetwork.OPTIMISTIC: "https://api-optimistic.etherscan.io",
-        EthereumNetwork.ARBITRUM: "https://api.arbiscan.io",
+        EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: "https://api.bscscan.com",
+        EthereumNetwork.POLYGON: "https://api.polygonscan.com",
+        EthereumNetwork.POLYGON_ZKEVM: "https://api-zkevm.polygonscan.com",
+        EthereumNetwork.OPTIMISM: "https://api-optimistic.etherscan.io",
+        EthereumNetwork.ARBITRUM_ONE: "https://api.arbiscan.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://api-nova.arbiscan.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://api-goerli.arbiscan.io",
-        EthereumNetwork.AVALANCHE: "https://api.snowtrace.io",
-        EthereumNetwork.MOON_MOONBEAM: "https://api-moonbeam.moonscan.io",
-        EthereumNetwork.MOON_MOONRIVER: "https://api-moonriver.moonscan.io",
-        EthereumNetwork.MOON_MOONBASE: "https://api-moonbase.moonscan.io",
-        EthereumNetwork.CRONOS_MAINNET: "https://api.cronoscan.com",
+        EthereumNetwork.AVALANCHE_C_CHAIN: "https://api.snowtrace.io",
+        EthereumNetwork.MOONBEAM: "https://api-moonbeam.moonscan.io",
+        EthereumNetwork.MOONRIVER: "https://api-moonriver.moonscan.io",
+        EthereumNetwork.MOONBASE_ALPHA: "https://api-moonbase.moonscan.io",
+        EthereumNetwork.CRONOS_MAINNET_BETA: "https://api.cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://api-testnet.cronoscan.com",
-        EthereumNetwork.CELO: "https://api.celoscan.io",
+        EthereumNetwork.CELO_MAINNET: "https://api.celoscan.io",
+        EthereumNetwork.BASE_GOERLI_TESTNET: "https://api-goerli.basescan.org",
+        EthereumNetwork.NEON_EVM_DEVNET: "https://devnet-api.neonscan.org",
     }
     HTTP_HEADERS = {
         "User-Agent": "curl/7.77.0",
     }
 
     def __init__(self, network: EthereumNetwork, api_key: Optional[str] = None):
         self.network = network
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/clients/sourcify.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/constants.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/CPKFactory.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/DelegateConstructorProxy.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC1155.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC20.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC20TestToken.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ERC721.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/MultiSend.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/PayingProxy.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/Proxy_V1_0_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/Proxy_V1_1_1.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/Proxy_V1_3_0.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/__init__.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/kyber_network_proxy.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_exchange.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_factory.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_v2_factory.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_v2_pair.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/contracts/uniswap_v2_router.json` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/admin.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/forms.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/models.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/serializers.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/models.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_models.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/eip712/__init__.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/eip712/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Based on https://github.com/jvinet/eip712, adjustments by https://github.com/uxio0
 
 Routines for EIP712 encoding and signing.
 
 Copyright (C) 2022 Judd Vinet <jvinet@zeroflux.org>
+                   Uxío Fuentefría <uxio@safe.global>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
@@ -22,15 +23,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import re
 from typing import Any, Dict, List, Union
 
-from eth_abi import encode_abi
+from eth_abi import encode as encode_abi
 from eth_account import Account
 from eth_typing import Hash32, HexStr
 from hexbytes import HexBytes
 
 from ..utils import fast_keccak
 
 
@@ -71,23 +72,24 @@
 
         if typ == "string":
             # Convert string to bytes.
             value = value.encode("utf-8")
             return ["bytes32", fast_keccak(value)]
 
         if typ.endswith("]"):
-            parsed_type = typ[:-2]
-            type_value_pairs = dict(
-                [_encode_field(name, parsed_type, v) for v in value]
-            )
-            h = fast_keccak(
-                encode_abi(
-                    list(type_value_pairs.keys()), list(type_value_pairs.values())
-                )
-            )
+            # Array type
+            if value:
+                parsed_type = typ[: typ.rindex("[")]
+                type_value_pairs = [_encode_field(name, parsed_type, v) for v in value]
+                data_types, data_hashes = zip(*type_value_pairs)
+            else:
+                # Empty array
+                data_types, data_hashes = [], []
+
+            h = fast_keccak(encode_abi(data_types, data_hashes))
             return ["bytes32", h]
 
         return [typ, value]
 
     for field in types[primary_type]:
         typ, val = _encode_field(field["name"], field["type"], data[field["name"]])
         encoded_types.append(typ)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/ethereum_client.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/ethereum_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,35 +23,34 @@
 from eth_typing import URI, BlockNumber, ChecksumAddress, Hash32, HexStr
 from hexbytes import HexBytes
 from web3 import HTTPProvider, Web3
 from web3._utils.abi import map_abi_data
 from web3._utils.method_formatters import (
     block_formatter,
     receipt_formatter,
+    trace_list_result_formatter,
     transaction_result_formatter,
 )
 from web3._utils.normalizers import BASE_RETURN_NORMALIZERS
-from web3.contract import ContractFunction
-from web3.datastructures import AttributeDict
+from web3.contract.contract import ContractFunction
 from web3.exceptions import (
-    BadFunctionCallOutput,
     BlockNotFound,
     TimeExhausted,
     TransactionNotFound,
+    Web3Exception,
 )
 from web3.middleware import geth_poa_middleware, simple_cache_middleware
 from web3.types import (
     BlockData,
     BlockIdentifier,
+    BlockTrace,
     FilterParams,
+    FilterTrace,
     LogReceipt,
     Nonce,
-    ParityBlockTrace,
-    ParityFilterParams,
-    ParityFilterTrace,
     TxData,
     TxParams,
     TxReceipt,
     Wei,
 )
 
 from gnosis.eth.utils import (
@@ -76,15 +75,14 @@
     GasLimitExceeded,
     InsufficientFunds,
     InvalidERC20Info,
     InvalidERC721Info,
     InvalidNonce,
     NonceTooHigh,
     NonceTooLow,
-    ParityTraceDecodeException,
     ReplacementTransactionUnderpriced,
     SenderAccountNotFoundInNode,
     TransactionAlreadyImported,
     TransactionGasPriceTooLow,
     TransactionQueueLimitReached,
     UnknownAccount,
 )
@@ -92,15 +90,15 @@
 from .utils import decode_string_or_bytes32
 
 logger = getLogger(__name__)
 
 
 def tx_with_exception_handling(func):
     """
-    Parity
+    Parity / OpenEthereum
         - https://github.com/openethereum/openethereum/blob/main/rpc/src/v1/helpers/errors.rs
     Geth
         - https://github.com/ethereum/go-ethereum/blob/master/core/error.go
         - https://github.com/ethereum/go-ethereum/blob/master/core/tx_pool.go
     Comparison
         - https://gist.github.com/kunal365roy/3c37ac9d1c3aaf31140f7c5faa083932
 
@@ -129,15 +127,15 @@
         "exceeds current gas limit": GasLimitExceeded,  # https://github.com/openethereum/openethereum/blob/f1dc6821689c7f47d8fd07dfc0a2c5ad557b98ec/crates/rpc/src/v1/helpers/errors.rs#L392
     }
 
     @wraps(func)
     def with_exception_handling(*args, **kwargs):
         try:
             return func(*args, **kwargs)
-        except ValueError as exc:
+        except (Web3Exception, ValueError) as exc:
             str_exc = str(exc).lower()
             for reason, custom_exception in error_with_exception.items():
                 if reason.lower() in str_exc:
                     raise custom_exception(str(exc)) from exc
             raise exc
 
     return with_exception_handling
@@ -286,15 +284,15 @@
             if "error" in result:
                 fn_name = payload.get("fn_name", HexBytes(payload["data"]).hex())
                 errors.append(f'`{fn_name}`: {result["error"]}')
                 return_values.append(None)
             else:
                 output_type = payload["output_type"]
                 try:
-                    decoded_values = self.w3.codec.decode_abi(
+                    decoded_values = eth_abi.decode(
                         output_type, HexBytes(result["result"])
                     )
                     normalized_data = map_abi_data(
                         BASE_RETURN_NORMALIZERS, output_type, decoded_values
                     )
                     if len(normalized_data) == 1:
                         return_values.append(normalized_data[0])
@@ -426,49 +424,49 @@
         self, data: EthereumData, topics: Sequence[bytes]
     ) -> Optional[Dict[str, Any]]:
         topics_len = len(topics)
         if topics_len and topics[0] == self.TRANSFER_TOPIC:
             if topics_len == 1:
                 # Not standard Transfer(address from, address to, uint256 unknown)
                 # 1 topic (transfer topic)
-                _from, to, unknown = eth_abi.decode_abi(
+                _from, to, unknown = eth_abi.decode(
                     ["address", "address", "uint256"], HexBytes(data)
                 )
                 return {"from": _from, "to": to, "unknown": unknown}
             elif topics_len == 3:
                 # ERC20 Transfer(address indexed from, address indexed to, uint256 value)
                 # 3 topics (transfer topic + from + to)
                 try:
                     value_data = HexBytes(data)
-                    value = eth_abi.decode_single("uint256", value_data)
+                    value = eth_abi.decode(["uint256"], value_data)[0]
                 except DecodingError:
                     logger.warning(
                         "Cannot decode Transfer event `uint256 value` from data=%s",
                         value_data.hex(),
                     )
                     return None
                 try:
                     from_to_data = b"".join(topics[1:])
                     _from, to = (
                         fast_to_checksum_address(address)
-                        for address in eth_abi.decode_abi(
+                        for address in eth_abi.decode(
                             ["address", "address"], from_to_data
                         )
                     )
                 except DecodingError:
                     logger.warning(
                         "Cannot decode Transfer event `address from, address to` from topics=%s",
                         HexBytes(from_to_data).hex(),
                     )
                     return None
                 return {"from": _from, "to": to, "value": value}
             elif topics_len == 4:
                 # ERC712 Transfer(address indexed from, address indexed to, uint256 indexed tokenId)
                 # 4 topics (transfer topic + from + to + tokenId)
-                _from, to, token_id = eth_abi.decode_abi(
+                _from, to, token_id = eth_abi.decode(
                     ["address", "address", "uint256"], b"".join(topics[1:])
                 )
                 _from, to = [
                     fast_to_checksum_address(address) for address in (_from, to)
                 ]
                 return {"from": _from, "to": to, "tokenId": token_id}
         return None
@@ -581,17 +579,17 @@
             response_json = sorted(response.json(), key=lambda x: x["id"])
             errors = [r["error"] for r in response_json if "error" in r]
             if errors:
                 raise InvalidERC20Info(f"{erc20_address} - {errors}")
             results = [HexBytes(r["result"]) for r in response_json]
             name = decode_string_or_bytes32(results[0])
             symbol = decode_string_or_bytes32(results[1])
-            decimals = self.ethereum_client.w3.codec.decode_single("uint8", results[2])
+            decimals = eth_abi.decode(["uint8"], results[2])[0]
             return Erc20Info(name, symbol, decimals)
-        except (ValueError, BadFunctionCallOutput, DecodingError) as e:
+        except (Web3Exception, DecodingError, ValueError) as e:
             raise InvalidERC20Info from e
 
     def get_total_transfer_history(
         self,
         addresses: Optional[Sequence[ChecksumAddress]] = None,
         from_block: BlockIdentifier = BlockNumber(0),
         to_block: Optional[BlockIdentifier] = None,
@@ -666,15 +664,15 @@
         :param to_block: Block to stop querying from
         :param token_address: Address of the token
         :return: List of events sorted by blockNumber
         """
         topic_0 = self.TRANSFER_TOPIC.hex()
         if addresses:
             addresses_encoded = [
-                HexBytes(eth_abi.encode_single("address", address)).hex()
+                HexBytes(eth_abi.encode(["address"], [address])).hex()
                 for address in addresses
             ]
             # Topics for transfer `to` and `from` an address
             all_topics = [
                 [topic_0, addresses_encoded],  # Topics from
                 [topic_0, None, addresses_encoded],  # Topics to
             ]
@@ -748,15 +746,15 @@
 
         argument_filters = {}
         if from_address:
             argument_filters["from"] = from_address
         if to_address:
             argument_filters["to"] = to_address
 
-        return erc20.events.Transfer.createFilter(
+        return erc20.events.Transfer.create_filter(
             fromBlock=from_block,
             toBlock=to_block,
             address=token_address,
             argument_filters=argument_filters,
         ).get_all_entries()
 
     def send_tokens(
@@ -898,87 +896,15 @@
                     for token_address, token_id in token_addresses_with_token_ids
                 ],
                 raise_exception=False,
             )
         ]
 
 
-class ParityManager(EthereumClientManager):
-    # TODO Test with mock
-    def _decode_trace_action(self, action: Dict[str, Any]) -> Dict[str, Any]:
-        decoded = {}
-
-        # CALL, DELEGATECALL, CREATE or CREATE2
-        if "from" in action:
-            decoded["from"] = fast_to_checksum_address(action["from"])
-        if "gas" in action:
-            decoded["gas"] = int(action["gas"], 16)
-        if "value" in action:
-            decoded["value"] = int(action["value"], 16)
-
-        # CALL or DELEGATECALL
-        if "callType" in action:
-            decoded["callType"] = action["callType"]
-        if "input" in action:
-            decoded["input"] = HexBytes(action["input"])
-        if "to" in action:
-            decoded["to"] = fast_to_checksum_address(action["to"])
-
-        # CREATE or CREATE2
-        if "init" in action:
-            decoded["init"] = HexBytes(action["init"])
-
-        # SELF-DESTRUCT
-        if "address" in action:
-            decoded["address"] = fast_to_checksum_address(action["address"])
-        if "balance" in action:
-            decoded["balance"] = int(action["balance"], 16)
-        if "refundAddress" in action:
-            decoded["refundAddress"] = fast_to_checksum_address(action["refundAddress"])
-
-        return decoded
-
-    def _decode_trace_result(self, result: Dict[str, Any]) -> Dict[str, Any]:
-        decoded: Dict[str, Any] = {
-            "gasUsed": int(result["gasUsed"], 16),
-        }
-
-        # CALL or DELEGATECALL
-        if "output" in result:
-            decoded["output"] = HexBytes(result["output"])
-
-        # CREATE or CREATE2
-        if "code" in result:
-            decoded["code"] = HexBytes(result["code"])
-        if "address" in result:
-            decoded["address"] = fast_to_checksum_address(result["address"])
-
-        return decoded
-
-    def _decode_traces(
-        self, traces: Sequence[Union[ParityBlockTrace, ParityFilterTrace]]
-    ) -> List[Dict[str, Any]]:
-        new_traces: List[Dict[str, Any]] = []
-        for trace in traces:
-            if isinstance(trace, dict):
-                trace_copy = trace.copy()
-            elif isinstance(trace, AttributeDict):
-                trace_copy = trace.__dict__.copy()
-            else:
-                raise ParityTraceDecodeException(
-                    "Expected dictionary, but found unexpected trace %s" % trace
-                )
-            new_traces.append(trace_copy)
-            # Txs with `error` field don't have `result` field
-            # Txs with `type=suicide` have `result` field but is `None`
-            if "result" in trace and trace["result"]:
-                trace_copy["result"] = self._decode_trace_result(trace["result"])
-            trace_copy["action"] = self._decode_trace_action(trace["action"])
-        return new_traces
-
+class TracingManager(EthereumClientManager):
     def filter_out_errored_traces(
         self, internal_txs: Sequence[Dict[str, Any]]
     ) -> Sequence[Dict[str, Any]]:
         """
         Filter out errored transactions (traces that are errored or that have an errored parent)
 
         :param internal_txs: Traces for the SAME ethereum tx, sorted ascending by `trace_address`
@@ -1060,24 +986,16 @@
                     pass
                 elif remove_calls and trace["action"].get("callType") == "call":
                     pass
                 else:
                     traces.append(trace)
         return traces
 
-    def trace_block(self, block_identifier: BlockIdentifier) -> List[Dict[str, Any]]:
-        try:
-            return self._decode_traces(
-                self.slow_w3.parity.trace_block(block_identifier)
-            )
-        except ParityTraceDecodeException as exc:
-            logger.warning("Problem decoding trace: %s - Retrying", exc)
-            return self._decode_traces(
-                self.slow_w3.parity.trace_block(block_identifier)
-            )
+    def trace_block(self, block_identifier: BlockIdentifier) -> List[BlockTrace]:
+        return self.slow_w3.tracing.trace_block(block_identifier)
 
     def trace_blocks(
         self, block_identifiers: List[BlockIdentifier]
     ) -> List[List[Dict[str, Any]]]:
         if not block_identifiers:
             return []
         payload = [
@@ -1091,41 +1009,26 @@
                     else block_identifier
                 ],
             }
             for i, block_identifier in enumerate(block_identifiers)
         ]
 
         results = self.ethereum_client.raw_batch_request(payload)
-        traces = []
-        for raw_tx in results:
-            if raw_tx:
-                try:
-                    decoded_traces = self._decode_traces(raw_tx)
-                except ParityTraceDecodeException as exc:
-                    logger.warning("Problem decoding trace: %s - Retrying", exc)
-                    decoded_traces = self._decode_traces(raw_tx)
-                traces.append(decoded_traces)
-            else:
-                traces.append([])
-        return traces
+        return [trace_list_result_formatter(block_traces) for block_traces in results]
 
-    def trace_transaction(self, tx_hash: EthereumHash) -> List[Dict[str, Any]]:
+    def trace_transaction(self, tx_hash: EthereumHash) -> List[FilterTrace]:
         """
         :param tx_hash:
         :return: List of internal txs for `tx_hash`
         """
-        try:
-            return self._decode_traces(self.slow_w3.parity.trace_transaction(tx_hash))
-        except ParityTraceDecodeException as exc:
-            logger.warning("Problem decoding trace: %s - Retrying", exc)
-            return self._decode_traces(self.slow_w3.parity.trace_transaction(tx_hash))
+        return self.slow_w3.tracing.trace_transaction(tx_hash)
 
     def trace_transactions(
         self, tx_hashes: Sequence[EthereumHash]
-    ) -> List[List[Dict[str, Any]]]:
+    ) -> List[List[FilterTrace]]:
         """
         :param tx_hashes:
         :return: For every `tx_hash` a list of internal txs (in the same order as the `tx_hashes` were provided)
         """
         if not tx_hashes:
             return []
         payload = [
@@ -1134,36 +1037,25 @@
                 "jsonrpc": "2.0",
                 "method": "trace_transaction",
                 "params": [HexBytes(tx_hash).hex()],
             }
             for i, tx_hash in enumerate(tx_hashes)
         ]
         results = self.ethereum_client.raw_batch_request(payload)
-        traces = []
-        for raw_tx in results:
-            if raw_tx:
-                try:
-                    decoded_traces = self._decode_traces(raw_tx)
-                except ParityTraceDecodeException as exc:
-                    logger.warning("Problem decoding trace: %s - Retrying", exc)
-                    decoded_traces = self._decode_traces(raw_tx)
-                traces.append(decoded_traces)
-            else:
-                traces.append([])
-        return traces
+        return [trace_list_result_formatter(tx_traces) for tx_traces in results]
 
     def trace_filter(
         self,
         from_block: int = 1,
         to_block: Optional[int] = None,
         from_address: Optional[Sequence[ChecksumAddress]] = None,
         to_address: Optional[Sequence[ChecksumAddress]] = None,
         after: Optional[int] = None,
         count: Optional[int] = None,
-    ) -> List[Dict[str, Any]]:
+    ) -> List[FilterTrace]:
         """
         Get events using ``trace_filter`` method
 
         :param from_block: Quantity or Tag - (optional) From this block. `0` is not working, it needs to be `>= 1`
         :param to_block: Quantity or Tag - (optional) To this block.
         :param from_address: Array - (optional) Sent from these addresses.
         :param to_address: Address - (optional) Sent to these addresses.
@@ -1232,33 +1124,29 @@
                 }
             ]
 
         """
         assert (
             from_address or to_address
         ), "You must provide at least `from_address` or `to_address`"
-        parameters: ParityFilterParams = {}
+        parameters: FilterParams = {}
         if after:
             parameters["after"] = after
         if count:
             parameters["count"] = count
         if from_block:
             parameters["fromBlock"] = HexStr("0x%x" % from_block)
         if to_block:
             parameters["toBlock"] = HexStr("0x%x" % to_block)
         if from_address:
             parameters["fromAddress"] = from_address
         if to_address:
             parameters["toAddress"] = to_address
 
-        try:
-            return self._decode_traces(self.slow_w3.parity.trace_filter(parameters))
-        except ParityTraceDecodeException as exc:
-            logger.warning("Problem decoding trace: %s - Retrying", exc)
-            return self._decode_traces(self.slow_w3.parity.trace_filter(parameters))
+        return self.slow_w3.tracing.trace_filter(parameters)
 
 
 class EthereumClient:
     """
     Manage ethereum operations. Uses web3 for the most part, but some other stuff is implemented from scratch.
     Note: If you want to use `pending` state with `Parity`, it must be run with `--pruning=archive` or `--force-sealing`
     """
@@ -1296,15 +1184,15 @@
             request_kwargs={"timeout": slow_provider_timeout},
             session=self.http_session,
         )
         self.w3: Web3 = Web3(self.w3_provider)
         self.slow_w3: Web3 = Web3(self.w3_slow_provider)
         self.erc20: Erc20Manager = Erc20Manager(self)
         self.erc721: Erc721Manager = Erc721Manager(self)
-        self.parity: ParityManager = ParityManager(self)
+        self.tracing: TracingManager = TracingManager(self)
         self.batch_call_manager: BatchCallManager = BatchCallManager(self)
         try:
             if self.get_network() != EthereumNetwork.MAINNET:
                 self.w3.middleware_onion.inject(geth_poa_middleware, layer=0)
             # For tests using dummy connections (like IPC)
         except (IOError, FileNotFoundError):
             self.w3.middleware_onion.inject(geth_poa_middleware, layer=0)
@@ -1403,30 +1291,31 @@
         """
         :return: RPC version information
         """
         return self.w3.clientVersion
 
     def get_network(self) -> EthereumNetwork:
         """
-        Get network name based on the chainId
+        Get network name based on the chainId. This method is not cached as the method for getting the
+        `chainId` already is.
 
         :return: EthereumNetwork based on the chainId. If network is not
-            on our list, `EthereumNetwork.UNKOWN` is returned
+            on our list, `EthereumNetwork.UNKNOWN` is returned
         """
         return EthereumNetwork(self.get_chain_id())
 
     @cache
     def is_eip1559_supported(self) -> EthereumNetwork:
         """
         :return: `True` if EIP1559 is supported by the node, `False` otherwise
         """
         try:
             self.w3.eth.fee_history(1, "latest", reward_percentiles=[50])
             return True
-        except ValueError:
+        except (Web3Exception, ValueError):
             return False
 
     @cached_property
     def multicall(self) -> "Multicall":  # noqa F821
         from .multicall import Multicall
 
         try:
@@ -1529,14 +1418,15 @@
             if data:
                 tx: TxParams = {
                     "from": deployer_account.address,
                     "data": data,
                     "gasPrice": self.w3.eth.gas_price,
                     "value": Wei(0),
                     "to": contract_address if contract_address else "",
+                    "chainId": self.get_chain_id(),
                 }
                 tx["gas"] = self.w3.eth.estimate_gas(tx)
                 tx_hash = self.send_unsigned_transaction(
                     tx, private_key=deployer_account.key
                 )
                 if check_receipt:
                     tx_receipt = self.get_transaction_receipt(
@@ -1601,15 +1491,15 @@
             tx["data"] = data
         if gas:
             tx["gas"] = gas
         if gas_price:
             tx["gasPrice"] = gas_price
         try:
             return self.w3.eth.estimate_gas(tx, block_identifier=block_identifier)
-        except ValueError:
+        except (Web3Exception, ValueError):
             if (
                 block_identifier is not None
             ):  # Geth does not support setting `block_identifier`
                 return self.w3.eth.estimate_gas(tx, block_identifier=None)
             else:
                 raise
 
@@ -1938,14 +1828,15 @@
 
         tx: TxParams = {
             "from": account.address,
             "to": to,
             "value": value,
             "gas": gas or Wei(self.estimate_gas(to, account.address, value)),
             "gasPrice": Wei(gas_price),
+            "chainId": self.get_chain_id(),
         }
 
         if nonce is not None:
             tx["nonce"] = Nonce(nonce)
 
         return self.send_unsigned_transaction(
             tx, private_key=private_key, retry=retry, block_identifier=block_identifier
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/exceptions.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,18 +50,14 @@
     pass
 
 
 class TransactionGasPriceTooLow(EthereumClientException):
     pass
 
 
-class ParityTraceDecodeException(EthereumClientException):
-    pass
-
-
 class InvalidERC20Info(EthereumClientException):
     pass
 
 
 class InvalidERC721Info(EthereumClientException):
     pass
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/__init__.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/cowswap.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/cowswap.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,13 +66,13 @@
                 )
 
             exception = None
         except IOError as exc:
             exception = exc
             result = {}
 
-        error_message = (
+        message = (
             f"Cannot get price from CowSwap {result} "
             f"for token-1={token_address_1} to token-2={token_address_2}"
         )
-        logger.warning(error_message)
-        raise CannotGetPriceFromOracle(error_message) from exception
+        logger.debug(message)
+        raise CannotGetPriceFromOracle(message) from exception
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/kyber.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/kyber.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from functools import cached_property
 from typing import Optional
 
 from eth_abi.exceptions import DecodingError
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import Web3Exception
 
 from .. import EthereumClient, EthereumNetwork
 from ..contracts import get_kyber_network_proxy_contract
 from .exceptions import CannotGetPriceFromOracle, InvalidPriceFromOracle
 from .oracles import PriceOracle
 from .utils import get_decimals
 
@@ -94,21 +94,21 @@
                     _,
                 ) = self.kyber_network_proxy_contract.functions.getExpectedRate(
                     token_address_2, token_address_1, int(token_unit)
                 ).call()
                 price = (token_unit / expected_rate) if expected_rate else 0
 
             if price <= 0.0:
-                error_message = (
+                message = (
                     f"price={price} <= 0 from kyber-network-proxy={self.kyber_network_proxy_address} "
                     f"for token-1={token_address_1} to token-2={token_address_2}"
                 )
-                logger.warning(error_message)
-                raise InvalidPriceFromOracle(error_message)
+                logger.debug(message)
+                raise InvalidPriceFromOracle(message)
             return price
-        except (ValueError, BadFunctionCallOutput, DecodingError) as e:
-            error_message = (
+        except (Web3Exception, DecodingError, ValueError) as e:
+            message = (
                 f"Cannot get price from kyber-network-proxy={self.kyber_network_proxy_address} "
                 f"for token-1={token_address_1} to token-2={token_address_2}"
             )
-            logger.warning(error_message)
-            raise CannotGetPriceFromOracle(error_message) from e
+            logger.debug(message)
+            raise CannotGetPriceFromOracle(message) from e
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/oracles.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/oracles.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from functools import cached_property
 from typing import List, Optional, Tuple
 
 import requests
+from eth_abi import decode as decode_abi
 from eth_abi.exceptions import DecodingError
-from eth_abi.packed import encode_abi_packed
+from eth_abi.packed import encode_packed
 from eth_typing import ChecksumAddress
 from hexbytes import HexBytes
 from web3.contract import Contract
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import Web3Exception
 
 from .. import EthereumClient, EthereumNetwork
 from ..constants import NULL_ADDRESS
 from ..contracts import (
     get_erc20_contract,
     get_uniswap_factory_contract,
     get_uniswap_v2_factory_contract,
@@ -176,60 +177,56 @@
         for result in r.json():
             if "result" not in result:
                 raise CannotGetPriceFromOracle(result["error"])
             else:
                 results.append(HexBytes(result["result"]))
 
         balance = int(results[0].hex(), 16)
-        token_decimals = self.ethereum_client.w3.codec.decode_single(
-            "uint8", results[1]
-        )
-        token_balance = self.ethereum_client.w3.codec.decode_single(
-            "uint256", results[2]
-        )
+        token_decimals = decode_abi(["uint8"], results[1])[0]
+        token_balance = decode_abi(["uint256"], results[2])[0]
         return balance, token_decimals, token_balance
 
     def get_price(self, token_address: str) -> float:
         try:
             uniswap_exchange_address = self.get_uniswap_exchange(token_address)
             if uniswap_exchange_address == NULL_ADDRESS:
                 raise ValueError
-        except (ValueError, BadFunctionCallOutput, DecodingError) as e:
-            error_message = f"Non existing uniswap exchange for token={token_address}"
-            logger.warning(error_message)
-            raise CannotGetPriceFromOracle(error_message) from e
+        except (Web3Exception, DecodingError, ValueError) as e:
+            message = f"Non existing uniswap exchange for token={token_address}"
+            logger.debug(message)
+            raise CannotGetPriceFromOracle(message) from e
 
         try:
             balance, token_decimals, token_balance = self._get_balances_using_batching(
                 uniswap_exchange_address, token_address
             )
             # Check liquidity. Require at least 2 ether to be on the pool
             if balance / 1e18 < 2:
                 raise CannotGetPriceFromOracle(
                     f"Not enough liquidity for token={token_address}"
                 )
 
             price = balance / token_balance / 10 ** (18 - token_decimals)
             if price <= 0.0:
-                error_message = (
+                message = (
                     f"price={price} <= 0 from uniswap-factory={uniswap_exchange_address} "
                     f"for token={token_address}"
                 )
-                logger.warning(error_message)
-                raise InvalidPriceFromOracle(error_message)
+                logger.debug(message)
+                raise InvalidPriceFromOracle(message)
             return price
         except (
+            Web3Exception,
+            DecodingError,
             ValueError,
             ZeroDivisionError,
-            BadFunctionCallOutput,
-            DecodingError,
         ) as e:
-            error_message = f"Cannot get token balance for token={token_address}"
-            logger.warning(error_message)
-            raise CannotGetPriceFromOracle(error_message) from e
+            message = f"Cannot get token balance for token={token_address}"
+            logger.debug(message)
+            raise CannotGetPriceFromOracle(message) from e
 
 
 class UniswapV2Oracle(PricePoolOracle, PriceOracle):
     ROUTER_ADDRESSES = {
         EthereumNetwork.MAINNET: "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D",
     }
 
@@ -277,23 +274,23 @@
             self.ethereum_client.w3, self.factory_address
         )
 
     @cached_property
     def factory_address(self) -> str:
         """
         :return: Uniswap factory checksummed address
-        :raises: BadFunctionCallOutput: If router contract is not deployed
+        :raises: Web3Exception: If router contract is not deployed
         """
         return self.router.functions.factory().call()
 
     @cached_property
     def weth_address(self) -> str:
         """
         :return: Wrapped ether checksummed address
-        :raises: BadFunctionCallOutput: If router contract is not deployed
+        :raises: Web3Exception: If router contract is not deployed
         """
         return self.router.functions.WETH().call()
 
     @functools.lru_cache(maxsize=2048)
     def get_pair_address(
         self, token_address: str, token_address_2: str
     ) -> Optional[str]:
@@ -323,18 +320,18 @@
         :param token_address:
         :param token_address_2:
         :return: Checksummed address for token pair. It could be not created yet
         """
         if token_address.lower() > token_address_2.lower():
             token_address, token_address_2 = token_address_2, token_address
         salt = fast_keccak(
-            encode_abi_packed(["address", "address"], [token_address, token_address_2])
+            encode_packed(["address", "address"], [token_address, token_address_2])
         )
         address = fast_keccak(
-            encode_abi_packed(
+            encode_packed(
                 ["bytes", "address", "bytes", "bytes"],
                 [HexBytes("ff"), self.factory_address, salt, self.PAIR_INIT_CODE],
             )
         )[-20:]
         return fast_bytes_to_checksum_address(address)
 
     def get_reserves(self, pair_address: str) -> Tuple[int, int]:
@@ -382,25 +379,25 @@
                     f"token_2={token_address_2}"
                 )
             decimals_normalized_reserves_1 = reserves_1 * 10**decimals_2
             decimals_normalized_reserves_2 = reserves_2 * 10**decimals_1
 
             return decimals_normalized_reserves_2 / decimals_normalized_reserves_1
         except (
+            Web3Exception,
+            DecodingError,
             ValueError,
             ZeroDivisionError,
-            BadFunctionCallOutput,
-            DecodingError,
         ) as e:
-            error_message = (
+            message = (
                 f"Cannot get uniswap v2 price for pair token_1={token_address} "
                 f"token_2={token_address_2}"
             )
-            logger.warning(error_message)
-            raise CannotGetPriceFromOracle(error_message) from e
+            logger.debug(message)
+            raise CannotGetPriceFromOracle(message) from e
 
     def get_price_without_exception(
         self, token_address: str, token_address_2: Optional[str] = None
     ) -> float:
         """
         :param token_address:
         :param token_address_2:
@@ -449,24 +446,22 @@
                 try:
                     price = self.get_price(token_address)
                     total_value = (reserves / 10**decimals_1) * price
                     return (total_value * 2) / (total_supply / 1e18)
                 except CannotGetPriceFromOracle:
                     continue
         except (
+            Web3Exception,
+            DecodingError,
             ValueError,
             ZeroDivisionError,
-            BadFunctionCallOutput,
-            DecodingError,
         ) as e:
-            error_message = (
-                f"Cannot get uniswap v2 price for pool token={pool_token_address}"
-            )
-            logger.warning(error_message)
-            raise CannotGetPriceFromOracle(error_message) from e
+            message = f"Cannot get uniswap v2 price for pool token={pool_token_address}"
+            logger.debug(message)
+            raise CannotGetPriceFromOracle(message) from e
 
 
 class AaveOracle(PriceOracle):
     def __init__(self, ethereum_client: EthereumClient, price_oracle: PriceOracle):
         """
         :param ethereum_client:
         :param price_oracle: Price oracle to get the price for the components of Aave Tokens, UniswapV2 is
@@ -497,15 +492,15 @@
         try:
             underlying_token = (
                 self.w3.eth.contract(token_address, abi=AAVE_ATOKEN_ABI)
                 .functions.UNDERLYING_ASSET_ADDRESS()
                 .call()
             )
             return self.price_oracle.get_price(underlying_token)
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (Web3Exception, DecodingError, ValueError):
             raise CannotGetPriceFromOracle(
                 f"Cannot get price for {token_address}. It is not an Aaave atoken"
             )
 
 
 class CreamOracle(PriceOracle):
     def __init__(self, ethereum_client: EthereumClient, price_oracle: PriceOracle):
@@ -533,15 +528,15 @@
         try:
             underlying_token = (
                 self.w3.eth.contract(token_address, abi=cream_ctoken_abi)
                 .functions.underlying()
                 .call()
             )
             return self.price_oracle.get_price(underlying_token)
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (Web3Exception, DecodingError, ValueError):
             raise CannotGetPriceFromOracle(
                 f"Cannot get price for {token_address}. It is not a Cream cToken"
             )
 
 
 class ZerionComposedOracle(ComposedPriceOracle):
     ZERION_ADAPTER_ADDRESS = None
@@ -615,15 +610,15 @@
                         if len(results) == 1
                         else quantity / 10 ** len(str(quantity))
                     )
                     underlying_tokens.append(
                         UnderlyingToken(token_address, normalized_quantity)
                     )
                 return underlying_tokens
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (ValueError, Web3Exception, DecodingError):
             pass
 
         raise CannotGetPriceFromOracle(
             f"{self.__class__.__name__}: Cannot get price for {token_address}. It is not a Zerion supported pool token"
         )
 
 
@@ -799,15 +794,15 @@
             ]
             total_eth_value = 0
             for token_balance, token_decimal, token_price in zip(
                 token_balances, token_decimals, token_prices
             ):
                 total_eth_value += (token_balance / 10**token_decimal) * token_price
             return total_eth_value / (total_supply / 1e18)
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (Web3Exception, DecodingError, ValueError):
             raise CannotGetPriceFromOracle(
                 f"Cannot get price for {pool_token_address}. "
                 f"It is not a balancer pool token"
             )
 
 
 class MooniswapOracle(BalancerOracle):
@@ -853,12 +848,12 @@
                         continue
 
                 raise CannotGetPriceFromOracle(
                     f"Cannot get price for {pool_token_address}. "
                     f"It is not a mooniswap pool token"
                 )
 
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (Web3Exception, DecodingError, ValueError):
             raise CannotGetPriceFromOracle(
                 f"Cannot get price for {pool_token_address}. "
                 f"It is not a mooniswap pool token"
             )
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/superfluid.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/superfluid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from eth_abi.exceptions import DecodingError
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import Web3Exception
 
 from .. import EthereumClient, EthereumNetwork
 from .abis.superfluid_abis import super_token_abi
 from .exceptions import CannotGetPriceFromOracle
 from .oracles import PriceOracle
 
 
@@ -23,25 +23,25 @@
         ethereum_client: EthereumClient,
     ) -> bool:
         """
         :param ethereum_client:
         :return: `True` if Oracle is available for the EthereumClient provided, `False` otherwise
         """
         return ethereum_client.get_network() in (
-            EthereumNetwork.MATIC,
-            EthereumNetwork.XDAI,
-            EthereumNetwork.ARBITRUM,
-            EthereumNetwork.OPTIMISTIC,
+            EthereumNetwork.POLYGON,
+            EthereumNetwork.GNOSIS,
+            EthereumNetwork.ARBITRUM_ONE,
+            EthereumNetwork.OPTIMISM,
         )
 
     def get_price(self, token_address: str) -> float:
         try:
             underlying_token = (
                 self.w3.eth.contract(token_address, abi=super_token_abi)
                 .functions.getUnderlyingToken()
                 .call()
             )
             return self.price_oracle.get_price(underlying_token)
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (Web3Exception, DecodingError, ValueError):
             raise CannotGetPriceFromOracle(
                 f"Cannot get price for {token_address}. It is not a wrapper Super Token"
             )
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/sushiswap.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 class SushiswapOracle(UniswapV2Oracle):
     PAIR_INIT_CODE = HexBytes(
         "0xe18a34eb0e04b04f7a0ac29a6e80748dca96319b42c54d679cb821dca90c6303"
     )
     ROUTER_ADDRESSES = {
         EthereumNetwork.MAINNET: "0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F",
-        EthereumNetwork.MATIC: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.ARBITRUM: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.AVALANCHE: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.MOON_MOONRIVER: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.FANTOM: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.BINANCE: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.XDAI: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.CELO: "0x1421bDe4B10e8dd459b3BCb598810B1337D56842",
+        EthereumNetwork.POLYGON: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.ARBITRUM_ONE: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.AVALANCHE_C_CHAIN: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.MOONRIVER: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.FANTOM_OPERA: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.GNOSIS: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.CELO_MAINNET: "0x1421bDe4B10e8dd459b3BCb598810B1337D56842",
         EthereumNetwork.FUSE_MAINNET: "0xF4d73326C13a4Fc5FD7A064217e12780e9Bd62c3",
-        EthereumNetwork.OKEXCHAIN: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.OKXCHAIN_MAINNET: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
         EthereumNetwork.PALM: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.MOON_MOONBEAM: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
-        EthereumNetwork.HECO: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.MOONBEAM: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
+        EthereumNetwork.HUOBI_ECO_CHAIN_MAINNET: "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506",
     }
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/oracles/uniswap_v3.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from functools import cached_property
 from typing import Optional
 
 from eth_abi.exceptions import DecodingError
 from eth_typing import ChecksumAddress
 from web3.contract import Contract
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import Web3Exception
 
-from .. import EthereumClient
+from .. import EthereumClient, EthereumNetwork
 from ..constants import NULL_ADDRESS
 from ..contracts import get_erc20_contract
 from .abis.uniswap_v3 import (
     uniswap_v3_factory_abi,
     uniswap_v3_pool_abi,
     uniswap_v3_router_abi,
 )
@@ -21,57 +21,66 @@
 from .utils import get_decimals
 
 logger = logging.getLogger(__name__)
 
 
 class UniswapV3Oracle(PriceOracle):
     # https://docs.uniswap.org/protocol/reference/deployments
-    UNISWAP_V3_ROUTER = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45"
+    DEFAULT_ROUTER_ADDRESS = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45"
+    ROUTER_ADDRESSES = {
+        # SwapRouter02
+        EthereumNetwork.MAINNET: DEFAULT_ROUTER_ADDRESS,
+        EthereumNetwork.CELO_MAINNET: "0x5615CDAb10dc425a742d643d949a7F474C01abc4",
+    }
 
     # Cache to optimize calculation: https://docs.uniswap.org/sdk/guides/fetching-prices#understanding-sqrtprice
     PRICE_CONVERSION_CONSTANT = 2**192
 
     def __init__(
         self,
         ethereum_client: EthereumClient,
         uniswap_v3_router_address: Optional[ChecksumAddress] = None,
     ):
         """
         :param ethereum_client:
+        :param uniswap_v3_router_address: Provide a custom `SwapRouter02` address
         """
         self.ethereum_client = ethereum_client
         self.w3 = ethereum_client.w3
 
-        self.router_address = uniswap_v3_router_address or self.UNISWAP_V3_ROUTER
+        self.router_address = uniswap_v3_router_address or self.ROUTER_ADDRESSES.get(
+            self.ethereum_client.get_network(), self.DEFAULT_ROUTER_ADDRESS
+        )
         self.factory = self.get_factory()
 
     @classmethod
     def is_available(
         cls,
         ethereum_client: EthereumClient,
         uniswap_v3_router_address: Optional[ChecksumAddress] = None,
     ) -> bool:
         """
         :param ethereum_client:
-        :param uniswap_v3_router_address:
+        :param uniswap_v3_router_address: Provide a custom `SwapRouter02` address
         :return: `True` if Uniswap V3 is available for the EthereumClient provided, `False` otherwise
         """
-        return ethereum_client.is_contract(
-            uniswap_v3_router_address or cls.UNISWAP_V3_ROUTER
+        router_address = uniswap_v3_router_address or cls.ROUTER_ADDRESSES.get(
+            ethereum_client.get_network(), cls.DEFAULT_ROUTER_ADDRESS
         )
+        return ethereum_client.is_contract(router_address)
 
     def get_factory(self) -> Contract:
         """
         Factory contract creates the pools for token pairs
 
         :return: Uniswap V3 Factory Contract
         """
         try:
             factory_address = self.router.functions.factory().call()
-        except BadFunctionCallOutput:
+        except Web3Exception:
             raise ValueError(
                 f"Uniswap V3 Router Contract {self.router_address} does not exist"
             )
         return self.w3.eth.contract(factory_address, abi=uniswap_v3_factory_abi)
 
     @cached_property
     def router(self) -> Contract:
@@ -158,31 +167,31 @@
                     ).functions.balanceOf(pool_address),
                     pool_contract.functions.slot0(),
                 ]
             )
             if (token_balance / 10**token_decimals) < 2 or (
                 token_2_balance / 10**token_2_decimals
             ) < 2:
-                error_message = (
+                message = (
                     f"Not enough liquidity on uniswap v3 for pair token_1={token_address} "
                     f"token_2={token_address_2}, at least 2 units of each token are required"
                 )
-                logger.warning(error_message)
-                raise CannotGetPriceFromOracle(error_message)
+                logger.debug(message)
+                raise CannotGetPriceFromOracle(message)
         except (
-            ValueError,
-            BadFunctionCallOutput,
+            Web3Exception,
             DecodingError,
+            ValueError,
         ) as e:
-            error_message = (
+            message = (
                 f"Cannot get uniswap v3 price for pair token_1={token_address} "
                 f"token_2={token_address_2}"
             )
-            logger.warning(error_message)
-            raise CannotGetPriceFromOracle(error_message) from e
+            logger.debug(message)
+            raise CannotGetPriceFromOracle(message) from e
 
         # https://docs.uniswap.org/sdk/guides/fetching-prices
         if not reversed:
             # Multiplying by itself is way faster than exponential
             price = (sqrt_price_x96 * sqrt_price_x96) / self.PRICE_CONVERSION_CONSTANT
         else:
             price = self.PRICE_CONVERSION_CONSTANT / (sqrt_price_x96 * sqrt_price_x96)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class TestBlockscoutClient(TestCase):
     @pytest.mark.flaky(reruns=5)
     def test_blockscout_client(self):
         with self.assertRaises(BlockScoutConfigurationProblem):
             BlockscoutClient(EthereumNetwork.MAINNET)
 
-        blockscout_client = BlockscoutClient(EthereumNetwork.XDAI)
+        blockscout_client = BlockscoutClient(EthereumNetwork.GNOSIS)
         safe_master_copy_abi = sourcify_safe_metadata["output"]["abi"]
         safe_master_copy_address = "0x6851D6fDFAfD08c0295C392436245E5bc78B0185"
         contract_metadata = blockscout_client.get_contract_metadata(
             safe_master_copy_address
         )
         self.assertEqual(contract_metadata.name, "GnosisSafe")
         self.assertEqual(contract_metadata.abi, safe_master_copy_abi)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/clients/test_sourcify.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/ethereum_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self, initial_ether: float = 0, initial_wei: int = 0
     ) -> LocalAccount:
         account = Account.create()
         if initial_ether > 0.0 or initial_wei > 0:
             self.send_tx(
                 {
                     "to": account.address,
-                    "value": self.w3.toWei(initial_ether, "ether") + initial_wei,
+                    "value": self.w3.to_wei(initial_ether, "ether") + initial_wei,
                 },
                 self.ethereum_test_account,
             )
         return account
 
     def deploy_erc20(
         self,
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,27 @@
             "from": "0x4e59b44847b379578588920cA78FbF26c0B4956C",
             "gas": 4619079,
             "value": 0,
             "init": HexBytes(
                 "0x608060405234801561001057600080fd5b5060016004819055506159ae80620000296000396000f3fe6080604052600436106101dc5760003560e01c8063affed0e011610102578063e19a9dd911610095578063f08a032311610064578063f08a032314611647578063f698da2514611698578063f8dc5dd9146116c3578063ffa1ad741461173e57610231565b8063e19a9dd91461139b578063e318b52b146113ec578063e75235b81461147d578063e86637db146114a857610231565b8063cc2f8452116100d1578063cc2f8452146110e8578063d4d9bdcd146111b5578063d8d11f78146111f0578063e009cfde1461132a57610231565b8063affed0e014610d94578063b4faba0914610dbf578063b63e800d14610ea7578063c4ca3a9c1461101757610231565b80635624b25b1161017a5780636a761202116101495780636a761202146109945780637d83297414610b50578063934f3a1114610bbf578063a0e67e2b14610d2857610231565b80635624b25b146107fb5780635ae6bd37146108b9578063610b592514610908578063694e80c31461095957610231565b80632f54bf6e116101b65780632f54bf6e146104d35780633408e4701461053a578063468721a7146105655780635229073f1461067a57610231565b80630d582f131461029e57806312fb68e0146102f95780632d9ad53d1461046c57610231565b36610231573373ffffffffffffffffffffffffffffffffffffffff167f3d0ce9bfc3ed7d6862dbb28b2dea94561fe714a1b4d019aa8af39730d1ad7c3d346040518082815260200191505060405180910390a2005b34801561023d57600080fd5b5060007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b905080548061027257600080f35b36600080373360601b365260008060143601600080855af13d6000803e80610299573d6000fd5b3d6000f35b3480156102aa57600080fd5b506102f7600480360360408110156102c157600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506117ce565b005b34801561030557600080fd5b5061046a6004803603608081101561031c57600080fd5b81019080803590602001909291908035906020019064010000000081111561034357600080fd5b82018360208201111561035557600080fd5b8035906020019184600183028401116401000000008311171561037757600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803590602001906401000000008111156103da57600080fd5b8201836020820111156103ec57600080fd5b8035906020019184600183028401116401000000008311171561040e57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190929190505050611bbe565b005b34801561047857600080fd5b506104bb6004803603602081101561048f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612440565b60405180821515815260200191505060405180910390f35b3480156104df57600080fd5b50610522600480360360208110156104f657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612512565b60405180821515815260200191505060405180910390f35b34801561054657600080fd5b5061054f6125e4565b6040518082815260200191505060405180910390f35b34801561057157600080fd5b506106626004803603608081101561058857600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156105cf57600080fd5b8201836020820111156105e157600080fd5b8035906020019184600183028401116401000000008311171561060357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506125f1565b60405180821515815260200191505060405180910390f35b34801561068657600080fd5b506107776004803603608081101561069d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156106e457600080fd5b8201836020820111156106f657600080fd5b8035906020019184600183028401116401000000008311171561071857600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506127d7565b60405180831515815260200180602001828103825283818151815260200191508051906020019080838360005b838110156107bf5780820151818401526020810190506107a4565b50505050905090810190601f1680156107ec5780820380516001836020036101000a031916815260200191505b50935050505060405180910390f35b34801561080757600080fd5b5061083e6004803603604081101561081e57600080fd5b81019080803590602001909291908035906020019092919050505061280d565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561087e578082015181840152602081019050610863565b50505050905090810190601f1680156108ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b3480156108c557600080fd5b506108f2600480360360208110156108dc57600080fd5b8101908080359060200190929190505050612894565b6040518082815260200191505060405180910390f35b34801561091457600080fd5b506109576004803603602081101561092b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff1690602001909291905050506128ac565b005b34801561096557600080fd5b506109926004803603602081101561097c57600080fd5b8101908080359060200190929190505050612c3e565b005b610b3860048036036101408110156109ab57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156109f257600080fd5b820183602082011115610a0457600080fd5b80359060200191846001830284011164010000000083111715610a2657600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610ab257600080fd5b820183602082011115610ac457600080fd5b80359060200191846001830284011164010000000083111715610ae657600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050612d78565b60405180821515815260200191505060405180910390f35b348015610b5c57600080fd5b50610ba960048036036040811015610b7357600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506132b5565b6040518082815260200191505060405180910390f35b348015610bcb57600080fd5b50610d2660048036036060811015610be257600080fd5b810190808035906020019092919080359060200190640100000000811115610c0957600080fd5b820183602082011115610c1b57600080fd5b80359060200191846001830284011164010000000083111715610c3d57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190640100000000811115610ca057600080fd5b820183602082011115610cb257600080fd5b80359060200191846001830284011164010000000083111715610cd457600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505091929192905050506132da565b005b348015610d3457600080fd5b50610d3d613369565b6040518080602001828103825283818151815260200191508051906020019060200280838360005b83811015610d80578082015181840152602081019050610d65565b505050509050019250505060405180910390f35b348015610da057600080fd5b50610da9613512565b6040518082815260200191505060405180910390f35b348015610dcb57600080fd5b50610ea560048036036040811015610de257600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610e1f57600080fd5b820183602082011115610e3157600080fd5b80359060200191846001830284011164010000000083111715610e5357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050613518565b005b348015610eb357600080fd5b506110156004803603610100811015610ecb57600080fd5b8101908080359060200190640100000000811115610ee857600080fd5b820183602082011115610efa57600080fd5b80359060200191846020830284011164010000000083111715610f1c57600080fd5b909192939192939080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610f6757600080fd5b820183602082011115610f7957600080fd5b80359060200191846001830284011164010000000083111715610f9b57600080fd5b9091929391929390803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919050505061353a565b005b34801561102357600080fd5b506110d26004803603608081101561103a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561108157600080fd5b82018360208201111561109357600080fd5b803590602001918460018302840111640100000000831117156110b557600080fd5b9091929391929390803560ff1690602001909291905050506136f8565b6040518082815260200191505060405180910390f35b3480156110f457600080fd5b506111416004803603604081101561110b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613820565b60405180806020018373ffffffffffffffffffffffffffffffffffffffff168152602001828103825284818151815260200191508051906020019060200280838360005b838110156111a0578082015181840152602081019050611185565b50505050905001935050505060405180910390f35b3480156111c157600080fd5b506111ee600480360360208110156111d857600080fd5b8101908080359060200190929190505050613a12565b005b3480156111fc57600080fd5b50611314600480360361014081101561121457600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561125b57600080fd5b82018360208201111561126d57600080fd5b8035906020019184600183028401116401000000008311171561128f57600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613bb1565b6040518082815260200191505060405180910390f35b34801561133657600080fd5b506113996004803603604081101561134d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613bde565b005b3480156113a757600080fd5b506113ea600480360360208110156113be57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613f6f565b005b3480156113f857600080fd5b5061147b6004803603606081101561140f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613ff3565b005b34801561148957600080fd5b50611492614665565b6040518082815260200191505060405180910390f35b3480156114b457600080fd5b506115cc60048036036101408110156114cc57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561151357600080fd5b82018360208201111561152557600080fd5b8035906020019184600183028401116401000000008311171561154757600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff1690602001909291908035906020019092919050505061466f565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561160c5780820151818401526020810190506115f1565b50505050905090810190601f1680156116395780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b34801561165357600080fd5b506116966004803603602081101561166a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050614817565b005b3480156116a457600080fd5b506116ad614878565b6040518082815260200191505060405180910390f35b3480156116cf57600080fd5b5061173c600480360360608110156116e657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506148f6565b005b34801561174a57600080fd5b50611753614d29565b6040518080602001828103825283818151815260200191508051906020019080838360005b83811015611793578082015181840152602081019050611778565b50505050905090810190601f1680156117c05780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6117d6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156118405750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b801561187857503073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6118ea576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146119eb576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508160026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506003600081548092919060010191905055507f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2682604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414611bba57611bb981612c3e565b5b5050565b611bd2604182614e0590919063ffffffff16565b82511015611c48576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6000808060008060005b8681101561243457611c648882614e3f565b80945081955082965050505060008460ff16141561206d578260001c9450611c96604188614e0590919063ffffffff16565b8260001c1015611d0e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8751611d2760208460001c614e6e90919063ffffffff16565b1115611d9b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006020838a01015190508851611dd182611dc360208760001c614e6e90919063ffffffff16565b614e6e90919063ffffffff16565b1115611e45576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60606020848b010190506320c13b0b60e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168773ffffffffffffffffffffffffffffffffffffffff166320c13b0b8d846040518363ffffffff1660e01b8152600401808060200180602001838103835285818151815260200191508051906020019080838360005b83811015611ee7578082015181840152602081019050611ecc565b50505050905090810190601f168015611f145780820380516001836020036101000a031916815260200191505b50838103825284818151815260200191508051906020019080838360005b83811015611f4d578082015181840152602081019050611f32565b50505050905090810190601f168015611f7a5780820380516001836020036101000a031916815260200191505b5094505050505060206040518083038186803b158015611f9957600080fd5b505afa158015611fad573d6000803e3d6000fd5b505050506040513d6020811015611fc357600080fd5b81019080805190602001909291905050507bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614612066576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b50506122b2565b60018460ff161415612181578260001c94508473ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16148061210a57506000600860008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008c81526020019081526020016000205414155b61217c576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6122b1565b601e8460ff1611156122495760018a60405160200180807f19457468657265756d205369676e6564204d6573736167653a0a333200000000815250601c018281526020019150506040516020818303038152906040528051906020012060048603858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa158015612238573d6000803e3d6000fd5b5050506020604051035194506122b0565b60018a85858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa1580156122a3573d6000803e3d6000fd5b5050506020604051035194505b5b5b8573ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff161180156123795750600073ffffffffffffffffffffffffffffffffffffffff16600260008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b80156123b25750600173ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff1614155b612424576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323600000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8495508080600101915050611c52565b50505050505050505050565b60008173ffffffffffffffffffffffffffffffffffffffff16600173ffffffffffffffffffffffffffffffffffffffff161415801561250b5750600073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156125dd5750600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000804690508091505090565b6000600173ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141580156126bc5750600073ffffffffffffffffffffffffffffffffffffffff16600160003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b61272e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61273b858585855a614e8d565b9050801561278b573373ffffffffffffffffffffffffffffffffffffffff167f6895c13664aa4f67288b25d7a21d7aaa34916e355fb9b6fae0a139a9085becb860405160405180910390a26127cf565b3373ffffffffffffffffffffffffffffffffffffffff167facd2c8702804128fdb0db2bb49f6d127dd0181c13fd45dbfe16de0930e2bd37560405160405180910390a25b949350505050565b600060606127e7868686866125f1565b915060405160203d0181016040523d81523d6000602083013e8091505094509492505050565b606060006020830267ffffffffffffffff8111801561282b57600080fd5b506040519080825280601f01601f19166020018201604052801561285e5781602001600182028036833780820191505090505b50905060005b8381101561288957808501548060208302602085010152508080600101915050612864565b508091505092915050565b60076020528060005260406000206000915090505481565b6128b4614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561291e5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b612990576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614612a91576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508060016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507fecdf3a3effea5783a3c4c2140e677577666428d44ed9d474a0b3a4c9943f844081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b612c46614d62565b600354811115612cbe576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001811015612d35576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b806004819055507f610f7ff2b304ae8903c3de74c60c6ab1f7d6226b3f52c5161905bb5ad4039c936004546040518082815260200191505060405180910390a150565b6000806000612d928e8e8e8e8e8e8e8e8e8e60055461466f565b905060056000815480929190600101919050555080805190602001209150612dbb8282866132da565b506000612dc6614ed9565b9050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614612fac578073ffffffffffffffffffffffffffffffffffffffff166375f0bb528f8f8f8f8f8f8f8f8f8f8f336040518d63ffffffff1660e01b8152600401808d73ffffffffffffffffffffffffffffffffffffffff1681526020018c8152602001806020018a6001811115612e6957fe5b81526020018981526020018881526020018781526020018673ffffffffffffffffffffffffffffffffffffffff1681526020018573ffffffffffffffffffffffffffffffffffffffff168152602001806020018473ffffffffffffffffffffffffffffffffffffffff16815260200183810383528d8d82818152602001925080828437600081840152601f19601f820116905080830192505050838103825285818151815260200191508051906020019080838360005b83811015612f3b578082015181840152602081019050612f20565b50505050905090810190601f168015612f685780820380516001836020036101000a031916815260200191505b509e505050505050505050505050505050600060405180830381600087803b158015612f9357600080fd5b505af1158015612fa7573d6000803e3d6000fd5b505050505b6101f4612fd36109c48b01603f60408d0281612fc457fe5b04614f0a90919063ffffffff16565b015a1015613049576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60005a90506130b28f8f8f8f8080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050508e60008d146130a7578e6130ad565b6109c45a035b614e8d565b93506130c75a82614f2490919063ffffffff16565b905083806130d6575060008a14155b806130e2575060008814155b613154576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60008089111561316e5761316b828b8b8b8b614f44565b90505b84156131b8577f442e715f626346e8c54381002da614f62bee8d27386535b2521ec8540898556e8482604051808381526020018281526020019250505060405180910390a16131f8565b7f23428b18acfb3ea64b08dc0c1d296ea9c09702c09083ca5272e64d115b687d238482604051808381526020018281526020019250505060405180910390a15b5050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16146132a4578073ffffffffffffffffffffffffffffffffffffffff16639327136883856040518363ffffffff1660e01b815260040180838152602001821515815260200192505050600060405180830381600087803b15801561328b57600080fd5b505af115801561329f573d6000803e3d6000fd5b505050505b50509b9a5050505050505050505050565b6008602052816000526040600020602052806000526040600020600091509150505481565b6000600454905060008111613357576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61336384848484611bbe565b50505050565b6060600060035467ffffffffffffffff8111801561338657600080fd5b506040519080825280602002602001820160405280156133b55781602001602082028036833780820191505090505b50905060008060026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614613509578083838151811061346057fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600260008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050818060010192505061341f565b82935050505090565b60055481565b600080825160208401855af4806000523d6020523d600060403e60403d016000fd5b6135858a8a80806020026020016040519081016040528093929190818152602001838360200280828437600081840152601f19601f820116905080830192505050505050508961514a565b600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16146135c3576135c28461564a565b5b6136118787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050615679565b600082111561362b5761362982600060018685614f44565b505b3373ffffffffffffffffffffffffffffffffffffffff167f141df868a6331af528e38c83b7aa03edc19be66e37ae67f9285bf4f8e3c6a1a88b8b8b8b8960405180806020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281038252878782818152602001925060200280828437600081840152601f19601f820116905080830192505050965050505050505060405180910390a250505050505050505050565b6000805a905061374f878787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050865a614e8d565b61375857600080fd5b60005a8203905080604051602001808281526020019150506040516020818303038152906040526040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825283818151815260200191508051906020019080838360005b838110156137e55780820151818401526020810190506137ca565b50505050905090810190601f1680156138125780820380516001836020036101000a031916815260200191505b509250505060405180910390fd5b606060008267ffffffffffffffff8111801561383b57600080fd5b5060405190808252806020026020018201604052801561386a5781602001602082028036833780820191505090505b509150600080600160008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561393d5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561394857508482105b15613a03578084838151811061395a57fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16905081806001019250506138d3565b80925081845250509250929050565b600073ffffffffffffffffffffffffffffffffffffffff16600260003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161415613b14576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001600860003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020016000206000838152602001908152602001600020819055503373ffffffffffffffffffffffffffffffffffffffff16817ff2a0eb156472d1440255b0d7c1e19cc07115d1051fe605b0dce69acfec884d9c60405160405180910390a350565b6000613bc68c8c8c8c8c8c8c8c8c8c8c61466f565b8051906020012090509b9a5050505050505050505050565b613be6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614158015613c505750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b613cc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614613dc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507faab4fa2b463f581b2b32cb3b7e3b704b9ce37cc209b5fb4d77e593ace405427681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613f77614d62565b60007f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b90508181557f1151116914515bc0891ff9047a6cb32cf902546f83066499bcf8ba33d2353fa282604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613ffb614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156140655750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561409d57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b61410f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614210576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff161415801561427a5750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6142ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146143ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555080600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a17f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a1505050565b6000600454905090565b606060007fbb8310d486368db6bd6f849402fdd73ad53d316b5a4b2644ad6efe0f941286d860001b8d8d8d8d60405180838380828437808301925050509250505060405180910390208c8c8c8c8c8c8c604051602001808c81526020018b73ffffffffffffffffffffffffffffffffffffffff1681526020018a815260200189815260200188600181111561470057fe5b81526020018781526020018681526020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281526020019b505050505050505050505050604051602081830303815290604052805190602001209050601960f81b600160f81b61478c614878565b8360405160200180857effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168152600101847effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff191681526001018381526020018281526020019450505050506040516020818303038152906040529150509b9a5050505050505050505050565b61481f614d62565b6148288161564a565b7f5ac6c46c93c8d0e53714ba3b53db3e7c046da994313d7ed0d192028bc7c228b081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b60007f47e79534a245952e8b16893a336b85a3d9ea9fa8c573f3d803afb92a7946921860001b6148a66125e4565b30604051602001808481526020018381526020018273ffffffffffffffffffffffffffffffffffffffff168152602001935050505060405160208183030381529060405280519060200120905090565b6148fe614d62565b806001600354031015614979576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156149e35750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b614a55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614b55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600360008154809291906001900391905055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414614d2457614d2381612c3e565b5b505050565b6040518060400160405280600581526020017f312e332e3000000000000000000000000000000000000000000000000000000081525081565b3073ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff1614614e03576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b565b600080831415614e185760009050614e39565b6000828402905082848281614e2957fe5b0414614e3457600080fd5b809150505b92915050565b60008060008360410260208101860151925060408101860151915060ff60418201870151169350509250925092565b600080828401905083811015614e8357600080fd5b8091505092915050565b6000600180811115614e9b57fe5b836001811115614ea757fe5b1415614ec0576000808551602087018986f49050614ed0565b600080855160208701888a87f190505b95945050505050565b6000807f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b9050805491505090565b600081831015614f1a5781614f1c565b825b905092915050565b600082821115614f3357600080fd5b600082840390508091505092915050565b600080600073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614614f815782614f83565b325b9050600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16141561509b57614fed3a8610614fca573a614fcc565b855b614fdf888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91508073ffffffffffffffffffffffffffffffffffffffff166108fc839081150290604051600060405180830381858888f19350505050615096576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b615140565b6150c0856150b2888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91506150cd8482846158b4565b61513f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5095945050505050565b6000600454146151c2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8151811115615239576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60018110156152b0576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006001905060005b83518110156155b65760008482815181106152d057fe5b60200260200101519050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156153445750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561537c57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b80156153b457508073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614155b615426576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614615527576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b80600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508092505080806001019150506152b9565b506001600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550825160038190555081600481905550505050565b60007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b90508181555050565b600073ffffffffffffffffffffffffffffffffffffffff1660016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161461577b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001806000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16146158b05761583d8260008360015a614e8d565b6158af576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5050565b60008063a9059cbb8484604051602401808373ffffffffffffffffffffffffffffffffffffffff168152602001828152602001925050506040516020818303038152906040529060e01b6020820180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff83818316178352505050509050602060008251602084016000896127105a03f13d6000811461595b5760208114615963576000935061596e565b81935061596e565b600051158215171593505b505050939250505056fea26469706673582212203874bcf92e1722cc7bfa0cef1a0985cf0dc3485ba0663db3747ccdf1605df53464736f6c63430007060033"
             ),
         },
-        "blockHash": "0x4160d3b92f3678386a108e0838016dd3010ba12389712a30f2b017d33799d05e",
+        "blockHash": HexBytes(
+            "0x4160d3b92f3678386a108e0838016dd3010ba12389712a30f2b017d33799d05e"
+        ),
         "blockNumber": 12504268,
         "result": {
             "gasUsed": 4619079,
             "code": HexBytes(
                 "0x6080604052600436106101dc5760003560e01c8063affed0e011610102578063e19a9dd911610095578063f08a032311610064578063f08a032314611647578063f698da2514611698578063f8dc5dd9146116c3578063ffa1ad741461173e57610231565b8063e19a9dd91461139b578063e318b52b146113ec578063e75235b81461147d578063e86637db146114a857610231565b8063cc2f8452116100d1578063cc2f8452146110e8578063d4d9bdcd146111b5578063d8d11f78146111f0578063e009cfde1461132a57610231565b8063affed0e014610d94578063b4faba0914610dbf578063b63e800d14610ea7578063c4ca3a9c1461101757610231565b80635624b25b1161017a5780636a761202116101495780636a761202146109945780637d83297414610b50578063934f3a1114610bbf578063a0e67e2b14610d2857610231565b80635624b25b146107fb5780635ae6bd37146108b9578063610b592514610908578063694e80c31461095957610231565b80632f54bf6e116101b65780632f54bf6e146104d35780633408e4701461053a578063468721a7146105655780635229073f1461067a57610231565b80630d582f131461029e57806312fb68e0146102f95780632d9ad53d1461046c57610231565b36610231573373ffffffffffffffffffffffffffffffffffffffff167f3d0ce9bfc3ed7d6862dbb28b2dea94561fe714a1b4d019aa8af39730d1ad7c3d346040518082815260200191505060405180910390a2005b34801561023d57600080fd5b5060007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b905080548061027257600080f35b36600080373360601b365260008060143601600080855af13d6000803e80610299573d6000fd5b3d6000f35b3480156102aa57600080fd5b506102f7600480360360408110156102c157600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506117ce565b005b34801561030557600080fd5b5061046a6004803603608081101561031c57600080fd5b81019080803590602001909291908035906020019064010000000081111561034357600080fd5b82018360208201111561035557600080fd5b8035906020019184600183028401116401000000008311171561037757600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803590602001906401000000008111156103da57600080fd5b8201836020820111156103ec57600080fd5b8035906020019184600183028401116401000000008311171561040e57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190929190505050611bbe565b005b34801561047857600080fd5b506104bb6004803603602081101561048f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612440565b60405180821515815260200191505060405180910390f35b3480156104df57600080fd5b50610522600480360360208110156104f657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612512565b60405180821515815260200191505060405180910390f35b34801561054657600080fd5b5061054f6125e4565b6040518082815260200191505060405180910390f35b34801561057157600080fd5b506106626004803603608081101561058857600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156105cf57600080fd5b8201836020820111156105e157600080fd5b8035906020019184600183028401116401000000008311171561060357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506125f1565b60405180821515815260200191505060405180910390f35b34801561068657600080fd5b506107776004803603608081101561069d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156106e457600080fd5b8201836020820111156106f657600080fd5b8035906020019184600183028401116401000000008311171561071857600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506127d7565b60405180831515815260200180602001828103825283818151815260200191508051906020019080838360005b838110156107bf5780820151818401526020810190506107a4565b50505050905090810190601f1680156107ec5780820380516001836020036101000a031916815260200191505b50935050505060405180910390f35b34801561080757600080fd5b5061083e6004803603604081101561081e57600080fd5b81019080803590602001909291908035906020019092919050505061280d565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561087e578082015181840152602081019050610863565b50505050905090810190601f1680156108ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b3480156108c557600080fd5b506108f2600480360360208110156108dc57600080fd5b8101908080359060200190929190505050612894565b6040518082815260200191505060405180910390f35b34801561091457600080fd5b506109576004803603602081101561092b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff1690602001909291905050506128ac565b005b34801561096557600080fd5b506109926004803603602081101561097c57600080fd5b8101908080359060200190929190505050612c3e565b005b610b3860048036036101408110156109ab57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156109f257600080fd5b820183602082011115610a0457600080fd5b80359060200191846001830284011164010000000083111715610a2657600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610ab257600080fd5b820183602082011115610ac457600080fd5b80359060200191846001830284011164010000000083111715610ae657600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050612d78565b60405180821515815260200191505060405180910390f35b348015610b5c57600080fd5b50610ba960048036036040811015610b7357600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506132b5565b6040518082815260200191505060405180910390f35b348015610bcb57600080fd5b50610d2660048036036060811015610be257600080fd5b810190808035906020019092919080359060200190640100000000811115610c0957600080fd5b820183602082011115610c1b57600080fd5b80359060200191846001830284011164010000000083111715610c3d57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190640100000000811115610ca057600080fd5b820183602082011115610cb257600080fd5b80359060200191846001830284011164010000000083111715610cd457600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505091929192905050506132da565b005b348015610d3457600080fd5b50610d3d613369565b6040518080602001828103825283818151815260200191508051906020019060200280838360005b83811015610d80578082015181840152602081019050610d65565b505050509050019250505060405180910390f35b348015610da057600080fd5b50610da9613512565b6040518082815260200191505060405180910390f35b348015610dcb57600080fd5b50610ea560048036036040811015610de257600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610e1f57600080fd5b820183602082011115610e3157600080fd5b80359060200191846001830284011164010000000083111715610e5357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050613518565b005b348015610eb357600080fd5b506110156004803603610100811015610ecb57600080fd5b8101908080359060200190640100000000811115610ee857600080fd5b820183602082011115610efa57600080fd5b80359060200191846020830284011164010000000083111715610f1c57600080fd5b909192939192939080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610f6757600080fd5b820183602082011115610f7957600080fd5b80359060200191846001830284011164010000000083111715610f9b57600080fd5b9091929391929390803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919050505061353a565b005b34801561102357600080fd5b506110d26004803603608081101561103a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561108157600080fd5b82018360208201111561109357600080fd5b803590602001918460018302840111640100000000831117156110b557600080fd5b9091929391929390803560ff1690602001909291905050506136f8565b6040518082815260200191505060405180910390f35b3480156110f457600080fd5b506111416004803603604081101561110b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613820565b60405180806020018373ffffffffffffffffffffffffffffffffffffffff168152602001828103825284818151815260200191508051906020019060200280838360005b838110156111a0578082015181840152602081019050611185565b50505050905001935050505060405180910390f35b3480156111c157600080fd5b506111ee600480360360208110156111d857600080fd5b8101908080359060200190929190505050613a12565b005b3480156111fc57600080fd5b50611314600480360361014081101561121457600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561125b57600080fd5b82018360208201111561126d57600080fd5b8035906020019184600183028401116401000000008311171561128f57600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613bb1565b6040518082815260200191505060405180910390f35b34801561133657600080fd5b506113996004803603604081101561134d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613bde565b005b3480156113a757600080fd5b506113ea600480360360208110156113be57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613f6f565b005b3480156113f857600080fd5b5061147b6004803603606081101561140f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613ff3565b005b34801561148957600080fd5b50611492614665565b6040518082815260200191505060405180910390f35b3480156114b457600080fd5b506115cc60048036036101408110156114cc57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561151357600080fd5b82018360208201111561152557600080fd5b8035906020019184600183028401116401000000008311171561154757600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff1690602001909291908035906020019092919050505061466f565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561160c5780820151818401526020810190506115f1565b50505050905090810190601f1680156116395780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b34801561165357600080fd5b506116966004803603602081101561166a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050614817565b005b3480156116a457600080fd5b506116ad614878565b6040518082815260200191505060405180910390f35b3480156116cf57600080fd5b5061173c600480360360608110156116e657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506148f6565b005b34801561174a57600080fd5b50611753614d29565b6040518080602001828103825283818151815260200191508051906020019080838360005b83811015611793578082015181840152602081019050611778565b50505050905090810190601f1680156117c05780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6117d6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156118405750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b801561187857503073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6118ea576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146119eb576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508160026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506003600081548092919060010191905055507f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2682604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414611bba57611bb981612c3e565b5b5050565b611bd2604182614e0590919063ffffffff16565b82511015611c48576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6000808060008060005b8681101561243457611c648882614e3f565b80945081955082965050505060008460ff16141561206d578260001c9450611c96604188614e0590919063ffffffff16565b8260001c1015611d0e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8751611d2760208460001c614e6e90919063ffffffff16565b1115611d9b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006020838a01015190508851611dd182611dc360208760001c614e6e90919063ffffffff16565b614e6e90919063ffffffff16565b1115611e45576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60606020848b010190506320c13b0b60e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168773ffffffffffffffffffffffffffffffffffffffff166320c13b0b8d846040518363ffffffff1660e01b8152600401808060200180602001838103835285818151815260200191508051906020019080838360005b83811015611ee7578082015181840152602081019050611ecc565b50505050905090810190601f168015611f145780820380516001836020036101000a031916815260200191505b50838103825284818151815260200191508051906020019080838360005b83811015611f4d578082015181840152602081019050611f32565b50505050905090810190601f168015611f7a5780820380516001836020036101000a031916815260200191505b5094505050505060206040518083038186803b158015611f9957600080fd5b505afa158015611fad573d6000803e3d6000fd5b505050506040513d6020811015611fc357600080fd5b81019080805190602001909291905050507bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614612066576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b50506122b2565b60018460ff161415612181578260001c94508473ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16148061210a57506000600860008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008c81526020019081526020016000205414155b61217c576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6122b1565b601e8460ff1611156122495760018a60405160200180807f19457468657265756d205369676e6564204d6573736167653a0a333200000000815250601c018281526020019150506040516020818303038152906040528051906020012060048603858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa158015612238573d6000803e3d6000fd5b5050506020604051035194506122b0565b60018a85858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa1580156122a3573d6000803e3d6000fd5b5050506020604051035194505b5b5b8573ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff161180156123795750600073ffffffffffffffffffffffffffffffffffffffff16600260008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b80156123b25750600173ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff1614155b612424576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323600000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8495508080600101915050611c52565b50505050505050505050565b60008173ffffffffffffffffffffffffffffffffffffffff16600173ffffffffffffffffffffffffffffffffffffffff161415801561250b5750600073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156125dd5750600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000804690508091505090565b6000600173ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141580156126bc5750600073ffffffffffffffffffffffffffffffffffffffff16600160003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b61272e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61273b858585855a614e8d565b9050801561278b573373ffffffffffffffffffffffffffffffffffffffff167f6895c13664aa4f67288b25d7a21d7aaa34916e355fb9b6fae0a139a9085becb860405160405180910390a26127cf565b3373ffffffffffffffffffffffffffffffffffffffff167facd2c8702804128fdb0db2bb49f6d127dd0181c13fd45dbfe16de0930e2bd37560405160405180910390a25b949350505050565b600060606127e7868686866125f1565b915060405160203d0181016040523d81523d6000602083013e8091505094509492505050565b606060006020830267ffffffffffffffff8111801561282b57600080fd5b506040519080825280601f01601f19166020018201604052801561285e5781602001600182028036833780820191505090505b50905060005b8381101561288957808501548060208302602085010152508080600101915050612864565b508091505092915050565b60076020528060005260406000206000915090505481565b6128b4614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561291e5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b612990576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614612a91576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508060016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507fecdf3a3effea5783a3c4c2140e677577666428d44ed9d474a0b3a4c9943f844081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b612c46614d62565b600354811115612cbe576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001811015612d35576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b806004819055507f610f7ff2b304ae8903c3de74c60c6ab1f7d6226b3f52c5161905bb5ad4039c936004546040518082815260200191505060405180910390a150565b6000806000612d928e8e8e8e8e8e8e8e8e8e60055461466f565b905060056000815480929190600101919050555080805190602001209150612dbb8282866132da565b506000612dc6614ed9565b9050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614612fac578073ffffffffffffffffffffffffffffffffffffffff166375f0bb528f8f8f8f8f8f8f8f8f8f8f336040518d63ffffffff1660e01b8152600401808d73ffffffffffffffffffffffffffffffffffffffff1681526020018c8152602001806020018a6001811115612e6957fe5b81526020018981526020018881526020018781526020018673ffffffffffffffffffffffffffffffffffffffff1681526020018573ffffffffffffffffffffffffffffffffffffffff168152602001806020018473ffffffffffffffffffffffffffffffffffffffff16815260200183810383528d8d82818152602001925080828437600081840152601f19601f820116905080830192505050838103825285818151815260200191508051906020019080838360005b83811015612f3b578082015181840152602081019050612f20565b50505050905090810190601f168015612f685780820380516001836020036101000a031916815260200191505b509e505050505050505050505050505050600060405180830381600087803b158015612f9357600080fd5b505af1158015612fa7573d6000803e3d6000fd5b505050505b6101f4612fd36109c48b01603f60408d0281612fc457fe5b04614f0a90919063ffffffff16565b015a1015613049576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60005a90506130b28f8f8f8f8080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050508e60008d146130a7578e6130ad565b6109c45a035b614e8d565b93506130c75a82614f2490919063ffffffff16565b905083806130d6575060008a14155b806130e2575060008814155b613154576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60008089111561316e5761316b828b8b8b8b614f44565b90505b84156131b8577f442e715f626346e8c54381002da614f62bee8d27386535b2521ec8540898556e8482604051808381526020018281526020019250505060405180910390a16131f8565b7f23428b18acfb3ea64b08dc0c1d296ea9c09702c09083ca5272e64d115b687d238482604051808381526020018281526020019250505060405180910390a15b5050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16146132a4578073ffffffffffffffffffffffffffffffffffffffff16639327136883856040518363ffffffff1660e01b815260040180838152602001821515815260200192505050600060405180830381600087803b15801561328b57600080fd5b505af115801561329f573d6000803e3d6000fd5b505050505b50509b9a5050505050505050505050565b6008602052816000526040600020602052806000526040600020600091509150505481565b6000600454905060008111613357576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61336384848484611bbe565b50505050565b6060600060035467ffffffffffffffff8111801561338657600080fd5b506040519080825280602002602001820160405280156133b55781602001602082028036833780820191505090505b50905060008060026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614613509578083838151811061346057fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600260008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050818060010192505061341f565b82935050505090565b60055481565b600080825160208401855af4806000523d6020523d600060403e60403d016000fd5b6135858a8a80806020026020016040519081016040528093929190818152602001838360200280828437600081840152601f19601f820116905080830192505050505050508961514a565b600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16146135c3576135c28461564a565b5b6136118787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050615679565b600082111561362b5761362982600060018685614f44565b505b3373ffffffffffffffffffffffffffffffffffffffff167f141df868a6331af528e38c83b7aa03edc19be66e37ae67f9285bf4f8e3c6a1a88b8b8b8b8960405180806020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281038252878782818152602001925060200280828437600081840152601f19601f820116905080830192505050965050505050505060405180910390a250505050505050505050565b6000805a905061374f878787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050865a614e8d565b61375857600080fd5b60005a8203905080604051602001808281526020019150506040516020818303038152906040526040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825283818151815260200191508051906020019080838360005b838110156137e55780820151818401526020810190506137ca565b50505050905090810190601f1680156138125780820380516001836020036101000a031916815260200191505b509250505060405180910390fd5b606060008267ffffffffffffffff8111801561383b57600080fd5b5060405190808252806020026020018201604052801561386a5781602001602082028036833780820191505090505b509150600080600160008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561393d5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561394857508482105b15613a03578084838151811061395a57fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16905081806001019250506138d3565b80925081845250509250929050565b600073ffffffffffffffffffffffffffffffffffffffff16600260003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161415613b14576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001600860003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020016000206000838152602001908152602001600020819055503373ffffffffffffffffffffffffffffffffffffffff16817ff2a0eb156472d1440255b0d7c1e19cc07115d1051fe605b0dce69acfec884d9c60405160405180910390a350565b6000613bc68c8c8c8c8c8c8c8c8c8c8c61466f565b8051906020012090509b9a5050505050505050505050565b613be6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614158015613c505750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b613cc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614613dc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507faab4fa2b463f581b2b32cb3b7e3b704b9ce37cc209b5fb4d77e593ace405427681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613f77614d62565b60007f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b90508181557f1151116914515bc0891ff9047a6cb32cf902546f83066499bcf8ba33d2353fa282604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613ffb614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156140655750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561409d57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b61410f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614210576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff161415801561427a5750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6142ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146143ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555080600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a17f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a1505050565b6000600454905090565b606060007fbb8310d486368db6bd6f849402fdd73ad53d316b5a4b2644ad6efe0f941286d860001b8d8d8d8d60405180838380828437808301925050509250505060405180910390208c8c8c8c8c8c8c604051602001808c81526020018b73ffffffffffffffffffffffffffffffffffffffff1681526020018a815260200189815260200188600181111561470057fe5b81526020018781526020018681526020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281526020019b505050505050505050505050604051602081830303815290604052805190602001209050601960f81b600160f81b61478c614878565b8360405160200180857effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168152600101847effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff191681526001018381526020018281526020019450505050506040516020818303038152906040529150509b9a5050505050505050505050565b61481f614d62565b6148288161564a565b7f5ac6c46c93c8d0e53714ba3b53db3e7c046da994313d7ed0d192028bc7c228b081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b60007f47e79534a245952e8b16893a336b85a3d9ea9fa8c573f3d803afb92a7946921860001b6148a66125e4565b30604051602001808481526020018381526020018273ffffffffffffffffffffffffffffffffffffffff168152602001935050505060405160208183030381529060405280519060200120905090565b6148fe614d62565b806001600354031015614979576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156149e35750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b614a55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614b55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600360008154809291906001900391905055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414614d2457614d2381612c3e565b5b505050565b6040518060400160405280600581526020017f312e332e3000000000000000000000000000000000000000000000000000000081525081565b3073ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff1614614e03576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b565b600080831415614e185760009050614e39565b6000828402905082848281614e2957fe5b0414614e3457600080fd5b809150505b92915050565b60008060008360410260208101860151925060408101860151915060ff60418201870151169350509250925092565b600080828401905083811015614e8357600080fd5b8091505092915050565b6000600180811115614e9b57fe5b836001811115614ea757fe5b1415614ec0576000808551602087018986f49050614ed0565b600080855160208701888a87f190505b95945050505050565b6000807f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b9050805491505090565b600081831015614f1a5781614f1c565b825b905092915050565b600082821115614f3357600080fd5b600082840390508091505092915050565b600080600073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614614f815782614f83565b325b9050600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16141561509b57614fed3a8610614fca573a614fcc565b855b614fdf888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91508073ffffffffffffffffffffffffffffffffffffffff166108fc839081150290604051600060405180830381858888f19350505050615096576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b615140565b6150c0856150b2888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91506150cd8482846158b4565b61513f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5095945050505050565b6000600454146151c2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8151811115615239576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60018110156152b0576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006001905060005b83518110156155b65760008482815181106152d057fe5b60200260200101519050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156153445750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561537c57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b80156153b457508073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614155b615426576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614615527576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b80600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508092505080806001019150506152b9565b506001600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550825160038190555081600481905550505050565b60007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b90508181555050565b600073ffffffffffffffffffffffffffffffffffffffff1660016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161461577b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001806000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16146158b05761583d8260008360015a614e8d565b6158af576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5050565b60008063a9059cbb8484604051602401808373ffffffffffffffffffffffffffffffffffffffff168152602001828152602001925050506040516020818303038152906040529060e01b6020820180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff83818316178352505050509050602060008251602084016000896127105a03f13d6000811461595b5760208114615963576000935061596e565b81935061596e565b600051158215171593505b505050939250505056fea26469706673582212203874bcf92e1722cc7bfa0cef1a0985cf0dc3485ba0663db3747ccdf1605df53464736f6c63430007060033"
             ),
             "address": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
         },
         "subtraces": 0,
         "traceAddress": [0],
-        "transactionHash": "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f",
+        "transactionHash": HexBytes(
+            "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f"
+        ),
         "transactionPosition": 12,
         "type": "create",
     }
 ]
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,47 +9,55 @@
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000000608060405234801561001057600080fd5b5060016004819055506159ae80620000296000396000f3fe6080604052600436106101dc5760003560e01c8063affed0e011610102578063e19a9dd911610095578063f08a032311610064578063f08a032314611647578063f698da2514611698578063f8dc5dd9146116c3578063ffa1ad741461173e57610231565b8063e19a9dd91461139b578063e318b52b146113ec578063e75235b81461147d578063e86637db146114a857610231565b8063cc2f8452116100d1578063cc2f8452146110e8578063d4d9bdcd146111b5578063d8d11f78146111f0578063e009cfde1461132a57610231565b8063affed0e014610d94578063b4faba0914610dbf578063b63e800d14610ea7578063c4ca3a9c1461101757610231565b80635624b25b1161017a5780636a761202116101495780636a761202146109945780637d83297414610b50578063934f3a1114610bbf578063a0e67e2b14610d2857610231565b80635624b25b146107fb5780635ae6bd37146108b9578063610b592514610908578063694e80c31461095957610231565b80632f54bf6e116101b65780632f54bf6e146104d35780633408e4701461053a578063468721a7146105655780635229073f1461067a57610231565b80630d582f131461029e57806312fb68e0146102f95780632d9ad53d1461046c57610231565b36610231573373ffffffffffffffffffffffffffffffffffffffff167f3d0ce9bfc3ed7d6862dbb28b2dea94561fe714a1b4d019aa8af39730d1ad7c3d346040518082815260200191505060405180910390a2005b34801561023d57600080fd5b5060007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b905080548061027257600080f35b36600080373360601b365260008060143601600080855af13d6000803e80610299573d6000fd5b3d6000f35b3480156102aa57600080fd5b506102f7600480360360408110156102c157600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506117ce565b005b34801561030557600080fd5b5061046a6004803603608081101561031c57600080fd5b81019080803590602001909291908035906020019064010000000081111561034357600080fd5b82018360208201111561035557600080fd5b8035906020019184600183028401116401000000008311171561037757600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803590602001906401000000008111156103da57600080fd5b8201836020820111156103ec57600080fd5b8035906020019184600183028401116401000000008311171561040e57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190929190505050611bbe565b005b34801561047857600080fd5b506104bb6004803603602081101561048f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612440565b60405180821515815260200191505060405180910390f35b3480156104df57600080fd5b50610522600480360360208110156104f657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612512565b60405180821515815260200191505060405180910390f35b34801561054657600080fd5b5061054f6125e4565b6040518082815260200191505060405180910390f35b34801561057157600080fd5b506106626004803603608081101561058857600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156105cf57600080fd5b8201836020820111156105e157600080fd5b8035906020019184600183028401116401000000008311171561060357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506125f1565b60405180821515815260200191505060405180910390f35b34801561068657600080fd5b506107776004803603608081101561069d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156106e457600080fd5b8201836020820111156106f657600080fd5b8035906020019184600183028401116401000000008311171561071857600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506127d7565b60405180831515815260200180602001828103825283818151815260200191508051906020019080838360005b838110156107bf5780820151818401526020810190506107a4565b50505050905090810190601f1680156107ec5780820380516001836020036101000a031916815260200191505b50935050505060405180910390f35b34801561080757600080fd5b5061083e6004803603604081101561081e57600080fd5b81019080803590602001909291908035906020019092919050505061280d565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561087e578082015181840152602081019050610863565b50505050905090810190601f1680156108ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b3480156108c557600080fd5b506108f2600480360360208110156108dc57600080fd5b8101908080359060200190929190505050612894565b6040518082815260200191505060405180910390f35b34801561091457600080fd5b506109576004803603602081101561092b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff1690602001909291905050506128ac565b005b34801561096557600080fd5b506109926004803603602081101561097c57600080fd5b8101908080359060200190929190505050612c3e565b005b610b3860048036036101408110156109ab57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156109f257600080fd5b820183602082011115610a0457600080fd5b80359060200191846001830284011164010000000083111715610a2657600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610ab257600080fd5b820183602082011115610ac457600080fd5b80359060200191846001830284011164010000000083111715610ae657600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050612d78565b60405180821515815260200191505060405180910390f35b348015610b5c57600080fd5b50610ba960048036036040811015610b7357600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506132b5565b6040518082815260200191505060405180910390f35b348015610bcb57600080fd5b50610d2660048036036060811015610be257600080fd5b810190808035906020019092919080359060200190640100000000811115610c0957600080fd5b820183602082011115610c1b57600080fd5b80359060200191846001830284011164010000000083111715610c3d57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190640100000000811115610ca057600080fd5b820183602082011115610cb257600080fd5b80359060200191846001830284011164010000000083111715610cd457600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505091929192905050506132da565b005b348015610d3457600080fd5b50610d3d613369565b6040518080602001828103825283818151815260200191508051906020019060200280838360005b83811015610d80578082015181840152602081019050610d65565b505050509050019250505060405180910390f35b348015610da057600080fd5b50610da9613512565b6040518082815260200191505060405180910390f35b348015610dcb57600080fd5b50610ea560048036036040811015610de257600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610e1f57600080fd5b820183602082011115610e3157600080fd5b80359060200191846001830284011164010000000083111715610e5357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050613518565b005b348015610eb357600080fd5b506110156004803603610100811015610ecb57600080fd5b8101908080359060200190640100000000811115610ee857600080fd5b820183602082011115610efa57600080fd5b80359060200191846020830284011164010000000083111715610f1c57600080fd5b909192939192939080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610f6757600080fd5b820183602082011115610f7957600080fd5b80359060200191846001830284011164010000000083111715610f9b57600080fd5b9091929391929390803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919050505061353a565b005b34801561102357600080fd5b506110d26004803603608081101561103a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561108157600080fd5b82018360208201111561109357600080fd5b803590602001918460018302840111640100000000831117156110b557600080fd5b9091929391929390803560ff1690602001909291905050506136f8565b6040518082815260200191505060405180910390f35b3480156110f457600080fd5b506111416004803603604081101561110b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613820565b60405180806020018373ffffffffffffffffffffffffffffffffffffffff168152602001828103825284818151815260200191508051906020019060200280838360005b838110156111a0578082015181840152602081019050611185565b50505050905001935050505060405180910390f35b3480156111c157600080fd5b506111ee600480360360208110156111d857600080fd5b8101908080359060200190929190505050613a12565b005b3480156111fc57600080fd5b50611314600480360361014081101561121457600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561125b57600080fd5b82018360208201111561126d57600080fd5b8035906020019184600183028401116401000000008311171561128f57600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613bb1565b6040518082815260200191505060405180910390f35b34801561133657600080fd5b506113996004803603604081101561134d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613bde565b005b3480156113a757600080fd5b506113ea600480360360208110156113be57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613f6f565b005b3480156113f857600080fd5b5061147b6004803603606081101561140f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613ff3565b005b34801561148957600080fd5b50611492614665565b6040518082815260200191505060405180910390f35b3480156114b457600080fd5b506115cc60048036036101408110156114cc57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561151357600080fd5b82018360208201111561152557600080fd5b8035906020019184600183028401116401000000008311171561154757600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff1690602001909291908035906020019092919050505061466f565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561160c5780820151818401526020810190506115f1565b50505050905090810190601f1680156116395780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b34801561165357600080fd5b506116966004803603602081101561166a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050614817565b005b3480156116a457600080fd5b506116ad614878565b6040518082815260200191505060405180910390f35b3480156116cf57600080fd5b5061173c600480360360608110156116e657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506148f6565b005b34801561174a57600080fd5b50611753614d29565b6040518080602001828103825283818151815260200191508051906020019080838360005b83811015611793578082015181840152602081019050611778565b50505050905090810190601f1680156117c05780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6117d6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156118405750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b801561187857503073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6118ea576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146119eb576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508160026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506003600081548092919060010191905055507f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2682604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414611bba57611bb981612c3e565b5b5050565b611bd2604182614e0590919063ffffffff16565b82511015611c48576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6000808060008060005b8681101561243457611c648882614e3f565b80945081955082965050505060008460ff16141561206d578260001c9450611c96604188614e0590919063ffffffff16565b8260001c1015611d0e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8751611d2760208460001c614e6e90919063ffffffff16565b1115611d9b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006020838a01015190508851611dd182611dc360208760001c614e6e90919063ffffffff16565b614e6e90919063ffffffff16565b1115611e45576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60606020848b010190506320c13b0b60e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168773ffffffffffffffffffffffffffffffffffffffff166320c13b0b8d846040518363ffffffff1660e01b8152600401808060200180602001838103835285818151815260200191508051906020019080838360005b83811015611ee7578082015181840152602081019050611ecc565b50505050905090810190601f168015611f145780820380516001836020036101000a031916815260200191505b50838103825284818151815260200191508051906020019080838360005b83811015611f4d578082015181840152602081019050611f32565b50505050905090810190601f168015611f7a5780820380516001836020036101000a031916815260200191505b5094505050505060206040518083038186803b158015611f9957600080fd5b505afa158015611fad573d6000803e3d6000fd5b505050506040513d6020811015611fc357600080fd5b81019080805190602001909291905050507bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614612066576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b50506122b2565b60018460ff161415612181578260001c94508473ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16148061210a57506000600860008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008c81526020019081526020016000205414155b61217c576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6122b1565b601e8460ff1611156122495760018a60405160200180807f19457468657265756d205369676e6564204d6573736167653a0a333200000000815250601c018281526020019150506040516020818303038152906040528051906020012060048603858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa158015612238573d6000803e3d6000fd5b5050506020604051035194506122b0565b60018a85858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa1580156122a3573d6000803e3d6000fd5b5050506020604051035194505b5b5b8573ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff161180156123795750600073ffffffffffffffffffffffffffffffffffffffff16600260008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b80156123b25750600173ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff1614155b612424576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323600000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8495508080600101915050611c52565b50505050505050505050565b60008173ffffffffffffffffffffffffffffffffffffffff16600173ffffffffffffffffffffffffffffffffffffffff161415801561250b5750600073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156125dd5750600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000804690508091505090565b6000600173ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141580156126bc5750600073ffffffffffffffffffffffffffffffffffffffff16600160003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b61272e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61273b858585855a614e8d565b9050801561278b573373ffffffffffffffffffffffffffffffffffffffff167f6895c13664aa4f67288b25d7a21d7aaa34916e355fb9b6fae0a139a9085becb860405160405180910390a26127cf565b3373ffffffffffffffffffffffffffffffffffffffff167facd2c8702804128fdb0db2bb49f6d127dd0181c13fd45dbfe16de0930e2bd37560405160405180910390a25b949350505050565b600060606127e7868686866125f1565b915060405160203d0181016040523d81523d6000602083013e8091505094509492505050565b606060006020830267ffffffffffffffff8111801561282b57600080fd5b506040519080825280601f01601f19166020018201604052801561285e5781602001600182028036833780820191505090505b50905060005b8381101561288957808501548060208302602085010152508080600101915050612864565b508091505092915050565b60076020528060005260406000206000915090505481565b6128b4614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561291e5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b612990576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614612a91576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508060016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507fecdf3a3effea5783a3c4c2140e677577666428d44ed9d474a0b3a4c9943f844081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b612c46614d62565b600354811115612cbe576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001811015612d35576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b806004819055507f610f7ff2b304ae8903c3de74c60c6ab1f7d6226b3f52c5161905bb5ad4039c936004546040518082815260200191505060405180910390a150565b6000806000612d928e8e8e8e8e8e8e8e8e8e60055461466f565b905060056000815480929190600101919050555080805190602001209150612dbb8282866132da565b506000612dc6614ed9565b9050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614612fac578073ffffffffffffffffffffffffffffffffffffffff166375f0bb528f8f8f8f8f8f8f8f8f8f8f336040518d63ffffffff1660e01b8152600401808d73ffffffffffffffffffffffffffffffffffffffff1681526020018c8152602001806020018a6001811115612e6957fe5b81526020018981526020018881526020018781526020018673ffffffffffffffffffffffffffffffffffffffff1681526020018573ffffffffffffffffffffffffffffffffffffffff168152602001806020018473ffffffffffffffffffffffffffffffffffffffff16815260200183810383528d8d82818152602001925080828437600081840152601f19601f820116905080830192505050838103825285818151815260200191508051906020019080838360005b83811015612f3b578082015181840152602081019050612f20565b50505050905090810190601f168015612f685780820380516001836020036101000a031916815260200191505b509e505050505050505050505050505050600060405180830381600087803b158015612f9357600080fd5b505af1158015612fa7573d6000803e3d6000fd5b505050505b6101f4612fd36109c48b01603f60408d0281612fc457fe5b04614f0a90919063ffffffff16565b015a1015613049576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60005a90506130b28f8f8f8f8080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050508e60008d146130a7578e6130ad565b6109c45a035b614e8d565b93506130c75a82614f2490919063ffffffff16565b905083806130d6575060008a14155b806130e2575060008814155b613154576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60008089111561316e5761316b828b8b8b8b614f44565b90505b84156131b8577f442e715f626346e8c54381002da614f62bee8d27386535b2521ec8540898556e8482604051808381526020018281526020019250505060405180910390a16131f8565b7f23428b18acfb3ea64b08dc0c1d296ea9c09702c09083ca5272e64d115b687d238482604051808381526020018281526020019250505060405180910390a15b5050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16146132a4578073ffffffffffffffffffffffffffffffffffffffff16639327136883856040518363ffffffff1660e01b815260040180838152602001821515815260200192505050600060405180830381600087803b15801561328b57600080fd5b505af115801561329f573d6000803e3d6000fd5b505050505b50509b9a5050505050505050505050565b6008602052816000526040600020602052806000526040600020600091509150505481565b6000600454905060008111613357576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61336384848484611bbe565b50505050565b6060600060035467ffffffffffffffff8111801561338657600080fd5b506040519080825280602002602001820160405280156133b55781602001602082028036833780820191505090505b50905060008060026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614613509578083838151811061346057fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600260008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050818060010192505061341f565b82935050505090565b60055481565b600080825160208401855af4806000523d6020523d600060403e60403d016000fd5b6135858a8a80806020026020016040519081016040528093929190818152602001838360200280828437600081840152601f19601f820116905080830192505050505050508961514a565b600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16146135c3576135c28461564a565b5b6136118787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050615679565b600082111561362b5761362982600060018685614f44565b505b3373ffffffffffffffffffffffffffffffffffffffff167f141df868a6331af528e38c83b7aa03edc19be66e37ae67f9285bf4f8e3c6a1a88b8b8b8b8960405180806020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281038252878782818152602001925060200280828437600081840152601f19601f820116905080830192505050965050505050505060405180910390a250505050505050505050565b6000805a905061374f878787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050865a614e8d565b61375857600080fd5b60005a8203905080604051602001808281526020019150506040516020818303038152906040526040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825283818151815260200191508051906020019080838360005b838110156137e55780820151818401526020810190506137ca565b50505050905090810190601f1680156138125780820380516001836020036101000a031916815260200191505b509250505060405180910390fd5b606060008267ffffffffffffffff8111801561383b57600080fd5b5060405190808252806020026020018201604052801561386a5781602001602082028036833780820191505090505b509150600080600160008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561393d5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561394857508482105b15613a03578084838151811061395a57fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16905081806001019250506138d3565b80925081845250509250929050565b600073ffffffffffffffffffffffffffffffffffffffff16600260003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161415613b14576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001600860003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020016000206000838152602001908152602001600020819055503373ffffffffffffffffffffffffffffffffffffffff16817ff2a0eb156472d1440255b0d7c1e19cc07115d1051fe605b0dce69acfec884d9c60405160405180910390a350565b6000613bc68c8c8c8c8c8c8c8c8c8c8c61466f565b8051906020012090509b9a5050505050505050505050565b613be6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614158015613c505750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b613cc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614613dc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507faab4fa2b463f581b2b32cb3b7e3b704b9ce37cc209b5fb4d77e593ace405427681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613f77614d62565b60007f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b90508181557f1151116914515bc0891ff9047a6cb32cf902546f83066499bcf8ba33d2353fa282604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613ffb614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156140655750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561409d57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b61410f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614210576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff161415801561427a5750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6142ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146143ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555080600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a17f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a1505050565b6000600454905090565b606060007fbb8310d486368db6bd6f849402fdd73ad53d316b5a4b2644ad6efe0f941286d860001b8d8d8d8d60405180838380828437808301925050509250505060405180910390208c8c8c8c8c8c8c604051602001808c81526020018b73ffffffffffffffffffffffffffffffffffffffff1681526020018a815260200189815260200188600181111561470057fe5b81526020018781526020018681526020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281526020019b505050505050505050505050604051602081830303815290604052805190602001209050601960f81b600160f81b61478c614878565b8360405160200180857effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168152600101847effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff191681526001018381526020018281526020019450505050506040516020818303038152906040529150509b9a5050505050505050505050565b61481f614d62565b6148288161564a565b7f5ac6c46c93c8d0e53714ba3b53db3e7c046da994313d7ed0d192028bc7c228b081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b60007f47e79534a245952e8b16893a336b85a3d9ea9fa8c573f3d803afb92a7946921860001b6148a66125e4565b30604051602001808481526020018381526020018273ffffffffffffffffffffffffffffffffffffffff168152602001935050505060405160208183030381529060405280519060200120905090565b6148fe614d62565b806001600354031015614979576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156149e35750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b614a55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614b55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600360008154809291906001900391905055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414614d2457614d2381612c3e565b5b505050565b6040518060400160405280600581526020017f312e332e3000000000000000000000000000000000000000000000000000000081525081565b3073ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff1614614e03576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b565b600080831415614e185760009050614e39565b6000828402905082848281614e2957fe5b0414614e3457600080fd5b809150505b92915050565b60008060008360410260208101860151925060408101860151915060ff60418201870151169350509250925092565b600080828401905083811015614e8357600080fd5b8091505092915050565b6000600180811115614e9b57fe5b836001811115614ea757fe5b1415614ec0576000808551602087018986f49050614ed0565b600080855160208701888a87f190505b95945050505050565b6000807f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b9050805491505090565b600081831015614f1a5781614f1c565b825b905092915050565b600082821115614f3357600080fd5b600082840390508091505092915050565b600080600073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614614f815782614f83565b325b9050600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16141561509b57614fed3a8610614fca573a614fcc565b855b614fdf888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91508073ffffffffffffffffffffffffffffffffffffffff166108fc839081150290604051600060405180830381858888f19350505050615096576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b615140565b6150c0856150b2888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91506150cd8482846158b4565b61513f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5095945050505050565b6000600454146151c2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8151811115615239576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60018110156152b0576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006001905060005b83518110156155b65760008482815181106152d057fe5b60200260200101519050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156153445750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561537c57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b80156153b457508073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614155b615426576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614615527576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b80600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508092505080806001019150506152b9565b506001600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550825160038190555081600481905550505050565b60007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b90508181555050565b600073ffffffffffffffffffffffffffffffffffffffff1660016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161461577b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001806000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16146158b05761583d8260008360015a614e8d565b6158af576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5050565b60008063a9059cbb8484604051602401808373ffffffffffffffffffffffffffffffffffffffff168152602001828152602001925050506040516020818303038152906040529060e01b6020820180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff83818316178352505050509050602060008251602084016000896127105a03f13d6000811461595b5760208114615963576000935061596e565b81935061596e565b600051158215171593505b505050939250505056fea26469706673582212203874bcf92e1722cc7bfa0cef1a0985cf0dc3485ba0663db3747ccdf1605df53464736f6c63430007060033"
                 ),
                 "to": "0x4e59b44847b379578588920cA78FbF26c0B4956C",
             },
-            "blockHash": "0x4160d3b92f3678386a108e0838016dd3010ba12389712a30f2b017d33799d05e",
+            "blockHash": HexBytes(
+                "0x4160d3b92f3678386a108e0838016dd3010ba12389712a30f2b017d33799d05e"
+            ),
             "blockNumber": 12504268,
             "result": {
                 "gasUsed": 4660797,
                 "output": HexBytes("0xd9db270c1b5e3bd161e8c8503c55ceabee709552"),
             },
             "subtraces": 1,
             "traceAddress": [],
-            "transactionHash": "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f",
+            "transactionHash": HexBytes(
+                "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f"
+            ),
             "transactionPosition": 12,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x4e59b44847b379578588920cA78FbF26c0B4956C",
                 "gas": 4619079,
                 "value": 0,
                 "init": HexBytes(
                     "0x608060405234801561001057600080fd5b5060016004819055506159ae80620000296000396000f3fe6080604052600436106101dc5760003560e01c8063affed0e011610102578063e19a9dd911610095578063f08a032311610064578063f08a032314611647578063f698da2514611698578063f8dc5dd9146116c3578063ffa1ad741461173e57610231565b8063e19a9dd91461139b578063e318b52b146113ec578063e75235b81461147d578063e86637db146114a857610231565b8063cc2f8452116100d1578063cc2f8452146110e8578063d4d9bdcd146111b5578063d8d11f78146111f0578063e009cfde1461132a57610231565b8063affed0e014610d94578063b4faba0914610dbf578063b63e800d14610ea7578063c4ca3a9c1461101757610231565b80635624b25b1161017a5780636a761202116101495780636a761202146109945780637d83297414610b50578063934f3a1114610bbf578063a0e67e2b14610d2857610231565b80635624b25b146107fb5780635ae6bd37146108b9578063610b592514610908578063694e80c31461095957610231565b80632f54bf6e116101b65780632f54bf6e146104d35780633408e4701461053a578063468721a7146105655780635229073f1461067a57610231565b80630d582f131461029e57806312fb68e0146102f95780632d9ad53d1461046c57610231565b36610231573373ffffffffffffffffffffffffffffffffffffffff167f3d0ce9bfc3ed7d6862dbb28b2dea94561fe714a1b4d019aa8af39730d1ad7c3d346040518082815260200191505060405180910390a2005b34801561023d57600080fd5b5060007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b905080548061027257600080f35b36600080373360601b365260008060143601600080855af13d6000803e80610299573d6000fd5b3d6000f35b3480156102aa57600080fd5b506102f7600480360360408110156102c157600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506117ce565b005b34801561030557600080fd5b5061046a6004803603608081101561031c57600080fd5b81019080803590602001909291908035906020019064010000000081111561034357600080fd5b82018360208201111561035557600080fd5b8035906020019184600183028401116401000000008311171561037757600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803590602001906401000000008111156103da57600080fd5b8201836020820111156103ec57600080fd5b8035906020019184600183028401116401000000008311171561040e57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190929190505050611bbe565b005b34801561047857600080fd5b506104bb6004803603602081101561048f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612440565b60405180821515815260200191505060405180910390f35b3480156104df57600080fd5b50610522600480360360208110156104f657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612512565b60405180821515815260200191505060405180910390f35b34801561054657600080fd5b5061054f6125e4565b6040518082815260200191505060405180910390f35b34801561057157600080fd5b506106626004803603608081101561058857600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156105cf57600080fd5b8201836020820111156105e157600080fd5b8035906020019184600183028401116401000000008311171561060357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506125f1565b60405180821515815260200191505060405180910390f35b34801561068657600080fd5b506107776004803603608081101561069d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156106e457600080fd5b8201836020820111156106f657600080fd5b8035906020019184600183028401116401000000008311171561071857600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506127d7565b60405180831515815260200180602001828103825283818151815260200191508051906020019080838360005b838110156107bf5780820151818401526020810190506107a4565b50505050905090810190601f1680156107ec5780820380516001836020036101000a031916815260200191505b50935050505060405180910390f35b34801561080757600080fd5b5061083e6004803603604081101561081e57600080fd5b81019080803590602001909291908035906020019092919050505061280d565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561087e578082015181840152602081019050610863565b50505050905090810190601f1680156108ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b3480156108c557600080fd5b506108f2600480360360208110156108dc57600080fd5b8101908080359060200190929190505050612894565b6040518082815260200191505060405180910390f35b34801561091457600080fd5b506109576004803603602081101561092b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff1690602001909291905050506128ac565b005b34801561096557600080fd5b506109926004803603602081101561097c57600080fd5b8101908080359060200190929190505050612c3e565b005b610b3860048036036101408110156109ab57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156109f257600080fd5b820183602082011115610a0457600080fd5b80359060200191846001830284011164010000000083111715610a2657600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610ab257600080fd5b820183602082011115610ac457600080fd5b80359060200191846001830284011164010000000083111715610ae657600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050612d78565b60405180821515815260200191505060405180910390f35b348015610b5c57600080fd5b50610ba960048036036040811015610b7357600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506132b5565b6040518082815260200191505060405180910390f35b348015610bcb57600080fd5b50610d2660048036036060811015610be257600080fd5b810190808035906020019092919080359060200190640100000000811115610c0957600080fd5b820183602082011115610c1b57600080fd5b80359060200191846001830284011164010000000083111715610c3d57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190640100000000811115610ca057600080fd5b820183602082011115610cb257600080fd5b80359060200191846001830284011164010000000083111715610cd457600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505091929192905050506132da565b005b348015610d3457600080fd5b50610d3d613369565b6040518080602001828103825283818151815260200191508051906020019060200280838360005b83811015610d80578082015181840152602081019050610d65565b505050509050019250505060405180910390f35b348015610da057600080fd5b50610da9613512565b6040518082815260200191505060405180910390f35b348015610dcb57600080fd5b50610ea560048036036040811015610de257600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610e1f57600080fd5b820183602082011115610e3157600080fd5b80359060200191846001830284011164010000000083111715610e5357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050613518565b005b348015610eb357600080fd5b506110156004803603610100811015610ecb57600080fd5b8101908080359060200190640100000000811115610ee857600080fd5b820183602082011115610efa57600080fd5b80359060200191846020830284011164010000000083111715610f1c57600080fd5b909192939192939080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610f6757600080fd5b820183602082011115610f7957600080fd5b80359060200191846001830284011164010000000083111715610f9b57600080fd5b9091929391929390803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919050505061353a565b005b34801561102357600080fd5b506110d26004803603608081101561103a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561108157600080fd5b82018360208201111561109357600080fd5b803590602001918460018302840111640100000000831117156110b557600080fd5b9091929391929390803560ff1690602001909291905050506136f8565b6040518082815260200191505060405180910390f35b3480156110f457600080fd5b506111416004803603604081101561110b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613820565b60405180806020018373ffffffffffffffffffffffffffffffffffffffff168152602001828103825284818151815260200191508051906020019060200280838360005b838110156111a0578082015181840152602081019050611185565b50505050905001935050505060405180910390f35b3480156111c157600080fd5b506111ee600480360360208110156111d857600080fd5b8101908080359060200190929190505050613a12565b005b3480156111fc57600080fd5b50611314600480360361014081101561121457600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561125b57600080fd5b82018360208201111561126d57600080fd5b8035906020019184600183028401116401000000008311171561128f57600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613bb1565b6040518082815260200191505060405180910390f35b34801561133657600080fd5b506113996004803603604081101561134d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613bde565b005b3480156113a757600080fd5b506113ea600480360360208110156113be57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613f6f565b005b3480156113f857600080fd5b5061147b6004803603606081101561140f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613ff3565b005b34801561148957600080fd5b50611492614665565b6040518082815260200191505060405180910390f35b3480156114b457600080fd5b506115cc60048036036101408110156114cc57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561151357600080fd5b82018360208201111561152557600080fd5b8035906020019184600183028401116401000000008311171561154757600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff1690602001909291908035906020019092919050505061466f565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561160c5780820151818401526020810190506115f1565b50505050905090810190601f1680156116395780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b34801561165357600080fd5b506116966004803603602081101561166a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050614817565b005b3480156116a457600080fd5b506116ad614878565b6040518082815260200191505060405180910390f35b3480156116cf57600080fd5b5061173c600480360360608110156116e657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506148f6565b005b34801561174a57600080fd5b50611753614d29565b6040518080602001828103825283818151815260200191508051906020019080838360005b83811015611793578082015181840152602081019050611778565b50505050905090810190601f1680156117c05780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6117d6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156118405750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b801561187857503073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6118ea576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146119eb576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508160026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506003600081548092919060010191905055507f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2682604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414611bba57611bb981612c3e565b5b5050565b611bd2604182614e0590919063ffffffff16565b82511015611c48576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6000808060008060005b8681101561243457611c648882614e3f565b80945081955082965050505060008460ff16141561206d578260001c9450611c96604188614e0590919063ffffffff16565b8260001c1015611d0e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8751611d2760208460001c614e6e90919063ffffffff16565b1115611d9b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006020838a01015190508851611dd182611dc360208760001c614e6e90919063ffffffff16565b614e6e90919063ffffffff16565b1115611e45576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60606020848b010190506320c13b0b60e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168773ffffffffffffffffffffffffffffffffffffffff166320c13b0b8d846040518363ffffffff1660e01b8152600401808060200180602001838103835285818151815260200191508051906020019080838360005b83811015611ee7578082015181840152602081019050611ecc565b50505050905090810190601f168015611f145780820380516001836020036101000a031916815260200191505b50838103825284818151815260200191508051906020019080838360005b83811015611f4d578082015181840152602081019050611f32565b50505050905090810190601f168015611f7a5780820380516001836020036101000a031916815260200191505b5094505050505060206040518083038186803b158015611f9957600080fd5b505afa158015611fad573d6000803e3d6000fd5b505050506040513d6020811015611fc357600080fd5b81019080805190602001909291905050507bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614612066576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b50506122b2565b60018460ff161415612181578260001c94508473ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16148061210a57506000600860008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008c81526020019081526020016000205414155b61217c576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6122b1565b601e8460ff1611156122495760018a60405160200180807f19457468657265756d205369676e6564204d6573736167653a0a333200000000815250601c018281526020019150506040516020818303038152906040528051906020012060048603858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa158015612238573d6000803e3d6000fd5b5050506020604051035194506122b0565b60018a85858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa1580156122a3573d6000803e3d6000fd5b5050506020604051035194505b5b5b8573ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff161180156123795750600073ffffffffffffffffffffffffffffffffffffffff16600260008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b80156123b25750600173ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff1614155b612424576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323600000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8495508080600101915050611c52565b50505050505050505050565b60008173ffffffffffffffffffffffffffffffffffffffff16600173ffffffffffffffffffffffffffffffffffffffff161415801561250b5750600073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156125dd5750600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000804690508091505090565b6000600173ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141580156126bc5750600073ffffffffffffffffffffffffffffffffffffffff16600160003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b61272e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61273b858585855a614e8d565b9050801561278b573373ffffffffffffffffffffffffffffffffffffffff167f6895c13664aa4f67288b25d7a21d7aaa34916e355fb9b6fae0a139a9085becb860405160405180910390a26127cf565b3373ffffffffffffffffffffffffffffffffffffffff167facd2c8702804128fdb0db2bb49f6d127dd0181c13fd45dbfe16de0930e2bd37560405160405180910390a25b949350505050565b600060606127e7868686866125f1565b915060405160203d0181016040523d81523d6000602083013e8091505094509492505050565b606060006020830267ffffffffffffffff8111801561282b57600080fd5b506040519080825280601f01601f19166020018201604052801561285e5781602001600182028036833780820191505090505b50905060005b8381101561288957808501548060208302602085010152508080600101915050612864565b508091505092915050565b60076020528060005260406000206000915090505481565b6128b4614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561291e5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b612990576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614612a91576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508060016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507fecdf3a3effea5783a3c4c2140e677577666428d44ed9d474a0b3a4c9943f844081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b612c46614d62565b600354811115612cbe576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001811015612d35576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b806004819055507f610f7ff2b304ae8903c3de74c60c6ab1f7d6226b3f52c5161905bb5ad4039c936004546040518082815260200191505060405180910390a150565b6000806000612d928e8e8e8e8e8e8e8e8e8e60055461466f565b905060056000815480929190600101919050555080805190602001209150612dbb8282866132da565b506000612dc6614ed9565b9050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614612fac578073ffffffffffffffffffffffffffffffffffffffff166375f0bb528f8f8f8f8f8f8f8f8f8f8f336040518d63ffffffff1660e01b8152600401808d73ffffffffffffffffffffffffffffffffffffffff1681526020018c8152602001806020018a6001811115612e6957fe5b81526020018981526020018881526020018781526020018673ffffffffffffffffffffffffffffffffffffffff1681526020018573ffffffffffffffffffffffffffffffffffffffff168152602001806020018473ffffffffffffffffffffffffffffffffffffffff16815260200183810383528d8d82818152602001925080828437600081840152601f19601f820116905080830192505050838103825285818151815260200191508051906020019080838360005b83811015612f3b578082015181840152602081019050612f20565b50505050905090810190601f168015612f685780820380516001836020036101000a031916815260200191505b509e505050505050505050505050505050600060405180830381600087803b158015612f9357600080fd5b505af1158015612fa7573d6000803e3d6000fd5b505050505b6101f4612fd36109c48b01603f60408d0281612fc457fe5b04614f0a90919063ffffffff16565b015a1015613049576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60005a90506130b28f8f8f8f8080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050508e60008d146130a7578e6130ad565b6109c45a035b614e8d565b93506130c75a82614f2490919063ffffffff16565b905083806130d6575060008a14155b806130e2575060008814155b613154576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60008089111561316e5761316b828b8b8b8b614f44565b90505b84156131b8577f442e715f626346e8c54381002da614f62bee8d27386535b2521ec8540898556e8482604051808381526020018281526020019250505060405180910390a16131f8565b7f23428b18acfb3ea64b08dc0c1d296ea9c09702c09083ca5272e64d115b687d238482604051808381526020018281526020019250505060405180910390a15b5050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16146132a4578073ffffffffffffffffffffffffffffffffffffffff16639327136883856040518363ffffffff1660e01b815260040180838152602001821515815260200192505050600060405180830381600087803b15801561328b57600080fd5b505af115801561329f573d6000803e3d6000fd5b505050505b50509b9a5050505050505050505050565b6008602052816000526040600020602052806000526040600020600091509150505481565b6000600454905060008111613357576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61336384848484611bbe565b50505050565b6060600060035467ffffffffffffffff8111801561338657600080fd5b506040519080825280602002602001820160405280156133b55781602001602082028036833780820191505090505b50905060008060026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614613509578083838151811061346057fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600260008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050818060010192505061341f565b82935050505090565b60055481565b600080825160208401855af4806000523d6020523d600060403e60403d016000fd5b6135858a8a80806020026020016040519081016040528093929190818152602001838360200280828437600081840152601f19601f820116905080830192505050505050508961514a565b600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16146135c3576135c28461564a565b5b6136118787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050615679565b600082111561362b5761362982600060018685614f44565b505b3373ffffffffffffffffffffffffffffffffffffffff167f141df868a6331af528e38c83b7aa03edc19be66e37ae67f9285bf4f8e3c6a1a88b8b8b8b8960405180806020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281038252878782818152602001925060200280828437600081840152601f19601f820116905080830192505050965050505050505060405180910390a250505050505050505050565b6000805a905061374f878787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050865a614e8d565b61375857600080fd5b60005a8203905080604051602001808281526020019150506040516020818303038152906040526040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825283818151815260200191508051906020019080838360005b838110156137e55780820151818401526020810190506137ca565b50505050905090810190601f1680156138125780820380516001836020036101000a031916815260200191505b509250505060405180910390fd5b606060008267ffffffffffffffff8111801561383b57600080fd5b5060405190808252806020026020018201604052801561386a5781602001602082028036833780820191505090505b509150600080600160008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561393d5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561394857508482105b15613a03578084838151811061395a57fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16905081806001019250506138d3565b80925081845250509250929050565b600073ffffffffffffffffffffffffffffffffffffffff16600260003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161415613b14576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001600860003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020016000206000838152602001908152602001600020819055503373ffffffffffffffffffffffffffffffffffffffff16817ff2a0eb156472d1440255b0d7c1e19cc07115d1051fe605b0dce69acfec884d9c60405160405180910390a350565b6000613bc68c8c8c8c8c8c8c8c8c8c8c61466f565b8051906020012090509b9a5050505050505050505050565b613be6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614158015613c505750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b613cc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614613dc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507faab4fa2b463f581b2b32cb3b7e3b704b9ce37cc209b5fb4d77e593ace405427681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613f77614d62565b60007f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b90508181557f1151116914515bc0891ff9047a6cb32cf902546f83066499bcf8ba33d2353fa282604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613ffb614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156140655750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561409d57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b61410f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614210576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff161415801561427a5750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6142ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146143ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555080600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a17f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a1505050565b6000600454905090565b606060007fbb8310d486368db6bd6f849402fdd73ad53d316b5a4b2644ad6efe0f941286d860001b8d8d8d8d60405180838380828437808301925050509250505060405180910390208c8c8c8c8c8c8c604051602001808c81526020018b73ffffffffffffffffffffffffffffffffffffffff1681526020018a815260200189815260200188600181111561470057fe5b81526020018781526020018681526020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281526020019b505050505050505050505050604051602081830303815290604052805190602001209050601960f81b600160f81b61478c614878565b8360405160200180857effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168152600101847effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff191681526001018381526020018281526020019450505050506040516020818303038152906040529150509b9a5050505050505050505050565b61481f614d62565b6148288161564a565b7f5ac6c46c93c8d0e53714ba3b53db3e7c046da994313d7ed0d192028bc7c228b081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b60007f47e79534a245952e8b16893a336b85a3d9ea9fa8c573f3d803afb92a7946921860001b6148a66125e4565b30604051602001808481526020018381526020018273ffffffffffffffffffffffffffffffffffffffff168152602001935050505060405160208183030381529060405280519060200120905090565b6148fe614d62565b806001600354031015614979576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156149e35750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b614a55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614b55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600360008154809291906001900391905055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414614d2457614d2381612c3e565b5b505050565b6040518060400160405280600581526020017f312e332e3000000000000000000000000000000000000000000000000000000081525081565b3073ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff1614614e03576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b565b600080831415614e185760009050614e39565b6000828402905082848281614e2957fe5b0414614e3457600080fd5b809150505b92915050565b60008060008360410260208101860151925060408101860151915060ff60418201870151169350509250925092565b600080828401905083811015614e8357600080fd5b8091505092915050565b6000600180811115614e9b57fe5b836001811115614ea757fe5b1415614ec0576000808551602087018986f49050614ed0565b600080855160208701888a87f190505b95945050505050565b6000807f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b9050805491505090565b600081831015614f1a5781614f1c565b825b905092915050565b600082821115614f3357600080fd5b600082840390508091505092915050565b600080600073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614614f815782614f83565b325b9050600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16141561509b57614fed3a8610614fca573a614fcc565b855b614fdf888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91508073ffffffffffffffffffffffffffffffffffffffff166108fc839081150290604051600060405180830381858888f19350505050615096576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b615140565b6150c0856150b2888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91506150cd8482846158b4565b61513f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5095945050505050565b6000600454146151c2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8151811115615239576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60018110156152b0576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006001905060005b83518110156155b65760008482815181106152d057fe5b60200260200101519050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156153445750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561537c57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b80156153b457508073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614155b615426576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614615527576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b80600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508092505080806001019150506152b9565b506001600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550825160038190555081600481905550505050565b60007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b90508181555050565b600073ffffffffffffffffffffffffffffffffffffffff1660016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161461577b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001806000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16146158b05761583d8260008360015a614e8d565b6158af576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5050565b60008063a9059cbb8484604051602401808373ffffffffffffffffffffffffffffffffffffffff168152602001828152602001925050506040516020818303038152906040529060e01b6020820180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff83818316178352505050509050602060008251602084016000896127105a03f13d6000811461595b5760208114615963576000935061596e565b81935061596e565b600051158215171593505b505050939250505056fea26469706673582212203874bcf92e1722cc7bfa0cef1a0985cf0dc3485ba0663db3747ccdf1605df53464736f6c63430007060033"
                 ),
             },
-            "blockHash": "0x4160d3b92f3678386a108e0838016dd3010ba12389712a30f2b017d33799d05e",
+            "blockHash": HexBytes(
+                "0x4160d3b92f3678386a108e0838016dd3010ba12389712a30f2b017d33799d05e"
+            ),
             "blockNumber": 12504268,
             "result": {
                 "gasUsed": 4619079,
                 "code": HexBytes(
                     "0x6080604052600436106101dc5760003560e01c8063affed0e011610102578063e19a9dd911610095578063f08a032311610064578063f08a032314611647578063f698da2514611698578063f8dc5dd9146116c3578063ffa1ad741461173e57610231565b8063e19a9dd91461139b578063e318b52b146113ec578063e75235b81461147d578063e86637db146114a857610231565b8063cc2f8452116100d1578063cc2f8452146110e8578063d4d9bdcd146111b5578063d8d11f78146111f0578063e009cfde1461132a57610231565b8063affed0e014610d94578063b4faba0914610dbf578063b63e800d14610ea7578063c4ca3a9c1461101757610231565b80635624b25b1161017a5780636a761202116101495780636a761202146109945780637d83297414610b50578063934f3a1114610bbf578063a0e67e2b14610d2857610231565b80635624b25b146107fb5780635ae6bd37146108b9578063610b592514610908578063694e80c31461095957610231565b80632f54bf6e116101b65780632f54bf6e146104d35780633408e4701461053a578063468721a7146105655780635229073f1461067a57610231565b80630d582f131461029e57806312fb68e0146102f95780632d9ad53d1461046c57610231565b36610231573373ffffffffffffffffffffffffffffffffffffffff167f3d0ce9bfc3ed7d6862dbb28b2dea94561fe714a1b4d019aa8af39730d1ad7c3d346040518082815260200191505060405180910390a2005b34801561023d57600080fd5b5060007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b905080548061027257600080f35b36600080373360601b365260008060143601600080855af13d6000803e80610299573d6000fd5b3d6000f35b3480156102aa57600080fd5b506102f7600480360360408110156102c157600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506117ce565b005b34801561030557600080fd5b5061046a6004803603608081101561031c57600080fd5b81019080803590602001909291908035906020019064010000000081111561034357600080fd5b82018360208201111561035557600080fd5b8035906020019184600183028401116401000000008311171561037757600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803590602001906401000000008111156103da57600080fd5b8201836020820111156103ec57600080fd5b8035906020019184600183028401116401000000008311171561040e57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190929190505050611bbe565b005b34801561047857600080fd5b506104bb6004803603602081101561048f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612440565b60405180821515815260200191505060405180910390f35b3480156104df57600080fd5b50610522600480360360208110156104f657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050612512565b60405180821515815260200191505060405180910390f35b34801561054657600080fd5b5061054f6125e4565b6040518082815260200191505060405180910390f35b34801561057157600080fd5b506106626004803603608081101561058857600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156105cf57600080fd5b8201836020820111156105e157600080fd5b8035906020019184600183028401116401000000008311171561060357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506125f1565b60405180821515815260200191505060405180910390f35b34801561068657600080fd5b506107776004803603608081101561069d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156106e457600080fd5b8201836020820111156106f657600080fd5b8035906020019184600183028401116401000000008311171561071857600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290803560ff1690602001909291905050506127d7565b60405180831515815260200180602001828103825283818151815260200191508051906020019080838360005b838110156107bf5780820151818401526020810190506107a4565b50505050905090810190601f1680156107ec5780820380516001836020036101000a031916815260200191505b50935050505060405180910390f35b34801561080757600080fd5b5061083e6004803603604081101561081e57600080fd5b81019080803590602001909291908035906020019092919050505061280d565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561087e578082015181840152602081019050610863565b50505050905090810190601f1680156108ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b3480156108c557600080fd5b506108f2600480360360208110156108dc57600080fd5b8101908080359060200190929190505050612894565b6040518082815260200191505060405180910390f35b34801561091457600080fd5b506109576004803603602081101561092b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff1690602001909291905050506128ac565b005b34801561096557600080fd5b506109926004803603602081101561097c57600080fd5b8101908080359060200190929190505050612c3e565b005b610b3860048036036101408110156109ab57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803590602001906401000000008111156109f257600080fd5b820183602082011115610a0457600080fd5b80359060200191846001830284011164010000000083111715610a2657600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610ab257600080fd5b820183602082011115610ac457600080fd5b80359060200191846001830284011164010000000083111715610ae657600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050612d78565b60405180821515815260200191505060405180910390f35b348015610b5c57600080fd5b50610ba960048036036040811015610b7357600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506132b5565b6040518082815260200191505060405180910390f35b348015610bcb57600080fd5b50610d2660048036036060811015610be257600080fd5b810190808035906020019092919080359060200190640100000000811115610c0957600080fd5b820183602082011115610c1b57600080fd5b80359060200191846001830284011164010000000083111715610c3d57600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929080359060200190640100000000811115610ca057600080fd5b820183602082011115610cb257600080fd5b80359060200191846001830284011164010000000083111715610cd457600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505091929192905050506132da565b005b348015610d3457600080fd5b50610d3d613369565b6040518080602001828103825283818151815260200191508051906020019060200280838360005b83811015610d80578082015181840152602081019050610d65565b505050509050019250505060405180910390f35b348015610da057600080fd5b50610da9613512565b6040518082815260200191505060405180910390f35b348015610dcb57600080fd5b50610ea560048036036040811015610de257600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610e1f57600080fd5b820183602082011115610e3157600080fd5b80359060200191846001830284011164010000000083111715610e5357600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050509192919290505050613518565b005b348015610eb357600080fd5b506110156004803603610100811015610ecb57600080fd5b8101908080359060200190640100000000811115610ee857600080fd5b820183602082011115610efa57600080fd5b80359060200191846020830284011164010000000083111715610f1c57600080fd5b909192939192939080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190640100000000811115610f6757600080fd5b820183602082011115610f7957600080fd5b80359060200191846001830284011164010000000083111715610f9b57600080fd5b9091929391929390803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919050505061353a565b005b34801561102357600080fd5b506110d26004803603608081101561103a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561108157600080fd5b82018360208201111561109357600080fd5b803590602001918460018302840111640100000000831117156110b557600080fd5b9091929391929390803560ff1690602001909291905050506136f8565b6040518082815260200191505060405180910390f35b3480156110f457600080fd5b506111416004803603604081101561110b57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613820565b60405180806020018373ffffffffffffffffffffffffffffffffffffffff168152602001828103825284818151815260200191508051906020019060200280838360005b838110156111a0578082015181840152602081019050611185565b50505050905001935050505060405180910390f35b3480156111c157600080fd5b506111ee600480360360208110156111d857600080fd5b8101908080359060200190929190505050613a12565b005b3480156111fc57600080fd5b50611314600480360361014081101561121457600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561125b57600080fd5b82018360208201111561126d57600080fd5b8035906020019184600183028401116401000000008311171561128f57600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff16906020019092919080359060200190929190505050613bb1565b6040518082815260200191505060405180910390f35b34801561133657600080fd5b506113996004803603604081101561134d57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613bde565b005b3480156113a757600080fd5b506113ea600480360360208110156113be57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613f6f565b005b3480156113f857600080fd5b5061147b6004803603606081101561140f57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050613ff3565b005b34801561148957600080fd5b50611492614665565b6040518082815260200191505060405180910390f35b3480156114b457600080fd5b506115cc60048036036101408110156114cc57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291908035906020019064010000000081111561151357600080fd5b82018360208201111561152557600080fd5b8035906020019184600183028401116401000000008311171561154757600080fd5b9091929391929390803560ff169060200190929190803590602001909291908035906020019092919080359060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff1690602001909291908035906020019092919050505061466f565b6040518080602001828103825283818151815260200191508051906020019080838360005b8381101561160c5780820151818401526020810190506115f1565b50505050905090810190601f1680156116395780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b34801561165357600080fd5b506116966004803603602081101561166a57600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190505050614817565b005b3480156116a457600080fd5b506116ad614878565b6040518082815260200191505060405180910390f35b3480156116cf57600080fd5b5061173c600480360360608110156116e657600080fd5b81019080803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803573ffffffffffffffffffffffffffffffffffffffff169060200190929190803590602001909291905050506148f6565b005b34801561174a57600080fd5b50611753614d29565b6040518080602001828103825283818151815260200191508051906020019080838360005b83811015611793578082015181840152602081019050611778565b50505050905090810190601f1680156117c05780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6117d6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156118405750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b801561187857503073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6118ea576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146119eb576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508160026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506003600081548092919060010191905055507f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2682604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414611bba57611bb981612c3e565b5b5050565b611bd2604182614e0590919063ffffffff16565b82511015611c48576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6000808060008060005b8681101561243457611c648882614e3f565b80945081955082965050505060008460ff16141561206d578260001c9450611c96604188614e0590919063ffffffff16565b8260001c1015611d0e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8751611d2760208460001c614e6e90919063ffffffff16565b1115611d9b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006020838a01015190508851611dd182611dc360208760001c614e6e90919063ffffffff16565b614e6e90919063ffffffff16565b1115611e45576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60606020848b010190506320c13b0b60e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168773ffffffffffffffffffffffffffffffffffffffff166320c13b0b8d846040518363ffffffff1660e01b8152600401808060200180602001838103835285818151815260200191508051906020019080838360005b83811015611ee7578082015181840152602081019050611ecc565b50505050905090810190601f168015611f145780820380516001836020036101000a031916815260200191505b50838103825284818151815260200191508051906020019080838360005b83811015611f4d578082015181840152602081019050611f32565b50505050905090810190601f168015611f7a5780820380516001836020036101000a031916815260200191505b5094505050505060206040518083038186803b158015611f9957600080fd5b505afa158015611fad573d6000803e3d6000fd5b505050506040513d6020811015611fc357600080fd5b81019080805190602001909291905050507bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614612066576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b50506122b2565b60018460ff161415612181578260001c94508473ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16148061210a57506000600860008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008c81526020019081526020016000205414155b61217c576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6122b1565b601e8460ff1611156122495760018a60405160200180807f19457468657265756d205369676e6564204d6573736167653a0a333200000000815250601c018281526020019150506040516020818303038152906040528051906020012060048603858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa158015612238573d6000803e3d6000fd5b5050506020604051035194506122b0565b60018a85858560405160008152602001604052604051808581526020018460ff1681526020018381526020018281526020019450505050506020604051602081039080840390855afa1580156122a3573d6000803e3d6000fd5b5050506020604051035194505b5b5b8573ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff161180156123795750600073ffffffffffffffffffffffffffffffffffffffff16600260008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b80156123b25750600173ffffffffffffffffffffffffffffffffffffffff168573ffffffffffffffffffffffffffffffffffffffff1614155b612424576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330323600000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8495508080600101915050611c52565b50505050505050505050565b60008173ffffffffffffffffffffffffffffffffffffffff16600173ffffffffffffffffffffffffffffffffffffffff161415801561250b5750600073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156125dd5750600073ffffffffffffffffffffffffffffffffffffffff16600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b9050919050565b6000804690508091505090565b6000600173ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141580156126bc5750600073ffffffffffffffffffffffffffffffffffffffff16600160003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614155b61272e576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61273b858585855a614e8d565b9050801561278b573373ffffffffffffffffffffffffffffffffffffffff167f6895c13664aa4f67288b25d7a21d7aaa34916e355fb9b6fae0a139a9085becb860405160405180910390a26127cf565b3373ffffffffffffffffffffffffffffffffffffffff167facd2c8702804128fdb0db2bb49f6d127dd0181c13fd45dbfe16de0930e2bd37560405160405180910390a25b949350505050565b600060606127e7868686866125f1565b915060405160203d0181016040523d81523d6000602083013e8091505094509492505050565b606060006020830267ffffffffffffffff8111801561282b57600080fd5b506040519080825280601f01601f19166020018201604052801561285e5781602001600182028036833780820191505090505b50905060005b8381101561288957808501548060208302602085010152508080600101915050612864565b508091505092915050565b60076020528060005260406000206000915090505481565b6128b4614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561291e5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b612990576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614612a91576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508060016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507fecdf3a3effea5783a3c4c2140e677577666428d44ed9d474a0b3a4c9943f844081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b612c46614d62565b600354811115612cbe576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001811015612d35576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b806004819055507f610f7ff2b304ae8903c3de74c60c6ab1f7d6226b3f52c5161905bb5ad4039c936004546040518082815260200191505060405180910390a150565b6000806000612d928e8e8e8e8e8e8e8e8e8e60055461466f565b905060056000815480929190600101919050555080805190602001209150612dbb8282866132da565b506000612dc6614ed9565b9050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614612fac578073ffffffffffffffffffffffffffffffffffffffff166375f0bb528f8f8f8f8f8f8f8f8f8f8f336040518d63ffffffff1660e01b8152600401808d73ffffffffffffffffffffffffffffffffffffffff1681526020018c8152602001806020018a6001811115612e6957fe5b81526020018981526020018881526020018781526020018673ffffffffffffffffffffffffffffffffffffffff1681526020018573ffffffffffffffffffffffffffffffffffffffff168152602001806020018473ffffffffffffffffffffffffffffffffffffffff16815260200183810383528d8d82818152602001925080828437600081840152601f19601f820116905080830192505050838103825285818151815260200191508051906020019080838360005b83811015612f3b578082015181840152602081019050612f20565b50505050905090810190601f168015612f685780820380516001836020036101000a031916815260200191505b509e505050505050505050505050505050600060405180830381600087803b158015612f9357600080fd5b505af1158015612fa7573d6000803e3d6000fd5b505050505b6101f4612fd36109c48b01603f60408d0281612fc457fe5b04614f0a90919063ffffffff16565b015a1015613049576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60005a90506130b28f8f8f8f8080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f820116905080830192505050505050508e60008d146130a7578e6130ad565b6109c45a035b614e8d565b93506130c75a82614f2490919063ffffffff16565b905083806130d6575060008a14155b806130e2575060008814155b613154576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60008089111561316e5761316b828b8b8b8b614f44565b90505b84156131b8577f442e715f626346e8c54381002da614f62bee8d27386535b2521ec8540898556e8482604051808381526020018281526020019250505060405180910390a16131f8565b7f23428b18acfb3ea64b08dc0c1d296ea9c09702c09083ca5272e64d115b687d238482604051808381526020018281526020019250505060405180910390a15b5050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16146132a4578073ffffffffffffffffffffffffffffffffffffffff16639327136883856040518363ffffffff1660e01b815260040180838152602001821515815260200192505050600060405180830381600087803b15801561328b57600080fd5b505af115801561329f573d6000803e3d6000fd5b505050505b50509b9a5050505050505050505050565b6008602052816000526040600020602052806000526040600020600091509150505481565b6000600454905060008111613357576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b61336384848484611bbe565b50505050565b6060600060035467ffffffffffffffff8111801561338657600080fd5b506040519080825280602002602001820160405280156133b55781602001602082028036833780820191505090505b50905060008060026000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614613509578083838151811061346057fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600260008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050818060010192505061341f565b82935050505090565b60055481565b600080825160208401855af4806000523d6020523d600060403e60403d016000fd5b6135858a8a80806020026020016040519081016040528093929190818152602001838360200280828437600081840152601f19601f820116905080830192505050505050508961514a565b600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16146135c3576135c28461564a565b5b6136118787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050615679565b600082111561362b5761362982600060018685614f44565b505b3373ffffffffffffffffffffffffffffffffffffffff167f141df868a6331af528e38c83b7aa03edc19be66e37ae67f9285bf4f8e3c6a1a88b8b8b8b8960405180806020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281038252878782818152602001925060200280828437600081840152601f19601f820116905080830192505050965050505050505060405180910390a250505050505050505050565b6000805a905061374f878787878080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050865a614e8d565b61375857600080fd5b60005a8203905080604051602001808281526020019150506040516020818303038152906040526040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825283818151815260200191508051906020019080838360005b838110156137e55780820151818401526020810190506137ca565b50505050905090810190601f1680156138125780820380516001836020036101000a031916815260200191505b509250505060405180910390fd5b606060008267ffffffffffffffff8111801561383b57600080fd5b5060405190808252806020026020018201604052801561386a5781602001602082028036833780820191505090505b509150600080600160008773ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1690505b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff161415801561393d5750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561394857508482105b15613a03578084838151811061395a57fe5b602002602001019073ffffffffffffffffffffffffffffffffffffffff16908173ffffffffffffffffffffffffffffffffffffffff1681525050600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16905081806001019250506138d3565b80925081845250509250929050565b600073ffffffffffffffffffffffffffffffffffffffff16600260003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161415613b14576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001600860003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020016000206000838152602001908152602001600020819055503373ffffffffffffffffffffffffffffffffffffffff16817ff2a0eb156472d1440255b0d7c1e19cc07115d1051fe605b0dce69acfec884d9c60405160405180910390a350565b6000613bc68c8c8c8c8c8c8c8c8c8c8c61466f565b8051906020012090509b9a5050505050505050505050565b613be6614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614158015613c505750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b613cc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8073ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614613dc2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600160008273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600160008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507faab4fa2b463f581b2b32cb3b7e3b704b9ce37cc209b5fb4d77e593ace405427681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613f77614d62565b60007f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b90508181557f1151116914515bc0891ff9047a6cb32cf902546f83066499bcf8ba33d2353fa282604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a15050565b613ffb614d62565b600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156140655750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561409d57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b61410f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614210576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff161415801561427a5750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b6142ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16146143ec576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555080600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a17f9465fa0c962cc76958e6373a993326400c1c94f8be2fe3a952adfa7f60b2ea2681604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a1505050565b6000600454905090565b606060007fbb8310d486368db6bd6f849402fdd73ad53d316b5a4b2644ad6efe0f941286d860001b8d8d8d8d60405180838380828437808301925050509250505060405180910390208c8c8c8c8c8c8c604051602001808c81526020018b73ffffffffffffffffffffffffffffffffffffffff1681526020018a815260200189815260200188600181111561470057fe5b81526020018781526020018681526020018581526020018473ffffffffffffffffffffffffffffffffffffffff1681526020018373ffffffffffffffffffffffffffffffffffffffff1681526020018281526020019b505050505050505050505050604051602081830303815290604052805190602001209050601960f81b600160f81b61478c614878565b8360405160200180857effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff19168152600101847effffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff191681526001018381526020018281526020019450505050506040516020818303038152906040529150509b9a5050505050505050505050565b61481f614d62565b6148288161564a565b7f5ac6c46c93c8d0e53714ba3b53db3e7c046da994313d7ed0d192028bc7c228b081604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a150565b60007f47e79534a245952e8b16893a336b85a3d9ea9fa8c573f3d803afb92a7946921860001b6148a66125e4565b30604051602001808481526020018381526020018273ffffffffffffffffffffffffffffffffffffffff168152602001935050505060405160208183030381529060405280519060200120905090565b6148fe614d62565b806001600354031015614979576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16141580156149e35750600173ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614155b614a55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8173ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614614b55576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303500000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff16600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506000600260008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600360008154809291906001900391905055507ff8d49fc529812e9a7c5c50e69c20f0dccc0db8fa95c98bc58cc9a4f1c1299eaf82604051808273ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390a18060045414614d2457614d2381612c3e565b5b505050565b6040518060400160405280600581526020017f312e332e3000000000000000000000000000000000000000000000000000000081525081565b3073ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff1614614e03576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330333100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b565b600080831415614e185760009050614e39565b6000828402905082848281614e2957fe5b0414614e3457600080fd5b809150505b92915050565b60008060008360410260208101860151925060408101860151915060ff60418201870151169350509250925092565b600080828401905083811015614e8357600080fd5b8091505092915050565b6000600180811115614e9b57fe5b836001811115614ea757fe5b1415614ec0576000808551602087018986f49050614ed0565b600080855160208701888a87f190505b95945050505050565b6000807f4a204f620c8c5ccdca3fd54d003badd85ba500436a431f0cbda4f558c93c34c860001b9050805491505090565b600081831015614f1a5781614f1c565b825b905092915050565b600082821115614f3357600080fd5b600082840390508091505092915050565b600080600073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614614f815782614f83565b325b9050600073ffffffffffffffffffffffffffffffffffffffff168473ffffffffffffffffffffffffffffffffffffffff16141561509b57614fed3a8610614fca573a614fcc565b855b614fdf888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91508073ffffffffffffffffffffffffffffffffffffffff166108fc839081150290604051600060405180830381858888f19350505050615096576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b615140565b6150c0856150b2888a614e6e90919063ffffffff16565b614e0590919063ffffffff16565b91506150cd8482846158b4565b61513f576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330313200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5095945050505050565b6000600454146151c2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b8151811115615239576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303100000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60018110156152b0576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303200000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b60006001905060005b83518110156155b65760008482815181106152d057fe5b60200260200101519050600073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff16141580156153445750600173ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b801561537c57503073ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff1614155b80156153b457508073ffffffffffffffffffffffffffffffffffffffff168373ffffffffffffffffffffffffffffffffffffffff1614155b615426576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303300000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b600073ffffffffffffffffffffffffffffffffffffffff16600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1614615527576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475332303400000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b80600260008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055508092505080806001019150506152b9565b506001600260008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550825160038190555081600481905550505050565b60007f6c9a6c4a39284e37ed1cf53d337577d14212a4870fb976a4366c693b939918d560001b90508181555050565b600073ffffffffffffffffffffffffffffffffffffffff1660016000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff161461577b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475331303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b6001806000600173ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff16146158b05761583d8260008360015a614e8d565b6158af576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260058152602001807f475330303000000000000000000000000000000000000000000000000000000081525060200191505060405180910390fd5b5b5050565b60008063a9059cbb8484604051602401808373ffffffffffffffffffffffffffffffffffffffff168152602001828152602001925050506040516020818303038152906040529060e01b6020820180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff83818316178352505050509050602060008251602084016000896127105a03f13d6000811461595b5760208114615963576000935061596e565b81935061596e565b600051158215171593505b505050939250505056fea26469706673582212203874bcf92e1722cc7bfa0cef1a0985cf0dc3485ba0663db3747ccdf1605df53464736f6c63430007060033"
                 ),
                 "address": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             },
             "subtraces": 0,
             "traceAddress": [0],
-            "transactionHash": "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f",
+            "transactionHash": HexBytes(
+                "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f"
+            ),
             "transactionPosition": 12,
             "type": "create",
         },
     ],
     "0xf325b4e52d0649593e8c82f35bd389c13c13b21b61bc17de295979a21e5cfdc0": [
         {
             "action": {
@@ -58,20 +66,24 @@
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0xb63e800d0000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000160000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000300000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000"
                 ),
                 "to": "0xaE32496491b53841efb51829d6f886387708F99B",
             },
-            "blockHash": "0xcdb7884d4d2c4565c3408092527196e90010a683d45decbe1ed6a12904700b19",
+            "blockHash": HexBytes(
+                "0xcdb7884d4d2c4565c3408092527196e90010a683d45decbe1ed6a12904700b19"
+            ),
             "blockNumber": 8915756,
             "result": {"gasUsed": 145115, "output": HexBytes("0x")},
             "subtraces": 0,
             "traceAddress": [],
-            "transactionHash": "0xf325b4e52d0649593e8c82f35bd389c13c13b21b61bc17de295979a21e5cfdc0",
+            "transactionHash": HexBytes(
+                "0xf325b4e52d0649593e8c82f35bd389c13c13b21b61bc17de295979a21e5cfdc0"
+            ),
             "transactionPosition": 15,
             "type": "call",
         }
     ],
     "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0": [
         {
             "action": {
@@ -80,378 +92,442 @@
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x6a76120200000000000000000000000040a2accbd92bca938b02010e17a5b8929b49130d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001400000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000003c2f80000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000064000000000000000000000000000000000000000000000000000000000000004c48d80ff0a0000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000046b00469788fe6e9e9681c6ebf3bf78e7fd26fc01544600000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044bd86e508736166652e657468000000000000000000000000000000000000000000000000000000000000000000000000d662e05ce522b3861b70fc376f60bf50e200abfa00a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002c4bf6213e4000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001a0000000000000000000000000000000000000000000000000000000005bacaa20000000000000000000000000000000000000000000000012dfc9a7680524000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000100142b9e197e79ca94c077397bec601d9758e6ad54bfb308c529fb1ccb649664629507b80014ff96094ee587f52aed4ea98ccdce3ed4cef1139f4cbc45abf4cf3efca2d62b9a7cace73dca2d91ef5456d3fcecc2549d7cfeb33bf495a2505190b3cc6a55a90d3f5817150ad9c8d4fb3c6157c5ab99a2bd90bde5385608e212b9f0c0eb5e6c10b114900b7f894fcd9ba6126d9495341e2b09a684d822a04ba9e3bf40757bdb25323893eeac40649684dae8d5ac9be1b5688df2c8c77ffb1df3a8920c9493e26704a190c539948597a25dd0eadc3e9d3c04eef5e8bbb84dff18696e8fd0248ce2387d7c823f3b28280a73edcfd1b00d103210f5ca8f817b8c90519736c3b51ea1b6472ba406c4456d5b01c3b59343e564aae747fdd47ff6dc8ff4629d28252544a7e92977dccd4b30fb02073f088b2ad1cf0b7f5b2205842f5a78ba2580459420e11a06505b18e5ee6f8ded5bb92ee903d2eaf5d63bbecd73e213ca0870e463abf45cb18f85a835919099f45c6c56581232b3be9c06448420b35c94f4f3628f31b808b09ced67b073ab97919ba14e9389e154be4fe2b10fcdd327302fdc9a0b8cea5373715d2fce8d9ddd244f4259aafb0a21305edfdda956dd84359d69bacd790ff82f7310dd382bf3f53e885e74f5dad9b3aeb7fe96ce926ff47f8e2791b9d07b3e620189a36bf17e30c874e66b205c79492a16cd5a9c5bb65b700a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000640087b83f9aef04d6a9b38aab1023696e3b35434a8ba4c1611b39074722e31473dd333d27000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a76400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000410ff58feb0cba6ef7e22c415a7936b8a81fa384ebc5d2ec3718cc5e72730ddcdd296b0b29dd3aba9c64edde30f65ea98066a2cfa3412f9877d6bf3fded867ffd01b00000000000000000000000000000000000000000000000000000000000000"
                 ),
                 "to": "0x826f446C587159897Db0aE01192dA1691f12007f",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 228534,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 1,
             "traceAddress": [],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x826f446C587159897Db0aE01192dA1691f12007f",
                 "gas": 265117,
                 "value": 0,
                 "callType": "delegatecall",
                 "input": HexBytes(
                     "0x6a76120200000000000000000000000040a2accbd92bca938b02010e17a5b8929b49130d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001400000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000003c2f80000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000064000000000000000000000000000000000000000000000000000000000000004c48d80ff0a0000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000046b00469788fe6e9e9681c6ebf3bf78e7fd26fc01544600000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044bd86e508736166652e657468000000000000000000000000000000000000000000000000000000000000000000000000d662e05ce522b3861b70fc376f60bf50e200abfa00a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002c4bf6213e4000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001a0000000000000000000000000000000000000000000000000000000005bacaa20000000000000000000000000000000000000000000000012dfc9a7680524000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000100142b9e197e79ca94c077397bec601d9758e6ad54bfb308c529fb1ccb649664629507b80014ff96094ee587f52aed4ea98ccdce3ed4cef1139f4cbc45abf4cf3efca2d62b9a7cace73dca2d91ef5456d3fcecc2549d7cfeb33bf495a2505190b3cc6a55a90d3f5817150ad9c8d4fb3c6157c5ab99a2bd90bde5385608e212b9f0c0eb5e6c10b114900b7f894fcd9ba6126d9495341e2b09a684d822a04ba9e3bf40757bdb25323893eeac40649684dae8d5ac9be1b5688df2c8c77ffb1df3a8920c9493e26704a190c539948597a25dd0eadc3e9d3c04eef5e8bbb84dff18696e8fd0248ce2387d7c823f3b28280a73edcfd1b00d103210f5ca8f817b8c90519736c3b51ea1b6472ba406c4456d5b01c3b59343e564aae747fdd47ff6dc8ff4629d28252544a7e92977dccd4b30fb02073f088b2ad1cf0b7f5b2205842f5a78ba2580459420e11a06505b18e5ee6f8ded5bb92ee903d2eaf5d63bbecd73e213ca0870e463abf45cb18f85a835919099f45c6c56581232b3be9c06448420b35c94f4f3628f31b808b09ced67b073ab97919ba14e9389e154be4fe2b10fcdd327302fdc9a0b8cea5373715d2fce8d9ddd244f4259aafb0a21305edfdda956dd84359d69bacd790ff82f7310dd382bf3f53e885e74f5dad9b3aeb7fe96ce926ff47f8e2791b9d07b3e620189a36bf17e30c874e66b205c79492a16cd5a9c5bb65b700a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000640087b83f9aef04d6a9b38aab1023696e3b35434a8ba4c1611b39074722e31473dd333d27000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a76400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000410ff58feb0cba6ef7e22c415a7936b8a81fa384ebc5d2ec3718cc5e72730ddcdd296b0b29dd3aba9c64edde30f65ea98066a2cfa3412f9877d6bf3fded867ffd01b00000000000000000000000000000000000000000000000000000000000000"
                 ),
                 "to": "0xb6029EA3B2c51D09a50B53CA8012FeEB05bDa35A",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 223320,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 1,
             "traceAddress": [0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x826f446C587159897Db0aE01192dA1691f12007f",
                 "gas": 239379,
                 "value": 0,
                 "callType": "delegatecall",
                 "input": HexBytes(
                     "0x8d80ff0a0000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000046b00469788fe6e9e9681c6ebf3bf78e7fd26fc01544600000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044bd86e508736166652e657468000000000000000000000000000000000000000000000000000000000000000000000000d662e05ce522b3861b70fc376f60bf50e200abfa00a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002c4bf6213e4000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001a0000000000000000000000000000000000000000000000000000000005bacaa20000000000000000000000000000000000000000000000012dfc9a7680524000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000100142b9e197e79ca94c077397bec601d9758e6ad54bfb308c529fb1ccb649664629507b80014ff96094ee587f52aed4ea98ccdce3ed4cef1139f4cbc45abf4cf3efca2d62b9a7cace73dca2d91ef5456d3fcecc2549d7cfeb33bf495a2505190b3cc6a55a90d3f5817150ad9c8d4fb3c6157c5ab99a2bd90bde5385608e212b9f0c0eb5e6c10b114900b7f894fcd9ba6126d9495341e2b09a684d822a04ba9e3bf40757bdb25323893eeac40649684dae8d5ac9be1b5688df2c8c77ffb1df3a8920c9493e26704a190c539948597a25dd0eadc3e9d3c04eef5e8bbb84dff18696e8fd0248ce2387d7c823f3b28280a73edcfd1b00d103210f5ca8f817b8c90519736c3b51ea1b6472ba406c4456d5b01c3b59343e564aae747fdd47ff6dc8ff4629d28252544a7e92977dccd4b30fb02073f088b2ad1cf0b7f5b2205842f5a78ba2580459420e11a06505b18e5ee6f8ded5bb92ee903d2eaf5d63bbecd73e213ca0870e463abf45cb18f85a835919099f45c6c56581232b3be9c06448420b35c94f4f3628f31b808b09ced67b073ab97919ba14e9389e154be4fe2b10fcdd327302fdc9a0b8cea5373715d2fce8d9ddd244f4259aafb0a21305edfdda956dd84359d69bacd790ff82f7310dd382bf3f53e885e74f5dad9b3aeb7fe96ce926ff47f8e2791b9d07b3e620189a36bf17e30c874e66b205c79492a16cd5a9c5bb65b700a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000640087b83f9aef04d6a9b38aab1023696e3b35434a8ba4c1611b39074722e31473dd333d27000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a7640000000000000000000000000000000000000000000000"
                 ),
                 "to": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {"gasUsed": 201030, "output": HexBytes("0x")},
             "subtraces": 3,
             "traceAddress": [0, 0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x826f446C587159897Db0aE01192dA1691f12007f",
                 "gas": 232202,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0xbd86e508736166652e657468000000000000000000000000000000000000000000000000000000000000000000000000d662e05ce522b3861b70fc376f60bf50e200abfa"
                 ),
                 "to": "0x469788fE6E9E9681C6ebF3bF78e7Fd26Fc015446",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {"gasUsed": 24983, "output": HexBytes("0x")},
             "subtraces": 0,
             "traceAddress": [0, 0, 0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x826f446C587159897Db0aE01192dA1691f12007f",
                 "gas": 204798,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0xbf6213e4000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001a0000000000000000000000000000000000000000000000000000000005bacaa20000000000000000000000000000000000000000000000012dfc9a7680524000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000100142b9e197e79ca94c077397bec601d9758e6ad54bfb308c529fb1ccb649664629507b80014ff96094ee587f52aed4ea98ccdce3ed4cef1139f4cbc45abf4cf3efca2d62b9a7cace73dca2d91ef5456d3fcecc2549d7cfeb33bf495a2505190b3cc6a55a90d3f5817150ad9c8d4fb3c6157c5ab99a2bd90bde5385608e212b9f0c0eb5e6c10b114900b7f894fcd9ba6126d9495341e2b09a684d822a04ba9e3bf40757bdb25323893eeac40649684dae8d5ac9be1b5688df2c8c77ffb1df3a8920c9493e26704a190c539948597a25dd0eadc3e9d3c04eef5e8bbb84dff18696e8fd0248ce2387d7c823f3b28280a73edcfd1b00d103210f5ca8f817b8c90519736c3b51ea1b6472ba406c4456d5b01c3b59343e564aae747fdd47ff6dc8ff4629d28252544a7e92977dccd4b30fb02073f088b2ad1cf0b7f5b2205842f5a78ba2580459420e11a06505b18e5ee6f8ded5bb92ee903d2eaf5d63bbecd73e213ca0870e463abf45cb18f85a835919099f45c6c56581232b3be9c06448420b35c94f4f3628f31b808b09ced67b073ab97919ba14e9389e154be4fe2b10fcdd327302fdc9a0b8cea5373715d2fce8d9ddd244f4259aafb0a21305edfdda956dd84359d69bacd790ff82f7310dd382bf3f53e885e74f5dad9b3aeb7fe96ce926ff47f8e2791b9d07b3e620189a36bf17e30c874e66b205c79492a16cd5a9c5bb65b7"
                 ),
                 "to": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {"gasUsed": 75351, "output": HexBytes("0x")},
             "subtraces": 1,
             "traceAddress": [0, 0, 1],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 188502,
                 "value": 0,
                 "callType": "staticcall",
                 "input": HexBytes(
                     "0x70a08231000000000000000000000000a0b937d5c8e32a80e3a8ed4227cd020221544ee6"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 2886,
                 "output": HexBytes(
                     "0x000000000000000000000000000000000000000000295bd306348cee3284339a"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 1, 0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x826f446C587159897Db0aE01192dA1691f12007f",
                 "gas": 130274,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x0087b83f9aef04d6a9b38aab1023696e3b35434a8ba4c1611b39074722e31473dd333d27000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a7640000"
                 ),
                 "to": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {"gasUsed": 93862, "output": HexBytes("0x")},
             "subtraces": 7,
             "traceAddress": [0, 0, 2],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 119997,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x095ea7b30000000000000000000000008cf60b289f8d31f737049b590b5e4285ff0bd1d10000000000000000000000000000000000000000000000000de0b6b3a7640000"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 25285,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 94401,
                 "value": 0,
                 "callType": "staticcall",
                 "input": HexBytes(
                     "0x70a08231000000000000000000000000a0b937d5c8e32a80e3a8ed4227cd020221544ee6"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 886,
                 "output": HexBytes(
                     "0x000000000000000000000000000000000000000000295bd306348cee3284339a"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 1],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 92834,
                 "value": 0,
                 "callType": "staticcall",
                 "input": HexBytes(
                     "0x70a08231000000000000000000000000826f446c587159897db0ae01192da1691f12007f"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 2886,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000000"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 2],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 85106,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x468721a70000000000000000000000005afe3855358e112b5647b952709e6165e1c1eeee000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006423b872dd000000000000000000000000a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a764000000000000000000000000000000000000000000000000000000000000"
                 ),
                 "to": "0x8CF60B289f8d31F737049B590b5E4285Ff0Bd1D1",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 41825,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 1,
             "traceAddress": [0, 0, 2, 3],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x8CF60B289f8d31F737049B590b5E4285Ff0Bd1D1",
                 "gas": 79018,
                 "value": 0,
                 "callType": "delegatecall",
                 "input": HexBytes(
                     "0x468721a70000000000000000000000005afe3855358e112b5647b952709e6165e1c1eeee000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006423b872dd000000000000000000000000a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a764000000000000000000000000000000000000000000000000000000000000"
                 ),
                 "to": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 36946,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 1,
             "traceAddress": [0, 0, 2, 3, 0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0x8CF60B289f8d31F737049B590b5E4285Ff0Bd1D1",
                 "gas": 74535,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x23b872dd000000000000000000000000a0b937d5c8e32a80e3a8ed4227cd020221544ee6000000000000000000000000826f446c587159897db0ae01192da1691f12007f0000000000000000000000000000000000000000000000000de0b6b3a7640000"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 32341,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 3, 0, 0],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 43002,
                 "value": 0,
                 "callType": "call",
                 "input": HexBytes(
                     "0x095ea7b30000000000000000000000008cf60b289f8d31f737049b590b5e4285ff0bd1d10000000000000000000000000000000000000000000000000000000000000000"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 3285,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000000000000000001"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 4],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 39062,
                 "value": 0,
                 "callType": "staticcall",
                 "input": HexBytes(
                     "0x70a08231000000000000000000000000a0b937d5c8e32a80e3a8ed4227cd020221544ee6"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 886,
                 "output": HexBytes(
                     "0x000000000000000000000000000000000000000000295bd2f853d63a8b20339a"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 5],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
         {
             "action": {
                 "from": "0xA0b937D5c8E32a80E3a8ed4227CD020221544ee6",
                 "gas": 37498,
                 "value": 0,
                 "callType": "staticcall",
                 "input": HexBytes(
                     "0x70a08231000000000000000000000000826f446c587159897db0ae01192da1691f12007f"
                 ),
                 "to": "0x5aFE3855358E112B5647B952709E6165e1c1eEEe",
             },
-            "blockHash": "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624",
+            "blockHash": HexBytes(
+                "0xa1dd687d41a835a1e173b5f69f656eaad52570ca864dfaeece6bec72e17bc624"
+            ),
             "blockNumber": 15630274,
             "result": {
                 "gasUsed": 886,
                 "output": HexBytes(
                     "0x0000000000000000000000000000000000000000000000000de0b6b3a7640000"
                 ),
             },
             "subtraces": 0,
             "traceAddress": [0, 0, 2, 6],
-            "transactionHash": "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
+            "transactionHash": HexBytes(
+                "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0"
+            ),
             "transactionPosition": 80,
             "type": "call",
         },
     ],
 }
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import mock
 
 from django.test import TestCase
 
+import pytest
 from eth_account import Account
 from requests import Session
 
 from ... import EthereumClient
 from ...oracles import CannotGetPriceFromOracle, CowswapOracle
 from ..ethereum_test_case import EthereumTestCaseMixin
 from ..test_oracles import (
@@ -13,14 +14,15 @@
     usdc_token_mainnet_address,
     usdt_token_mainnet_address,
     weth_token_mainnet_address,
 )
 from ..utils import just_test_if_mainnet_node
 
 
+@pytest.skip("Having issues often", allow_module_level=True)
 class TestCowswapOracle(EthereumTestCaseMixin, TestCase):
     def test_get_price(self):
         mainnet_node = just_test_if_mainnet_node()
         ethereum_client = EthereumClient(mainnet_node)
 
         self.assertTrue(CowswapOracle.is_available(ethereum_client))
 
@@ -54,34 +56,24 @@
             usdc_token_mainnet_address, dai_token_mainnet_address
         )
         self.assertAlmostEqual(price, 1.0, delta=0.5)
 
         with mock.patch.object(
             Session, "post", side_effect=IOError("Connection Error")
         ):
-            with self.assertRaisesMessage(
-                CannotGetPriceFromOracle,
-                f"Cannot get price from CowSwap "
-                f"{{}} "
-                f"for token-1={usdc_token_mainnet_address} to token-2={dai_token_mainnet_address}",
-            ):
+            with self.assertRaises(CannotGetPriceFromOracle):
                 cowswap_oracle.get_price(
                     usdc_token_mainnet_address, dai_token_mainnet_address
                 )
 
         random_token = Account.create().address
         with self.assertRaisesMessage(
             CannotGetPriceFromOracle,
             f"Cannot get decimals for token={random_token}",
         ):
             cowswap_oracle.get_price(random_token)
 
         with mock.patch(
             "gnosis.eth.oracles.cowswap.get_decimals", autospec=True, return_value=18
         ):
-            with self.assertRaisesMessage(
-                CannotGetPriceFromOracle,
-                f"Cannot get price from CowSwap "
-                f"{{'errorType': 'UnsupportedToken', 'description': 'Token address {random_token.lower()}'}} "
-                f"for token-1={random_token} to token-2={weth_token_mainnet_address}",
-            ):
+            with self.assertRaises(CannotGetPriceFromOracle):
                 cowswap_oracle.get_price(random_token)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,10 +77,10 @@
         ):
             uniswap_v3_oracle.get_price(wrapped_nxm_token_mainnet_address)
 
     def test_get_price_contract_not_deployed(self):
         self.assertFalse(UniswapV3Oracle.is_available(self.ethereum_client))
         with self.assertRaisesMessage(
             ValueError,
-            f"Uniswap V3 Router Contract {UniswapV3Oracle.UNISWAP_V3_ROUTER} does not exist",
+            f"Uniswap V3 Router Contract {UniswapV3Oracle.DEFAULT_ROUTER_ADDRESS} does not exist",
         ):
             UniswapV3Oracle(self.ethereum_client)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_ethereum_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,27 @@
 from ..ethereum_client import (
     EthereumClient,
     EthereumClientProvider,
     EthereumNetwork,
     FromAddressNotFound,
     InsufficientFunds,
     InvalidNonce,
-    ParityManager,
     SenderAccountNotFoundInNode,
+    TracingManager,
 )
 from ..exceptions import BatchCallException, ChainIdIsRequired, InvalidERC20Info
-from ..utils import fast_to_checksum_address, get_eth_address_with_key
+from ..utils import get_eth_address_with_key
 from .ethereum_test_case import EthereumTestCaseMixin
 from .mocks.mock_internal_txs import creation_internal_txs, internal_txs_errored
 from .mocks.mock_log_receipts import invalid_log_receipt, log_receipts
-from .mocks.mock_trace_block import trace_block_2191709_mock, trace_block_13191781_mock
+from .mocks.mock_trace_block import (
+    trace_block_2191709_mock,
+    trace_block_13191781_mock,
+    trace_block_15630274_mock,
+)
 from .mocks.mock_trace_filter import trace_filter_mock_1
 from .mocks.mock_trace_transaction import trace_transaction_mocks
 from .utils import deploy_example_erc20, just_test_if_mainnet_node
 
 
 class TestERC20Module(EthereumTestCaseMixin, TestCase):
     def test_decode_transfer_log(self):
@@ -415,139 +419,17 @@
         )
         self.assertEqual(
             self.ethereum_client.erc20.get_balance(owner_2.address, erc20.address),
             amount_2,
         )
 
 
-class TestParityManager(EthereumTestCaseMixin, TestCase):
-    def test_decode_trace(self):
-        example_traces = [
-            {
-                "action": {
-                    "callType": "call",
-                    "from": "0x32be343b94f860124dc4fee278fdcbd38c102d88",
-                    "gas": "0x4c40d",
-                    "input": "0x",
-                    "to": "0x8bbb73bcb5d553b5a556358d27625323fd781d37",
-                    "value": "0x3f0650ec47fd240000",
-                },
-                "blockHash": "0x86df301bcdd8248d982dbf039f09faf792684e1aeee99d5b58b77d620008b80f",
-                "blockNumber": 3068183,
-                "result": {"gasUsed": "0x0", "output": "0x"},
-                "subtraces": 0,
-                "traceAddress": [],
-                "transactionHash": "0x3321a7708b1083130bd78da0d62ead9f6683033231617c9d268e2c7e3fa6c104",
-                "transactionPosition": 3,
-                "type": "call",
-            },
-            {
-                "action": {
-                    "from": "0x3b169a0fb55ea0b6bafe54c272b1fe4983742bf7",
-                    "gas": "0x49b0b",
-                    "init": "0x608060405234801561001057600080fd5b5060405161060a38038061060a833981018060405281019080805190602001909291908051820192919060200180519060200190929190805190602001909291908051906020019092919050505084848160008173ffffffffffffffffffffffffffffffffffffffff1614151515610116576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260248152602001807f496e76616c6964206d617374657220636f707920616464726573732070726f7681526020017f696465640000000000000000000000000000000000000000000000000000000081525060400191505060405180910390fd5b806000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550506000815111156101a35773ffffffffffffffffffffffffffffffffffffffff60005416600080835160208501846127105a03f46040513d6000823e600082141561019f573d81fd5b5050505b5050600081111561036d57600073ffffffffffffffffffffffffffffffffffffffff168273ffffffffffffffffffffffffffffffffffffffff1614156102b7578273ffffffffffffffffffffffffffffffffffffffff166108fc829081150290604051600060405180830381858888f1935050505015156102b2576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260268152602001807f436f756c64206e6f74207061792073616665206372656174696f6e207769746881526020017f206574686572000000000000000000000000000000000000000000000000000081525060400191505060405180910390fd5b61036c565b6102d1828483610377640100000000026401000000009004565b151561036b576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004018080602001828103825260268152602001807f436f756c64206e6f74207061792073616665206372656174696f6e207769746881526020017f20746f6b656e000000000000000000000000000000000000000000000000000081525060400191505060405180910390fd5b5b5b5050505050610490565b600060608383604051602401808373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168152602001828152602001925050506040516020818303038152906040527fa9059cbb000000000000000000000000000000000000000000000000000000007bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19166020820180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff838183161783525050505090506000808251602084016000896127105a03f16040513d6000823e3d60008114610473576020811461047b5760009450610485565b829450610485565b8151158315171594505b505050509392505050565b61016b8061049f6000396000f30060806040526004361061004c576000357c0100000000000000000000000000000000000000000000000000000000900463ffffffff1680634555d5c91461008b5780635c60da1b146100b6575b73ffffffffffffffffffffffffffffffffffffffff600054163660008037600080366000845af43d6000803e6000811415610086573d6000fd5b3d6000f35b34801561009757600080fd5b506100a061010d565b6040518082815260200191505060405180910390f35b3480156100c257600080fd5b506100cb610116565b604051808273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390f35b60006002905090565b60008060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050905600a165627a7a7230582007fffd557dfc8c4d2fdf56ba6381a6ce5b65b6260e1492d87f26c6d4f1d0410800290000000000000000000000008942595a2dc5181df0465af0d7be08c8f23c93af00000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000d9e09beaeb338d81a7c5688358df0071d498811500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001b15f91a8c35300000000000000000000000000000000000000000000000000000000000001640ec78d9e00000000000000000000000000000000000000000000000000000000000000800000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001200000000000000000000000000000000000000000000000000000000000000004000000000000000000000000f763ea5fbb191d47dc4b083dcdc3cdfb586468f8000000000000000000000000ad25c9717d04c0a12086a1d352c1ccf4bf5fcbf80000000000000000000000000da7155692446c80a4e7ad72018e586f20fa3bfe000000000000000000000000bce0cc48ce44e0ac9ee38df4d586afbacef191fa0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
-                    "value": "0x0",
-                },
-                "blockHash": "0x03f9f64dfeb7807b5df608e6957dd4d521fd71685aac5533451d27f0abe03660",
-                "blockNumber": 3793534,
-                "result": {
-                    "address": "0x61a7cc907c47c133d5ff5b685407201951fcbd08",
-                    "code": "0x60806040526004361061004c576000357c0100000000000000000000000000000000000000000000000000000000900463ffffffff1680634555d5c91461008b5780635c60da1b146100b6575b73ffffffffffffffffffffffffffffffffffffffff600054163660008037600080366000845af43d6000803e6000811415610086573d6000fd5b3d6000f35b34801561009757600080fd5b506100a061010d565b6040518082815260200191505060405180910390f35b3480156100c257600080fd5b506100cb610116565b604051808273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390f35b60006002905090565b60008060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050905600a165627a7a7230582007fffd557dfc8c4d2fdf56ba6381a6ce5b65b6260e1492d87f26c6d4f1d041080029",
-                    "gasUsed": "0x4683f",
-                },
-                "subtraces": 2,
-                "traceAddress": [],
-                "transactionHash": "0x6c7e8f8778d33d81b29c4bd7526ee50a4cea340d69eed6c89ada4e6fab731789",
-                "transactionPosition": 1,
-                "type": "create",
-            },
-            {
-                "action": {
-                    "callType": "call",
-                    "from": "0xed85033a23027439fb20f381f5930ba67f1ebee0",
-                    "gas": "0x0",
-                    "input": "0x",
-                    "to": "0x0affccd762f0a7fa1bca40c51afe1a806a74a6f9",
-                    "value": "0x11c290633b7000",
-                },
-                "blockHash": "0xbf3a508137e72b20399852becdee1752c7b9986184f835014d12b10c01746f39",
-                "blockNumber": 7556887,
-                "error": "Out of gas",
-                "subtraces": 0,
-                "traceAddress": [],
-                "transactionHash": "0xec7e447ce8eef033a8c85442a281bd34436e576553c7d98fbe859af7754a9064",
-                "transactionPosition": 117,
-                "type": "call",
-            },
-            {
-                "action": {
-                    "address": "0x4440adafbc6c4e45c299451c0eedc7c8b98c14ac",
-                    "balance": "0xa",
-                    "refundAddress": "0x1240adafbc6c4e45c299451c0eedc7c8b98c2222",
-                },
-                "blockHash": "0x8512d367492371edf44ebcbbbd935bc434946dddc2b126cb558df5906012186c",
-                "blockNumber": 7829689,
-                "result": None,
-                "subtraces": 0,
-                "traceAddress": [0, 0, 0, 0, 0, 0],
-                "transactionHash": "0x5f7af6aa390f9f8dd79ee692c37cbde76bb7869768b1bac438b6d176c94f637d",
-                "transactionPosition": 35,
-                "type": "suicide",
-            },
-        ]
-        at_least_one_error = False
-        at_least_one_self_destruct = False
-        decoded_traces = self.ethereum_client.parity._decode_traces(example_traces)
-        for example_trace, decoded_trace in zip(example_traces, decoded_traces):
-            if decoded_trace["type"] == "suicide":
-                self.assertEqual(
-                    decoded_trace["action"]["address"],
-                    "0x4440AdaFBc6c4E45C299451C0eEdC7C8B98c14Ac",
-                )
-                self.assertEqual(decoded_trace["action"]["balance"], 10)
-                self.assertEqual(
-                    decoded_trace["action"]["refundAddress"],
-                    "0x1240aDafBC6C4e45C299451C0eEdC7c8B98C2222",
-                )
-                at_least_one_self_destruct = True
-            else:
-                self.assertEqual(
-                    decoded_trace["action"]["gas"],
-                    int(example_trace["action"]["gas"], 16),
-                )
-                self.assertEqual(
-                    decoded_trace["action"]["value"],
-                    int(example_trace["action"]["value"], 16),
-                )
-                if "error" in decoded_trace:
-                    self.assertNotIn("result", decoded_trace)
-                    at_least_one_error = True
-                else:
-                    self.assertEqual(
-                        decoded_trace["result"]["gasUsed"],
-                        int(example_trace["result"]["gasUsed"], 16),
-                    )
-
-        self.assertTrue(at_least_one_error)
-        self.assertTrue(at_least_one_self_destruct)
-
-        self.assertEqual(decoded_traces[0]["result"]["output"], HexBytes(""))
-        self.assertEqual(
-            decoded_traces[1]["result"]["address"],
-            fast_to_checksum_address(example_traces[1]["result"]["address"]),
-        )
-        self.assertEqual(
-            decoded_traces[1]["result"]["code"],
-            HexBytes(example_traces[1]["result"]["code"]),
-        )
-
-        self.assertEqual(decoded_traces[2]["error"], "Out of gas")
-
+class TestTracingManager(EthereumTestCaseMixin, TestCase):
     def test_filter_out_errored_traces(self):
-        self.assertEqual(self.ethereum_client.parity.filter_out_errored_traces([]), [])
+        self.assertEqual(self.ethereum_client.tracing.filter_out_errored_traces([]), [])
         traces = internal_txs_errored
         expected = [
             {
                 "action": {
                     "from": "0x667dEb5A98f77052cf561658575cF1530Ee42C7a",
                     "gas": 60066,
                     "value": 0,
@@ -594,15 +476,15 @@
                 "traceAddress": [0],
                 "transactionHash": "0xf097d5e5dd39a6799fc13dfa49732a115b457386520dc92f99f0135a1d196851",
                 "transactionPosition": 3,
                 "type": "call",
             },
         ]
         self.assertEqual(
-            self.ethereum_client.parity.filter_out_errored_traces(traces), expected
+            self.ethereum_client.tracing.filter_out_errored_traces(traces), expected
         )
 
         traces = [
             {
                 "traceAddress": [],
             },
             {
@@ -671,101 +553,101 @@
                 "traceAddress": [0, 0, 2],
             },
         ]
         self.assertEqual(
             sorted(traces, key=lambda trace: trace["traceAddress"]), traces
         )
         self.assertEqual(
-            self.ethereum_client.parity.filter_out_errored_traces(traces), expected
+            self.ethereum_client.tracing.filter_out_errored_traces(traces), expected
         )
 
     @mock.patch.object(
-        ParityManager, "trace_transaction", return_value=internal_txs_errored
+        TracingManager, "trace_transaction", return_value=internal_txs_errored
     )
     def test_get_previous_trace(self, trace_transaction_mock: MagicMock):
         self.assertEqual(
-            self.ethereum_client.parity.get_previous_trace("0x12", [0, 0])[
+            self.ethereum_client.tracing.get_previous_trace("0x12", [0, 0])[
                 "traceAddress"
             ],
             [0],
         )
         self.assertEqual(
-            self.ethereum_client.parity.get_previous_trace(
+            self.ethereum_client.tracing.get_previous_trace(
                 "0x12", [0, 0], number_traces=2
             )["traceAddress"],
             [],
         )
         self.assertEqual(
-            self.ethereum_client.parity.get_previous_trace(
+            self.ethereum_client.tracing.get_previous_trace(
                 "0x12", [0, 0], skip_delegate_calls=True
             )["traceAddress"],
             [],
         )
         self.assertIsNone(
-            self.ethereum_client.parity.get_previous_trace(
+            self.ethereum_client.tracing.get_previous_trace(
                 "0x12", [0, 0], number_traces=3
             )
         )
         self.assertEqual(
-            self.ethereum_client.parity.get_previous_trace(
+            self.ethereum_client.tracing.get_previous_trace(
                 "0x12", [0, 0, 0], skip_delegate_calls=True
             )["traceAddress"],
             [0, 0],
         )
 
     @mock.patch.object(
-        ParityManager, "trace_transaction", return_value=creation_internal_txs
+        TracingManager, "trace_transaction", return_value=creation_internal_txs
     )
     def test_get_next_traces(self, trace_transaction_mock: MagicMock):
         def trace_addresses(traces: Sequence[Dict[str, Any]]) -> List[List[int]]:
             return [trace["traceAddress"] for trace in traces]
 
         self.assertEqual(
-            trace_addresses(self.ethereum_client.parity.get_next_traces("0x12", [])),
+            trace_addresses(self.ethereum_client.tracing.get_next_traces("0x12", [])),
             [[0], [1]],
         )
         self.assertEqual(
             trace_addresses(
-                self.ethereum_client.parity.get_next_traces(
+                self.ethereum_client.tracing.get_next_traces(
                     "0x12", [], remove_delegate_calls=True
                 )
             ),
             [[1]],
         )
         self.assertEqual(
             trace_addresses(
-                self.ethereum_client.parity.get_next_traces(
+                self.ethereum_client.tracing.get_next_traces(
                     "0x12", [], remove_calls=True
                 )
             ),
             [[0]],
         )
         self.assertEqual(
             trace_addresses(
-                self.ethereum_client.parity.get_next_traces(
+                self.ethereum_client.tracing.get_next_traces(
                     "0x12", [], remove_delegate_calls=True, remove_calls=True
                 )
             ),
             [],
         )
-        self.assertEqual(self.ethereum_client.parity.get_next_traces("0x12", [0]), [])
+        self.assertEqual(self.ethereum_client.tracing.get_next_traces("0x12", [0]), [])
         self.assertEqual(
-            trace_addresses(self.ethereum_client.parity.get_next_traces("0x12", [1])),
+            trace_addresses(self.ethereum_client.tracing.get_next_traces("0x12", [1])),
             [[1, 0]],
         )
 
     def test_trace_filter(self):
         with self.assertRaisesMessage(AssertionError, "at least"):
-            self.ethereum_client.parity.trace_filter()
+            self.ethereum_client.tracing.trace_filter()
 
         with self.assertRaisesMessage(
             ValueError, "The method trace_filter does not exist/is not available"
         ):
-            self.ethereum_client.parity.trace_filter(
-                from_address=Account.create().address
+            self.ethereum_client.tracing.trace_filter(
+                to_address=[Account.create().address]
             )
 
     @mock.patch.object(requests.Response, "json")
     def test_raw_batch_request(self, session_post_mock: MagicMock):
         # Ankr
         session_post_mock.return_value = {
             "jsonrpc": "2.0",
@@ -1356,57 +1238,65 @@
         tx["chainId"] = 1
         with self.assertRaises(InsufficientFunds):
             self.ethereum_client.send_unsigned_transaction(
                 tx, private_key=random_sender_account.key
             )
 
     def test_trace_block(self):
-        block_numbers = [13191781, 2191709]
-        for block_number, trace_block_mock in zip(
-            block_numbers, [trace_block_13191781_mock, trace_block_2191709_mock]
-        ):
+        block_numbers = [13191781, 2191709, 15630274]
+        block_mocks = [
+            trace_block_13191781_mock,
+            trace_block_2191709_mock,
+            trace_block_15630274_mock,
+        ]
+        for block_number, trace_block_mock in zip(block_numbers, block_mocks):
             with self.subTest(block_number=block_number):
                 self.assertEqual(
-                    self.ethereum_client.parity.trace_block(block_number),
+                    self.ethereum_client.tracing.trace_block(block_number),
                     trace_block_mock,
                 )
 
     def test_trace_blocks(self):
-        block_numbers = [13191781, 2191709]
+        block_numbers = [13191781, 2191709, 15630274]
+        block_mocks = [
+            trace_block_13191781_mock,
+            trace_block_2191709_mock,
+            trace_block_15630274_mock,
+        ]
         self.assertEqual(
-            self.ethereum_client.parity.trace_blocks(block_numbers),
-            [trace_block_13191781_mock, trace_block_2191709_mock],
+            self.ethereum_client.tracing.trace_blocks(block_numbers),
+            block_mocks,
         )
 
     def test_trace_transaction(self):
         for tx_hash in [
             # Safe 1.3.0 deployment
             "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f",
             # Erigon v2.31.0 traceAddress issue https://github.com/ledgerwatch/erigon/issues/6375
             "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
         ]:
             with self.subTest(tx_hash=tx_hash):
                 self.assertEqual(
-                    self.ethereum_client.parity.trace_transaction(tx_hash),
+                    self.ethereum_client.tracing.trace_transaction(tx_hash),
                     trace_transaction_mocks[tx_hash],
                 )
 
     def test_trace_transactions(self):
         tx_hashes = [
             "0x0b04589bdc11585fb98f270b1bfeff0fb3bbb3c56d35b104f62d8115d6f7c57f",  # Safe 1.3.0 deployment
             "0xf325b4e52d0649593e8c82f35bd389c13c13b21b61bc17de295979a21e5cfdc0",  # Safe 1.1.0 setup
             # Erigon v2.31.0 traceAddress issue https://github.com/ledgerwatch/erigon/issues/6375
             "0xc27273dc6e631d275baa527e1b07cd9097887317c26034bf8ea7bbe38c9353f0",
         ]
         self.assertEqual(
-            self.ethereum_client.parity.trace_transactions(tx_hashes),
+            self.ethereum_client.tracing.trace_transactions(tx_hashes),
             [trace_transaction_mocks[tx_hash] for tx_hash in tx_hashes],
         )
 
     def test_trace_filter(self):
         safe_1_3_0_address = "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552"
-        self.assertEqual(
-            self.ethereum_client.parity.trace_filter(
+        self.assertListEqual(
+            self.ethereum_client.tracing.trace_filter(
                 from_block=12504268, to_block=12504268, to_address=[safe_1_3_0_address]
             ),
             trace_filter_mock_1,
         )
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_multicall.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_oracles.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/test_utils.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from django.test import TestCase
 
-from eth_abi.packed import encode_abi_packed
+from eth_abi.packed import encode_packed
 from eth_account import Account
 from eth_utils import to_checksum_address
 from hexbytes import HexBytes
 
 from ..contracts import get_proxy_1_0_0_deployed_bytecode, get_proxy_factory_contract
 from ..utils import (
     compare_byte_code,
@@ -69,28 +69,28 @@
                 "nonce": nonce + 1,
                 "from": deployer_account.address,
             }
         )
         signed_tx = deployer_account.sign_transaction(tx)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
-        logs = proxy_factory_contract.events.ProxyCreation().processReceipt(tx_receipt)
+        logs = proxy_factory_contract.events.ProxyCreation().process_receipt(tx_receipt)
         log = logs[0]
         self.assertEqual(log["event"], "ProxyCreation")
         proxy_address = log["args"]["proxy"]
 
         proxy_creation_code = (
             proxy_factory_contract.functions.proxyCreationCode().call()
         )
         salt = self.w3.keccak(
-            encode_abi_packed(
+            encode_packed(
                 ["bytes", "uint256"], [self.w3.keccak(initializer), salt_nonce]
             )
         )
-        deployment_data = encode_abi_packed(
+        deployment_data = encode_packed(
             ["bytes", "uint256"], [proxy_creation_code, int(master_copy, 16)]
         )
         address2 = mk_contract_address_2(
             proxy_factory_contract.address, salt, deployment_data
         )
         self.assertEqual(proxy_address, address2)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/tests/utils.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 json={
                     "jsonrpc": "2.0",
                     "method": "eth_blockNumber",
                     "params": [],
                     "id": 1,
                 },
             ).ok:
-                pytest.skip("Cannot connect to poylgon node", allow_module_level=True)
+                pytest.skip("Cannot connect to polygon node", allow_module_level=True)
         except IOError:
             pytest.skip(
                 "Problem connecting to the polygon node", allow_module_level=True
             )
     just_test_if_polygon_node.checked = True
     return polygon_node_url
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/eth/utils.py` & `safe-eth-py_suraneti-5.3.0/gnosis/eth/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,17 +111,17 @@
     return "0x" + "".join(
         [c.lower() if c.isupper() else c.upper() for c in address[2:]]
     )
 
 
 def decode_string_or_bytes32(data: bytes) -> str:
     try:
-        return eth_abi.decode_abi(["string"], data)[0]
+        return eth_abi.decode(["string"], data)[0]
     except OverflowError:
-        name = eth_abi.decode_abi(["bytes32"], data)[0]
+        name = eth_abi.decode(["bytes32"], data)[0]
         end_position = name.find(b"\x00")
         if end_position == -1:
             return name.decode()
         else:
             return name[:end_position].decode()
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py_suraneti-5.3.0/gnosis/protocol/gnosis_protocol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,21 @@
     """
     Client for GnosisProtocol API. More info: https://docs.cowswap.exchange/
     """
 
     SETTLEMENT_CONTRACT_ADDRESSES = {
         EthereumNetwork.MAINNET: "0x9008D19f58AAbD9eD0D60971565AA8510560ab41",
         EthereumNetwork.GOERLI: "0x9008D19f58AAbD9eD0D60971565AA8510560ab41",
-        EthereumNetwork.XDAI: "0x9008D19f58AAbD9eD0D60971565AA8510560ab41",
+        EthereumNetwork.GNOSIS: "0x9008D19f58AAbD9eD0D60971565AA8510560ab41",
     }
 
     API_BASE_URLS = {
         EthereumNetwork.MAINNET: "https://api.cow.fi/mainnet/api/v1/",
         EthereumNetwork.GOERLI: "https://api.cow.fi/goerli/api/v1/",
-        EthereumNetwork.XDAI: "https://api.cow.fi/xdai/api/v1/",
+        EthereumNetwork.GNOSIS: "https://api.cow.fi/xdai/api/v1/",
     }
 
     def __init__(self, ethereum_network: EthereumNetwork):
         self.network = ethereum_network
         if self.network not in self.API_BASE_URLS:
             raise EthereumNetworkNotSupported(
                 f"{self.network.name} network not supported by Gnosis Protocol"
@@ -67,29 +67,30 @@
         self.http_session = requests.Session()
 
     @cached_property
     def weth_address(self) -> ChecksumAddress:
         """
         :return: Wrapped ether checksummed address
         """
-        if self.network == EthereumNetwork.MAINNET:
-            return ChecksumAddress("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2")
-        elif self.network == EthereumNetwork.RINKEBY:
-            return ChecksumAddress("0xc778417E063141139Fce010982780140Aa0cD5Ab")
-        else:  # XDAI
-            return ChecksumAddress("0x6A023CCd1ff6F2045C3309768eAd9E68F978f6e1")
+        if self.network == EthereumNetwork.GNOSIS:  # WXDAI
+            return ChecksumAddress("0xe91D153E0b41518A2Ce8Dd3D7944Fa863463a97d")
+        if self.network == EthereumNetwork.GOERLI:  # Goerli WETH9
+            return ChecksumAddress("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6")
+
+        # Mainnet WETH9
+        return ChecksumAddress("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2")
 
     def get_quote(
         self, order: Order, from_address: ChecksumAddress
     ) -> Union[Dict[str, Any], ErrorResponse]:
         url = self.base_url + "quote"
         data_json = {
             "sellToken": order.sellToken.lower(),
             "buyToken": order.buyToken.lower(),
-            "sellAmountBeforeFee": str(order.sellAmount),
+            "sellAmountAfterFee": str(order.sellAmount),
             # "validTo": order.validTo,
             "appData": HexBytes(order.appData).hex()
             if isinstance(order.appData, bytes)
             else order.appData,
             "feeAmount": str(order.feeAmount),
             "kind": order.kind,
             "partiallyFillable": order.partiallyFillable,
@@ -125,17 +126,18 @@
             order.buyAmount and order.sellAmount
         ), "Order buyAmount and sellAmount cannot be empty"
 
         url = self.base_url + "orders/"
         from_address = Account.from_key(private_key).address
         if not order.feeAmount:
             fee_amount = self.get_fee(order, from_address)
-            if "errorType" in fee_amount:  # ErrorResponse
+            if isinstance(fee_amount, int):
+                order.feeAmount = fee_amount
+            elif "errorType" in fee_amount:  # ErrorResponse
                 return fee_amount
-            order.feeAmount = fee_amount
 
         signable_hash = eip712_encode_hash(
             order.get_eip712_structured_data(
                 self.network.value, self.settlement_contract_address
             )
         )
         message = encode_defunct(primitive=signable_hash)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/protocol/order.py` & `safe-eth-py_suraneti-5.3.0/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py_suraneti-5.3.0/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from web3 import Web3
 
 from ...eth import EthereumNetwork
 from ...eth.constants import NULL_ADDRESS
 from .. import GnosisProtocolAPI, Order, OrderKind
 
 
+@pytest.skip("Having issues often", allow_module_level=True)
 class TestGnosisProtocolAPI(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.mainnet_gnosis_protocol_api = GnosisProtocolAPI(EthereumNetwork.MAINNET)
         cls.goerli_gnosis_protocol_api = GnosisProtocolAPI(EthereumNetwork.GOERLI)
         cls.mainnet_gno_token_address = "0x6810e776880C02933D47DB1b9fc05908e5386b96"
         cls.goerli_cow_token_address = "0x3430d04E42a722c5Ae52C5Bffbf1F230C2677600"
 
     def test_api_is_available(self):
         random_owner = Account.create().address
         for ethereum_network in (
             EthereumNetwork.MAINNET,
             EthereumNetwork.GOERLI,
-            EthereumNetwork.XDAI,
+            EthereumNetwork.GNOSIS,
         ):
             with self.subTest(ethereum_network=ethereum_network):
                 self.assertEqual(
                     self.goerli_gnosis_protocol_api.get_orders(random_owner), []
                 )
 
     def test_get_estimated_amount(self):
@@ -147,12 +148,11 @@
         order.sellToken = self.goerli_gnosis_protocol_api.weth_address
         order.buyToken = self.goerli_cow_token_address
         order_id = self.goerli_gnosis_protocol_api.place_order(
             order, Account().create().key
         )
 
         if type(order_id) is dict:
-            if order_id["errorType"] == "NoLiquidity":
-                pytest.xfail("NoLiquidity Error")
-
-        self.assertEqual(order_id[:2], "0x")
-        self.assertEqual(len(order_id), 114)
+            pytest.xfail(order_id["errorType"])
+        else:
+            self.assertEqual(order_id[:2], "0x")
+            self.assertEqual(len(order_id), 114)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/__init__.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/api/base_api.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/api/relay_service_api.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/api/transaction_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 from .base_api import SafeAPIException, SafeBaseAPI
 
 logger = logging.getLogger(__name__)
 
 
 class TransactionServiceApi(SafeBaseAPI):
     URL_BY_NETWORK = {
-        EthereumNetwork.ARBITRUM: "https://safe-transaction-arbitrum.safe.global",
-        EthereumNetwork.AURORA: "https://safe-transaction-aurora.safe.global",
-        EthereumNetwork.AVALANCHE: "https://safe-transaction-avalanche.safe.global",
-        EthereumNetwork.BINANCE: "https://safe-transaction-bsc.safe.global",
+        EthereumNetwork.ARBITRUM_ONE: "https://safe-transaction-arbitrum.safe.global",
+        EthereumNetwork.AURORA_MAINNET: "https://safe-transaction-aurora.safe.global",
+        EthereumNetwork.AVALANCHE_C_CHAIN: "https://safe-transaction-avalanche.safe.global",
+        EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: "https://safe-transaction-bsc.safe.global",
         EthereumNetwork.ENERGY_WEB_CHAIN: "https://safe-transaction-ewc.safe.global",
         EthereumNetwork.GOERLI: "https://safe-transaction-goerli.safe.global",
         EthereumNetwork.MAINNET: "https://safe-transaction-mainnet.safe.global",
-        EthereumNetwork.MATIC: "https://safe-transaction-polygon.safe.global",
-        EthereumNetwork.OPTIMISTIC: "https://safe-transaction-optimism.safe.global",
-        EthereumNetwork.VOLTA: "https://safe-transaction-volta.safe.global",
-        EthereumNetwork.XDAI: "https://safe-transaction-gnosis-chain.safe.global",
+        EthereumNetwork.POLYGON: "https://safe-transaction-polygon.safe.global",
+        EthereumNetwork.OPTIMISM: "https://safe-transaction-optimism.safe.global",
+        EthereumNetwork.ENERGY_WEB_VOLTA_TESTNET: "https://safe-transaction-volta.safe.global",
+        EthereumNetwork.GNOSIS: "https://safe-transaction-gnosis-chain.safe.global",
     }
 
     @classmethod
     def create_delegate_message_hash(cls, delegate_address: str) -> str:
         totp = int(time.time()) // 3600
         hash_to_sign = Web3.keccak(text=delegate_address + str(totp))
         return hash_to_sign
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/exceptions.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/multi_send.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/proxy_factory.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/safe.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/safe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import dataclasses
 import math
 from enum import Enum
 from functools import cached_property
 from logging import getLogger
 from typing import Callable, List, NamedTuple, Optional, Union
 
-from eth_abi import encode_abi
+from eth_abi import encode as encode_abi
 from eth_abi.exceptions import DecodingError
-from eth_abi.packed import encode_abi_packed
+from eth_abi.packed import encode_packed
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
 from eth_typing import ChecksumAddress, Hash32
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.contract import Contract
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import Web3Exception
 from web3.types import BlockIdentifier, Wei
 
 from gnosis.eth import EthereumClient, EthereumTxSent
 from gnosis.eth.constants import GAS_CALL_DATA_BYTE, NULL_ADDRESS, SENTINEL_ADDRESS
 from gnosis.eth.contracts import (
     get_compatibility_fallback_handler_V1_3_0_contract,
     get_delegate_constructor_proxy_contract,
@@ -120,15 +120,15 @@
     @cached_property
     def domain_separator(self) -> Optional[bytes]:
         """
         :return: EIP721 DomainSeparator for the Safe. Returns `None` if not supported (for Safes < 1.0.0)
         """
         try:
             return self.retrieve_domain_separator()
-        except (ValueError, BadFunctionCallOutput, DecodingError):
+        except (Web3Exception, DecodingError, ValueError):
             logger.warning("Safe %s does not support domainSeparator", self.address)
             return None
 
     @staticmethod
     def create(
         ethereum_client: EthereumClient,
         deployer_account: LocalAccount,
@@ -729,15 +729,15 @@
         :param data:
         :return: Estimation using web3 `estimate_gas`
         """
         try:
             return self.ethereum_client.estimate_gas(
                 to, from_=self.address, value=value, data=data
             )
-        except ValueError as exc:
+        except (Web3Exception, ValueError) as exc:
             raise CannotEstimateGas(
                 f"Cannot estimate gas with `eth_estimateGas`: {exc}"
             ) from exc
 
     def estimate_tx_gas_by_trying(
         self, to: str, value: int, data: Union[bytes, str], operation: int
     ):
@@ -858,15 +858,15 @@
 
         safe_message_hash = Web3.keccak(
             encode_abi(
                 ["bytes32", "bytes32"], [self.SAFE_MESSAGE_TYPEHASH, message_hash]
             )
         )
         return Web3.keccak(
-            encode_abi_packed(
+            encode_packed(
                 ["bytes1", "bytes1", "bytes32", "bytes32"],
                 [
                     bytes.fromhex("19"),
                     bytes.fromhex("01"),
                     self.domain_separator,
                     safe_message_hash,
                 ],
@@ -917,15 +917,15 @@
                 master_copy,
                 modules,
                 nonce,
                 owners,
                 threshold,
                 version,
             )
-        except (ValueError, BadFunctionCallOutput) as e:
+        except (Web3Exception, ValueError) as e:
             raise CannotRetrieveSafeInfoException(self.address) from e
 
     def retrieve_domain_separator(
         self, block_identifier: Optional[BlockIdentifier] = "latest"
     ) -> str:
         return self.contract.functions.domainSeparator().call(
             block_identifier=block_identifier
@@ -980,15 +980,15 @@
             # Contracts with Safe version < 1.1.0 were not paginated
             contract = get_safe_V1_0_0_contract(
                 self.ethereum_client.w3, address=self.address
             )
             return contract.functions.getModules().call(
                 block_identifier=block_identifier
             )
-        except BadFunctionCallOutput:
+        except Web3Exception:
             pass
 
         contract = self.contract
         address = SENTINEL_ADDRESS
         all_modules: List[str] = []
         while True:
             (modules, address) = contract.functions.getModulesPaginated(
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_create2_tx.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_create2_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 from logging import getLogger
 from typing import List, NamedTuple, Optional
 
-from eth_abi.packed import encode_abi_packed
+from eth_abi.packed import encode_packed
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.types import TxParams, Wei
 
 from gnosis.eth.constants import GAS_CALL_DATA_BYTE, NULL_ADDRESS
 from gnosis.eth.contracts import (
     get_proxy_factory_contract,
@@ -210,19 +210,19 @@
             return fixed_creation_cost
 
     def calculate_create2_address(self, safe_setup_data: bytes, salt_nonce: int):
         proxy_creation_code = (
             self.proxy_factory_contract.functions.proxyCreationCode().call()
         )
         salt = self.w3.keccak(
-            encode_abi_packed(
+            encode_packed(
                 ["bytes", "uint256"], [self.w3.keccak(safe_setup_data), salt_nonce]
             )
         )
-        deployment_data = encode_abi_packed(
+        deployment_data = encode_packed(
             ["bytes", "uint256"],
             [proxy_creation_code, int(self.master_copy_address, 16)],
         )
         return mk_contract_address_2(
             self.proxy_factory_contract.address, salt, deployment_data
         )
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_creation_tx.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_creation_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import rlp
 from eth.vm.forks.frontier.transactions import FrontierTransaction
 from eth_keys.exceptions import BadSignature
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.contract import ContractConstructor
+from web3.exceptions import Web3Exception
 
 from gnosis.eth.constants import GAS_CALL_DATA_BYTE, NULL_ADDRESS, SECPK1_N
 from gnosis.eth.contracts import (
     get_erc20_contract,
     get_paying_proxy_contract,
     get_safe_V0_0_1_contract,
 )
@@ -307,15 +308,15 @@
             # If it was a new tx sending 5000 tokens would be more expensive than sending 1 because of data costs
             try:
                 gas += (
                     get_erc20_contract(self.w3, payment_token)
                     .functions.transfer(funder, 1)
                     .estimate_gas({"from": payment_token})
                 )
-            except ValueError as exc:
+            except Web3Exception as exc:
                 if "transfer amount exceeds balance" in str(exc):
                     return 70000
                 raise InvalidERC20Token from exc
 
         return gas
 
     def _get_initial_setup_safe_data(self, owners: List[str], threshold: int) -> bytes:
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_signature.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from logging import getLogger
 from typing import List, Union
 
-from eth_abi import decode_single, encode_single
+from eth_abi import decode as decode_abi
+from eth_abi import encode as encode_abi
 from eth_abi.exceptions import DecodingError
 from eth_account.messages import defunct_hash_message
 from eth_typing import ChecksumAddress
 from hexbytes import HexBytes
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import Web3Exception
 
 from gnosis.eth import EthereumClient
 from gnosis.eth.contracts import get_safe_contract, get_safe_V1_1_1_contract
 from gnosis.eth.utils import fast_to_checksum_address
 from gnosis.safe.signatures import (
     get_signing_address,
     signature_split,
@@ -54,19 +55,19 @@
 def uint_to_address(value: int) -> ChecksumAddress:
     """
     Convert a Solidity `uint` value to a checksummed `address`, removing
     invalid padding bytes if present
 
     :return: Checksummed address
     """
-    encoded = encode_single("uint", value)
+    encoded = encode_abi(["uint"], [value])
     # Remove padding bytes, as Solidity will ignore it but `eth_abi` will not
     encoded_without_padding_bytes = b"\x00" * 12 + encoded[-20:]
     return fast_to_checksum_address(
-        decode_single("address", encoded_without_padding_bytes)
+        decode_abi(["address"], encoded_without_padding_bytes)[0]
     )
 
 
 class SafeSignature(ABC):
     def __init__(self, signature: EthereumBytes, safe_tx_hash: EthereumBytes):
         self.signature = HexBytes(signature)
         self.safe_tx_hash = HexBytes(safe_tx_hash)
@@ -191,33 +192,37 @@
     @property
     def signature_type(self) -> SafeSignatureType:
         return SafeSignatureType.CONTRACT_SIGNATURE
 
     def export_signature(self) -> HexBytes:
         """
         Fix offset (s) and append `contract_signature` at the end of the signature
+
         :return:
         """
+        # encode_abi adds {32 bytes offset}{32 bytes size}. We don't need offset
+        contract_signature = encode_abi(["bytes"], [self.contract_signature])[32:]
+        dynamic_offset = 65
+
         return HexBytes(
-            signature_to_bytes(self.v, self.r, 65)
-            + encode_single("bytes", self.contract_signature)
+            signature_to_bytes(self.v, self.r, dynamic_offset) + contract_signature
         )
 
     def is_valid(self, ethereum_client: EthereumClient, *args) -> bool:
         safe_contract = get_safe_V1_1_1_contract(ethereum_client.w3, self.owner)
         # Newest versions of the Safe contract have `isValidSignature` on the compatibility fallback handler
         for block_identifier in ("pending", "latest"):
             try:
                 return safe_contract.functions.isValidSignature(
                     self.safe_tx_hash, self.contract_signature
                 ).call(block_identifier=block_identifier) in (
                     self.EIP1271_MAGIC_VALUE,
                     self.EIP1271_MAGIC_VALUE_UPDATED,
                 )
-            except (ValueError, BadFunctionCallOutput, DecodingError):
+            except (Web3Exception, DecodingError, ValueError):
                 # Error using `pending` block identifier or contract does not exist
                 logger.warning(
                     "Cannot check EIP1271 signature from contract %s", self.owner
                 )
         return False
 
 
@@ -246,15 +251,16 @@
             try:
                 return (
                     safe_contract.functions.approvedHashes(
                         self.owner, self.safe_tx_hash
                     ).call(block_identifier=block_identifier)
                     == 1
                 )
-            except BadFunctionCallOutput as e:  # Error using `pending` block identifier
+            except (Web3Exception, DecodingError, ValueError) as e:
+                # Error using `pending` block identifier
                 exception = e
         raise exception  # This should never happen
 
 
 class SafeSignatureEthSign(SafeSignature):
     @property
     def owner(self):
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/safe_tx.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/safe_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import cached_property
 from typing import Any, Dict, List, NoReturn, Optional, Tuple, Type
 
 from eth_account import Account
 from hexbytes import HexBytes
 from packaging.version import Version
-from web3.exceptions import BadFunctionCallOutput, ContractLogicError
+from web3.exceptions import Web3Exception
 from web3.types import BlockIdentifier, TxParams, Wei
 
 from gnosis.eth import EthereumClient
 from gnosis.eth.constants import NULL_ADDRESS
 from gnosis.eth.contracts import get_safe_contract
 from gnosis.eth.eip712 import eip712_encode_hash
 from gnosis.eth.ethereum_client import TxSpeed
@@ -304,15 +304,15 @@
             success = self.w3_tx.call(parameters, block_identifier=block_identifier)
 
             if not success:
                 raise InvalidInternalTx(
                     "Success bit is %d, should be equal to 1" % success
                 )
             return success
-        except (ContractLogicError, BadFunctionCallOutput, ValueError) as exc:
+        except (Web3Exception, ValueError) as exc:
             # e.g. web3.exceptions.ContractLogicError: execution reverted: Invalid owner provided
             return self._raise_safe_vm_exception(str(exc))
         except ValueError as exc:  # Parity
             """
             Parity throws a ValueError, e.g.
             {'code': -32015,
              'message': 'VM execution error.',
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/serializers.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/signatures.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_proxy_factory.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         keys = [x[1] for x in owners_with_keys]
         threshold = len(owners_with_keys)
 
         safe = self.deploy_test_safe(threshold=threshold, owners=owners)
         my_safe_address = safe.address
 
         # The balance we will send to the safe
-        safe_balance = w3.toWei(0.02, "ether")
+        safe_balance = w3.to_wei(0.02, "ether")
 
         # Send something to the owner[0], who will be sending the tx
         owner0_balance = safe_balance
         self.send_tx({"to": owners[0], "value": owner0_balance}, funder_account)
 
         my_safe_contract = get_safe_contract(w3, my_safe_address)
         safe = Safe(my_safe_address, self.ethereum_client)
@@ -270,15 +270,15 @@
     def test_send_multisig_tx_gas_token(self):
         # Create safe with one owner, fund the safe and the owner with `safe_balance`
         receiver, _ = get_eth_address_with_key()
         threshold = 1
         funder_account = self.ethereum_test_account
         funder = funder_account.address
         safe_balance_ether = 0.02
-        safe_balance = self.w3.toWei(safe_balance_ether, "ether")
+        safe_balance = self.w3.to_wei(safe_balance_ether, "ether")
         owner_account = self.create_account(initial_ether=safe_balance_ether)
         owner = owner_account.address
 
         safe = self.deploy_test_safe(
             threshold=threshold, owners=[owner], initial_funding_wei=safe_balance
         )
         my_safe_address = safe.address
@@ -476,15 +476,15 @@
             {"from": self.w3.eth.accounts[0]}
         )
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         nester = self.w3.eth.contract(address=tx_receipt.contractAddress, abi=abi)
 
         safe = self.deploy_test_safe(
             owners=[self.ethereum_test_account.address],
-            initial_funding_wei=self.w3.toWei(0.1, "ether"),
+            initial_funding_wei=self.w3.to_wei(0.1, "ether"),
         )
         nester_tx = nester.functions.useGas(80).build_transaction(
             {"gasPrice": 1, "from": safe.address, "gas": 1}
         )
         nester_data = nester_tx["data"]
 
         safe_tx_gas_no_call = safe.estimate_tx_gas_with_safe(
@@ -525,18 +525,18 @@
 
         # Tx was successfully executed if refund_receiver gets ether
         self.assertGreater(self.ethereum_client.get_balance(refund_receiver), 0)
 
     def test_estimate_tx_gas_with_web3(self):
         safe = self.deploy_test_safe(
             owners=[self.ethereum_test_account.address],
-            initial_funding_wei=self.w3.toWei(0.1, "ether"),
+            initial_funding_wei=self.w3.to_wei(0.1, "ether"),
         )
         to = Account.create().address
-        value = self.w3.toWei(0.01, "ether")
+        value = self.w3.to_wei(0.01, "ether")
         data = b""
         gas_estimated_web3 = safe.estimate_tx_gas_with_web3(to, value, data)
         gas_estimated_safe = safe.estimate_tx_gas_with_safe(to, value, data, 0)
         self.assertGreater(
             gas_estimated_safe, gas_estimated_web3
         )  # Web3 estimation should use less gas
         self.assertGreater(gas_estimated_web3, 0)
@@ -741,22 +741,24 @@
         accounts = [
             self.create_account(initial_ether=0.01) for _ in range(number_owners)
         ]
         accounts.sort(key=lambda x: x.address.lower())
         owners = [account.address for account in accounts]
 
         safe = self.deploy_test_safe(
-            threshold=2, owners=owners, initial_funding_wei=self.w3.toWei(0.01, "ether")
+            threshold=2,
+            owners=owners,
+            initial_funding_wei=self.w3.to_wei(0.01, "ether"),
         )
         safe_address = safe.address
         safe = Safe(safe_address, self.ethereum_client)
         safe_instance = get_safe_contract(self.w3, safe_address)
 
         to, _ = get_eth_address_with_key()
-        value = self.w3.toWei(0.001, "ether")
+        value = self.w3.to_wei(0.001, "ether")
         data = b""
         operation = 0
         safe_tx_gas = 500000
         data_gas = 500000
         gas_price = 1
         gas_token = NULL_ADDRESS
         refund_receiver = NULL_ADDRESS
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         tx_receipt = w3.eth.wait_for_transaction_receipt(ethereum_tx_sent.tx_hash)
         self.assertEqual(tx_receipt.status, 1)
 
         # Funder balance must be bigger after a Safe deployment, as Safe deployment is a little overpriced
         self.assertGreater(
             self.ethereum_client.get_balance(funder_account.address), funder_balance
         )
-        logs = self.proxy_factory_contract.events.ProxyCreation().processReceipt(
+        logs = self.proxy_factory_contract.events.ProxyCreation().process_receipt(
             tx_receipt
         )
         log = logs[0]
         self.assertIsNone(tx_receipt.contractAddress)
         self.assertEqual(log["event"], "ProxyCreation")
         proxy_address = log["args"]["proxy"]
         self.assertEqual(proxy_address, safe_creation_tx.safe_address)
@@ -130,15 +130,15 @@
         tx_receipt = w3.eth.wait_for_transaction_receipt(ethereum_tx_sent.tx_hash)
         self.assertEqual(tx_receipt.status, 1)
 
         # Funder balance must be bigger after a Safe deployment, as Safe deployment is a little overpriced
         self.assertGreater(
             self.ethereum_client.get_balance(funder_account.address), funder_balance
         )
-        logs = self.proxy_factory_contract.events.ProxyCreation().processReceipt(
+        logs = self.proxy_factory_contract.events.ProxyCreation().process_receipt(
             tx_receipt
         )
         log = logs[0]
         self.assertIsNone(tx_receipt.contractAddress)
         self.assertEqual(log["event"], "ProxyCreation")
         proxy_address = log["args"]["proxy"]
         self.assertEqual(proxy_address, safe_creation_tx.safe_address)
@@ -195,15 +195,15 @@
             safe_creation_tx.safe_setup_data,
             salt_nonce,
             gas=safe_creation_tx.gas,
             gas_price=safe_creation_tx.gas_price,
         )
         tx_receipt = w3.eth.wait_for_transaction_receipt(ethereum_tx_sent.tx_hash)
         self.assertEqual(tx_receipt.status, 1)
-        logs = self.proxy_factory_contract.events.ProxyCreation().processReceipt(
+        logs = self.proxy_factory_contract.events.ProxyCreation().process_receipt(
             tx_receipt
         )
         log = logs[0]
         self.assertIsNone(tx_receipt.contractAddress)
         self.assertEqual(log["event"], "ProxyCreation")
         proxy_address = log["args"]["proxy"]
         self.assertEqual(proxy_address, safe_creation_tx.safe_address)
@@ -266,15 +266,15 @@
             safe_creation_tx.safe_setup_data,
             salt_nonce,
             gas=safe_creation_tx.gas,
             gas_price=safe_creation_tx.gas_price,
         )
         tx_receipt = w3.eth.wait_for_transaction_receipt(ethereum_tx_sent.tx_hash)
         self.assertEqual(tx_receipt.status, 1)
-        logs = self.proxy_factory_contract.events.ProxyCreation().processReceipt(
+        logs = self.proxy_factory_contract.events.ProxyCreation().process_receipt(
             tx_receipt
         )
         log = logs[0]
         self.assertIsNone(tx_receipt.contractAddress)
         self.assertEqual(log["event"], "ProxyCreation")
         proxy_address = log["args"]["proxy"]
         self.assertEqual(proxy_address, safe_creation_tx.safe_address)
@@ -305,15 +305,15 @@
         self.assertEqual(
             erc20_contract.functions.balanceOf(erc20_deployer.address).call(),
             token_amount,
         )
 
         # Send something to the erc20 deployer
         self.send_tx(
-            {"to": erc20_deployer.address, "value": w3.toWei(1, "ether")},
+            {"to": erc20_deployer.address, "value": w3.to_wei(1, "ether")},
             funder_account,
         )
 
         safe_creation_tx = SafeCreate2TxBuilder(
             w3=w3,
             master_copy_address=self.safe_contract_address,
             proxy_factory_address=self.proxy_factory_contract_address,
@@ -349,15 +349,15 @@
             safe_creation_tx.safe_setup_data,
             salt_nonce,
             gas=safe_creation_tx.gas,
             gas_price=safe_creation_tx.gas_price,
         )
         tx_receipt = w3.eth.wait_for_transaction_receipt(ethereum_tx_sent.tx_hash)
         self.assertEqual(tx_receipt.status, 1)
-        logs = self.proxy_factory_contract.events.ProxyCreation().processReceipt(
+        logs = self.proxy_factory_contract.events.ProxyCreation().process_receipt(
             tx_receipt
         )
         self.assertEqual(len(logs), 1)
         log = logs[0]
         self.assertIsNone(tx_receipt.contractAddress)
         self.assertEqual(log["event"], "ProxyCreation")
         proxy_address = log["args"]["proxy"]
@@ -415,15 +415,15 @@
                 safe_creation_tx.safe_setup_data,
                 salt_nonce,
                 gas=safe_creation_tx.gas,
                 gas_price=safe_creation_tx.gas_price,
             )
             tx_receipt = w3.eth.wait_for_transaction_receipt(ethereum_tx_sent.tx_hash)
             self.assertEqual(tx_receipt.status, 1)
-            logs = self.proxy_factory_contract.events.ProxyCreation().processReceipt(
+            logs = self.proxy_factory_contract.events.ProxyCreation().process_receipt(
                 tx_receipt
             )
             log = logs[0]
             self.assertIsNone(tx_receipt.contractAddress)
             self.assertEqual(log["event"], "ProxyCreation")
             proxy_address = log["args"]["proxy"]
             self.assertEqual(proxy_address, safe_creation_tx.safe_address)
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_creation_tx.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             master_copy=self.safe_contract_V0_0_1_address,
             gas_price=gas_price,
             funder=NULL_ADDRESS,
         )
 
         logger.info(
             "Send %d gwei to deployer %s",
-            w3.fromWei(safe_creation_tx.payment_ether, "gwei"),
+            w3.from_wei(safe_creation_tx.payment_ether, "gwei"),
             safe_creation_tx.deployer_address,
         )
 
         self.send_tx(
             {
                 "to": safe_creation_tx.deployer_address,
                 "value": safe_creation_tx.payment_ether,
@@ -63,15 +63,15 @@
         tx_receipt = w3.eth.wait_for_transaction_receipt(tx_hash)
         self.assertEqual(tx_receipt.contractAddress, safe_creation_tx.safe_address)
 
         deployed_safe_proxy_contract = get_safe_contract(w3, tx_receipt.contractAddress)
 
         logger.info(
             "Deployer account has still %d gwei left (will be lost)",
-            w3.fromWei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
+            w3.from_wei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
         )
 
         self.assertEqual(
             deployed_safe_proxy_contract.functions.getThreshold().call(), threshold
         )
         self.assertEqual(
             deployed_safe_proxy_contract.functions.getOwners().call(), owners
@@ -93,15 +93,15 @@
             master_copy=self.safe_contract_V0_0_1_address,
             gas_price=gas_price,
             funder=NULL_ADDRESS,
         )
 
         logger.info(
             "Send %d gwei to deployer %s",
-            w3.fromWei(safe_creation_tx.payment_ether - 1, "gwei"),
+            w3.from_wei(safe_creation_tx.payment_ether - 1, "gwei"),
             safe_creation_tx.deployer_address,
         )
         self.send_tx(
             {
                 "to": safe_creation_tx.deployer_address,
                 "value": safe_creation_tx.payment_ether - 1,
             },
@@ -132,36 +132,36 @@
             master_copy=self.safe_contract_V0_0_1_address,
             gas_price=gas_price,
             funder=funder_account.address,
         )
 
         user_external_account = Account.create()
         # Send some ether to that account
-        safe_balance = w3.toWei(0.01, "ether")
+        safe_balance = w3.to_wei(0.01, "ether")
         self.send_tx(
             {"to": user_external_account.address, "value": safe_balance * 2},
             funder_account,
         )
 
         logger.info(
             "Send %d ether to safe %s",
-            w3.fromWei(safe_balance, "ether"),
+            w3.from_wei(safe_balance, "ether"),
             safe_creation_tx.safe_address,
         )
         self.send_tx(
             {"to": safe_creation_tx.safe_address, "value": safe_balance},
             user_external_account,
         )
         self.assertEqual(
             w3.eth.get_balance(safe_creation_tx.safe_address), safe_balance
         )
 
         logger.info(
             "Send %d gwei to deployer %s",
-            w3.fromWei(safe_creation_tx.payment_ether, "gwei"),
+            w3.from_wei(safe_creation_tx.payment_ether, "gwei"),
             safe_creation_tx.deployer_address,
         )
         self.send_tx(
             {
                 "to": safe_creation_tx.deployer_address,
                 "value": safe_creation_tx.payment_ether,
             },
@@ -182,15 +182,15 @@
         self.assertEqual(
             w3.eth.get_balance(funder_account.address),
             funder_balance + safe_creation_tx.payment,
         )
 
         logger.info(
             "Deployer account has still %d gwei left (will be lost)",
-            w3.fromWei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
+            w3.from_wei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
         )
 
         deployed_safe_proxy_contract = get_safe_contract(w3, tx_receipt.contractAddress)
 
         self.assertEqual(
             deployed_safe_proxy_contract.functions.getThreshold().call(), threshold
         )
@@ -207,15 +207,15 @@
         s = generate_valid_s()
 
         erc20_deployer = Account.create()
         funder_account = self.ethereum_test_account
 
         # Send something to the erc20 deployer
         self.send_tx(
-            {"to": erc20_deployer.address, "value": w3.toWei(1, "ether")},
+            {"to": erc20_deployer.address, "value": w3.to_wei(1, "ether")},
             funder_account,
         )
 
         funder = funder_account.address
         owners = [get_eth_address_with_key()[0] for _ in range(2)]
         threshold = len(owners) - 1
         gas_price = self.gas_price
@@ -250,15 +250,15 @@
         )
         self.assertEqual(
             erc20_contract.functions.balanceOf(safe_address).call(), payment
         )
 
         logger.info(
             "Send %d ether to deployer %s",
-            w3.fromWei(payment, "ether"),
+            w3.from_wei(payment, "ether"),
             deployer_address,
         )
         self.send_tx(
             {
                 "to": safe_creation_tx.deployer_address,
                 "value": safe_creation_tx.payment,
             },
@@ -276,15 +276,15 @@
         self.assertEqual(tx_receipt.contractAddress, safe_address)
         self.assertEqual(w3.eth.get_balance(funder), funder_balance)
         self.assertEqual(erc20_contract.functions.balanceOf(funder).call(), payment)
         self.assertEqual(erc20_contract.functions.balanceOf(safe_address).call(), 0)
 
         logger.info(
             "Deployer account has still %d gwei left (will be lost)",
-            w3.fromWei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
+            w3.from_wei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
         )
 
         deployed_safe_proxy_contract = get_safe_contract(w3, tx_receipt.contractAddress)
 
         self.assertEqual(
             deployed_safe_proxy_contract.functions.getThreshold().call(), threshold
         )
@@ -379,24 +379,24 @@
         self.assertEqual(
             safe_creation_tx.payment_ether,
             safe_creation_tx.gas * safe_creation_tx.gas_price,
         )
 
         deployer_address = safe_creation_tx.deployer_address
         safe_address = safe_creation_tx.safe_address
-        safe_balance = w3.toWei(0.01, "ether")
+        safe_balance = w3.to_wei(0.01, "ether")
         logger.info(
-            "Send %d ether to safe %s", w3.fromWei(safe_balance, "ether"), safe_address
+            "Send %d ether to safe %s", w3.from_wei(safe_balance, "ether"), safe_address
         )
         self.send_tx({"to": safe_address, "value": safe_balance}, funder_account)
         self.assertEqual(w3.eth.get_balance(safe_address), safe_balance)
 
         logger.info(
             "Send %d ether to deployer %s",
-            w3.fromWei(safe_creation_tx.payment_ether, "ether"),
+            w3.from_wei(safe_creation_tx.payment_ether, "ether"),
             deployer_address,
         )
         self.send_tx(
             {"to": deployer_address, "value": safe_creation_tx.payment_ether},
             funder_account,
         )
 
@@ -419,15 +419,15 @@
         self.assertEqual(
             w3.eth.get_balance(funder_account.address),
             funder_balance + safe_creation_tx.payment,
         )
 
         logger.info(
             "Deployer account has still %d gwei left (will be lost)",
-            w3.fromWei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
+            w3.from_wei(w3.eth.get_balance(safe_creation_tx.deployer_address), "gwei"),
         )
 
         deployed_safe_proxy_contract = get_safe_contract(w3, safe_address)
 
         self.assertEqual(
             deployed_safe_proxy_contract.functions.getThreshold().call(), threshold
         )
@@ -444,15 +444,15 @@
         w3 = self.w3
         funder_account = self.ethereum_test_account
         number_of_accounts = 10
         for i in range(2, number_of_accounts):
             s = generate_valid_s()
             owners = [get_eth_address_with_key()[0] for _ in range(i + 1)]
             threshold = len(owners)
-            gas_price = w3.toWei(15, "gwei")
+            gas_price = w3.to_wei(15, "gwei")
 
             safe_creation_tx = SafeCreationTx(
                 w3=w3,
                 owners=owners,
                 threshold=threshold,
                 signature_s=s,
                 master_copy=self.safe_contract_V0_0_1_address,
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from django.test import TestCase
 
-from eth_abi import encode_single
-from eth_abi.packed import encode_single_packed
+from eth_abi import encode as encode_abi
+from eth_abi.packed import encode_packed
 from eth_account import Account
 from eth_account.messages import defunct_hash_message
 from hexbytes import HexBytes
 from web3 import Web3
 
 from ...eth.tests.ethereum_test_case import EthereumTestCaseMixin
 from ..safe_signature import (
@@ -123,16 +123,16 @@
         self.assertTrue(str(safe_signature))  # Test __str__
 
     def test_defunct_hash_message(self):
         safe_tx_hash = HexBytes(
             "0x4c9577d1b1b8dec52329a983ae26238b65f74b7dd9fb28d74ad9548e92aaf196"
         )
         ethereum_signed_message = "\x19Ethereum Signed Message:\n32"
-        encoded_message = encode_single_packed(
-            "(string,bytes32)", (ethereum_signed_message, HexBytes(safe_tx_hash))
+        encoded_message = encode_packed(
+            ["(string,bytes32)"], [(ethereum_signed_message, HexBytes(safe_tx_hash))]
         )
         encoded_hash = Web3.keccak(encoded_message)
         self.assertEqual(encoded_hash, defunct_hash_message(primitive=safe_tx_hash))
 
     def test_parse_signature(self):
         owner_1 = "0x05c85Ab5B09Eb8A55020d72daf6091E04e264af9"
         owner_2 = "0xADb7CB706e9A1bd9F96a397da340bF34a9984E1E"
@@ -176,24 +176,25 @@
             self.assertEqual(SafeSignature.parse_signature(value, safe_tx_hash), [])
 
 
 class TestSafeContractSignature(SafeTestCaseMixin, TestCase):
     def test_contract_signature(self):
         owner_1 = self.ethereum_test_account
         safe = self.deploy_test_safe_v1_1_1(
-            owners=[owner_1.address], initial_funding_wei=Web3.toWei(0.01, "ether")
+            owners=[owner_1.address], initial_funding_wei=Web3.to_wei(0.01, "ether")
         )
         safe_contract = safe.contract
         safe_tx_hash = Web3.keccak(text="test")
         signature_r = HexBytes(safe.address.replace("0x", "").rjust(64, "0"))
         signature_s = HexBytes(
-            "0" * 62 + "41"
+            "41".rjust(64, "0")
         )  # Position of end of signature `0x41 == 65`
         signature_v = HexBytes("00")
-        contract_signature = encode_single("bytes", b"")
+        # First 32 bytes signature size, in this case 0
+        contract_signature = HexBytes("0" * 64)
         signature = signature_r + signature_s + signature_v + contract_signature
 
         safe_signature = SafeSignature.parse_signature(signature, safe_tx_hash)[0]
         self.assertFalse(safe_signature.is_valid(self.ethereum_client, None))
 
         # Check with previously signedMessage
         tx = safe_contract.functions.signMessage(safe_tx_hash).build_transaction(
@@ -212,22 +213,22 @@
         safe_signature = SafeSignature.parse_signature(signature, safe_tx_hash_2)[0]
         self.assertFalse(safe_signature.is_valid(self.ethereum_client, None))
 
         safe_tx_hash_2_message_hash = safe_contract.functions.getMessageHash(
             safe_tx_hash_2
         ).call()
         contract_signature = owner_1.signHash(safe_tx_hash_2_message_hash)["signature"]
-        encoded_contract_signature = encode_single(
-            "bytes", contract_signature
-        )  # It will add size of bytes
-        # `32` bytes with the abi encoded size of array. 65 bytes will be padded to next multiple of 32 -> 96
-        # 96 - 65 = `31`
-        self.assertEqual(
-            len(encoded_contract_signature), len(contract_signature) + 32 + 31
+
+        encoded_contract_signature_with_offset = encode_abi(
+            ["bytes"], [contract_signature]
         )
+        # {32 bytes - offset for the length}{32 bytes - length = 65 bytes}{65 bytes - content}
+        self.assertEqual(len(encoded_contract_signature_with_offset), 160)
+        # Safe dynamic part does not use the offset
+        encoded_contract_signature = encoded_contract_signature_with_offset[32:]
         crafted_signature = (
             signature_r + signature_s + signature_v + encoded_contract_signature
         )
         safe_signature = SafeSignature.parse_signature(
             crafted_signature, safe_tx_hash_2
         )[0]
         self.assertEqual(contract_signature, safe_signature.contract_signature)
@@ -235,15 +236,15 @@
 
     def test_contract_multiple_signatures(self):
         """
         Test decode of multiple `CONTRACT_SIGNATURE` together
         """
         owner_1 = self.ethereum_test_account
         safe = self.deploy_test_safe_v1_1_1(
-            owners=[owner_1.address], initial_funding_wei=Web3.toWei(0.01, "ether")
+            owners=[owner_1.address], initial_funding_wei=Web3.to_wei(0.01, "ether")
         )
         safe_contract = safe.contract
         safe_tx_hash = Web3.keccak(text="test")
 
         tx = safe_contract.functions.signMessage(safe_tx_hash).build_transaction(
             {"from": safe.address}
         )
@@ -251,32 +252,34 @@
         safe_tx.sign(owner_1.key)
         safe_tx.execute(owner_1.key)
 
         # Check multiple signatures. In this case we reuse signatures for the same owner, it won't make sense
         # in real life
         signature_r_1 = HexBytes(safe.address.replace("0x", "").rjust(64, "0"))
         signature_s_1 = HexBytes(
-            "0" * 62 + "82"
+            "82".rjust(64, "0")
         )  # Position of end of signature `0x82 == (65 * 2)`
         signature_v_1 = HexBytes("00")
         contract_signature_1 = b""
-        encoded_contract_signature_1 = encode_single("bytes", contract_signature_1)
+        encoded_contract_signature_1 = encode_abi(["bytes"], [contract_signature_1])[
+            32:
+        ]  # It will {32 bytes offset}{32 bytes size}, we don't need offset
 
         signature_r_2 = HexBytes(safe.address.replace("0x", "").rjust(64, "0"))
         signature_s_2 = HexBytes(
-            "0" * 62 + "c2"
-        )  # Position of end of signature `0xc2 == (65 * 2) + 64`
+            "a2".rjust(64, "0")
+        )  # Position of end of signature `0xa2 == (65 * 2) + 32`
         signature_v_2 = HexBytes("00")
         safe_tx_hash_message_hash = safe_contract.functions.getMessageHash(
             safe_tx_hash
         ).call()
         contract_signature_2 = owner_1.signHash(safe_tx_hash_message_hash)["signature"]
-        encoded_contract_signature_2 = encode_single(
-            "bytes", contract_signature_2
-        )  # It will add size of bytes
+        encoded_contract_signature_2 = encode_abi(["bytes"], [contract_signature_2])[
+            32:
+        ]  # It will {32 bytes offset}{32 bytes size}, we don't need offset
 
         signature = (
             signature_r_1
             + signature_s_1
             + signature_v_1
             + signature_r_2
             + signature_s_2
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_safe_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def test_multi_send_safe_tx(self):
         owners = [Account.create() for _ in range(2)]
         owner_addresses = [owner.address for owner in owners]
         threshold = 1
         safe = self.deploy_test_safe(
             owners=owner_addresses,
             threshold=threshold,
-            initial_funding_wei=self.w3.toWei(0.1, "ether"),
+            initial_funding_wei=self.w3.to_wei(0.1, "ether"),
         )
         safe_contract = safe.contract
         to = self.multi_send_contract.address
         value = 0
         safe_tx_gas = 600000
         base_gas = 200000
 
@@ -82,18 +82,18 @@
     def test_send_safe_tx(self):
         owners = [Account.create() for _ in range(2)]
         owner_addresses = [owner.address for owner in owners]
         threshold = 1
         safe = self.deploy_test_safe(
             owners=owner_addresses,
             threshold=threshold,
-            initial_funding_wei=self.w3.toWei(0.1, "ether"),
+            initial_funding_wei=self.w3.to_wei(0.1, "ether"),
         )
         to = Account().create().address
-        value = self.w3.toWei(0.01, "ether")
+        value = self.w3.to_wei(0.01, "ether")
         safe_tx_gas = 200000
         data_gas = 100000
 
         safe_tx = SafeTx(
             self.ethereum_client,
             safe.address,
             to,
@@ -138,18 +138,18 @@
         owners = [Account.create() for _ in range(3)]
         owners_unsorted = sorted(owners, key=lambda x: int(x.address, 16), reverse=True)
         owner_addresses = [owner.address for owner in owners_unsorted]
         threshold = 1
         safe = self.deploy_test_safe(
             owners=owner_addresses,
             threshold=threshold,
-            initial_funding_wei=self.w3.toWei(0.1, "ether"),
+            initial_funding_wei=self.w3.to_wei(0.1, "ether"),
         )
         to = Account().create().address
-        value = self.w3.toWei(0.01, "ether")
+        value = self.w3.to_wei(0.01, "ether")
 
         safe_tx = SafeTx(
             self.ethereum_client,
             safe.address,
             to,
             value,
             b"",
```

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_serializers.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/test_signatures.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/gnosis/safe/tests/utils.py` & `safe-eth-py_suraneti-5.3.0/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/PKG-INFO` & `safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: safe-eth-py-suraneti
-Version: 0.0.2
+Version: 5.3.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
-Home-page: 
+Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
 Project-URL: Tracker, https://github.com/safe-global/safe-eth-py/issues
 Keywords: ethereum,web3,django,safe,cowswap,gnosis
```

### Comparing `safe-eth-py_suraneti-0.0.2/safe_eth_py_suraneti.egg-info/SOURCES.txt` & `safe-eth-py_suraneti-5.3.0/safe_eth_py_suraneti.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 gnosis/eth/constants.py
 gnosis/eth/ethereum_client.py
 gnosis/eth/ethereum_network.py
 gnosis/eth/exceptions.py
 gnosis/eth/multicall.py
 gnosis/eth/typing.py
 gnosis/eth/utils.py
+gnosis/eth/abis/__init__.py
+gnosis/eth/abis/multicall.py
 gnosis/eth/clients/__init__.py
 gnosis/eth/clients/blockscout_client.py
 gnosis/eth/clients/contract_metadata.py
 gnosis/eth/clients/etherscan_client.py
 gnosis/eth/clients/sourcify.py
 gnosis/eth/contracts/CPKFactory.json
 gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
@@ -83,15 +85,14 @@
 gnosis/eth/oracles/uniswap_v3.py
 gnosis/eth/oracles/utils.py
 gnosis/eth/oracles/abis/__init__.py
 gnosis/eth/oracles/abis/aave_abis.py
 gnosis/eth/oracles/abis/balancer_abis.py
 gnosis/eth/oracles/abis/cream_abis.py
 gnosis/eth/oracles/abis/curve_abis.py
-gnosis/eth/oracles/abis/makerdao.py
 gnosis/eth/oracles/abis/mooniswap_abis.py
 gnosis/eth/oracles/abis/superfluid_abis.py
 gnosis/eth/oracles/abis/uniswap_v3.py
 gnosis/eth/oracles/abis/yearn_abis.py
 gnosis/eth/oracles/abis/zerion_abis.py
 gnosis/eth/oracles/helpers/__init__.py
 gnosis/eth/oracles/helpers/curve_gauge_list.py
@@ -123,14 +124,15 @@
 gnosis/eth/tests/oracles/test_uniswap_v3.py
 gnosis/protocol/__init__.py
 gnosis/protocol/gnosis_protocol_api.py
 gnosis/protocol/order.py
 gnosis/protocol/tests/__init__.py
 gnosis/protocol/tests/test_gnosis_protocol_api.py
 gnosis/safe/__init__.py
+gnosis/safe/addresses.py
 gnosis/safe/exceptions.py
 gnosis/safe/multi_send.py
 gnosis/safe/proxy_factory.py
 gnosis/safe/safe.py
 gnosis/safe/safe_create2_tx.py
 gnosis/safe/safe_creation_tx.py
 gnosis/safe/safe_signature.py
```

### Comparing `safe-eth-py_suraneti-0.0.2/setup.cfg` & `safe-eth-py_suraneti-5.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = safe-eth-py_suraneti
-version = 0.0.2
+version = 5.3.0
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
 	safe
 	cowswap
 	gnosis
-url = 
+url = https://github.com/safe-global/safe-eth-py
 author = Uxío
 author_email = uxio@safe.global
 license = MIT License
 license_files = 
 	LICENSE
 classifiers = 
 	Environment :: Web Environment
@@ -39,18 +39,20 @@
 
 [options]
 packages = find:
 platforms = any
 include_package_data = True
 install_requires = 
 	packaging
-	py-evm==0.5.0a3
+	py-evm>=0.7.0a1
 	pysha3>=1.0.0
+	pysha3>=1.0.0,<2.0.0; python_version<"3.9"
+	safe-pysha3>=1.0.0; python_version>="3.9"
 	requests>=2
-	web3>=5.23.0
+	web3>=6.2.0
 python_requires = >=3.8
 
 [options.package_data]
 gnosis = 
 	py.typed
 	*.json
```

