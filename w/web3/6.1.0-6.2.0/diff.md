# Comparing `tmp/web3-6.1.0.tar.gz` & `tmp/web3-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3-6.1.0.tar", last modified: Wed Apr  5 17:29:07 2023, max compression
+gzip compressed data, was "web3-6.2.0.tar", last modified: Wed Apr 12 19:40:44 2023, max compression
```

## Comparing `web3-6.1.0.tar` & `web3-6.2.0.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.652324 web3-6.1.0/
--rw-r--r--   0 eve        (501) staff       (20)     1080 2023-04-03 22:45:42.000000 web3-6.1.0/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      260 2023-04-03 22:45:42.000000 web3-6.1.0/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     2184 2023-04-05 17:29:07.652067 web3-6.1.0/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1294 2023-04-03 22:45:42.000000 web3-6.1.0/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.605579 web3-6.1.0/ens/
--rw-r--r--   0 eve        (501) staff       (20)      285 2023-04-03 22:45:42.000000 web3-6.1.0/ens/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    23773 2023-04-03 22:45:42.000000 web3-6.1.0/ens/abis.py
--rw-r--r--   0 eve        (501) staff       (20)    20886 2023-04-03 22:45:42.000000 web3-6.1.0/ens/async_ens.py
--rw-r--r--   0 eve        (501) staff       (20)       41 2023-04-03 22:45:42.000000 web3-6.1.0/ens/auto.py
--rw-r--r--   0 eve        (501) staff       (20)     3287 2023-04-03 22:45:42.000000 web3-6.1.0/ens/base_ens.py
--rw-r--r--   0 eve        (501) staff       (20)      601 2023-04-03 22:45:42.000000 web3-6.1.0/ens/constants.py
--rw-r--r--   0 eve        (501) staff       (20)   199089 2023-04-03 22:45:42.000000 web3-6.1.0/ens/contract_data.py
--rw-r--r--   0 eve        (501) staff       (20)    20044 2023-04-03 22:45:42.000000 web3-6.1.0/ens/ens.py
--rw-r--r--   0 eve        (501) staff       (20)     2390 2023-04-03 22:45:42.000000 web3-6.1.0/ens/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)     8978 2023-04-03 22:45:42.000000 web3-6.1.0/ens/utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.606883 web3-6.1.0/ethpm/
--rw-r--r--   0 eve        (501) staff       (20)      580 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.607879 web3-6.1.0/ethpm/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2511 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/backend.py
--rw-r--r--   0 eve        (501) staff       (20)     1477 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/cache.py
--rw-r--r--   0 eve        (501) staff       (20)     2848 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/chains.py
--rw-r--r--   0 eve        (501) staff       (20)     1030 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/contract.py
--rw-r--r--   0 eve        (501) staff       (20)     5263 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/deployments.py
--rw-r--r--   0 eve        (501) staff       (20)     2717 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/ipfs.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.608120 web3-6.1.0/ethpm/_utils/protobuf/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/protobuf/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1938 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-r--r--   0 eve        (501) staff       (20)     1488 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/_utils/registry.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.608356 web3-6.1.0/ethpm/assets/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.608590 web3-6.1.0/ethpm/assets/ens/
--rw-r--r--   0 eve        (501) staff       (20)    74682 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/ens/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.609030 web3-6.1.0/ethpm/assets/escrow/
--rw-r--r--   0 eve        (501) staff       (20)     8007 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/escrow/with_bytecode_v3.json
--rw-r--r--   0 eve        (501) staff       (20)      760 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/ipfs_file.proto
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.609351 web3-6.1.0/ethpm/assets/owned/
--rw-r--r--   0 eve        (501) staff       (20)     2655 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/owned/output_v3.json
--rw-r--r--   0 eve        (501) staff       (20)      746 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/owned/with_contract_type_v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.611372 web3-6.1.0/ethpm/assets/registry/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.613390 web3-6.1.0/ethpm/assets/registry/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     3129 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/Authority.sol
--rw-r--r--   0 eve        (501) staff       (20)     2876 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
--rw-r--r--   0 eve        (501) staff       (20)     6380 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/PackageDB.sol
--rw-r--r--   0 eve        (501) staff       (20)    10553 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/PackageRegistry.sol
--rw-r--r--   0 eve        (501) staff       (20)     2966 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 eve        (501) staff       (20)     9041 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/ReleaseDB.sol
--rw-r--r--   0 eve        (501) staff       (20)     4980 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
--rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/solc_input.json
--rw-r--r--   0 eve        (501) staff       (20)   727775 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/solc_output.json
--rw-r--r--   0 eve        (501) staff       (20)   270218 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/registry/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.613516 web3-6.1.0/ethpm/assets/safe-math-lib/
--rw-r--r--   0 eve        (501) staff       (20)     2845 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.614672 web3-6.1.0/ethpm/assets/simple-registry/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.615488 web3-6.1.0/ethpm/assets/simple-registry/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1841 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/simple-registry/contracts/Ownable.sol
--rw-r--r--   0 eve        (501) staff       (20)    12350 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
--rw-r--r--   0 eve        (501) staff       (20)     3278 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 eve        (501) staff       (20)      950 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/simple-registry/solc_input.json
--rw-r--r--   0 eve        (501) staff       (20)   199338 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/simple-registry/solc_output.json
--rw-r--r--   0 eve        (501) staff       (20)    75677 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/simple-registry/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.616184 web3-6.1.0/ethpm/assets/standard-token/
--rw-r--r--   0 eve        (501) staff       (20)    22292 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/standard-token/output_v3.json
--rw-r--r--   0 eve        (501) staff       (20)     8765 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/standard-token/with_bytecode_v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.617000 web3-6.1.0/ethpm/assets/vyper_registry/
--rw-r--r--   0 eve        (501) staff       (20)    81363 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/vyper_registry/0.1.0.json
--rw-r--r--   0 eve        (501) staff       (20)     6339 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/vyper_registry/registry.vy
--rw-r--r--   0 eve        (501) staff       (20)     7596 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/assets/vyper_registry/registry_with_delete.vy
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.617708 web3-6.1.0/ethpm/backends/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      956 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)     3006 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/backends/http.py
--rw-r--r--   0 eve        (501) staff       (20)     6551 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/backends/ipfs.py
--rw-r--r--   0 eve        (501) staff       (20)     4174 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/backends/registry.py
--rw-r--r--   0 eve        (501) staff       (20)      405 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     6256 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1890 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/dependencies.py
--rw-r--r--   0 eve        (501) staff       (20)     2134 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/deployments.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.599797 web3-6.1.0/ethpm/ethpm-spec/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.599544 web3-6.1.0/ethpm/ethpm-spec/examples/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.618670 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/
--rw-r--r--   0 eve        (501) staff       (20)     6810 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5361 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.618950 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      888 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
--rw-r--r--   0 eve        (501) staff       (20)      644 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
--rw-r--r--   0 eve        (501) staff       (20)    11598 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     8669 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/escrow/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.619461 web3-6.1.0/ethpm/ethpm-spec/examples/owned/
--rw-r--r--   0 eve        (501) staff       (20)      544 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      443 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.619587 web3-6.1.0/ethpm/ethpm-spec/examples/owned/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      222 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
--rw-r--r--   0 eve        (501) staff       (20)      728 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/owned/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.620115 web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/
--rw-r--r--   0 eve        (501) staff       (20)     5272 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5030 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
--rw-r--r--   0 eve        (501) staff       (20)     5220 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     4993 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.620792 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/
--rw-r--r--   0 eve        (501) staff       (20)     3976 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3143 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.621033 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      802 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
--rw-r--r--   0 eve        (501) staff       (20)     5517 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3289 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.621638 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/
--rw-r--r--   0 eve        (501) staff       (20)     3794 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3238 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.621899 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1155 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
--rw-r--r--   0 eve        (501) staff       (20)     2949 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
--rw-r--r--   0 eve        (501) staff       (20)    17129 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     6100 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.622487 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/
--rw-r--r--   0 eve        (501) staff       (20)      590 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      507 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.622700 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      396 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
--rw-r--r--   0 eve        (501) staff       (20)      786 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/transferable/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.623407 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/
--rw-r--r--   0 eve        (501) staff       (20)     6669 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5456 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.624277 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1454 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
--rw-r--r--   0 eve        (501) staff       (20)     9710 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     7326 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.624031 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/
--rw-r--r--   0 eve        (501) staff       (20)     8052 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     6657 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.624156 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      621 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
--rw-r--r--   0 eve        (501) staff       (20)    12191 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     9503 2022-04-27 21:13:00.000000 web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.624701 web3-6.1.0/ethpm/ethpm-spec/spec/
--rw-r--r--   0 eve        (501) staff       (20)    10302 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/spec/package.spec.json
--rw-r--r--   0 eve        (501) staff       (20)    12879 2021-02-11 20:53:14.000000 web3-6.1.0/ethpm/ethpm-spec/spec/v3.spec.json
--rw-r--r--   0 eve        (501) staff       (20)     1194 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    14493 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/package.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.625346 web3-6.1.0/ethpm/tools/
--rw-r--r--   0 eve        (501) staff       (20)      103 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/tools/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    27045 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/tools/builder.py
--rw-r--r--   0 eve        (501) staff       (20)    10373 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/tools/checker.py
--rw-r--r--   0 eve        (501) staff       (20)      475 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/tools/get_manifest.py
--rw-r--r--   0 eve        (501) staff       (20)     4368 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/uri.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.626102 web3-6.1.0/ethpm/validation/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/validation/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4716 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/validation/manifest.py
--rw-r--r--   0 eve        (501) staff       (20)     1072 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/validation/misc.py
--rw-r--r--   0 eve        (501) staff       (20)     2317 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/validation/package.py
--rw-r--r--   0 eve        (501) staff       (20)     4873 2023-04-03 22:45:42.000000 web3-6.1.0/ethpm/validation/uri.py
--rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-03 22:45:42.000000 web3-6.1.0/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-04-05 17:29:07.652381 web3-6.1.0/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     3168 2023-04-05 17:24:31.000000 web3-6.1.0/setup.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.629384 web3-6.1.0/web3/
--rw-r--r--   0 eve        (501) staff       (20)      752 2023-04-03 22:45:42.000000 web3-6.1.0/web3/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.636154 web3-6.1.0/web3/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    28771 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      456 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/async_caching.py
--rw-r--r--   0 eve        (501) staff       (20)     6865 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/async_transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     2059 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      992 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/caching.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.636585 web3-6.1.0/web3/_utils/compat/
--rw-r--r--   0 eve        (501) staff       (20)      319 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/compat/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/compat/compat_py2.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/compat/compat_py3.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.636762 web3-6.1.0/web3/_utils/contract_sources/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     6406 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/compile_contracts.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.640384 web3-6.1.0/web3/_utils/contract_sources/contract_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      517 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-r--r--   0 eve        (501) staff       (20)     5344 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/address_reflector.py
--rw-r--r--   0 eve        (501) staff       (20)    19324 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    15157 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     6219 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     6492 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-r--r--   0 eve        (501) staff       (20)    38375 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     5673 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/event_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)    16216 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)     1685 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     7829 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/math_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    17122 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-r--r--   0 eve        (501) staff       (20)    33495 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)     1863 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/payable_tester.py
--rw-r--r--   0 eve        (501) staff       (20)    17734 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     5410 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     2719 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/revert_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     3653 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)    11900 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/string_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    23756 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)    14980 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     1640 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     1738 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/decorators.py
--rw-r--r--   0 eve        (501) staff       (20)      144 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/empty.py
--rw-r--r--   0 eve        (501) staff       (20)     9065 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)     2120 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/ens.py
--rw-r--r--   0 eve        (501) staff       (20)    17073 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/events.py
--rw-r--r--   0 eve        (501) staff       (20)     2113 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/fee_utils.py
--rw-r--r--   0 eve        (501) staff       (20)    11886 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/filters.py
--rw-r--r--   0 eve        (501) staff       (20)     3071 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/formatters.py
--rw-r--r--   0 eve        (501) staff       (20)       55 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/function_identifiers.py
--rw-r--r--   0 eve        (501) staff       (20)      195 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/http.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/hypothesis.py
--rw-r--r--   0 eve        (501) staff       (20)     1047 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/math.py
--rw-r--r--   0 eve        (501) staff       (20)    32178 2023-04-05 15:12:26.000000 web3-6.1.0/web3/_utils/method_formatters.py
--rw-r--r--   0 eve        (501) staff       (20)     1146 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/miner.py
--rw-r--r--   0 eve        (501) staff       (20)     3147 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.641891 web3-6.1.0/web3/_utils/module_testing/
--rw-r--r--   0 eve        (501) staff       (20)      539 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)   141877 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/eth_module.py
--rw-r--r--   0 eve        (501) staff       (20)     3406 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/go_ethereum_admin_module.py
--rw-r--r--   0 eve        (501) staff       (20)    10338 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/go_ethereum_personal_module.py
--rw-r--r--   0 eve        (501) staff       (20)     1176 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
--rw-r--r--   0 eve        (501) staff       (20)     4825 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/module_testing_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1272 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/net_module.py
--rw-r--r--   0 eve        (501) staff       (20)     9335 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/module_testing/web3_module.py
--rw-r--r--   0 eve        (501) staff       (20)     6493 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/normalizers.py
--rw-r--r--   0 eve        (501) staff       (20)     8833 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/request.py
--rw-r--r--   0 eve        (501) staff       (20)     9449 2023-04-05 15:12:26.000000 web3-6.1.0/web3/_utils/rpc_abi.py
--rw-r--r--   0 eve        (501) staff       (20)     4207 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/threads.py
--rw-r--r--   0 eve        (501) staff       (20)     8670 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      816 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/type_conversion.py
--rw-r--r--   0 eve        (501) staff       (20)     1669 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/utility_methods.py
--rw-r--r--   0 eve        (501) staff       (20)     6291 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/validation.py
--rw-r--r--   0 eve        (501) staff       (20)      994 2023-04-03 22:45:42.000000 web3-6.1.0/web3/_utils/windows.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.642139 web3-6.1.0/web3/auto/
--rw-r--r--   0 eve        (501) staff       (20)       44 2023-04-03 22:45:42.000000 web3-6.1.0/web3/auto/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      263 2023-04-03 22:45:42.000000 web3-6.1.0/web3/auto/gethdev.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.642633 web3-6.1.0/web3/beacon/
--rw-r--r--   0 eve        (501) staff       (20)       91 2023-04-03 22:45:42.000000 web3-6.1.0/web3/beacon/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1516 2023-04-03 22:45:42.000000 web3-6.1.0/web3/beacon/api_endpoints.py
--rw-r--r--   0 eve        (501) staff       (20)     5421 2023-04-03 22:45:42.000000 web3-6.1.0/web3/beacon/async_beacon.py
--rw-r--r--   0 eve        (501) staff       (20)     4772 2023-04-03 22:45:42.000000 web3-6.1.0/web3/beacon/main.py
--rw-r--r--   0 eve        (501) staff       (20)      396 2023-04-03 22:45:42.000000 web3-6.1.0/web3/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.643712 web3-6.1.0/web3/contract/
--rw-r--r--   0 eve        (501) staff       (20)      215 2023-04-03 22:45:42.000000 web3-6.1.0/web3/contract/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    19756 2023-04-03 22:45:42.000000 web3-6.1.0/web3/contract/async_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    35710 2023-04-03 22:45:42.000000 web3-6.1.0/web3/contract/base_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    18804 2023-04-03 22:45:42.000000 web3-6.1.0/web3/contract/contract.py
--rw-r--r--   0 eve        (501) staff       (20)    12338 2023-04-03 22:45:42.000000 web3-6.1.0/web3/contract/utils.py
--rw-r--r--   0 eve        (501) staff       (20)     8271 2023-04-03 22:45:42.000000 web3-6.1.0/web3/datastructures.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.644232 web3-6.1.0/web3/eth/
--rw-r--r--   0 eve        (501) staff       (20)      166 2023-04-03 22:45:42.000000 web3-6.1.0/web3/eth/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    17870 2023-04-03 22:45:42.000000 web3-6.1.0/web3/eth/async_eth.py
--rw-r--r--   0 eve        (501) staff       (20)     5943 2023-04-03 22:45:42.000000 web3-6.1.0/web3/eth/base_eth.py
--rw-r--r--   0 eve        (501) staff       (20)    19295 2023-04-03 22:45:42.000000 web3-6.1.0/web3/eth/eth.py
--rw-r--r--   0 eve        (501) staff       (20)     5780 2023-04-03 22:45:42.000000 web3-6.1.0/web3/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.644589 web3-6.1.0/web3/gas_strategies/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/gas_strategies/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      430 2023-04-03 22:45:42.000000 web3-6.1.0/web3/gas_strategies/rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     9010 2023-04-03 22:45:42.000000 web3-6.1.0/web3/gas_strategies/time_based.py
--rw-r--r--   0 eve        (501) staff       (20)    11826 2023-04-03 22:45:42.000000 web3-6.1.0/web3/geth.py
--rw-r--r--   0 eve        (501) staff       (20)      198 2023-04-03 22:45:42.000000 web3-6.1.0/web3/logs.py
--rw-r--r--   0 eve        (501) staff       (20)    12686 2023-04-05 15:12:26.000000 web3-6.1.0/web3/main.py
--rw-r--r--   0 eve        (501) staff       (20)     7875 2023-04-03 22:45:42.000000 web3-6.1.0/web3/manager.py
--rw-r--r--   0 eve        (501) staff       (20)     8430 2023-04-03 22:45:42.000000 web3-6.1.0/web3/method.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.647253 web3-6.1.0/web3/middleware/
--rw-r--r--   0 eve        (501) staff       (20)     3724 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      239 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/abi.py
--rw-r--r--   0 eve        (501) staff       (20)     2755 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/async_cache.py
--rw-r--r--   0 eve        (501) staff       (20)     1779 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/attrdict.py
--rw-r--r--   0 eve        (501) staff       (20)     1785 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/buffered_gas_estimate.py
--rw-r--r--   0 eve        (501) staff       (20)    12617 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/cache.py
--rw-r--r--   0 eve        (501) staff       (20)     1167 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/exception_handling.py
--rw-r--r--   0 eve        (501) staff       (20)     3119 2023-04-05 15:12:26.000000 web3-6.1.0/web3/middleware/exception_retry_request.py
--rw-r--r--   0 eve        (501) staff       (20)    21131 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/filter.py
--rw-r--r--   0 eve        (501) staff       (20)     4596 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/fixture.py
--rw-r--r--   0 eve        (501) staff       (20)     4762 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/formatting.py
--rw-r--r--   0 eve        (501) staff       (20)     4212 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/gas_price_strategy.py
--rw-r--r--   0 eve        (501) staff       (20)     1657 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/geth_poa.py
--rw-r--r--   0 eve        (501) staff       (20)      590 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/names.py
--rw-r--r--   0 eve        (501) staff       (20)      246 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/normalize_request_parameters.py
--rw-r--r--   0 eve        (501) staff       (20)      351 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/pythonic.py
--rw-r--r--   0 eve        (501) staff       (20)     4450 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/signing.py
--rw-r--r--   0 eve        (501) staff       (20)     1014 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/simulate_unmined_transaction.py
--rw-r--r--   0 eve        (501) staff       (20)     3739 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/stalecheck.py
--rw-r--r--   0 eve        (501) staff       (20)     4573 2023-04-03 22:45:42.000000 web3-6.1.0/web3/middleware/validation.py
--rw-r--r--   0 eve        (501) staff       (20)     3615 2023-04-03 22:45:42.000000 web3-6.1.0/web3/module.py
--rw-r--r--   0 eve        (501) staff       (20)     1562 2023-04-03 22:45:42.000000 web3-6.1.0/web3/net.py
--rw-r--r--   0 eve        (501) staff       (20)    21609 2023-04-03 22:45:42.000000 web3-6.1.0/web3/pm.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.648232 web3-6.1.0/web3/providers/
--rw-r--r--   0 eve        (501) staff       (20)      368 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3544 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/async_base.py
--rw-r--r--   0 eve        (501) staff       (20)     2469 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/async_rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     3403 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/auto.py
--rw-r--r--   0 eve        (501) staff       (20)     3477 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.648700 web3-6.1.0/web3/providers/eth_tester/
--rw-r--r--   0 eve        (501) staff       (20)       97 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/eth_tester/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    14296 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/eth_tester/defaults.py
--rw-r--r--   0 eve        (501) staff       (20)     5452 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/eth_tester/main.py
--rw-r--r--   0 eve        (501) staff       (20)    12665 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/eth_tester/middleware.py
--rw-r--r--   0 eve        (501) staff       (20)     6534 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/ipc.py
--rw-r--r--   0 eve        (501) staff       (20)     2686 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     3919 2023-04-03 22:45:42.000000 web3-6.1.0/web3/providers/websocket.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.648824 web3-6.1.0/web3/scripts/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/scripts/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.648982 web3-6.1.0/web3/scripts/release/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/scripts/release/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1534 2023-04-03 22:45:42.000000 web3-6.1.0/web3/scripts/release/test_package.py
--rw-r--r--   0 eve        (501) staff       (20)      951 2023-04-03 22:45:42.000000 web3-6.1.0/web3/testing.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.649105 web3-6.1.0/web3/tools/
--rw-r--r--   0 eve        (501) staff       (20)       73 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.649697 web3-6.1.0/web3/tools/benchmark/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/benchmark/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5886 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/benchmark/main.py
--rw-r--r--   0 eve        (501) staff       (20)     3435 2023-04-05 15:12:26.000000 web3-6.1.0/web3/tools/benchmark/node.py
--rw-r--r--   0 eve        (501) staff       (20)      912 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/benchmark/reporting.py
--rw-r--r--   0 eve        (501) staff       (20)     1722 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/benchmark/utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.650709 web3-6.1.0/web3/tools/pytest_ethereum/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/pytest_ethereum/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4158 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/pytest_ethereum/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1423 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/pytest_ethereum/deployer.py
--rw-r--r--   0 eve        (501) staff       (20)      380 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/pytest_ethereum/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)     3927 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/pytest_ethereum/linker.py
--rw-r--r--   0 eve        (501) staff       (20)      645 2023-04-03 22:45:42.000000 web3-6.1.0/web3/tools/pytest_ethereum/plugins.py
--rw-r--r--   0 eve        (501) staff       (20)     2958 2023-04-05 15:12:26.000000 web3-6.1.0/web3/tracing.py
--rw-r--r--   0 eve        (501) staff       (20)    10612 2023-04-05 15:12:26.000000 web3-6.1.0/web3/types.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.651757 web3-6.1.0/web3/utils/
--rw-r--r--   0 eve        (501) staff       (20)      454 2023-04-03 22:45:42.000000 web3-6.1.0/web3/utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      498 2023-04-03 22:45:42.000000 web3-6.1.0/web3/utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      967 2023-04-03 22:45:42.000000 web3-6.1.0/web3/utils/address.py
--rw-r--r--   0 eve        (501) staff       (20)     3096 2023-04-03 22:45:42.000000 web3-6.1.0/web3/utils/async_exception_handling.py
--rw-r--r--   0 eve        (501) staff       (20)     1521 2023-04-03 22:45:42.000000 web3-6.1.0/web3/utils/caching.py
--rw-r--r--   0 eve        (501) staff       (20)     3052 2023-04-03 22:45:42.000000 web3-6.1.0/web3/utils/exception_handling.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-05 17:29:07.630231 web3-6.1.0/web3.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     2184 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     9743 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)       64 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/entry_points.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)     1165 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       15 2023-04-05 17:29:07.000000 web3-6.1.0/web3.egg-info/top_level.txt
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.284804 web3-6.2.0/
+-rw-r--r--   0 eve        (501) staff       (20)     1080 2023-04-06 21:34:13.000000 web3-6.2.0/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      260 2023-04-06 21:34:13.000000 web3-6.2.0/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     2184 2023-04-12 19:40:44.284632 web3-6.2.0/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     1294 2023-04-10 20:16:28.000000 web3-6.2.0/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.229828 web3-6.2.0/ens/
+-rw-r--r--   0 eve        (501) staff       (20)      285 2023-04-10 20:16:28.000000 web3-6.2.0/ens/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    23773 2023-04-06 21:34:13.000000 web3-6.2.0/ens/abis.py
+-rw-r--r--   0 eve        (501) staff       (20)    20886 2023-04-10 20:16:28.000000 web3-6.2.0/ens/async_ens.py
+-rw-r--r--   0 eve        (501) staff       (20)       41 2023-04-10 20:16:28.000000 web3-6.2.0/ens/auto.py
+-rw-r--r--   0 eve        (501) staff       (20)     3287 2023-04-10 20:16:28.000000 web3-6.2.0/ens/base_ens.py
+-rw-r--r--   0 eve        (501) staff       (20)      601 2023-04-06 21:34:13.000000 web3-6.2.0/ens/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)   199089 2023-04-06 21:34:13.000000 web3-6.2.0/ens/contract_data.py
+-rw-r--r--   0 eve        (501) staff       (20)    20044 2023-04-10 20:16:28.000000 web3-6.2.0/ens/ens.py
+-rw-r--r--   0 eve        (501) staff       (20)     2390 2023-04-06 21:34:13.000000 web3-6.2.0/ens/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)     8978 2023-04-10 20:16:28.000000 web3-6.2.0/ens/utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.231611 web3-6.2.0/ethpm/
+-rw-r--r--   0 eve        (501) staff       (20)      580 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.233226 web3-6.2.0/ethpm/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2511 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/_utils/backend.py
+-rw-r--r--   0 eve        (501) staff       (20)     1477 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     2848 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/chains.py
+-rw-r--r--   0 eve        (501) staff       (20)     1030 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     5263 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/deployments.py
+-rw-r--r--   0 eve        (501) staff       (20)     2717 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/ipfs.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.233576 web3-6.2.0/ethpm/_utils/protobuf/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/protobuf/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1938 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-r--r--   0 eve        (501) staff       (20)     1488 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/_utils/registry.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.233896 web3-6.2.0/ethpm/assets/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.234181 web3-6.2.0/ethpm/assets/ens/
+-rw-r--r--   0 eve        (501) staff       (20)    74682 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/ens/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.234522 web3-6.2.0/ethpm/assets/escrow/
+-rw-r--r--   0 eve        (501) staff       (20)     8007 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/escrow/with_bytecode_v3.json
+-rw-r--r--   0 eve        (501) staff       (20)      760 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/ipfs_file.proto
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.234858 web3-6.2.0/ethpm/assets/owned/
+-rw-r--r--   0 eve        (501) staff       (20)     2655 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/owned/output_v3.json
+-rw-r--r--   0 eve        (501) staff       (20)      746 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/owned/with_contract_type_v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.237090 web3-6.2.0/ethpm/assets/registry/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.239286 web3-6.2.0/ethpm/assets/registry/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     3129 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/Authority.sol
+-rw-r--r--   0 eve        (501) staff       (20)     2876 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
+-rw-r--r--   0 eve        (501) staff       (20)     6380 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/PackageDB.sol
+-rw-r--r--   0 eve        (501) staff       (20)    10553 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 eve        (501) staff       (20)     2966 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 eve        (501) staff       (20)     9041 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/ReleaseDB.sol
+-rw-r--r--   0 eve        (501) staff       (20)     4980 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
+-rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/solc_input.json
+-rw-r--r--   0 eve        (501) staff       (20)   727775 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/solc_output.json
+-rw-r--r--   0 eve        (501) staff       (20)   270218 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/registry/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.239477 web3-6.2.0/ethpm/assets/safe-math-lib/
+-rw-r--r--   0 eve        (501) staff       (20)     2845 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.240964 web3-6.2.0/ethpm/assets/simple-registry/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.242277 web3-6.2.0/ethpm/assets/simple-registry/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     1841 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/simple-registry/contracts/Ownable.sol
+-rw-r--r--   0 eve        (501) staff       (20)    12350 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 eve        (501) staff       (20)     3278 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 eve        (501) staff       (20)      950 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/simple-registry/solc_input.json
+-rw-r--r--   0 eve        (501) staff       (20)   199338 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/simple-registry/solc_output.json
+-rw-r--r--   0 eve        (501) staff       (20)    75677 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/simple-registry/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.242912 web3-6.2.0/ethpm/assets/standard-token/
+-rw-r--r--   0 eve        (501) staff       (20)    22292 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/standard-token/output_v3.json
+-rw-r--r--   0 eve        (501) staff       (20)     8765 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/standard-token/with_bytecode_v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.243514 web3-6.2.0/ethpm/assets/vyper_registry/
+-rw-r--r--   0 eve        (501) staff       (20)    81363 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/vyper_registry/0.1.0.json
+-rw-r--r--   0 eve        (501) staff       (20)     6339 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/vyper_registry/registry.vy
+-rw-r--r--   0 eve        (501) staff       (20)     7596 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/assets/vyper_registry/registry_with_delete.vy
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.244199 web3-6.2.0/ethpm/backends/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/backends/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      956 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/backends/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     3006 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/backends/http.py
+-rw-r--r--   0 eve        (501) staff       (20)     6551 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/backends/ipfs.py
+-rw-r--r--   0 eve        (501) staff       (20)     4174 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/backends/registry.py
+-rw-r--r--   0 eve        (501) staff       (20)      405 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     6256 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     1890 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/dependencies.py
+-rw-r--r--   0 eve        (501) staff       (20)     2134 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/deployments.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.223567 web3-6.2.0/ethpm/ethpm-spec/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.223357 web3-6.2.0/ethpm/ethpm-spec/examples/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.245020 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/
+-rw-r--r--   0 eve        (501) staff       (20)     6810 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     5361 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.245333 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      888 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
+-rw-r--r--   0 eve        (501) staff       (20)      644 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
+-rw-r--r--   0 eve        (501) staff       (20)    11598 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     8669 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/escrow/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.245891 web3-6.2.0/ethpm/ethpm-spec/examples/owned/
+-rw-r--r--   0 eve        (501) staff       (20)      544 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      443 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.246031 web3-6.2.0/ethpm/ethpm-spec/examples/owned/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      222 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
+-rw-r--r--   0 eve        (501) staff       (20)      728 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/owned/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.246603 web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/
+-rw-r--r--   0 eve        (501) staff       (20)     5272 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     5030 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
+-rw-r--r--   0 eve        (501) staff       (20)     5220 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     4993 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.247187 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/
+-rw-r--r--   0 eve        (501) staff       (20)     3976 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     3143 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.247419 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      802 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
+-rw-r--r--   0 eve        (501) staff       (20)     5517 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     3289 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.248060 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/
+-rw-r--r--   0 eve        (501) staff       (20)     3794 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     3238 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.248354 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     1155 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
+-rw-r--r--   0 eve        (501) staff       (20)     2949 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
+-rw-r--r--   0 eve        (501) staff       (20)    17129 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     6100 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.249251 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/
+-rw-r--r--   0 eve        (501) staff       (20)      590 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      507 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.249537 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      396 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
+-rw-r--r--   0 eve        (501) staff       (20)      786 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      548 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/transferable/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.250357 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/
+-rw-r--r--   0 eve        (501) staff       (20)     6669 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     5456 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.251349 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     1454 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
+-rw-r--r--   0 eve        (501) staff       (20)     9710 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     7326 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.251041 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/
+-rw-r--r--   0 eve        (501) staff       (20)     8052 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     6657 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.251207 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      621 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
+-rw-r--r--   0 eve        (501) staff       (20)    12191 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     9503 2022-04-27 21:13:00.000000 web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.251757 web3-6.2.0/ethpm/ethpm-spec/spec/
+-rw-r--r--   0 eve        (501) staff       (20)    10302 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/spec/package.spec.json
+-rw-r--r--   0 eve        (501) staff       (20)    12879 2021-02-11 20:53:14.000000 web3-6.2.0/ethpm/ethpm-spec/spec/v3.spec.json
+-rw-r--r--   0 eve        (501) staff       (20)     1194 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    14493 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/package.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.252529 web3-6.2.0/ethpm/tools/
+-rw-r--r--   0 eve        (501) staff       (20)      103 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/tools/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    27045 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/tools/builder.py
+-rw-r--r--   0 eve        (501) staff       (20)    10373 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/tools/checker.py
+-rw-r--r--   0 eve        (501) staff       (20)      475 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/tools/get_manifest.py
+-rw-r--r--   0 eve        (501) staff       (20)     4368 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/uri.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.253398 web3-6.2.0/ethpm/validation/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/validation/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4716 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/validation/manifest.py
+-rw-r--r--   0 eve        (501) staff       (20)     1072 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/validation/misc.py
+-rw-r--r--   0 eve        (501) staff       (20)     2317 2023-04-06 21:34:13.000000 web3-6.2.0/ethpm/validation/package.py
+-rw-r--r--   0 eve        (501) staff       (20)     4873 2023-04-10 20:16:28.000000 web3-6.2.0/ethpm/validation/uri.py
+-rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-10 20:16:28.000000 web3-6.2.0/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-04-12 19:40:44.284843 web3-6.2.0/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     3168 2023-04-12 19:39:58.000000 web3-6.2.0/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.257621 web3-6.2.0/web3/
+-rw-r--r--   0 eve        (501) staff       (20)      752 2023-04-10 20:16:28.000000 web3-6.2.0/web3/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.265895 web3-6.2.0/web3/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    28771 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)      456 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/async_caching.py
+-rw-r--r--   0 eve        (501) staff       (20)     7693 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/async_transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     2059 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      992 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/caching.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.266378 web3-6.2.0/web3/_utils/compat/
+-rw-r--r--   0 eve        (501) staff       (20)      319 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/compat/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/compat/compat_py2.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/compat/compat_py3.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.266564 web3-6.2.0/web3/_utils/contract_sources/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     6406 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/compile_contracts.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.270509 web3-6.2.0/web3/_utils/contract_sources/contract_data/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      517 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-r--r--   0 eve        (501) staff       (20)     5344 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/address_reflector.py
+-rw-r--r--   0 eve        (501) staff       (20)    19324 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    15157 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     6219 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     6492 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-r--r--   0 eve        (501) staff       (20)    38375 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     5673 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/event_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)    16216 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-r--r--   0 eve        (501) staff       (20)     1685 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     7829 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/math_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    17122 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-r--r--   0 eve        (501) staff       (20)    33495 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-r--r--   0 eve        (501) staff       (20)     1863 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/payable_tester.py
+-rw-r--r--   0 eve        (501) staff       (20)    17734 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     5410 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     2719 2023-04-12 17:22:18.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/revert_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     3653 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-r--r--   0 eve        (501) staff       (20)    11900 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/string_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    23756 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)    14980 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     1640 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1738 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/decorators.py
+-rw-r--r--   0 eve        (501) staff       (20)      144 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/empty.py
+-rw-r--r--   0 eve        (501) staff       (20)     9065 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)     2120 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/ens.py
+-rw-r--r--   0 eve        (501) staff       (20)    17073 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/events.py
+-rw-r--r--   0 eve        (501) staff       (20)     2113 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/fee_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)    11886 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/filters.py
+-rw-r--r--   0 eve        (501) staff       (20)     3071 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)       55 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/function_identifiers.py
+-rw-r--r--   0 eve        (501) staff       (20)      195 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/http.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/hypothesis.py
+-rw-r--r--   0 eve        (501) staff       (20)     1047 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/math.py
+-rw-r--r--   0 eve        (501) staff       (20)    32178 2023-04-12 17:22:18.000000 web3-6.2.0/web3/_utils/method_formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)     1146 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/miner.py
+-rw-r--r--   0 eve        (501) staff       (20)     3147 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.272274 web3-6.2.0/web3/_utils/module_testing/
+-rw-r--r--   0 eve        (501) staff       (20)      539 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)   157070 2023-04-12 17:22:18.000000 web3-6.2.0/web3/_utils/module_testing/eth_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     3406 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/go_ethereum_admin_module.py
+-rw-r--r--   0 eve        (501) staff       (20)    10338 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/go_ethereum_personal_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     1176 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     4825 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/module_testing_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1272 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/net_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     9335 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/module_testing/web3_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     6493 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/normalizers.py
+-rw-r--r--   0 eve        (501) staff       (20)     8833 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/request.py
+-rw-r--r--   0 eve        (501) staff       (20)     9449 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/rpc_abi.py
+-rw-r--r--   0 eve        (501) staff       (20)     4207 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/threads.py
+-rw-r--r--   0 eve        (501) staff       (20)     8737 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      816 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/type_conversion.py
+-rw-r--r--   0 eve        (501) staff       (20)     1669 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/utility_methods.py
+-rw-r--r--   0 eve        (501) staff       (20)     6291 2023-04-10 20:16:28.000000 web3-6.2.0/web3/_utils/validation.py
+-rw-r--r--   0 eve        (501) staff       (20)      994 2023-04-06 21:34:13.000000 web3-6.2.0/web3/_utils/windows.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.272559 web3-6.2.0/web3/auto/
+-rw-r--r--   0 eve        (501) staff       (20)       44 2023-04-10 20:16:28.000000 web3-6.2.0/web3/auto/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      263 2023-04-06 21:34:13.000000 web3-6.2.0/web3/auto/gethdev.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.273125 web3-6.2.0/web3/beacon/
+-rw-r--r--   0 eve        (501) staff       (20)       91 2023-04-10 20:16:28.000000 web3-6.2.0/web3/beacon/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1516 2023-04-06 21:34:13.000000 web3-6.2.0/web3/beacon/api_endpoints.py
+-rw-r--r--   0 eve        (501) staff       (20)     5421 2023-04-06 21:34:13.000000 web3-6.2.0/web3/beacon/async_beacon.py
+-rw-r--r--   0 eve        (501) staff       (20)     4772 2023-04-06 21:34:13.000000 web3-6.2.0/web3/beacon/main.py
+-rw-r--r--   0 eve        (501) staff       (20)      396 2023-04-06 21:34:13.000000 web3-6.2.0/web3/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.274402 web3-6.2.0/web3/contract/
+-rw-r--r--   0 eve        (501) staff       (20)      215 2023-04-10 20:16:28.000000 web3-6.2.0/web3/contract/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    19756 2023-04-10 20:16:28.000000 web3-6.2.0/web3/contract/async_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    35710 2023-04-10 20:16:28.000000 web3-6.2.0/web3/contract/base_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    18804 2023-04-10 20:16:28.000000 web3-6.2.0/web3/contract/contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    12338 2023-04-10 20:16:28.000000 web3-6.2.0/web3/contract/utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     8271 2023-04-06 21:34:13.000000 web3-6.2.0/web3/datastructures.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.275111 web3-6.2.0/web3/eth/
+-rw-r--r--   0 eve        (501) staff       (20)      166 2023-04-10 20:16:28.000000 web3-6.2.0/web3/eth/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    19275 2023-04-10 20:16:28.000000 web3-6.2.0/web3/eth/async_eth.py
+-rw-r--r--   0 eve        (501) staff       (20)     5943 2023-04-10 20:16:28.000000 web3-6.2.0/web3/eth/base_eth.py
+-rw-r--r--   0 eve        (501) staff       (20)    19295 2023-04-10 20:16:28.000000 web3-6.2.0/web3/eth/eth.py
+-rw-r--r--   0 eve        (501) staff       (20)     5780 2023-04-12 17:22:18.000000 web3-6.2.0/web3/exceptions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.275611 web3-6.2.0/web3/gas_strategies/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/gas_strategies/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      430 2023-04-10 20:16:28.000000 web3-6.2.0/web3/gas_strategies/rpc.py
+-rw-r--r--   0 eve        (501) staff       (20)     9010 2023-04-10 20:16:28.000000 web3-6.2.0/web3/gas_strategies/time_based.py
+-rw-r--r--   0 eve        (501) staff       (20)    11826 2023-04-10 20:16:28.000000 web3-6.2.0/web3/geth.py
+-rw-r--r--   0 eve        (501) staff       (20)      198 2023-04-06 21:34:13.000000 web3-6.2.0/web3/logs.py
+-rw-r--r--   0 eve        (501) staff       (20)    12686 2023-04-10 20:16:28.000000 web3-6.2.0/web3/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     7875 2023-04-10 20:16:28.000000 web3-6.2.0/web3/manager.py
+-rw-r--r--   0 eve        (501) staff       (20)     8430 2023-04-06 21:34:13.000000 web3-6.2.0/web3/method.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.279111 web3-6.2.0/web3/middleware/
+-rw-r--r--   0 eve        (501) staff       (20)     3724 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      239 2023-04-06 21:34:13.000000 web3-6.2.0/web3/middleware/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)     2755 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/async_cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     1779 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/attrdict.py
+-rw-r--r--   0 eve        (501) staff       (20)     1785 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/buffered_gas_estimate.py
+-rw-r--r--   0 eve        (501) staff       (20)    12617 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     1167 2023-04-06 21:34:13.000000 web3-6.2.0/web3/middleware/exception_handling.py
+-rw-r--r--   0 eve        (501) staff       (20)     3119 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/exception_retry_request.py
+-rw-r--r--   0 eve        (501) staff       (20)    21131 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/filter.py
+-rw-r--r--   0 eve        (501) staff       (20)     4596 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/fixture.py
+-rw-r--r--   0 eve        (501) staff       (20)     4762 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/formatting.py
+-rw-r--r--   0 eve        (501) staff       (20)     4212 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/gas_price_strategy.py
+-rw-r--r--   0 eve        (501) staff       (20)     1657 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/geth_poa.py
+-rw-r--r--   0 eve        (501) staff       (20)      590 2023-04-06 21:34:13.000000 web3-6.2.0/web3/middleware/names.py
+-rw-r--r--   0 eve        (501) staff       (20)      246 2023-04-06 21:34:13.000000 web3-6.2.0/web3/middleware/normalize_request_parameters.py
+-rw-r--r--   0 eve        (501) staff       (20)      351 2023-04-06 21:34:13.000000 web3-6.2.0/web3/middleware/pythonic.py
+-rw-r--r--   0 eve        (501) staff       (20)     4450 2023-04-06 21:34:13.000000 web3-6.2.0/web3/middleware/signing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1014 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/simulate_unmined_transaction.py
+-rw-r--r--   0 eve        (501) staff       (20)     3739 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/stalecheck.py
+-rw-r--r--   0 eve        (501) staff       (20)     4573 2023-04-10 20:16:28.000000 web3-6.2.0/web3/middleware/validation.py
+-rw-r--r--   0 eve        (501) staff       (20)     3615 2023-04-10 20:16:28.000000 web3-6.2.0/web3/module.py
+-rw-r--r--   0 eve        (501) staff       (20)     1562 2023-04-06 21:34:13.000000 web3-6.2.0/web3/net.py
+-rw-r--r--   0 eve        (501) staff       (20)    21609 2023-04-10 20:16:28.000000 web3-6.2.0/web3/pm.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.280364 web3-6.2.0/web3/providers/
+-rw-r--r--   0 eve        (501) staff       (20)      368 2023-04-06 21:34:13.000000 web3-6.2.0/web3/providers/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3544 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/async_base.py
+-rw-r--r--   0 eve        (501) staff       (20)     2469 2023-04-06 21:34:13.000000 web3-6.2.0/web3/providers/async_rpc.py
+-rw-r--r--   0 eve        (501) staff       (20)     3403 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/auto.py
+-rw-r--r--   0 eve        (501) staff       (20)     3477 2023-04-06 21:34:13.000000 web3-6.2.0/web3/providers/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.280885 web3-6.2.0/web3/providers/eth_tester/
+-rw-r--r--   0 eve        (501) staff       (20)       97 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/eth_tester/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    14296 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/eth_tester/defaults.py
+-rw-r--r--   0 eve        (501) staff       (20)     5452 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/eth_tester/main.py
+-rw-r--r--   0 eve        (501) staff       (20)    12665 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/eth_tester/middleware.py
+-rw-r--r--   0 eve        (501) staff       (20)     6534 2023-04-10 20:16:28.000000 web3-6.2.0/web3/providers/ipc.py
+-rw-r--r--   0 eve        (501) staff       (20)     2686 2023-04-06 21:34:13.000000 web3-6.2.0/web3/providers/rpc.py
+-rw-r--r--   0 eve        (501) staff       (20)     3919 2023-04-06 21:34:13.000000 web3-6.2.0/web3/providers/websocket.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.281035 web3-6.2.0/web3/scripts/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/scripts/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.281221 web3-6.2.0/web3/scripts/release/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/scripts/release/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1534 2023-04-06 21:34:13.000000 web3-6.2.0/web3/scripts/release/test_package.py
+-rw-r--r--   0 eve        (501) staff       (20)      951 2023-04-06 21:34:13.000000 web3-6.2.0/web3/testing.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.281386 web3-6.2.0/web3/tools/
+-rw-r--r--   0 eve        (501) staff       (20)       73 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.282332 web3-6.2.0/web3/tools/benchmark/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/benchmark/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5886 2023-04-10 20:16:28.000000 web3-6.2.0/web3/tools/benchmark/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     3435 2023-04-10 20:16:28.000000 web3-6.2.0/web3/tools/benchmark/node.py
+-rw-r--r--   0 eve        (501) staff       (20)      912 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/benchmark/reporting.py
+-rw-r--r--   0 eve        (501) staff       (20)     1722 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/benchmark/utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.283488 web3-6.2.0/web3/tools/pytest_ethereum/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/pytest_ethereum/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4158 2023-04-10 20:16:28.000000 web3-6.2.0/web3/tools/pytest_ethereum/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1423 2023-04-10 20:16:28.000000 web3-6.2.0/web3/tools/pytest_ethereum/deployer.py
+-rw-r--r--   0 eve        (501) staff       (20)      380 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/pytest_ethereum/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)     3927 2023-04-06 21:34:13.000000 web3-6.2.0/web3/tools/pytest_ethereum/linker.py
+-rw-r--r--   0 eve        (501) staff       (20)      645 2023-04-10 20:16:28.000000 web3-6.2.0/web3/tools/pytest_ethereum/plugins.py
+-rw-r--r--   0 eve        (501) staff       (20)     2968 2023-04-12 17:56:02.000000 web3-6.2.0/web3/tracing.py
+-rw-r--r--   0 eve        (501) staff       (20)    10665 2023-04-12 17:20:28.000000 web3-6.2.0/web3/types.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.284407 web3-6.2.0/web3/utils/
+-rw-r--r--   0 eve        (501) staff       (20)      454 2023-04-06 21:34:13.000000 web3-6.2.0/web3/utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      498 2023-04-06 21:34:13.000000 web3-6.2.0/web3/utils/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)      967 2023-04-06 21:34:13.000000 web3-6.2.0/web3/utils/address.py
+-rw-r--r--   0 eve        (501) staff       (20)     3096 2023-04-06 21:34:13.000000 web3-6.2.0/web3/utils/async_exception_handling.py
+-rw-r--r--   0 eve        (501) staff       (20)     1521 2023-04-06 21:34:13.000000 web3-6.2.0/web3/utils/caching.py
+-rw-r--r--   0 eve        (501) staff       (20)     3052 2023-04-06 21:34:13.000000 web3-6.2.0/web3/utils/exception_handling.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-12 19:40:44.258881 web3-6.2.0/web3.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     2184 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     9743 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)       64 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/entry_points.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)     1165 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)       15 2023-04-12 19:40:44.000000 web3-6.2.0/web3.egg-info/top_level.txt
```

### Comparing `web3-6.1.0/LICENSE` & `web3-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/PKG-INFO` & `web3-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.1.0
+Version: 6.2.0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.1.0/README.md` & `web3-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/abis.py` & `web3-6.2.0/ens/abis.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/async_ens.py` & `web3-6.2.0/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/base_ens.py` & `web3-6.2.0/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/constants.py` & `web3-6.2.0/ens/constants.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/contract_data.py` & `web3-6.2.0/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/ens.py` & `web3-6.2.0/ens/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/exceptions.py` & `web3-6.2.0/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ens/utils.py` & `web3-6.2.0/ens/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/__init__.py` & `web3-6.2.0/ethpm/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/backend.py` & `web3-6.2.0/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/cache.py` & `web3-6.2.0/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/chains.py` & `web3-6.2.0/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/contract.py` & `web3-6.2.0/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/deployments.py` & `web3-6.2.0/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/ipfs.py` & `web3-6.2.0/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `web3-6.2.0/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/_utils/registry.py` & `web3-6.2.0/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/ens/v3.json` & `web3-6.2.0/ethpm/assets/ens/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/escrow/with_bytecode_v3.json` & `web3-6.2.0/ethpm/assets/escrow/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/ipfs_file.proto` & `web3-6.2.0/ethpm/assets/ipfs_file.proto`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/owned/output_v3.json` & `web3-6.2.0/ethpm/assets/owned/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/owned/with_contract_type_v3.json` & `web3-6.2.0/ethpm/assets/owned/with_contract_type_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/Authority.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/Authority.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/PackageDB.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/PackageDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/PackageRegistry.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/ReleaseDB.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/ReleaseDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/contracts/ReleaseValidator.sol` & `web3-6.2.0/ethpm/assets/registry/contracts/ReleaseValidator.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/solc_input.json` & `web3-6.2.0/ethpm/assets/registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/solc_output.json` & `web3-6.2.0/ethpm/assets/registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/registry/v3.json` & `web3-6.2.0/ethpm/assets/registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json` & `web3-6.2.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/simple-registry/contracts/Ownable.sol` & `web3-6.2.0/ethpm/assets/simple-registry/contracts/Ownable.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol` & `web3-6.2.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol` & `web3-6.2.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/simple-registry/solc_input.json` & `web3-6.2.0/ethpm/assets/simple-registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/simple-registry/solc_output.json` & `web3-6.2.0/ethpm/assets/simple-registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/simple-registry/v3.json` & `web3-6.2.0/ethpm/assets/simple-registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/standard-token/output_v3.json` & `web3-6.2.0/ethpm/assets/standard-token/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/standard-token/with_bytecode_v3.json` & `web3-6.2.0/ethpm/assets/standard-token/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/vyper_registry/0.1.0.json` & `web3-6.2.0/ethpm/assets/vyper_registry/0.1.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/vyper_registry/registry.vy` & `web3-6.2.0/ethpm/assets/vyper_registry/registry.vy`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/assets/vyper_registry/registry_with_delete.vy` & `web3-6.2.0/ethpm/assets/vyper_registry/registry_with_delete.vy`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/backends/base.py` & `web3-6.2.0/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/backends/http.py` & `web3-6.2.0/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/backends/ipfs.py` & `web3-6.2.0/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/backends/registry.py` & `web3-6.2.0/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/contract.py` & `web3-6.2.0/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/dependencies.py` & `web3-6.2.0/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/deployments.py` & `web3-6.2.0/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/escrow/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/escrow/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/piper-coin/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/piper-coin/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/standard-token/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/standard-token/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/transferable/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/transferable/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json` & `web3-6.2.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/spec/package.spec.json` & `web3-6.2.0/ethpm/ethpm-spec/spec/package.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/ethpm-spec/spec/v3.spec.json` & `web3-6.2.0/ethpm/ethpm-spec/spec/v3.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/exceptions.py` & `web3-6.2.0/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/package.py` & `web3-6.2.0/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/tools/builder.py` & `web3-6.2.0/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/tools/checker.py` & `web3-6.2.0/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/uri.py` & `web3-6.2.0/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/validation/manifest.py` & `web3-6.2.0/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/validation/misc.py` & `web3-6.2.0/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/validation/package.py` & `web3-6.2.0/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/ethpm/validation/uri.py` & `web3-6.2.0/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/pyproject.toml` & `web3-6.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/setup.py` & `web3-6.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="web3",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="6.1.0",
+    version="6.2.0",
     description="""web3.py""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/web3.py",
     include_package_data=True,
```

### Comparing `web3-6.1.0/web3/__init__.py` & `web3-6.2.0/web3/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/abi.py` & `web3-6.2.0/web3/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/async_transactions.py` & `web3-6.2.0/web3/_utils/async_transactions.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,26 @@
 from eth_typing import (
     URI,
 )
 from eth_utils.toolz import (
     curry,
     merge,
 )
+from hexbytes import (
+    HexBytes,
+)
 
 from web3._utils.request import (
     async_get_json_from_client_response,
     async_get_response_from_get_request,
     async_get_response_from_post_request,
 )
+from web3._utils.transactions import (
+    prepare_replacement_transaction,
+)
 from web3._utils.type_conversion import (
     to_bytes_if_hex,
     to_hex_if_bytes,
 )
 from web3._utils.utility_methods import (
     any_in_dict,
 )
@@ -33,16 +39,18 @@
     DYNAMIC_FEE_TXN_PARAMS,
 )
 from web3.exceptions import (
     Web3ValidationError,
 )
 from web3.types import (
     BlockIdentifier,
+    TxData,
     TxParams,
     Wei,
+    _Hash32,
 )
 
 if TYPE_CHECKING:
     from web3.eth import AsyncEth  # noqa: F401
     from web3.main import (  # noqa: F401
         AsyncWeb3,
     )
@@ -211,7 +219,27 @@
                     ],
                 ),
             ]
         )
 
         return encoded_data_with_function_selector
     raise Exception("Offchain lookup failed for supplied urls.")
+
+
+async def async_get_required_transaction(
+    async_w3: "AsyncWeb3", transaction_hash: _Hash32
+) -> TxData:
+    current_transaction = await async_w3.eth.get_transaction(transaction_hash)
+    if not current_transaction:
+        raise ValueError(
+            f"Supplied transaction with hash {transaction_hash!r} does not exist"
+        )
+    return current_transaction
+
+
+async def async_replace_transaction(
+    async_w3: "AsyncWeb3", current_transaction: TxData, new_transaction: TxParams
+) -> HexBytes:
+    new_transaction = prepare_replacement_transaction(
+        async_w3, current_transaction, new_transaction
+    )
+    return await async_w3.eth.send_transaction(new_transaction)
```

### Comparing `web3-6.1.0/web3/_utils/blocks.py` & `web3-6.2.0/web3/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/caching.py` & `web3-6.2.0/web3/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/compile_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/address_reflector.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/arrays_contract.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/arrays_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/emitter_contract.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/event_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/extended_resolver.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/math_contract.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/math_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/payable_tester.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/payable_tester.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/revert_contract.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/revert_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/simple_resolver.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/simple_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/string_contract.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/string_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py` & `web3-6.2.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/contracts.py` & `web3-6.2.0/web3/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/datatypes.py` & `web3-6.2.0/web3/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/decorators.py` & `web3-6.2.0/web3/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/encoding.py` & `web3-6.2.0/web3/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/ens.py` & `web3-6.2.0/web3/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/events.py` & `web3-6.2.0/web3/_utils/events.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/fee_utils.py` & `web3-6.2.0/web3/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/filters.py` & `web3-6.2.0/web3/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/formatters.py` & `web3-6.2.0/web3/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/math.py` & `web3-6.2.0/web3/_utils/math.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/method_formatters.py` & `web3-6.2.0/web3/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/miner.py` & `web3-6.2.0/web3/_utils/miner.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module.py` & `web3-6.2.0/web3/_utils/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/__init__.py` & `web3-6.2.0/web3/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/eth_module.py` & `web3-6.2.0/web3/_utils/module_testing/eth_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,115 @@
         assert is_same_address(txn["from"], cast(ChecksumAddress, txn_params["from"]))
         assert is_same_address(txn["to"], cast(ChecksumAddress, txn_params["to"]))
         assert txn["value"] == 1
         assert txn["gas"] == 21000
         assert txn["gasPrice"] == txn_params["gasPrice"]
 
     @pytest.mark.asyncio
+    async def test_async_eth_sign_transaction(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": async_w3.to_wei(2, "gwei"),
+            "maxPriorityFeePerGas": async_w3.to_wei(1, "gwei"),
+            "nonce": Nonce(0),
+        }
+        result = await async_w3.eth.sign_transaction(txn_params)
+        signatory_account = async_w3.eth.account.recover_transaction(result["raw"])
+        assert unlocked_account == signatory_account
+        assert result["tx"]["to"] == txn_params["to"]
+        assert result["tx"]["value"] == txn_params["value"]
+        assert result["tx"]["gas"] == txn_params["gas"]
+        assert result["tx"]["maxFeePerGas"] == txn_params["maxFeePerGas"]
+        assert (
+            result["tx"]["maxPriorityFeePerGas"] == txn_params["maxPriorityFeePerGas"]
+        )
+        assert result["tx"]["nonce"] == txn_params["nonce"]
+
+    @pytest.mark.asyncio
+    async def test_async_eth_sign_transaction_legacy(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "gasPrice": await async_w3.eth.gas_price,
+            "nonce": Nonce(0),
+        }
+        result = await async_w3.eth.sign_transaction(txn_params)
+        signatory_account = async_w3.eth.account.recover_transaction(result["raw"])
+        assert unlocked_account == signatory_account
+        assert result["tx"]["to"] == txn_params["to"]
+        assert result["tx"]["value"] == txn_params["value"]
+        assert result["tx"]["gas"] == txn_params["gas"]
+        assert result["tx"]["gasPrice"] == txn_params["gasPrice"]
+        assert result["tx"]["nonce"] == txn_params["nonce"]
+
+    @pytest.mark.asyncio
+    async def test_async_eth_sign_transaction_hex_fees(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": hex(async_w3.to_wei(2, "gwei")),
+            "maxPriorityFeePerGas": hex(async_w3.to_wei(1, "gwei")),
+            "nonce": Nonce(0),
+        }
+        result = await async_w3.eth.sign_transaction(txn_params)
+        signatory_account = async_w3.eth.account.recover_transaction(result["raw"])
+        assert unlocked_account == signatory_account
+        assert result["tx"]["to"] == txn_params["to"]
+        assert result["tx"]["value"] == txn_params["value"]
+        assert result["tx"]["gas"] == txn_params["gas"]
+        assert result["tx"]["maxFeePerGas"] == int(str(txn_params["maxFeePerGas"]), 16)
+        assert result["tx"]["maxPriorityFeePerGas"] == int(
+            str(txn_params["maxPriorityFeePerGas"]), 16
+        )
+        assert result["tx"]["nonce"] == txn_params["nonce"]
+
+    @pytest.mark.asyncio
+    @pytest.mark.xfail(
+        reason="async name_to_address_middleware has not been implemented yet"
+    )
+    async def test_async_eth_sign_transaction_ens_names(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        with ens_addresses(async_w3, {"unlocked-account.eth": unlocked_account}):
+            txn_params: TxParams = {
+                "from": "unlocked-account.eth",
+                "to": "unlocked-account.eth",
+                "value": Wei(1),
+                "gas": 21000,
+                "maxFeePerGas": async_w3.to_wei(2, "gwei"),
+                "maxPriorityFeePerGas": async_w3.to_wei(1, "gwei"),
+                "nonce": Nonce(0),
+            }
+            result = await async_w3.eth.sign_transaction(txn_params)
+            signatory_account = async_w3.eth.account.recover_transaction(result["raw"])
+            assert unlocked_account == signatory_account
+            assert result["tx"]["to"] == unlocked_account
+            assert result["tx"]["value"] == txn_params["value"]
+            assert result["tx"]["gas"] == txn_params["gas"]
+            assert result["tx"]["maxFeePerGas"] == txn_params["maxFeePerGas"]
+            assert (
+                result["tx"]["maxPriorityFeePerGas"]
+                == txn_params["maxPriorityFeePerGas"]
+            )
+            assert result["tx"]["nonce"] == txn_params["nonce"]
+
+    @pytest.mark.asyncio
     async def test_eth_send_transaction(
         self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
     ) -> None:
         txn_params: TxParams = {
             "from": unlocked_account_dual_type,
             "to": unlocked_account_dual_type,
             "value": Wei(1),
@@ -1485,14 +1586,32 @@
             block_with_txn["hash"]
         )
 
         assert is_integer(transaction_count)
         assert transaction_count >= 1
 
     @pytest.mark.asyncio
+    async def test_eth_getUncleCountByBlockHash(
+        self, async_w3: "AsyncWeb3", empty_block: BlockData
+    ) -> None:
+        uncle_count = await async_w3.eth.get_uncle_count(empty_block["hash"])
+
+        assert is_integer(uncle_count)
+        assert uncle_count == 0
+
+    @pytest.mark.asyncio
+    async def test_eth_getUncleCountByBlockNumber(
+        self, async_w3: "AsyncWeb3", empty_block: BlockData
+    ) -> None:
+        uncle_count = await async_w3.eth.get_uncle_count(empty_block["number"])
+
+        assert is_integer(uncle_count)
+        assert uncle_count == 0
+
+    @pytest.mark.asyncio
     async def test_eth_getBlockTransactionCountByNumber_block_with_txn(
         self, async_w3: "AsyncWeb3", block_with_txn: BlockData
     ) -> None:
         transaction_count = await async_w3.eth.get_block_transaction_count(
             block_with_txn["number"]
         )
 
@@ -1545,14 +1664,259 @@
             signature = await async_w3.eth.sign(
                 ENS("unlocked-acct.eth"), text="Message tö sign. Longer than hash!"
             )
             assert is_bytes(signature)
             assert len(signature) == 32 + 32 + 1
 
     @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_legacy(
+        self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account_dual_type,
+            "to": unlocked_account_dual_type,
+            "value": Wei(1),
+            "gas": 21000,
+            "gasPrice": async_w3.to_wei(
+                1, "gwei"
+            ),  # must be greater than base_fee post London
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        txn_params["gasPrice"] = async_w3.to_wei(2, "gwei")
+        replace_txn_hash = await async_w3.eth.replace_transaction(txn_hash, txn_params)
+        replace_txn = await async_w3.eth.get_transaction(replace_txn_hash)
+
+        assert is_same_address(
+            replace_txn["from"], cast(ChecksumAddress, txn_params["from"])
+        )
+        assert is_same_address(
+            replace_txn["to"], cast(ChecksumAddress, txn_params["to"])
+        )
+        assert replace_txn["value"] == 1
+        assert replace_txn["gas"] == 21000
+        assert replace_txn["gasPrice"] == txn_params["gasPrice"]
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction(
+        self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
+    ) -> None:
+        two_gwei_in_wei = async_w3.to_wei(2, "gwei")
+        three_gwei_in_wei = async_w3.to_wei(3, "gwei")
+
+        txn_params: TxParams = {
+            "from": unlocked_account_dual_type,
+            "to": unlocked_account_dual_type,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": two_gwei_in_wei,
+            "maxPriorityFeePerGas": async_w3.to_wei(1, "gwei"),
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        txn_params["maxFeePerGas"] = three_gwei_in_wei
+        txn_params["maxPriorityFeePerGas"] = two_gwei_in_wei
+
+        replace_txn_hash = await async_w3.eth.replace_transaction(txn_hash, txn_params)
+        replace_txn = await async_w3.eth.get_transaction(replace_txn_hash)
+
+        assert is_same_address(
+            replace_txn["from"], cast(ChecksumAddress, txn_params["from"])
+        )
+        assert is_same_address(
+            replace_txn["to"], cast(ChecksumAddress, txn_params["to"])
+        )
+        assert replace_txn["value"] == 1
+        assert replace_txn["gas"] == 21000
+        assert replace_txn["maxFeePerGas"] == three_gwei_in_wei
+        assert replace_txn["maxPriorityFeePerGas"] == two_gwei_in_wei
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_underpriced(
+        self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account_dual_type,
+            "to": unlocked_account_dual_type,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": async_w3.to_wei(3, "gwei"),
+            "maxPriorityFeePerGas": async_w3.to_wei(2, "gwei"),
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        one_gwei_in_wei = async_w3.to_wei(1, "gwei")
+        txn_params["maxFeePerGas"] = one_gwei_in_wei
+        txn_params["maxPriorityFeePerGas"] = one_gwei_in_wei
+
+        with pytest.raises(ValueError, match="replacement transaction underpriced"):
+            await async_w3.eth.replace_transaction(txn_hash, txn_params)
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_non_existing_transaction(
+        self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account_dual_type,
+            "to": unlocked_account_dual_type,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": async_w3.to_wei(3, "gwei"),
+            "maxPriorityFeePerGas": async_w3.to_wei(1, "gwei"),
+        }
+        with pytest.raises(TransactionNotFound):
+            await async_w3.eth.replace_transaction(
+                HexStr(
+                    "0x98e8cc09b311583c5079fa600f6c2a3bea8611af168c52e4b60b5b243a441997"
+                ),
+                txn_params,
+            )
+
+    @pytest.mark.asyncio
+    @pytest.mark.xfail(reason="AsyncGethMiner is missing.")
+    async def test_async_eth_replace_transaction_already_mined(
+        self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account_dual_type,
+            "to": unlocked_account_dual_type,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": async_w3.to_wei(2, "gwei"),
+            "maxPriorityFeePerGas": async_w3.to_wei(1, "gwei"),
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+        try:
+            async_w3.geth.miner.start()  # type: ignore
+            await async_w3.eth.wait_for_transaction_receipt(txn_hash, timeout=10)
+        finally:
+            async_w3.geth.miner.stop()  # type: ignore
+
+        txn_params["maxFeePerGas"] = async_w3.to_wei(3, "gwei")
+        txn_params["maxPriorityFeePerGas"] = async_w3.to_wei(2, "gwei")
+        with pytest.raises(ValueError, match="Supplied transaction with hash"):
+            await async_w3.eth.replace_transaction(txn_hash, txn_params)
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_incorrect_nonce(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "maxFeePerGas": async_w3.to_wei(2, "gwei"),
+            "maxPriorityFeePerGas": async_w3.to_wei(1, "gwei"),
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+        txn = await async_w3.eth.get_transaction(txn_hash)
+
+        txn_params["maxFeePerGas"] = async_w3.to_wei(3, "gwei")
+        txn_params["maxPriorityFeePerGas"] = async_w3.to_wei(2, "gwei")
+        txn_params["nonce"] = Nonce(txn["nonce"] + 1)
+        with pytest.raises(ValueError):
+            await async_w3.eth.replace_transaction(txn_hash, txn_params)
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_gas_price_too_low(
+        self, async_w3: "AsyncWeb3", unlocked_account_dual_type: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account_dual_type,
+            "to": unlocked_account_dual_type,
+            "value": Wei(1),
+            "gas": 21000,
+            "gasPrice": async_w3.to_wei(2, "gwei"),
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        txn_params["gasPrice"] = async_w3.to_wei(1, "gwei")
+        with pytest.raises(ValueError):
+            await async_w3.eth.replace_transaction(txn_hash, txn_params)
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_gas_price_defaulting_minimum(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        gas_price = async_w3.to_wei(1, "gwei")
+
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "gasPrice": gas_price,
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        txn_params.pop("gasPrice")
+        replace_txn_hash = await async_w3.eth.replace_transaction(txn_hash, txn_params)
+        replace_txn = await async_w3.eth.get_transaction(replace_txn_hash)
+
+        assert replace_txn["gasPrice"] == math.ceil(
+            gas_price * 1.125
+        )  # minimum gas price
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_gas_price_defaulting_strategy_higher(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "gasPrice": async_w3.to_wei(1, "gwei"),
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        two_gwei_in_wei = async_w3.to_wei(2, "gwei")
+
+        def higher_gas_price_strategy(async_w3: "AsyncWeb3", txn: TxParams) -> Wei:
+            return two_gwei_in_wei
+
+        async_w3.eth.set_gas_price_strategy(higher_gas_price_strategy)
+
+        txn_params.pop("gasPrice")
+        replace_txn_hash = await async_w3.eth.replace_transaction(txn_hash, txn_params)
+        replace_txn = await async_w3.eth.get_transaction(replace_txn_hash)
+        assert (
+            replace_txn["gasPrice"] == two_gwei_in_wei
+        )  # Strategy provides higher gas price
+        async_w3.eth.set_gas_price_strategy(None)  # reset strategy
+
+    @pytest.mark.asyncio
+    async def test_async_eth_replace_transaction_gas_price_defaulting_strategy_lower(
+        self, async_w3: "AsyncWeb3", unlocked_account: ChecksumAddress
+    ) -> None:
+        gas_price = async_w3.to_wei(2, "gwei")
+
+        txn_params: TxParams = {
+            "from": unlocked_account,
+            "to": unlocked_account,
+            "value": Wei(1),
+            "gas": 21000,
+            "gasPrice": gas_price,
+        }
+        txn_hash = await async_w3.eth.send_transaction(txn_params)
+
+        def lower_gas_price_strategy(async_w3: "AsyncWeb3", txn: TxParams) -> Wei:
+            return async_w3.to_wei(1, "gwei")
+
+        async_w3.eth.set_gas_price_strategy(lower_gas_price_strategy)
+
+        txn_params.pop("gasPrice")
+        replace_txn_hash = await async_w3.eth.replace_transaction(txn_hash, txn_params)
+        replace_txn = await async_w3.eth.get_transaction(replace_txn_hash)
+        # Strategy provides lower gas price - minimum preferred
+        assert replace_txn["gasPrice"] == math.ceil(gas_price * 1.125)
+        async_w3.eth.set_gas_price_strategy(None)  # reset strategy
+
+    @pytest.mark.asyncio
     async def test_async_eth_new_filter(self, async_w3: "AsyncWeb3") -> None:
         filter = await async_w3.eth.filter({})
 
         changes = await async_w3.eth.get_filter_changes(filter.filter_id)
         assert is_list_like(changes)
         assert not changes
```

### Comparing `web3-6.1.0/web3/_utils/module_testing/go_ethereum_admin_module.py` & `web3-6.2.0/web3/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/go_ethereum_personal_module.py` & `web3-6.2.0/web3/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/go_ethereum_txpool_module.py` & `web3-6.2.0/web3/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/module_testing_utils.py` & `web3-6.2.0/web3/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/net_module.py` & `web3-6.2.0/web3/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/module_testing/web3_module.py` & `web3-6.2.0/web3/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/normalizers.py` & `web3-6.2.0/web3/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/request.py` & `web3-6.2.0/web3/_utils/request.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/rpc_abi.py` & `web3-6.2.0/web3/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/threads.py` & `web3-6.2.0/web3/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/transactions.py` & `web3-6.2.0/web3/_utils/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 from typing import (
     TYPE_CHECKING,
     List,
     Optional,
+    Union,
     cast,
 )
 
 from eth_typing import (
     ChecksumAddress,
 )
 from eth_utils.toolz import (
@@ -75,15 +76,18 @@
         + (2 * w3.eth.get_block("latest")["baseFeePerGas"])
     ),
     "maxPriorityFeePerGas": lambda w3, tx: w3.eth.max_priority_fee,
     "chainId": lambda w3, tx: w3.eth.chain_id,
 }
 
 if TYPE_CHECKING:
-    from web3 import Web3  # noqa: F401
+    from web3 import (  # noqa: F401
+        AsyncWeb3,
+        Web3,
+    )
 
 
 @curry
 def fill_nonce(w3: "Web3", transaction: TxParams) -> TxParams:
     if "from" in transaction and "nonce" not in transaction:
         return assoc(
             transaction,
@@ -215,15 +219,15 @@
 def assert_valid_transaction_params(transaction_params: TxParams) -> None:
     for param in transaction_params:
         if param not in VALID_TRANSACTION_PARAMS:
             raise ValueError(f"{param} is not a valid transaction parameter")
 
 
 def prepare_replacement_transaction(
-    w3: "Web3",
+    w3: Union["Web3", "AsyncWeb3"],
     original_transaction: TxData,
     replacement_transaction: TxParams,
     gas_multiplier: float = 1.125,
 ) -> TxParams:
     if original_transaction["blockHash"] is not None:
         raise ValueError(
             f'Supplied transaction with hash {original_transaction["hash"]!r} '
```

### Comparing `web3-6.1.0/web3/_utils/type_conversion.py` & `web3-6.2.0/web3/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/utility_methods.py` & `web3-6.2.0/web3/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/validation.py` & `web3-6.2.0/web3/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/_utils/windows.py` & `web3-6.2.0/web3/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/beacon/api_endpoints.py` & `web3-6.2.0/web3/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/beacon/async_beacon.py` & `web3-6.2.0/web3/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/beacon/main.py` & `web3-6.2.0/web3/beacon/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/contract/async_contract.py` & `web3-6.2.0/web3/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/contract/base_contract.py` & `web3-6.2.0/web3/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/contract/contract.py` & `web3-6.2.0/web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/contract/utils.py` & `web3-6.2.0/web3/contract/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/datastructures.py` & `web3-6.2.0/web3/datastructures.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/eth/async_eth.py` & `web3-6.2.0/web3/eth/async_eth.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     ChecksumAddress,
     HexStr,
 )
 from hexbytes import (
     HexBytes,
 )
 
+from web3._utils.async_transactions import (
+    async_get_required_transaction,
+    async_replace_transaction,
+)
 from web3._utils.blocks import (
     select_method_for_block_identifier,
 )
 from web3._utils.fee_utils import (
     async_fee_history_priority_fee,
 )
 from web3._utils.filters import (
@@ -59,14 +63,15 @@
     BlockIdentifier,
     BlockParams,
     CallOverride,
     FeeHistory,
     FilterParams,
     LogReceipt,
     Nonce,
+    SignedTx,
     SyncStatus,
     TxData,
     TxParams,
     TxReceipt,
     Wei,
     _Hash32,
 )
@@ -514,14 +519,24 @@
         self,
         account: Union[Address, ChecksumAddress, ENS],
         position: int,
         block_identifier: Optional[BlockIdentifier] = None,
     ) -> HexBytes:
         return await self._get_storage_at(account, position, block_identifier)
 
+    async def replace_transaction(
+        self, transaction_hash: _Hash32, new_transaction: TxParams
+    ) -> HexBytes:
+        current_transaction = await async_get_required_transaction(
+            self.w3, transaction_hash
+        )
+        return await async_replace_transaction(
+            self.w3, current_transaction, new_transaction
+        )
+
     # eth_sign
 
     _sign: Method[Callable[..., Awaitable[HexStr]]] = Method(
         RPC.eth_sign, mungers=[BaseEth.sign_munger]
     )
 
     async def sign(
@@ -529,14 +544,39 @@
         account: Union[Address, ChecksumAddress, ENS],
         data: Union[int, bytes] = None,
         hexstr: HexStr = None,
         text: str = None,
     ) -> HexStr:
         return await self._sign(account, data, hexstr, text)
 
+    # eth_signTransaction
+
+    _sign_transaction: Method[Callable[[TxParams], Awaitable[SignedTx]]] = Method(
+        RPC.eth_signTransaction,
+        mungers=[default_root_munger],
+    )
+
+    async def sign_transaction(self, transaction: TxParams) -> SignedTx:
+        return await self._sign_transaction(transaction)
+
+    # eth_getUncleCountByBlockHash
+    # eth_getUncleCountByBlockNumber
+
+    _get_uncle_count: Method[Callable[[BlockIdentifier], Awaitable[int]]] = Method(
+        method_choice_depends_on_args=select_method_for_block_identifier(
+            if_predefined=RPC.eth_getUncleCountByBlockNumber,
+            if_hash=RPC.eth_getUncleCountByBlockHash,
+            if_number=RPC.eth_getUncleCountByBlockNumber,
+        ),
+        mungers=[default_root_munger],
+    )
+
+    async def get_uncle_count(self, block_identifier: BlockIdentifier) -> int:
+        return await self._get_uncle_count(block_identifier)
+
     # eth_newFilter, eth_newBlockFilter, eth_newPendingTransactionFilter
 
     filter: Method[
         Callable[[Optional[Union[str, FilterParams, HexStr]]], Awaitable[AsyncFilter]]
     ] = Method(
         method_choice_depends_on_args=select_filter_method(
             if_new_block_filter=RPC.eth_newBlockFilter,
```

### Comparing `web3-6.1.0/web3/eth/base_eth.py` & `web3-6.2.0/web3/eth/base_eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/eth/eth.py` & `web3-6.2.0/web3/eth/eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/exceptions.py` & `web3-6.2.0/web3/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/gas_strategies/time_based.py` & `web3-6.2.0/web3/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/geth.py` & `web3-6.2.0/web3/geth.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/main.py` & `web3-6.2.0/web3/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/manager.py` & `web3-6.2.0/web3/manager.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/method.py` & `web3-6.2.0/web3/method.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/__init__.py` & `web3-6.2.0/web3/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/async_cache.py` & `web3-6.2.0/web3/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/attrdict.py` & `web3-6.2.0/web3/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/buffered_gas_estimate.py` & `web3-6.2.0/web3/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/cache.py` & `web3-6.2.0/web3/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/exception_handling.py` & `web3-6.2.0/web3/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/exception_retry_request.py` & `web3-6.2.0/web3/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/filter.py` & `web3-6.2.0/web3/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/fixture.py` & `web3-6.2.0/web3/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/formatting.py` & `web3-6.2.0/web3/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/gas_price_strategy.py` & `web3-6.2.0/web3/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/geth_poa.py` & `web3-6.2.0/web3/middleware/geth_poa.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/names.py` & `web3-6.2.0/web3/middleware/names.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/signing.py` & `web3-6.2.0/web3/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/simulate_unmined_transaction.py` & `web3-6.2.0/web3/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/stalecheck.py` & `web3-6.2.0/web3/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/middleware/validation.py` & `web3-6.2.0/web3/middleware/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/module.py` & `web3-6.2.0/web3/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/net.py` & `web3-6.2.0/web3/net.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/pm.py` & `web3-6.2.0/web3/pm.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/async_base.py` & `web3-6.2.0/web3/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/async_rpc.py` & `web3-6.2.0/web3/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/auto.py` & `web3-6.2.0/web3/providers/auto.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/base.py` & `web3-6.2.0/web3/providers/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/eth_tester/defaults.py` & `web3-6.2.0/web3/providers/eth_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/eth_tester/main.py` & `web3-6.2.0/web3/providers/eth_tester/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/eth_tester/middleware.py` & `web3-6.2.0/web3/providers/eth_tester/middleware.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/ipc.py` & `web3-6.2.0/web3/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/rpc.py` & `web3-6.2.0/web3/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/providers/websocket.py` & `web3-6.2.0/web3/providers/websocket.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/scripts/release/test_package.py` & `web3-6.2.0/web3/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/testing.py` & `web3-6.2.0/web3/testing.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/benchmark/main.py` & `web3-6.2.0/web3/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/benchmark/node.py` & `web3-6.2.0/web3/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/benchmark/reporting.py` & `web3-6.2.0/web3/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/benchmark/utils.py` & `web3-6.2.0/web3/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/pytest_ethereum/_utils.py` & `web3-6.2.0/web3/tools/pytest_ethereum/_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/pytest_ethereum/deployer.py` & `web3-6.2.0/web3/tools/pytest_ethereum/deployer.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/pytest_ethereum/linker.py` & `web3-6.2.0/web3/tools/pytest_ethereum/linker.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tools/pytest_ethereum/plugins.py` & `web3-6.2.0/web3/tools/pytest_ethereum/plugins.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/tracing.py` & `web3-6.2.0/web3/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 )
 from web3.module import (
     Module,
 )
 from web3.types import (
     BlockIdentifier,
     BlockTrace,
-    FilterParams,
     FilterTrace,
+    TraceFilterParams,
     TraceMode,
     TxParams,
     _Hash32,
 )
 
 
 class Tracing(Module):
@@ -69,15 +69,15 @@
     )
 
     trace_block: Method[Callable[[BlockIdentifier], List[BlockTrace]]] = Method(
         RPC.trace_block,
         mungers=[default_root_munger],
     )
 
-    trace_filter: Method[Callable[[FilterParams], List[FilterTrace]]] = Method(
+    trace_filter: Method[Callable[[TraceFilterParams], List[FilterTrace]]] = Method(
         RPC.trace_filter,
         mungers=[default_root_munger],
     )
 
     trace_transaction: Method[Callable[[_Hash32], List[FilterTrace]]] = Method(
         RPC.trace_transaction,
         mungers=[default_root_munger],
```

### Comparing `web3-6.1.0/web3/types.py` & `web3-6.2.0/web3/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,17 @@
     total=False,
 )
 
 
 CallOverride = Dict[ChecksumAddress, CallOverrideParams]
 
 
-GasPriceStrategy = Callable[["Web3", TxParams], Wei]
+GasPriceStrategy = Union[
+    Callable[["Web3", TxParams], Wei], Callable[["AsyncWeb3", TxParams], Wei]
+]
 
 
 # syntax b/c "from" keyword not allowed w/ class construction
 TxReceipt = TypedDict(
     "TxReceipt",
     {
         "blockHash": HexBytes,
```

### Comparing `web3-6.1.0/web3/utils/address.py` & `web3-6.2.0/web3/utils/address.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/utils/async_exception_handling.py` & `web3-6.2.0/web3/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/utils/caching.py` & `web3-6.2.0/web3/utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3/utils/exception_handling.py` & `web3-6.2.0/web3/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3.egg-info/PKG-INFO` & `web3-6.2.0/web3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.1.0
+Version: 6.2.0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.1.0/web3.egg-info/SOURCES.txt` & `web3-6.2.0/web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `web3-6.1.0/web3.egg-info/requires.txt` & `web3-6.2.0/web3.egg-info/requires.txt`

 * *Files identical despite different names*

