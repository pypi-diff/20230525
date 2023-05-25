# Comparing `tmp/gnosis-neon-safe-eth-py-5.3.1.tar.gz` & `tmp/gnosis-neon-safe-eth-py-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnosis-neon-safe-eth-py-5.3.1.tar", last modified: Tue May 16 10:43:39 2023, max compression
+gzip compressed data, was "gnosis-neon-safe-eth-py-5.4.3.tar", last modified: Thu May 25 14:26:27 2023, max compression
```

## Comparing `gnosis-neon-safe-eth-py-5.3.1.tar` & `gnosis-neon-safe-eth-py-5.4.3.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:38.989516 gnosis-neon-safe-eth-py-5.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:38.993516 gnosis-neon-safe-eth-py-5.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:38.993516 gnosis-neon-safe-eth-py-5.3.1/gnosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:38.993516 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:38.993516 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/abis/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:38.993516 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.001516 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.005517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.005517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.005517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77427 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.005517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.009517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.009517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.009517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.009517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.009517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.013517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.013517 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.013517 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.013517 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.013517 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    41997 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:43:39.017517 gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-16 10:43:38.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 10:43:38.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:43:38.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 10:43:38.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 10:43:38.000000 gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-16 10:43:39.021517 gnosis-neon-safe-eth-py-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 10:43:21.000000 gnosis-neon-safe-eth-py-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.819790 gnosis-neon-safe-eth-py-5.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.819790 gnosis-neon-safe-eth-py-5.4.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.819790 gnosis-neon-safe-eth-py-5.4.3/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.823790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.823790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/abis/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.823790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.831790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.831790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.831790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.831790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77427 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.835790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.835790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.835790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.835790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.835790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.835790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.839790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.839790 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.839790 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.839790 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.839790 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42768 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34197 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-25 14:26:27.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-25 14:26:27.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:26:27.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 14:26:27.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 14:26:27.000000 gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-25 14:26:27.843790 gnosis-neon-safe-eth-py-5.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 14:26:13.000000 gnosis-neon-safe-eth-py-5.4.3/setup.py
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/LICENSE` & `gnosis-neon-safe-eth-py-5.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/PKG-INFO` & `gnosis-neon-safe-eth-py-5.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnosis-neon-safe-eth-py
-Version: 5.3.1
+Version: 5.4.3
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/README.rst` & `gnosis-neon-safe-eth-py-5.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/Makefile` & `gnosis-neon-safe-eth-py-5.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/make.bat` & `gnosis-neon-safe-eth-py-5.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/conf.py` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.clients.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.django.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.oracles.abis.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.eth.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/gnosis.safe.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/index.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/docs/source/quickstart.rst` & `gnosis-neon-safe-eth-py-5.4.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/__init__.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/abis/multicall.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/__init__.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/blockscout_client.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/etherscan_client.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/etherscan_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         EthereumNetwork.MOONRIVER: "https://moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://goerli.basescan.org",
         EthereumNetwork.NEON_EVM_DEVNET: "https://neonscan.org",
+        EthereumNetwork.SEPOLIA: "https://sepolia.etherscan.io",
     }
 
     NETWORK_WITH_API_URL = {
         EthereumNetwork.MAINNET: "https://api.etherscan.io",
         EthereumNetwork.RINKEBY: "https://api-rinkeby.etherscan.io",
         EthereumNetwork.ROPSTEN: "https://api-ropsten.etherscan.io",
         EthereumNetwork.GOERLI: "https://api-goerli.etherscan.io",
@@ -64,14 +65,15 @@
         EthereumNetwork.MOONRIVER: "https://api-moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://api-moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://api.cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://api-testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://api.celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://api-goerli.basescan.org",
         EthereumNetwork.NEON_EVM_DEVNET: "https://devnet-api.neonscan.org",
+        EthereumNetwork.SEPOLIA: "https://api-sepolia.etherscan.io",
     }
     HTTP_HEADERS = {
         "User-Agent": "curl/7.77.0",
     }
 
     def __init__(self, network: EthereumNetwork, api_key: Optional[str] = None):
         self.network = network
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/clients/sourcify.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/constants.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/CPKFactory.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/DelegateConstructorProxy.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC1155.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC20TestToken.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ERC721.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/MultiSend.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/PayingProxy.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_0_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_1_1.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/Proxy_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/__init__.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/kyber_network_proxy.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_exchange.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_factory.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_factory.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_pair.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/contracts/uniswap_v2_router.json` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/admin.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/forms.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/models.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/serializers.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/models.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_forms.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_models.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/django/tests/test_serializers.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/eip712/__init__.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/ethereum_client.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/ethereum_network.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/exceptions.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/multicall.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/__init__.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/aave_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/balancer_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/cream_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/curve_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/mooniswap_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/uniswap_v3.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/yearn_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/abis/zerion_abis.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/cowswap.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/kyber.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/oracles.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/superfluid.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/sushiswap.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/uniswap_v3.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/oracles/utils.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/mocks.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_blockscout_client.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_etherscan_client.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/clients/test_sourcify.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/eip712/test_eip712.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/ethereum_test_case.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_internal_txs.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_log_receipts.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_block.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_filter.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_cowswap.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_kyber.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_superfluid.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_sushiswap.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_ethereum_client.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_multicall.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_oracles.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/test_utils.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/tests/utils.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/eth/utils.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/gnosis_protocol_api.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/order.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/__init__.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/addresses.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,16 +184,19 @@
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 8944351, "1.3.0"),
     ],
     EthereumNetwork.AVALANCHE_C_CHAIN: [
         (
             "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             22_123_383,
             "1.3.0+L2",
-        )(  # default singleton address
-            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 4_949_507, "1.3.0+L2"
+        ),  # default singleton address
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            4_949_507,
+            "1.3.0+L2",
         ),  # safe singleton address
         (
             "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             14_747_111,
             "1.3.0",
         ),  # default singleton address
         (
@@ -447,14 +450,36 @@
         ),  # need to change block number
         (
             "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
             205147000,
             "1.3.0",
         ),  # need to change block number
     ],
+    EthereumNetwork.SEPOLIA: [
+        (
+            "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            2086878,
+            "1.3.0+L2",
+        ),  # Default singleton address
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            2087039,
+            "1.3.0+L2",
+        ),  # Safe singleton address
+        (
+            "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            2086880,
+            "1.3.0",
+        ),  # Default singleton address
+        (
+            "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
+            2087040,
+            "1.3.0",
+        ),  # Safe singleton address
+    ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
         (
             "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
             14981216,
@@ -558,18 +583,20 @@
         ),  # v1.3.0 default singleton address
     ],
     EthereumNetwork.CELO_MAINNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 8944342),  # v1.3.0
     ],
     EthereumNetwork.AVALANCHE_C_CHAIN: [
         (
-            " 0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             14_747_108,
-        )(  # v1.3.0 default singleton address
-            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 4_949_487
+        ),  # v1.3.0 default singleton address
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            4_949_487,
         ),  # v1.3.0 safe singleton address
     ],
     EthereumNetwork.MOONBEAM: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 172078),  # v1.3.0
     ],
     EthereumNetwork.MOONRIVER: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 707_721),  # v1.3.0
@@ -740,14 +767,27 @@
     ],
     EthereumNetwork.ETHEREUM_CLASSIC_MAINNET: [
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 15904946),  # v1.3.0
     ],
     EthereumNetwork.ETHEREUM_CLASSIC_TESTNET_MORDOR: [
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 6333172),  # v1.3.0
     ],
+    EthereumNetwork.ETHEREUM_CLASSIC_TESTNET_MORDOR: [
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 6333172),  # v1.3.0
+    ],
     EthereumNetwork.NEON_EVM_DEVNET: [
         (
-            "0xc22834581ebc8527d974f8a1c97e1bea4ef910bc",
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
             205146874,
         ),  # v1.3.0. need to change block number
     ],
+    EthereumNetwork.SEPOLIA: [
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            2087031,
+        ),  # v1.3.0  Safe singleton address
+        (
+            "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            2086864,
+        ),  # v1.3.0  Default singleton address
+    ],
 }
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/base_api.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/relay_service_api.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/api/transaction_service_api.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/exceptions.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/multi_send.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/proxy_factory.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe.py`

 * *Files 2% similar despite different names*

```diff
@@ -900,20 +900,23 @@
                     contract.functions.VERSION(),
                 ],
                 from_address=self.address,
                 block_identifier=block_identifier,
                 raise_exception=False,
             )
             modules_response, nonce, owners, threshold, version = results
-            if modules_response:
-                modules, next_module = modules_response
-            if (
-                not modules_response or next_module != SENTINEL_ADDRESS
-            ):  # < 1.1.1 or still more elements in the list
+            if not modules_response:
+                # < 1.1.1
                 modules = self.retrieve_modules()
+            else:
+                modules, next_module = modules_response
+                if modules and next_module != SENTINEL_ADDRESS:
+                    # Still more elements in the list
+                    modules = self.retrieve_modules()
+
             return SafeInfo(
                 self.address,
                 fallback_handler,
                 guard,
                 master_copy,
                 modules,
                 nonce,
@@ -966,18 +969,20 @@
         )[-20:].rjust(20, b"\0")
         return fast_bytes_to_checksum_address(address)
 
     def retrieve_modules(
         self,
         pagination: Optional[int] = 50,
         block_identifier: Optional[BlockIdentifier] = "latest",
-    ) -> List[str]:
+        max_modules_to_retrieve: Optional[int] = 500,
+    ) -> List[ChecksumAddress]:
         """
         :param pagination: Number of modules to get per request
         :param block_identifier:
+        :param max_modules_to_retrieve: Maximum number of modules to retrieve
         :return: List of module addresses
         """
         try:
             # Contracts with Safe version < 1.1.0 were not paginated
             contract = get_safe_V1_0_0_contract(
                 self.ethereum_client.w3, address=self.address
             )
@@ -985,25 +990,32 @@
                 block_identifier=block_identifier
             )
         except Web3Exception:
             pass
 
         contract = self.contract
         address = SENTINEL_ADDRESS
-        all_modules: List[str] = []
-        while True:
+        all_modules: List[ChecksumAddress] = []
+
+        for _ in range(max_modules_to_retrieve // pagination):
+            # If we use a `while True` loop a custom coded Safe could get us into an infinite loop
             (modules, address) = contract.functions.getModulesPaginated(
                 address, pagination
             ).call(block_identifier=block_identifier)
 
-            all_modules.extend(modules)
-            if address == SENTINEL_ADDRESS:
+            if not modules or address in (NULL_ADDRESS, SENTINEL_ADDRESS):
+                # `NULL_ADDRESS` is only seen in uninitialized Safes
                 break
-            else:
-                all_modules.append(address)
+
+            # Safes with version < 1.4.0 don't include the `starter address` used as pagination in the module list
+            # From 1.4.0 onwards it is included, so we check for duplicated addresses before inserting
+            modules_to_insert = [
+                module for module in modules + [address] if module not in all_modules
+            ]
+            all_modules.extend(modules_to_insert)
         return all_modules
 
     def retrieve_is_hash_approved(
         self,
         owner: str,
         safe_hash: bytes,
         block_identifier: Optional[BlockIdentifier] = "latest",
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_create2_tx.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_creation_tx.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_signature.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/safe_tx.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/serializers.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/signatures.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/api/test_transaction_service_api.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/safe_test_case.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_multi_send.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_proxy_factory.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe.py`

 * *Files 2% similar despite different names*

```diff
@@ -664,14 +664,49 @@
                 tx_gas_price=self.gas_price,
             )
 
         self.assertCountEqual(
             safe.retrieve_modules(pagination=1), [module_address] + more_modules
         )
 
+    def test_retrieve_modules_below_v1_1_1(self):
+        safe_v1_0_0 = self.deploy_test_safe_v1_0_0(
+            owners=[self.ethereum_test_account.address]
+        )
+        safe_contract = safe_v1_0_0.contract
+        module_address = Account.create().address
+        self.assertEqual(safe_v1_0_0.retrieve_modules(), [])
+
+        tx = safe_contract.functions.enableModule(module_address).build_transaction(
+            {"from": self.ethereum_test_account.address, "gas": 0, "gasPrice": 0}
+        )
+        safe_tx = safe_v1_0_0.build_multisig_tx(safe_v1_0_0.address, 0, tx["data"])
+        safe_tx.sign(self.ethereum_test_account.key)
+        safe_tx.execute(
+            tx_sender_private_key=self.ethereum_test_account.key,
+            tx_gas_price=self.gas_price,
+        )
+        self.assertEqual(safe_v1_0_0.retrieve_modules(), [module_address])
+        self.assertEqual(safe_v1_0_0.retrieve_all_info().modules, [module_address])
+
+    def test_retrieve_modules_unitialized_safe(self):
+        """
+        Unitialized Safes will return `[[], '0x0000000000000000000000000000000000000000']` when calling
+        `getModulesPaginated`, as `SENTINEL_ADDRESS` is only set when initialized
+        """
+
+        ethereum_tx_sent = self.proxy_factory.deploy_proxy_contract(
+            self.ethereum_test_account,
+            self.safe_contract.address,
+            initializer=b"",
+        )
+        safe = Safe(ethereum_tx_sent.contract_address, self.ethereum_client)
+        self.assertEqual(safe.retrieve_modules(), [])
+        self.assertEqual(safe.retrieve_all_info().modules, [])
+
     def test_retrieve_is_hash_approved(self):
         safe = self.deploy_test_safe(owners=[self.ethereum_test_account.address])
         safe_contract = safe.contract
         fake_tx_hash = Web3.keccak(text="Knopfler")
         another_tx_hash = Web3.keccak(text="Marc")
         tx = safe_contract.functions.approveHash(fake_tx_hash).build_transaction(
             {"from": self.ethereum_test_account.address}
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_create2_tx.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_creation_tx.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_signature.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_safe_tx.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_serializers.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/test_signatures.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis/safe/tests/utils.py` & `gnosis-neon-safe-eth-py-5.4.3/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/PKG-INFO` & `gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnosis-neon-safe-eth-py
-Version: 5.3.1
+Version: 5.4.3
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt` & `gnosis-neon-safe-eth-py-5.4.3/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 gnosis/safe/signatures.py
 gnosis/safe/api/__init__.py
 gnosis/safe/api/base_api.py
 gnosis/safe/api/relay_service_api.py
 gnosis/safe/api/transaction_service_api.py
 gnosis/safe/tests/__init__.py
 gnosis/safe/tests/safe_test_case.py
+gnosis/safe/tests/test_addresses.py
 gnosis/safe/tests/test_multi_send.py
 gnosis/safe/tests/test_proxy_factory.py
 gnosis/safe/tests/test_safe.py
 gnosis/safe/tests/test_safe_create2_tx.py
 gnosis/safe/tests/test_safe_creation_tx.py
 gnosis/safe/tests/test_safe_signature.py
 gnosis/safe/tests/test_safe_tx.py
```

### Comparing `gnosis-neon-safe-eth-py-5.3.1/setup.cfg` & `gnosis-neon-safe-eth-py-5.4.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gnosis-neon-safe-eth-py
-version = 5.3.1
+version = 5.4.3
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

