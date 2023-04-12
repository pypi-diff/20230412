# Comparing `tmp/smartredis-0.3.1.tar.gz` & `tmp/smartredis-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartredis-0.3.1.tar", last modified: Fri Jun 24 23:04:06 2022, max compression
+gzip compressed data, was "smartredis-0.4.0.tar", last modified: Wed Apr 12 19:48:02 2023, max compression
```

## Comparing `smartredis-0.3.1.tar` & `smartredis-0.4.0.tar`

### file list

```diff
@@ -1,157 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-06-24 23:03:48.000000 smartredis-0.3.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-06-24 23:03:48.000000 smartredis-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-24 23:03:48.000000 smartredis-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6545 2022-06-24 23:03:48.000000 smartredis-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2022-06-24 23:04:06.215478 smartredis-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-06-24 23:03:48.000000 smartredis-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.203478 smartredis-0.3.1/build-scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      389 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build-catch.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      600 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build-keydb.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      468 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build-lcov.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      583 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build-redis.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      984 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build-redisai-cpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2025 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build-redisai-gpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      349 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_c_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      869 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_cpp_cov.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      356 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_cpp_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      599 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_cpp_unit_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2052 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_deps.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      607 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_fortran_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1093 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_lib.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1006 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_parallel_examples.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1336 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_serial_examples.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1168 2022-06-24 23:03:48.000000 smartredis-0.3.1/build-scripts/build_test_deps.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.211478 smartredis-0.3.1/include/
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/addressallcommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/addressanycommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/addressatcommand.h
--rw-r--r--   0 runner    (1001) docker     (121)    79284 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/c_client.h
--rw-r--r--   0 runner    (1001) docker     (121)    10368 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/c_dataset.h
--rw-r--r--   0 runner    (1001) docker     (121)    82427 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/client.h
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/clusterinfocommand.h
--rw-r--r--   0 runner    (1001) docker     (121)    15327 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/command.h
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/command.tcc
--rw-r--r--   0 runner    (1001) docker     (121)     4950 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/commandlist.h
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/commandlist.tcc
--rw-r--r--   0 runner    (1001) docker     (121)    10633 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/commandreply.h
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/compoundcommand.h
--rw-r--r--   0 runner    (1001) docker     (121)    17938 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/dataset.h
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/dbinfocommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/dbnode.h
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/enum_fortran.inc
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/gettensorcommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/keyedcommand.h
--rw-r--r--   0 runner    (1001) docker     (121)    14758 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/metadata.h
--rw-r--r--   0 runner    (1001) docker     (121)    13043 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/metadatabuffer.h
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/metadatafield.h
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/multikeycommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/nonkeyedcommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     7211 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/pipelinereply.h
--rw-r--r--   0 runner    (1001) docker     (121)    45023 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/pyclient.h
--rw-r--r--   0 runner    (1001) docker     (121)     5089 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/pydataset.h
--rw-r--r--   0 runner    (1001) docker     (121)    22793 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/redis.h
--rw-r--r--   0 runner    (1001) docker     (121)    31467 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/rediscluster.h
--rw-r--r--   0 runner    (1001) docker     (121)    28299 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/redisserver.h
--rw-r--r--   0 runner    (1001) docker     (121)     5365 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/scalarfield.h
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/scalarfield.tcc
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/sharedmemorylist.h
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/sharedmemorylist.tcc
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/singlekeycommand.h
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/sr_enums.h
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/srassert.h
--rw-r--r--   0 runner    (1001) docker     (121)     9915 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/srexception.h
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/stringfield.h
--rw-r--r--   0 runner    (1001) docker     (121)    13028 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/tensor.h
--rw-r--r--   0 runner    (1001) docker     (121)    15124 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/tensor.tcc
--rw-r--r--   0 runner    (1001) docker     (121)     9746 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/tensorbase.h
--rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/tensorpack.h
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-06-24 23:03:48.000000 smartredis-0.3.1/include/threadpool.h
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-06-24 23:03:48.000000 smartredis-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-24 23:03:48.000000 smartredis-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-24 23:03:48.000000 smartredis-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-06-24 23:04:06.219478 smartredis-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-06-24 23:03:48.000000 smartredis-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.203478 smartredis-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.211478 smartredis-0.3.1/src/c/
--rw-r--r--   0 runner    (1001) docker     (121)    61531 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/c/c_client.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9967 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/c/c_dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/c/c_error.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.211478 smartredis-0.3.1/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/addressallcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/addressanycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/addressatcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    70355 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/client.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/clusterinfocommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10081 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/command.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/commandlist.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    14579 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/commandreply.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/compoundcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9762 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/dbinfocommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/dbnode.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/gettensorcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/keyedcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    20974 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/metadata.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/metadatafield.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/multikeycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/nonkeyedcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/pipelinereply.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    24198 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/redis.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    49248 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/rediscluster.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7251 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/redisserver.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/singlekeycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/stringfield.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6415 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/tensorbase.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/tensorpack.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/cpp/threadpool.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.211478 smartredis-0.3.1/src/fortran/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/src/fortran/client/
--rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/aggregation_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/client_dataset_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     6493 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/client_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/ensemble_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/misc_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)    21033 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/model_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/put_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/put_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (121)    13313 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/script_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/unpack_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client/unpack_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (121)    87099 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/client.F90
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/src/fortran/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/add_meta_scalar_common.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/add_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/add_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/dataset_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/get_meta_scalars_common.inc
--rw-r--r--   0 runner    (1001) docker     (121)     4227 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/metadata_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (121)    21576 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/dataset.F90
--rw-r--r--   0 runner    (1001) docker     (121)     4073 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/fortran/fortran_c_interop.F90
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.203478 smartredis-0.3.1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/src/python/bindings/
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/bindings/bind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.203478 smartredis-0.3.1/src/python/module/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/src/python/module/smartredis/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/module/smartredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    68217 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/module/smartredis/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5801 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/module/smartredis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/module/smartredis/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/module/smartredis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/src/python/module/smartredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2022-06-24 23:04:06.000000 smartredis-0.3.1/src/python/module/smartredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-06-24 23:04:06.000000 smartredis-0.3.1/src/python/module/smartredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 23:04:06.000000 smartredis-0.3.1/src/python/module/smartredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 23:04:06.000000 smartredis-0.3.1/src/python/module/smartredis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-24 23:04:06.000000 smartredis-0.3.1/src/python/module/smartredis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-24 23:04:06.000000 smartredis-0.3.1/src/python/module/smartredis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/src/python/src/
--rw-r--r--   0 runner    (1001) docker     (121)    42475 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/src/pyclient.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10332 2022-06-24 23:03:48.000000 smartredis-0.3.1/src/python/src/pydataset.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.203478 smartredis-0.3.1/utils/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 23:04:06.215478 smartredis-0.3.1/utils/create_cluster/
--rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-06-24 23:03:48.000000 smartredis-0.3.1/utils/create_cluster/local_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     5890 2022-06-24 23:03:48.000000 smartredis-0.3.1/utils/create_cluster/slurm_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    71347 2022-06-24 23:03:48.000000 smartredis-0.3.1/utils/create_cluster/smartredisdb.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-12 19:47:54.000000 smartredis-0.4.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 19:47:54.000000 smartredis-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 19:47:54.000000 smartredis-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-12 19:47:54.000000 smartredis-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-12 19:48:02.582703 smartredis-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-12 19:47:54.000000 smartredis-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.570703 smartredis-0.4.0/build-scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-catch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-keydb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-lcov.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      583 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-redis.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      984 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-redisai-cpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-redisai-gpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_c_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      548 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_cpp_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_cpp_unit_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_deps.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_fortran_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_lib.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_parallel_examples.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_serial_examples.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_test_deps.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.574703 smartredis-0.4.0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/address.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/addressallcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/addressanycommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/addressatcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80168 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_client.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_dataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_logcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    84208 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/client.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/clusterinfocommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/command.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/command.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/commandlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/commandlist.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/commandreply.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/compoundcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/dataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/dbinfocommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/dbnode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/enum_fortran.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/gettensorcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/keyedcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/logcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/metadatabuffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/metadatafield.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/multikeycommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/nonkeyedcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pipelinereply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46159 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pyclient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pydataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pylogcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pysrobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25115 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/redis.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/rediscluster.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30049 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/redisserver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/scalarfield.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/scalarfield.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/sharedmemorylist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/sharedmemorylist.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/singlekeycommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/sr_enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/srassert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/srexception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/srobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/stringfield.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensor.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensorbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensorpack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/utility.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 19:47:54.000000 smartredis-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-12 19:47:54.000000 smartredis-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 19:47:54.000000 smartredis-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-12 19:48:02.586703 smartredis-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-12 19:47:54.000000 smartredis-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.566703 smartredis-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.574703 smartredis-0.4.0/src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)    45629 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_error.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_logcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_logger.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.578703 smartredis-0.4.0/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/addressallcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/addressanycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/addressatcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    75366 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/clusterinfocommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/command.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/commandlist.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/commandreply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/compoundcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/dbinfocommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/dbnode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/gettensorcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/keyedcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/metadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/metadatafield.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/multikeycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/nonkeyedcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/pipelinereply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28292 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/redis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    51252 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/rediscluster.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/redisserver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/singlekeycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/srobject.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/stringfield.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/tensorbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/tensorpack.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/threadpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/utility.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.578703 smartredis-0.4.0/src/fortran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/aggregation_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/client_dataset_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/client_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/ensemble_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/misc_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/model_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/put_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/put_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/script_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/unpack_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/unpack_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    91170 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/add_meta_scalar_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/add_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/dataset_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/get_meta_scalars_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/metadata_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    26425 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/errors/errors_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/errors.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/fortran_c_interop.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/logcontext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logcontext/logcontext_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logcontext.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logger/logger_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logger.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.566703 smartredis-0.4.0/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/bindings/bind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.566703 smartredis-0.4.0/src/python/module/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/module/smartredis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69915 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/logcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/srobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/module/smartredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22479 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pyclient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pydataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pylogcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pysrobject.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      726 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/check_redis.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/utils/create_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/create_cluster/local_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/create_cluster/slurm_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71347 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/create_cluster/smartredisdb.conf
```

### Comparing `smartredis-0.3.1/LICENSE.md` & `smartredis-0.4.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2021-2022, Hewlett Packard Enterprise
+Copyright (c) 2021-2023, Hewlett Packard Enterprise
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/Makefile` & `smartredis-0.4.0/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 MAKEFLAGS += --no-print-directory
+COV_FLAGS :=
 
 # Do not remove this block. It is used by the 'help' rule when
 # constructing the help output.
 # help:
 # help: SmartRedis Makefile help
 # help:
 
@@ -18,26 +19,38 @@
 
 # help: deps                           - Make SmartRedis dependencies
 .PHONY: deps
 deps: SHELL:=/bin/bash
 deps:
 	@bash ./build-scripts/build_deps.sh
 
-# help: lib                            - Build SmartRedis clients into a dynamic library
+# help: lib                            - Build SmartRedis C/C++/Python clients into a dynamic library
 .PHONY: lib
 lib: SHELL:=/bin/bash
 lib: deps
 	@bash ./build-scripts/build_lib.sh $(LIB_BUILD_ARGS)
 
+# help: lib-with-fortran               - Build SmartRedis C/C++/Python and Fortran clients into a dynamic library
+.PHONY: lib-with-fortran
+lib-with-fortran: SHELL:=/bin/bash
+lib-with-fortran: deps
+	@bash ./build-scripts/build_lib.sh $(LIB_BUILD_ARGS) $(CMAKE_ARGS) -DBUILD_FORTRAN=ON
+
 # help: test-lib                       - Build SmartRedis clients into a dynamic library with least permissive compiler settings
 .PHONY: test-lib
 test-lib: SHELL:=/bin/bash
 test-lib: LIB_BUILD_ARGS="-DWERROR=ON"
 test-lib: lib
 
+# help: test-lib-with-fortran          - Build SmartRedis clients into a dynamic library with least permissive compiler settings
+.PHONY: test-lib-with-fortran
+test-lib-with-fortran: SHELL:=/bin/bash
+test-lib-with-fortran: LIB_BUILD_ARGS="-DWERROR=ON"
+test-lib-with-fortran: lib-with-fortran
+
 # help: test-deps                      - Make SmartRedis testing dependencies
 .PHONY: test-deps
 test-deps: SHELL:=/bin/bash
 test-deps:
 	@bash ./build-scripts/build_test_deps.sh
 
 # help: test-deps-gpu                  - Make SmartRedis GPU testing dependencies
@@ -45,19 +58,19 @@
 test-deps-gpu: SHELL:=/bin/bash
 test-deps-gpu:
 	@bash ./build-scripts/build_test_deps.sh gpu
 
 
 # help: build-tests                    - build all tests (C, C++, Fortran)
 .PHONY: build-tests
-build-tests: test-lib
-	./build-scripts/build_cpp_tests.sh
-	./build-scripts/build_cpp_unit_tests.sh
-	./build-scripts/build_c_tests.sh
-	./build-scripts/build_fortran_tests.sh
+build-tests: test-lib-with-fortran
+	./build-scripts/build_cpp_tests.sh $(CMAKE_ARGS)
+	./build-scripts/build_cpp_unit_tests.sh $(CMAKE_ARGS)
+	./build-scripts/build_c_tests.sh $(CMAKE_ARGS)
+	./build-scripts/build_fortran_tests.sh $(CMAKE_ARGS)
 
 
 # help: build-test-cpp                 - build the C++ tests
 .PHONY: build-test-cpp
 build-test-cpp: test-lib
 	./build-scripts/build_cpp_tests.sh
 	./build-scripts/build_cpp_unit_tests.sh
@@ -71,21 +84,21 @@
 .PHONY: build-test-c
 build-test-c: test-lib
 	./build-scripts/build_c_tests.sh
 
 
 # help: build-test-fortran             - build the Fortran tests
 .PHONY: build-test-fortran
-build-test-fortran: test-lib
+build-test-fortran: test-lib-with-fortran
 	./build-scripts/build_fortran_tests.sh
 
 
 # help: build-examples                 - build all examples (serial, parallel)
 .PHONY: build-examples
-build-examples: lib
+build-examples: lib-with-fortran
 	./build-scripts/build_serial_examples.sh
 	./build-scripts/build_parallel_examples.sh
 
 # help: build-example-serial           - buld serial examples
 .PHONY: build-example-serial
 build-example-serial: lib
 	./build-scripts/build_serial_examples.sh
@@ -184,15 +197,22 @@
 	@PYTHONFAULTHANDLER=1 python -m pytest --ignore ./tests/docker -vv ./tests
 
 
 # help: test-verbose                   - Build and run all tests [verbosely]
 .PHONY: test-verbose
 test-verbose: build-tests
 test-verbose:
-	@PYTHONFAULTHANDLER=1 python -m pytest --ignore ./tests/docker -vv -s ./tests
+	PYTHONFAULTHANDLER=1 python -m pytest $(COV_FLAGS) --ignore ./tests/docker -vv -s ./tests
+
+# help: test-verbose-with-coverage                   - Build and run all tests [verbose-with-coverage]
+.PHONY: test-verbose-with-coverage
+test-verbose-with-coverage: build-tests
+test-verbose-with-coverage: CMAKE_ARGS="-DCOVERAGE=on"
+test-verbose-with-coverage:
+	PYTHONFAULTHANDLER=1 python -m pytest $(COV_FLAGS) --ignore ./tests/docker -vv -s ./tests
 
 # help: test-c                         - Build and run all C tests
 .PHONY: test-c
 test-c: build-test-c
 test-c:
 	@python -m pytest -vv -s ./tests/c/
 
@@ -220,18 +240,13 @@
 	@python -m pytest -vv ./tests/fortran/
 
 # help: testpy-cov                     - run python tests with coverage
 .PHONY: testpy-cov
 testpy-cov:
 	@PYTHONFAULTHANDLER=1 python -m pytest --cov=./src/python/module/smartredis/ -vv ./tests/python/
 
-# help: testcpp-cov                    - run cpp unit tests with coverage
-.PHONY: testcpp-cov
-testcpp-cov: unit-test-cpp
-	./build-scripts/build_cpp_cov.sh
-
 # help: test-examples                   - Build and run all examples
 .PHONY: test-examples
 test-examples: build-examples
 test-examples:
 	@python -m pytest -vv -s ./examples
```

### Comparing `smartredis-0.3.1/PKG-INFO` & `smartredis-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartredis
-Version: 0.3.1
+Version: 0.4.0
 Summary: RedisAI clients for SmartSim
 Home-page: https://github.com/CrayLabs/SmartRedis
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartRedis
 Project-URL: Documentation, https://www.craylabs.org
@@ -106,11 +106,12 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: xarray
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartredis Version: 0.3.1 Summary: RedisAI clients
+Metadata-Version: 2.1 Name: smartredis Version: 0.4.0 Summary: RedisAI clients
 for SmartSim Home-page: https://github.com/CrayLabs/SmartRedis Author:
 CrayLabs, a Hewlett Packard Enterprise OSS Organization Author-email:
 craylabs@hpe.com License: BSD 2-Clause License Project-URL: Source, https://
 github.com/CrayLabs/SmartRedis Project-URL: Documentation, https://
 www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
@@ -54,9 +54,9 @@
 Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins}, year=
 {2021}, eprint={2104.09355}, archivePrefix={arXiv}, primaryClass={cs.CE} } ```
 Keywords: redis,clients,hpc,ai,deep learning Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: BSD License Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
-Extra: doc
+<3.11,>=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
+Provides-Extra: doc Provides-Extra: xarray
```

### Comparing `smartredis-0.3.1/README.md` & `smartredis-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build-keydb.sh` & `smartredis-0.4.0/build-scripts/build-keydb.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build-redis.sh` & `smartredis-0.4.0/build-scripts/build-redis.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build-redisai-cpu.sh` & `smartredis-0.4.0/build-scripts/build-redisai-cpu.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build-redisai-gpu.sh` & `smartredis-0.4.0/build-scripts/build-redisai-gpu.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build_cpp_unit_tests.sh` & `smartredis-0.4.0/build-scripts/build_cpp_unit_tests.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/bin/bash
 
+# Any command line arguments are assumed to be CMake arguments
+CMAKE_ARGS=$@
+
 # get the number of processors
 NPROC=$(python -c "import multiprocessing as mp; print(mp.cpu_count())")
 
 CMAKE=$(which cmake)
 
 BASEDIR=$(pwd)
 
 cd ./tests/cpp/unit-tests
-
 if [[ -d "./build" ]]; then
     echo "Removing previous cpp unit test build directory"
     rm -rf ./build
 fi
 
 # setup build dirs
 mkdir build
 cd ./build
 
 # TODO add platform dependent build step here
-$CMAKE ..
+$CMAKE .. $CMAKE_ARGS
 
 if [ $? != 0 ]; then
     echo "ERROR: cmake for CPP tests failed"
     cd ..
     exit 1
 fi
```

### Comparing `smartredis-0.3.1/build-scripts/build_deps.sh` & `smartredis-0.4.0/build-scripts/build_deps.sh`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 #Install Redis-plus-plus
 if ls ../install/lib/libredis++.a 1>/dev/null 2>&1; then
     echo "Redis-plus-plus has already been installed"
 else
     if [[ ! -d "./redis-plus-plus" ]]; then
-        git clone https://github.com/sewenew/redis-plus-plus.git redis-plus-plus --branch 1.3.2 --depth=1
+        git clone https://github.com/sewenew/redis-plus-plus.git redis-plus-plus --branch 1.3.5 --depth=1
 	    echo "Redis-plus-plus downloaded"
     fi
     cd redis-plus-plus
     #ex -s -c '2i|SET_PROPERTY(GLOBAL PROPERTY TARGET_SUPPORTS_SHARED_LIBS TRUE)' -c x CMakeLists.txt
     mkdir compile
     cd compile
 
@@ -55,15 +55,15 @@
     echo "Finished installing Redis-plus-plus"
 fi
 
 # Install Pybind11
 if [[ -d "./pybind" ]]; then
     echo "PyBind11 has already been downloaded and installed"
 else
-    git clone https://github.com/pybind/pybind11.git pybind --branch v2.6.2 --depth=1
+    git clone https://github.com/pybind/pybind11.git pybind --branch v2.10.3 --depth=1
     cd pybind
     mkdir build
     cd ..
     echo "PyBind11 downloaded"
 fi
```

### Comparing `smartredis-0.3.1/build-scripts/build_fortran_tests.sh` & `smartredis-0.4.0/build-scripts/build_fortran_tests.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #!/bin/bash
 
 CMAKE=$(which cmake)
 
+# Any command line arguments are assumed to be CMake arguments
+CMAKE_ARGS=$@
+
 cd ./tests/fortran/
 
 # setup build dirs
+if [[ -d "./build" ]]; then
+    echo "Removing previous cpp unit test build directory"
+    rm -rf ./build
+fi
 mkdir build
 cd ./build
 
 DO_FORTRAN="yes"
 
 if [ "$(uname)" == "Darwin" ]; then
     DO_FORTRAN="yes"
 fi
 
 if [[ $DO_FORTRAN == "yes" ]]; then
     # TODO add platform dependent build step here
-    $CMAKE ..
+    $CMAKE .. $CMAKE_ARGS
 
     if [ $? != 0 ]; then
         echo "ERROR: cmake for Fortran tests failed"
         cd ..
         exit 1
     fi
```

### Comparing `smartredis-0.3.1/build-scripts/build_lib.sh` & `smartredis-0.4.0/build-scripts/build_lib.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build_parallel_examples.sh` & `smartredis-0.4.0/build-scripts/build_parallel_examples.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build_serial_examples.sh` & `smartredis-0.4.0/build-scripts/build_serial_examples.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/build-scripts/build_test_deps.sh` & `smartredis-0.4.0/build-scripts/build_test_deps.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.3.1/include/addressallcommand.h` & `smartredis-0.4.0/include/addressallcommand.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -71,10 +71,10 @@
         *  \brief Field index for a key to prefixed for each target
         *         execution environment (-1 if none)
         */
         int key_index;
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_ADDRRESSALLCOMMAND_H
+#endif // SMARTREDIS_ADDRRESSALLCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/addressanycommand.h` & `smartredis-0.4.0/include/addressanycommand.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -64,10 +64,10 @@
         *   \returns A pointer to dynamically allocated
         *            derived type cast to parent Command
         *            type.
         */
         virtual Command* clone();
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //ADDRESSANYCOMMAND
+#endif // SMARTREDIS_ADDRESSANYCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/addressatcommand.h` & `smartredis-0.4.0/include/addressatcommand.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -130,10 +130,10 @@
                 throw SRRuntimeException(oor.what());
             }
             return port;
         }
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //ADDRESSATCOMMAND
+#endif // SMARTREDIS_ADDRESSATCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/c_client.h` & `smartredis-0.4.0/include/c_client.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -24,60 +24,68 @@
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_C_CLIENT_H
 #define SMARTREDIS_C_CLIENT_H
-///@file
-///\brief C-wrappers for the C++ Client class
+
 #include <stdlib.h>
 #include <stdbool.h>
 #include "client.h"
 #include "sr_enums.h"
 #include "srexception.h"
 
+///@file
+///\brief C-wrappers for the C++ Client class
+
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /*!
 *   \brief C-client constructor
 *   \param cluster Flag to indicate if a database cluster is being used
+*   \param logger_name Identifier for the current client
+*   \param logger_name_length Length in characters of the logger_name string
 *   \param new_client Receives the new client
 *   \return Returns SRNoError on success or an error code on failure
 */
-SRError SmartRedisCClient(bool cluster, void **new_client);
+SRError SmartRedisCClient(
+    bool cluster,
+    const char* logger_name,
+    const size_t logger_name_length,
+    void **new_client);
 
 /*!
 *   \brief C-client destructor
 *   \param c_client A pointer to a pointer to the c-client to destroy.
 *                   The client is set to NULL on completion
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError DeleteCClient(void** c_client);
 
 /*!
 *   \brief Put a DataSet object into the database
 *   \details The final dataset key under which the dataset is stored
 *            is generated from the name that was supplied when the
 *            dataset was created and may be prefixed. See
-*            use_tensor_ensemble_prefix() for more details.
+*            use_dataset_ensemble_prefix() for more details.
 *   \param c_client The client object to use for communication
 *   \param dataset The DataSet object to send
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError put_dataset(void* c_client, void* dataset);
 
 /*!
 *   \brief Get a DataSet object from the database
 *   \details The final dataset key used to locate the dataset
 *            may be formed by applying a prefix to the supplied
 *            name. See set_data_source() and
-*            use_tensor_ensemble_prefix() for more details.
+*            use_dataset_ensemble_prefix() for more details.
 *   \param c_client The client object to use for communication
 *   \param name The name of the dataset object to fetch
 *   \param name_length The length of the name string,
 *                      excluding null terminating character
 *   \param dataset Receives the DataSet
 *   \return Returns SRNoError on success or an error code on failure
 */
@@ -87,15 +95,15 @@
                     void** dataset);
 
 /*!
 *   \brief Move a DataSet to a new name
 *   \details The old and new dataset keys used to
 *            find and relocate the dataset may be formed by applying
 *            prefixes to the supplied old_name and new_name.
-*            See set_data_source() and use_tensor_ensemble_prefix()
+*            See set_data_source() and use_dataset_ensemble_prefix()
 *            for more details.
 *   \param c_client The client object to use for communication
 *   \param old_name The current name key of the dataset object
 *   \param old_name_length The length of the current name string,
 *                          excluding null terminating character
 *   \param new_name The new name key for the dataset object
 *   \param new_name_length The length of the new name string,
@@ -109,15 +117,15 @@
                        const size_t new_name_length);
 
 /*!
 *   \brief Copy a DataSet to a new name
 *   \details The source and destination dataset keys used to
 *            locate and store the dataset may be formed by applying
 *            prefixes to the supplied src_name and dest_name.
-*            See set_data_source() and use_tensor_ensemble_prefix()
+*            See set_data_source() and use_dataset_ensemble_prefix()
 *            for more details.
 *   \param c_client The client object to use for communication
 *   \param src_name The source name of the dataset object
 *   \param src_name_length The length of the src_name string,
 *                          excluding null terminating character
 *   \param dest_name The destination name for the dataset object
 *   \param dest_name_length The length of the dest_name string,
@@ -131,15 +139,15 @@
                      const size_t dest_name_length);
 
 /*!
 *   \brief Delete a DataSet
 *   \details The dataset key used to locate the dataset to be deleted
 *            may be formed by applying a prefix to the supplied
 *            name. See set_data_source()
-*            and use_tensor_ensemble_prefix() for more details.
+*            and use_dataset_ensemble_prefix() for more details.
 *   \param c_client The client object to use for communication
 *   \param name The name of the dataset object
 *   \param name_length The length of the name string,
 *                      excluding null terminating character
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError delete_dataset(void* c_client,
@@ -506,15 +514,15 @@
                   const size_t tag_length,
                   const char** inputs,
                   const size_t* input_lengths,
                   const size_t n_inputs,
                   const char** outputs,
                   const size_t* output_lengths,
                   const size_t n_outputs);
- 
+
  /*!
 *   \brief Set a model (from buffer) in the database for future execution
 *          in a multi-GPU system
 *   \details The final model key used to store the model
 *            may be formed by applying a prefix to the supplied
 *            name. Similarly, the tensor names in the
 *            input and output nodes for TF models may be prefixed.
@@ -623,20 +631,14 @@
 *   \details The final script key used to store the script
 *            may be formed by applying a prefix to the supplied
 *            name. See use_model_ensemble_prefix() for more details
 *   \param c_client The client object to use for communication
 *   \param name The name to associate with the script
 *   \param name_length The length of the name string,
 *                      excluding null terminating character
-*   \param device The name of the device for execution. May be either
-*                 CPU or GPU. If multiple GPUs are present, a specific
-*                 GPU can be targeted by appending its zero-based
-*                 index, i.e. "GPU:1"
-*   \param device_length The length of the device name string,
-*                        excluding null terminating character
 *   \param script_file The source file for the script
 *   \param script_file_length The length of the script file name string,
 *                             excluding null terminating character
 *   \param first_gpu the first gpu (zero-based) to use with the model
 *   \param num_gpus the number of gpus to use with the model
 *   \return Returns SRNoError on success or an error code on failure
 */
@@ -736,15 +738,14 @@
 *                        excluding null terminating character
 *   \param n_inputs The number of inputs
 *   \param outputs The tensor keys of output tensors that will be used
 *                  to save script results
 *   \param output_lengths The length of each output name string,
 *                         excluding null terminating character
 *   \param n_outputs The number of outputs
-*   \return Returns SRNoError on success or an error code on failure
 */
 void _check_params_run_script(void* c_client,
                               const char* name,
                               const char* function,
                               const char** inputs,
                               const size_t* input_lengths,
                               const size_t n_inputs,
@@ -987,15 +988,15 @@
 *            name. See set_data_source() and use_model_ensemble_prefix()
 *            for more details.
 *            The first_gpu and num_gpus parameters must match those used
 *            when the model was stored.
 *   \param c_client The client object to use for communication
 *   \param name The name associated with the model
 *   \param name_length The length of the name string,
-*   \param first_cpu the first GPU (zero-based) to use with the model
+*   \param first_gpu the first GPU (zero-based) to use with the model
 *   \param num_gpus the number of gpus for which the model was stored
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError delete_model_multigpu(void* c_client,
                               const char* name,
                               const size_t name_length,
                               const int first_gpu,
@@ -1020,15 +1021,15 @@
 *            name. See set_data_source() and use_model_ensemble_prefix()
 *            for more details.
 *            The first_gpu and num_gpus parameters must match those used
 *            when the script was stored.
 *   \param c_client The client object to use for communication
 *   \param name The name associated with the model
 *   \param name_length The length of the name string,
-*   \param first_cpu the first GPU (zero-based) to use with the model
+*   \param first_gpu the first GPU (zero-based) to use with the model
 *   \param num_gpus the number of gpus for which the model was stored
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError delete_script_multigpu(void* c_client,
                             const char* name,
                             const size_t name_length,
                             const int first_gpu,
@@ -1092,15 +1093,15 @@
                      bool* exists);
 
 /*!
 *   \brief Check if a dataset exists in the database
 *   \details The dataset key used to check for dataset existence
 *            may be formed by applying a prefix to the supplied
 *            name. See set_data_source()
-*            and use_tensor_ensemble_prefix() for more details.
+*            and use_dataset_ensemble_prefix() for more details.
 *   \param c_client The client object to use for communication
 *   \param name The name of the dataset that will be checked in the database.
 *               The full key corresponding to \p name will be formed
 *               in accordance with the current prefixing behavior
 *   \param name_length The length of the name string,
 *                      excluding null terminating character
 *   \param exists Receives whether the dataset exists
@@ -1188,15 +1189,15 @@
 
 /*!
 *   \brief Check if a dataset exists in the database, repeating the check
 *          at a specified frequency and number of repetitions
 *   \details The dataset key used to check for dataset existence
 *            may be formed by applying a prefix to the supplied
 *            name. See set_data_source()
-*            and use_tensor_ensemble_prefix() for more details.
+*            and use_dataset_ensemble_prefix() for more details.
 *   \param c_client The client object to use for communication
 *   \param name The name of the entity to be checked in the database.
 *               The full key associated to \p name will be formed according
 *               to the prefixing behavior
 *   \param name_length The length of the name string,
 *                      excluding null terminating character
 *   \param poll_frequency_ms The time delay between checks, in milliseconds
@@ -1237,35 +1238,56 @@
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError set_data_source(void* c_client,
                         const char* source_id,
                         const size_t source_id_length);
 
 /*!
-*   \brief Control whether tensor and dataset names are
-*          prefixed (e.g. in an ensemble) when forming database keys
+*   \brief Control whether tensor names are prefixed (e.g. in an
+*          ensemble) when forming database keys
 *   \details This function can be used to avoid key collisions in an
 *            ensemble by prepending the string value from the
-*            environment variable SSKEYIN to tensor and dataset names.
+*            environment variable SSKEYIN to tensor names.
 *            Prefixes will only be used if they were previously set through
 *            Keys for entities created before this function is called
 *            the environment variables SSKEYOUT and SSKEYIN.
 *            will not be retroactively prefixed.
-*            By default, the client prefixes tensor and dataset keys
+*            By default, the client prefixes tensor keys
 *            with the first prefix specified with the SSKEYIN
 *            and SSKEYOUT environment variables.
 *
 *   \param c_client The client object to use for communication
 *   \param use_prefix If true, all future operations on tensors and
 *                     datasets will use a prefix, if available.
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError use_tensor_ensemble_prefix(void* c_client, bool use_prefix);
 
 /*!
+*   \brief Control whether dataset names are prefixed (e.g. in an
+*          ensemble) when forming database keys
+*   \details This function can be used to avoid key collisions in an
+*            ensemble by prepending the string value from the
+*            environment variable SSKEYIN to tensor and dataset names.
+*            Prefixes will only be used if they were previously set through
+*            Keys for entities created before this function is called
+*            the environment variables SSKEYOUT and SSKEYIN.
+*            will not be retroactively prefixed.
+*            By default, the client prefixes dataset keys
+*            with the first prefix specified with the SSKEYIN
+*            and SSKEYOUT environment variables.
+*
+*   \param c_client The client object to use for communication
+*   \param use_prefix If true, all future operations on tensors and
+*                     datasets will use a prefix, if available.
+*   \return Returns SRNoError on success or an error code on failure
+*/
+SRError use_dataset_ensemble_prefix(void* c_client, bool use_prefix);
+
+/*!
 *   \brief Control whether model and script names are
 *          prefixed (e.g. in an ensemble) when forming database keys
 *   \details This function can be used to avoid key collisions in an
 *            ensemble by prepending the string value from the
 *            environment variable SSKEYIN to model and script names.
 *            Prefixes will only be used if they were previously set through
 *            Keys for entities created before this function is called
@@ -1289,17 +1311,17 @@
 *            aggregation list names.  Prefixes will only be used if
 *            they were previously set through the environment variables
 *            SSKEYOUT and SSKEYIN. Keys for aggregation lists created
 *            before this function is called will not be retroactively
 *            prefixed. By default, the client prefixes aggregation
 *            list keys with the first prefix specified with the SSKEYIN
 *            and SSKEYOUT environment variables.  Note that
-*            use_tensor_ensemble_prefix() controls prefixing
+*            use_dataset_ensemble_prefix() controls prefixing
 *            for the entities in the aggregation list, and
-*            use_tensor_ensemble_prefix() should be given the
+*            use_dataset_ensemble_prefix() should be given the
 *            same value that was used during the initial
 *            setting of the DataSet into the database.
 *   \param c_client The client object to use for communication
 *   \param use_prefix If set to true, all future operations
 *                    on aggregation lists will use
 *                    a prefix, if available.
 *   \return Returns SRNoError on success or an error code on failure
@@ -1360,25 +1382,25 @@
 */
 SRError copy_list(void* c_client,
                   const char* src_name, const size_t src_name_length,
                   const char* dest_name, const size_t dest_name_length);
 
 /*!
 *   \brief Rename an aggregation list
-*   \details The old and new aggregation list key used to find and
+*   \details The initial and target aggregation list key used to find and
 *            relocate the list may be formed by applying prefixes to
-*            the supplied old_name and new_name. See set_data_source()
+*            the supplied src_name and dest_name. See set_data_source()
 *            and use_list_ensemble_prefix() for more details.
 *   \param c_client The client object to use for communication
-*   \param old_name The old list name
-*   \param src_name_length The size in characters of the old list name,
-*                          including null terminator
-*   \param new_name The new list name
-*   \param new_name_length The size in characters of the new list name,
+*   \param src_name The initial list name
+*   \param src_name_length The size in characters of the initial list name,
 *                          including null terminator
+*   \param dest_name The target list name
+*   \param dest_name_length The size in characters of the target list name,
+*                           including null terminator
 *   \return Returns SRNoError on success or an error code on failure
 */
 SRError rename_list(void* c_client,
                     const char* src_name, const size_t src_name_length,
                     const char* dest_name, const size_t dest_name_length);
 
 /*!
@@ -1514,19 +1536,24 @@
 *                    supported.  A negative value indicates offsets
 *                    starting at the end of the list. For example, -1 is
 *                    the last element of the list.
 *   \param datasets Receives an array of datasets included in the list
 *   \param num_datasets Receives the number of datasets returned
 *   \return Returns SRNoError on success or an error code on failure
 */
-SRError get_dataset_list_range(void* c_client, const char* list_name,
-                               const size_t list_name_length,
-                               const int start_index, const int end_index,
-                               void*** datasets, size_t* num_datasets);
-/*
+SRError get_dataset_list_range(
+    void* c_client,
+    const char* list_name,
+    const size_t list_name_length,
+    const int start_index,
+    const int end_index,
+    void*** datasets,
+    size_t* num_datasets);
+
+/*!
 *   \brief Get a range of datasets (by index) from an aggregation list and
            copy them into an already allocated vector of datasets. Note,
            while this method could be used by C clients, its primary
            use case is for the Fortran client.
 *   \details The aggregation list key used to retrieve datasets
 *            may be formed by applying a prefix to the supplied
 *            name. See set_data_source()  and use_list_ensemble_prefix()
@@ -1547,20 +1574,30 @@
 *                      the last element of the list.
 *   \param end_index The ending index of the range (inclusive,
 *                    starting at zero).  Negative values are
 *                    supported.  A negative value indicates offsets
 *                    starting at the end of the list. For example, -1 is
 *                    the last element of the list.
 *   \param datasets Receives an array of datasets included in the list
-*   \param num_datasets Receives the number of datasets returned
 *   \return Returns SRNoError on success or an error code on failure
 */
-SRError _get_dataset_list_range_allocated(void* c_client, const char* list_name,
-                                         const size_t list_name_length,
-                                         const int start_index, const int end_index,
-                                         void** datasets);
+SRError _get_dataset_list_range_allocated(
+    void* c_client,
+    const char* list_name,
+    const size_t list_name_length,
+    const int start_index,
+    const int end_index,
+    void** datasets);
+
+
+/*!
+*   \brief Retrieve a string representation of the client
+*   \param c_client The client object to use for communication
+*   \return A string with either the client representation or an error message
+*/
+const char* client_to_string(void* c_client);
 
 #ifdef __cplusplus
 }
 
 #endif
 #endif // SMARTREDIS_C_CLIENT_H
```

### Comparing `smartredis-0.3.1/include/c_dataset.h` & `smartredis-0.4.0/include/c_dataset.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,20 +25,22 @@
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_C_DATASET_H
 #define SMARTREDIS_C_DATASET_H
-///@file
-///\brief C-wrappers for the C++ DataSet class
+
 #include "dataset.h"
 #include "sr_enums.h"
 #include "srexception.h"
 
+///@file
+///\brief C-wrappers for the C++ DataSet class
+
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /*!
 *   \brief C-DataSet constructor
 *   \param name The name of the dataset
@@ -218,11 +220,83 @@
 SRError get_meta_strings(void* dataset,
                          const char* name,
                          const size_t name_length,
                          char*** data,
                          size_t* n_strings,
                          size_t** lengths);
 
+/*!
+*   \brief Retrieve the names of tensors in the DataSet
+*   \param dataset The dataset to use for this operation
+*   \param data Receives an array of tensor names
+*   \param n_strings Receives the number of strings returned in \p data
+*   \param lengths Receives an array containing the lengths of the strings
+*                  returned in \p data
+*   \return Returns SRNoError on success or an error code on failure
+*/
+SRError get_tensor_names(
+    void* dataset, char*** data, size_t* n_strings, size_t** lengths);
+
+/*!
+*   \brief Retrieve the data type of a Tensor in the DataSet
+*   \param dataset The dataset to use for this operation
+*   \param name The name of the tensor (null-terminated string)
+*   \param name_len The length in bytes of the tensor name
+*   \param ttype Receives the type for the specified tensor
+*   \return Returns SRNoError on success or an error code on failure
+*/
+SRError get_tensor_type(
+    void* dataset, const char* name, size_t name_len, SRTensorType* ttype);
+
+/*!
+*   \brief Retrieve the dimensions of a Tensor in the DataSet
+*   \param dataset The dataset to use for this operation
+*   \param name The name of the tensor (null-terminated string)
+*   \param name_len The length in bytes of the tensor name
+*   \param dims A buffer in which to receive the dimensions for
+*               the specified tensor.
+*   \param ndims The size of the buffer supplied in \p dims when this function
+*                is called; receives the number of dimensions supplied on exit.
+*                If the supplied the buffer isn't large enough to contain all
+*                the tensor dimensions, \p ndims will still receive the needed
+*                size.
+*   \return Returns SRNoError on success or an error code on failure. If the
+*           buffer supplied in \p dims is too small, returns SRBadAllocError.
+*/
+SRError get_tensor_dims(
+    void* dataset, const char* name, size_t name_len,
+    size_t** dims, size_t *ndims);
+
+/*!
+*   \brief Retrieve the names of all metadata fields in the DataSet
+*   \param dataset The dataset to use for this operation
+*   \param data Receives an array of metadata field names
+*   \param n_strings Receives the number of strings returned in \p data
+*   \param lengths Receives an array containing the lengths of the strings
+*                  returned in \p data
+*   \return Returns SRNoError on success or an error code on failure
+*/
+SRError get_metadata_field_names(
+    void* dataset, char*** data, size_t* n_strings, size_t** lengths);
+
+/*!
+*   \brief Retrieve the data type of a metadata field in the DataSet
+*   \param dataset The dataset to use for this operation
+*   \param name The name of the metadata field (null-terminated string)
+*   \param name_len The length in bytes of the metadata field name
+*   \param mdtype Receives the type for the specified metadata field
+*   \return Returns SRNoError on success or an error code on failure
+*/
+ SRError get_metadata_field_type(
+    void* dataset, const char* name, size_t name_len, SRMetaDataType* mdtype);
+
+/*!
+*   \brief Retrieve a string representation of the dataset
+*   \param dataset The dataset to use for this operation
+*   \return A string with either the client representation or an error message
+*/
+const char* dataset_to_string(void* dataset);
+
 #ifdef __cplusplus
 }
 #endif
-#endif //SMARTREDIS_C_DATASET_H
+#endif // SMARTREDIS_C_DATASET_H
```

### Comparing `smartredis-0.3.1/include/client.h` & `smartredis-0.4.0/include/client.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,65 +22,67 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef SMARTREDIS_CPP_CLIENT_H
-#define SMARTREDIS_CPP_CLIENT_H
+#ifndef SMARTREDIS_CLIENT_H
+#define SMARTREDIS_CLIENT_H
+
 #ifdef __cplusplus
-#include "string.h"
-#include "stdlib.h"
+#include <string.h>
+#include <stdlib.h>
 #include <iostream>
 #include <fstream>
 #include <vector>
 #include <chrono>
 #include <thread>
 #include <algorithm>
+#include "srobject.h"
 #include "redisserver.h"
 #include "rediscluster.h"
 #include "redis.h"
 #include "dataset.h"
 #include "sharedmemorylist.h"
 #include "command.h"
 #include "commandlist.h"
 #include "commandreply.h"
 #include "tensorbase.h"
 #include "tensor.h"
 #include "sr_enums.h"
+#include "logger.h"
 
 ///@file
 
 namespace SmartRedis {
 
-class Client;
-
 /*!
 *  \brief The database response to a command
 */
 typedef redisReply ReplyElem;
 
 ///@file
 /*!
 *   \brief The Client class is the primary user-facing
 *          class for executing server commands.
 */
-class Client
+class Client : public SRObject
 {
 
     public:
 
         /*!
         *   \brief Client constructor
         *   \param cluster Flag for if a database cluster is being used
+        *   \param logger_name Name to use for this client when logging
         *   \throw SmartRedis::Exception if client connection or
         *          object initialization fails
         */
-        Client(bool cluster);
+        Client(bool cluster, const std::string& logger_name = "default");
 
         /*!
         *   \brief Client copy constructor is not available
         */
         Client(const Client& client) = delete;
 
         /*!
@@ -98,60 +100,60 @@
         *   \brief Client move assignment operator
         */
         Client& operator=(Client&& client) = default;
 
         /*!
         *   \brief Client destructor
         */
-        ~Client();
+        virtual ~Client();
 
         /*!
         *   \brief Send a DataSet object to the database
         *   \details The final dataset key under which the dataset is stored
         *            is generated from the name that was supplied when the
         *            dataset was created and may be prefixed. See
-        *            use_tensor_ensemble_prefix() for more details.
+        *            use_dataset_ensemble_prefix() for more details.
         *   \param dataset The DataSet object to send to the database
         *   \throw SmartRedis::Exception if put dataset command fails
         */
         void put_dataset(DataSet& dataset);
 
         /*!
         *   \brief Get a DataSet object from the database
         *   \details The dataset key used to locate the dataset
         *            may be formed by applying a prefix to the supplied
         *            name. See set_data_source()
-        *            and use_tensor_ensemble_prefix() for more details.
+        *            and use_dataset_ensemble_prefix() for more details.
         *   \param name The name of the dataset to retrieve
         *   \returns DataSet object retrieved from the database
         *   \throw SmartRedis::Exception if get dataset command fails
         */
         DataSet get_dataset(const std::string& name);
 
         /*!
         *   \brief Move a dataset to a new name.  All tensors
         *          and metdata in the dataset will be moved with it.
         *   \details The old and new dataset keys used to find and relocate
         *            the dataset may be formed by applying prefixes to the
         *            supplied old_name and new_name. See set_data_source()
-        *            and use_tensor_ensemble_prefix() for more details.
+        *            and use_dataset_ensemble_prefix() for more details.
         *   \param old_name The original dataset key for the dataset
         *   \param new_name The new dataset key for the dataset
         *   \throw SmartRedis::Exception if dataset rename command fails
         */
         void rename_dataset(const std::string& old_name,
                             const std::string& new_name);
 
         /*!
         *   \brief Copy a dataset to a new name. All tensors and metadata
         *          in the DataSet will be copied as well.
         *   \details The source and destination dataset keys used to
         *            locate and store the dataset may be formed by
         *            applying prefix to the supplied src_name and dest_name.
-        *            See set_data_source() and use_tensor_ensemble_prefix()
+        *            See set_data_source() and use_dataset_ensemble_prefix()
         *            for more details.
         *   \param src_name The source dataset key
         *   \param dest_name The destination dataset key
         *   \throw SmartRedis::Exception if copy dataset command fails
         */
         void copy_dataset(const std::string& src_name,
                           const std::string& dest_name);
@@ -160,15 +162,15 @@
         /*!
         *   \brief Delete a dataset from the database.  All
         *          tensors and metdata in the dataset will be
         *          deleted.
         *   \details The dataset key used to locate the dataset to be
         *            deleted may be formed by applying a prefix to the
         *            supplied name. See set_data_source()
-        *            and use_tensor_ensemble_prefix() for more details.
+        *            and use_dataset_ensemble_prefix() for more details.
         *   \param name The dataset key for the dataset to be deleted.
         *   \throw SmartRedis::Exception if delete dataset command fails
         */
         void delete_dataset(const std::string& name);
 
         /*!
         *   \brief Put a tensor into the database
@@ -706,15 +708,15 @@
         *   \details The model key used to locate the model to be deleted
         *            may be formed by applying a prefix to the supplied
         *            name. See set_data_source() and use_model_ensemble_prefix()
         *            for more details.
         *            The first_gpu and num_gpus parameters must match those used
         *            when the model was stored.
         *   \param name The name associated with the model
-        *   \param first_cpu the first GPU (zero-based) to use with the model
+        *   \param first_gpu the first GPU (zero-based) to use with the model
         *   \param num_gpus the number of gpus for which the model was stored
         *   \throw SmartRedis::Exception if model deletion fails
         */
         void delete_model_multigpu(const std::string& name, int first_gpu, int num_gpus);
 
         /*!
         *   \brief Remove a script from the database
@@ -733,15 +735,15 @@
         *   \details The script key used to locate the script to be deleted
         *            may be formed by applying a prefix to the supplied
         *            name. See set_data_source() and use_model_ensemble_prefix()
         *            for more details.
         *            The first_gpu and num_gpus parameters must match those used
         *            when the script was stored.
         *   \param name The name associated with the script
-        *   \param first_cpu the first GPU (zero-based) to use with the script
+        *   \param first_gpu the first GPU (zero-based) to use with the script
         *   \param num_gpus the number of gpus for which the script was stored
         *   \throw SmartRedis::Exception if script deletion fails
         */
         void delete_script_multigpu(const std::string& name, int first_gpu, int num_gpus);
 
         /*!
         *   \brief Check if a key exists in the database
@@ -777,15 +779,15 @@
         bool tensor_exists(const std::string& name);
 
         /*!
         *   \brief Check if a dataset exists in the database
         *   \details The dataset key used to check for existence
         *            may be formed by applying a prefix to the supplied
         *            name. See set_data_source()
-        *            and use_tensor_ensemble_prefix() for more details.
+        *            and use_dataset_ensemble_prefix() for more details.
         *   \param name The dataset name to be checked in the database
         *   \returns Returns true if the dataset exists in the database
         *   \throw SmartRedis::Exception if dataset exists command fails
         */
         bool dataset_exists(const std::string& name);
 
         /*!
@@ -824,15 +826,15 @@
 
         /*!
         *   \brief Check if a dataset exists in the database, repeating
         *          the check at a specified polling interval
         *   \details The dataset key used to check for existence
         *            may be formed by applying a prefix to the supplied
         *            name. See set_data_source()
-        *            and use_tensor_ensemble_prefix() for more details.
+        *            and use_dataset_ensemble_prefix() for more details.
         *   \param name The dataset name to be checked in the database
         *   \param poll_frequency_ms The time delay between checks,
         *                            in milliseconds
         *   \param num_tries The total number of times to check for the name
         *   \returns Returns true if the dataset is found within the
         *            specified number of tries, otherwise false.
         *   \throw SmartRedis::Exception if poll dataset command fails
@@ -880,35 +882,54 @@
         *   \param source_id The prefix for read operations; must have
         *          previously been set via the SSKEYIN environment variable
         *   \throw SmartRedis::Exception for failed setting of data source
         */
         void set_data_source(std::string source_id);
 
         /*!
-        *   \brief Control whether names of tensor and dataset keys are
+        *   \brief Control whether names of tensor keys are
         *          prefixed (e.g. in an ensemble) when forming database keys.
         *   \details This function can be used to avoid key collisions in an
         *            ensemble by prepending the string value from the
-        *            environment variable SSKEYIN to tensor and dataset names.
+        *            environment variable SSKEYIN to tensor names.
         *            Prefixes will only be used if they were previously set
         *            through the environment variables SSKEYOUT and SSKEYIN.
         *            Keys of entities created before this function is called
         *            will not be retroactively prefixed.
-        *            By default, the client prefixes tensor and dataset keys
+        *            By default, the client prefixes tensor keys
         *            with the first prefix specified with the SSKEYIN
         *            and SSKEYOUT environment variables.
         *
-        *  \param use_prefix If set to true, all future operations
-        *                    on tensors and datasets will use
-        *                    a prefix, if available.
+        *  \param use_prefix If set to true, all future operations on tensors
+        *                    will use a prefix, if available.
         *  \throw SmartRedis::Exception for failed activation of tensor prefixing
         */
         void use_tensor_ensemble_prefix(bool use_prefix);
 
         /*!
+        *   \brief Control whether names of dataset keys are
+        *          prefixed (e.g. in an ensemble) when forming database keys.
+        *   \details This function can be used to avoid key collisions in an
+        *            ensemble by prepending the string value from the
+        *            environment variable SSKEYIN to dataset names.
+        *            Prefixes will only be used if they were previously set
+        *            through the environment variables SSKEYOUT and SSKEYIN.
+        *            Keys of entities created before this function is called
+        *            will not be retroactively prefixed.
+        *            By default, the client prefixes dataset keys
+        *            with the first prefix specified with the SSKEYIN
+        *            and SSKEYOUT environment variables.
+        *
+        *  \param use_prefix If set to true, all future operations on datasets
+        *                    will use a prefix, if available.
+        *  \throw SmartRedis::Exception for failed activation of dataset prefixing
+        */
+        void use_dataset_ensemble_prefix(bool use_prefix);
+
+        /*!
         *   \brief Control whether model and script keys are
         *          prefixed (e.g. in an ensemble) when forming database keys.
         *   \details This function can be used to avoid key collisions in an
         *            ensemble by prepending the string value from the
         *            environment variable SSKEYIN to model and script names.
         *            Prefixes will only be used if they were previously set
         *            through the environment variables SSKEYOUT and SSKEYIN.
@@ -932,17 +953,17 @@
         *            aggregation list names.  Prefixes will only be used if
         *            they were previously set through the environment variables
         *            SSKEYOUT and SSKEYIN. Keys for aggregation lists created
         *            before this function is called will not be retroactively
         *            prefixed. By default, the client prefixes aggregation
         *            list keys with the first prefix specified with the SSKEYIN
         *            and SSKEYOUT environment variables.  Note that
-        *            use_tensor_ensemble_prefix() controls prefixing
+        *            use_dataset_ensemble_prefix() controls prefixing
         *            for the entities in the aggregation list, and
-        *            use_tensor_ensemble_prefix() should be given the
+        *            use_dataset_ensemble_prefix() should be given the
         *            same value that was used during the initial
         *            setting of the DataSet into the database.
         *  \param use_prefix If set to true, all future operations
         *                    on aggregation lists will use
         *                    a prefix, if available.
         *  \throw SmartRedis::Exception for failed activation of
         *         aggregation list prefixing
@@ -1125,18 +1146,18 @@
         void copy_list(const std::string& src_name,
                        const std::string& dest_name);
 
         /*!
         *   \brief Rename an aggregation list
         *   \details The old and new aggregation list key used to find and
         *            relocate the list may be formed by applying prefixes to
-        *            the supplied old_name and new_name. See set_data_source()
+        *            the supplied src_name and dest_name. See set_data_source()
         *            and use_list_ensemble_prefix() for more details.
-        *   \param old_name The old list name
-        *   \param new_name The new list name
+        *   \param src_name The initial list name
+        *   \param dest_name The target list name
         *   \throw SmartRedis::Exception if the command fails
         */
         void rename_list(const std::string& src_name,
                          const std::string& dest_name);
 
         /*!
         *   \brief Get the number of entries in the list
@@ -1244,14 +1265,20 @@
         *   \throw SmartRedis::Exception if retrieval fails or
         *          input parameters are invalid
         */
         std::vector<DataSet> get_dataset_list_range(const std::string& list_name,
                                                     const int start_index,
                                                     const int end_index);
 
+        /*!
+        *   \brief Create a string representation of the client
+        *   \returns A string containing client details
+        */
+        std::string to_string() const;
+
     protected:
 
         /*!
         *  \brief Abstract base class used to generalized
         *         running with cluster or non-cluster
         */
         RedisServer* _redis_server;
@@ -1273,65 +1300,65 @@
         /*!
         *   \brief Execute an AddressAtCommand
         *   \param cmd The AddresseAtCommand to execute
         *   \returns The CommandReply after execution
         */
         inline CommandReply _run(AddressAtCommand& cmd)
         {
-            return this->_redis_server->run(cmd);
+            return _redis_server->run(cmd);
         }
 
         /*!
         *   \brief Execute an AddressAnyCommand
         *   \param cmd The AddressAnyCommand to execute
         *   \returns The CommandReply after execution
         */
         inline CommandReply _run(AddressAnyCommand& cmd)
         {
-            return this->_redis_server->run(cmd);
+            return _redis_server->run(cmd);
         }
 
         /*!
         *   \brief Execute a SingleKeyCommand Command
         *   \param cmd The SingleKeyCommand to execute
         *   \returns The CommandReply after execution
         */
         inline CommandReply _run(SingleKeyCommand& cmd)
         {
-            return this->_redis_server->run(cmd);
+            return _redis_server->run(cmd);
         }
 
         /*!
         *   \brief Execute a MultiKeyCommand Command
         *   \param cmd The MultiKeyCommand to execute
         *   \returns The CommandReply after execution
         */
         inline CommandReply _run(MultiKeyCommand& cmd)
         {
-            return this->_redis_server->run(cmd);
+            return _redis_server->run(cmd);
         }
 
         /*!
         *   \brief Execute a CompoundCommand
         *   \param cmd The CompoundCommand to execute
         *   \returns The CommandReply after execution
         */
         inline CommandReply _run(CompoundCommand& cmd)
         {
-            return this->_redis_server->run(cmd);
+            return _redis_server->run(cmd);
         }
 
         /*!
         *   \brief Execute a list of commands
         *   \param cmd_list The CommandList to execute
         *   \returns The CommandReply from the last command execution
         */
         inline std::vector<CommandReply> _run(CommandList& cmd_list)
         {
-            return this->_redis_server->run(cmd_list);
+            return _redis_server->run(cmd_list);
         }
 
         /*!
         *  \brief Set the prefixes that are used for set and get methods
         *         using SSKEYIN and SSKEYOUT environment variables.
         */
         void _set_prefixes_from_env();
@@ -1370,42 +1397,43 @@
         *          input parameters are invalid
         */
         inline CommandReply _get_dataset_metadata(const std::string& name);
 
         /*!
         *  \brief Execute the command to retrieve a subset of a DataSet
         *         aggregation list
-        *   \param name The name of the dataset aggregation list
+        *   \param list_name The name of the dataset aggregation list
         *   \param start_index The starting index of the range
         *                      (inclusive, starting at zero)
         *   \param end_index The ending index of the range
         *                    (inclusive, starting at zero)
         *   \returns A vector containing DataSet objects.
         *   \throw SmartRedis::Exception if retrieval fails or
         *          input parameters are invalid
         */
         inline std::vector<DataSet>
         _get_dataset_list_range(const std::string& list_name,
                                 const int start_index,
                                 const int end_index);
 
+
+        // Add a retrieved tensor to a dataset
         /*!
-        *  \brief Retrieve a tensor and add it to the dataset object
-        *  \param dataset The dataset which will be augmented with the
-        *                 retrieved tensor
-        *  \param name The name (not key) of the tensor to retrieve and add
+        *  \brief Add a tensor retrieved via get_tensor() to a dataset
+        *  \param dataset The dataset which will receive the tensor
+        *  \param name The name by which the tensor shall be added
         *              to the dataset
-        *  \param key The key (not name) of the tensor to retrieve and add
-        *             to the dataset
-        *   \throw SmartRedis::Exception if retrieval or addition
-        *          of tensor fails
-        */
-        inline void _get_and_add_dataset_tensor(DataSet& dataset,
-                                                const std::string& name,
-                                                const std::string& key);
+        *   \param tensor_data get_tensor command reply containing
+        *                      tensor data
+        *   \throw SmartRedis::Exception if addition of tensor fails
+        */
+       inline void _add_dataset_tensor(
+            DataSet& dataset,
+            const std::string& name,
+            CommandReply tensor_data);
 
         /*!
         *   \brief Retrieve the tensor from the DataSet and return
         *          a TensorBase object that can be used to return
         *          tensor information to the user. The returned
         *          TensorBase object has been dynamically allocated,
         *          but not yet tracked for memory management in
@@ -1464,14 +1492,20 @@
         * \brief Flag determining whether prefixes should be used
         *        for tensor keys.
         */
         bool _use_tensor_prefix;
 
         /*!
         * \brief Flag determining whether prefixes should be used
+        *        for dataset keys.
+        */
+        bool _use_dataset_prefix;
+
+        /*!
+        * \brief Flag determining whether prefixes should be used
         *        for model and script keys.
         */
         bool _use_model_prefix;
 
         /*!
         * \brief Flag determining whether prefixes should be used
         *        for model and script keys.
@@ -1647,11 +1681,25 @@
         */
         bool _poll_list_length(const std::string& name, int list_length,
                                int poll_frequency_ms, int num_tries,
                                std::function<bool(int,int)> comp_func);
 
 };
 
-} //namespace SmartRedis
+/*!
+*   \brief Serialize a client
+*   \param stream The stream onto which to serialize the client
+*   \param client The client to serialize
+*   \returns The output stream, for chaining
+*/
+inline
+std::ostream& operator<<(std::ostream& stream, const Client& client)
+{
+    stream << client.to_string();
+    return stream;
+}
+
+
+} // namespace SmartRedis
 
-#endif //__cplusplus
-#endif //SMARTREDIS_CPP_CLIENT_H
+#endif // __cplusplus
+#endif // SMARTREDIS_CLIENT_H
```

### Comparing `smartredis-0.3.1/include/clusterinfocommand.h` & `smartredis-0.4.0/include/clusterinfocommand.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -27,21 +27,21 @@
  */
 
 #ifndef SMARTREDIS_CLUSTERINFOCOMMAND_H
 #define SMARTREDIS_CLUSTERINFOCOMMAND_H
 
 #include "addressatcommand.h"
 
+///@file
+
 /*!
 *  \brief A map of reply data from a database response
 */
 using parsed_reply_map = std::unordered_map<std::string, std::string>;
 
-///@file
-
 namespace SmartRedis {
 
 class RedisServer;
 
 /*!
 *   \brief The ClusterInfoCommand class constructs the Redis CLUSTER INFO command.
 */
@@ -53,10 +53,10 @@
         *          into a nested unordered_map
         *   \param info containing the database cluster information
         *   \return parsed_reply_map containing the database node cluster information
         */
         static parsed_reply_map parse_db_cluster_info(std::string info);
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //CLUSTERINFOCOMMAND
+#endif // SMARTREDIS_CLUSTERINFOCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/command.h` & `smartredis-0.4.0/include/command.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,22 +25,22 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_COMMAND_H
 #define SMARTREDIS_COMMAND_H
 
-#include "stdlib.h"
-#include "commandreply.h"
+#include <stdlib.h>
 #include <string>
 #include <vector>
 #include <unordered_map>
 #include <unordered_set>
 #include <cstring>
 #include <iostream>
+#include "commandreply.h"
 
 ///@file
 
 namespace SmartRedis {
 
 class RedisServer;
 
@@ -49,16 +49,24 @@
 *   \details Keyfield inherits everything from std::string and has
 *            no additional functionality. RTTI enables differentiation
 *            between Keyfields and other command fields.
 */
 class Keyfield: public std::string
 {
     public:
-    Keyfield(std::string s) : _s(s) {};
-    std::string _s;
+        /*!
+        *   \brief Keyfield constructor
+        *   \param s The field name for this key field
+        */
+        Keyfield(std::string s) : _s(s) {};
+
+        /*!
+        *   \brief The name of this key field
+        */
+        std::string _s;
 };
 
 /*!
 *   \brief The Command class constructs Client commands.
 *   \details The Command class has multiple methods for adding
 *          fields to the Command.  The Command.add_field()
 *          methods will copy the underlying field data,
@@ -282,32 +290,30 @@
 
     public:
         /*!
         *   \brief Add key fields to the Command
         *          from a vector of strings.
         *   \details The string key field values are copied to the
         *            Command.
-        *   \param fields The key fields to add to the Command
-        *   \param is_key Boolean indicating if the all
-        *                 of the fields are Command keys
+        *   \param keyfields The key fields to add to the Command
         */
-        void add_keys(const std::vector<std::string>& fields);
+        void add_keys(const std::vector<std::string>& keyfields);
 
         /*!
         *   \brief Add key fields to the Command
         *          from a vector of type T
         *   \details The key field values are copied to the
-        *            Command.  The type T must be convertable
+        *            Command.  The type T must be convertible
         *            to a string via std::to_string.
         *   \tparam T Any type that can be converted
         *             to a string via std::to_string.
         *   \param keyfields The key fields to add to the Command
         */
         template <class T>
-        void add_keys(const std::vector<T>& fields);
+        void add_keys(const std::vector<T>& keyfields);
 
         /*!
         *   \brief Return true if the Command has keys
         *   \returns True if the Command has keys, otherwise
         *            False
         */
         bool has_keys();
@@ -382,14 +388,16 @@
         */
         int get_field_count() const { return _fields.size(); }
 
         /*!
         *   \brief Replace a field in a command
         *   \param new_field The string to swap in
         *   \param pos The location to swap
+        *   \param is_key True IFF the field supplied in new_field
+        *                 is a key field
         */
         void set_field_at(std::string new_field,
                           size_t pos,
                           bool is_key=false);
 
     private:
 
@@ -425,10 +433,10 @@
         *   \brief Helper function for emptying the Command
         */
         void make_empty();
 };
 
 #include "command.tcc"
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_COMMAND_H
+#endif // SMARTREDIS_COMMAND_H
```

### Comparing `smartredis-0.3.1/include/command.tcc` & `smartredis-0.4.0/include/command.tcc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -41,8 +41,8 @@
 void Command::add_keys(const std::vector<T>& keyfields)
 {
     for (size_t i = 0; i < keyfields.size(); i++) {
         this->add_field(std::to_string(keyfields[i]), true);
     }
 }
 
-#endif //SMARTREDIS_COMMAND_TCC
+#endif // SMARTREDIS_COMMAND_TCC
```

### Comparing `smartredis-0.3.1/include/commandlist.h` & `smartredis-0.4.0/include/commandlist.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -30,19 +30,20 @@
 #define SMARTREDIS_COMMANDLIST_H
 
 #include <stdlib.h>
 #include <vector>
 #include "command.h"
 #include "srexception.h"
 
+///@file
+
 namespace SmartRedis {
 
 class CommandList;
 
-//@file
 /*!
 *   \brief The CommandList class constructs multiple Client
 *          Command.
 *   \details CommandList handles the dynamic allocation of a new
 *            message in the list and provides iterators
 *            for iterating over Command.
 */
@@ -150,10 +151,10 @@
         *   \brief A vector container a pointer to all Command
         */
         std::vector<Command*> _commands;
 };
 
 #include "commandlist.tcc"
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_COMMANDLIST_H
+#endif // SMARTREDIS_COMMANDLIST_H
```

### Comparing `smartredis-0.3.1/include/commandlist.tcc` & `smartredis-0.4.0/include/commandlist.tcc`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -38,8 +38,8 @@
         return new_cmd;
     }
     catch (std::bad_alloc &e) {
         throw SRBadAllocException("command");
     }
 };
 
-#endif //SMARTREDIS_COMMANDLIST_TCC
+#endif // SMARTREDIS_COMMANDLIST_TCC
```

### Comparing `smartredis-0.3.1/include/commandreply.h` & `smartredis-0.4.0/include/commandreply.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -31,25 +31,24 @@
 
 #include "stdlib.h"
 #include <sw/redis++/redis++.h>
 #include <iostream>
 #include <vector>
 #include <queue>
 
-namespace SmartRedis {
+///@file
 
-class CommandReply;
+namespace SmartRedis {
 
 /*!
 *   \brief Redis++ command reply type
 */
 typedef std::unique_ptr<redisReply, sw::redis::ReplyDeleter>
         RedisReplyUPtr;
 
-///@file
 /*!
 *   \brief The CommandReply class stores and processes Command
 *          replies.
 *   \details The command reply was built around processing
 *          redis-plus-plus replies.  The redis-plus-plus
 *          generic command execution returns a unique
 *          ptr to a hiredis redisReply.  The destructor
@@ -307,10 +306,10 @@
         *   \param index_tracker String representing previous
         *                        levels of the nested structure
         */
         void _print_nested_reply_structure(redisReply* reply,
                                            std::string index_tracker);
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_COMMANDREPLY_H
+#endif // SMARTREDIS_COMMANDREPLY_H
```

### Comparing `smartredis-0.3.1/include/compoundcommand.h` & `smartredis-0.4.0/include/compoundcommand.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -65,10 +65,10 @@
         *            derived type cast to parent Command
         *            type.
         */
         virtual Command* clone();
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //COMPOUNDCOMMAND
+#endif // SMARTREDIS_COMPOUNDCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/dataset.h` & `smartredis-0.4.0/include/dataset.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -24,43 +24,43 @@
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_DATASET_H
 #define SMARTREDIS_DATASET_H
+
 #ifdef __cplusplus
-#include "stdlib.h"
+#include <stdlib.h>
 #include <string>
 #include <vector>
+#include "srobject.h"
 #include "tensor.h"
 #include "tensorpack.h"
 #include "metadata.h"
 #include "sharedmemorylist.h"
 #include "sr_enums.h"
 
 ///@file
 
-namespace SmartRedis{
-
-class DataSet;
+namespace SmartRedis {
 
 ///@file
 /*!
 *   \brief The DataSet class aggregates tensors
 *          and metadata into a nested data structure
 *          for storage.
 *   \details Tensors in the DataSet can be used in
 *            Client commands such as Client.run_model()
 *            and Client.run_script() as inputs or outputs
 *            by prefixing the input or output tensor with
 *            the DataSet name
 *            (e.g. {dataset_name}.tensor_name).
 */
-class DataSet
+class DataSet : public SRObject
 {
     public:
 
         /*!
         *   \brief DataSet constructor
         *   \param name The name used to reference the DataSet
         */
@@ -87,14 +87,19 @@
         /*!
         *   \brief DataSet move assignment operator
         *   \param dataset The DataSet to move and assign
         */
         DataSet& operator=(DataSet&& dataset) = default;
 
         /*!
+        *   \brief DataSet destructor
+        */
+        virtual ~DataSet();
+
+        /*!
         *   \brief Add a tensor to the DataSet.
         *   \param name The name used to reference the tensor
         *               within the DataSet
         *   \param data The tensor data
         *   \param dims The number of elements in each dimension of the tensor
         *   \param type The data type of the provided tensor data
         *   \param mem_layout The memory layout of the provided tensor data
@@ -232,15 +237,16 @@
         *          std::vector<std::string>.
         *   \param name The name of the metadata string field
         *   \return The strings associated with the metadata field, or
         *           an empty vector if no field matches the supplied
         *           metadata field name
         *   \throw SmartRedis::Exception if metadata retrieval fails
         */
-        std::vector<std::string> get_meta_strings(const std::string& name);
+        std::vector<std::string> get_meta_strings(
+            const std::string& name) const;
 
         /*!
         *   \brief Retrieve metadata string field values from the DataSet.
         *   \details The memory of the data pointer is valid until the
         *            DataSet is destroyed.
         *   \param name The name of the metadata field in the DataSet
         *   \param data Receives an array of strings associated with the
@@ -257,41 +263,110 @@
                               size_t*& lengths);
 
         /*!
         *   \brief Check whether the dataset contains a field
         *   \param field_name The name of the field to check
         *   \returns True iff the DataSet contains the field
         */
-        bool has_field(const std::string& field_name);
+        bool has_field(const std::string& field_name) const;
 
 
         /*!
         *   \brief Clear all entries from a DataSet field.
         *   \param field_name The name of the field to clear
         */
         void clear_field(const std::string& field_name);
 
         /*!
+        *   \brief Retrieve the name of the DataSet
+        *   \returns The name of the DataSet
+        */
+        std::string get_name() const { return _dsname; }
+
+        /*!
+        *   \brief Change the name for the DataSet
+        *   \param name The name for the DataSet
+        */
+        void set_name(std::string name) {
+            if (name.length() > 0)
+                _dsname = name;
+            else
+                throw SRParameterException("Name must be non-zero length");
+        }
+
+        /*!
         *   \brief Retrieve the names of tensors in the DataSet
         *   \returns The name of the tensors in the DataSet
         *   \throw SmartRedis::Exception if metadata retrieval fails
         */
-        std::vector<std::string> get_tensor_names();
+        std::vector<std::string> get_tensor_names() const;
 
         /*!
-        *   \brief Retrieve the name of the DataSet
-        *   \returns The name of the DataSet
+        *   \brief Retrieve tensor names from the DataSet.
+        *   \details The memory of the data pointer is valid until the
+        *            DataSet is destroyed.
+        *   \param data Receives an array of tensor names
+        *   \param n_strings Receives the number of tensor names
+        *   \param lengths Receives an array of the lengths of the tensor names
+        *   \throw SmartRedis::Exception if tensor name retrieval fails
         */
-        std::string get_name() const { return _dsname; }
+        void get_tensor_names(char**& data,
+                              size_t& n_strings,
+                              size_t*& lengths);
 
         /*!
-        *   \brief Change the name for the DataSet
-        *   \param name The name for the DataSet
+        *   \brief Retrieve the data type of a Tensor in the DataSet
+        *   \param name The name of the tensor
+        *   \returns The data type for the tensor
+        *   \throw SmartRedis::Exception if tensor name retrieval fails
         */
-        void set_name(std::string name) { _dsname = name; }
+        SRTensorType get_tensor_type(const std::string& name) const;
+
+        /*!
+        *   \brief Retrieve the dimensions of a Tensor in the DataSet
+        *   \param name The name of the tensor
+        *   \returns A vector of the tensor's dimensions
+        *   \throw SmartRedis::Exception if tensor name retrieval fails
+        */
+        const std::vector<size_t> get_tensor_dims(
+            const std::string& name) const;
+
+        /*!
+        *   \brief Retrieve the names of all metadata fields in the DataSet
+        *   \returns A vector of metadata field names
+        */
+        std::vector<std::string> get_metadata_field_names() const;
+
+        /*!
+        *   \brief Retrieve metadata field names from the DataSet.
+        *   \details The memory of the data pointer is valid until the
+        *            DataSet is destroyed.
+        *   \param data Receives an array of metadata field names
+        *   \param n_strings Receives the number of metadata field names
+        *   \param lengths Receives an array of the lengths of the metadata
+        *                  field names
+        *   \throw SmartRedis::Exception if metadata field name retrieval fails
+        */
+        void get_metadata_field_names(char**& data,
+                                      size_t& n_strings,
+                                      size_t*& lengths);
+
+        /*!
+        *   \brief Retrieve the data type of a metadata field in the DataSet
+        *   \param name The name of the metadata field
+        *   \returns The data type for the metadata field
+        *   \throw SmartRedis::Exception if metadata field name retrieval fails
+        */
+        SRMetaDataType get_metadata_field_type(const std::string& name) const;
+
+        /*!
+        *   \brief Create a string representation of the DataSet
+        *   \returns A string containing DataSet details
+        */
+        std::string to_string() const;
 
         friend class Client;
         friend class PyDataset;
 
     protected:
 
         /*!
@@ -327,21 +402,14 @@
         *   \brief Returns an const iterator pointing to the
         *          past-the-end tensor
         *   \returns const_tensor_iterator to the past-the-end Tensor
         */
         const_tensor_iterator tensor_cend();
 
         /*!
-        *   \brief Retrieve the data type of a Tensor in the DataSet
-        *   \param name The name of the tensor
-        *   \returns The data type for the tensor
-        */
-        SRTensorType get_tensor_type(const std::string& name);
-
-        /*!
         *   \brief Returns a vector of std::pair with
         *          the field name and the field serialization
         *          for all fields in the MetaData set.
         *   \returns std::pair<std::string, std::string> containing
         *            the field name and the field serialization.
         */
         std::vector<std::pair<std::string, std::string>>
@@ -419,11 +487,24 @@
         *         by name, but is used to manage memory associated
         *         with get_tensor() function calls.
         */
         TensorPack _tensor_memory;
 
 };
 
-} //namespace SmartRedis
+/*!
+*   \brief Serialize a dataset
+*   \param stream The stream onto which to serialize the dataset
+*   \param dataset The dataset to serialize
+*   \returns The output stream, for chaining
+*/
+inline
+std::ostream& operator<<(std::ostream& stream, const DataSet& dataset)
+{
+    stream << dataset.to_string();
+    return stream;
+}
+
+} // namespace SmartRedis
 
 #endif
-#endif //SMARTREDIS_DATASET_H
+#endif // SMARTREDIS_DATASET_H
```

### Comparing `smartredis-0.3.1/include/dbinfocommand.h` & `smartredis-0.4.0/include/dbinfocommand.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -27,22 +27,22 @@
  */
 
 #ifndef SMARTREDIS_DBINFOCOMMAND_H
 #define SMARTREDIS_DBINFOCOMMAND_H
 
 #include "addressatcommand.h"
 
+///@file
+
 /*!
 *  \brief A nested map of reply data from a database response
 */
 using parsed_reply_nested_map = std::unordered_map<std::string,
                                 std::unordered_map<std::string, std::string>>;
 
-///@file
-
 namespace SmartRedis {
 
 class RedisServer;
 
 /*!
 *   \brief The DBInfoCommand class constructs the Redis DB INFO command.
 */
@@ -54,10 +54,10 @@
         *          into a nested unordered_map
         *   \param info containing the database node information
         *   \return parsed_reply_nested_map containing the database node information
         */
         static parsed_reply_nested_map parse_db_node_info(std::string info);
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //DBINFOCOMMAND
+#endif // SMARTREDIS_DBINFOCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/dbnode.h` & `smartredis-0.4.0/include/dbnode.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,29 +25,27 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_DBNODE_H
 #define SMARTREDIS_DBNODE_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <string>
+#include "address.h"
 
 ///@file
 
 namespace SmartRedis {
 
-class DBNode;
-
-//@file
 /*!
 *   \brief The DBNode class stores connection and hash slot
 *          information for the database node.
 */
-class DBNode{
+class DBNode {
 
     public:
 
         /*!
         *   \brief DBNode constructor
         */
         DBNode();
@@ -78,27 +76,25 @@
         */
         DBNode& operator=(DBNode&& dbnode) = default;
 
         /*!
         *   \brief DBNode constructor with connection
         *          and hash slot information.
         *   \param name The name of the DBNode
-        *   \param ip The IP address of the DBNode
-        *   \param port The port of the DBNode
+        *   \param addr_spec The TCP or UDS address of the database
         *   \param l_slot The lower hash slot of the DBNode
         *   \param u_slot The upper hash slot of the DBNode
         *   \param prefix A prefix that can be placed into
         *                 a hash tag that can be placed in
         *                 front of a key to ensure placement
         *                 on this DBNode.
         *
         */
         DBNode(std::string name,
-               std::string ip,
-               uint64_t port,
+               SRAddress& addr_spec,
                uint64_t l_slot,
                uint64_t u_slot,
                std::string prefix
                );
 
         /*!
         *   \brief Default DBNode destructor
@@ -111,22 +107,17 @@
         *          node is less than the other lower
         *          hash slot.
         *   \param db_node DBNode to compare to
         */
         bool operator<(const DBNode& db_node) const;
 
         /*!
-        *   \brief The IP address of the DBNode
-        */
-        std::string ip;
-
-        /*!
-        *   \brief The port of the DBNode
+        *   \brief The TCP or UDS address of the DBNode
         */
-        uint64_t port;
+        SRAddress address;
 
         /*!
         *   \brief The name of the DBNode
         */
         std::string name;
 
         /*!
@@ -145,10 +136,10 @@
         *          front of a key to ensure placement
         *          on this DBNode.
         */
         std::string prefix;
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_DBNODE_H
+#endif // SMARTREDIS_DBNODE_H
```

### Comparing `smartredis-0.3.1/include/enum_fortran.inc` & `smartredis-0.4.0/include/enum_fortran.inc`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -73,7 +73,16 @@
   enumerator :: SRRuntimeError   = 4  ! Runtime error executing an operation
   enumerator :: SRParameterError = 5  ! Bad parameter error
   enumerator :: SRTimeoutError   = 6  ! Timeout error
   enumerator :: SRKeyError       = 7  ! Key error
   enumerator :: SRInvalidError   = -1 ! Uninitialized error variable
   enumerator :: SRTypeError      = 9  ! Type mismatch
 end enum
+
+! SRLoggingLevel
+enum, bind(c)
+  enumerator :: LLInvalid   = -1 ! Invalid or uninitialized logging level
+  enumerator :: LLQuiet     = 1  ! No logging at all
+  enumerator :: LLInfo      = 2  ! Informational logging only
+  enumerator :: LLDebug     = 3  ! Verbose logging for debugging purposes
+  enumerator :: LLDeveloper = 4  ! Extra verbose logging for internal use
+end enum
```

### Comparing `smartredis-0.3.1/include/gettensorcommand.h` & `smartredis-0.4.0/include/gettensorcommand.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -79,10 +79,10 @@
         *            are going to just index into the base reply.
         *   \param reply CommandReply from running "AI.TENSORGET"
         *   \return string of the tensor type
         */
        static SRTensorType get_data_type(CommandReply& reply);
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //GETTENSORCOMMAND
+#endif // SMARTREDIS_GETTENSORCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/keyedcommand.h` & `smartredis-0.4.0/include/keyedcommand.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -97,10 +97,10 @@
         /*!
         *   \brief Run this Command on the RedisServer.
         *   \param server A pointer to the RedisServer
         */
         virtual CommandReply run_me(RedisServer* server) = 0;
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //KEYEDCOMMAND
+#endif // SMARTREDIS_KEYEDCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/metadata.h` & `smartredis-0.4.0/include/metadata.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
  /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,15 +25,15 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_METADATA_H
 #define SMARTREDIS_METADATA_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <string>
 #include <vector>
 #include <unordered_map>
 #include "sharedmemorylist.h"
 #include "sr_enums.h"
 #include "metadatafield.h"
 #include "metadatabuffer.h"
@@ -61,16 +61,14 @@
         {DATATYPE_METADATA_STR_FLOAT, SRMetadataTypeFloat},
         {DATATYPE_METADATA_STR_INT32, SRMetadataTypeInt32},
         {DATATYPE_METADATA_STR_INT64, SRMetadataTypeInt64},
         {DATATYPE_METADATA_STR_UINT32, SRMetadataTypeUint32},
         {DATATYPE_METADATA_STR_UINT64, SRMetadataTypeUint64},
         {DATATYPE_METADATA_STR_STRING, SRMetadataTypeString} };
 
-class MetaData;
-
 /*!
 *   \brief The MetaData class stages metadata fields and
            values.  Memory associated with metadata
            retrieval from the MetaData object is valid
            until the MetaData object is destroyed.
 */
 class MetaData
@@ -179,15 +177,16 @@
         *   \brief  Get metadata values string field
         *   \details The string field is returned as a std::vector
         *            of std::string which means that the memory
         *            for the field is managed by the returned object.
         *   \param name The name of the string field to retrieve
         *   \returns A vector of the strings in the field
         */
-        std::vector<std::string> get_string_values(const std::string& name);
+        std::vector<std::string> get_string_values(
+            const std::string& name) const;
 
         /*!
         *   \brief  Get metadata string field using a c-style
         *           interface.
         *   \details This function allocates memory to
         *            return a pointer (via pointer reference "data")
         *            to the user and sets the value of n_strings to
@@ -212,15 +211,15 @@
         /*!
         *   \brief This function checks if the DataSet has a
         *          field
         *   \param field_name The name of the field to check
         *   \returns Boolean indicating if the DataSet has
         *            the field.
         */
-        bool has_field(const std::string& field_name);
+        bool has_field(const std::string& field_name) const;
 
         /*!
         *   \brief This function clears all entries in a
         *          DataSet field.
         *   \param field_name The name of the field to clear
         */
         void clear_field(const std::string& field_name);
@@ -231,15 +230,53 @@
         *          for all fields in the MetaData set.
         *   \returns std::pair<std::string, std::string> containing
         *            the field name and the field serialization.
         */
         std::vector<std::pair<std::string, std::string>>
             get_metadata_serialization_map();
 
+        /*!
+        *   \brief Retrieve the type of a metadata field
+        *   \param name The name of the field to check
+        *   \throw KeyException if the name is not present
+        */
+        SRMetaDataType get_field_type(const std::string& name) const;
+
+        /*!
+        *   \brief Retrieve a vector of metadata field names
+        *   \param skip_internal Omit internal items (such as .tensor_names)
+        *                        from the results
+        */
+        std::vector<std::string> get_field_names(
+            bool skip_internal = false) const;
 
+        /*!
+        *   \brief  Get metadata field names using a c-style
+        *           interface
+        *   \details This function allocates memory to
+        *            return a pointer (via pointer reference "data")
+        *            to the user and sets the value of n_strings to
+        *            the number of strings in the field.  Memory is also
+        *            allocated to store the length of each string in the
+        *            field, and the provided lengths pointer is pointed
+        *            to this new memory.  The memory for the strings and
+        *            string lengths is valid until the MetaData object is
+        *            destroyed.
+        *   \param data A c-ptr pointed to newly allocated memory
+        *               for the names
+        *   \param n_strings The number of names returned
+        *   \param lengths A size_t pointer pointed to newly allocated
+        *                  memory that stores the length of each string
+        *   \param skip_internal Omit internal items (such as .tensor_names)
+        *                        from the results
+        */
+        void get_field_names(char**& data,
+                             size_t& n_strings,
+                             size_t*& lengths,
+                             bool skip_internal = false);
     private:
 
        /*!
         *   \brief Clone data from another Metadata instance
         *   \param other The MetaData object to clone
         */
         void _clone_from(const MetaData& other);
@@ -369,10 +406,10 @@
         *   \brief Delete the memory associated with all fields
         *          and clear inventory
         */
         void _delete_fields();
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_METADATA_H
+#endif // SMARTREDIS_METADATA_H
```

### Comparing `smartredis-0.3.1/include/metadatabuffer.h` & `smartredis-0.4.0/include/metadatabuffer.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -377,10 +377,10 @@
     size_t n_vals = (total_bytes - byte_position) / sizeof(T);
     std::vector<T> vals(n_vals);
 
     std::memcpy(vals.data(), (T*)data, total_bytes - byte_position);
     return vals;
 }
 
-} //namespace MetadataBuffer
+} // namespace MetadataBuffer
 
-#endif
+#endif // SMARTREDIS_METADATABUFFER_H
```

### Comparing `smartredis-0.3.1/include/metadatafield.h` & `smartredis-0.4.0/include/metadatafield.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -29,17 +29,17 @@
 #ifndef SMARTREDIS_METADATAFIELD_H
 #define SMARTREDIS_METADATAFIELD_H
 
 #include <vector>
 #include <string>
 #include "sr_enums.h"
 
-namespace SmartRedis {
+///@file
 
-class MetadataField;
+namespace SmartRedis {
 
 /*!
 *   \brief  Abstract base class for interfacing with
 *           different metadata field types.
 */
 class MetadataField {
 
@@ -63,27 +63,27 @@
     */
     virtual std::string serialize() = 0;
 
     /*!
     *   \brief Retrieve the MetadataField name
     *   \returns MetadataField name
     */
-    std::string name();
+    std::string name() const;
 
     /*!
     *   \brief Retrieve the Metadatafield type
     *   \returns MetadataField type
     */
-    SRMetaDataType type();
+    SRMetaDataType type() const;
 
     /*!
     *   \brief Retrieve the number of values in the field
     *   \returns The number of values
     */
-    virtual size_t size() = 0;
+    virtual size_t size() const = 0;
 
     /*!
     *   \brief Clear the values in the field
     */
     virtual void clear() = 0;
 
     protected:
@@ -97,12 +97,10 @@
     *   \brief The field type.
     */
     SRMetaDataType _type;
 
 };
 
 
-}  //namespace SmartRedis
-
-
+}  // namespace SmartRedis
 
-#endif //SMARTREDIS_METADATAFIELD_H
+#endif // SMARTREDIS_METADATAFIELD_H
```

### Comparing `smartredis-0.3.1/include/multikeycommand.h` & `smartredis-0.4.0/include/multikeycommand.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -64,10 +64,10 @@
         *   \returns A pointer to dynamically allocated
         *            derived type cast to parent Command
         *            type.
         */
         virtual Command* clone();
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //MULTIKEYCOMMAND
+#endif // SMARTREDIS_MULTIKEYCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/pipelinereply.h` & `smartredis-0.4.0/include/pipelinereply.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,26 +25,24 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_PIPELINEREPLY_H
 #define SMARTREDIS_PIPELINEREPLY_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <sw/redis++/redis++.h>
 #include <iostream>
 #include <vector>
 #include <queue>
 
 #include "commandreply.h"
 
 namespace SmartRedis {
 
-class PipelineReply;
-
 /*!
 *   \brief Redis++ pipeline command reply type
 */
 typedef sw::redis::QueuedReplies QueuedReplies;
 
 ///@file
 /*!
@@ -187,10 +185,10 @@
         *          of replies.
         *   \param reply The QueuedReplies object to add
         */
         void _add_queuedreplies(QueuedReplies&& reply);
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_PIPELINEREPLY_H
+#endif // SMARTREDIS_PIPELINEREPLY_H
```

### Comparing `smartredis-0.3.1/include/pyclient.h` & `smartredis-0.4.0/include/pyclient.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,55 +22,57 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#define PY_CLIENT_H
-#ifdef __cplusplus
+#ifndef SMARTREDIS_PYCLIENT_H
+#define SMARTREDIS_PYCLIENT_H
 
-#include "client.h"
-#include "pydataset.h"
 #include <pybind11/pybind11.h>
 #include <pybind11/pytypes.h>
 #include <pybind11/stl_bind.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 #include <string>
 #include <unordered_map>
+#include "client.h"
+#include "pydataset.h"
+#include "pysrobject.h"
 
 ///@file
 
 namespace SmartRedis {
 
 namespace py = pybind11;
 
-class PyClient;
-
 /*!
 *   \brief The PyClient class is a wrapper around the
            C++ client that is needed for the Python
            client.
 */
-class PyClient
+class PyClient : public PySRObject
 {
     public:
 
         /*!
         *   \brief PyClient constructor
         *   \param cluster Flag to indicate if a database cluster
         *                  is being used
+        *   \param logger_name Identifier for the current client
         */
-        PyClient(bool cluster);
+        PyClient(
+            bool cluster,
+            const std::string& logger_name = std::string("default"));
 
         /*!
         *   \brief PyClient destructor
         */
-        ~PyClient();
+        virtual ~PyClient();
 
         /*!
         *   \brief Put a tensor into the database
         *   \param name The name to associate with this tensor
         *              in the database
         *   \param type The data type of the tensor
         *   \param data Numpy array with Pybind*
@@ -441,15 +443,15 @@
         *   \throw RuntimeException for all client errors
         */
         void delete_model(const std::string& name);
 
         /*!
         *   \brief Remove a model from the database
         *   \param name The name associated with the model
-        *   \param first_cpu the first GPU (zero-based) to use with the model
+        *   \param first_gpu the first GPU (zero-based) to use with the model
         *   \param num_gpus the number of gpus for which the model was stored
         *   \throw RuntimeException for all client errors
         */
         void delete_model_multigpu(const std::string& name, int first_gpu, int num_gpus);
 
         /*!
         *   \brief Remove a script from the database
@@ -458,15 +460,15 @@
         */
         void delete_script(const std::string& name);
 
         /*!
         *   \brief Remove a script from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the script
-        *   \param first_cpu the first GPU (zero-based) to use with the script
+        *   \param first_gpu the first GPU (zero-based) to use with the script
         *   \param num_gpus the number of gpus for which the script was stored
         *   \throw RuntimeException for all client errors
         */
         void delete_script_multigpu(const std::string& name, int first_gpu, int num_gpus);
 
         /*!
         *   \brief Retrieve the model from the database
@@ -612,42 +614,56 @@
         *            aggregation list names.  Prefixes will only be used if
         *            they were previously set through the environment variables
         *            SSKEYOUT and SSKEYIN. Keys for aggregation lists created
         *            before this function is called will not be retroactively
         *            prefixed. By default, the client prefixes aggregation
         *            list keys with the first prefix specified with the SSKEYIN
         *            and SSKEYOUT environment variables.  Note that
-        *            use_tensor_ensemble_prefix() controls prefixing
+        *            use_dataset_ensemble_prefix() controls prefixing
         *            for the entities in the aggregation list, and
-        *            use_tensor_ensemble_prefix() should be given the
+        *            use_dataset_ensemble_prefix() should be given the
         *            same value that was used during the initial
         *            setting of the DataSet into the database.
         *  \param use_prefix If set to true, all future operations
         *                    on aggregation lists will use
         *                    a prefix, if available.
         */
         void use_list_ensemble_prefix(bool use_prefix);
 
         /*!
-        * \brief Set whether names of tensors or datasets should be
-        *        prefixed (e.g. in an ensemble) to form database keys.
+        * \brief Set whether names of tensors should be prefixed (e.g.
+        *        in an ensemble) to form database keys.
         *        Prefixes will only be used if they were previously set through
         *        the environment variables SSKEYOUT and SSKEYIN.
         *        Keys formed before this function is called will not be affected.
-        *        By default, the client prefixes tensor and dataset keys
-        *        with the first prefix specified with the SSKEYIN
-        *        and SSKEYOUT environment variables.
+        *        By default, the client prefixes tensor keys with the first
+        *        prefix specified with the SSKEYIN and SSKEYOUT environment
+        *        variables.
         *
-        * \param use_prefix If set to true, all future operations
-        *                   on tensors and datasets will add
-        *                   a prefix to the entity names, if available.
+        * \param use_prefix If set to true, all future operations on tensors will
+        *                   add a prefix to the entity names, if available.
         */
         void use_tensor_ensemble_prefix(bool use_prefix);
 
         /*!
+        * \brief Set whether names of datasets should be prefixed (e.g.
+        *        in an ensemble) to form database keys.
+        *        Prefixes will only be used if they were previously set through
+        *        the environment variables SSKEYOUT and SSKEYIN.
+        *        Keys formed before this function is called will not be affected.
+        *        By default, the client prefixes tensor keys with the first
+        *        prefix specified with the SSKEYIN and SSKEYOUT environment
+        *        variables.
+        *
+        * \param use_prefix If set to true, all future operations on datasets will
+        *                   add a prefix to the entity names, if available.
+        */
+        void use_dataset_ensemble_prefix(bool use_prefix);
+
+        /*!
         *   \brief Returns information about the given database nodes
         *   \param addresses The addresses of the database nodes. Each address is
         *                    formatted as address:port e.g. 127.0.0.1:6379
         *   \returns A list of parsed_map objects containing all the
         *            information about the given database nodes
         *   \throw RuntimeException if the address is not addressable by this
         *          client.  In the case of using a cluster of database nodes,
@@ -784,20 +800,20 @@
         *   \throw SmartRedis::Exception if the command fails
         */
         void copy_list(const std::string& src_name,
                        const std::string& dest_name);
 
         /*!
         *   \brief Rename an aggregation list
-        *   \details The old and new aggregation list key used to find and
+        *   \details The initial and target aggregation list key used to find and
         *            relocate the list may be formed by applying prefixes to
-        *            the supplied old_name and new_name. See set_data_source()
+        *            the supplied src_name and dest_name. See set_data_source()
         *            and use_list_ensemble_prefix() for more details.
-        *   \param old_name The old list name
-        *   \param new_name The new list name
+        *   \param src_name The initial list name
+        *   \param dest_name The target list name
         *   \throw SmartRedis::Exception if the command fails
         */
         void rename_list(const std::string& src_name,
                          const std::string& dest_name);
 
         /*!
         *   \brief Get the number of entries in the list
@@ -905,20 +921,27 @@
         *   \throw SmartRedis::Exception if retrieval fails or
         *          input parameters are invalid
         */
         py::list get_dataset_list_range(const std::string& list_name,
                                         const int start_index,
                                         const int end_index);
 
+        /*!
+        *   \brief Create a string representation of the Client
+        *   \returns A string representation of the Client
+        */
+        std::string to_string();
+
+
     private:
 
         /*!
         *   \brief Pointer to a Client object for
         *          executing server commands
         */
         Client* _client;
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //PY_CLIENT_H
+#endif // SMARTREDIS_PYCLIENT_H
```

### Comparing `smartredis-0.3.1/include/pydataset.h` & `smartredis-0.4.0/include/pydataset.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,33 +22,35 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#include "dataset.h"
+#ifndef SMARTREDIS_PYDATASET_H
+#define SMARTREDIS_PYDATASET_H
+
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 #include <string>
+#include "dataset.h"
+#include "pysrobject.h"
 
 ///@file
 
 namespace py = pybind11;
 
 namespace SmartRedis {
 
-class PyDataset;
-
 /*!
 *   \brief The PyDataset class is a wrapper around the
            C++ dataset abstraction class.
 */
-class PyDataset
+class PyDataset : public PySRObject
 {
     public:
 
         /*!
         *   \brief PyDataset constructor
         *   \param name The name of the dataset
         */
@@ -64,15 +66,15 @@
         *                  deletion.
         */
         PyDataset(DataSet* dataset);
 
         /*!
         *   \brief PyDataset destructor
         */
-        ~PyDataset();
+        virtual ~PyDataset();
 
         /*!
         *   \brief Add a tensor to the PyDataset
         *   \param name The name of the tensor
         *   \param data A py::array containing the tensor data
         *   \param type A std::string corresponding to the tensor
         *               data type
@@ -126,25 +128,67 @@
         *          PyDataset
         *   \param name The name of the field
         *   \returns A py::array with all of the field values
         */
         py::list get_meta_strings(const std::string& name);
 
         /*!
+        *   \brief Retrieve the names of all tensors in the DataSet
+        *   \returns A vector of tensor names
+        */
+        py::list get_tensor_names();
+
+        /*!
+        *   \brief Retrieve the data type of a Tensor in the DataSet
+        *   \param name The name of the tensor
+        *   \returns The data type for the tensor
+        */
+        std::string get_tensor_type(const std::string& name);
+
+        /*!
+        *   \brief Retrieve the dimensions of a Tensor in the DataSet
+        *   \param name The name of the tensor
+        *   \returns A list of the tensor's dimensions
+        *   \throw SmartRedis::Exception if tensor name retrieval fails
+        */
+        py::list get_tensor_dims(const std::string& name);
+
+        /*!
+        *   \brief Retrieve the names of all metadata fields in the DataSet
+        *   \returns A vector of metadata field names
+        */
+        py::list get_metadata_field_names();
+
+        /*!
+        *   \brief Retrieve the data type of a metadata field in the DataSet
+        *   \param name The name of the metadata field
+        *   \returns The data type for the metadata field
+        */
+        std::string get_metadata_field_type(const std::string& name);
+
+        /*!
         *   \brief Get the name of the PyDataset
         *   \returns std::string of the PyDataset name
         */
         std::string get_name();
 
         /*!
         *   \brief Retrieve a pointer to the underlying
         *          SmartRedis::DataSet object
         *   \returns DataSet pointer within PyDataset
         */
-        DataSet* get();
+        DataSet* get() { return _dataset; }
+
+        /*!
+        *   \brief Create a string representation of the DataSet
+        *   \returns A string representation of the DataSet
+        */
+        std::string to_string();
 
     private:
 
         DataSet* _dataset;
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
+
+#endif // SMARTREDIS_PYDATASET_H
```

### Comparing `smartredis-0.3.1/include/redis.h` & `smartredis-0.4.0/include/redis.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,43 +22,47 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef SMARTREDIS_CPP_REDIS_H
-#define SMARTREDIS_CPP_REDIS_H
+#ifndef SMARTREDIS_REDIS_H
+#define SMARTREDIS_REDIS_H
 
 #include "redisserver.h"
 
+///@file
+
 namespace SmartRedis {
 
-///@file
+class SRObject;
 
 /*!
 *   \brief  The Redis class executes RedisServer
 *           commands on a non-cluster redis server.
 */
 class Redis : public RedisServer
 {
     public:
         /*!
         *   \brief Redis constructor.
+        *   \param context The owning context
         */
-        Redis();
+        Redis(const SRObject* context);
 
         /*!
         *   \brief Redis constructor.
         *          Uses address provided to constructor instead
         *          of environment variables.
-        *   \param address_port The address and port in the form of
-        *                       "tcp://address:port"
+        *   \param context The owning context
+        *   \param addr_spec The TCP or UDS server address
+        *   \throw SmartRedis::Exception if connection fails
         */
-        Redis(std::string address_port);
+        Redis(const SRObject* context, std::string addr_spec);
 
         /*!
         *   \brief Redis copy constructor is not allowed
         *   \param cluster The Redis to copy for construction
         */
         Redis(const Redis& cluster) = delete;
 
@@ -84,176 +88,189 @@
         *   \param cluster The Redis to move for assignment
         */
         Redis& operator=(Redis&& cluster) = default;
 
        /*!
         *   \brief Run a SingleKeyCommand on the server
         *   \param cmd The SingleKeyCommand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(SingleKeyCommand& cmd);
 
         /*!
         *   \brief Run a MultiKeyCommand on the server
         *   \param cmd The MultiKeyCommand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(MultiKeyCommand& cmd);
 
         /*!
         *   \brief Run a CompoundCommand on the server
         *   \param cmd The CompoundCommand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(CompoundCommand& cmd);
 
         /*!
         *   \brief Run an AddressAtCommand on the server
         *   \param cmd The AddressAtCommand command to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAtCommand& cmd);
 
         /*!
         *   \brief Run an AddressAnyCommand on the server
         *   \param cmd The AddressAnyCommand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAnyCommand& cmd);
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses every db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses any db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses any db node
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAllCommand& cmd);
 
         /*!
         *   \brief Run multiple single-key or single-hash slot
         *          Command on the server.  Each Command in the
         *          CommandList is run sequentially.
-        *   \param cmd The CommandList containing multiple
-        *              single-key or single-hash
-        *              slot Comand to run
+        *   \param cmd The CommandList containing multiple single-key or
+        *              single-hash slot Command to run
         *   \returns A list of CommandReply for each Command
         *            in the CommandList
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual std::vector<CommandReply> run(CommandList& cmd);
 
         /*!
         *   \brief Run multiple single-key or single-hash slot
         *          Command on the server in pipelines.  The
         *          Command in the CommandList will be grouped
         *          by shard, and executed in groups by shard.
         *          Commands are not guaranteed to be executed
         *          in any sequence or ordering.
-        *   \param cmd The CommandList containing multiple
-        *              single-key or single-hash
-        *              slot Command to run
+        *   \param cmd_list The CommandList containing multiple single-key
+        *                   or single-hash slot Commands to run
         *   \returns A list of CommandReply for each Command
         *            in the CommandList. The order of the result
         *            matches the order of the input CommandList.
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual PipelineReply
         run_via_unordered_pipelines(CommandList& cmd_list);
 
         /*!
         *   \brief Check if a key exists in the database. This
         *          function does not work for models and scripts.
         *          For models and scripts, model_key_exists should
         *          be used.
         *   \param key The key to check
         *   \returns True if the key exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool key_exists(const std::string& key);
 
         /*!
         *   \brief Check if a hash field exists
         *   \param key The key containing the field
         *   \param field The field in the key to check
         *   \returns True if the hash field exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool hash_field_exists(const std::string& key,
                                        const std::string& field);
 
         /*!
         *   \brief Check if a model or script key exists in the database
         *   \param key The key to check
         *   \returns True if the key exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool model_key_exists(const std::string& key);
 
         /*!
          *  \brief Check if address is valid
-         *  \param address Address of database
-         *  \param port Port of database
+         *  \param address Address (TCP or UDS) of database
          *  \return True if address is valid
          */
-        virtual bool is_addressable(const std::string& address, const uint64_t& port);
+        virtual bool is_addressable(const SRAddress& address) const;
 
         /*!
         *   \brief Put a Tensor on the server
         *   \param tensor The Tensor to put on the server
-        *   \returns The CommandReply from the put tensor
-        *            command execution
+        *   \returns The CommandReply from the put tensor command execution
+        *   \throw SmartRedis::Exception if tensor storage fails
         */
         virtual CommandReply put_tensor(TensorBase& tensor);
 
         /*!
         *   \brief Get a Tensor from the server
         *   \param key The name of the tensor to retrieve
         *   \returns The CommandReply from the get tensor server
         *            command execution
+        *   \throw SmartRedis::Exception if tensor retrieval fails
         */
         virtual CommandReply get_tensor(const std::string& key);
 
         /*!
+        *   \brief Get a list of Tensor from the server
+        *   \param keys The keys of the tensor to retrieve
+        *   \returns The PipelineReply from executing the get tensor commands
+        *   \throw SmartRedis::Exception if tensor retrieval fails
+        */
+        virtual PipelineReply get_tensors(
+            const std::vector<std::string>& keys);
+
+        /*!
         *   \brief Rename a tensor in the database
         *   \param key The original key for the tensor
         *   \param new_key The new key for the tensor
-        *   \returns The CommandReply from executing the RENAME
-        *            command
+        *   \returns The CommandReply from executing the RENAME command
+        *   \throw SmartRedis::Exception if tensor rename fails
         */
         virtual CommandReply rename_tensor(const std::string& key,
                                            const std::string& new_key);
 
         /*!
         *   \brief Delete a tensor in the database
         *   \param key The database key for the tensor
         *   \returns The CommandReply from delete command
         *            executed on the server
+        *   \throw SmartRedis::Exception if tensor removal fails
         */
         virtual CommandReply delete_tensor(const std::string& key);
 
         /*!
         *   \brief Copy a tensor from the source key to
         *          the destination key
         *   \param src_key The source key for the tensor copy
         *   \param dest_key The destination key for the tensor copy
-        *   \returns The CommandReply from executing the COPY
-        *            command
+        *   \returns The CommandReply from executing the COPY command
+        *   \throw SmartRedis::Exception if tensor copy fails
         */
         virtual CommandReply copy_tensor(const std::string& src_key,
                                          const std::string& dest_key);
 
         /*!
         *   \brief Copy a vector of tensors from source keys
         *          to destination keys
         *   \param src Vector of source keys
         *   \param dest Vector of destination keys
         *   \returns The CommandReply from the last put command
         *            associated with the tensor copy
+        *   \throw SmartRedis::Exception if tensor copy fails
         */
         virtual CommandReply copy_tensors(const std::vector<std::string>& src,
                                           const std::vector<std::string>& dest);
 
 
         /*!
         *   \brief Set a model from std::string_view buffer in the
@@ -261,23 +278,22 @@
         *   \param key The key to associate with the model
         *   \param model The model as a continuous buffer string_view
         *   \param backend The name of the backend
         *                  (TF, TFLITE, TORCH, ONNX)
         *   \param device The name of the device for execution
         *                 (e.g. CPU or GPU)
         *   \param batch_size The batch size for model execution
-        *   \param min_batch_size The minimum batch size for model
-        *                         execution
-        *   \param tag A tag to attach to the model for
-        *              information purposes
+        *   \param min_batch_size The minimum batch size for model execution
+        *   \param tag A tag to attach to the model for information purposes
         *   \param inputs One or more names of model input nodes
         *                 (TF models only)
         *   \param outputs One or more names of model output nodes
         *                 (TF models only)
         *   \returns The CommandReply from the set_model Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply set_model(const std::string& key,
                                        std::string_view model,
                                        const std::string& backend,
                                        const std::string& device,
                                        int batch_size = 0,
                                        int min_batch_size = 0,
@@ -293,18 +309,16 @@
         *   \param name The name to associate with the model
         *   \param model The model as a continuous buffer string_view
         *   \param backend The name of the backend
         *                  (TF, TFLITE, TORCH, ONNX)
         *   \param first_gpu The first GPU to use with this model
         *   \param num_gpus The number of GPUs to use with this model
         *   \param batch_size The batch size for model execution
-        *   \param min_batch_size The minimum batch size for model
-        *                         execution
-        *   \param tag A tag to attach to the model for
-        *              information purposes
+        *   \param min_batch_size The minimum batch size for model execution
+        *   \param tag A tag to attach to the model for information purposes
         *   \param inputs One or more names of model input nodes
         *                 (TF models only)
         *   \param outputs One or more names of model output nodes
         *                 (TF models only)
         *   \throw RuntimeException for all client errors
         */
         virtual void set_model_multigpu(const std::string& name,
@@ -324,14 +338,15 @@
         *   \brief Set a script from std::string_view buffer in the
         *          database for future execution
         *   \param key The key to associate with the script
         *   \param device The name of the device for execution
         *                 (e.g. CPU or GPU)
         *   \param script The script source in a std::string_view
         *   \returns The CommandReply from set_script Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply set_script(const std::string& key,
                                         const std::string& device,
                                         std::string_view script);
 
         /*!
         *   \brief Set a script from std::string_view buffer in the
@@ -340,27 +355,26 @@
         *   \param script The script source in a std::string_view
         *   \param first_gpu The first GPU to use with this script
         *   \param num_gpus The number of GPUs to use with this script
         *   \throw RuntimeException for all client errors
         */
         virtual void set_script_multigpu(const std::string& name,
                                          const std::string_view& script,
-                                         int first_cpu,
+                                         int first_gpu,
                                          int num_gpus);
 
         /*!
         *   \brief Run a model in the database using the
         *          specified input and output tensors
         *   \param key The key associated with the model
-        *   \param inputs The keys of inputs tensors to use
-        *                 in the model
+        *   \param inputs The keys of inputs tensors to use in the model
         *   \param outputs The keys of output tensors that
         *                 will be used to save model results
-        *   \returns The CommandReply from the run model server
-        *            Command
+        *   \returns The CommandReply from the run model server Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply run_model(const std::string& key,
                                        std::vector<std::string> inputs,
                                        std::vector<std::string> outputs);
 
         /*!
         *   \brief Run a model in the database using the
@@ -383,20 +397,19 @@
                                         int num_gpus);
 
         /*!
         *   \brief Run a script function in the database using the
         *          specified input and output tensors
         *   \param key The key associated with the script
         *   \param function The name of the function in the script to run
-        *   \param inputs The keys of inputs tensors to use
-        *                 in the script
+        *   \param inputs The keys of inputs tensors to use in the script
         *   \param outputs The keys of output tensors that
         *                 will be used to save script results
-        *   \returns The CommandReply from script run Command
-        *            execution
+        *   \returns The CommandReply from script run Command execution
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply run_script(const std::string& key,
                                         const std::string& function,
                                         std::vector<std::string> inputs,
                                         std::vector<std::string> outputs);
 
         /*!
@@ -429,15 +442,15 @@
         */
         virtual CommandReply delete_model(const std::string& key);
 
         /*!
         *   \brief Remove a model from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the model
-        *   \param first_cpu the first GPU (zero-based) to use with the model
+        *   \param first_gpu the first GPU (zero-based) to use with the model
         *   \param num_gpus the number of gpus for which the model was stored
         *   \throw SmartRedis::Exception if model deletion fails
         */
         virtual void delete_model_multigpu(
             const std::string& name, int first_gpu, int num_gpus);
 
         /*!
@@ -448,78 +461,102 @@
         */
         virtual CommandReply delete_script(const std::string& key);
 
         /*!
         *   \brief Remove a script from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the script
-        *   \param first_cpu the first GPU (zero-based) to use with the script
+        *   \param first_gpu the first GPU (zero-based) to use with the script
         *   \param num_gpus the number of gpus for which the script was stored
         *   \throw SmartRedis::Exception if script deletion fails
         */
         virtual void delete_script_multigpu(
             const std::string& name, int first_gpu, int num_gpus);
 
         /*!
         *   \brief Retrieve the model from the database
         *   \param key The key associated with the model
         *   \returns The CommandReply that contains the result
         *            of the get model execution on the server
+        *   \throw SmartRedis::Exception if model retrieval fails
         */
         virtual CommandReply get_model(const std::string& key);
 
         /*!
         *   \brief Retrieve the script from the database
         *   \param key The key associated with the script
         *   \returns The CommandReply that contains the result
         *            of the get script execution on the server
+        *   \throw SmartRedis::Exception if script retrieval fails
         */
         virtual CommandReply get_script(const std::string& key);
 
         /*!
         *   \brief Retrieve model/script runtime statistics
         *   \param address The address of the database node (host:port)
         *   \param key The key associated with the model or script
         *   \param reset_stat Boolean indicating if the counters associated
         *                     with the model or script should be reset.
         *   \returns The CommandReply that contains the result
         *            of the AI.INFO execution on the server
+        *   \throw SmartRedis::Exception if info retrieval fails
         */
         virtual CommandReply
         get_model_script_ai_info(const std::string& address,
                                  const std::string& key,
                                  const bool reset_stat);
 
+        /*!
+        *   \brief Run a CommandList via a Pipeline
+        *   \param cmdlist The list of commands to run
+        *   \returns The PipelineReply with the result of command execution
+        *   \throw SmartRedis::Exception if execution fails
+        */
+        PipelineReply run_in_pipeline(CommandList& cmdlist);
+
+        /*!
+        *   \brief Create a string representation of the Redis connection
+        *   \returns A string representation of the Redis connection
+        */
+        virtual std::string to_string() const;
+
     private:
 
         /*!
         *   \brief sw::redis::Redis object pointer
         */
         sw::redis::Redis* _redis;
 
         /*!
         *   \brief Run a Command on the server
         *   \param cmd The Command to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         inline CommandReply _run(const Command& cmd);
 
         /*!
-        *   \brief Inserts a string formatted as address:port
-                   into _address_node_map. Strips the protocol
-                   (tcp:// or unix://) before inserting.
-        *   \param address_port A string formatted as protocol://address:port
+        *   \brief Inserts an address into _address_node_map
+        *   \param db_address The server address
         */
-        inline void _add_to_address_map(std::string address_port);
+        inline void _add_to_address_map(SRAddress& db_address);
 
         /*!
         *   \brief Connect to the server at the address and port
-        *   \param address_port A string formatted as tcp://address:port
-        *                       for redis connection
+        *   \param db_address The server address
+        *   \throw SmartRedis::Exception if connection fails
         */
-        inline void _connect(std::string address_port);
+        inline void _connect(SRAddress& db_address);
+
+        /*!
+        *   \brief Pipeline execute a series of commands
+        *   \param cmds The commands to execute
+        *   \returns Pipeline reply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
+        */
+        PipelineReply _run_pipeline(std::vector<Command*>& cmds);
+
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_CPP_REDIS_H
+#endif // SMARTREDIS_REDIS_H
```

### Comparing `smartredis-0.3.1/include/rediscluster.h` & `smartredis-0.4.0/include/rediscluster.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,53 +22,55 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef SMARTREDIS_CPP_CLUSTER_H
-#define SMARTREDIS_CPP_CLUSTER_H
+#ifndef SMARTREDIS_REDISCLUSTER_H
+#define SMARTREDIS_REDISCLUSTER_H
 
 #include <unordered_set>
 #include <mutex>
 
 #include "redisserver.h"
 #include "dbnode.h"
 #include "nonkeyedcommand.h"
 #include "keyedcommand.h"
 #include "pipelinereply.h"
+#include "address.h"
 
 namespace SmartRedis {
 
 ///@file
 
-class RedisCluster;
+class SRObject;
 
 /*!
 *   \brief  The RedisCluster class executes RedisServer
 *           commands on a redis cluster.
 */
 class RedisCluster : public RedisServer
 {
     public:
 
         /*!
         *   \brief RedisCluster constructor.
+        *   \param context The owning context
         */
-        RedisCluster();
+        RedisCluster(const SRObject* context);
 
         /*!
-        *   \brief RedisCluster constructor.
-        *          Uses address provided to constructor instead
-        *          of environment variables.
-        *   \param address_port The address and port in the form of
-        *                       "tcp://address:port"
+        *   \brief RedisCluster constructor. Uses address provided to
+        *          constructor instead of environment variables.
+        *   \param context The owning context
+        *   \param address_spec The TCP or UDS address of the server
+        *   \throw SmartRedis::Exception if connection fails
         */
-        RedisCluster(std::string address_port);
+        RedisCluster(const SRObject* context, std::string address_spec);
 
         /*!
         *   \brief RedisCluster copy constructor is not allowed
         *   \param cluster The RedisCluster to copy for construction
         */
         RedisCluster(const RedisCluster& cluster) = delete;
 
@@ -93,187 +95,201 @@
         *   \brief RedisCluster move assignment
         *   \param cluster The RedisCluster to move for assignment
         */
         RedisCluster& operator=(RedisCluster&& cluster) = default;
 
         /*!
         *   \brief Run a single-key Command on the server
-        *   \param cmd The single-key Comand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The single-key Command to run
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(SingleKeyCommand& cmd);
 
         /*!
         *   \brief Run a multi-key Command on the server
-        *   \param cmd The multi-key Comand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The multi-key Command to run
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(MultiKeyCommand& cmd);
 
         /*!
         *   \brief Run a compound Command on the server
-        *   \param cmd The compound Comand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The compound Command to run
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(CompoundCommand& cmd);
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses the given db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses the given db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses the given db node
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAtCommand& cmd);
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses any db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses any db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses any db node
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAnyCommand& cmd);
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses every db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses any db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses all db nodes
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAllCommand& cmd);
 
         /*!
         *   \brief Run multiple single-key or single-hash slot
         *          Command on the server.  Each Command in the
         *          CommandList is run sequentially.
-        *   \param cmd The CommandList containing multiple
-        *              single-key or single-hash
-        *              slot Command to run
+        *   \param cmd The CommandList containing multiple single-key or
+        *              single-hash slot Command to run
         *   \returns A list of CommandReply for each Command
         *            in the CommandList
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual std::vector<CommandReply> run(CommandList& cmd);
 
         /*!
         *   \brief Run multiple single-key or single-hash slot
         *          Command on the server in pipelines.  The
         *          Command in the CommandList will be grouped
         *          by shard, and executed in groups by shard.
         *          Commands are not guaranteed to be executed
         *          in any sequence or ordering.
-        *   \param cmd The CommandList containing multiple
-        *              single-key or single-hash
-        *              slot Command to run
+        *   \param cmd_list The CommandList containing multiple single-key
+        *                   or single-hash slot Commands to run
         *   \returns A list of CommandReply for each Command
         *            in the CommandList. The order of the result
         *            matches the order of the input CommandList.
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual PipelineReply
         run_via_unordered_pipelines(CommandList& cmd_list);
 
         /*!
-        *   \brief Check if a key exists in the database. This
-        *          function does not work for models and scripts.
-        *          For models and scripts, model_key_exists should
-        *          be used.
+        *   \brief Check if a key exists in the database. This function does
+        *          not work for models and scripts. For models and scripts,
+        *          model_key_exists should be used.
         *   \param key The key to check
         *   \returns True if the key exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool key_exists(const std::string& key);
 
         /*!
         *   \brief Check if a hash field exists
         *   \param key The key containing the field
         *   \param field The field in the key to check
         *   \returns True if the hash field exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool hash_field_exists(const std::string& key,
                                        const std::string& field);
 
         /*!
         *   \brief Check if a model or script key exists in the database
         *   \param key The key to check
         *   \returns True if the key exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool model_key_exists(const std::string& key);
 
         /*!
          *  \brief Check if address is valid
-         *  \param address address of database
-         *  \param port port of database
+         *  \param address Address (TCP or UDS) of database
          *  \return True if address is valid
          */
-        virtual bool is_addressable(const std::string& address, const uint64_t& port);
+        virtual bool is_addressable(const SRAddress& address) const;
 
         /*!
         *   \brief Put a Tensor on the server
         *   \param tensor The Tensor to put on the server
         *   \returns The CommandReply from the put tensor
         *            command execution
+        *   \throw SmartRedis::Exception if tensor storage fails
         */
         virtual CommandReply put_tensor(TensorBase& tensor);
 
         /*!
         *   \brief Get a Tensor from the server
         *   \param key The name of the tensor to retrieve
         *   \returns The CommandReply from the get tensor server
         *            command execution
+        *   \throw SmartRedis::Exception if tensor retrieval fails
         */
         virtual CommandReply get_tensor(const std::string& key);
 
         /*!
+        *   \brief Get a list of Tensor from the server. All tensors
+        *          must be on the same node
+        *   \param keys The keys of the tensor to retrieve
+        *   \returns The PipelineReply from executing the get tensor commands
+        *   \throw SmartRedis::Exception if tensor retrieval fails
+        */
+        virtual PipelineReply get_tensors(
+            const std::vector<std::string>& keys);
+
+    /*!
         *   \brief Rename a tensor in the database
         *   \param key The original key for the tensor
         *   \param new_key The new key for the tensor
         *   \returns The CommandReply from the last Command
         *            execution in the renaming of the tensor.
         *            In the case of RedisCluster, this is
         *            the reply for the final delete_tensor call.
+        *   \throw SmartRedis::Exception if tensor rename fails
         */
         virtual CommandReply rename_tensor(const std::string& key,
                                            const std::string& new_key);
 
         /*!
         *   \brief Delete a tensor in the database
         *   \param key The database key for the tensor
         *   \returns The CommandReply from delete command
         *            executed on the server
+        *   \throw SmartRedis::Exception if tensor removal fails
         */
         virtual CommandReply delete_tensor(const std::string& key);
 
         /*!
         *   \brief Copy a tensor from the source key to
         *          the destination key
         *   \param src_key The source key for the tensor copy
         *   \param dest_key The destination key for the tensor copy
         *   \returns The CommandReply from the last Command
         *            execution in the copying of the tensor.
         *            In the case of RedisCluster, this is
         *            the CommandReply from a put_tensor commands.
+        *   \throw SmartRedis::Exception if tensor copy fails
         */
         virtual CommandReply copy_tensor(const std::string& src_key,
                                          const std::string& dest_key);
 
         /*!
         *   \brief Copy a vector of tensors from source keys
         *          to destination keys
         *   \param src Vector of source keys
         *   \param dest Vector of destination keys
         *   \returns The CommandReply from the last Command
         *            execution in the copying of the tensor.
         *            Different implementations may have different
         *            sequences of commands.
+        *   \throw SmartRedis::Exception if tensor copy fails
         */
         virtual CommandReply copy_tensors(const std::vector<std::string>& src,
                                           const std::vector<std::string>& dest);
 
         /*!
         *   \brief Set a model from std::string_view buffer in the
         *          database for future execution
@@ -289,14 +305,15 @@
         *   \param tag A tag to attach to the model for
         *              information purposes
         *   \param inputs One or more names of model input nodes
         *                 (TF models only)
         *   \param outputs One or more names of model output nodes
         *                 (TF models only)
         *   \returns The CommandReply from the set_model Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply set_model(const std::string& key,
                                        std::string_view model,
                                        const std::string& backend,
                                        const std::string& device,
                                        int batch_size = 0,
                                        int min_batch_size = 0,
@@ -343,14 +360,15 @@
         *   \brief Set a script from std::string_view buffer in the
         *          database for future execution
         *   \param key The key to associate with the script
         *   \param device The name of the device for execution
         *                 (e.g. CPU or GPU)
         *   \param script The script source in a std::string_view
         *   \returns The CommandReply from set_script Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply set_script(const std::string& key,
                                         const std::string& device,
                                         std::string_view script);
 
         /*!
         *   \brief Set a script from std::string_view buffer in the
@@ -366,20 +384,19 @@
                                          int first_gpu,
                                          int num_gpus);
 
         /*!
         *   \brief Run a model in the database using the
         *          specified input and output tensors
         *   \param key The key associated with the model
-        *   \param inputs The keys of inputs tensors to use
-        *                 in the model
+        *   \param inputs The keys of inputs tensors to use in the model
         *   \param outputs The keys of output tensors that
         *                 will be used to save model results
-        *   \returns The CommandReply from the run model server
-        *            Command
+        *   \returns The CommandReply from the run model server Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply run_model(const std::string& key,
                                        std::vector<std::string> inputs,
                                        std::vector<std::string> outputs);
 
         /*!
         *   \brief Run a model in the database using the
@@ -406,16 +423,16 @@
         *          specified input and output tensors
         *   \param key The key associated with the script
         *   \param function The name of the function in the script to run
         *   \param inputs The keys of inputs tensors to use
         *                 in the script
         *   \param outputs The keys of output tensors that
         *                 will be used to save script results
-        *   \returns The CommandReply from script run Command
-        *            execution
+        *   \returns The CommandReply from script run Command execution
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply run_script(const std::string& key,
                                         const std::string& function,
                                         std::vector<std::string> inputs,
                                         std::vector<std::string> outputs);
 
         /*!
@@ -448,15 +465,15 @@
         */
         CommandReply delete_model(const std::string& key);
 
         /*!
         *   \brief Remove a model from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the model
-        *   \param first_cpu the first GPU (zero-based) to use with the model
+        *   \param first_gpu the first GPU (zero-based) to use with the model
         *   \param num_gpus the number of gpus for which the model was stored
         *   \throw SmartRedis::Exception if model deletion fails
         */
         virtual void delete_model_multigpu(
             const std::string& name, int first_gpu, int num_gpus);
 
         /*!
@@ -467,51 +484,69 @@
         */
         CommandReply delete_script(const std::string& key);
 
         /*!
         *   \brief Remove a script from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the script
-        *   \param first_cpu the first GPU (zero-based) to use with the script
+        *   \param first_gpu the first GPU (zero-based) to use with the script
         *   \param num_gpus the number of gpus for which the script was stored
         *   \throw SmartRedis::Exception if script deletion fails
         */
         virtual void delete_script_multigpu(
             const std::string& name, int first_gpu, int num_gpus);
 
         /*!
         *   \brief Retrieve the model from the database
         *   \param key The key associated with the model
         *   \returns The CommandReply that contains the result
         *            of the get model execution on the server
+        *   \throw SmartRedis::Exception if model retrieval fails
         */
         virtual CommandReply get_model(const std::string& key);
 
         /*!
         *   \brief Retrieve the script from the database
         *   \param key The key associated with the script
         *   \returns The CommandReply that contains the result
         *            of the get script execution on the server
+        *   \throw SmartRedis::Exception if script retrieval fails
         */
         virtual CommandReply get_script(const std::string& key);
 
         /*!
         *   \brief Retrieve model/script runtime statistics
         *   \param address The address of the database node (host:port)
         *   \param key The key associated with the model or script
         *   \param reset_stat Boolean indicating if the counters associated
         *                     with the model or script should be reset.
         *   \returns The CommandReply that contains the result
         *            of the AI.INFO execution on the server
+        *   \throw SmartRedis::Exception if info retrieval fails
         */
         virtual CommandReply
         get_model_script_ai_info(const std::string& address,
                                  const std::string& key,
                                  const bool reset_stat);
 
+        /*!
+        *   \brief Run a CommandList via a Pipeline.
+        *          All commands must go to the same shard
+        *   \param cmdlist The list of commands to run
+        *   \returns The PipelineReply with the result of command execution
+        *   \throw SmartRedis::Exception if execution fails
+        */
+        PipelineReply run_in_pipeline(CommandList& cmdlist);
+
+        /*!
+        *   \brief Create a string representation of the Redis connection
+        *   \returns A string representation of the Redis connection
+        */
+        virtual std::string to_string() const;
+
     protected:
 
         /*!
         *   \brief Get a DBNode prefix for the provided hash slot
         *   \param hash_slot The hash slot to get a prefix for
         *   \throw RuntimeException if there is an error
         *          creating a prefix for a particular hash slot
@@ -537,30 +572,29 @@
         std::string _last_prefix;
 
         /*!
         *   \brief Run the command on the correct db node
         *   \param cmd The command to run on the server
         *   \param db_prefix The prefix of the db node the
         *                    command addresses
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         inline CommandReply _run(const Command& cmd, std::string db_prefix);
 
         /*!
         *   \brief Connect to the cluster at the address and port
-        *   \param address_port A string formatted as
-        *                       tcp:://address:port
-        *                       for redis connection
+        *   \param db_address The server address
+        *   \throw SmartRedis::Exception if connection fails
         */
-        inline void _connect(std::string address_port);
+        inline void _connect(SRAddress& db_address);
 
         /*!
-        *   \brief Map the RedisCluster via the CLUSTER SLOTS
-        *          command.
+        *   \brief Map the RedisCluster via the CLUSTER SLOTS command.
+        *   \throw SmartRedis::Exception if the command fails
         */
         inline void _map_cluster();
 
         /*!
         *   \brief Get the prefix that can be used to address
         *          the correct database for a given command
         *   \param cmd The Command to analyze for DBNode prefix
@@ -673,24 +707,26 @@
                                                  std::string db_prefix);
 
         /*!
         *   \brief  Delete multiple keys with the assumption that all
         *           keys use the same hash slot
         *   \param keys The keys to be deleted
         *   \returns A vector of updated names
+        *   \throw SmartRedis::Exception deletion fails
         */
         void _delete_keys(std::vector<std::string> keys);
 
         /*!
         *   \brief  Run a model in the database that uses dagrun
         *   \param key The key associated with the model
         *   \param inputs The keys of inputs tensors to use
         *                 in the model
         *   \param outputs The keys of output tensors that
         *                 will be used to save model results
+        *   \throw SmartRedis::Exception execution fails
         */
         void __run_model_dagrun(const std::string& key,
                                 std::vector<std::string> inputs,
                                 std::vector<std::string> outputs);
 
         /*!
         *   \brief  Retrieve the optimum model prefix for
@@ -713,15 +749,16 @@
         *   \param shard_prefix The prefix corresponding to the shard
         *                       where the pipeline is executed
         *   \throw SmartRedis::Exception if an error is encountered following
         *          multiple attempts
         *   \return A PipelineReply for the provided commands.  The
         *           PipelineReply will be in the same order as the provided
         *           Command vector.
+        *   \throw SmartRedis::Exception if pipelined execution fails
         */
         PipelineReply _run_pipeline(std::vector<Command*>& cmds,
                                     std::string& shard_prefix);
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_CPP_CLUSTER_H
+#endif // SMARTREDIS_REDISCLUSTER_H
```

### Comparing `smartredis-0.3.1/include/redisserver.h` & `smartredis-0.4.0/include/redisserver.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,22 +22,21 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef SMARTREDIS_CPP_REDISSERVER_H
-#define SMARTREDIS_CPP_REDISSERVER_H
+#ifndef SMARTREDIS_REDISSERVER_H
+#define SMARTREDIS_REDISSERVER_H
 
 #include <thread>
 #include <iostream>
 #include <random>
-#include "limits.h"
-
+#include <limits.h>
 #include <sw/redis++/redis++.h>
 
 #include "command.h"
 #include "commandreply.h"
 #include "commandlist.h"
 #include "tensorbase.h"
 #include "dbnode.h"
@@ -50,214 +49,230 @@
 #include "addressanycommand.h"
 #include "addressallcommand.h"
 #include "clusterinfocommand.h"
 #include "dbinfocommand.h"
 #include "gettensorcommand.h"
 #include "pipelinereply.h"
 #include "threadpool.h"
+#include "address.h"
 
 ///@file
 
 namespace SmartRedis {
 
-class RedisServer;
-
+class SRObject;
 
 /*!
 *   \brief Abstract class that defines interface for
 *          objects that execute commands on server.
 */
 class RedisServer {
 
     public:
 
         /*!
         *   \brief Default constructor
+        *   \param context The owning context
+        *   \throw SmartRedis::Exception if connection fails
         */
-        RedisServer();
+        RedisServer(const SRObject* context);
 
         /*!
         *   \brief Destructor
         */
         virtual ~RedisServer();
 
         /*!
         *   \brief Run a single-key Command on the server
-        *   \param cmd The single-key Comand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The single-key Command to run
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(SingleKeyCommand& cmd) = 0;
 
         /*!
         *   \brief Run a multi-key Command on the server
-        *   \param cmd The multi-key Comand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The multi-key Command to run
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(MultiKeyCommand& cmd) = 0;
 
         /*!
         *   \brief Run a compound Command on the server
-        *   \param cmd The compound Comand to run
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The compound Command to run
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(CompoundCommand& cmd) = 0;
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses the given db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses the given db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses the given db node
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAtCommand& cmd) = 0;
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses any db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses any db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses any db node
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAnyCommand& cmd) = 0;
 
         /*!
         *   \brief Run a non-keyed Command that
         *          addresses every db node on the server
-        *   \param cmd The non-keyed Command that
-        *              addresses any db node
-        *   \returns The CommandReply from the
-        *            command execution
+        *   \param cmd The non-keyed Command that addresses all db nodes
+        *   \returns The CommandReply from the command execution
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual CommandReply run(AddressAllCommand& cmd) = 0;
 
         /*!
         *   \brief Run multiple single-key or single-hash slot
         *          Command on the server.  Each Command in the
         *          CommandList is run sequentially.
-        *   \param cmd The CommandList containing multiple
-        *              single-key or single-hash
-        *              slot Comand to run
-        *   \returns A list of CommandReply for each Command
-        *            in the CommandList
+        *   \param cmd The CommandList containing multiple single-key or
+        *              single-hash slot Comand to run
+        *   \returns A list of CommandReply for each Command in the CommandList
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual std::vector<CommandReply> run(CommandList& cmd) = 0;
 
         /*!
         *   \brief Run multiple single-key or single-hash slot
         *          Command on the server in pipelines.  The
         *          Command in the CommandList will be grouped
         *          by shard, and executed in groups by shard.
         *          Commands are not guaranteed to be executed
         *          in any sequence or ordering.
-        *   \param cmd The CommandList containing multiple
-        *              single-key or single-hash
-        *              slot Command to run
+        *   \param cmd_list The CommandList containing multiple single-key
+        *                   or single-hash slot Command to run
         *   \returns A list of CommandReply for each Command
         *            in the CommandList. The order of the result
         *            matches the order of the input CommandList.
+        *   \throw SmartRedis::Exception if command execution fails
         */
         virtual PipelineReply
         run_via_unordered_pipelines(CommandList& cmd_list) = 0;
 
         /*!
         *   \brief Check if a key exists in the database
         *   \param key The key to check
         *   \returns True if the key exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool key_exists(const std::string& key) = 0;
 
         /*!
         *   \brief Check if a hash field exists
         *   \param key The key containing the field
         *   \param field The field in the key to check
         *   \returns True if the hash field exists, otherwise False
+        *   \throw SmartRedis::Exception if existence check fails
         */
         virtual bool hash_field_exists(const std::string& key,
                                        const std::string& field) = 0;
 
         /*!
          *  \brief Check if a model or script exists in the database
          *  \param key The script or model key
          *  \return True if the model or script exists
+        *   \throw SmartRedis::Exception if existence check fails
          */
         virtual bool model_key_exists(const std::string& key) = 0;
 
         /*!
-         *  \brief Check if address and port maps to database node
-         *  \param address address of database
-         *  \param port port of database
+         *  \brief Check if address is valid
+         *  \param address Address (TCP or UDS) of database
          *  \return True if address is valid
          */
-        virtual bool is_addressable(const std::string& address, const uint64_t& port) = 0;
+        virtual bool is_addressable(const SRAddress& address) const = 0;
 
         /*!
         *   \brief Put a Tensor on the server
         *   \param tensor The Tensor to put on the server
         *   \returns The CommandReply from the put tensor
         *            command execution
+        *   \throw SmartRedis::Exception if tensor storage fails
         */
         virtual CommandReply put_tensor(TensorBase& tensor) = 0;
 
         /*!
         *   \brief Get a Tensor from the server
         *   \param key The name of the tensor to retrieve
         *   \returns The CommandReply from the get tensor server
         *            command execution
+        *   \throw SmartRedis::Exception if tensor retrieval fails
         */
         virtual CommandReply get_tensor(const std::string& key) = 0;
 
         /*!
+        *   \brief Get a list of Tensor from the server. For clustered
+        *          servers, all tensors must be on the same node
+        *   \param keys The keys of the tensor to retrieve
+        *   \returns The PipelineReply from executing the get tensor commands
+        *   \throw SmartRedis::Exception if tensor retrieval fails
+        */
+        virtual PipelineReply get_tensors(
+            const std::vector<std::string>& keys) = 0;
+
+        /*!
         *   \brief Rename a tensor in the database
         *   \param key The original key for the tensor
         *   \param new_key The new key for the tensor
         *   \returns The CommandReply from the last Command
         *            execution in the renaming of the tensor.
         *            Different implementations may have different
         *            sequences of commands.
+        *   \throw SmartRedis::Exception if tensor rename fails
         */
         virtual CommandReply rename_tensor(const std::string& key,
                                            const std::string& new_key)
                                            = 0;
 
         /*!
         *   \brief Delete a tensor in the database
         *   \param key The database key for the tensor
         *   \returns The CommandReply from delete command
         *            executed on the server
+        *   \throw SmartRedis::Exception if tensor removal fails
         */
         virtual CommandReply delete_tensor(const std::string& key) = 0;
 
         /*!
         *   \brief Copy a tensor from the source key to
         *          the destination key
         *   \param src_key The source key for the tensor copy
         *   \param dest_key The destination key for the tensor copy
         *   \returns The CommandReply from the last Command
         *            execution in the copying of the tensor.
         *            Different implementations may have different
         *            sequences of commands.
+        *   \throw SmartRedis::Exception if tensor copy fails
         */
         virtual CommandReply copy_tensor(const std::string& src_key,
                                          const std::string& dest_key)
                                          = 0;
 
         /*!
         *   \brief Copy a vector of tensors from source keys
         *          to destination keys
         *   \param src Vector of source keys
         *   \param dest Vector of destination keys
         *   \returns The CommandReply from the last Command
         *            execution in the copying of the tensor.
         *            Different implementations may have different
         *            sequences of commands.
+        *   \throw SmartRedis::Exception if tensor copy fails
         */
         virtual CommandReply copy_tensors(const std::vector<std::string>& src,
                                           const std::vector<std::string>& dest
                                           ) = 0;
 
         /*!
         *   \brief Set a model from std::string_view buffer in the
@@ -274,14 +289,15 @@
         *   \param tag A tag to attach to the model for
         *              information purposes
         *   \param inputs One or more names of model input nodes
         *                 (TF models only)
         *   \param outputs One or more names of model output nodes
         *                 (TF models only)
         *   \returns The CommandReply from the set_model Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply set_model(const std::string& key,
                                        std::string_view model,
                                        const std::string& backend,
                                        const std::string& device,
                                        int batch_size = 0,
                                        int min_batch_size = 0,
@@ -329,14 +345,15 @@
         *   \brief Set a script from std::string_view buffer in the
         *          database for future execution
         *   \param key The key to associate with the script
         *   \param device The name of the device for execution
         *                 (e.g. CPU or GPU)
         *   \param script The script source in a std::string_view
         *   \returns The CommandReply from set_script Command
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply set_script(const std::string& key,
                                         const std::string& device,
                                         std::string_view script) = 0;
 
         /*!
         *   \brief Set a script from std::string_view buffer in the
@@ -360,14 +377,15 @@
         *                 in the model
         *   \param outputs The keys of output tensors that
         *                 will be used to save model results
         *   \returns The CommandReply from a Command
         *            execution in the model run execution.
         *            Different implementations may have different
         *            sequences of commands.
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply run_model(const std::string& key,
                                        std::vector<std::string> inputs,
                                        std::vector<std::string> outputs) = 0;
 
         /*!
         *   \brief Run a model in the database using the
@@ -398,14 +416,15 @@
         *                 in the script
         *   \param outputs The keys of output tensors that
         *                 will be used to save script results
         *   \returns The CommandReply from a Command
         *            execution in the script run execution.
         *            Different implementations may have different
         *            sequences of commands.
+        *   \throw RuntimeException for all client errors
         */
         virtual CommandReply run_script(const std::string& key,
                                         const std::string& function,
                                         std::vector<std::string> inputs,
                                         std::vector<std::string> outputs)
                                          = 0;
 
@@ -439,15 +458,15 @@
         */
         virtual CommandReply delete_model(const std::string& key) = 0;
 
         /*!
         *   \brief Remove a model from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the model
-        *   \param first_cpu the first GPU (zero-based) to use with the model
+        *   \param first_gpu the first GPU (zero-based) to use with the model
         *   \param num_gpus the number of gpus for which the model was stored
         *   \throw SmartRedis::Exception if model deletion fails
         */
         virtual void delete_model_multigpu(
             const std::string& name, int first_gpu, int num_gpus) = 0;
 
         /*!
@@ -458,51 +477,69 @@
         */
         virtual CommandReply delete_script(const std::string& key) = 0;
 
         /*!
         *   \brief Remove a script from the database that was stored
         *          for use with multiple GPUs
         *   \param name The name associated with the script
-        *   \param first_cpu the first GPU (zero-based) to use with the script
+        *   \param first_gpu the first GPU (zero-based) to use with the script
         *   \param num_gpus the number of gpus for which the script was stored
         *   \throw SmartRedis::Exception if script deletion fails
         */
         virtual void delete_script_multigpu(
             const std::string& name, int first_gpu, int num_gpus) = 0;
 
         /*!
         *   \brief Retrieve the model from the database
         *   \param key The key associated with the model
         *   \returns The CommandReply that contains the result
         *            of the get model execution on the server
+        *   \throw SmartRedis::Exception if model retrieval fails
         */
         virtual CommandReply get_model(const std::string& key) = 0;
 
         /*!
         *   \brief Retrieve the script from the database
         *   \param key The key associated with the script
         *   \returns The CommandReply that contains the result
         *            of the get script execution on the server
+        *   \throw SmartRedis::Exception if script retrieval fails
         */
         virtual CommandReply get_script(const std::string& key) = 0;
 
         /*!
         *   \brief Retrieve model/script runtime statistics
-        *   \param address The address of the database node (host:port)
+        *   \param address The TCP or UDS address of the database node
         *   \param key The key associated with the model or script
         *   \param reset_stat Boolean indicating if the counters associated
         *                     with the model or script should be reset.
         *   \returns The CommandReply that contains the result
         *            of the AI.INFO execution on the server
+        *   \throw SmartRedis::Exception if info retrieval fails
         */
         virtual CommandReply
         get_model_script_ai_info(const std::string& address,
                                  const std::string& key,
                                  const bool reset_stat) = 0;
 
+        /*!
+        *   \brief Run a CommandList via a Pipeline. For clustered databases
+        *          all commands must go to the same shard
+        *   \param cmdlist The list of commands to run
+        *   \returns The PipelineReply with the result of command execution
+        *   \throw SmartRedis::Exception if execution fails
+        */
+        virtual PipelineReply run_in_pipeline(CommandList& cmdlist) = 0;
+
+        /*!
+        *   \brief Create a string representation of the Redis connection
+        *   \returns A string representation of the Redis connection
+        */
+        virtual std::string to_string() const = 0;
+
     protected:
 
         /*!
         *   \brief Timeout (in seconds) of connection attempt(s).
         */
         int _connection_timeout;
 
@@ -559,14 +596,19 @@
 
         /*!
         *   \brief Default number of threads for thread pool
         */
         static constexpr int _DEFAULT_THREAD_COUNT = 4;
 
         /*!
+        *   \brief The owning context
+        */
+        const SRObject* _context;
+
+        /*!
         *   \brief Seeding for the random number engine
         */
         std::random_device _rd;
 
         /*!
         *   \brief Random number generator
         */
@@ -579,14 +621,21 @@
 
         /*!
         *   \brief The thread pool
         */
         ThreadPool *_tp;
 
         /*!
+        *   \brief Indicates whether the server was connected to
+        *          via a Unix domain socket (true) or TCP connection
+        *          (false)
+        */
+        bool _is_domain_socket;
+
+        /*!
         *   \brief Environment variable for connection timeout
         */
         inline static const std::string _CONN_TIMEOUT_ENV_VAR =
             "SR_CONN_TIMEOUT";
 
         /*!
         *   \brief Environment variable for connection interval
@@ -619,51 +668,32 @@
             "SR_THREAD_COUNT";
 
         /*!
         *   \brief Retrieve a single address, randomly
         *          chosen from a list of addresses if
         *          applicable, from the SSDB environment
         *          variable.
-        *   \returns A address and port pair in the form of
-        *            address:port
+        *   \returns An SRAddress representing the selected server address
         */
-        std::string _get_ssdb();
+        SRAddress _get_ssdb();
 
         /*!
-        *   \brief Unordered map of address:port to DBNode in the cluster
+        *   \brief Unordered map of server address string to DBNode in the cluster
         */
         std::unordered_map<std::string, DBNode*> _address_node_map;
 
         /*!
         *   \brief Check that the SSDB environment variable
         *          value does not have any errors
         *   \throw RuntimeException if there is an error
         *          in SSDB environment variable format
         */
         void _check_ssdb_string(const std::string& env_str);
 
         /*!
-        *   \brief Initialize a variable of type integer from an environment
-        *          variable.  If the environment variable is not set,
-        *          the default value is assigned.
-        *   \param value Reference to a integer value which will be assigned
-        *                a default value or environment variable value
-        *   \param env_var std::string of the environment variable name
-        *   \param default_value The default value to assign if the environment
-        *                        variable is not set.
-        *   \throw SmartRedis::RuntimeException if environment variable
-        *          retrieval fails, conversion to integer fails, or
-        *          if the value of the environment value contains
-        *          characters other than [0,9] or a negative sign ('-').
-        */
-        void _init_integer_from_env(int& value,
-                                    const std::string& env_var,
-                                    const int& default_value);
-
-        /*!
         *   \brief This function checks that _connection_timeout,
         *          _connection_interval, _command_timeout, and
         *          _command_interval, which have been set from environment
         *          variables, are within valid ranges.
         *   \throw SmartRedis::RuntimeException if any of the runtime
         *          settings is outside of the allowable range
         */
@@ -679,8 +709,8 @@
             return (((value % modulus) + modulus) % modulus);
          }
 
 };
 
 } // namespace SmartRedis
 
-#endif //SMARTREDIS_CPP_REDISSERVER_H
+#endif // SMARTREDIS_REDISSERVER_H
```

### Comparing `smartredis-0.3.1/include/scalarfield.h` & `smartredis-0.4.0/include/scalarfield.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -27,14 +27,17 @@
  */
 
 #ifndef SMARTREDIS_SCALARFIELD_H
 #define SMARTREDIS_SCALARFIELD_H
 
 #include "metadatafield.h"
 #include <iostream>
+
+///@file
+
 namespace SmartRedis {
 
 /*!
 *   \brief  The ScalarField class implements
 *   MetadataField class methods needed for
 *   storage and transfer of metadata scalar
 *   fields (e.g. double, float, int64, etc.)
@@ -116,15 +119,15 @@
         */
         void append(const void* value);
 
         /*!
         *   \brief Retrieve the number of values in the field
         *   \returns The number of values
         */
-        virtual size_t size();
+        virtual size_t size() const;
 
         /*!
         *   \brief Clear the values in the field
         */
         virtual void clear();
 
         /*!
@@ -150,10 +153,10 @@
         */
         std::vector<T> _vals;
 
 };
 
 #include "scalarfield.tcc"
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_SCALARFIELD_H
+#endif // SMARTREDIS_SCALARFIELD_H
```

### Comparing `smartredis-0.3.1/include/scalarfield.tcc` & `smartredis-0.4.0/include/scalarfield.tcc`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -71,15 +71,15 @@
 {
     if (value != NULL)
         _vals.push_back(*((T*)value));
 }
 
 // Retrieve the number of values in a scalar
 template <class T>
-size_t ScalarField<T>::size()
+size_t ScalarField<T>::size() const
 {
     return _vals.size();
 }
 
 // Clear out all values from a scalar
 template <class T>
 void ScalarField<T>::clear()
@@ -97,8 +97,8 @@
 // Retrieve a pointer to the underlying value structure
 template <class T>
 const std::vector<T>& ScalarField<T>::immutable_values()
 {
     return _vals;
 }
 
-#endif //SMARTREDIS_SCALARFIELD_TCC
+#endif // SMARTREDIS_SCALARFIELD_TCC
```

### Comparing `smartredis-0.3.1/include/sharedmemorylist.h` & `smartredis-0.4.0/include/sharedmemorylist.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -30,14 +30,16 @@
 #define SMARTREDIS_SHAREDMEMORYLIST_H
 
 #include <forward_list>
 #include <cstring>
 #include <memory>
 #include "srexception.h"
 
+///@file
+
 namespace SmartRedis {
 
 /*!
 *   \brief  The SharedMemoryList class allocates
 *           and manages memory of type T.
 *   \details This class is useful for repeated
 *            allocations of ype T that need to be
@@ -118,11 +120,10 @@
     */
     typename std::forward_list<std::shared_ptr<T>> _inventory;
 
 };
 
 #include "sharedmemorylist.tcc"
 
-} //namespace SmartRedis
-
-#endif //SMARTREDIS_SHAREDMEMORYLIST_H
+} // namespace SmartRedis
 
+#endif // SMARTREDIS_SHAREDMEMORYLIST_H
```

### Comparing `smartredis-0.3.1/include/sharedmemorylist.tcc` & `smartredis-0.4.0/include/sharedmemorylist.tcc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -55,8 +55,8 @@
 template <class T>
 T* SharedMemoryList<T>::allocate(size_t n_values)
 {
     size_t bytes = n_values * sizeof(T);
     return allocate_bytes(bytes);
 }
 
-#endif //SMARTREDIS_SHAREDMEMORYLIST_TCC
+#endif // SMARTREDIS_SHAREDMEMORYLIST_TCC
```

### Comparing `smartredis-0.3.1/include/singlekeycommand.h` & `smartredis-0.4.0/include/singlekeycommand.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -64,10 +64,10 @@
         *   \returns A pointer to dynamically allocated
         *            derived type cast to parent Command
         *            type.
         */
         virtual Command* clone();
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SINGLEKEYCOMMAND
+#endif // SMARTREDIS_SINGLEKEYCOMMAND_H
```

### Comparing `smartredis-0.3.1/include/sr_enums.h` & `smartredis-0.4.0/include/sr_enums.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -23,16 +23,16 @@
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 
-#ifndef SMARTREDIS_ENUMS_H
-#define SMARTREDIS_ENUMS_H
+#ifndef SMARTREDIS_SR_ENUMS_H
+#define SMARTREDIS_SR_ENUMS_H
 
 ///@file
 
 /*!
 *   \brief  Enumeration for memory layout of tensor data
 */
 typedef enum {
@@ -68,8 +68,19 @@
     SRTensorTypeInt16   = 4, // 16-bit signed integer tensor type
     SRTensorTypeInt32   = 5, // 32-bit signed integer tensor type
     SRTensorTypeInt64   = 6, // 64-bit signed integer tensor type
     SRTensorTypeUint8   = 7, // 8-bit unsigned integer tensor type
     SRTensorTypeUint16  = 8  // 16-bit unsigned integer tensor type
 } SRTensorType;
 
-#endif // SMARTREDIS_ENUMS_H
+/*!
+*   \brief  Enumeration for logging levels
+*/
+typedef enum {
+    LLInvalid   = 0, // Invalid or uninitialized logging level
+    LLQuiet     = 1, // No logging at all
+    LLInfo      = 2, // Informational logging only
+    LLDebug     = 3, // Verbose logging for debugging purposes
+    LLDeveloper = 4  // Extra verbose logging for internal use
+} SRLoggingLevel;
+
+#endif // SMARTREDIS_SR_ENUMS_H
```

### Comparing `smartredis-0.3.1/include/srassert.h` & `smartredis-0.4.0/include/srassert.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,16 +22,16 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef SMARTREDIS_ASSERT_H
-#define SMARTREDIS_ASSERT_H
+#ifndef SMARTREDIS_SRASSERT_H
+#define SMARTREDIS_SRASSERT_H
 
 #include "srexception.h"
 
 using namespace SmartRedis;
 
 ///@file
 
@@ -72,8 +72,8 @@
 
 /*!
 *   \brief Validate a parameter list (via a boolean condition) or throw a RuntimeException
 */
 #define SR_CHECK_PARAMS(condition) \
     ((condition) || throw_param_exception(std::string("Assertion failed!") + #condition, __FILE__, __LINE__))
 
-#endif // SMARTREDIS_ASSERT_H
+#endif // SMARTREDIS_SRASSERT_H
```

### Comparing `smartredis-0.3.1/include/srexception.h` & `smartredis-0.4.0/include/srexception.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -22,19 +22,21 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef SMARTREDIS_SRException_H
-#define SMARTREDIS_SRException_H
+#ifndef SMARTREDIS_SREXCEPTION_H
+#define SMARTREDIS_SREXCEPTION_H
 
 #include <stdio.h>
 #include <stdlib.h>
+#include "sr_enums.h"
+#include "logger.h"
 
 ///@file
 
 /*!
 *   \brief  SRError lists possible errors encountered in SmartRedis.
 */
 typedef enum {
@@ -46,66 +48,97 @@
     SRParameterError = 5, // Bad parameter error
     SRTimeoutError   = 6, // Timeout error
     SRKeyError       = 7, // Key error
     SRInvalidError   = 8, // Uninitialized error variable
     SRTypeError      = 9  // Type mismatch
 } SRError;
 
+#ifdef __cplusplus
+namespace SmartRedis {
+class Exception;
+}
+#endif // __cplusplus
 
 /*!
 *   \brief Return the last error encountered
 *   \return The text data for the last error encountered
 */
 #ifdef __cplusplus
 extern "C"
 #endif
 const char* SRGetLastError();
 
+/*!
+*   \brief Return the location for the last error encountered
+*   \return The text data for the last error's location
+*/
+#ifdef __cplusplus
+extern "C"
+#endif
+const char* SRGetLastErrorLocation();
+
 #ifdef __cplusplus
 #include <string>
 namespace SmartRedis {
 
 /*!
+*   \brief Store the last error encountered in a global variable. Not
+*          currently thread-safe
+*   \param last_error Exception to be stored as the last error encountered
+*/
+extern "C"
+void SRSetLastError(const Exception& last_error);
+
+
+/*!
 *   \brief  Smart error: custom exception class for the SmartRedis library
 */
 class Exception: public std::exception
 {
     public:
     /*!
     *   \brief Exception default constructor
     *   \param what_arg The message for the exception
     */
     Exception(const char* what_arg)
-      : _msg(what_arg)
+      : _msg(what_arg), _loc("unavailable")
     {
-        // NOP
+        SRSetLastError(*this);
     }
 
     /*!
     *   \brief Exception constructor with location information
     *   \param what_arg The message for the exception
     *   \param file The source file from which the exception was thrown
     *   \param line The line number from which the exception was thrown
     */
     Exception(const char* what_arg, const char* file, int line)
-      : _msg(what_arg), _loc(file + std::string(":") + std::to_string(line))
+      : _msg(what_arg),
+        _loc(std::string("\"") + file + std::string("\", line ") + std::to_string(line))
     {
-        // NOP
+        SRSetLastError(*this);
+        log_error(
+            "SmartRedis Library", LLInfo,
+            exception_class() + " at " + _loc + ": " + _msg);
     }
 
     /*!
     *   \brief Exception constructor with location information
     *   \param what_arg The message for the exception
     *   \param file The source file from which the exception was thrown
     *   \param line The line number from which the exception was thrown
     */
     Exception(const std::string& what_arg, const char* file, int line)
-      : _msg(what_arg), _loc(file + std::string(":") + std::to_string(line))
+      : _msg(what_arg),
+        _loc(std::string("\"") + file + std::string("\", line ") + std::to_string(line))
     {
-        // NOP
+        SRSetLastError(*this);
+        log_error(
+            "SmartRedis Library", LLInfo,
+            exception_class() + " at " + _loc + ": " + _msg);
     }
 
     /*!
     *   \brief Exception copy constructor
     *   \param other Exception to copy
     */
     Exception(const Exception& other) noexcept
@@ -152,14 +185,22 @@
     *   \returns Error code corresponding to the exception type
     */
     virtual SRError to_error_code() const noexcept {
         return SRInvalidError;
     }
 
     /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("Exception");
+    }
+
+    /*!
     *   \brief Retrieve the message for an exception
     *   \returns String of message data
     */
     const char* what() const noexcept override {
         return _msg.c_str();
     }
 
@@ -187,23 +228,32 @@
 
 /*!
 *   \brief  Memory allocation exception for SmartRedis
 */
 class BadAllocException: public Exception
 {
     public:
+
     using Exception::Exception;
 
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRBadAllocError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("BadAllocException");
+    }
 };
 
 /*!
 *   \brief Instantiate a BadAllocException with message
 */
 #define SRBadAllocException(txt) BadAllocException(txt, __FILE__, __LINE__)
 
@@ -219,14 +269,22 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRDatabaseError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("DatabaseException");
+    }
 };
 
 /*!
 *   \brief Instantiate a DatabaseException with message
 */
 #define SRDatabaseException(txt) DatabaseException(txt, __FILE__, __LINE__)
 
@@ -242,14 +300,22 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRRuntimeError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("RuntimeException");
+    }
 };
 
 /*!
 *   \brief Instantiate a RuntimeException with message
 \*/
 #define SRRuntimeException(txt) RuntimeException(txt, __FILE__, __LINE__)
 
@@ -265,14 +331,22 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRParameterError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("ParameterException");
+    }
 };
 
 /*!
 *   \brief Instantiate a ParameterException with message
 */
 #define SRParameterException(txt) ParameterException(txt, __FILE__, __LINE__)
 
@@ -288,14 +362,22 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRTimeoutError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("TimeoutException");
+    }
 };
 
 /*!
 *   \brief Instantiate a TimeoutException with message
 */
 #define SRTimeoutException(txt) TimeoutException(txt, __FILE__, __LINE__)
 
@@ -311,14 +393,22 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRInternalError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("InternalException");
+    }
 };
 
 /*!
 *   \brief Instantiate a InternalException with message
 */
 #define SRInternalException(txt) InternalException(txt, __FILE__, __LINE__)
 
@@ -334,14 +424,22 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRKeyError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("KeyException");
+    }
 };
 
 /*!
 *   \brief Instantiate a KeyException with message
 */
 #define SRKeyException(txt) KeyException(txt, __FILE__, __LINE__)
 
@@ -356,26 +454,26 @@
     /*!
     *   \brief Retrieve an error code matching the exception type
     *   \returns Error code corresponding to the exception type
     */
     SRError to_error_code() const noexcept override {
         return SRTypeError;
     }
+
+    /*!
+    *   \brief Get a string representation of the exception class
+    *   \returns Stringified version of the class name
+    */
+    virtual std::string exception_class() {
+        return std::string("TypeException");
+    }
 };
 
 /*!
 *   \brief Instantiate a TypeException with message
 */
 #define SRTypeException(txt) TypeException(txt, __FILE__, __LINE__)
 
-/*!
-*   \brief Store the last error encountered in a global variable. Not
-*          currently thread-safe
-*   \param last_error Exception to be stored as the last error encountered
-*/
-extern "C"
-void SRSetLastError(const Exception& last_error);
-
 } // namespace SmartRedis
 
 #endif // __cplusplus
-#endif // SMARTREDIS_SRException_H
+#endif // SMARTREDIS_SREXCEPTION_H
```

### Comparing `smartredis-0.3.1/include/stringfield.h` & `smartredis-0.4.0/include/stringfield.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -28,14 +28,16 @@
 
 #ifndef SMARTREDIS_STRINGFIELD_H
 #define SMARTREDIS_STRINGFIELD_H
 
 #include "metadatafield.h"
 #include "metadatabuffer.h"
 
+///@file
+
 namespace SmartRedis {
 
 /*!
 *   \brief  The StringField class implements
 *   MetadataField class methods needed for
 *   storage and transfer of metadata string
 *   fields.
@@ -111,15 +113,15 @@
         */
         void append(const std::string& value);
 
         /*!
         *   \brief Retrieve the number of values in the field
         *   \returns The number of values
         */
-        virtual size_t size();
+        virtual size_t size() const;
 
         /*!
         *   \brief Clear the values in the field
         */
         virtual void clear();
 
         /*!
@@ -142,10 +144,10 @@
         /*!
         *   \brief The ScalarField values
         */
         std::vector<std::string> _vals;
 
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_STRINGFIELD_H
+#endif // SMARTREDIS_STRINGFIELD_H
```

### Comparing `smartredis-0.3.1/include/tensor.h` & `smartredis-0.4.0/include/tensor.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,15 +25,15 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_TENSOR_H
 #define SMARTREDIS_TENSOR_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <string>
 #include <stdexcept>
 #include "tensorbase.h"
 #include "sharedmemorylist.h"
 #include "srexception.h"
 
 ///@file
@@ -311,10 +311,10 @@
         *   \brief Memory allocated for f nested tensor memory views
         */
         SharedMemoryList<T> _f_mem_views;
 };
 
 #include "tensor.tcc"
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_TENSOR_H
+#endif // SMARTREDIS_TENSOR_H
```

### Comparing `smartredis-0.3.1/include/tensor.tcc` & `smartredis-0.4.0/include/tensor.tcc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,14 +25,16 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_TENSOR_TCC
 #define SMARTREDIS_TENSOR_TCC
 
+///@file
+
 // Tensor constructor
 template <class T>
 Tensor<T>::Tensor(const std::string& name,
                   void* data,
                   const std::vector<size_t>& dims,
                   const SRTensorType type,
                   const SRMemoryLayout mem_layout) :
@@ -442,8 +444,8 @@
             sum_product *= dims[m];
         }
         position += sum_product;
     }
     return position;
 }
 
-#endif //SMARTREDIS_TENSOR_TCC
+#endif // SMARTREDIS_TENSOR_TCC
```

### Comparing `smartredis-0.3.1/include/tensorbase.h` & `smartredis-0.4.0/include/tensorbase.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,15 +25,15 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_TENSORBASE_H
 #define SMARTREDIS_TENSORBASE_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <vector>
 #include <unordered_map>
 #include <string>
 #include <string_view>
 #include <stdexcept>
 #include "sr_enums.h"
 
@@ -73,16 +73,14 @@
         {SRTensorTypeInt64, DATATYPE_TENSOR_STR_INT64},
         {SRTensorTypeInt32, DATATYPE_TENSOR_STR_INT32},
         {SRTensorTypeInt16, DATATYPE_TENSOR_STR_INT16},
         {SRTensorTypeInt8, DATATYPE_TENSOR_STR_INT8},
         {SRTensorTypeUint16, DATATYPE_TENSOR_STR_UINT16},
         {SRTensorTypeUint8, DATATYPE_TENSOR_STR_UINT8} };
 
-class TensorBase;
-
 /*!
 *   \brief  The TensorBase class is a base class that
 *           defines an interface for templated classes
 *           that inherit from TensorBase.
 */
 class TensorBase{
 
@@ -149,40 +147,40 @@
         */
         TensorBase& operator=(TensorBase&& tb);
 
         /*!
         *   \brief Retrieve the name of the TensorBase
         *   \returns The name of the TensorBase
         */
-        std::string name();
+        std::string name() const;
 
         /*!
         *   \brief Retrieve the type of the TensorBase
         *   \returns The type of the TensorBase
         */
-        SRTensorType type();
+        SRTensorType type() const;
 
         /*!
         *   \brief Retrieve a string representation of
         *          the TensorBase
         *   \returns A string representation of the TensorBase
         */
         std::string type_str();
 
         /*!
         *   \brief Retrieve the dimensions of the TensorBase
         *   \returns TensorBase dimensions
         */
-        std::vector<size_t> dims();
+        std::vector<size_t> dims() const;
 
         /*!
         *   \brief Retrieve number of values in the TensorBase
         *   \returns The number values in the TensorBase
         */
-        size_t num_values();
+        size_t num_values() const;
 
         /*!
         *   \brief Retrieve a pointer to the TensorBase data
         *          memory
         *   \returns A pointer to the TenorBase data memory
         */
         void* data();
@@ -268,10 +266,10 @@
         /*!
         *   \brief Get the total number of bytes of the data
         *   \returns Total number of bytes of the data
         */
         virtual size_t _n_data_bytes() = 0;
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_TENSORBASE_H
+#endif // SMARTREDIS_TENSORBASE_H
```

### Comparing `smartredis-0.3.1/include/tensorpack.h` & `smartredis-0.4.0/include/tensorpack.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,28 +25,26 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_TENSORPACK_H
 #define SMARTREDIS_TENSORPACK_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <string>
 #include <vector>
 #include <unordered_map>
 #include <forward_list>
 #include "tensor.h"
 #include "tensorbase.h"
 
 ///@file
 
 namespace SmartRedis {
 
-class TensorPack;
-
 /*!
 *   \brief The TensorPack class is a container that
 *          manages Tensors of multiple data types.
 */
 class TensorPack
 {
     public:
@@ -131,15 +129,15 @@
                 const_tensorbase_iterator;
 
         /*!
         *   \brief Return a TensorBase pointer based on name.
         *   \param name The name used to reference the tensor
         *   \returns A pointer to the TensorBase object
         */
-        TensorBase* get_tensor(const std::string& name);
+        TensorBase* get_tensor(const std::string& name) const;
 
         /*!
         *   \brief Return a pointer to the tensor data memory space
         *   \param name The name used to reference the tensor
         *   \returns A c-ptr to the tensor data
         */
         void* get_tensor_data(const std::string& name);
@@ -147,15 +145,15 @@
         /*!
         *   \brief Returns boolean indicating if tensor by
         *          that name exists in the TensorPack
         *   \param name The name used to reference the tensor
         *   \returns True if the name corresponds to a tensor
         *            in the TensorPack, otherwise False.
         */
-        bool tensor_exists(const std::string& name);
+        bool tensor_exists(const std::string& name) const;
 
         /*!
         *   \brief Returns an iterator pointing to the
         *          first TensorBase in the TensorPack
         *   \returns TensorPack iterator to the first
         *            TensorBase
         */
@@ -212,10 +210,10 @@
         *   \brief Copy the tensor inventory from one
         *          TensorPack to this TensorPack
         *   \param tp The source TensorPack for copying
         */
         void _copy_tensor_inventory(const TensorPack& tp);
 };
 
-} //namespace SmartRedis
+} // namespace SmartRedis
 
-#endif //SMARTREDIS_TENSORPACK_H
+#endif // SMARTREDIS_TENSORPACK_H
```

### Comparing `smartredis-0.3.1/setup.cfg` & `smartredis-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartredis
-version = 0.3.1
+version = 0.4.0
 description = RedisAI clients for SmartSim
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrayLabs/SmartRedis
 project_urls = 
 	Source = https://github.com/CrayLabs/SmartRedis
 	Documentation = https://www.craylabs.org
@@ -27,30 +27,31 @@
 	=src/python/module
 packages = find:
 setup_requires = 
 	setuptools>=39.2
 include_package_data = True
 install_requires = 
 	numpy>=1.18.2
-python_requires = >=3.7
+python_requires = >=3.7,<3.11
 
 [options.extras_require]
 dev = 
-	numpy>=1.18.2
 	pytest>=6.0.0
 	pytest-cov==2.10.1
 	black==20.8b1
 	isort==5.6.4
 	pylint==2.6.0
 	torch==1.7.1
 doc = 
 	sphinx==3.1.1
 	sphinx-fortran==1.1.1
 	sphinx_rtd_theme>=0.5.0
 	breathe==4.25.1
+xarray = 
+	xarray>=0.14.1
 
 [options.packages.find]
 where = src/python/module
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `smartredis-0.3.1/setup.py` & `smartredis-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/c/c_client.cpp` & `smartredis-0.4.0/src/c/c_client.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -31,424 +31,300 @@
 #include <stdio.h>
 #include "c_client.h"
 #include "srexception.h"
 #include "srassert.h"
 
 using namespace SmartRedis;
 
-// Return a pointer to a new Client.
-// The caller is responsible for deleting the client via DeleteClient().
-extern "C"
-SRError SmartRedisCClient(bool cluster, void** new_client)
+// Decorator to standardize exception handling in C Client API methods
+template <class T>
+auto c_client_api(T&& client_api_func, const char* name)
+{
+  // we create a closure below
+  auto decorated = [name, client_api_func =
+    std::forward<T>(client_api_func)](auto&&... args)
+  {
+    SRError result = SRNoError;
+    try {
+      client_api_func(std::forward<decltype(args)>(args)...);
+    }
+    catch (const Exception& e) {
+      SRSetLastError(e);
+      result = e.to_error_code();
+    }
+    catch (...) {
+      std::string msg(
+          "A non-standard exception was encountered while executing ");
+      msg += name;
+      SRSetLastError(SRInternalException(msg));
+      result = SRInternalError;
+    }
+    return result;
+  };
+  return decorated;
+}
+
+// Macro to invoke the decorator with a lambda function
+#define MAKE_CLIENT_API(stuff)\
+    c_client_api([&] { stuff }, __func__)()
+
+
+// Return a pointer to a new Client
+extern "C" SRError SmartRedisCClient(
+  bool cluster,
+  const char* logger_name,
+  const size_t logger_name_length,
+  void** new_client)
 {
-  SRError result = SRNoError;
-  try {
+  return MAKE_CLIENT_API({
     // Sanity check params
-    SR_CHECK_PARAMS(new_client != NULL);
-
-    Client* s = new Client(cluster);
-    *new_client = reinterpret_cast<void*>(s);
-  }
-  catch (const std::bad_alloc& e) {
-    *new_client = NULL;
-    SRSetLastError(SRBadAllocException("client allocation"));
-    result = SRBadAllocError;
-  }
-  catch (const Exception& e) {
-    *new_client = NULL;
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    *new_client = NULL;
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
+    SR_CHECK_PARAMS(new_client != NULL && logger_name != NULL);
 
-  return result;
+    std::string _logger_name(logger_name, logger_name_length);
+    try {
+      *new_client = NULL;
+      Client* s = new Client(cluster, _logger_name);
+      *new_client = reinterpret_cast<void*>(s);
+    }
+    catch (const std::bad_alloc& e) {
+      throw SRBadAllocException("client allocation");
+    }
+  });
 }
 
-// Free the memory associated with the c client.
-extern "C"
-SRError DeleteCClient(void** c_client)
+// Free the memory associated with the c client
+extern "C" SRError DeleteCClient(void** c_client)
 {
-  SRError result = SRNoError;
-
-  try {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL);
 
     delete reinterpret_cast<Client*>(*c_client);
     *c_client = NULL;
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Put a dataset into the database.
-extern "C"
-SRError put_dataset(void* c_client, void* dataset)
+// Put a dataset into the database
+extern "C" SRError put_dataset(void* c_client, void* dataset)
 {
-  SRError result = SRNoError;
-
-  try {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && dataset != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     DataSet* d = reinterpret_cast<DataSet*>(dataset);
-
     s->put_dataset(*d);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Return a pointer to a new dataset.  The user is
-// responsible for deleting the dataset via DeallocateeDataSet()
-extern "C"
-SRError get_dataset(void* c_client, const char* name,
-                    const size_t name_length, void **dataset)
+// Return a pointer to a new dataset
+extern "C" SRError get_dataset(
+  void* c_client, const char* name, const size_t name_length, void **dataset)
 {
-  SRError result = SRNoError;
-
-  try {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && dataset != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string dataset_name(name, name_length);
     DataSet* d = NULL;
 
     try {
       d = new DataSet(s->get_dataset(dataset_name));
       *dataset = reinterpret_cast<void*>(d);
     } catch (const std::bad_alloc& e) {
       *dataset = NULL;
-      throw SRBadAllocException("client allocation");
+      throw SRBadAllocException("dataset allocation");
     }
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Rename a dataset in the database.
-extern "C"
-SRError rename_dataset(void* c_client, const char* old_name,
-                       const size_t old_name_length, const char* new_name,
-                       const size_t new_name_length)
+// Rename a dataset in the database
+extern "C" SRError rename_dataset(
+  void* c_client, const char* old_name,
+  const size_t old_name_length, const char* new_name,
+  const size_t new_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && old_name != NULL && new_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(old_name, old_name_length);
     std::string new_name_str(new_name, new_name_length);
 
     s->rename_dataset(name_str, new_name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-
 // Copy a dataset from the src_name to the dest_name
-extern "C"
-SRError copy_dataset(void* c_client, const char* src_name,
-                    const size_t src_name_length, const char* dest_name,
-                    const size_t dest_name_length)
+extern "C" SRError copy_dataset(
+  void* c_client, const char* src_name,
+  const size_t src_name_length, const char* dest_name,
+  const size_t dest_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && src_name != NULL && dest_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string src_name_str(src_name, src_name_length);
     std::string dest_name_str(dest_name, dest_name_length);
 
     s->copy_dataset(src_name_str, dest_name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Delete a dataset (all metadata and tensors) from the database.
-extern "C"
-SRError delete_dataset(void* c_client, const char* name, const size_t name_length)
+// Delete a dataset (all metadata and tensors) from the database
+extern "C" SRError delete_dataset(
+  void* c_client, const char* name, const size_t name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string dataset_name(name, name_length);
     s->delete_dataset(dataset_name);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Put a tensor of a specified type into the database
-extern "C"
-SRError put_tensor(void* c_client,
-                  const char* name,
-                  const size_t name_length,
-                  void* data,
-                  const size_t* dims,
-                  const size_t n_dims,
-                  const SRTensorType type,
-                  const SRMemoryLayout mem_layout)
+extern "C" SRError put_tensor(
+  void* c_client,
+  const char* name,
+  const size_t name_length,
+  void* data,
+  const size_t* dims,
+  const size_t n_dims,
+  const SRTensorType type,
+  const SRMemoryLayout mem_layout)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL &&
                     data != NULL && dims != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     std::vector<size_t> dims_vec;
     dims_vec.assign(dims, dims + n_dims);
 
     s->put_tensor(name_str, data, dims_vec, type, mem_layout);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Get a tensor of a specified type from the database
-extern "C"
-SRError get_tensor(void* c_client,
-                  const char* name,
-                  const size_t name_length,
-                  void** result,
-                  size_t** dims,
-                  size_t* n_dims,
-                  SRTensorType* type,
-                  const SRMemoryLayout mem_layout)
+extern "C" SRError get_tensor(
+  void* c_client,
+    const char* name,
+    const size_t name_length,
+    void** result,
+    size_t** dims,
+    size_t* n_dims,
+    SRTensorType* type,
+    const SRMemoryLayout mem_layout)
 {
-  SRError outcome = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && result != NULL &&
                     dims != NULL && n_dims != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     s->get_tensor(name_str, *result, *dims, *n_dims, *type, mem_layout);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    outcome = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    outcome = SRInternalError;
-  }
-
-  return outcome;
+  });
 }
 
 // Get a tensor of a specified type from the database
-// and put the values into the user provided memory space.
-extern "C"
-SRError unpack_tensor(void* c_client,
-                     const char* name,
-                     const size_t name_length,
-                     void* result,
-                     const size_t* dims,
-                     const size_t n_dims,
-                     const SRTensorType type,
-                     const SRMemoryLayout mem_layout)
+// and put the values into the user provided memory space
+extern "C" SRError unpack_tensor(
+  void* c_client,
+  const char* name,
+  const size_t name_length,
+  void* result,
+  const size_t* dims,
+  const size_t n_dims,
+  const SRTensorType type,
+  const SRMemoryLayout mem_layout)
 {
-  SRError outcome = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && result != NULL &&
                     dims != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     std::vector<size_t> dims_vec;
     dims_vec.assign(dims, dims + n_dims);
 
     s->unpack_tensor(name_str, result, dims_vec, type, mem_layout);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    outcome = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    outcome = SRInternalError;
-  }
-
-  return outcome;
+  });
 }
 
 // Rename a tensor from old_name to new_name
-extern "C"
-SRError rename_tensor(void* c_client,
-                      const char* old_name, const size_t old_name_length,
-                      const char* new_name, const size_t new_name_length)
+extern "C" SRError rename_tensor(
+  void* c_client,
+  const char* old_name,
+  const size_t old_name_length,
+  const char* new_name,
+  const size_t new_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && old_name != NULL && new_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string old_name_str(old_name, old_name_length);
     std::string new_name_str(new_name, new_name_length);
 
     s->rename_tensor(old_name_str, new_name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Delete a tensor from the database.
-extern "C"
-SRError delete_tensor(void* c_client, const char* name,
-                      const size_t name_length)
+// Delete a tensor from the database
+extern "C" SRError delete_tensor(
+  void* c_client, const char* name, const size_t name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     s->delete_tensor(name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Copy a tensor from src_name to dest_name.
-extern "C"
-SRError copy_tensor(void* c_client,
-                   const char* src_name,
-                   const size_t src_name_length,
-                   const char* dest_name,
-                   const size_t dest_name_length)
+// Copy a tensor from src_name to dest_name
+extern "C" SRError copy_tensor(
+  void* c_client,
+  const char* src_name,
+  const size_t src_name_length,
+  const char* dest_name,
+  const size_t dest_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && src_name != NULL && dest_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string src_str(src_name, src_name_length);
     std::string dest_str(dest_name, dest_name_length);
 
     s->copy_tensor(src_str, dest_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-bool CompareCaseInsensitive(const char* a,const char* b) {
+// Perform a case insensitive compare fo two strings
+static bool _compareCaseInsensitive(const char* a,const char* b) {
   while (*a != '\0' && *b != '\0') {
     // Check current character
     if (toupper(*a) != toupper(*b))
       return false;
 
     // Advance to next character
     a++;
@@ -458,37 +334,39 @@
   // Make sure there is no additional data in b
   return (*a == *b);
 }
 
 // Return True if the backend is TF or TFLITE
 bool _isTensorFlow(const char* backend)
 {
-  return CompareCaseInsensitive(backend, "TF") || CompareCaseInsensitive(backend, "TFLITE");
+  return _compareCaseInsensitive(backend, "TF") ||
+         _compareCaseInsensitive(backend, "TFLITE");
 }
 
 // Check the parameters common to all set_model functions
-void _check_params_set_model(void* c_client,
-                            const char* name, const char* backend,
-                            const char** inputs, const size_t* input_lengths, const size_t n_inputs,
-                            const char** outputs, const size_t* output_lengths, const size_t n_outputs)
+void _check_params_set_model(
+  void* c_client, const char* name, const char* backend,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs)
 {
   // Sanity check params. Tag is strictly optional, and inputs/outputs are
   // mandatory IFF backend is TensorFlow (TF or TFLITE)
   SR_CHECK_PARAMS(c_client != NULL && name != NULL && backend != NULL);
 
   if (_isTensorFlow(backend)) {
     if (inputs == NULL || input_lengths == NULL ||
         outputs == NULL || output_lengths == NULL) {
-      throw SRParameterException("Inputs and outputs are required with TensorFlow");
+      throw SRParameterException(
+        "Inputs and outputs are required with TensorFlow");
     }
   }
 
   // For the inputs and outputs arrays, a single empty string is ok (this means
-  // that the array should be skipped) but if more than one entry is present, the
-  // strings must be nonzero length
+  // that the array should be skipped) but if more than one entry is present,
+  // the strings must be nonzero length
   if (_isTensorFlow(backend)) {
     if (n_inputs != 1 && input_lengths[0] != 0) {
       for (size_t i = 0; i < n_inputs; i++){
         if (inputs[i] == NULL || input_lengths[i] == 0) {
           throw SRParameterException(
             "inputs[" + std::to_string(i) + "] is NULL or empty");
         }
@@ -501,31 +379,28 @@
             "outputs[" + std::to_string(i) + "] is NULL or empty");
         }
       }
     }
   }
 }
 
-// Set a model stored in a binary file.
-extern "C"
-SRError set_model_from_file(void* c_client,
-                           const char* name, const size_t name_length,
-                           const char* model_file, const size_t model_file_length,
-                           const char* backend, const size_t backend_length,
-                           const char* device, const size_t device_length,
-                           const int batch_size, const int min_batch_size,
-                           const char* tag, const size_t tag_length,
-                           const char** inputs, const size_t* input_lengths,
-                           const size_t n_inputs,
-                           const char** outputs, const size_t* output_lengths,
-                           const size_t n_outputs)
+// Set a model stored in a binary file
+extern "C" SRError set_model_from_file(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* model_file, const size_t model_file_length,
+  const char* backend, const size_t backend_length,
+  const char* device, const size_t device_length,
+  const int batch_size,
+  const int min_batch_size,
+  const char* tag, const size_t tag_length,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params. Tag is strictly optional, and inputs/outputs are
     // mandatory IFF backend is TensorFlow (TF or TFLITE)
     _check_params_set_model(c_client, name, backend, inputs, input_lengths, n_inputs,
                           outputs, output_lengths, n_outputs);
     SR_CHECK_PARAMS(model_file != NULL && device != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
@@ -551,43 +426,33 @@
         for (size_t i = 0; i < n_outputs; i++) {
           output_vec.push_back(std::string(outputs[i], output_lengths[i]));
         }
       }
     }
 
     s->set_model_from_file(name_str, model_file_str, backend_str, device_str,
-                           batch_size, min_batch_size, tag_str, input_vec,
-                           output_vec);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
-}
-extern "C"
-SRError set_model_from_file_multigpu(void* c_client,
-                                     const char* name, const size_t name_length,
-                                     const char* model_file, const size_t model_file_length,
-                                     const char* backend, const size_t backend_length,
-                                     const int first_gpu, const int num_gpus,
-                                     const int batch_size, const int min_batch_size,
-                                     const char* tag, const size_t tag_length,
-                                     const char** inputs, const size_t* input_lengths,
-                                     const size_t n_inputs, const char** outputs,
-                                     const size_t* output_lengths, const size_t n_outputs)
+                            batch_size, min_batch_size, tag_str, input_vec,
+                            output_vec);
+  });
+}
+
+// Set a model stored in a binary file for use with multiple GPUs
+extern "C" SRError set_model_from_file_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* model_file, const size_t model_file_length,
+  const char* backend, const size_t backend_length,
+  const int first_gpu, const int num_gpus,
+  const int batch_size, const int min_batch_size,
+  const char* tag, const size_t tag_length,
+  const char** inputs, const size_t* input_lengths,
+  const size_t n_inputs, const char** outputs,
+  const size_t* output_lengths, const size_t n_outputs)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params. Tag is strictly optional, and inputs/outputs are
     // mandatory IFF backend is TensorFlow (TF or TFLITE)
     _check_params_set_model(c_client, name, backend, inputs, input_lengths, n_inputs,
                           outputs, output_lengths, n_outputs);
     SR_CHECK_PARAMS(model_file != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
@@ -612,46 +477,34 @@
         for (size_t i = 0; i < n_outputs; i++) {
           output_vec.push_back(std::string(outputs[i], output_lengths[i]));
         }
       }
     }
 
     s->set_model_from_file_multigpu(name_str, model_file_str, backend_str, first_gpu,
-                                   num_gpus, batch_size, min_batch_size, tag_str,
-                                   input_vec, output_vec);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+                                    num_gpus, batch_size, min_batch_size, tag_str,
+                                    input_vec, output_vec);
+  });
 }
 
 // Set a model stored in a buffer c-string.
-extern "C"
-SRError set_model(void* c_client,
-                 const char* name, const size_t name_length,
-                 const char* model, const size_t model_length,
-                 const char* backend, const size_t backend_length,
-                 const char* device, const size_t device_length,
-                 const int batch_size, const int min_batch_size,
-                 const char* tag, const size_t tag_length,
-                 const char** inputs, const size_t* input_lengths,
-                 const size_t n_inputs,
-                 const char** outputs, const size_t* output_lengths,
-                 const size_t n_outputs)
+extern "C" SRError set_model(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* model, const size_t model_length,
+  const char* backend, const size_t backend_length,
+  const char* device, const size_t device_length,
+  const int batch_size, const int min_batch_size,
+  const char* tag, const size_t tag_length,
+  const char** inputs, const size_t* input_lengths,
+  const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths,
+  const size_t n_outputs)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params. Tag is strictly optional, and inputs/outputs are
     // mandatory IFF backend is TensorFlow (TF or TFLITE)
     _check_params_set_model(c_client, name, backend, inputs, input_lengths, n_inputs,
                           outputs, output_lengths, n_outputs);
     SR_CHECK_PARAMS(model != NULL && device != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
@@ -679,44 +532,32 @@
         }
       }
     }
 
     s->set_model(name_str, model_str, backend_str, device_str,
                 batch_size, min_batch_size, tag_str, input_vec,
                 output_vec);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Set a model stored in a buffer c-string.
-extern "C"
-SRError set_model_multigpu(void* c_client,
-                          const char* name, const size_t name_length,
-                          const char* model, const size_t model_length,
-                          const char* backend, const size_t backend_length,
-                          const int first_gpu, const int num_gpus,
-                          const int batch_size, const int min_batch_size,
-                          const char* tag, const size_t tag_length,
-                          const char** inputs, const size_t* input_lengths,
-                          const size_t n_inputs,
-                          const char** outputs, const size_t* output_lengths,
-                          const size_t n_outputs)
+// Set a model stored in a buffer c-string
+extern "C" SRError set_model_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* model, const size_t model_length,
+  const char* backend, const size_t backend_length,
+  const int first_gpu, const int num_gpus,
+  const int batch_size, const int min_batch_size,
+  const char* tag, const size_t tag_length,
+  const char** inputs, const size_t* input_lengths,
+  const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths,
+  const size_t n_outputs)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params. Tag is strictly optional, and inputs/outputs are
     // mandatory IFF backend is TensorFlow (TF or TFLITE)
     _check_params_set_model(c_client, name, backend, inputs, input_lengths, n_inputs,
                           outputs, output_lengths, n_outputs);
     SR_CHECK_PARAMS(model != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
@@ -741,292 +582,183 @@
         for (size_t i = 0; i < n_outputs; i++) {
           output_vec.push_back(std::string(outputs[i], output_lengths[i]));
         }
       }
     }
 
     s->set_model_multigpu(name_str, model_str, backend_str, first_gpu, num_gpus,
-                         batch_size, min_batch_size, tag_str, input_vec,
-                         output_vec);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+                          batch_size, min_batch_size, tag_str, input_vec,
+                          output_vec);
+  });
 }
 
-
 // Retrieve the model and model length from the database
-extern "C"
-SRError get_model(void* c_client,
-                  const char* name,
-                  const size_t name_length,
-                  size_t* model_length,
-                  const char** model)
+extern "C" SRError get_model(
+  void* c_client,
+  const char* name, const size_t name_length,
+  size_t* model_length, const char** model)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && model_length != NULL &&
                     model != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
     std::string_view model_str_view(s->get_model(name_str));
 
     *model_length = model_str_view.size();
     *model = model_str_view.data();
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Put a script in the database that is stored in a file.
-extern "C"
-SRError set_script_from_file(void* c_client,
-                            const char* name,
-                            const size_t name_length,
-                            const char* device,
-                            const size_t device_length,
-                            const char* script_file,
-                            const size_t script_file_length)
+extern "C" SRError set_script_from_file(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* device, const size_t device_length,
+  const char* script_file, const size_t script_file_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && device != NULL &&
                     script_file != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
     std::string device_str(device, device_length);
     std::string script_file_str(script_file, script_file_length);
 
     s->set_script_from_file(name_str, device_str, script_file_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Put a script in the database that is stored in a file in a multi-GPU system
-extern "C"
-SRError set_script_from_file_multigpu(void* c_client,
-                                     const char* name,
-                                     const size_t name_length,
-                                     const char* script_file,
-                                     const size_t script_file_length,
-                                     const int first_gpu,
-                                     const int num_gpus)
+extern "C" SRError set_script_from_file_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* script_file, const size_t script_file_length,
+  const int first_gpu,
+  const int num_gpus)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && script_file != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
     std::string script_file_str(script_file, script_file_length);
 
     s->set_script_from_file_multigpu(name_str, script_file_str, first_gpu, num_gpus);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Put a script in the database that is stored in a string.
-extern "C"
-SRError set_script(void* c_client,
-                  const char* name,
-                  const size_t name_length,
-                  const char* device,
-                  const size_t device_length,
-                  const char* script,
-                  const size_t script_length)
+extern "C" SRError set_script(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* device, const size_t device_length,
+  const char* script, const size_t script_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && device != NULL &&
                     script != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
 
     std::string name_str(name, name_length);
     std::string device_str(device, device_length);
     std::string script_str(script, script_length);
 
     s->set_script(name_str, device_str, script_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Put a script in the database that is stored in a string in a multi-GPU system
-extern "C"
-SRError set_script_multigpu(void* c_client,
-                           const char* name,
-                           const size_t name_length,
-                           const char* script,
-                           const size_t script_length,
-                           const int first_gpu,
-                           const int num_gpus)
+extern "C" SRError set_script_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* script, const size_t script_length,
+  const int first_gpu,
+  const int num_gpus)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && script != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
 
     std::string name_str(name, name_length);
     std::string script_str(script, script_length);
 
     s->set_script_multigpu(name_str, script_str, first_gpu, num_gpus);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-
-
 // Retrieve the script stored in the database
-extern "C"
-SRError get_script(void* c_client,
-                  const char* name,
-                  const size_t name_length,
-                  const char** script,
-                  size_t* script_length)
+extern "C" SRError get_script(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char** script, size_t* script_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && script != NULL &&
                     script_length != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
     std::string_view script_str_view(s->get_script(name_str));
 
     (*script) = script_str_view.data();
     (*script_length) = script_str_view.size();
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-void _check_params_run_script(void* c_client,
-                              const char* name,
-                              const char* function,
-                              const char** inputs,
-                              const size_t* input_lengths,
-                              const size_t n_inputs,
-                              const char** outputs,
-                              const size_t* output_lengths,
-                              const size_t n_outputs)
-{
-    // Sanity check params
-    SR_CHECK_PARAMS(c_client != NULL && name != NULL && function != NULL &&
-                    inputs != NULL && input_lengths != NULL &&
-                    outputs != NULL && output_lengths != NULL);
-
-    // Inputs and outputs are mandatory for run_script
-    for (size_t i = 0; i < n_inputs; i++){
-      if (inputs[i] == NULL || input_lengths[i] == 0) {
-        throw SRParameterException(
-          "inputs[" + std::to_string(i) + "] is NULL or empty");
-      }
-    }
-    for (size_t i = 0; i < n_outputs; i++) {
-      if (outputs[i] == NULL || output_lengths[i] == 0) {
-        throw SRParameterException(
-          "outputs[" + std::to_string(i) + "] is NULL or empty");
-      }
+// Validate parameters for running scripts
+void _check_params_run_script(
+  void* c_client,
+  const char* name,
+  const char* function,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs)
+{
+  // Sanity check params
+  SR_CHECK_PARAMS(c_client != NULL && name != NULL && function != NULL &&
+                  inputs != NULL && input_lengths != NULL &&
+                  outputs != NULL && output_lengths != NULL);
+
+  // Inputs and outputs are mandatory for run_script
+  for (size_t i = 0; i < n_inputs; i++){
+    if (inputs[i] == NULL || input_lengths[i] == 0) {
+      throw SRParameterException(
+        "inputs[" + std::to_string(i) + "] is NULL or empty");
+    }
+  }
+  for (size_t i = 0; i < n_outputs; i++) {
+    if (outputs[i] == NULL || output_lengths[i] == 0) {
+      throw SRParameterException(
+        "outputs[" + std::to_string(i) + "] is NULL or empty");
     }
+  }
 }
 
 // Run  a script function in the database
-extern "C"
-SRError run_script(void* c_client,
-                  const char* name,
-                  const size_t name_length,
-                  const char* function,
-                  const size_t function_length,
-                  const char** inputs,
-                  const size_t* input_lengths,
-                  const size_t n_inputs,
-                  const char** outputs,
-                  const size_t* output_lengths,
-                  const size_t n_outputs)
+extern "C" SRError run_script(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* function, const size_t function_length,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     _check_params_run_script(c_client, name, function,
-                             inputs, input_lengths, n_inputs,
-                             outputs, output_lengths, n_outputs);
+                              inputs, input_lengths, n_inputs,
+                              outputs, output_lengths, n_outputs);
     std::string name_str(name, name_length);
     std::string function_str(function, function_length);
 
     std::vector<std::string> input_vec;
     if (n_inputs != 1 || input_lengths[0] != 0) {
       for (size_t i = 0; i < n_inputs; i++) {
         input_vec.push_back(std::string(inputs[i], input_lengths[i]));
@@ -1038,50 +770,32 @@
       for (size_t i = 0; i < n_outputs; i++) {
         output_vec.push_back(std::string(outputs[i], output_lengths[i]));
       }
     }
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->run_script(name_str, function_str, input_vec, output_vec);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Run  a script function in the database in a multi-GPU system
-extern "C"
-SRError run_script_multigpu(void* c_client,
-                           const char* name,
-                           const size_t name_length,
-                           const char* function,
-                           const size_t function_length,
-                           const char** inputs,
-                           const size_t* input_lengths,
-                           const size_t n_inputs,
-                           const char** outputs,
-                           const size_t* output_lengths,
-                           const size_t n_outputs,
-                           const int offset,
-                           const int first_gpu,
-                           const int num_gpus)
+extern "C" SRError run_script_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char* function, const size_t function_length,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs,
+  const int offset,
+  const int first_gpu,
+  const int num_gpus)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     _check_params_run_script(c_client, name, function,
-                             inputs, input_lengths, n_inputs,
-                             outputs, output_lengths, n_outputs);
+                            inputs, input_lengths, n_inputs,
+                            outputs, output_lengths, n_outputs);
     std::string name_str(name, name_length);
     std::string function_str(function, function_length);
 
     std::vector<std::string> input_vec;
     if (n_inputs != 1 || input_lengths[0] != 0) {
       for (size_t i = 0; i < n_inputs; i++) {
         input_vec.push_back(std::string(inputs[i], input_lengths[i]));
@@ -1093,74 +807,55 @@
       for (size_t i = 0; i < n_outputs; i++) {
         output_vec.push_back(std::string(outputs[i], output_lengths[i]));
       }
     }
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->run_script_multigpu(name_str, function_str, input_vec, output_vec,
-                           offset, first_gpu, num_gpus);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+                          offset, first_gpu, num_gpus);
+  });
 }
 
-void _check_params_run_model(void* c_client,
-                  const char* name,
-                  const char** inputs,
-                  const size_t* input_lengths,
-                  const size_t n_inputs,
-                  const char** outputs,
-                  const size_t* output_lengths,
-                  const size_t n_outputs)
-{
-    // Sanity check params
-    SR_CHECK_PARAMS(c_client != NULL && name != NULL &&
-                    inputs != NULL && input_lengths != NULL &&
-                    outputs != NULL && output_lengths != NULL);
-
-    // Inputs and outputs are mandatory for run_script
-    for (size_t i = 0; i < n_inputs; i++){
-      if (inputs[i] == NULL || input_lengths[i] == 0) {
-        throw SRParameterException(
-          "inputs[" + std::to_string(i) + "] is NULL or empty");
-      }
-    }
-    for (size_t i = 0; i < n_outputs; i++) {
-      if (outputs[i] == NULL || output_lengths[i] == 0) {
-        throw SRParameterException(
-          "outputs[" + std::to_string(i) + "] is NULL or empty");
-      }
+// Validate the parameters for running models
+void _check_params_run_model(
+  void* c_client,
+  const char* name,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs)
+{
+  // Sanity check params
+  SR_CHECK_PARAMS(c_client != NULL && name != NULL &&
+                  inputs != NULL && input_lengths != NULL &&
+                  outputs != NULL && output_lengths != NULL);
+
+  // Inputs and outputs are mandatory for run_script
+  for (size_t i = 0; i < n_inputs; i++){
+    if (inputs[i] == NULL || input_lengths[i] == 0) {
+      throw SRParameterException(
+        "inputs[" + std::to_string(i) + "] is NULL or empty");
+    }
+  }
+  for (size_t i = 0; i < n_outputs; i++) {
+    if (outputs[i] == NULL || output_lengths[i] == 0) {
+      throw SRParameterException(
+        "outputs[" + std::to_string(i) + "] is NULL or empty");
     }
+  }
 }
 
 // Run a model in the database
-extern "C"
-SRError run_model(void* c_client,
-                 const char* name,
-                 const size_t name_length,
-                 const char** inputs,
-                 const size_t* input_lengths,
-                 const size_t n_inputs,
-                 const char** outputs,
-                 const size_t* output_lengths,
-                 const size_t n_outputs)
+extern "C" SRError run_model(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     _check_params_run_model(c_client, name, inputs, input_lengths, n_inputs,
-                           outputs, output_lengths, n_outputs);
+                            outputs, output_lengths, n_outputs);
     std::string name_str(name, name_length);
 
     std::vector<std::string> input_vec;
     if (n_inputs != 1 || input_lengths[0] != 0) {
       for (size_t i = 0; i < n_inputs; i++) {
         input_vec.push_back(std::string(inputs[i], input_lengths[i]));
       }
@@ -1171,47 +866,30 @@
       for (size_t i = 0; i < n_outputs; i++) {
         output_vec.push_back(std::string(outputs[i], output_lengths[i]));
       }
     }
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->run_model(name_str, input_vec, output_vec);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Run a model in the database
-extern "C"
-SRError run_model_multigpu(void* c_client,
-                          const char* name,
-                          const size_t name_length,
-                          const char** inputs,
-                          const size_t* input_lengths,
-                          const size_t n_inputs,
-                          const char** outputs,
-                          const size_t* output_lengths,
-                          const size_t n_outputs,
-                          const int offset,
-                          const int first_gpu,
-                          const int num_gpus)
+// Run a model in the database for multiple GPUs
+extern "C" SRError run_model_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const char** inputs, const size_t* input_lengths, const size_t n_inputs,
+  const char** outputs, const size_t* output_lengths, const size_t n_outputs,
+  const int offset,
+  const int first_gpu,
+  const int num_gpus)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     _check_params_run_model(c_client, name, inputs, input_lengths, n_inputs,
-                           outputs, output_lengths, n_outputs);
+                            outputs, output_lengths, n_outputs);
     std::string name_str(name, name_length);
 
     std::vector<std::string> input_vec;
     if (n_inputs != 1 || input_lengths[0] != 0) {
       for (size_t i = 0; i < n_inputs; i++) {
         input_vec.push_back(std::string(inputs[i], input_lengths[i]));
       }
@@ -1222,735 +900,436 @@
       for (size_t i = 0; i < n_outputs; i++) {
         output_vec.push_back(std::string(outputs[i], output_lengths[i]));
       }
     }
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->run_model_multigpu(name_str, input_vec, output_vec, offset,
-                         first_gpu, num_gpus);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+                          first_gpu, num_gpus);
+  });
 }
 
 // Remove a model from the database
-extern "C"
-SRError delete_model(void* c_client,
-                     const char* name,
-                     const size_t name_length)
+extern "C" SRError delete_model(
+  void* c_client, const char* name, const size_t name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL);
 
     std::string name_str(name, name_length);
     Client* s = reinterpret_cast<Client*>(c_client);
     s->delete_model(name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Remove a model from the database on a system with multiple GPUs
-extern "C"
-SRError delete_model_multigpu(void* c_client,
-                              const char* name,
-                              const size_t name_length,
-                              const int first_gpu,
-                              const int num_gpus)
+extern "C" SRError delete_model_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const int first_gpu,
+  const int num_gpus)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL);
 
     std::string name_str(name, name_length);
     Client* s = reinterpret_cast<Client*>(c_client);
     s->delete_model_multigpu(name_str, first_gpu, num_gpus);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Remove a script from the database
-extern "C"
-SRError delete_script(void* c_client,
-                      const char* name,
-                      const size_t name_length)
+extern "C" SRError delete_script(
+  void* c_client, const char* name, const size_t name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL);
 
     std::string name_str(name, name_length);
     Client* s = reinterpret_cast<Client*>(c_client);
     s->delete_script(name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Remove a script from the database in a system with multiple GPUs
-extern "C"
-SRError delete_script_multigpu(void* c_client,
-                               const char* name,
-                               const size_t name_length,
-                               const int first_gpu,
-                               const int num_gpus)
+extern "C" SRError delete_script_multigpu(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const int first_gpu,
+  const int num_gpus)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL);
 
     std::string name_str(name, name_length);
     Client* s = reinterpret_cast<Client*>(c_client);
     s->delete_script_multigpu(name_str, first_gpu, num_gpus);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Check whether a key exists in the database
-extern "C"
-SRError key_exists(void* c_client, const char* key, const size_t key_length,
-                   bool* exists)
+extern "C" SRError key_exists(
+  void* c_client, const char* key, const size_t key_length, bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && key != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string key_str(key, key_length);
 
     *exists = s->key_exists(key_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Check whether a model exists in the database
-extern "C"
-SRError model_exists(void* c_client, const char* name, const size_t name_length,
-                     bool* exists)
+extern "C" SRError model_exists(
+  void* c_client, const char* name, const size_t name_length, bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     *exists = s->model_exists(name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Check whether a tensor exists in the database
-extern "C"
-SRError tensor_exists(void* c_client, const char* name, const size_t name_length,
-                      bool* exists)
+extern "C" SRError tensor_exists(
+  void* c_client, const char* name, const size_t name_length, bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     *exists = s->tensor_exists(name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Delay until a dataset exists in the database
-extern "C"
-SRError dataset_exists(void* c_client, const char* name, const size_t name_length,
-                       bool* exists)
+// Check whether a dataset exists in the database
+extern "C" SRError dataset_exists(
+  void* c_client, const char* name, const size_t name_length, bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client *>(c_client);
     std::string name_str(name, name_length);
 
     *exists = s->dataset_exists(name_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Delay until a key exists in the database
-extern "C"
-SRError poll_key(void* c_client,
-                 const char* key,
-                 const size_t key_length,
-                 const int poll_frequency_ms,
-                 const int num_tries,
-                 bool* exists)
+extern "C" SRError poll_key(
+  void* c_client,
+  const char* key, const size_t key_length,
+  const int poll_frequency_ms,
+  const int num_tries,
+  bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && key != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string key_str(key, key_length);
 
     *exists = s->poll_key(key_str, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Delay until a model exists in the database
-extern "C"
-SRError poll_model(void* c_client,
-                   const char* name,
-                   const size_t name_length,
-                   const int poll_frequency_ms,
-                   const int num_tries,
-                   bool* exists)
+extern "C" SRError poll_model(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const int poll_frequency_ms,
+  const int num_tries,
+  bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     *exists = s->poll_model(name_str, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Delay until a tensor exists in the database
-extern "C"
-SRError poll_tensor(void* c_client,
-                 const char* name,
-                 const size_t name_length,
-                 const int poll_frequency_ms,
-                 const int num_tries,
-                 bool* exists)
+extern "C" SRError poll_tensor(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const int poll_frequency_ms,
+  const int num_tries,
+  bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     *exists = s->poll_tensor(name_str, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Delay until a dataset exists in the database
-extern "C"
-SRError poll_dataset(void* c_client,
-                     const char* name,
-                     const size_t name_length,
-                     const int poll_frequency_ms,
-                     const int num_tries,
-                     bool* exists)
+extern "C" SRError poll_dataset(
+  void* c_client,
+  const char* name, const size_t name_length,
+  const int poll_frequency_ms,
+  const int num_tries,
+  bool* exists)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && exists != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string name_str(name, name_length);
 
     *exists = s->poll_dataset(name_str, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Establish a data source
-extern "C"
-SRError set_data_source(void* c_client,
-                        const char* source_id,
-                        const size_t source_id_length)
+extern "C" SRError set_data_source(
+  void* c_client, const char* source_id, const size_t source_id_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && source_id != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string source_id_str(source_id, source_id_length);
 
     s->set_data_source(source_id_str);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Control whether a model ensemble prefix is used
-extern "C"
-SRError use_model_ensemble_prefix(void* c_client, bool use_prefix)
+extern "C" SRError use_model_ensemble_prefix(void* c_client, bool use_prefix)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->use_model_ensemble_prefix(use_prefix);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Control whether a tensor ensemble prefix is used
-extern "C"
-SRError use_tensor_ensemble_prefix(void* c_client, bool use_prefix)
+extern "C" SRError use_tensor_ensemble_prefix(void* c_client, bool use_prefix)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->use_tensor_ensemble_prefix(use_prefix);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
+  });
+}
 
-  return result;
+// Control whether a dataset ensemble prefix is used
+extern "C" SRError use_dataset_ensemble_prefix(void* c_client, bool use_prefix)
+{
+  return MAKE_CLIENT_API({
+    // Sanity check params
+    SR_CHECK_PARAMS(c_client != NULL);
+
+    Client* s = reinterpret_cast<Client*>(c_client);
+    s->use_dataset_ensemble_prefix(use_prefix);
+  });
 }
 
 // Control whether aggregation lists are prefixed
-extern "C"
-SRError use_list_ensemble_prefix(void* c_client, bool use_prefix)
+extern "C" SRError use_list_ensemble_prefix(void* c_client, bool use_prefix)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     s->use_list_ensemble_prefix(use_prefix);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Append a dataset to the aggregation list
-extern "C"
-SRError append_to_list(void* c_client, const char* list_name,
-                       const size_t list_name_length, const void* dataset)
+extern "C" SRError append_to_list(
+  void* c_client,
+  const char* list_name, const size_t list_name_length,
+  const void* dataset)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && list_name != NULL && dataset != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     const DataSet* d = reinterpret_cast<const DataSet*>(dataset);
     std::string lname(list_name, list_name_length);
 
     s->append_to_list(lname, *d);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Delete an aggregation list
-extern "C"
-SRError delete_list(void* c_client, const char* list_name,
-                    const size_t list_name_length)
+extern "C" SRError delete_list(
+  void* c_client, const char* list_name, const size_t list_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && list_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(list_name, list_name_length);
 
     s->delete_list(lname);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Copy an aggregation list
-extern "C"
-SRError copy_list(void* c_client,
-                  const char* src_name, const size_t src_name_length,
-                  const char* dest_name, const size_t dest_name_length)
+extern "C" SRError copy_list(
+  void* c_client,
+  const char* src_name, const size_t src_name_length,
+  const char* dest_name, const size_t dest_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && src_name != NULL && dest_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string sname(src_name, src_name_length);
     std::string dname(dest_name, dest_name_length);
 
     s->copy_list(sname, dname);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Rename an aggregation list
-extern "C"
-SRError rename_list(void* c_client,
-                    const char* src_name, const size_t src_name_length,
-                    const char* dest_name, const size_t dest_name_length)
+extern "C" SRError rename_list(
+  void* c_client,
+  const char* src_name, const size_t src_name_length,
+  const char* dest_name, const size_t dest_name_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && src_name != NULL && dest_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string sname(src_name, src_name_length);
     std::string dname(dest_name, dest_name_length);
 
     s->rename_list(sname, dname);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Get the number of entries in the list
-extern "C"
-SRError get_list_length(void* c_client, const char* list_name,
-                        const size_t list_name_length, int* result_length)
+extern "C" SRError get_list_length(
+  void* c_client,
+  const char* list_name, const size_t list_name_length,
+  int* result_length)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && list_name != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(list_name, list_name_length);
 
     *result_length = s->get_list_length(lname);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Poll list length until length is equal to the provided length
-extern "C"
-SRError poll_list_length(void* c_client, const char* name,
-                         const size_t name_length, int list_length,
-                         int poll_frequency_ms, int num_tries,
-                         bool* poll_result)
+// Poll until list length is equal to the provided length
+extern "C" SRError poll_list_length(
+  void* c_client,
+  const char* name, const size_t name_length,
+  int list_length,
+  int poll_frequency_ms,
+  int num_tries,
+  bool* poll_result)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && poll_result != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(name, name_length);
 
     *poll_result = s->poll_list_length(
       lname, list_length, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
-// Poll list length until length is greater than or equal to the provided length
-extern "C"
-SRError poll_list_length_gte(void* c_client, const char* name,
-                             const size_t name_length, int list_length,
-                             int poll_frequency_ms, int num_tries,
-                             bool* poll_result)
+// Poll until list length is greater than or equal to the provided length
+extern "C" SRError poll_list_length_gte(
+  void* c_client,
+  const char* name, const size_t name_length,
+  int list_length,
+  int poll_frequency_ms,
+  int num_tries,
+  bool* poll_result)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && poll_result != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(name, name_length);
 
     *poll_result = s->poll_list_length_gte(
       lname, list_length, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Poll list length until length is less than or equal to the provided length
-extern "C"
-SRError poll_list_length_lte(void* c_client, const char* name,
-                             const size_t name_length, int list_length,
-                             int poll_frequency_ms, int num_tries,
-                             bool* poll_result)
+extern "C" SRError poll_list_length_lte(
+  void* c_client,
+  const char* name, const size_t name_length,
+  int list_length,
+  int poll_frequency_ms,
+  int num_tries,
+  bool* poll_result)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && name != NULL && poll_result != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(name, name_length);
 
     *poll_result = s->poll_list_length_lte(
       lname, list_length, poll_frequency_ms, num_tries);
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Get datasets from an aggregation list
-extern "C"
-SRError get_datasets_from_list(void* c_client, const char* list_name,
-                               const size_t list_name_length,
-                               void*** datasets, size_t* num_datasets)
+extern "C" SRError get_datasets_from_list(
+  void* c_client,
+  const char* list_name, const size_t list_name_length,
+  void*** datasets,
+  size_t* num_datasets)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && list_name != NULL &&
                     datasets != NULL && num_datasets != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(list_name, list_name_length);
 
@@ -1961,37 +1340,27 @@
       DataSet** alloc = new DataSet*[ndatasets];
       for (size_t i = 0; i < ndatasets; i++) {
         alloc[i] = new DataSet(std::move(result_datasets[i]));
       }
       *datasets = (void**)alloc;
     }
     *num_datasets = ndatasets;
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
 
 // Get a range of datasets (by index) from an aggregation list
-extern "C"
-SRError get_dataset_list_range(void* c_client, const char* list_name,
-                               const size_t list_name_length,
-                               const int start_index, const int end_index,
-                               void*** datasets, size_t* num_datasets)
+extern "C" SRError get_dataset_list_range(
+  void* c_client,
+  const char* list_name, const size_t list_name_length,
+  const int start_index,
+  const int end_index,
+  void*** datasets,
+  size_t* num_datasets)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && list_name != NULL &&
                     datasets != NULL && num_datasets != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(list_name, list_name_length);
 
@@ -2003,63 +1372,67 @@
       DataSet** alloc = new DataSet*[ndatasets];
       for (size_t i = 0; i < ndatasets; i++) {
         alloc[i] = new DataSet(std::move(result_datasets[i]));
       }
       *datasets = (void**)alloc;
     }
     *num_datasets = ndatasets;
-  }
-  catch (const Exception& e) {
-    SRSetLastError(e);
-    result = e.to_error_code();
-  }
-  catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
-  }
-
-  return result;
+  });
 }
+
 // Get a range of datasets (by index) from an aggregation list into an
 // already allocated vector of datasets
-extern "C"
-SRError _get_dataset_list_range_allocated(void* c_client, const char* list_name,
-                               const size_t list_name_length,
-                               const int start_index, const int end_index,
-                               void** datasets)
+extern "C" SRError _get_dataset_list_range_allocated(
+  void* c_client,
+  const char* list_name, const size_t list_name_length,
+  const int start_index,
+  const int end_index,
+  void** datasets)
 {
-  SRError result = SRNoError;
-  try
-  {
+  return MAKE_CLIENT_API({
     // Sanity check params
     SR_CHECK_PARAMS(c_client != NULL && list_name != NULL &&
                     datasets != NULL);
 
     Client* s = reinterpret_cast<Client*>(c_client);
     std::string lname(list_name, list_name_length);
 
     std::vector<DataSet> result_datasets = s->get_dataset_list_range(
       lname, start_index, end_index);
     size_t num_datasets = result_datasets.size();
-    if ( num_datasets != (size_t) (end_index-start_index+1)) {
-      SRSetLastError(SRInternalException(
-        "Returned dataset list is not equal to the requested range"
-      ));
+    if (num_datasets != (size_t)(end_index - start_index + 1)) {
+      throw SRInternalException(
+        "Returned dataset list is not equal to the requested range");
     }
 
     if (num_datasets > 0) {
       for (size_t i = 0; i < num_datasets; i++) {
         datasets[i] = (void*)(new DataSet(std::move(result_datasets[i])));
       }
     }
+  });
+}
+
+// Retrieve a string representation of the client
+const char* client_to_string(void* c_client)
+{
+  static std::string result;
+  try
+  {
+    // Sanity check params
+    SR_CHECK_PARAMS(c_client != NULL);
+
+    Client* s = reinterpret_cast<Client*>(c_client);
+    result = s->to_string();
   }
   catch (const Exception& e) {
     SRSetLastError(e);
-    result = e.to_error_code();
+    result = e.what();
   }
   catch (...) {
-    SRSetLastError(SRInternalException("Unknown exception occurred"));
-    result = SRInternalError;
+    result = "A non-standard exception was encountered while executing ";
+    result += __func__;
+    SRSetLastError(SRInternalException(result));
   }
 
-  return result;
+  return result.c_str();
 }
```

### Comparing `smartredis-0.3.1/src/c/c_error.cpp` & `smartredis-0.4.0/src/c/c_error.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -35,34 +35,22 @@
 // The last error encountered
 static Exception __lastError = Exception("no error");
 
 // Store the last error encountered
 extern "C"
 void SRSetLastError(const Exception& last_error)
 {
-  // Check environment for debug level if we haven't done so yet
-  static bool __debug_level_verbose = false;
-  static bool __debug_level_checked = false;
-  if (!__debug_level_checked)
-  {
-    __debug_level_checked = true;
-    char *dbg_setting = getenv("SMARTREDIS_DEBUG_LEVEL");
-    if (dbg_setting != NULL) {
-      std::string dbgLevel(dbg_setting);
-      __debug_level_verbose = dbgLevel.compare("VERBOSE") == 0;
-    }
-  }
-
-  // Print out the error message if verbose
-  if (__debug_level_verbose && SRNoError != last_error.to_error_code()) {
-    printf("%s\n", last_error.what());
-  }
-
   // Store the last error
   __lastError = last_error;
 }
 
 // Return the last error encountered
 extern "C"
 const char* SRGetLastError()  {
   return __lastError.what();
 }
+
+// Return the location for the last error encountered
+extern "C"
+const char* SRGetLastErrorLocation()  {
+  return __lastError.where();
+}
```

### Comparing `smartredis-0.3.1/src/cpp/addressallcommand.cpp` & `smartredis-0.4.0/src/cpp/addressallcommand.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/addressanycommand.cpp` & `smartredis-0.4.0/src/cpp/addressanycommand.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/addressatcommand.cpp` & `smartredis-0.4.0/src/cpp/addressatcommand.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/client.cpp` & `smartredis-0.4.0/src/cpp/client.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -23,32 +23,43 @@
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include <ctype.h>
+#include <algorithm>
 #include "client.h"
 #include "srexception.h"
+#include "logger.h"
+#include "utility.h"
 
 using namespace SmartRedis;
 
 // Constructor
-Client::Client(bool cluster)
-    : _redis_cluster(cluster ? new RedisCluster() : NULL),
-      _redis(cluster ? NULL : new Redis())
+Client::Client(bool cluster, const std::string& logger_name)
+    : SRObject(logger_name)
 {
+    // Log that a new client has been instantiated
+    log_data(LLDebug, "New client created");
+
+    // Set up Redis server connection
     // A std::bad_alloc exception on the initializer will be caught
     // by the call to new for the client
+    _redis_cluster = (cluster ? new RedisCluster(this) : NULL);
+    _redis = (cluster ? NULL : new Redis(this));
     if (cluster)
         _redis_server =  _redis_cluster;
     else
         _redis_server =  _redis;
+
+    // Initialize key prefixing
     _set_prefixes_from_env();
     _use_tensor_prefix = true;
+    _use_dataset_prefix = true;
     _use_model_prefix = false;
     _use_list_prefix = true;
 }
 
 // Destructor
 Client::~Client()
 {
@@ -59,67 +70,92 @@
     }
     if (_redis != NULL)
     {
         delete _redis;
         _redis = NULL;
     }
     _redis_server = NULL;
+
+    // Log Client destruction
+    log_data(LLDebug, "Client destroyed");
 }
 
 // Put a DataSet object into the database
 void Client::put_dataset(DataSet& dataset)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     CommandList cmds;
     _append_dataset_metadata_commands(cmds, dataset);
     _append_dataset_tensor_commands(cmds, dataset);
     _append_dataset_ack_command(cmds, dataset);
-    _run(cmds);
+    _redis_server->run_in_pipeline(cmds);
 }
 
 // Retrieve a DataSet object from the database
 DataSet Client::get_dataset(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Get the metadata message and construct DataSet
     CommandReply reply = _get_dataset_metadata(name);
 
     // If the reply has no elements, it didn't exist
     if (reply.n_elements() == 0) {
         throw SRKeyException("The requested DataSet, \"" +
                              name + "\", does not exist.");
     }
 
     DataSet dataset(name);
     _unpack_dataset_metadata(dataset, reply);
 
+    // Build the tensor keys
     std::vector<std::string> tensor_names = dataset.get_tensor_names();
+    if (tensor_names.size() == 0)
+        return dataset; // If no tensors, we're done
+    std::vector<std::string> tensor_keys;
+    std::transform(
+        tensor_names.cbegin(),
+        tensor_names.cend(),
+        std::back_inserter(tensor_keys),
+        [this, name](std::string s){
+            return _build_dataset_tensor_key(name, s, true);
+        });
+
+    // Retrieve DataSet tensors
+    PipelineReply tensors = _redis_server->get_tensors(tensor_keys);
 
-    // Retrieve DataSet tensors and fill the DataSet object
-    for(size_t i = 0; i < tensor_names.size(); i++) {
-        // Build the tensor key
-        std::string tensor_key =
-            _build_dataset_tensor_key(name, tensor_names[i], true);
-        // Retrieve tensor and add it to the dataset
-        _get_and_add_dataset_tensor(dataset, tensor_names[i], tensor_key);
+    // Put them into the dataset
+    for (size_t i = 0; i < tensor_names.size(); i++) {
+        _add_dataset_tensor(dataset, tensor_names[i], tensors[i]);
     }
 
     return dataset;
 }
 
 // Rename the current dataset
 void Client::rename_dataset(const std::string& old_name,
                             const std::string& new_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     copy_dataset(old_name, new_name);
     delete_dataset(old_name);
 }
 
 // Clone the dataset to a new name
 void Client::copy_dataset(const std::string& src_name,
                           const std::string& dest_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Get the metadata message and construct DataSet
     CommandReply reply = _get_dataset_metadata(src_name);
     if (reply.n_elements() == 0) {
         throw SRKeyException("The requested DataSet " +
                              src_name + " does not exist.");
     }
     DataSet dataset(src_name);
@@ -138,21 +174,24 @@
     // Update the DataSet name to the destination name
     // so we can reuse the object for placing metadata
     // and ack commands
     dataset.set_name(dest_name);
     CommandList put_meta_cmds;
     _append_dataset_metadata_commands(put_meta_cmds, dataset);
     _append_dataset_ack_command(put_meta_cmds, dataset);
-    (void)_run(put_meta_cmds);
+    (void)_redis_server->run_in_pipeline(put_meta_cmds);
 }
 
 // Delete a DataSet from the database.
 // All tensors and metdata in the DataSet will be deleted.
 void Client::delete_dataset(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     CommandReply reply = _get_dataset_metadata(name);
     if (reply.n_elements() == 0) {
         throw SRRuntimeException("The requested DataSet " +
                                  name + " does not exist.");
     }
 
     DataSet dataset(name);
@@ -180,14 +219,17 @@
 // Put a tensor into the database
 void Client::put_tensor(const std::string& name,
                         void* data,
                         const std::vector<size_t>& dims,
                         const SRTensorType type,
                         const SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_tensor_key(name, false);
 
     TensorBase* tensor = NULL;
     try {
         switch (type) {
             case SRTensorTypeDouble:
                 tensor = new Tensor<double>(key, data, dims, type, mem_layout);
@@ -236,14 +278,17 @@
 // tensor data.
 void Client::get_tensor(const std::string& name,
                         void*& data,
                         std::vector<size_t>& dims,
                         SRTensorType& type,
                         const SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Retrieve the TensorBase from the database
     TensorBase* ptr = _get_tensorbase_obj(name);
 
     // Set the user values
     dims = ptr->dims();
     type = ptr->type();
     data = ptr->data_view(mem_layout);
@@ -259,14 +304,16 @@
  void Client::get_tensor(const std::string& name,
                         void*& data,
                         size_t*& dims,
                         size_t& n_dims,
                         SRTensorType& type,
                         const SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
 
     std::vector<size_t> dims_vec;
     get_tensor(name, data, dims_vec, type, mem_layout);
 
     size_t dims_bytes = sizeof(size_t) * dims_vec.size();
     dims = _dim_queries.allocate_bytes(dims_bytes);
     n_dims = dims_vec.size();
@@ -283,14 +330,17 @@
 // tensor data.
 void Client::unpack_tensor(const std::string& name,
                            void* data,
                            const std::vector<size_t>& dims,
                            const SRTensorType type,
                            const SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (mem_layout == SRMemLayoutContiguous && dims.size() > 1) {
         throw SRRuntimeException("The destination memory space "\
                                  "dimension vector should only "\
                                  "be of size one if the memory "\
                                  "layout is contiguous.");
     }
 
@@ -401,34 +451,43 @@
     tensor = NULL;
 }
 
 // Move a tensor from one name to another name
 void Client::rename_tensor(const std::string& old_name,
                            const std::string& new_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string old_key = _build_tensor_key(old_name, true);
     std::string new_key = _build_tensor_key(new_name, false);
     CommandReply reply = _redis_server->rename_tensor(old_key, new_key);
     if (reply.has_error())
         throw SRRuntimeException("rename_tensor failed");
 }
 
 // Delete a tensor from the database
 void Client::delete_tensor(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_tensor_key(name, true);
     CommandReply reply = _redis_server->delete_tensor(key);
     if (reply.has_error())
         throw SRRuntimeException("delete_tensor failed");
 }
 
 // Copy the tensor from the source name to the destination name
 void Client::copy_tensor(const std::string& src_name,
                          const std::string& dest_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string src_key = _build_tensor_key(src_name, true);
     std::string dest_key = _build_tensor_key(dest_name, false);
     CommandReply reply = _redis_server->copy_tensor(src_key, dest_key);
     if (reply.has_error())
         throw SRRuntimeException("copy_tensor failed");
 }
 
@@ -439,14 +498,17 @@
                                  const std::string& device,
                                  int batch_size,
                                  int min_batch_size,
                                  const std::string& tag,
                                  const std::vector<std::string>& inputs,
                                  const std::vector<std::string>& outputs)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (model_file.size() == 0) {
         throw SRParameterException("model_file is a required "
                                    "parameter of set_model_from_file.");
     }
 
     std::ifstream fin(model_file, std::ios::binary);
     std::ostringstream ostream;
@@ -467,14 +529,17 @@
                                           int num_gpus,
                                           int batch_size,
                                           int min_batch_size,
                                           const std::string& tag,
                                           const std::vector<std::string>& inputs,
                                           const std::vector<std::string>& outputs)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (model_file.size() == 0) {
         throw SRParameterException("model_file is a required "
                                    "parameter of set_model_from_file_multigpu.");
     }
 
     std::ifstream fin(model_file, std::ios::binary);
     std::ostringstream ostream;
@@ -493,14 +558,17 @@
                        const std::string& device,
                        int batch_size,
                        int min_batch_size,
                        const std::string& tag,
                        const std::vector<std::string>& inputs,
                        const std::vector<std::string>& outputs)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (name.size() == 0) {
         throw SRParameterException("name is a required parameter of set_model.");
     }
 
     if (backend.size() == 0) {
         throw SRParameterException("backend is a required "\
                                    "parameter of set_model.");
@@ -531,30 +599,38 @@
     }
     if (device.compare("CPU") != 0 &&
         std::string(device).find("GPU") == std::string::npos) {
         throw SRRuntimeException(device + " is not a valid device.");
     }
 
     std::string key = _build_model_key(name, false);
-    _redis_server->set_model(key, model, backend, device,
-                             batch_size, min_batch_size,
-                             tag, inputs, outputs);
+    auto response = _redis_server->set_model(
+        key, model, backend, device,
+        batch_size, min_batch_size,
+        tag, inputs, outputs);
+    if (response.has_error()) {
+        throw SRInternalException(
+            "An unknown error occurred while setting the model");
+    }
 }
 
 void Client::set_model_multigpu(const std::string& name,
                                 const std::string_view& model,
                                 const std::string& backend,
                                 int first_gpu,
                                 int num_gpus,
                                 int batch_size,
                                 int min_batch_size,
                                 const std::string& tag,
                                 const std::vector<std::string>& inputs,
                                 const std::vector<std::string>& outputs)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (name.size() == 0) {
         throw SRParameterException("name is a required parameter of set_model.");
     }
     if (backend.size() == 0) {
         throw SRParameterException("backend is a required "\
                                    "parameter of set_model.");
     }
@@ -592,14 +668,17 @@
         tag, inputs, outputs);
 }
 
 
 // Retrieve the model from the database
 std::string_view Client::get_model(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string get_key = _build_model_key(name, true);
     CommandReply reply = _redis_server->get_model(get_key);
     if (reply.has_error())
         throw SRRuntimeException("failed to get model from server");
 
     char* model = _model_queries.allocate(reply.str_len());
     if (model == NULL)
@@ -609,14 +688,17 @@
 }
 
 // Set a script from file in the database for future execution
 void Client::set_script_from_file(const std::string& name,
                                   const std::string& device,
                                   const std::string& script_file)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Read the script from the file
     std::ifstream fin(script_file);
     std::ostringstream ostream;
     ostream << fin.rdbuf();
 
     const std::string tmp = ostream.str();
     std::string_view script(tmp.data(), tmp.length());
@@ -628,14 +710,17 @@
 // Set a script from file in the database for future execution
 // in a multi-GPU system
 void Client::set_script_from_file_multigpu(const std::string& name,
                                            const std::string& script_file,
                                            int first_gpu,
                                            int num_gpus)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Read the script from the file
     std::ifstream fin(script_file);
     std::ostringstream ostream;
     ostream << fin.rdbuf();
 
     const std::string tmp = ostream.str();
     std::string_view script(tmp.data(), tmp.length());
@@ -645,33 +730,43 @@
 }
 
 // Set a script from a string buffer in the database for future execution
 void Client::set_script(const std::string& name,
                         const std::string& device,
                         const std::string_view& script)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (device.size() == 0) {
         throw SRParameterException("device is a required "
                                    "parameter of set_script.");
     }
     if (device.compare("CPU") != 0 &&
         std::string(device).find("GPU") == std::string::npos) {
         throw SRRuntimeException(device + " is not a valid device.");
     }
 
     std::string key = _build_model_key(name, false);
-    _redis_server->set_script(key, device, script);
+    auto response = _redis_server->set_script(key, device, script);
+    if (response.has_error()) {
+        throw SRInternalException(
+            "An unknown error occurred while setting the script");
+    }
 }
 
 // Set a script in the database for future execution in a multi-GPU system
 void Client::set_script_multigpu(const std::string& name,
                                  const std::string_view& script,
                                  int first_gpu,
                                  int num_gpus)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (first_gpu < 0) {
         throw SRParameterException("first_gpu must be a non-negative integer.");
     }
     if (num_gpus < 1) {
         throw SRParameterException("num_gpus must be a positive integer.");
     }
 
@@ -692,14 +787,17 @@
 }
 
 // Run a model in the database using the specified input and output tensors
 void Client::run_model(const std::string& name,
                        std::vector<std::string> inputs,
                        std::vector<std::string> outputs)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_model_key(name, true);
 
     if (_use_tensor_prefix) {
         _append_with_get_prefix(inputs);
         _append_with_put_prefix(outputs);
     }
     _redis_server->run_model(key, inputs, outputs);
@@ -710,14 +808,17 @@
 void Client::run_model_multigpu(const std::string& name,
                                 std::vector<std::string> inputs,
                                 std::vector<std::string> outputs,
                                 int offset,
                                 int first_gpu,
                                 int num_gpus)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (first_gpu < 0) {
         throw SRParameterException("first_gpu must be a non-negative integer.");
     }
     if (num_gpus < 1) {
         throw SRParameterException("num_gpus must be a positive integer.");
     }
 
@@ -733,14 +834,17 @@
 
 // Run a script function in the database using the specified input and output tensors
 void Client::run_script(const std::string& name,
                         const std::string& function,
                         std::vector<std::string> inputs,
                         std::vector<std::string> outputs)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_model_key(name, true);
 
     if (_use_tensor_prefix) {
         _append_with_get_prefix(inputs);
         _append_with_put_prefix(outputs);
     }
     _redis_server->run_script(key, function, inputs, outputs);
@@ -752,14 +856,17 @@
                                  const std::string& function,
                                  std::vector<std::string> inputs,
                                  std::vector<std::string> outputs,
                                  int offset,
                                  int first_gpu,
                                  int num_gpus)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (first_gpu < 0) {
         throw SRParameterException("first_gpu must be a non-negative integer");
     }
     if (num_gpus < 1) {
         throw SRParameterException("num_gpus must be a positive integer.");
     }
 
@@ -772,93 +879,120 @@
     _redis_server->run_script_multigpu(
         key, function, inputs, outputs, offset, first_gpu, num_gpus);
 }
 
 // Delete a model from the database
 void Client::delete_model(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_model_key(name, true);
     CommandReply reply = _redis_server->delete_model(key);
 
     if (reply.has_error())
         throw SRRuntimeException("AI.MODELDEL command failed on server");
 }
 
 // Delete a multiGPU model from the database
 void Client::delete_model_multigpu(
     const std::string& name, int first_gpu, int num_gpus)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (first_gpu < 0) {
         throw SRParameterException("first_gpu must be a non-negative integer");
     }
     if (num_gpus < 1) {
         throw SRParameterException("num_gpus must be a positive integer.");
     }
 
     std::string key = _build_model_key(name, true);
     _redis_server->delete_model_multigpu(key, first_gpu, num_gpus);
 }
 
 // Delete a script from the database
 void Client::delete_script(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_model_key(name, true);
     CommandReply reply = _redis_server->delete_script(key);
 
     if (reply.has_error())
         throw SRRuntimeException("AI.SCRIPTDEL command failed on server");
 }
 
 // Delete a multiGPU script from the database
 void Client::delete_script_multigpu(
     const std::string& name, int first_gpu, int num_gpus)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (first_gpu < 0) {
         throw SRParameterException("first_gpu must be a non-negative integer");
     }
     if (num_gpus < 1) {
         throw SRParameterException("num_gpus must be a positive integer.");
     }
 
     std::string key = _build_model_key(name, true);
     _redis_server->delete_script_multigpu(key, first_gpu, num_gpus);
 }
 
 // Check if the key exists in the database
 bool Client::key_exists(const std::string& key)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     return _redis_server->key_exists(key);
 }
 
 // Check if the tensor (or the dataset) exists in the database
 bool Client::tensor_exists(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_tensor_key(name, true);
     return _redis_server->key_exists(key);
 }
 
 // Check if the dataset exists in the database
 bool Client::dataset_exists(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_dataset_ack_key(name, true);
     return _redis_server->hash_field_exists(key, _DATASET_ACK_FIELD);
 }
 
 // Check if the model (or the script) exists in the database
 bool Client::model_exists(const std::string& name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::string key = _build_model_key(name, true);
     return _redis_server->model_key_exists(key);
 }
 
 // Check if the key exists in the database at a specified frequency for a specified number of times
 bool Client::poll_key(const std::string& key,
                       int poll_frequency_ms,
                       int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Check for the key however many times requested
     for (int i = 0; i < num_tries; i++) {
         if (key_exists(key))
             return true;
         std::this_thread::sleep_for(std::chrono::milliseconds(poll_frequency_ms));
     }
 
@@ -867,14 +1001,17 @@
 }
 
 // Check if the model (or script) exists in the database at a specified frequency for a specified number of times.
 bool Client::poll_model(const std::string& name,
                         int poll_frequency_ms,
                         int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Check for the model/script however many times requested
     for (int i = 0; i < num_tries; i++) {
         if (model_exists(name))
             return true;
         std::this_thread::sleep_for(std::chrono::milliseconds(poll_frequency_ms));
     }
 
@@ -883,14 +1020,17 @@
 }
 
 // Check if the tensor exists in the database at a specified frequency for a specified number of times
 bool Client::poll_tensor(const std::string& name,
                          int poll_frequency_ms,
                          int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Check for the tensor however many times requested
     for (int i = 0; i < num_tries; i++) {
         if (tensor_exists(name))
             return true;
         std::this_thread::sleep_for(std::chrono::milliseconds(poll_frequency_ms));
     }
 
@@ -899,28 +1039,34 @@
 }
 
 // Check if the dataset exists in the database at a specified frequency for a specified number of times
 bool Client::poll_dataset(const std::string& name,
                           int poll_frequency_ms,
                           int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Check for the dataset however many times requested
     for (int i = 0; i < num_tries; i++) {
         if (dataset_exists(name))
             return true;
         std::this_thread::sleep_for(std::chrono::milliseconds(poll_frequency_ms));
     }
 
     // If we get here, it was never found
     return false;
 }
 
 // Establish a datasource
 void Client::set_data_source(std::string source_id)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Validate the source prefix
     bool valid_prefix = false;
     size_t num_prefix = _get_key_prefixes.size();
     size_t save_index = -1;
     for (size_t i = 0; i < num_prefix; i++) {
         if (_get_key_prefixes[i].compare(source_id) == 0) {
             valid_prefix = true;
@@ -944,72 +1090,98 @@
 // (e.g. in an ensemble) to form database keys. Prefixes will only be
 // used if they were previously set through the environment variables
 // SSKEYOUT and SSKEYIN. Keys of entities created before this function
 // is called will not be affected. By default, the client does not
 // prefix model and script keys.
 void Client::use_model_ensemble_prefix(bool use_prefix)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _use_model_prefix = use_prefix;
 }
 
 // Set whether names of aggregation lists should be prefixed
 // (e.g. in an ensemble) to form database keys. Prefixes will only be
 // used if they were previously set through the environment variables
 // SSKEYOUT and SSKEYIN. Keys of entities created before this function
 // is called will not be affected. By default, the client prefixes
 // aggregation list keys.
 void Client::use_list_ensemble_prefix(bool use_prefix)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _use_list_prefix = use_prefix;
 }
 
 
-// Set whether names of tensor and dataset entities should be prefixed
+// Set whether names of tensor entities should be prefixed
 // (e.g. in an ensemble) to form database keys. Prefixes will only be used
 // if they were previously set through the environment variables SSKEYOUT
 // and SSKEYIN. Keys of entities created before this function is called
 // will not be affected. By default, the client prefixes tensor and dataset
 // keys with the first prefix specified with the SSKEYIN and SSKEYOUT
 // environment variables.
 void Client::use_tensor_ensemble_prefix(bool use_prefix)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _use_tensor_prefix = use_prefix;
 }
 
+// Set whether names of dataset entities should be prefixed
+// (e.g. in an ensemble) to form database keys. Prefixes will only be used
+// if they were previously set through the environment variables SSKEYOUT
+// and SSKEYIN. Keys of entities created before this function is called
+// will not be affected. By default, the client prefixes dataset
+// keys with the first prefix specified with the SSKEYIN and SSKEYOUT
+// environment variables.
+void Client::use_dataset_ensemble_prefix(bool use_prefix)
+{
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    _use_dataset_prefix = use_prefix;
+}
+
 // Returns information about the given database node
 parsed_reply_nested_map Client::get_db_node_info(std::string address)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Run an INFO EVERYTHING command to get node info
     DBInfoCommand cmd;
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
-
-    cmd.set_exec_address_port(host, port);
+    SRAddress db_address(address);
+    cmd.set_exec_address(db_address);
     cmd << "INFO" << "EVERYTHING";
     CommandReply reply = _run(cmd);
     if (reply.has_error())
         throw SRRuntimeException("INFO EVERYTHING command failed on server");
 
     // Parse the results
     std::string db_node_info(reply.str(), reply.str_len());
     return DBInfoCommand::parse_db_node_info(db_node_info);
 }
 
 // Returns the CLUSTER INFO command reply addressed to a single cluster node.
 parsed_reply_map Client::get_db_cluster_info(std::string address)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (_redis_cluster == NULL)
         throw SRRuntimeException("Cannot run on non-cluster environment");
 
     // Run the CLUSTER INFO command
     ClusterInfoCommand cmd;
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
-
-    cmd.set_exec_address_port(host, port);
+    SRAddress db_address(address);
+    cmd.set_exec_address(db_address);
     cmd << "CLUSTER" << "INFO";
     CommandReply reply = _run(cmd);
     if (reply.has_error())
         throw SRRuntimeException("CLUSTER INFO command failed on server");
 
     // Parse the results
     std::string db_cluster_info(reply.str(), reply.str_len());
@@ -1017,14 +1189,17 @@
 }
 
 // Returns the AI.INFO command reply
 parsed_reply_map Client::get_ai_info(const std::string& address,
                                      const std::string& key,
                                      const bool reset_stat)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Run the command
     CommandReply reply =
         _redis_server->get_model_script_ai_info(address, key, reset_stat);
 
     if (reply.has_error())
         throw SRRuntimeException("AI.INFO command failed on server");
 
@@ -1058,38 +1233,37 @@
     }
     return reply_map;
 }
 
 // Delete all the keys of the given database
 void Client::flush_db(std::string address)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     AddressAtCommand cmd;
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
-    if (host.empty() or port == 0){
-        throw SRRuntimeException(std::string(address) +
-                                 "is not a valid database node address.");
-    }
-    cmd.set_exec_address_port(host, port);
+    SRAddress db_address(address);
+    cmd.set_exec_address(db_address);
     cmd << "FLUSHDB";
 
     CommandReply reply = _run(cmd);
     if (reply.has_error() > 0)
         throw SRRuntimeException("FLUSHDB command failed");
 }
 
 // Read the configuration parameters of a running server
 std::unordered_map<std::string,std::string>
 Client::config_get(std::string expression, std::string address)
 {
-    AddressAtCommand cmd;
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
+    // Track calls to this API function
+    LOG_API_FUNCTION();
 
-    cmd.set_exec_address_port(host, port);
+    AddressAtCommand cmd;
+    SRAddress db_address(address);
+    cmd.set_exec_address(db_address);
     cmd << "CONFIG" << "GET" << expression;
 
     CommandReply reply = _run(cmd);
     if (reply.has_error() > 0)
         throw SRRuntimeException("CONFIG GET command failed");
 
     // parse reply
@@ -1101,44 +1275,49 @@
 
     return reply_map;
 }
 
 // Reconfigure the server
 void Client::config_set(std::string config_param, std::string value, std::string address)
 {
-    AddressAtCommand cmd;
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
+    // Track calls to this API function
+    LOG_API_FUNCTION();
 
-    cmd.set_exec_address_port(host, port);
+    AddressAtCommand cmd;
+    SRAddress db_address(address);
+    cmd.set_exec_address(db_address);
     cmd << "CONFIG" << "SET" << config_param << value;
 
     CommandReply reply = _run(cmd);
     if (reply.has_error() > 0)
         throw SRRuntimeException("CONFIG SET command failed");
 }
 
 void Client::save(std::string address)
 {
-    AddressAtCommand cmd;
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
+    // Track calls to this API function
+    LOG_API_FUNCTION();
 
-    cmd.set_exec_address_port(host, port);
+    AddressAtCommand cmd;
+    SRAddress db_address(address);
+    cmd.set_exec_address(db_address);
     cmd << "SAVE";
 
     CommandReply reply = _run(cmd);
     if (reply.has_error() > 0)
         throw SRRuntimeException("SAVE command failed");
 }
 
 // Append dataset to aggregation list
 void Client::append_to_list(const std::string& list_name,
                             const DataSet& dataset)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Build the list key
     std::string list_key = _build_list_key(list_name, false);
 
     // The aggregation list stores dataset key (not the meta key)
     std::string dataset_key = _build_dataset_key(dataset.get_name(), false);
 
     // Build the command
@@ -1151,14 +1330,17 @@
         throw SRRuntimeException("RPUSH command failed. DataSet could not "\
                                  "be added to the aggregation list.");
 }
 
 // Delete an aggregation list
 void Client::delete_list(const std::string& list_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Build the list key
     std::string list_key = _build_list_key(list_name, true);
 
     // Build the command
     SingleKeyCommand cmd;
     cmd << "DEL" << Keyfield(list_key);
 
@@ -1168,14 +1350,17 @@
         throw SRRuntimeException("DEL command failed.");
 }
 
 // Copy aggregation list
 void Client::copy_list(const std::string& src_name,
                        const std::string& dest_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Check for empty string inputs
     if (src_name.size() == 0) {
         throw SRParameterException("The src_name parameter cannot "\
                                    "be an empty string.");
     }
 
     if (dest_name.size() == 0) {
@@ -1244,25 +1429,28 @@
                                      " contains an empty key, which is "\
                                      "not permitted.");
         }
 
         copy_cmd.add_field_ptr(reply[i].str(), reply[i].str_len());
     }
 
-    CommandReply copy_reply = this->_run(copy_cmd);
+    CommandReply copy_reply = _run(copy_cmd);
 
     if (reply.has_error() > 0)
         throw SRRuntimeException("Dataset aggregation list copy "
                                  "operation failed.");
 }
 
 // Rename an aggregation list
 void Client::rename_list(const std::string& src_name,
                          const std::string& dest_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (src_name.size() == 0) {
         throw SRParameterException("The src_name parameter cannot "\
                                    "be an empty string.");
     }
 
     if (dest_name.size() == 0) {
         throw SRParameterException("The dest_name parameter cannot "\
@@ -1276,16 +1464,19 @@
     copy_list(src_name, dest_name);
     delete_list(src_name);
 }
 
 // Get the length of the list
 int Client::get_list_length(const std::string& list_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Build the list key
-    std::string list_key = _build_list_key(list_name, false);
+    std::string list_key = _build_list_key(list_name, true);
 
     // Build the command
     SingleKeyCommand cmd;
     cmd << "LLEN" << Keyfield(list_key);
 
     // Run the command
     CommandReply reply = _run(cmd);
@@ -1308,42 +1499,51 @@
     return list_length;
 }
 
 // Poll the list length (strictly equal)
 bool Client::poll_list_length(const std::string& name, int list_length,
                               int poll_frequency_ms, int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Enforce positive list length
     if (list_length < 0) {
         throw SRParameterException("A positive value for list_length "\
                                    "must be provided.");
     }
 
     return _poll_list_length(name, list_length, poll_frequency_ms,
                              num_tries, std::equal_to<int>());
 }
 
 // Poll the list length (strictly equal)
 bool Client::poll_list_length_gte(const std::string& name, int list_length,
                                  int poll_frequency_ms, int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Enforce positive list length
     if (list_length < 0) {
         throw SRParameterException("A positive value for list_length "\
                                    "must be provided.");
     }
 
     return _poll_list_length(name, list_length, poll_frequency_ms,
                              num_tries, std::greater_equal<int>());
 }
 
 // Poll the list length (strictly equal)
 bool Client::poll_list_length_lte(const std::string& name, int list_length,
                                  int poll_frequency_ms, int num_tries)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Enforce positive list length
     if (list_length < 0) {
         throw SRParameterException("A positive value for list_length "\
                                    "must be provided.");
     }
 
     return _poll_list_length(name, list_length, poll_frequency_ms,
@@ -1351,51 +1551,59 @@
 
     return false;
 }
 
 // Retrieve datasets in aggregation list
 std::vector<DataSet> Client::get_datasets_from_list(const std::string& list_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (list_name.size() == 0) {
         throw SRParameterException("The list name must have length "\
                                    "greater than zero");
     }
 
     return _get_dataset_list_range(list_name, 0, -1);
 }
 
 // Retrieve a subset of datsets in the aggregation list
 std::vector<DataSet> Client::get_dataset_list_range(const std::string& list_name,
                                                     const int start_index,
                                                     const int end_index)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (list_name.size() == 0) {
         throw SRParameterException("The list name must have length "\
                                    "greater than zero");
     }
 
     return _get_dataset_list_range(list_name, start_index, end_index);
 }
 
 // Set the prefixes that are used for set and get methods using SSKEYIN
 // and SSKEYOUT environment variables.
 void Client::_set_prefixes_from_env()
 {
     // Establish set prefix
-    const char* keyout_p = std::getenv("SSKEYOUT");
-    if (keyout_p != NULL)
-        _put_key_prefix = keyout_p;
+    std::string put_key_prefix;
+    get_config_string(put_key_prefix, "SSKEYOUT", "");
+    if (put_key_prefix.length() > 0)
+        _put_key_prefix = put_key_prefix;
     else
         _put_key_prefix.clear();
 
     // Establish get prefix(es)
-    char* keyin_p = std::getenv("SSKEYIN");
-    if (keyin_p != NULL) {
-        char* a = keyin_p;
-        char* b = a;
+    std::string get_key_prefixes;
+    get_config_string(get_key_prefixes, "SSKEYIN", "");
+    if (get_key_prefixes.length() > 0) {
+        const char* a = get_key_prefixes.c_str();
+        const char* b = a;
         char parse_char = ',';
         while (*b != '\0') {
             if (*b == parse_char) {
                 if (a != b)
                     _get_key_prefixes.push_back(std::string(a, b - a));
                 a = ++b;
             }
@@ -1451,26 +1659,24 @@
 inline CommandReply Client::_get_dataset_metadata(const std::string& name)
 {
     SingleKeyCommand cmd;
     cmd << "HGETALL" << Keyfield(_build_dataset_meta_key(name, true));
     return _run(cmd);
 }
 
-// Retrieve a tensor and add it to the dataset
-inline void Client::_get_and_add_dataset_tensor(DataSet& dataset,
-                                                const std::string& name,
-                                                const std::string& key)
+// Add a retrieved tensor to a dataset
+inline void Client::_add_dataset_tensor(
+    DataSet& dataset,
+    const std::string& name,
+    CommandReply tensor_data)
 {
-    // Run tensor retrieval command
-    CommandReply reply = _redis_server->get_tensor(key);
-
     // Extract tensor properties from command reply
-    std::vector<size_t> reply_dims = GetTensorCommand::get_dims(reply);
-    std::string_view blob = GetTensorCommand::get_data_blob(reply);
-    SRTensorType type = GetTensorCommand::get_data_type(reply);
+    std::vector<size_t> reply_dims = GetTensorCommand::get_dims(tensor_data);
+    std::string_view blob = GetTensorCommand::get_data_blob(tensor_data);
+    SRTensorType type = GetTensorCommand::get_data_type(tensor_data);
 
     // Add tensor to the dataset
     dataset._add_to_tensorpack(name, (void*)blob.data(), reply_dims,
                                type, SRMemLayoutContiguous);
 }
 
 inline std::vector<DataSet>
@@ -1616,39 +1822,39 @@
     return dataset_list;
 }
 
 // Build full formatted key of a tensor, based on current prefix settings.
 inline std::string Client::_build_tensor_key(const std::string& key,
                                              const bool on_db)
 {
-    std::string prefix;
+    std::string prefix("");
     if (_use_tensor_prefix)
         prefix = on_db ? _get_prefix() : _put_prefix();
 
     return prefix + key;
 }
 
 // Build full formatted key of a model or a script,
 // based on current prefix settings.
 inline std::string Client::_build_model_key(const std::string& key,
                                             const bool on_db)
 {
-    std::string prefix;
+    std::string prefix("");
     if (_use_model_prefix)
         prefix = on_db ? _get_prefix() : _put_prefix();
 
     return prefix + key;
 }
 
 // Build full formatted key of a dataset, based on current prefix settings.
 inline std::string Client::_build_dataset_key(const std::string& dataset_name,
                                               const bool on_db)
 {
-    std::string prefix;
-    if (_use_tensor_prefix)
+    std::string prefix("");
+    if (_use_dataset_prefix)
         prefix = on_db ? _get_prefix() : _put_prefix();
 
     return prefix + "{" + dataset_name + "}";
 }
 
 // Create the key for putting or getting a DataSet tensor in the database
 inline std::string
@@ -1903,8 +2109,17 @@
         if (comp_func(get_list_length(name),list_length)) {
             return true;
         }
         std::this_thread::sleep_for(std::chrono::milliseconds(poll_frequency_ms));
     }
 
     return false;
-}
+}
+
+// Create a string representation of the client
+std::string Client::to_string() const
+{
+    std::string result;
+    result = "Client (" + _lname + "):\n";
+    result += _redis_server->to_string();
+    return result;
+}
```

### Comparing `smartredis-0.3.1/src/cpp/clusterinfocommand.cpp` & `smartredis-0.4.0/src/cpp/clusterinfocommand.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/command.cpp` & `smartredis-0.4.0/src/cpp/command.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/commandlist.cpp` & `smartredis-0.4.0/src/cpp/commandlist.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/commandreply.cpp` & `smartredis-0.4.0/src/cpp/commandreply.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/compoundcommand.cpp` & `smartredis-0.4.0/src/cpp/compoundcommand.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/dataset.cpp` & `smartredis-0.4.0/src/cpp/dataset.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,63 +25,85 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include <string_view>
 #include "dataset.h"
 #include "srexception.h"
+#include "logger.h"
+#include "utility.h"
 
 using namespace SmartRedis;
 
 // DataSet constructor
 DataSet::DataSet(const std::string& name)
- : _dsname(name)
+ : SRObject(name), _dsname(name)
 {
-    // NOP
+    // Log that a new DataSet has been instantiated
+    log_data(LLDebug, "New DataSet created");
+}
+
+// DataSet Destructor
+DataSet::~DataSet()
+{
+    // Log DataSet destruction
+    log_data(LLDebug, "DataSet destroyed");
 }
 
 // Add a tensor to the DataSet.
 void DataSet::add_tensor(const std::string& name,
                          void* data,
                          const std::vector<size_t>& dims,
                          const SRTensorType type,
                          SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _add_to_tensorpack(name, data, dims, type, mem_layout);
     _metadata.add_string(".tensor_names", name);
 }
 
 // Add metadata scalar field (non-string) with value to the DataSet.
 // If the field does not exist, it will be created. If the field exists,
 // the value will be appended to existing field.
 void DataSet::add_meta_scalar(const std::string& name,
                               const void* data,
                               const SRMetaDataType type)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _metadata.add_scalar(name, data, type);
 }
 
 // Add metadata string field with value to the DataSet. If the field
 // does not exist, it will be created. If the field exists the value
 // will be appended to existing field.
 void DataSet::add_meta_string(const std::string& name,
                               const std::string& data)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _metadata.add_string(name, data);
 }
 
 // Get the tensor data, dimensions, and type for the tensor in the DataSet.
 // This function will allocate and retain management of the memory for
 // the tensor data.
 void DataSet::get_tensor(const std::string& name,
                          void*& data,
                          std::vector<size_t>& dims,
                          SRTensorType& type,
                          SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     // Clone the tensor in the DataSet
     TensorBase* tensor = _get_tensorbase_obj(name);
     if (tensor == NULL) {
         throw SRRuntimeException("tensor creation failed");
     }
     _tensor_memory.add_tensor(tensor);
     type = tensor->type();
@@ -95,14 +117,17 @@
 void DataSet::get_tensor(const std::string&  name,
                          void*& data,
                          size_t*& dims,
                          size_t& n_dims,
                          SRTensorType& type,
                          SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     std::vector<size_t> dims_vec;
     get_tensor(name, data, dims_vec, type, mem_layout);
 
     // Get number of dimensions
     dims = _dim_queries.allocate(dims_vec.size());
     n_dims = dims_vec.size();
 
@@ -120,78 +145,182 @@
 // tensor data from a DataSet
 void DataSet::unpack_tensor(const std::string& name,
                             void* data,
                             const std::vector<size_t>& dims,
                             const SRTensorType type,
                             SRMemoryLayout mem_layout)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _enforce_tensor_exists(name);
     _tensorpack.get_tensor(name)->fill_mem_space(data, dims, mem_layout);
 }
 
 // Get the metadata scalar field values from the DataSet. The data pointer
 // reference will be pointed to newly allocated memory that will contain all
 // values in the metadata field. The length variable will be set to the number
 // of entries in the allocated memory space to allow for iteration over the values.
 // The TensorType enum will be set to the type of the MetaData field.
 void DataSet::get_meta_scalars(const std::string& name,
                                void*& data,
                                size_t& length,
                                SRMetaDataType& type)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _metadata.get_scalar_values(name, data, length, type);
 }
 
 // Get the metadata scalar field values from the DataSet. The data pointer
 // reference will be pointed to newly allocated memory that will contain all
 // values in the metadata field. The length variable will be set to the number
 // of entries in the allocated memory space to allow for iteration over the values.
 // The TensorType enum will be set to the type of the MetaData field.
 void DataSet::get_meta_strings(const std::string& name,
                                char**& data,
                                size_t& n_strings,
                                size_t*& lengths)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _metadata.get_string_values(name, data, n_strings, lengths);
 }
 
 // Check if the DataSet has a field
-bool DataSet::has_field(const std::string& field_name)
+bool DataSet::has_field(const std::string& field_name) const
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     return _metadata.has_field(field_name);
 }
 
 // Clear all entries in a DataSet field.
 void DataSet::clear_field(const std::string& field_name)
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     _metadata.clear_field(field_name);
 }
 
 // Retrieve the names of the tensors in the DataSet
-std::vector<std::string> DataSet::get_tensor_names()
+std::vector<std::string> DataSet::get_tensor_names() const
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     if (_metadata.has_field(".tensor_names"))
         return _metadata.get_string_values(".tensor_names");
     else
         return std::vector<std::string>();
 
 }
 
+// Retrieve tensor names from the DataSet
+void DataSet::get_tensor_names(
+    char**& data, size_t& n_strings, size_t*& lengths)
+{
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    if (_metadata.has_field(".tensor_names")) {
+        _metadata.get_string_values(
+            ".tensor_names", data, n_strings, lengths);
+    }
+    else {
+        data = NULL;
+        lengths = NULL;
+        n_strings = 0;
+    }
+
+}
+
 // Get the strings in a metadata string field. Because standard C++
 // containers are used, memory management is handled by the returned
-// std::vectorstd::string.
-std::vector<std::string> DataSet::get_meta_strings(const std::string& name)
+// std::vector<std::string>.
+std::vector<std::string> DataSet::get_meta_strings(
+    const std::string& name) const
 {
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
     return _metadata.get_string_values(name);
 }
 
 // Get the Tensor type of the Tensor
-SRTensorType DataSet::get_tensor_type(const std::string& name)
+SRTensorType DataSet::get_tensor_type(const std::string& name) const
 {
-    return _tensorpack.get_tensor(name)->type();
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    // Get the tensor
+    auto tensor = _tensorpack.get_tensor(name);
+    if (tensor == NULL) {
+        throw SRKeyException(
+            "No tensor named " + name + " is in the dataset");
+    }
+
+    // Return its type
+    return tensor->type();
+}
+
+// Retrieve the dimensions of a Tensor in the DataSet
+const std::vector<size_t> DataSet::get_tensor_dims(
+    const std::string& name) const
+{
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    // Get the tensor
+    auto tensor = _tensorpack.get_tensor(name);
+    if (tensor == NULL) {
+        throw SRKeyException(
+            "No tensor named " + name + " is in the dataset");
+    }
+
+    // Return its dimensions
+    return tensor->dims();
+}
+
+// Retrieve the names of all metadata fields in the DataSet
+std::vector<std::string> DataSet::get_metadata_field_names() const
+{
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    return _metadata.get_field_names(true);
+}
+
+// Retrieve metadata field names from the DataSet
+void DataSet::get_metadata_field_names(
+    char**& data, size_t& n_strings, size_t*& lengths)
+{
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    _metadata.get_field_names(data, n_strings, lengths, true);
+}
+
+// Retrieve the data type of a metadata field in the DataSet
+SRMetaDataType DataSet::get_metadata_field_type(
+    const std::string& name) const
+{
+    // Track calls to this API function
+    LOG_API_FUNCTION();
+
+    if (!_metadata.has_field(name)) {
+        throw SRKeyException(
+            "Dataset " + _dsname +
+            " does not contain the field " + name);
+    }
+    return _metadata.get_field_type(name);
 }
 
 // Add a Tensor (not yet allocated) to the TensorPack
 void DataSet::_add_to_tensorpack(const std::string& name,
                                  void* data,
                                  const std::vector<size_t>& dims,
                                  const SRTensorType type,
@@ -255,7 +384,55 @@
 // object has been dynamically allocated, but not yet tracked for memory
 // management in any object.
 TensorBase* DataSet::_get_tensorbase_obj(const std::string& name)
 {
     _enforce_tensor_exists(name);
     return _tensorpack.get_tensor(name)->clone();
 }
+
+// Create a string representation of the DataSet
+std::string DataSet::to_string() const
+{
+    std::string result;
+    result = "DataSet (" + _lname + "):\n";
+
+    // Tensors
+    result += "Tensors:\n";
+    auto it = _tensorpack.tensor_cbegin();
+    int ntensors = 0;
+    for ( ; it != _tensorpack.tensor_cend(); ++it) {
+        ntensors++;
+        result += "  " + (*it)->name() + ":\n";
+        result += "    type: " + ::to_string((*it)->type()) + "\n";
+        auto dims = (*it)->dims();
+        result += "    dimensions: [";
+        size_t ndims = dims.size();
+        for (auto itdims = dims.cbegin(); itdims != dims.cend(); ++itdims) {
+            result += std::to_string(*itdims);
+            if (--ndims > 0)
+                result += ", ";
+        }
+        result += "]\n";
+        result += "    elements: " + std::to_string((*it)->num_values()) + "\n";
+    }
+    if (ntensors == 0) {
+        result += "  none\n";
+    }
+
+    // Metadata
+    result += "Metadata:\n";
+    auto mdnames = get_metadata_field_names();
+    int nmetadata = 0;
+    for (auto itmd = mdnames.cbegin(); itmd != mdnames.cend(); ++itmd) {
+        nmetadata++;
+        result += "  " + (*itmd) + ":\n";
+        result += "    type: "
+                + ::to_string(get_metadata_field_type(*itmd)) + "\n";
+    }
+    if (nmetadata == 0) {
+        result += "  none\n";
+    }
+
+    // Done
+    return result;
+}
+
```

### Comparing `smartredis-0.3.1/src/cpp/dbinfocommand.cpp` & `smartredis-0.4.0/src/cpp/dbinfocommand.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/dbnode.cpp` & `smartredis-0.4.0/src/cpp/dbnode.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -28,23 +28,23 @@
 
 #include "dbnode.h"
 
 using namespace SmartRedis;
 
 // DBNode constructor
 DBNode::DBNode()
-    : ip(""), port(-1), name(""), lower_hash_slot(-1), upper_hash_slot(-1)
+    : address(), name(""), lower_hash_slot(-1), upper_hash_slot(-1)
 {
    // NOP
 }
 
 // DBNode constructor with connection and hash slot information.
-DBNode::DBNode(std::string _ip, std::string _name, uint64_t _port,
+DBNode::DBNode(std::string _name, SRAddress& addr_spec,
                uint64_t l_slot, uint64_t u_slot, std::string _prefix)
-    : ip(_ip), port(_port), name(_name), lower_hash_slot(l_slot),
+    : address(addr_spec), name(_name), lower_hash_slot(l_slot),
       upper_hash_slot(u_slot), prefix(_prefix)
 {
     // NOP
 }
 
 // Less than operator. Returns True if the lower hash slot of this node
 // is less than the other lower hash slot.
```

### Comparing `smartredis-0.3.1/src/cpp/gettensorcommand.cpp` & `smartredis-0.4.0/src/cpp/gettensorcommand.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/keyedcommand.cpp` & `smartredis-0.4.0/src/cpp/keyedcommand.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/metadata.cpp` & `smartredis-0.4.0/src/cpp/metadata.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -230,14 +230,76 @@
         default:
             throw SRRuntimeException("MetaData.get_scalar_values() "\
                                      "requested unknown MetaDataType.");
             break;
     }
 }
 
+// Retrieve the type of a metadata field
+SRMetaDataType MetaData::get_field_type(const std::string& name) const
+{
+    try {
+        // Return the type. If it doesn't exist, the exception below will
+        // be thrown
+        return _field_map.at(name)->type();
+    }
+    catch (std::out_of_range& e) {
+        throw SRKeyException(
+            "The metadata field " + name + " does not exist.");
+    }
+}
+
+// Retrieve a vector of metadata field names
+std::vector<std::string> MetaData::get_field_names(bool skip_internal) const
+{
+    std::vector<std::string> fieldnames;
+    fieldnames.reserve(_field_map.size());
+
+    for (auto mapping : _field_map) {
+        if (skip_internal && mapping.first == ".tensor_names")
+            continue;
+        fieldnames.push_back(mapping.first);
+    }
+    return fieldnames;
+}
+
+// Get metadata field names using a c-style interface
+void MetaData::get_field_names(char**& data,
+                               size_t& n_strings,
+                               size_t*& lengths,
+                               bool skip_internal /*= false*/)
+{
+    // Retrieve the names
+    std::vector<std::string> name_strings = get_field_names(skip_internal);
+
+    // Allocate space to copy the strings
+    n_strings = 0; // Set to zero until all data copied
+    data = _char_array_mem_mgr.allocate(name_strings.size());
+    if (data == NULL)
+        throw SRBadAllocException("name strings array");
+    lengths = _str_len_mem_mgr.allocate(name_strings.size());
+    if (lengths == NULL)
+        throw SRBadAllocException("name string lengths");
+
+    // Copy each metadata string into the string buffer
+    for (size_t i = 0; i < name_strings.size(); i++) {
+        size_t size = name_strings[i].size();
+        char* cstr = _char_mem_mgr.allocate(size + 1);
+        if (cstr == NULL)
+            throw SRBadAllocException("name string data");
+        name_strings[i].copy(cstr, size, 0);
+        cstr[size] = '\0';
+        data[i] = cstr;
+        lengths[i] = size;
+    }
+
+    // Write down the number of strings copied
+    n_strings = name_strings.size();
+}
+
 // Get metadata string field using a c-style interface.
 void MetaData::get_string_values(const std::string& name,
                                  char**& data,
                                  size_t& n_strings,
                                  size_t*& lengths)
 
 {
@@ -267,19 +329,22 @@
 
     // Write down the number of strings copied
     n_strings = field_strings.size();
 }
 
 // Get metadata values string field
 std::vector<std::string>
-MetaData::get_string_values(const std::string& name)
+MetaData::get_string_values(const std::string& name) const
 {
     // Get the field
-    MetadataField* mdf = _field_map[name];
-    if (mdf == NULL) {
+    const MetadataField* mdf = NULL;
+    try {
+        mdf = _field_map.at(name);
+    }
+    catch (std::out_of_range& e) {
         throw SRRuntimeException("The metadata field " + name +
                                  " does not exist.");
     }
 
     // Double-check its type
     if (mdf->type() != SRMetadataTypeString) {
         throw SRRuntimeException("The metadata field " + name +
@@ -287,15 +352,15 @@
     }
 
     // Return the values
     return ((StringField*)mdf)->values();
 }
 
 // This function checks if the DataSet has a field
-bool MetaData::has_field(const std::string& field_name)
+bool MetaData::has_field(const std::string& field_name) const
 {
     return (_field_map.count(field_name) > 0);
 }
 
 // Clear all entries in a DataSet field.
 void MetaData::clear_field(const std::string& field_name)
 {
@@ -402,18 +467,19 @@
     }
     _field_map[field_name] = mdf;
 }
 
 // Allocate new memory to hold metadata field values and return these values
 // via the c-ptr reference being pointed to the newly allocated memory
 template <typename T>
-void MetaData::_get_numeric_field_values(const std::string& name,
-                                         void*& data,
-                                         size_t& n_values,
-                                         SharedMemoryList<T>& mem_list)
+void MetaData::_get_numeric_field_values(
+    const std::string& name,
+    void*& data,
+    size_t& n_values,
+    SharedMemoryList<T>& mem_list)
 {
     // Make sure the field exists
     MetadataField* mdf = _field_map[name];
     if (mdf == NULL) {
         throw SRRuntimeException("Field " + name + " does not exist.");
     }
```

### Comparing `smartredis-0.3.1/src/cpp/metadatafield.cpp` & `smartredis-0.4.0/src/cpp/metadatafield.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -34,17 +34,17 @@
 MetadataField::MetadataField(const std::string& name, SRMetaDataType type)
  : _name(name), _type(type)
 {
     // NOP
 }
 
 // Retrieve the MetadataField name
-std::string MetadataField::name()
+std::string MetadataField::name() const
 {
     return _name;
 }
 
 // Retrieve the MetadataField name
-SRMetaDataType MetadataField::type()
+SRMetaDataType MetadataField::type() const
 {
     return _type;
 }
```

### Comparing `smartredis-0.3.1/src/cpp/multikeycommand.cpp` & `smartredis-0.4.0/src/cpp/multikeycommand.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/nonkeyedcommand.cpp` & `smartredis-0.4.0/src/cpp/nonkeyedcommand.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -28,24 +28,17 @@
 
 #include "nonkeyedcommand.h"
 #include "redisserver.h"
 
 using namespace SmartRedis;
 
 // Set address and port for command to be executed on
-void NonKeyedCommand::set_exec_address_port(std::string address, uint64_t port)
+void NonKeyedCommand::set_exec_address(const SRAddress &addr_spec)
 {
-    _address = address;
-    _port = port;
+    _address = addr_spec;
 }
 
 // Get address that command will be to be executed on
-std::string NonKeyedCommand::get_address()
+SRAddress NonKeyedCommand::get_address()
 {
     return _address;
 }
-
-// Get port that command will be to be executed on
-uint64_t NonKeyedCommand::get_port()
-{
-    return _port;
-}
```

### Comparing `smartredis-0.3.1/src/cpp/pipelinereply.cpp` & `smartredis-0.4.0/src/cpp/pipelinereply.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/redis.cpp` & `smartredis-0.4.0/src/cpp/redis.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -24,30 +24,37 @@
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include "redis.h"
 #include "srexception.h"
+#include "utility.h"
+#include "srobject.h"
 
 using namespace SmartRedis;
 
 // Redis constructor.
-Redis::Redis() : RedisServer()
+Redis::Redis(const SRObject* context)
+    : RedisServer(context)
 {
-    std::string address_port = _get_ssdb();
-    _add_to_address_map(address_port);
-    _connect(address_port);
+    SRAddress db_address(_get_ssdb());
+    // Remember whether it's a unix domain socket for later
+    _is_domain_socket = !db_address._is_tcp;
+    _add_to_address_map(db_address);
+    _connect(db_address);
 }
 
 // Redis constructor. Uses address provided to constructor instead of environment variables
-Redis::Redis(std::string address_port) : RedisServer()
+Redis::Redis(const SRObject* context, std::string addr_spec)
+    : RedisServer(context)
 {
-    _add_to_address_map(address_port);
-    _connect(address_port);
+    SRAddress db_address(addr_spec);
+    _add_to_address_map(db_address);
+    _connect(db_address);
 }
 
 // Redis destructor
 Redis::~Redis()
 {
     if (_redis != NULL) {
         delete _redis;
@@ -68,17 +75,17 @@
 // Run a compound Command on the server
 CommandReply Redis::run(CompoundCommand& cmd){
     return _run(cmd);
 }
 
 // Run an address-at Command on the server
 CommandReply Redis::run(AddressAtCommand& cmd){
-    if (not is_addressable(cmd.get_address(), cmd.get_port()))
-        throw SRRuntimeException("The provided host and port do not match "\
-                                 "the host and port used to initialize the "\
+    if (!is_addressable(cmd.get_address()))
+        throw SRRuntimeException("The provided address does not match "\
+                                 "the address used to initialize the "\
                                  "non-cluster client connection.");
     return this->_run(cmd);
 }
 
 // Run an address-any Command on the server
 CommandReply Redis::run(AddressAnyCommand& cmd){
     return _run(cmd);
@@ -152,18 +159,17 @@
         throw SRRuntimeException("Error encountered while checking "\
                                  "for existence of hash field " +
                                  field + " at key " + key);
     return (bool)reply.integer();
 }
 
 // Check if address is valid
-bool Redis::is_addressable(const std::string& address,
-                           const uint64_t& port)
+bool Redis::is_addressable(const SRAddress& address) const
 {
-    return _address_node_map.find(address + ":" + std::to_string(port)) !=
+    return _address_node_map.find(address.to_string()) !=
         _address_node_map.end();
 }
 
 // Put a Tensor on the server
 CommandReply Redis::put_tensor(TensorBase& tensor)
 {
     // Build the command
@@ -182,14 +188,30 @@
     GetTensorCommand cmd;
     cmd << "AI.TENSORGET" << Keyfield(key) << "META" << "BLOB";
 
     // Run it
     return run(cmd);
 }
 
+// Get a list of Tensor from the server
+PipelineReply Redis::get_tensors(const std::vector<std::string>& keys)
+{
+    // Build up the commands to get the tensors
+    CommandList cmdlist; // This just holds the memory
+    std::vector<Command*> cmds;
+    for (auto it = keys.begin(); it != keys.end(); ++it) {
+        GetTensorCommand* cmd = cmdlist.add_command<GetTensorCommand>();
+        (*cmd) << "AI.TENSORGET" << Keyfield(*it) << "META" << "BLOB";
+        cmds.push_back(cmd);
+    }
+
+    // Run them via pipeline
+    return _run_pipeline(cmds);
+}
+
 // Rename a tensor in the database
 CommandReply Redis::rename_tensor(const std::string& key,
                                   const std::string& new_key)
 {
     // Build the command
     MultiKeyCommand cmd;
     cmd << "RENAME" << Keyfield(key) << Keyfield(new_key);
@@ -322,15 +344,15 @@
 {
     // Store a copy of the model for each GPU
     CommandReply result;
     for (int i = first_gpu; i < num_gpus; i++) {
         std::string device = "GPU:" + std::to_string(i);
         std::string model_key = name + "." + device;
         result = set_model(
-            name, model_key, backend, device, batch_size, min_batch_size, tag, inputs, outputs);
+            model_key, model, backend, device, batch_size, min_batch_size, tag, inputs, outputs);
         if (result.has_error() > 0) {
             throw SRRuntimeException("Failed to set model for GPU " + std::to_string(i));
         }
     }
 
     // Add a version for get_model to find
     result = set_model(
@@ -381,16 +403,16 @@
 // Run a model in the database using the specified input and output tensors
 CommandReply Redis::run_model(const std::string& key,
                               std::vector<std::string> inputs,
                               std::vector<std::string> outputs)
 {
     // Check for a non-default timeout setting
     int run_timeout;
-    _init_integer_from_env(run_timeout, _MODEL_TIMEOUT_ENV_VAR,
-                           _DEFAULT_MODEL_TIMEOUT);
+    get_config_integer(run_timeout, _MODEL_TIMEOUT_ENV_VAR,
+                       _DEFAULT_MODEL_TIMEOUT);
 
     // Build the command
     CompoundCommand cmd;
     cmd << "AI.MODELEXECUTE" << Keyfield(key)
         << "INPUTS" << std::to_string(inputs.size()) << inputs
         << "OUTPUTS" << std::to_string(outputs.size()) << outputs
         << "TIMEOUT" << std::to_string(run_timeout);
@@ -545,28 +567,25 @@
 
 // Retrieve the model and script AI.INFO
 CommandReply Redis::get_model_script_ai_info(const std::string& address,
                                              const std::string& key,
                                              const bool reset_stat)
 {
     AddressAtCommand cmd;
-
-    // Parse the host and port
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
+    SRAddress db_address(address);
 
     // Determine the prefix we need for the model or script
-    if (!is_addressable(host, port)) {
-        throw SRRuntimeException("The provided host and port do not match "\
-                                 "the host and port used to initialize the "\
+    if (!is_addressable(db_address)) {
+        throw SRRuntimeException("The provided address does not match "\
+                                 "the address used to initialize the "\
                                  "non-cluster client connection.");
     }
 
     //Build the Command
-    cmd.set_exec_address_port(host, port);
+    cmd.set_exec_address(db_address);
     cmd << "AI.INFO" << Keyfield(key);
 
     // Optionally add RESETSTAT to the command
     if (reset_stat) {
         cmd << "RESETSTAT";
     }
 
@@ -589,29 +608,35 @@
         }
         catch (SmartRedis::Exception& e) {
             // Exception is already prepared, just propagate it
             throw;
         }
         catch (sw::redis::IoError &e) {
             // For an error from Redis, retry unless we're out of chances
+            std::string message("Redis IO error when executing command: ");
+            message += e.what();
             if (i == _command_attempts) {
-                throw SRDatabaseException(
-                    std::string("Redis IO error when executing command: ") +
-                    e.what());
+                throw SRDatabaseException(message);
+            }
+            // Else log, retry, and fall through for a retry
+            else {
+                _context->log_error(LLInfo, message);
             }
-            // else, Fall through for a retry
         }
         catch (sw::redis::ClosedError &e) {
             // For an error from Redis, retry unless we're out of chances
+            std::string message("Redis Closed error when executing command: ");
+            message += e.what();
             if (i == _command_attempts) {
-                throw SRDatabaseException(
-                    std::string("Redis Closed error when executing command: ") +
-                    e.what());
+                throw SRDatabaseException(message);
+            }
+            // Else log, retry, and fall through for a retry
+            else {
+                _context->log_error(LLInfo, message);
             }
-            // else, Fall through for a retry
         }
         catch (sw::redis::Error &e) {
             // For other errors from Redis, report them immediately
             throw SRRuntimeException(
                 std::string("Redis error when executing command: ") +
                 e.what());
         }
@@ -633,30 +658,25 @@
         std::this_thread::sleep_for(std::chrono::milliseconds(_command_interval));
     }
 
     // If we get here, we've run out of retry attempts
     throw SRTimeoutException("Unable to execute command" + cmd.first_field());
 }
 
-inline void Redis::_add_to_address_map(std::string address_port)
+inline void Redis::_add_to_address_map(SRAddress& db_address)
 {
-    if (address_port.rfind("tcp://", 0) == 0)
-        address_port = address_port.substr(6, std::string::npos);
-    else if (address_port.rfind("unix://", 0) == 0)
-        address_port = address_port.substr(7, std::string::npos);
-
-    _address_node_map.insert({address_port, nullptr});
+    _address_node_map.insert({db_address.to_string(), nullptr});
 }
 
-inline void Redis::_connect(std::string address_port)
+inline void Redis::_connect(SRAddress& db_address)
 {
     for (int i = 1; i <= _connection_attempts; i++) {
         try {
             // Try to create the sw::redis::Redis object
-            _redis = new sw::redis::Redis(address_port);
+            _redis = new sw::redis::Redis(db_address.to_string(true));
 
             // Attempt to have the sw::redis::Redis object
             // make a connection using the PING command
             if (_redis->ping().compare("PONG") == 0) {
                 return;
             }
         }
@@ -670,18 +690,22 @@
         }
         catch (sw::redis::Error& e) {
             // For an error from Redis, retry unless we're out of chances
             if (_redis != NULL) {
                 delete _redis;
                 _redis = NULL;
             }
+            std::string message("Unable to connect to backend database: ");
+            message += e.what();
             if (i == _connection_attempts) {
-                throw SRDatabaseException(
-                    std::string("Unable to connect to backend database: ") +
-                                e.what());
+                throw SRDatabaseException(message);
+            }
+            // Else log, retry, and fall through for a retry
+            else {
+                _context->log_error(LLInfo, message);
             }
         }
         catch (std::exception& e) {
             // Should never hit this, so bail immediately if we do
             if (_redis != NULL) {
                 delete _redis;
                 _redis = NULL;
@@ -712,7 +736,102 @@
         }
     }
 
     // If we get here, we've run out of retry attempts
     throw SRTimeoutException(std::string("Connection attempt failed after ") +
                              std::to_string(_connection_attempts) + "tries");
 }
+
+// Run a CommandList via a Pipeline
+PipelineReply Redis::run_in_pipeline(CommandList& cmdlist)
+{
+    // Convert from CommandList to vector
+    std::vector<Command*> cmds;
+    for (auto it = cmdlist.begin(); it != cmdlist.end(); ++it) {
+        cmds.push_back(*it);
+    }
+
+    // Run the commands
+    return _run_pipeline(cmds);
+}
+
+// Build and run unordered pipeline
+PipelineReply Redis::_run_pipeline(std::vector<Command*>& cmds)
+{
+    PipelineReply reply;
+    for (int i = 1; i <= _command_attempts; i++) {
+        try {
+            // Get pipeline object for shard (no new connection)
+            auto pipeline = _redis->pipeline(false);
+
+            // Loop over all commands and add to the pipeline
+            for (size_t i = 0; i < cmds.size(); i++) {
+                // Add the commands to the pipeline
+                pipeline.command(cmds[i]->cbegin(), cmds[i]->cend());
+            }
+
+            // Execute the pipeline
+            reply = pipeline.exec();
+
+            // Check the replies
+            if (reply.has_error()) {
+                throw SRRuntimeException("Redis failed to execute the pipeline");
+            }
+
+            // If we get here, it all worked
+            return reply;
+        }
+        catch (SmartRedis::Exception& e) {
+            // Exception is already prepared, just propagate it
+            throw;
+        }
+        catch (sw::redis::IoError &e) {
+            // For an error from Redis, retry unless we're out of chances
+            if (i == _command_attempts) {
+                throw SRDatabaseException(
+                    std::string("Redis IO error when executing the pipeline: ") +
+                    e.what());
+            }
+            // else, Fall through for a retry
+        }
+        catch (sw::redis::ClosedError &e) {
+            // For an error from Redis, retry unless we're out of chances
+            if (i == _command_attempts) {
+                throw SRDatabaseException(
+                    std::string("Redis Closed error when executing the "\
+                                "pipeline: ") + e.what());
+            }
+            // else, Fall through for a retry
+        }
+        catch (sw::redis::Error &e) {
+            // For other errors from Redis, report them immediately
+            throw SRRuntimeException(
+                std::string("Redis error when executing the pipeline: ") +
+                    e.what());
+        }
+        catch (std::exception& e) {
+            // Should never hit this, so bail immediately if we do
+            throw SRInternalException(
+                std::string("Unexpected exception executing the pipeline: ") +
+                    e.what());
+        }
+        catch (...) {
+            // Should never hit this, so bail immediately if we do
+            throw SRInternalException(
+                "Non-standard exception encountered executing the pipeline");
+        }
+
+        // Sleep before the next attempt
+        std::this_thread::sleep_for(std::chrono::milliseconds(_command_interval));
+    }
+
+    // If we get here, we've run out of retry attempts
+    throw SRTimeoutException("Unable to execute pipeline");
+}
+
+// Create a string representation of the Redis connection
+std::string Redis::to_string() const
+{
+    std::string result("Non-clustered Redis connection:\n");
+    result += RedisServer::to_string();
+    return result;
+}
```

### Comparing `smartredis-0.3.1/src/cpp/rediscluster.cpp` & `smartredis-0.4.0/src/cpp/rediscluster.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -26,39 +26,48 @@
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include "rediscluster.h"
 #include "nonkeyedcommand.h"
 #include "keyedcommand.h"
 #include "srexception.h"
+#include "utility.h"
+#include "srobject.h"
 
 using namespace SmartRedis;
 
 // RedisCluster constructor
-RedisCluster::RedisCluster() : RedisServer()
+RedisCluster::RedisCluster(const SRObject* context)
+    : RedisServer(context)
 {
-    std::string address_port = _get_ssdb();
-    _connect(address_port);
+    SRAddress db_address(_get_ssdb());
+    if (!db_address._is_tcp) {
+        throw SRRuntimeException("Unix Domain Socket is not supported with clustered Redis");
+    }
+    _is_domain_socket = false;
+    _connect(db_address);
     _map_cluster();
-    if (_address_node_map.count(address_port) > 0)
-        _last_prefix = _address_node_map.at(address_port)->prefix;
+    if (_address_node_map.count(db_address.to_string()) > 0)
+        _last_prefix = _address_node_map.at(db_address.to_string())->prefix;
     else if (_db_nodes.size() > 0)
         _last_prefix = _db_nodes[0].prefix;
     else
         throw SRRuntimeException("Cluster mapping failed in client initialization");
 }
 
 // RedisCluster constructor. Uses address provided to constructor instead of
 // environment variables
-RedisCluster::RedisCluster(std::string address_port) : RedisServer()
+RedisCluster::RedisCluster(const SRObject* context, std::string address_spec)
+    : RedisServer(context)
 {
-    _connect(address_port);
+    SRAddress db_address(address_spec);
+    _connect(db_address);
     _map_cluster();
-    if (_address_node_map.count(address_port) > 0)
-        _last_prefix = _address_node_map.at(address_port)->prefix;
+    if (_address_node_map.count(db_address.to_string()) > 0)
+        _last_prefix = _address_node_map.at(db_address.to_string())->prefix;
     else if (_db_nodes.size() > 0)
         _last_prefix = _db_nodes[0].prefix;
     else
         throw SRRuntimeException("Cluster mapping failed in client initialization");
 }
 
 // RedisCluster destructor
@@ -107,17 +116,17 @@
     return _run(cmd, db_prefix);
 }
 
 // Run a non-keyed Command that addresses the given db node on the server
 CommandReply RedisCluster::run(AddressAtCommand& cmd)
 {
     std::string db_prefix;
-    if (is_addressable(cmd.get_address(), cmd.get_port()))
-        db_prefix = _address_node_map.at(cmd.get_address() + ":"
-                    + std::to_string(cmd.get_port()))->prefix;
+    SRAddress address(cmd.get_address());
+    if (is_addressable(address))
+        db_prefix = _address_node_map.at(address.to_string())->prefix;
     else
         throw SRRuntimeException("Redis has failed to find database");
 
     return _run(cmd, db_prefix);
 }
 
 // Run a non-keyed Command that addresses any db node on the server
@@ -151,15 +160,15 @@
     CommandReply reply;
     for ( ; node != _db_nodes.cend(); node++) {
         // swap in a replacement segment for each one
         std::string new_field = "{" + node->prefix + "}." + field;
         cmd.set_field_at(new_field, cmd.key_index, true);
 
         // Execute the updated command
-        cmd.set_exec_address_port(node->ip, node->port);
+        cmd.set_exec_address(node->address);
         reply = _run(cmd, node->prefix);
         if (reply.has_error() > 0)
             break; // Short-circuit failure on error
     }
     return reply;
 }
 
@@ -344,19 +353,18 @@
         throw SRRuntimeException("Error encountered while checking "\
                                  "for existence of hash field " +
                                  field + " at key " + key);
     return (bool)reply.integer();
 }
 
 // Check if a key exists in the database
-bool RedisCluster::is_addressable(const std::string& address,
-                                  const uint64_t& port)
+bool RedisCluster::is_addressable(const SRAddress& address) const
 {
-    std::string addr = address + ":" + std::to_string(port);
-    return _address_node_map.find(addr) != _address_node_map.end();
+    return _address_node_map.find(address.to_string()) !=
+        _address_node_map.end();
 }
 
 // Put a Tensor on the server
 CommandReply RedisCluster::put_tensor(TensorBase& tensor)
 {
     // Build the command
     SingleKeyCommand cmd;
@@ -374,14 +382,34 @@
     GetTensorCommand cmd;
     cmd << "AI.TENSORGET"<< Keyfield(key) << "META" << "BLOB";
 
     // Run it
     return run(cmd);
 }
 
+// Get a list of Tensor from the server
+PipelineReply RedisCluster::get_tensors(const std::vector<std::string>& keys)
+{
+    // Build up the commands to get the tensors
+    CommandList cmdlist; // This just holds the memory
+    std::vector<Command*> cmds;
+    for (auto it = keys.begin(); it != keys.end(); ++it) {
+        GetTensorCommand* cmd = cmdlist.add_command<GetTensorCommand>();
+        (*cmd) << "AI.TENSORGET" << Keyfield(*it) << "META" << "BLOB";
+        cmds.push_back(cmd);
+    }
+
+    // Get the shard index for the first key
+    size_t db_index = _get_db_node_index(keys[0]);
+    std::string shard_prefix = _db_nodes[db_index].prefix;
+
+    // Run them via pipeline
+    return _run_pipeline(cmds, shard_prefix);
+}
+
 // Rename a tensor in the database
 CommandReply RedisCluster::rename_tensor(const std::string& key,
                                          const std::string& new_key)
 {
     // Check whether we have to switch hash slots
     uint16_t key_hash_slot = _get_hash_slot(key);
     uint16_t new_key_hash_slot = _get_hash_slot(new_key);
@@ -608,16 +636,16 @@
 // Run a model in the database using the specified input and output tensors
 CommandReply RedisCluster::run_model(const std::string& model_name,
                                      std::vector<std::string> inputs,
                                      std::vector<std::string> outputs)
 {
     // Check for a non-default timeout setting
     int run_timeout;
-    _init_integer_from_env(run_timeout, _MODEL_TIMEOUT_ENV_VAR,
-                           _DEFAULT_MODEL_TIMEOUT);
+    get_config_integer(run_timeout, _MODEL_TIMEOUT_ENV_VAR,
+                       _DEFAULT_MODEL_TIMEOUT);
 
     /*  For this version of run model, we have to copy all
         input and output tensors, so we will randomly select
         a model.  We can't use rand, because MPI would then
         have the same random number across all ranks.  Instead
         We will choose it based on the db of the first input tensor.
     */
@@ -885,32 +913,27 @@
 
 // Retrieve the model and script AI.INFO
 CommandReply RedisCluster::get_model_script_ai_info(const std::string& address,
                                                     const std::string& key,
                                                     const bool reset_stat)
 {
     AddressAtCommand cmd;
-
-    // Parse the host and port
-    std::string host = cmd.parse_host(address);
-    uint64_t port = cmd.parse_port(address);
+    SRAddress db_address(address);
 
     // Determine the prefix we need for the model or script
-    if (!is_addressable(host, port)) {
-        throw SRRuntimeException("The provided host and port does "\
+    if (!is_addressable(db_address)) {
+        throw SRRuntimeException("The provided address does "\
                                  "not match a cluster shard address.");
     }
 
-    std::string host_port = host + ":" + std::to_string(port);
-    std::string db_prefix = _address_node_map.at(host_port)->prefix;
-
+    std::string db_prefix = _address_node_map.at(db_address.to_string())->prefix;
     std::string prefixed_key = "{" + db_prefix + "}." + key;
 
     // Build the Command
-    cmd.set_exec_address_port(host, port);
+    cmd.set_exec_address(db_address);
     cmd << "AI.INFO" << Keyfield(prefixed_key);
 
     // Optionally add RESETSTAT to the command
     if (reset_stat) {
         cmd << "RESETSTAT";
     }
 
@@ -938,29 +961,35 @@
         }
         catch (SmartRedis::Exception& e) {
             // Exception is already prepared, just propagate it
             throw;
         }
         catch (sw::redis::IoError &e) {
             // For an error from Redis, retry unless we're out of chances
+            std::string message("Redis IO error when executing command: ");
+            message += e.what();
             if (i == _command_attempts) {
-                throw SRDatabaseException(
-                    std::string("Redis IO error when executing command: ") +
-                    e.what());
+                throw SRDatabaseException(message);
+            }
+            // Else log, retry, and fall through for a retry
+            else {
+                _context->log_error(LLInfo, message);
             }
-            // else, Fall through for a retry
         }
         catch (sw::redis::ClosedError &e) {
             // For an error from Redis, retry unless we're out of chances
+            std::string message("Redis Closed error when executing command: ");
+            message += e.what();
             if (i == _command_attempts) {
-                throw SRDatabaseException(
-                    std::string("Redis Closed error when executing command: ") +
-                    e.what());
+                throw SRDatabaseException(message);
+            }
+            // Else log, retry, and fall through for a retry
+            else {
+                _context->log_error(LLInfo, message);
             }
-            // else, Fall through for a retry
         }
         catch (sw::redis::Error &e) {
             // For other errors from Redis, report them immediately
             throw SRRuntimeException(
                 std::string("Redis error when executing command: ") +
                 e.what());
         }
@@ -982,36 +1011,39 @@
     }
 
     // If we get here, we've run out of retry attempts
     throw SRTimeoutException("Unable to execute command " + cmd.first_field());
 }
 
 // Connect to the cluster at the address and port
-inline void RedisCluster::_connect(std::string address_port)
+inline void RedisCluster::_connect(SRAddress& db_address)
 {
     for (int i = 1; i <= _connection_attempts; i++) {
         try {
             // Attempt the connection
-            _redis_cluster = new sw::redis::RedisCluster(address_port);
+            _redis_cluster = new sw::redis::RedisCluster(db_address.to_string(true));
             return;
         }
         catch (std::bad_alloc& e) {
             // On a memory error, bail immediately
             _redis_cluster = NULL;
             throw SRBadAllocException("RedisCluster connection");
         }
         catch (sw::redis::Error& e) {
             // For an error from Redis, retry unless we're out of chances
             _redis_cluster = NULL;
+            std::string message("Unable to connect to backend database: ");
+            message += e.what();
             if (i == _connection_attempts) {
-                throw SRDatabaseException(
-                    std::string("Unable to connect to backend database: ") +
-                    e.what());
+                throw SRDatabaseException(message);
+            }
+            // Else log, retry, and fall through for a retry
+            else {
+                _context->log_error(LLInfo, message);
             }
-            // Else, fall through to retry
         }
         catch (std::exception& e) {
             // Should never hit this, so bail immediately if we do
             _redis_cluster = NULL;
             throw SRInternalException(
                 std::string("Unexpected exception while connecting: ") +
                 e.what());
@@ -1097,32 +1129,32 @@
 inline void RedisCluster::_parse_reply_for_slots(CommandReply& reply)
 {
     /* Each reply element of the main message, of which there should
     be n_db_nodes, is:
     0) (integer) min slot
     1) (integer) max slot
     2) 0) "ip address"
-       1) (integer) port
+       1) (integer) port   (note that for clustered Redis, this will always be a TCP address)
        2) "name"
     */
     size_t n_db_nodes = reply.n_elements();
     _db_nodes = std::vector<DBNode>(n_db_nodes);
 
     for (size_t i = 0; i < n_db_nodes; i++) {
         _db_nodes[i].lower_hash_slot = reply[i][0].integer();
         _db_nodes[i].upper_hash_slot = reply[i][1].integer();
-        _db_nodes[i].ip = std::string(reply[i][2][0].str(),
+        _db_nodes[i].address._is_tcp = true;
+        _db_nodes[i].address._tcp_host = std::string(reply[i][2][0].str(),
                                             reply[i][2][0].str_len());
-        _db_nodes[i].port = reply[i][2][1].integer();
+        _db_nodes[i].address._tcp_port = reply[i][2][1].integer();
         _db_nodes[i].name = std::string(reply[i][2][2].str(),
                                               reply[i][2][2].str_len());
         _db_nodes[i].prefix = _get_crc16_prefix(_db_nodes[i].lower_hash_slot);
-        _address_node_map.insert({_db_nodes[i].ip + ":"
-                                    + std::to_string(_db_nodes[i].port),
-                                    &_db_nodes[i]});
+        _address_node_map.insert({_db_nodes[i].address.to_string(),
+                                  &_db_nodes[i]});
     }
 
     //Put the vector of db nodes in order based on lower hash slot
     std::sort(_db_nodes.begin(), _db_nodes.end());
 }
 
 // Perform inverse CRC16 XOR and shifts
@@ -1328,18 +1360,38 @@
             max_hash = hash_slot_tally[i];
             db = &(_db_nodes[i]);
         }
     }
     return db;
 }
 
+// Run a CommandList via a Pipeline
+PipelineReply RedisCluster::run_in_pipeline(CommandList& cmdlist)
+{
+    // Convert from CommandList to vector and grab the shard along
+    // the way
+    std::vector<Command*> cmds;
+    std::string shard_prefix = _db_nodes[0].prefix;
+    bool shard_found = false;
+    for (auto it = cmdlist.begin(); it != cmdlist.end(); ++it) {
+        cmds.push_back(*it);
+        if (!shard_found && (*it)->has_keys()) {
+            shard_prefix = _get_db_node_prefix(*(*it));
+            shard_found = true;
+        }
+    }
+
+    // Run the commands
+    return _run_pipeline(cmds, shard_prefix);
+}
+
 // Build and run unordered pipeline
-PipelineReply
-RedisCluster::_run_pipeline(std::vector<Command*>& cmds,
-                            std::string& shard_prefix)
+PipelineReply RedisCluster::_run_pipeline(
+    std::vector<Command*>& cmds,
+    std::string& shard_prefix)
 {
     PipelineReply reply;
     for (int i = 1; i <= _command_attempts; i++) {
         try {
             // Get pipeline object for shard (no new connection)
             sw::redis::Pipeline pipeline =
                 _redis_cluster->pipeline(shard_prefix, false);
@@ -1353,14 +1405,17 @@
             // Execute the pipeline
             reply = pipeline.exec();
 
             // Check the replies
             if (reply.has_error()) {
                 throw SRRuntimeException("Redis failed to execute the pipeline");
             }
+
+            // If we get here, it all worked
+            return reply;
         }
         catch (SmartRedis::Exception& e) {
             // Exception is already prepared, just propagate it
             throw;
         }
         catch (sw::redis::IoError &e) {
             // For an error from Redis, retry unless we're out of chances
@@ -1396,18 +1451,20 @@
             // Should never hit this, so bail immediately if we do
             throw SRInternalException(
                 "Non-standard exception encountered executing the pipeline");
         }
 
         // Sleep before the next attempt
         std::this_thread::sleep_for(std::chrono::milliseconds(_command_interval));
-
-        // Return the reply
-        return reply;
     }
 
     // If we get here, we've run out of retry attempts
     throw SRTimeoutException("Unable to execute pipeline");
+}
 
-    // Return the reply
-    return reply;
-}
+// Create a string representation of the Redis connection
+std::string RedisCluster::to_string() const
+{
+    std::string result("Clustered Redis connection:\n");
+    result += RedisServer::to_string();
+    return result;
+}
```

### Comparing `smartredis-0.3.1/src/cpp/redisserver.cpp` & `smartredis-0.4.0/src/cpp/redisserver.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -25,155 +25,118 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include <ctype.h>
 #include "redisserver.h"
 #include "srexception.h"
+#include "utility.h"
+#include "srobject.h"
 
 using namespace SmartRedis;
 
 // RedisServer constructor
-RedisServer::RedisServer()
-    : _gen(_rd())
+RedisServer::RedisServer(const SRObject* context)
+    : _context(context), _gen(_rd())
 {
-    _init_integer_from_env(_connection_timeout, _CONN_TIMEOUT_ENV_VAR,
-                           _DEFAULT_CONN_TIMEOUT);
-    _init_integer_from_env(_connection_interval, _CONN_INTERVAL_ENV_VAR,
-                           _DEFAULT_CONN_INTERVAL);
-    _init_integer_from_env(_command_timeout, _CMD_TIMEOUT_ENV_VAR,
-                           _DEFAULT_CMD_TIMEOUT);
-    _init_integer_from_env(_command_interval, _CMD_INTERVAL_ENV_VAR,
-                           _DEFAULT_CMD_INTERVAL);
-    _init_integer_from_env(_thread_count, _TP_THREAD_COUNT,
-                           _DEFAULT_THREAD_COUNT);
+    get_config_integer(_connection_timeout, _CONN_TIMEOUT_ENV_VAR,
+                         _DEFAULT_CONN_TIMEOUT);
+    get_config_integer(_connection_interval, _CONN_INTERVAL_ENV_VAR,
+                         _DEFAULT_CONN_INTERVAL);
+    get_config_integer(_command_timeout, _CMD_TIMEOUT_ENV_VAR,
+                         _DEFAULT_CMD_TIMEOUT);
+    get_config_integer(_command_interval, _CMD_INTERVAL_ENV_VAR,
+                         _DEFAULT_CMD_INTERVAL);
+    get_config_integer(_thread_count, _TP_THREAD_COUNT,
+                         _DEFAULT_THREAD_COUNT);
 
     _check_runtime_variables();
 
     _connection_attempts = (_connection_timeout * 1000) /
                             _connection_interval + 1;
 
     _command_attempts = (_command_timeout * 1000) /
                          _command_interval + 1;
 
-    _tp = new ThreadPool(_thread_count);
+    _tp = new ThreadPool(_context, _thread_count);
 }
 
 // RedisServer destructor
 RedisServer::~RedisServer()
 {
     // Terminate the thread pool
     _tp->shutdown();
     delete _tp;
 }
 
 
 // Retrieve a single address, randomly chosen from a list of addresses if
 // applicable, from the SSDB environment variable
-std::string RedisServer::_get_ssdb()
+SRAddress RedisServer::_get_ssdb()
 {
     // Retrieve the environment variable
-    char* env_char = getenv("SSDB");
-    if (env_char == NULL)
+    std::string db_spec;
+    get_config_string(db_spec, "SSDB", "");
+    if (db_spec.length() == 0)
         throw SRRuntimeException("The environment variable SSDB "\
                                  "must be set to use the client.");
-    std::string env_str = std::string(env_char);
-    _check_ssdb_string(env_str);
+    _check_ssdb_string(db_spec);
 
     // Parse the data in it
-    std::vector<std::string> hosts_ports;
+    std::vector<SRAddress> address_choices;
     const char delim = ',';
 
     size_t i_pos = 0;
-    size_t j_pos = env_str.find(delim);
+    size_t j_pos = db_spec.find(delim);
     while (j_pos != std::string::npos) {
-        hosts_ports.push_back("tcp://"+
-        env_str.substr(i_pos, j_pos - i_pos));
+        std::string substr = db_spec.substr(i_pos, j_pos - i_pos);
+        SRAddress addr_spec(substr);
+        address_choices.push_back(addr_spec);
         i_pos = j_pos + 1;
-        j_pos = env_str.find(delim, i_pos);
+        j_pos = db_spec.find(delim, i_pos);
+    }
+    // Catch the last value that does not have a trailing ','
+    if (i_pos < db_spec.size()) {
+        std::string substr = db_spec.substr(i_pos, j_pos - i_pos);
+        SRAddress addr_spec(substr);
+        address_choices.push_back(addr_spec);
     }
-    // Catch the last value that does not have a trailing ';'
-    if (i_pos < env_str.size())
-        hosts_ports.push_back("tcp://"+
-        env_str.substr(i_pos, j_pos - i_pos));
 
     // Pick an entry from the list at random
-    std::uniform_int_distribution<> distrib(0, hosts_ports.size() - 1);
-    return hosts_ports[distrib(_gen)];
+    std::uniform_int_distribution<> distrib(0, address_choices.size() - 1);
+    return address_choices[distrib(_gen)];
 }
 
 // Check that the SSDB environment variable value does not have any errors
 void RedisServer::_check_ssdb_string(const std::string& env_str) {
     for (size_t i = 0; i < env_str.size(); i++) {
         char c = env_str[i];
-        if (!isalnum(c) && c != '.' && c != ':' && c != ',') {
+        if (!isalnum(c) && c != '.' && c != ':' && c != ',' && c != '/') {
             throw SRRuntimeException("The provided SSDB value, " + env_str +
                                      " is invalid because of character " + c);
         }
     }
 }
 
-//Initialize variable of type integer from environment variable
-void RedisServer::_init_integer_from_env(int& value,
-                                         const std::string& env_var,
-                                         const int& default_value)
-{
-    value = default_value;
-
-    char* env_char = getenv(env_var.c_str());
-
-    if (env_char != NULL && strlen(env_char) > 0) {
-        // Enforce that all characters are digits because std::stoi
-        // will truncate a string like "10xy" to 10.
-        // We want to guard users from input errors they might have.
-        char* c = env_char;
-        while (*c != '\0') {
-            if (!isdigit(*c) && !(*c == '-' && c == env_char)) {
-                throw SRParameterException("The value of " + env_var +
-                                           " must be a valid number.");
-            }
-            c++;
-        }
-
-        try {
-            value = std::stoi(env_char);
-        }
-        catch (std::invalid_argument& e) {
-            throw SRParameterException("The value of " + env_var + " could "\
-                                       "not be converted to type integer.");
-        }
-        catch (std::out_of_range& e) {
-            throw SRParameterException("The value of " + env_var + " is too "\
-                                       "large to be stored as an integer "\
-                                       "value.");
-        }
-        catch (std::exception& e) {
-            throw SRInternalException("An unexpected error occurred  "\
-                                      "while attempting to convert the "\
-                                      "environment variable " + env_var +
-                                      " to an integer.");
-        }
-    }
-}
-
 // Check that runtime variables are within valid ranges
 inline void RedisServer::_check_runtime_variables()
 {
     if (_connection_timeout <= 0) {
         throw SRParameterException(_CONN_TIMEOUT_ENV_VAR +
                                    " must be greater than 0.");
     }
 
     if (_connection_interval <= 0) {
         throw SRParameterException(_CONN_INTERVAL_ENV_VAR +
                                    " must be greater than 0.");
     }
 
     if (_command_timeout <= 0) {
-        throw SRParameterException(_CMD_TIMEOUT_ENV_VAR +
+        throw SRParameterException(_CMD_TIMEOUT_ENV_VAR + " " +
+                                   std::to_string(_command_timeout) +
                                    " must be greater than 0.");
     }
 
     if (_command_interval <= 0) {
         throw SRParameterException(_CMD_INTERVAL_ENV_VAR +
                                    " must be greater than 0.");
     }
@@ -181,12 +144,52 @@
     if (_connection_timeout > (INT_MAX / 1000)) {
         throw SRParameterException(_CONN_TIMEOUT_ENV_VAR +
                                    " must be less than "
                                    + std::to_string(INT_MAX / 1000));
     }
 
     if (_command_timeout > (INT_MAX / 1000)) {
-        throw SRParameterException(_CMD_TIMEOUT_ENV_VAR +
+        throw SRParameterException(_CMD_TIMEOUT_ENV_VAR + " " +
+                                   std::to_string(_command_timeout) +
                                    " must be less than "
                                    + std::to_string(INT_MAX / 1000));
     }
-}
+}
+
+// Create a string representation of the Redis connection
+std::string RedisServer::to_string() const
+{
+    std::string result;
+
+    // Shards
+    result += "  Redis shards at:\n";
+    auto it = _address_node_map.begin();
+    for ( ; it != _address_node_map.end(); it++) {
+        result += "    " + it->first + "\n";
+    }
+
+    // Protocol
+    result += "  Protocol: ";
+    result += _is_domain_socket ? "Unix Domain Socket" : "TCP";
+    result += "\n";
+
+    // Parameters
+    result += "  Command parameters:\n";
+    result += "    Retry attempts: "
+           + std::to_string(_command_attempts) + "\n";
+    result += "    Retry interval (ms): "
+           + std::to_string(_command_interval) + "\n";
+    result += "    Attempt timeout (ms): "
+           + std::to_string(_command_timeout) + "\n";
+    result += "  Connection parameters:\n";
+    result += "    Retry attempts: "
+           + std::to_string(_connection_attempts) + "\n";
+    result += "    Retry interval (ms): "
+           + std::to_string(_connection_interval) + "\n";
+    result += "    Attempt timeout (ms): "
+           + std::to_string(_connection_timeout) + "\n";
+
+    // Threadpool
+    result += "  Threadpool: " + std::to_string(_thread_count) + " threads\n";
+
+    return result;
+}
```

### Comparing `smartredis-0.3.1/src/cpp/singlekeycommand.cpp` & `smartredis-0.4.0/src/cpp/singlekeycommand.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/cpp/stringfield.cpp` & `smartredis-0.4.0/src/cpp/stringfield.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -62,15 +62,15 @@
 // Add a string to the field
 void StringField::append(const std::string& value)
 {
     _vals.push_back(value);
 }
 
 // Retrieve the number of values in the field
-size_t StringField::size()
+size_t StringField::size() const
 {
     return _vals.size();
 }
 
 // Clear the values in the field
 void StringField::clear()
 {
```

### Comparing `smartredis-0.3.1/src/cpp/tensorbase.cpp` & `smartredis-0.4.0/src/cpp/tensorbase.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -135,39 +135,39 @@
     tb._data = NULL;
 
     // Done
     return *this;
 }
 
 // Retrieve the tensor name.
-std::string TensorBase::name()
+std::string TensorBase::name() const
 {
     return _name;
 }
 
 // Retrieve the tensor type.
-SRTensorType TensorBase::type()
+SRTensorType TensorBase::type() const
 {
    return _type;
 }
 
 // Retrieve the string version of the tensor type.
 std::string TensorBase::type_str()
 {
     return TENSOR_STR_MAP.at(type());
 }
 
 // Retrieve the tensor dims.
-std::vector<size_t> TensorBase::dims()
+std::vector<size_t> TensorBase::dims() const
 {
    return _dims;
 }
 
 // Retrieve the total number of values in the tensor.
-size_t TensorBase::num_values()
+size_t TensorBase::num_values() const
 {
     if (_dims.size() == 0)
         throw SRRuntimeException("Invalid dimensionality for tensor detected");
     size_t n_values = 1;
     for (size_t i = 0; i < _dims.size(); i++)
         n_values *= _dims[i];
```

### Comparing `smartredis-0.3.1/src/cpp/tensorpack.cpp` & `smartredis-0.4.0/src/cpp/tensorpack.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * BSD 2-Clause License
  *
- * Copyright (c) 2021-2022, Hewlett Packard Enterprise
+ * Copyright (c) 2021-2023, Hewlett Packard Enterprise
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *
  * 1. Redistributions of source code must retain the above copyright notice, this
  *    list of conditions and the following disclaimer.
@@ -125,30 +125,30 @@
         throw SRRuntimeException("The tensor name must be nonempty.");
 
     _tensorbase_inventory[name] = tensor;
     _all_tensors.push_front(tensor);
 }
 
 // Return a TensorBase pointer based on name.
-TensorBase* TensorPack::get_tensor(const std::string& name)
+TensorBase* TensorPack::get_tensor(const std::string& name) const
 {
     return _tensorbase_inventory.at(name);
 }
 
 // Retrieve a pointer to the tensor data memory space
 void* TensorPack::get_tensor_data(const std::string& name)
 {
     TensorBase* ptr = _tensorbase_inventory.at(name);
     if (ptr == NULL)
         throw SRRuntimeException("Tensor not found: " + name);
     return ptr->data();
 }
 
 // Check whether a tensor with a given name exists in the TensorPack
-bool TensorPack::tensor_exists(const std::string& name)
+bool TensorPack::tensor_exists(const std::string& name) const
 {
     return (_tensorbase_inventory.count(name) > 0);
 }
 
 // Retrieve an iterator pointing to the first Tensor
 TensorPack::tensorbase_iterator TensorPack::tensor_begin()
 {
```

### Comparing `smartredis-0.3.1/src/cpp/threadpool.cpp` & `smartredis-0.4.0/src/cpp/threadpool.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -3,45 +3,41 @@
 #include <thread>
 #include <mutex>
 #include <condition_variable>
 #include <chrono>
 
 #include "threadpool.h"
 #include "srexception.h"
+#include "logger.h"
+#include "srobject.h"
 
 using namespace SmartRedis;
 using namespace std::chrono_literals;
 
-// TIME_THREADPOOL
-// Enable this flag to display timings for the threadpool activity.
-// Currently, this will be to screen, but eventually it will go to
-// the SmartRedis log
-#undef TIME_THREADPOOL
-
 // Constructor
-ThreadPool::ThreadPool(unsigned int num_threads)
+ThreadPool::ThreadPool(const SRObject* context, unsigned int num_threads)
+    : _context(context)
 {
-    // Flag that we're initializing
+    // Flags that we're initializing and not shutting down
     initialization_complete = false;
+    shutting_down = false;
 
     // By default, we'll make one thread for each hardware context
     if (num_threads == 0)
         num_threads = std::thread::hardware_concurrency();
 
     // Create worker threads
 	if (num_threads < 1) num_threads = 1; // Force a minimum of 1 thread
     for (unsigned int i = 0; i < num_threads; i++) {
-        #ifdef TIME_THREADPOOL
-        std::cout << "Kicking off thread " + std::to_string(i) << std::endl;
-        #endif
+        _context->log_data(
+            LLDeveloper, "Kicking off thread " + std::to_string(i));
         threads.push_back(std::thread(&ThreadPool::perform_jobs, this, i));
     }
 
     // Announce that we're open for business
-    shutting_down = false;
     shutdown_complete = false;
     initialization_complete = true;
 }
 
 // Desstructor
 ThreadPool::~ThreadPool()
 {
@@ -54,57 +50,49 @@
 // Shut down the thread pool, blocking any further jobs from submission
 void ThreadPool::shutdown()
 {
     // Make sure initialization is complete before we shut down
     while (!initialization_complete)
         ; // Spin
 
-    #ifdef TIME_THREADPOOL
-    std::cout << "Shutting down thread pool" << std::endl;
-    #endif
+    _context->log_data(LLDeveloper, "Shutting down thread pool");
 
     // We're closed for business
     shutting_down = true;
 
     // Wait for worker threads to finish up
-    #ifdef TIME_THREADPOOL
     int i = 0;
     size_t num_threads = threads.size();
-    #endif
     for (std::thread& thr : threads) {
         cv.notify_all(); // Wake up all the threads
-        #ifdef TIME_THREADPOOL
-        std::cout << "Waiting for a thread to terminate (" << std::to_string(i++) << " of "
-                  << std::to_string(num_threads) << ")" << std::endl;
-        #endif
+        std::string message =
+            "Waiting for thread to terminate (" +
+            std::to_string(i++) + " of " +
+            std::to_string(num_threads) + ")";
+        _context->log_data(LLDeveloper, message);
         thr.join(); // Blocks until the thread finishes execution
     }
 
     // Done
-    #ifdef TIME_THREADPOOL
-    std::cout << "Shutdown complete" << std::endl;
-    #endif
+    _context->log_data(LLDeveloper, "Shutdown complete");
     shutdown_complete = true;
 }
 
 // Worker thread main loop to acquire and perform jobs
 void ThreadPool::perform_jobs(unsigned int tid)
 {
-    #ifdef TIME_THREADPOOL
     int jobid = 0;
-    std::cout << "Thread " << std::to_string(tid) << " reporting for duty" << std::endl;
-    #endif
+    _context->log_data(
+        LLDebug, "Thread " + std::to_string(tid) + " reporting for duty");
 
     // Loop forever processing jobs until we get killed
     std::function<void()> job;
     while (!shutting_down)
     {
-        #ifdef TIME_THREADPOOL
         auto start = std::chrono::steady_clock::now();
-        #endif
 
         // Get a job, blocking until one appears if none immediately available
         do {
             std::unique_lock<std::mutex> lock(queue_mutex);
             cv.wait_for(lock, 250ms, [this](){
                 return !jobs.empty() || shutting_down;
             });
@@ -118,33 +106,34 @@
                 job = jobs.front();
                 jobs.pop();
                 break;
             }
         } // End scope and release lock
         while (!shutting_down);
 
-        #ifdef TIME_THREADPOOL
         auto have_job = std::chrono::steady_clock::now();
-        #endif
+
         // Perform the job
         if (!shutting_down) {
             job();
-            #ifdef TIME_THREADPOOL
             auto job_done = std::chrono::steady_clock::now();
             std::chrono::duration<double> get_job = have_job - start;
             std::chrono::duration<double> execute_job = job_done - have_job;
-            std::cout << "Thread " << std::to_string(tid) << " "
-                      << "time to get job " << std::to_string(jobid++) << ": " << get_job.count() << " s; "
-                      << "time to execute job: " << execute_job.count() << " s" << std::endl;
-            #endif
+            std::string message =
+                "Thread " + std::to_string(tid) +
+                " time to get job " + std::to_string(jobid++) +
+                ": " + std::to_string(get_job.count()) + " s; " +
+                "time to execute job: " +
+                std::to_string(execute_job.count()) + " s";
+            _context->log_data(LLDeveloper, message);
         }
     }
-    #ifdef TIME_THREADPOOL
-    std::cout << "Thread " << std::to_string(tid) << " shutting down" << std::endl;
-    #endif
+
+    _context->log_data(
+        LLDeveloper, "Thread " + std::to_string(tid) + " shutting down");
 }
 
 // Submit a job to threadpool for execution
 void ThreadPool::submit_job(std::function<void()> job)
 {
     // If the threadpool is shutting down, reject the job
     if (shutting_down) {
```

### Comparing `smartredis-0.3.1/src/fortran/client/aggregation_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/aggregation_interfaces.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -158,15 +158,15 @@
 end interface
 
 interface
   function get_dataset_list_range_allocated_c(client, list_name, list_name_length, start_index, end_index, &
     datasets) bind(c, name="_get_dataset_list_range_allocated")
     use iso_c_binding, only : c_ptr, c_char, c_bool, c_size_t, c_int
     import :: enum_kind
-    integer(kind=enum_kind)       :: get_dataset_list_range_c
+    integer(kind=enum_kind)       :: get_dataset_list_range_allocated_c
     type(c_ptr), value            :: client
     character(kind=c_char)        :: list_name(*)
     integer(kind=c_size_t), value :: list_name_length
     integer(kind=c_int),    value :: start_index
     integer(kind=c_int),    value :: end_index
     type(c_ptr), value            :: datasets
   end function get_dataset_list_range_allocated_c
```

### Comparing `smartredis-0.3.1/src/fortran/client/client_dataset_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/client_dataset_interfaces.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/client_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/client_interfaces.inc`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -21,20 +21,23 @@
 ! DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 ! SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 interface
-  function c_constructor(cluster, new_client) bind(c, name="SmartRedisCClient")
-    use iso_c_binding, only : c_ptr, c_bool
+  function c_constructor(cluster, logger_name, logger_name_length, new_client) bind(c, name="SmartRedisCClient")
+    use iso_c_binding, only : c_ptr, c_bool, c_char, c_size_t
     import :: enum_kind
-    integer(kind=enum_kind)     :: c_constructor
-    logical(kind=c_bool), value :: cluster !< True if a database cluster is being used
-    type(c_ptr)                 :: new_client !< Receives the newly constructed client
+    integer(kind=enum_kind)       :: c_constructor
+    logical(kind=c_bool), value   :: cluster !< True if a database cluster is being used
+    character(kind=c_char)        :: logger_name(*)
+    integer(kind=c_size_t), value :: logger_name_length
+
+    type(c_ptr)                   :: new_client !< Receives the newly constructed client
   end function c_constructor
 end interface
 
 interface
   function c_destructor(client) bind(c, name="DeleteCClient")
     use iso_c_binding, only : c_ptr
     import :: enum_kind
@@ -145,7 +148,15 @@
     character(kind=c_char)        :: key(*)
     integer(kind=c_size_t), value :: key_length
     integer(kind=c_int),    value :: poll_frequency_ms
     integer(kind=c_int),    value :: num_tries
     logical(kind=c_bool)          :: exists
   end function poll_key_c
 end interface
+
+interface
+  function client_to_string_c(client) bind(c, name="client_to_string")
+    use iso_c_binding, only : c_ptr, c_char
+    type(c_ptr)                   :: client_to_string_c
+    type(c_ptr), value            :: client
+  end function client_to_string_c
+end interface
```

### Comparing `smartredis-0.3.1/src/fortran/client/ensemble_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/ensemble_interfaces.inc`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -21,36 +21,50 @@
 ! DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 ! SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 interface
-  function set_data_source_c( client, source_id, source_id_length ) bind(c, name="set_data_source")
+  function set_data_source_c( client, source_id, source_id_length ) &
+    bind(c, name="set_data_source")
     use iso_c_binding, only : c_ptr, c_char, c_bool, c_size_t
     import :: enum_kind
     integer(kind=enum_kind)       :: set_data_source_c
     type(c_ptr),            value :: client
     character(kind=c_char)        :: source_id(*)
     integer(kind=c_size_t), value :: source_id_length
   end function set_data_source_c
 end interface
 
 interface
-  function use_model_ensemble_prefix_c( client, use_prefix) bind(c, name="use_model_ensemble_prefix")
+  function use_model_ensemble_prefix_c( client, use_prefix) &
+    bind(c, name="use_model_ensemble_prefix")
     use iso_c_binding, only : c_ptr, c_bool
     import :: enum_kind
     integer(kind=enum_kind)       :: use_model_ensemble_prefix_c
     type(c_ptr),            value :: client
     logical(kind=c_bool),   value :: use_prefix
   end function use_model_ensemble_prefix_c
 end interface
 
 interface
-  function use_tensor_ensemble_prefix_c( client, use_prefix) bind(c, name="use_tensor_ensemble_prefix")
+  function use_tensor_ensemble_prefix_c( client, use_prefix) &
+    bind(c, name="use_tensor_ensemble_prefix")
     use iso_c_binding, only : c_ptr, c_bool
     import :: enum_kind
     integer(kind=enum_kind)       :: use_tensor_ensemble_prefix_c
     type(c_ptr),            value :: client
     logical(kind=c_bool),   value :: use_prefix
   end function use_tensor_ensemble_prefix_c
+end interface
+
+interface
+  function use_dataset_ensemble_prefix_c( client, use_prefix) &
+    bind(c, name="use_dataset_ensemble_prefix")
+    use iso_c_binding, only : c_ptr, c_bool
+    import :: enum_kind
+    integer(kind=enum_kind)       :: use_dataset_ensemble_prefix_c
+    type(c_ptr),            value :: client
+    logical(kind=c_bool),   value :: use_prefix
+  end function use_dataset_ensemble_prefix_c
 end interface
```

### Comparing `smartredis-0.3.1/src/fortran/client/misc_tensor_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/misc_tensor_interfaces.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/model_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/model_interfaces.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/put_tensor_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/put_tensor_interfaces.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/put_tensor_methods_common.inc` & `smartredis-0.4.0/src/fortran/client/put_tensor_methods_common.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/script_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/script_interfaces.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/unpack_tensor_interfaces.inc` & `smartredis-0.4.0/src/fortran/client/unpack_tensor_interfaces.inc`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/client/unpack_tensor_methods_common.inc` & `smartredis-0.4.0/src/fortran/client/unpack_tensor_methods_common.inc`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -23,15 +23,14 @@
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
   !** Beginning of code common to all unpack_tensor subroutines
 
   ! Local variables
-  integer(kind=c_size_t) :: ndim ! Number of dimensions
   type(c_ptr) :: data_ptr, c_dims_ptr
   character(kind=c_char, len=len_trim(name)) :: c_name !< Transformed fortran 'name' to a c-string
   integer(kind=c_size_t) :: name_length, c_n_dims
   integer(kind=c_size_t), target :: c_dims(size(dims))
   integer(kind=enum_kind) :: data_type, mem_layout
 
   c_name = trim(name)
```

### Comparing `smartredis-0.3.1/src/fortran/client.F90` & `smartredis-0.4.0/src/fortran/client.F90`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -29,34 +29,37 @@
 use iso_c_binding, only : c_ptr, c_bool, c_null_ptr, c_char, c_int
 use iso_c_binding, only : c_int8_t, c_int16_t, c_int32_t, c_int64_t, c_float, c_double, c_size_t
 use iso_c_binding, only : c_loc, c_f_pointer
 
 use, intrinsic :: iso_fortran_env, only: stderr => error_unit
 
 use smartredis_dataset, only : dataset_type
-use fortran_c_interop, only : convert_char_array_to_c, enum_kind
+use fortran_c_interop, only : convert_char_array_to_c, enum_kind, C_MAX_STRING
+
 
 implicit none; private
 
 #include "enum_fortran.inc"
 #include "client/client_interfaces.inc"
 #include "client/put_tensor_interfaces.inc"
 #include "client/unpack_tensor_interfaces.inc"
 #include "client/misc_tensor_interfaces.inc"
 #include "client/model_interfaces.inc"
 #include "client/script_interfaces.inc"
 #include "client/client_dataset_interfaces.inc"
 #include "client/ensemble_interfaces.inc"
 #include "client/aggregation_interfaces.inc"
+#include "errors/errors_interfaces.inc"
 
 public :: enum_kind !< The kind of integer equivalent to a C enum. According to C an Fortran
                     !! standards this should be c_int, but is renamed here to ensure that
                     !! users do not have to import the iso_c_binding module into their
                     !! programs
 
+
 !> Stores all data and methods associated with the SmartRedis client that is used to communicate with the database
 type, public :: client_type
   private
 
   logical(kind=c_bool) :: cluster = .false.        !< True if a database cluster is being used
   type(c_ptr)          :: client_ptr = c_null_ptr !< Pointer to the initialized SmartRedisClient
   logical              :: is_initialized = .false.    !< True if client is initialized
@@ -74,14 +77,16 @@
   procedure :: SR_error_parser
   !> Initializes a new instance of the SmartRedis client
   procedure :: initialize => initialize_client
   !> Check if a SmartRedis client has been initialized
   procedure :: isinitialized
   !> Destructs a new instance of the SmartRedis client
   procedure :: destructor
+  !> Access the raw C pointer for the client
+  procedure :: get_c_pointer
   !> Check the database for the existence of a specific model
   procedure :: model_exists
   !> Check the database for the existence of a specific tensor
   procedure :: tensor_exists
   !> Check the database for the existence of a specific key
   procedure :: key_exists
   !> Check the database for the existence of a specific dataset
@@ -145,14 +150,16 @@
   !> Copy a dataset stored in the database into another name
   procedure :: copy_dataset
   !> Delete the dataset from the database
   procedure :: delete_dataset
 
   !> If true, preprend the ensemble id for tensor-related keys
   procedure :: use_tensor_ensemble_prefix
+  !> If true, preprend the ensemble id for dataset-related keys
+  procedure :: use_dataset_ensemble_prefix
   !> If true, preprend the ensemble id for model-related keys
   procedure :: use_model_ensemble_prefix
   !> If true, preprend the ensemble id for dataset list-related keys
   procedure :: use_list_ensemble_prefix
   !> Specify a specific source of data (e.g. another ensemble member)
   procedure :: set_data_source
 
@@ -168,16 +175,22 @@
   procedure :: get_list_length
   !> Repeatedly check the length of the list until it is a given size
   procedure :: poll_list_length
   !> Repeatedly check the length of the list until it greater than or equal to the given size
   procedure :: poll_list_length_gte
   !> Repeatedly check the length of the list until it less than or equal to the given size
   procedure :: poll_list_length_lte
-  !> Retrieve vector of datasetes from the list
+  !> Retrieve vector of datasets from the list
   procedure :: get_datasets_from_list
+  !> Retrieve vector of datasets from the list over a given range
+  procedure :: get_datasets_from_list_range
+  !> Retrieve a string representation of the client
+  procedure :: to_string
+  !> Print a string representation of the client
+  procedure :: print_client
 
   ! Private procedures
   procedure, private :: put_tensor_i8
   procedure, private :: put_tensor_i16
   procedure, private :: put_tensor_i32
   procedure, private :: put_tensor_i64
   procedure, private :: put_tensor_float
@@ -196,47 +209,64 @@
 !> Decode a response code from an API function
 function SR_error_parser(self, response_code) result(is_error)
   class(client_type),       intent(in) :: self    !< Receives the initialized client
   integer (kind=enum_kind), intent(in) :: response_code !< The response code to decode
   logical                              :: is_error      !< Indicates whether this is an error response
 
   is_error = .true.
-  select case (response_code)
-    case(SRNoError)
-      is_error = .false.
-    case(SRBadAllocError)
-      write(stderr,*) "Memory allocation error"
-    case(SRDatabaseError)
-      write(stderr,*) "Backend database error"
-    case(SRInternalError)
-      write(stderr,*) "Internal SmartRedis error"
-    case(SRRuntimeError)
-      write(stderr,*) "Runtime error executing an operation"
-    case(SRParameterError)
-      write(stderr,*) "Bad parameter error"
-    case(SRTimeoutError)
-      write(stderr,*) "Timeout error"
-    case(SRKeyError)
-      write(stderr,*) "Key error"
-    case(SRTypeError)
-      write(stderr,*) "Type mismatch error"
-    case default
-       write(stderr,*) "Invalid or uninitialized response code"
-  end select
+  if (self%isinitialized()) then
+    select case (response_code)
+      case(SRNoError)
+        is_error = .false.
+      case(SRBadAllocError)
+        write(stderr,*) "Memory allocation error"
+      case(SRDatabaseError)
+        write(stderr,*) "Backend database error"
+      case(SRInternalError)
+        write(stderr,*) "Internal SmartRedis error"
+      case(SRRuntimeError)
+        write(stderr,*) "Runtime error executing an operation"
+      case(SRParameterError)
+        write(stderr,*) "Bad parameter error"
+      case(SRTimeoutError)
+        write(stderr,*) "Timeout error"
+      case(SRKeyError)
+        write(stderr,*) "Key error"
+      case(SRTypeError)
+        write(stderr,*) "Type mismatch error"
+      case default
+        write(stderr,*) "Invalid or uninitialized response code"
+    end select
+  else
+    write(stderr,*) "SmartRedis Client has not been initialized"
+  endif
 end function SR_error_parser
 
 !> Initializes a new instance of a SmartRedis client
-function initialize_client(self, cluster)
-  integer(kind=enum_kind)           :: initialize_client
-  class(client_type), intent(inout) :: self    !< Receives the initialized client
-  logical, optional,  intent(in   ) :: cluster !< If true, client uses a database cluster (Default: .false.)
+function initialize_client(self, cluster, logger_name)
+  integer(kind=enum_kind)                     :: initialize_client
+  class(client_type),         intent(inout)   :: self      !< Receives the initialized client
+  logical, optional,          intent(in   )   :: cluster   !< If true, client uses a database cluster (Default: .false.)
+  character(len=*), optional, intent(in   )   :: logger_name !< Identifier for the current client
+
+  ! Local variables
+  character(kind=c_char, len=:), allocatable :: c_logger_name
+  integer(kind=c_size_t) :: logger_name_length
+
+  if (present(logger_name)) then
+    c_logger_name = logger_name
+  else
+    c_logger_name = 'default'
+  endif
+  logger_name_length = len_trim(c_logger_name)
 
   if (present(cluster)) self%cluster = cluster
-  initialize_client = c_constructor(self%cluster, self%client_ptr)
+  initialize_client = c_constructor(self%cluster, c_logger_name, logger_name_length, self%client_ptr)
   self%is_initialized = initialize_client .eq. SRNoError
+  if (allocated(c_logger_name)) deallocate(c_logger_name)
 end function initialize_client
 
 !> Check whether the client has been initialized
 logical function isinitialized(this)
   class(client_type) :: this
   isinitialized = this%is_initialized
 end function isinitialized
@@ -246,14 +276,21 @@
   integer(kind=enum_kind)           :: destructor
   class(client_type), intent(inout) :: self
 
   destructor = c_destructor(self%client_ptr)
   self%client_ptr = C_NULL_PTR
 end function destructor
 
+!> Access the raw C pointer for the client
+function get_c_pointer(self)
+  type(c_ptr)                    :: get_c_pointer
+  class(client_type), intent(in) :: self
+  get_c_pointer = self%client_ptr
+end function get_c_pointer
+
 !> Check if the specified key exists in the database
 function key_exists(self, key, exists)
   class(client_type),   intent(in)  :: self   !< The client
   character(len=*),     intent(in)  :: key    !< The key to check
   logical(kind=c_bool), intent(out) :: exists !< Receives whether the key exists
   integer(kind=enum_kind)           :: key_exists
 
@@ -665,15 +702,15 @@
   integer(kind=enum_kind)                        :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   integer(kind=c_size_t) :: name_length, model_length
   character(kind=c_char), dimension(:), pointer :: f_str_ptr
   type(c_ptr) :: c_str_ptr
-  integer :: i
+  integer(kind=c_size_t) :: i
 
   c_name = trim(name)
   name_length = len_trim(name)
 
   code = get_model_c(self%client_ptr, name, name_length, c_str_ptr, model_length, c_str_ptr)
 
   call c_f_pointer(c_str_ptr, f_str_ptr, [ model_length ])
@@ -703,27 +740,24 @@
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(model_file)) :: c_model_file
   character(kind=c_char, len=len_trim(backend)) :: c_backend
   character(kind=c_char, len=len_trim(device)) :: c_device
   character(kind=c_char, len=:), allocatable :: c_tag
 
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
   character(kind=c_char,len=1), target, dimension(1) :: dummy_inputs, dummy_outputs
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: name_length, model_file_length, backend_length, device_length, tag_length, n_inputs, &
                             n_outputs
   integer(kind=c_int)    :: c_batch_size, c_min_batch_size
   type(c_ptr)            :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   ! Set default values for the optional inputs
   c_batch_size = 0
   if (present(batch_size)) c_batch_size = batch_size
   c_min_batch_size = 0
   if (present(min_batch_size)) c_min_batch_size = min_batch_size
   if (present(tag)) then
     allocate(character(kind=c_char, len=len_trim(tag)) :: c_tag)
@@ -744,29 +778,32 @@
   name_length = len_trim(name)
   model_file_length = len_trim(model_file)
   backend_length = len_trim(backend)
   device_length = len_trim(device)
 
   dummy_inputs = ''
   if (present(inputs)) then
-    call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
-                                  n_inputs)
+    code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, &
+                                        input_lengths_ptr, n_inputs)
   else
-    call convert_char_array_to_c(dummy_inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr,&
-                                  n_inputs)
+    code = convert_char_array_to_c(dummy_inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, &
+                                 input_lengths_ptr, n_inputs)
   endif
 
+  if (code /= SRNoError) return
+
   dummy_outputs =''
   if (present(outputs)) then
-    call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, output_lengths_ptr,&
-                                  n_outputs)
+    code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+                                   output_lengths_ptr, n_outputs)
   else
-    call convert_char_array_to_c(dummy_outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
-                                  output_lengths_ptr, n_outputs)
+    code = convert_char_array_to_c(dummy_outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+                                   output_lengths_ptr, n_outputs)
   endif
+  if (code /= SRNoError) return
 
   code = set_model_from_file_c(self%client_ptr, c_name, name_length, c_model_file, model_file_length, &
                              c_backend, backend_length, c_device, device_length, c_batch_size, c_min_batch_size, &
                              c_tag, tag_length, inputs_ptr, input_lengths_ptr, n_inputs, outputs_ptr, &
                              output_lengths_ptr, n_outputs)
   if (allocated(c_inputs))        deallocate(c_inputs)
   if (allocated(input_lengths))   deallocate(input_lengths)
@@ -796,27 +833,24 @@
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(model_file)) :: c_model_file
   character(kind=c_char, len=len_trim(backend)) :: c_backend
   character(kind=c_char, len=:), allocatable :: c_tag
 
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
   character(kind=c_char,len=1), target, dimension(1) :: dummy_inputs, dummy_outputs
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: name_length, model_file_length, backend_length, tag_length, n_inputs, &
                             n_outputs
   integer(kind=c_int)    :: c_batch_size, c_min_batch_size, c_first_gpu, c_num_gpus
   type(c_ptr)            :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   ! Set default values for the optional inputs
   c_batch_size = 0
   if (present(batch_size)) c_batch_size = batch_size
   c_min_batch_size = 0
   if (present(min_batch_size)) c_min_batch_size = min_batch_size
   if (present(tag)) then
     allocate(character(kind=c_char, len=len_trim(tag)) :: c_tag)
@@ -839,29 +873,31 @@
 
   ! Convert to C int
   c_first_gpu = first_gpu
   c_num_gpus  = num_gpus
 
   dummy_inputs = ''
   if (present(inputs)) then
-    call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+    code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
                                   n_inputs)
   else
-    call convert_char_array_to_c(dummy_inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr,&
-                                  n_inputs)
+    code = convert_char_array_to_c(dummy_inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, &
+                                   input_lengths_ptr, n_inputs)
   endif
+  if (code /= SRNoError) return
 
   dummy_outputs =''
   if (present(outputs)) then
-    call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, output_lengths_ptr,&
-                                  n_outputs)
+    code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+                                   output_lengths_ptr, n_outputs)
   else
-    call convert_char_array_to_c(dummy_outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+    code = convert_char_array_to_c(dummy_outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
                                   output_lengths_ptr, n_outputs)
   endif
+  if (code /= SRNoError) return
 
   code = set_model_from_file_multigpu_c(self%client_ptr, c_name, name_length, c_model_file, model_file_length, &
                              c_backend, backend_length, c_first_gpu, c_num_gpus, c_batch_size, c_min_batch_size, &
                              c_tag, tag_length, inputs_ptr, input_lengths_ptr, n_inputs, outputs_ptr, &
                              output_lengths_ptr, n_outputs)
 
   if (allocated(c_inputs))        deallocate(c_inputs)
@@ -890,43 +926,42 @@
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(model)) :: c_model
   character(kind=c_char, len=len_trim(backend)) :: c_backend
   character(kind=c_char, len=len_trim(device)) :: c_device
   character(kind=c_char, len=len_trim(tag)) :: c_tag
 
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: name_length, model_length, backend_length, device_length, tag_length, n_inputs, &
                             n_outputs
   integer(kind=c_int)    :: c_batch_size, c_min_batch_size
   type(c_ptr)            :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   c_name = trim(name)
   c_model = trim(model)
   c_backend = trim(backend)
   c_device = trim(device)
   c_tag = trim(tag)
 
   name_length = len_trim(name)
   model_length = len_trim(model)
   backend_length = len_trim(backend)
   device_length = len_trim(device)
   tag_length = len_trim(tag)
 
   ! Copy the input array into a c_char
-  call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+  code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
                                 n_inputs)
-  call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+  if (code /= SRNoError) return
+  code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
                                 output_lengths_ptr, n_outputs)
+  if (code /= SRNoError) return
 
   ! Cast the batch sizes to C integers
   c_batch_size = batch_size
   c_min_batch_size = min_batch_size
 
   code = set_model_c(self%client_ptr, c_name, name_length, c_model, model_length, c_backend, backend_length, &
                  c_device, device_length, batch_size, min_batch_size, c_tag, tag_length, &
@@ -958,40 +993,39 @@
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(model)) :: c_model
   character(kind=c_char, len=len_trim(backend)) :: c_backend
   character(kind=c_char, len=len_trim(tag)) :: c_tag
 
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: name_length, model_length, backend_length, tag_length, n_inputs, n_outputs
   integer(kind=c_int)    :: c_batch_size, c_min_batch_size, c_first_gpu, c_num_gpus
   type(c_ptr)            :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   c_name = trim(name)
   c_model = trim(model)
   c_backend = trim(backend)
   c_tag = trim(tag)
 
   name_length = len_trim(name)
   model_length = len_trim(model)
   backend_length = len_trim(backend)
   tag_length = len_trim(tag)
 
   ! Copy the input array into a c_char
-  call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
-                                n_inputs)
-  call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
-                                output_lengths_ptr, n_outputs)
+  code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+                                 n_inputs)
+  if (code /= SRNoError) return
+  code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+                                 output_lengths_ptr, n_outputs)
+  if (code /= SRNoError) return
 
   ! Cast the batch sizes to C integers
   c_batch_size = batch_size
   c_min_batch_size = min_batch_size
   c_first_gpu = first_gpu
   c_num_gpus = num_gpus
 
@@ -1013,31 +1047,30 @@
   character(len=*),               intent(in) :: name    !< The name to use to place the model
   character(len=*), dimension(:), intent(in) :: inputs  !< One or more names of model input nodes (TF models)
   character(len=*), dimension(:), intent(in) :: outputs !< One or more names of model output nodes (TF models)
   integer(kind=enum_kind)                    :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: n_inputs, n_outputs, name_length
   type(c_ptr) :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   c_name = trim(name)
   name_length = len_trim(name)
 
-  call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+  code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
                                 n_inputs)
-  call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+  if (code /= SRNoError) return
+  code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
                                 output_lengths_ptr, n_outputs)
+  if (code /= SRNoError) return
 
   code = run_model_c(self%client_ptr, c_name, name_length, inputs_ptr, input_lengths_ptr, n_inputs, outputs_ptr, &
                           output_lengths_ptr, n_outputs)
 
   if (allocated(c_inputs))        deallocate(c_inputs)
   if (allocated(input_lengths))   deallocate(input_lengths)
   if (allocated(ptrs_to_inputs))  deallocate(ptrs_to_inputs)
@@ -1056,32 +1089,31 @@
                                                         !! or MPI rank
   integer,                        intent(in) :: first_gpu !< The first GPU (zero-based) to use with the model
   integer,                        intent(in) :: num_gpus  !< The number of GPUs to use with the model
   integer(kind=enum_kind)                    :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
 
   integer(kind=c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: n_inputs, n_outputs, name_length
   integer(kind=c_int) :: c_first_gpu, c_num_gpus, c_offset
   type(c_ptr) :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   c_name = trim(name)
   name_length = len_trim(name)
 
-  call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+  code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
                                 n_inputs)
-  call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+  if (code /= SRNoError) return
+  code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
                                 output_lengths_ptr, n_outputs)
+  if (code /= SRNoError) return
 
   ! Cast to c integer
   c_offset = offset
   c_first_gpu = first_gpu
   c_num_gpus = num_gpus
   code = run_model_multigpu_c(self%client_ptr, c_name, name_length, inputs_ptr, input_lengths_ptr, n_inputs, &
                               outputs_ptr, output_lengths_ptr, n_outputs, c_offset, c_first_gpu, c_num_gpus)
@@ -1139,15 +1171,15 @@
   integer(kind=enum_kind)          :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   integer(kind=c_size_t) :: name_length, script_length
   character(kind=c_char), dimension(:), pointer :: f_str_ptr
   type(c_ptr) :: c_str_ptr
-  integer :: i
+  integer(kind=c_size_t) :: i
 
   c_name = trim(name)
   name_length = len_trim(name)
 
   code = get_script_c(self%client_ptr, name, name_length, c_str_ptr, script_length)
 
   call c_f_pointer(c_str_ptr, f_str_ptr, [ script_length ])
@@ -1197,15 +1229,14 @@
 
   ! Local variables
   character(kind=c_char, len=len_trim(name))        :: c_name
   character(kind=c_char, len=len_trim(script_file)) :: c_script_file
 
   integer(kind=c_size_t) :: name_length
   integer(kind=c_size_t) :: script_file_length
-  integer(kind=c_size_t) :: device_length
   integer(kind=c_int)    :: c_first_gpu, c_num_gpus
 
   c_name = trim(name)
   c_script_file = trim(script_file)
 
   name_length = len_trim(name)
   script_file_length = len_trim(script_file)
@@ -1256,15 +1287,14 @@
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(script)) :: c_script
 
   integer(kind=c_size_t) :: name_length
   integer(kind=c_size_t) :: script_length
-  integer(kind=c_size_t) :: device_length
   integer(kind=c_int)    :: c_first_gpu, c_num_gpus
 
   c_name = trim(name)
   c_script = trim(script)
 
   name_length = len_trim(name)
   script_length = len_trim(script)
@@ -1282,34 +1312,33 @@
   character(len=*), dimension(:), intent(in) :: inputs         !< One or more names of script input nodes (TF scripts)
   character(len=*), dimension(:), intent(in) :: outputs        !< One or more names of script output nodes (TF scripts)
   integer(kind=enum_kind)                    :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(func)) :: c_func
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), allocatable, target :: c_inputs(:), c_outputs(:)
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: n_inputs, n_outputs, name_length, func_length
   type(c_ptr) :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   c_name  = trim(name)
   c_func = trim(func)
 
   name_length = len_trim(name)
   func_length = len_trim(func)
 
-  call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+  code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
                                 n_inputs)
-  call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+  if (code /= SRNoError) return
+  code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
                                 output_lengths_ptr, n_outputs)
+  if (code /= SRNoError) return
 
   code = run_script_c(self%client_ptr, c_name, name_length, c_func, func_length, inputs_ptr, input_lengths_ptr, &
                             n_inputs, outputs_ptr, output_lengths_ptr, n_outputs)
 
   if (allocated(c_inputs))        deallocate(c_inputs)
   if (allocated(input_lengths))   deallocate(input_lengths)
   if (allocated(ptrs_to_inputs))  deallocate(ptrs_to_inputs)
@@ -1330,34 +1359,37 @@
   integer,                        intent(in) :: num_gpus  !< The number of GPUs to use with the model
   integer(kind=enum_kind)                    :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(name)) :: c_name
   character(kind=c_char, len=len_trim(func)) :: c_func
   integer(kind=c_int) :: c_first_gpu, c_num_gpus, c_offset
-  character(kind=c_char, len=:), allocatable, target :: c_inputs(:), c_outputs(:)
+  character(kind=c_char, len=C_MAX_STRING), dimension(:), allocatable, target :: c_inputs
+  character(kind=c_char, len=C_MAX_STRING), dimension(:), allocatable, target :: c_outputs
 
   integer(c_size_t), dimension(:), allocatable, target :: input_lengths, output_lengths
   integer(kind=c_size_t) :: n_inputs, n_outputs, name_length, func_length
+  integer :: input_length, output_length
   type(c_ptr) :: inputs_ptr, input_lengths_ptr, outputs_ptr, output_lengths_ptr
   type(c_ptr), dimension(:), allocatable :: ptrs_to_inputs, ptrs_to_outputs
 
-  integer :: i
-  integer :: max_length, length
-
   c_name  = trim(name)
   c_func = trim(func)
 
   name_length = len_trim(name)
   func_length = len_trim(func)
+  input_length = len_trim(inputs(1))
+  output_length = len_trim(outputs(1))
 
-  call convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
+  code = convert_char_array_to_c(inputs, c_inputs, ptrs_to_inputs, inputs_ptr, input_lengths, input_lengths_ptr, &
                                 n_inputs)
-  call convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
+  if (code /= SRNoError) return
+  code = convert_char_array_to_c(outputs, c_outputs, ptrs_to_outputs, outputs_ptr, output_lengths, &
                                 output_lengths_ptr, n_outputs)
+  if (code /= SRNoError) return
 
   ! Cast to c integer
   c_offset = offset
   c_first_gpu = first_gpu
   c_num_gpus = num_gpus
   code = run_script_multigpu_c(self%client_ptr, c_name, name_length, c_func, func_length, inputs_ptr, input_lengths_ptr, &
                             n_inputs, outputs_ptr, output_lengths_ptr, n_outputs, c_offset, c_first_gpu, c_num_gpus)
@@ -1512,26 +1544,38 @@
   logical,              intent(in) :: use_prefix !< The prefix setting
   integer(kind=enum_kind)          :: code
 
   code = use_model_ensemble_prefix_c(self%client_ptr, logical(use_prefix,kind=c_bool))
 end function use_model_ensemble_prefix
 
 
-!> Set whether names of tensor and dataset entities should be prefixed (e.g. in an ensemble) to form database keys.
+!> Set whether names of tensor entities should be prefixed (e.g. in an ensemble) to form database keys.
 !! Prefixes will only be used if they were previously set through the environment variables SSKEYOUT and SSKEYIN.
 !! Keys of entities created before client function is called will not be affected. By default, the client prefixes
-!! tensor and dataset keys with the first prefix specified with the SSKEYIN and SSKEYOUT environment variables.
+!! tensor keys with the first prefix specified with the SSKEYIN and SSKEYOUT environment variables.
 function use_tensor_ensemble_prefix(self, use_prefix) result(code)
   class(client_type),   intent(in) :: self       !< An initialized SmartRedis client
   logical,              intent(in) :: use_prefix !< The prefix setting
   integer(kind=enum_kind)          :: code
 
   code = use_tensor_ensemble_prefix_c(self%client_ptr, logical(use_prefix,kind=c_bool))
 end function use_tensor_ensemble_prefix
 
+!> Set whether names of dataset entities should be prefixed (e.g. in an ensemble) to form database keys.
+!! Prefixes will only be used if they were previously set through the environment variables SSKEYOUT and SSKEYIN.
+!! Keys of entities created before client function is called will not be affected. By default, the client prefixes
+!! dataset keys with the first prefix specified with the SSKEYIN and SSKEYOUT environment variables.
+function use_dataset_ensemble_prefix(self, use_prefix) result(code)
+  class(client_type),   intent(in) :: self       !< An initialized SmartRedis client
+  logical,              intent(in) :: use_prefix !< The prefix setting
+  integer(kind=enum_kind)          :: code
+
+  code = use_dataset_ensemble_prefix_c(self%client_ptr, logical(use_prefix,kind=c_bool))
+end function use_dataset_ensemble_prefix
+
 !> Control whether aggregation lists are prefixed
 function use_list_ensemble_prefix(self, use_prefix) result(code)
   class(client_type),   intent(in) :: self       !< An initialized SmartRedis client
   logical,              intent(in) :: use_prefix !< The prefix setting
   integer(kind=enum_kind)          :: code
 
   code = use_list_ensemble_prefix_c(self%client_ptr, logical(use_prefix,kind=c_bool))
@@ -1713,15 +1757,15 @@
   type(dataset_type), dimension(:), allocatable, intent(  out) :: datasets !< The array of datasets included
   integer(kind=enum_kind)          :: code
                                                                            !! in the list
   integer,              intent(out) :: num_datasets !< The numbr of datasets returned
 
   character(kind=c_char, len=len_trim(list_name)) :: list_name_c
   integer(kind=c_size_t) :: list_name_length
-  integer(kind=c_int) :: c_poll_frequency, c_num_tries, c_list_length, c_num_datasets
+  integer(kind=c_int) :: c_num_datasets
 
   type(c_ptr), dimension(:), allocatable, target :: dataset_ptrs
   type(c_ptr) :: ptr_to_dataset_ptrs
   integer :: i
 
   code = self%get_list_length(list_name, num_datasets)
   allocate(dataset_ptrs(num_datasets))
@@ -1759,36 +1803,77 @@
                                                   !! the last element of the list.
 
   type(dataset_type), dimension(:), allocatable, intent(  out) :: datasets !< The array of datasets included
   integer(kind=enum_kind)          :: code
                                                                            !! in the list
   character(kind=c_char, len=len_trim(list_name)) :: list_name_c
   integer(kind=c_size_t) :: list_name_length
-  integer(kind=c_int) :: c_poll_frequency, c_num_tries, c_list_length, c_num_datasets
+  integer(kind=c_int) :: c_num_datasets
   integer(kind=c_int) :: c_start_index, c_end_index
   integer :: num_datasets, i
   type(c_ptr), dimension(:), allocatable, target :: dataset_ptrs
   type(c_ptr) :: ptr_to_dataset_ptrs
 
   code = self%get_list_length(list_name, num_datasets)
   if (code /= SRNoError) return
   allocate(dataset_ptrs(num_datasets))
   ptr_to_dataset_ptrs = c_loc(dataset_ptrs)
 
   list_name_c = trim(list_name)
   list_name_length = len_trim(list_name)
 
   c_num_datasets = num_datasets
+  c_start_index = start_index
+  c_end_index = end_index
 
   code = get_dataset_list_range_allocated_c(self%client_ptr, list_name_c, list_name_length, &
                                             c_start_index, c_end_index, ptr_to_dataset_ptrs)
 
   if (allocated(datasets)) deallocate(datasets)
   allocate(datasets(num_datasets))
   do i=1,num_datasets
     datasets(i)%dataset_ptr = dataset_ptrs(i)
   enddo
   deallocate(dataset_ptrs)
 end function get_datasets_from_list_range
 
+!> Retrieve a string representation of the client
+function to_string(self)
+  character(kind=c_char, len=:), allocatable :: to_string  !< Text version of client
+  class(client_type),   intent(in)           :: self       !< An initialized SmartRedis client
+
+  type(c_ptr)                                :: c_cli_str
+  integer(kind=c_size_t)                     :: c_cli_str_len
+
+  ! Get the string representation of the client from C
+  c_cli_str = client_to_string_c(self%client_ptr)
+  c_cli_str_len = c_strlen(c_cli_str)
+  to_string = make_str(c_cli_str, c_cli_str_len)
+end function to_string
+
+!> Convert a pointer view of a string to a Fortran string
+function make_str(strptr, str_len)
+  character(kind=c_char, len=:), allocatable :: make_str
+  type(c_ptr), intent(in), value             :: strptr
+  integer(kind=c_size_t)                     :: str_len
+
+  character(len=str_len, kind=c_char), pointer :: ptrview
+  call c_f_pointer(strptr, ptrview)
+  make_str = ptrview
+end function make_str
+
+!> Print a string representation of the client
+subroutine print_client(self, unit)
+  class(client_type), intent(in)  :: self !< An initialized SmartRedis client
+  integer, optional,  intent(in)  :: unit !< Unit to which to print the client
+
+  ! Determine which unit to write to
+  integer :: target_unit
+  target_unit = STDERR
+  if (present(unit)) target_unit = unit
+
+  ! Write the error to the target unit
+  write(target_unit,*) to_string(self)
+end subroutine print_client
+
 end module smartredis_client
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/add_meta_scalar_common.inc` & `smartredis-0.4.0/src/fortran/dataset/add_meta_scalar_common.inc`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -23,15 +23,14 @@
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
   !** Beginning of code common to all add_meta_scalar subroutines
 
   character(kind=c_char, len=len_trim(name))  :: c_name
-  integer(kind=enum_kind) :: c_data_type, expected_data_type
   integer(kind=c_size_t) :: name_length
   type(c_ptr) :: meta_ptr
 
   c_name = trim(name)
   name_length = len_trim(name)
   meta_ptr = c_loc(meta)
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/add_tensor_interfaces.inc` & `smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -21,23 +21,24 @@
 ! DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 ! SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 interface
-  function add_tensor_c(dataset, name, name_length, data, dims, n_dims, data_type, mem_layout) &
-      bind(c, name="add_tensor")
-    use iso_c_binding, only : c_ptr, c_char, c_size_t
+  function unpack_dataset_tensor_c(dataset, name, name_length, result, dims, &
+      n_dims, data_type, mem_layout) bind(c, name="unpack_dataset_tensor")
+    use iso_c_binding, only: c_ptr, c_char, c_size_t
     import :: enum_kind
-    integer(kind=enum_kind)                    :: add_tensor_c
-    type(c_ptr),             value, intent(in) :: dataset     !< Pointer to the initialized client
-    character(kind=c_char),         intent(in) :: name(*)     !< The name to use to place the tensor
-    integer(kind=c_size_t),  value, intent(in) :: name_length !< The length of the name c-string,
-                                                              !! excluding null terminating character
-    type(c_ptr),             value, intent(in) :: data        !< A c ptr to the beginning of the data
-    type(c_ptr),             value, intent(in) :: dims        !< Length along each dimension of the tensor
-    integer(kind=c_size_t),  value, intent(in) :: n_dims      !< The number of dimensions of the tensor
-    integer(kind=enum_kind), value, intent(in) :: data_type   !< The data type of the tensor
-    integer(kind=enum_kind), value, intent(in) :: mem_layout  !< The memory layout of the data
-  end function add_tensor_c
+    integer(kind=enum_kind)                                 :: unpack_dataset_tensor_c
+    type(c_ptr),                          value, intent(in) :: dataset     !< Pointer to the initialized client
+    character(kind=c_char),                      intent(in) :: name(*)     !< The name to use to place the tensor
+    integer(kind=c_size_t),               value, intent(in) :: name_length !< The length of the name c-string,
+                                                                          !! excluding null terminating character
+    type(c_ptr),                          value, intent(in) :: result     !< A c ptr to the beginning of the data
+    type(c_ptr),                          value, intent(in) :: dims       !< Length along each dimension of the
+                                                                          !! tensor
+    integer(kind=c_size_t),               value, intent(in) :: n_dims     !< The number of dimensions of the tensor
+    integer(kind=enum_kind),              value, intent(in) :: data_type  !< The data type of the tensor
+    integer(kind=enum_kind),              value, intent(in) :: mem_layout !< The memory layout of the data
+  end function unpack_dataset_tensor_c
 end interface
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/add_tensor_methods_common.inc` & `smartredis-0.4.0/src/fortran/dataset/add_tensor_methods_common.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/dataset_interfaces.inc` & `smartredis-0.4.0/src/fortran/dataset/dataset_interfaces.inc`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -30,7 +30,15 @@
     import :: enum_kind
     integer(kind=enum_kind)       :: dataset_constructor
     character(kind=c_char)        :: name !< Name of the dataset
     integer(kind=c_size_t), value :: name_length !< How many characters in the dataset's name
     type(c_ptr)                   :: dataset !< Receives the constructed dataset
   end function dataset_constructor
 end interface
+
+interface
+  function dataset_to_string_c(client) bind(c, name="dataset_to_string")
+    use iso_c_binding, only : c_ptr, c_char
+    type(c_ptr)                   :: dataset_to_string_c
+    type(c_ptr), value            :: client
+  end function dataset_to_string_c
+end interface
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/get_meta_scalars_common.inc` & `smartredis-0.4.0/src/fortran/dataset/get_meta_scalars_common.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/metadata_interfaces.inc` & `smartredis-0.4.0/src/fortran/dataset/metadata_interfaces.inc`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -64,8 +64,22 @@
     character(kind=c_char),        intent(in)    :: name(*)     !< The name to use to reference the metadata
     integer(kind=c_size_t), value, intent(in)    :: name_length !< The length of the name c-string,
                                                                 !! excluding null terminating character
     integer(kind=c_size_t),        intent(  out) :: length      !< The number of entries in the field
     integer(kind=enum_kind),       intent(  out) :: data_type   !< The c-type of the data
     type(c_ptr),                   intent(  out) :: scalar_data !< Receives scalar data
   end function get_meta_scalars_c
-end interface
+end interface
+
+interface
+  function get_metadata_field_type_c( dataset, name, name_length, mdtype ) &
+      bind(c, name="get_metadata_field_type")
+    use iso_c_binding, only : c_ptr, c_size_t, c_char
+    import :: enum_kind
+    integer(kind=enum_kind)                     :: get_metadata_field_type_c
+    type(c_ptr),             value, intent(in)  :: dataset     !< A c_ptr to the dataset object
+    character(kind=c_char),         intent(in)  :: name(*)     !< The name of the metadata field
+    integer(kind=c_size_t),  value, intent(in)  :: name_length !< The length of the name c-string,
+                                                               !! excluding null terminating character
+    integer(kind=enum_kind),        intent(out) :: mdtype      !< Receives the metadata type
+  end function get_metadata_field_type_c
+end interface
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc` & `smartredis-0.4.0/src/fortran/errors.F90`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -20,25 +20,68 @@
 ! FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 ! DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 ! SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-interface
-  function unpack_dataset_tensor_c(dataset, name, name_length, result, dims, &
-      n_dims, data_type, mem_layout) bind(c, name="unpack_dataset_tensor")
-    use iso_c_binding, only: c_ptr, c_char, c_size_t
-    import :: enum_kind
-    integer(kind=enum_kind)                                 :: unpack_dataset_tensor_c
-    type(c_ptr),                          value, intent(in) :: dataset     !< Pointer to the initialized client
-    character(kind=c_char),                      intent(in) :: name(*)     !< The name to use to place the tensor
-    integer(kind=c_size_t),               value, intent(in) :: name_length !< The length of the name c-string,
-                                                                          !! excluding null terminating character
-    type(c_ptr),                          value, intent(in) :: result     !< A c ptr to the beginning of the data
-    type(c_ptr),                          value, intent(in) :: dims       !< Length along each dimension of the
-                                                                          !! tensor
-    integer(kind=c_size_t),               value, intent(in) :: n_dims     !< The number of dimensions of the tensor
-    integer(kind=enum_kind),              value, intent(in) :: data_type  !< The data type of the tensor
-    integer(kind=enum_kind),              value, intent(in) :: mem_layout !< The memory layout of the data
-  end function unpack_dataset_tensor_c
-end interface
+module smartredis_errors
+
+use iso_c_binding, only : c_ptr, c_char, c_size_t, c_f_pointer
+
+use, intrinsic :: iso_fortran_env, only: stderr => error_unit
+implicit none; private
+
+#include "enum_fortran.inc"
+#include "errors/errors_interfaces.inc"
+
+public :: get_last_error, print_last_error
+
+contains
+
+!> Convert a pointer view of a string to a Fortran string
+function make_str(strptr, str_len)
+  character(kind=c_char, len=:), allocatable :: make_str
+  type(c_ptr), intent(in), value             :: strptr
+  integer(kind=c_size_t)                     :: str_len
+
+  character(len=str_len, kind=c_char), pointer :: ptrview
+  call c_f_pointer(strptr, ptrview)
+  make_str = ptrview
+end function make_str
+
+!> Get the last error that occurred in the SmartRedis library
+function get_last_error()
+  character(kind=c_char, len=:), allocatable :: get_last_error  !< Text associated with the last error
+
+  character(kind=c_char, len=:), allocatable :: last_error, last_error_loc
+  type(c_ptr)                                :: cerrstr, clocstr
+  integer(kind=c_size_t)                     :: cerrstr_len, clocstr_len
+
+  ! Get the last error string from C
+  cerrstr = c_get_last_error()
+  cerrstr_len = c_strlen(cerrstr)
+  last_error = make_str(cerrstr, cerrstr_len)
+
+  ! Get the last error location string from C
+  clocstr = c_get_last_error_location()
+  clocstr_len = c_strlen(clocstr)
+  last_error_loc = make_str(clocstr, clocstr_len)
+
+  get_last_error = last_error//new_line('a')//last_error_loc
+end function get_last_error
+
+!> Print the last error that occurred in the SmartRedis libary
+subroutine print_last_error(unit)
+  integer, optional, intent(in)              :: unit
+
+  ! Determine which unit to write to
+  integer :: target_unit
+  target_unit = STDERR
+  if (present(unit)) target_unit = unit
+
+  ! Write the error to the target unit
+  write(target_unit,*) get_last_error()
+end subroutine print_last_error
+
+end module smartredis_errors
+
```

### Comparing `smartredis-0.3.1/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc` & `smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -23,15 +23,14 @@
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
   !** Beginning of code common to all unpack_dataset_tensor subroutines
 
   ! Local variables
-  integer(kind=c_size_t) :: ndim ! Number of dimensions
   type(c_ptr) :: data_ptr, c_dims_ptr
   character(kind=c_char, len=len_trim(name)) :: c_name !< Transformed fortran 'name' to a c-string
   integer(kind=c_size_t) :: name_length, c_n_dims
   integer(kind=c_size_t), target :: c_dims(size(dims))
   integer(kind=enum_kind) :: data_type, mem_layout
 
   c_name = trim(name)
```

### Comparing `smartredis-0.3.1/src/fortran/dataset.F90` & `smartredis-0.4.0/src/fortran/dataset.F90`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -25,52 +25,77 @@
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 module smartredis_dataset
 
 use iso_c_binding,   only : c_ptr, c_bool, c_null_ptr, c_char, c_int
 use iso_c_binding,   only : c_int8_t, c_int16_t, c_int32_t, c_int64_t, c_float, c_double, c_size_t
 use iso_c_binding,   only : c_loc, c_f_pointer
+
+use, intrinsic :: iso_fortran_env, only: stderr => error_unit
+
 use fortran_c_interop, only : enum_kind
 
 implicit none; private
 
 include 'enum_fortran.inc'
 include 'dataset/dataset_interfaces.inc'
-include 'dataset/add_tensor_interfaces.inc'
+include 'dataset/tensor_interfaces.inc'
 include 'dataset/unpack_dataset_tensor_interfaces.inc'
 include 'dataset/metadata_interfaces.inc'
+#include "errors/errors_interfaces.inc"
 
 public :: enum_kind !< The kind of integer equivalent to a C enum. According to C an Fortran
                     !! standards this should be c_int, but is renamed here to ensure that
                     !! users do not have to import the iso_c_binding module into their
                     !! programs
 
 !> Contains multiple tensors and metadata used to describe an entire set of data
 type, public :: dataset_type
   type(c_ptr) :: dataset_ptr !< A pointer to the initialized dataset object
 
   contains
 
   !> Initialize a new dataset with a given name
   procedure :: initialize => initialize_dataset
+  !> Access the raw C pointer for the client
+  procedure :: get_c_pointer
+
+  ! Metadata procedures
   !> Add metadata to the dataset with a given field and string
   procedure :: add_meta_string
-  ! procedure :: get_meta_strings ! Not supported currently
+  ! Retrieve the strings associated with a metadata string field
+  !> procedure :: get_meta_strings ! Not supported currently
+  !> Add metadata of type 'scalar' into a given field
+  generic :: add_meta_scalar => add_meta_scalar_double, add_meta_scalar_float, add_meta_scalar_i32, add_meta_scalar_i64
+  !> Retrieve scalar-type metadata as a vector
+  generic :: get_meta_scalars => get_meta_scalars_double, get_meta_scalars_float, get_meta_scalars_i32, &
+                                 get_meta_scalars_i64
+  ! Retrieve the names of metadata fields
+  !> procedure :: get_metadata_field_names ! Not supported currently
+  !> Retrieve the type for a metadata field
+  procedure :: get_metadata_field_type
+
+  ! Tensor procedures
   !> Add a tensor to be included as part of the dataset
   generic :: add_tensor => add_tensor_i8, add_tensor_i16, add_tensor_i32, add_tensor_i64, &
                            add_tensor_float, add_tensor_double
   !> Unpack a tensor that has previously been added to the dataset
   generic :: unpack_dataset_tensor => unpack_dataset_tensor_i8, unpack_dataset_tensor_i16, &
                                       unpack_dataset_tensor_i32, unpack_dataset_tensor_i64, &
                                       unpack_dataset_tensor_float, unpack_dataset_tensor_double
-  !> Add metadata of type 'scalar' into a given field
-  generic :: add_meta_scalar => add_meta_scalar_double, add_meta_scalar_float, add_meta_scalar_i32, add_meta_scalar_i64
-  !> Retrieve scalar-type metadata as a vector
-  generic :: get_meta_scalars => get_meta_scalars_double, get_meta_scalars_float, get_meta_scalars_i32, &
-                                 get_meta_scalars_i64
+  ! Retrieve the names of tensors
+  !> procedure :: get_tensor_names ! Not supported currently
+  !> Retrieve the type for a tensor
+  procedure :: get_tensor_type
+  !> Retrieve the dimensions for a tensor
+  procedure :: get_tensor_dims
+  !> Retrieve a string representation of the dataset
+  procedure :: to_string
+  !> Print a string representation of the dataset
+  procedure :: print_dataset
 
   ! Private procedures
   procedure, private :: add_tensor_i8
   procedure, private :: add_tensor_i16
   procedure, private :: add_tensor_i32
   procedure, private :: add_tensor_i64
   procedure, private :: add_tensor_float
@@ -106,14 +131,21 @@
 
   name_length = len_trim(name)
   c_name = trim(name)
 
   code = dataset_constructor(c_name, name_length, self%dataset_ptr)
 end function initialize_dataset
 
+!> Access the raw C pointer for the dataset
+function get_c_pointer(self)
+  type(c_ptr)                     :: get_c_pointer
+  class(dataset_type), intent(in) :: self
+  get_c_pointer = self%dataset_ptr
+end function get_c_pointer
+
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'int8' C-type
 function add_tensor_i8(self, name, data, dims) result(code)
   integer(kind=c_int8_t), dimension(..), target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
@@ -307,52 +339,44 @@
 !> Get scalar metadata whose Fortran type is the equivalent 'int32' C-type
 function get_meta_scalars_i32(self, name, meta) result(code)
   class(dataset_type),                intent(in) :: self !< The dataset
   character(len=*),                   intent(in) :: name !< The name of the metadata field
   integer(kind=c_int32_t), dimension(:), pointer :: meta !< The actual metadata
   integer(kind=enum_kind)                        :: code !< Result of the operation
 
-  ! local variables
-  integer(kind=enum_kind) :: expected_data_type = meta_int32
   include 'dataset/get_meta_scalars_common.inc'
 end function get_meta_scalars_i32
 
 !> Get scalar metadata whose Fortran type is the equivalent 'int64' C-type
 function get_meta_scalars_i64(self, name, meta) result(code)
   class(dataset_type),                intent(in) :: self !< The dataset
   character(len=*),                   intent(in) :: name !< The name of the metadata field
   integer(kind=c_int64_t), dimension(:), pointer :: meta !< The actual metadata
   integer(kind=enum_kind)                        :: code !< Result of the operation
 
-  ! local variables
-  integer(kind=enum_kind) :: expected_data_type = meta_int64
   include 'dataset/get_meta_scalars_common.inc'
 end function get_meta_scalars_i64
 
 !> Get scalar metadata whose Fortran type is the equivalent 'float' C-type
 function get_meta_scalars_float(self, name, meta) result(code)
   class(dataset_type),           intent(in) :: self !< The dataset
   character(len=*),              intent(in) :: name !< The name of the metadata field
   real(kind=c_float), dimension(:), pointer :: meta !< The actual metadata
   integer(kind=enum_kind)                   :: code !< Result of the operation
 
-  ! local variables
-  integer(kind=enum_kind) :: expected_data_type = meta_flt
   include 'dataset/get_meta_scalars_common.inc'
 end function get_meta_scalars_float
 
 !> Get scalar metadata whose Fortran type is the equivalent 'double' C-type
 function get_meta_scalars_double(self, name, meta) result(code)
   class(dataset_type),            intent(in) :: self !< The dataset
   character(len=*),               intent(in) :: name !< The name of the metadata field
   real(kind=c_double), dimension(:), pointer :: meta !< The actual metadata
   integer(kind=enum_kind)                    :: code !< Result of the operation
 
-  ! local variables
-  integer(kind=enum_kind) :: expected_data_type = meta_dbl
   include 'dataset/get_meta_scalars_common.inc'
 end function get_meta_scalars_double
 
 !> Add scalar metadata whose Fortran type is the equivalent 'int32' C-type
 function add_meta_scalar_i32(self, name, meta) result(code)
   class(dataset_type),             intent(in) :: self !< The dataset
   character(len=*),                intent(in) :: name !< The name of the metadata field
@@ -397,15 +421,15 @@
 
   ! local variables
   integer(kind=enum_kind), parameter :: meta_type = meta_dbl
   include 'dataset/add_meta_scalar_common.inc'
 end function add_meta_scalar_double
 
 !> Add string-like metadata to the dataset
-function add_meta_string( self, name, meta) result(code)
+function add_meta_string(self, name, meta) result(code)
   class(dataset_type),     intent(in) :: self !< The dataset
   character(len=*),        intent(in) :: name !< The name of the metadata field
   character(len=*),        intent(in) :: meta !< The actual metadata
   integer(kind=enum_kind)             :: code !< Result of the operation
 
   ! local variables
   character(kind=c_char, len=len_trim(meta)) :: c_meta
@@ -418,8 +442,113 @@
 
   meta_length = len_trim(c_meta)
   name_length = len_trim(c_name)
 
   code = add_meta_string_c(self%dataset_ptr, c_name, name_length, c_meta, meta_length)
 end function add_meta_string
 
+!> Retrieve the type for a metadata field
+function get_metadata_field_type(self, name, mdtype) result(code)
+  class(dataset_type),     intent(in)  :: self   !< The dataset
+  character(len=*),        intent(in)  :: name   !< The name of the metadata field
+  integer(kind=enum_kind), intent(out) :: mdtype !< Receives the type
+  integer(kind=enum_kind)              :: code   !< Result of the operation
+
+  ! local variables
+  character(kind=c_char, len=len_trim(name)) :: c_name
+  integer(kind=c_size_t) :: name_length
+
+  c_name = trim(name)
+  name_length = len_trim(c_name)
+
+  code = get_metadata_field_type_c(self%dataset_ptr, c_name, name_length, mdtype)
+end function get_metadata_field_type
+
+!> Retrieve the type for a tensor
+function get_tensor_type(self, name, ttype) result(code)
+  class(dataset_type),     intent(in)  :: self  !< The dataset
+  character(len=*),        intent(in)  :: name  !< The name of the tensor
+  integer(kind=enum_kind), intent(out) :: ttype !< Receives the type
+  integer(kind=enum_kind)              :: code  !< Result of the operation
+
+  ! local variables
+  character(kind=c_char, len=len_trim(name)) :: c_name
+  integer(kind=c_size_t) :: name_length
+
+  c_name = trim(name)
+  name_length = len_trim(c_name)
+
+  code = get_tensor_type_c(self%dataset_ptr, c_name, name_length, ttype)
+end function get_tensor_type
+
+
+!> Retrieve the dimensions for a tensor into a supplied buffer, or receive the
+!! number of dimensions if the supplied buffer is too small
+function get_tensor_dims(self, name, dims, dims_length) result(code)
+  class(dataset_type),     intent(in)    :: self  !< The dataset
+  character(len=*),        intent(in)    :: name  !< The name of the tensor
+  integer, dimension(:), target, intent(inout) :: dims !< Receives the tensor dimensions
+  integer,  intent(inout) :: dims_length !< Receives the number of tensor dimensions
+  integer(kind=enum_kind)                :: code  !< Result of the operation
+
+  ! local variables
+  character(kind=c_char, len=len_trim(name)) :: c_name
+  integer(kind=c_size_t) :: name_length
+  type(c_ptr) :: dims_ptr
+  integer(kind=c_size_t), dimension(size(dims)), target :: c_dims
+  integer(kind=c_size_t) ::  c_dims_length
+
+  c_name = trim(name)
+  name_length = len_trim(c_name)
+
+  if (dims_length .gt. size(dims)) then
+    error stop 'dims_length .gt. size(dims) in call to get_tensor_dims'
+  end if
+  dims_ptr = c_loc(c_dims)
+  c_dims_length = dims_length
+
+  code = get_tensor_dims_c(self%dataset_ptr, c_name, name_length, dims_ptr, c_dims_length)
+  dims = int(c_dims, kind(dims))
+  dims_length = int(c_dims_length, kind(dims_length))
+end function get_tensor_dims
+
+
+!> Retrieve a string representation of the dataset
+function to_string(self)
+  character(kind=c_char, len=:), allocatable :: to_string !< Text version of dataset
+  class(dataset_type),     intent(in)        :: self      !< The dataset
+
+  type(c_ptr)                                :: c_ds_str
+  integer(kind=c_size_t)                     :: c_ds_str_len
+
+  ! Get the string representation of the dataset from C
+  c_ds_str = dataset_to_string_c(self%dataset_ptr)
+  c_ds_str_len = c_strlen(c_ds_str)
+  to_string = make_str(c_ds_str, c_ds_str_len)
+end function to_string
+
+!> Convert a pointer view of a string to a Fortran string
+function make_str(strptr, str_len)
+  character(kind=c_char, len=:), allocatable :: make_str
+  type(c_ptr), intent(in), value             :: strptr
+  integer(kind=c_size_t)                     :: str_len
+
+  character(len=str_len, kind=c_char), pointer :: ptrview
+  call c_f_pointer(strptr, ptrview)
+  make_str = ptrview
+end function make_str
+
+!> Print a string representation of the dataset
+subroutine print_dataset(self, unit)
+  class(dataset_type), intent(in)  :: self  !< The dataset
+  integer, optional,   intent(in)  :: unit !< Unit to which to print the dataset
+
+  ! Determine which unit to write to
+  integer :: target_unit
+  target_unit = STDERR
+  if (present(unit)) target_unit = unit
+
+  ! Write the error to the target unit
+  write(target_unit,*) to_string(self)
+end subroutine print_dataset
+
 end module smartredis_dataset
```

### Comparing `smartredis-0.3.1/src/fortran/fortran_c_interop.F90` & `smartredis-0.4.0/src/fortran/fortran_c_interop.F90`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ! BSD 2-Clause License
 !
-! Copyright (c) 2021-2022, Hewlett Packard Enterprise
+! Copyright (c) 2021-2023, Hewlett Packard Enterprise
 ! All rights reserved.
 !
 ! Redistribution and use in source and binary forms, with or without
 ! modification, are permitted provided that the following conditions are met:
 !
 ! 1. Redistributions of source code must retain the above copyright notice, this
 !    list of conditions and the following disclaimer.
@@ -23,65 +23,77 @@
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 module fortran_c_interop
 
 use iso_c_binding, only : c_ptr, c_char, c_size_t, c_loc, c_null_ptr, c_int
+use iso_fortran_env, only : stderr => error_unit
 
 implicit none; private
 
 integer, parameter, public :: enum_kind = c_int !< The kind of integer equivalent to a C enum. According
                                                 !! to the standard this is a c_int
+integer, parameter, public :: C_MAX_STRING = 255 !< A bug in gfortran prevents the use of deferred length, allocatable
+                                                 !! character arrays. This parameter specifies the maximum length of a
+                                                 !! string passed to the C interface
+#include "enum_fortran.inc"
 public :: convert_char_array_to_c
 
 contains
 
 !> Returns pointers to the start of each string and lengths for each string in a Fortran character array
-subroutine convert_char_array_to_c(character_array_f, character_array_c, string_ptrs, ptr_to_string_ptrs, &
-                                   string_lengths, ptr_to_string_lengths, n_strings )
+function convert_char_array_to_c(character_array_f, character_array_c, string_ptrs, ptr_to_string_ptrs, &
+                                   string_lengths, ptr_to_string_lengths, n_strings ) result(code)
   !> The 2D Fortran character array
   character(len=*),             dimension(:),                      intent(in   ) :: character_array_f
   !> The character array converted to c_character types
-  character(kind=c_char,len=:), dimension(:), allocatable, target, intent(  out) :: character_array_c
+  character(kind=c_char,len=C_MAX_STRING), dimension(:), allocatable, target, intent(  out) :: character_array_c
   !> C-style pointers to the start of each string
   type(c_ptr),                  dimension(:), allocatable, target, intent(  out) :: string_ptrs
   !> A pointer to the the string pointers
   type(c_ptr),                                                     intent(  out) :: ptr_to_string_ptrs
   !> The length of each string
   integer(kind=c_size_t),       dimension(:), allocatable, target, intent(  out) :: string_lengths
   !> Pointer to the array containing the string_lengths
   type(c_ptr),                                                     intent(  out) :: ptr_to_string_lengths
   !> The length of each string
   integer(kind=c_size_t),                                          intent(  out) :: n_strings
+  integer(kind=enum_kind) :: code
 
-  integer :: i, max_length, length
+  integer :: max_length, length
+  integer(kind=c_size_t) :: i
 
+  code = SRNoError
   ! Find the size of the 2D array and allocate some of the 1D arrays
   n_strings= size(character_array_f)
   allocate(string_lengths(n_strings))
   allocate(string_ptrs(n_strings))
+  allocate(character_array_c(n_strings))
 
   ! Need to find the length of the string, so we can allocate the c_array
   max_length = 0
   do i=1,n_strings
     length = len_trim(character_array_f(i))
     max_length = max(max_length, length)
     string_lengths(i) = length
   enddo
+  if (max_length > C_MAX_STRING) then
+    code = SRRuntimeError
+    write(stderr,*) "Length of string exceeded, increase C_MAX_STRING and recompile"
+  endif
   ptr_to_string_lengths = c_loc(string_lengths)
-  allocate(character(len=max_length) :: character_array_c(n_strings))
 
   ! Copy the character into a c_char and create pointers to each of the strings
   do i=1,n_strings
      if (string_lengths(i) .gt. 0) then
-        character_array_c(i) = transfer(character_array_f(i),character_array_c(i))
+        character_array_c(i) = character_array_f(i)
         string_ptrs(i) = c_loc(character_array_c(i))
      else
         string_ptrs(i) = c_null_ptr;
      endif
   enddo
   ptr_to_string_ptrs = c_loc(string_ptrs)
 
-end subroutine convert_char_array_to_c
+end function convert_char_array_to_c
 
 end module fortran_c_interop
```

### Comparing `smartredis-0.3.1/src/python/module/smartredis/client.py` & `smartredis-0.4.0/src/python/module/smartredis/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -28,47 +28,64 @@
 import os
 import os.path as osp
 import functools
 
 import numpy as np
 
 from .dataset import Dataset
+from .srobject import SRObject
 from .smartredisPy import PyClient
 from .util import Dtypes, init_default, exception_handler, typecheck
 
 from .error import *
 from .smartredisPy import RedisReplyError as PybindRedisReplyError
 
-class Client(PyClient):
-    def __init__(self, address=None, cluster=False):
+class Client(SRObject):
+    def __init__(self, address=None, cluster=False, logger_name="default"):
         """Initialize a RedisAI client
 
         For clusters, the address can be a single tcp/ip address and port
         of a database node. The rest of the cluster will be discovered
         by the client itself. (e.g. address="127.0.0.1:6379")
 
         If an address is not set, the client will look for the environment
         variable ``SSDB`` (e.g. SSDB="127.0.0.1:6379;")
 
         :param address: Address of the database
         :param cluster: True if connecting to a redis cluster, defaults to False
         :type cluster: bool, optional
+        :param logger_name: Identifier for the current client
+        :type logger_name: str
         :raises RedisConnectionError: if connection initialization fails
         """
         if address:
             self.__set_address(address)
         if "SSDB" not in os.environ:
             raise RedisConnectionError("Could not connect to database. $SSDB not set")
         try:
-            super().__init__(cluster)
+            super().__init__(PyClient(cluster, logger_name))
         except PybindRedisReplyError as e:
             raise RedisConnectionError(str(e)) from None
         except RuntimeError as e:
             raise RedisConnectionError(str(e)) from None
 
+    def __str__(self):
+        """Create a string representation of the client
+
+        :return: A string representation of the client
+        :rtype: str
+        """
+        return self._client.to_string()
+
+    @property
+    def _client(self):
+        """Alias _srobject to _client
+        """
+        return self._srobject
+
     @exception_handler
     def put_tensor(self, name, data):
         """Put a tensor to a Redis database
 
         The final tensor key under which the tensor is stored
         may be formed by applying a prefix to the supplied
         name. See use_tensor_ensemble_prefix() for more details.
@@ -78,15 +95,15 @@
         :param data: numpy array of tensor data
         :type data: np.array
         :raises RedisReplyError: if put fails
         """
         typecheck(name, "name", str)
         typecheck(data, "data", np.ndarray)
         dtype = Dtypes.tensor_from_numpy(data)
-        super().put_tensor(name, dtype, data)
+        self._client.put_tensor(name, dtype, data)
 
     @exception_handler
     def get_tensor(self, name):
         """Get a tensor from the database
 
         The tensor key used to locate the tensor
         may be formed by applying a prefix to the supplied
@@ -96,15 +113,15 @@
         :param name: name to get tensor from
         :type name: str
         :raises RedisReplyError: if get fails
         :return: numpy array of tensor data
         :rtype: np.array
         """
         typecheck(name, "name", str)
-        return super().get_tensor(name)
+        return self._client.get_tensor(name)
 
     @exception_handler
     def delete_tensor(self, name):
         """Delete a tensor from the database
 
         The tensor key used to locate the tensor to be deleted
         may be formed by applying a prefix to the supplied
@@ -112,15 +129,15 @@
         and use_tensor_ensemble_prefix() for more details.
 
         :param name: name tensor is stored at
         :type name: str
         :raises RedisReplyError: if deletion fails
         """
         typecheck(name, "name", str)
-        super().delete_tensor(name)
+        self._client.delete_tensor(name)
 
     @exception_handler
     def copy_tensor(self, src_name, dest_name):
         """Copy a tensor at one name to another name
 
         The source and destination tensor keys used to locate
         and store the tensor may be formed by applying prefixes
@@ -131,15 +148,15 @@
         :type src_name: str
         :param dest_name: name to store new copy at
         :type dest_name: str
         :raises RedisReplyError: if copy operation fails
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
-        super().copy_tensor(src_name, dest_name)
+        self._client.copy_tensor(src_name, dest_name)
 
     @exception_handler
     def rename_tensor(self, old_name, new_name):
         """Rename a tensor in the database
 
         The old and new tensor keys used to find and relocate
         the tensor may be formed by applying prefixes to the supplied
@@ -150,110 +167,110 @@
         :type old_name: str
         :param new_name: new name for the tensor
         :type new_name: str
         :raises RedisReplyError: if rename operation fails
         """
         typecheck(old_name, "old_name", str)
         typecheck(new_name, "new_name", str)
-        super().rename_tensor(old_name, new_name)
+        self._client.rename_tensor(old_name, new_name)
 
     @exception_handler
     def put_dataset(self, dataset):
         """Put a Dataset instance into the database
 
         The final dataset key under which the dataset is stored
         is generated from the name that was supplied when the
         dataset was created and may be prefixed. See
-        use_tensor_ensemble_prefix() for more details.
+        use_dataset_ensemble_prefix() for more details.
 
         All associated tensors and metadata within the Dataset
         instance will also be stored.
 
         :param dataset: a Dataset instance
         :type dataset: Dataset
         :raises TypeError: if argument is not a Dataset
         :raises RedisReplyError: if update fails
         """
         typecheck(dataset, "dataset", Dataset)
         pybind_dataset = dataset.get_data()
-        super().put_dataset(pybind_dataset)
+        self._client.put_dataset(pybind_dataset)
 
     @exception_handler
     def get_dataset(self, name):
         """Get a dataset from the database
 
         The dataset key used to locate the dataset
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
-        and use_tensor_ensemble_prefix() for more details.
+        and use_dataset_ensemble_prefix() for more details.
 
         :param name: name the dataset is stored under
         :type name: str
         :raises RedisReplyError: if retrieval fails
         :return: Dataset instance
         :rtype: Dataset
         """
         typecheck(name, "name", str)
-        dataset = super().get_dataset(name)
+        dataset = self._client.get_dataset(name)
         python_dataset = Dataset.from_pybind(dataset)
         return python_dataset
 
     @exception_handler
     def delete_dataset(self, name):
         """Delete a dataset within the database
 
         The dataset key used to locate the dataset to be deleted
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
-        and use_tensor_ensemble_prefix() for more details.
+        and use_dataset_ensemble_prefix() for more details.
 
         :param name: name of the dataset
         :type name: str
         :raises RedisReplyError: if deletion fails
         """
         typecheck(name, "name", str)
-        super().delete_dataset(name)
+        self._client.delete_dataset(name)
 
     @exception_handler
     def copy_dataset(self, src_name, dest_name):
         """Copy a dataset from one key to another
 
         The source and destination dataset keys used to
         locate the dataset may be formed by applying prefixes
         to the supplied src_name and dest_name. See set_data_source()
-        and use_tensor_ensemble_prefix() for more details.
+        and use_dataset_ensemble_prefix() for more details.
 
         :param src_name: source name for dataset to be copied
         :type src_name: str
         :param dest_name: new name of dataset
         :type dest_name: str
         :raises RedisReplyError: if copy operation fails
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
-        super().copy_dataset(src_name, dest_name)
+        self._client.copy_dataset(src_name, dest_name)
 
     @exception_handler
     def rename_dataset(self, old_name, new_name):
         """Rename a dataset in the database
 
         The old and new dataset keys used to find and relocate
         the dataset may be formed by applying prefixes to the supplied
         old_name and new_name. See set_data_source()
-        and use_tensor_ensemble_prefix() for more details.
+        and use_dataset_ensemble_prefix() for more details.
 
         :param old_name: original name of the dataset to be renamed
         :type old_name: str
         :param new_name: new name for the dataset
         :type new_name: str
         :raises RedisReplyError: if rename operation fails
         """
         typecheck(old_name, "old_name", str)
         typecheck(new_name, "new_name", str)
-        super().rename_dataset(old_name, new_name)
+        self._client.rename_dataset(old_name, new_name)
 
     @exception_handler
     def set_function(self, name, function, device="CPU"):
         """Set a callable function into the database
 
         The final script key used to store the function may be formed
         by applying a prefix to the supplied name.
@@ -276,15 +293,15 @@
         """
         typecheck(name, "name", str)
         typecheck(device, "device", str)
         if not callable(function):
             raise TypeError(f"Argument provided for function, {type(function)}, is not callable")
         device = self.__check_device(device)
         fn_src = inspect.getsource(function)
-        super().set_script(name, device, fn_src)
+        self._client.set_script(name, device, fn_src)
 
     @exception_handler
     def set_function_multigpu(self, name, function, first_gpu, num_gpus):
         """Set a callable function into the database for use
         in a multi-GPU system
 
         The final script key used to store the function may be formed
@@ -308,15 +325,15 @@
         """
         typecheck(name, "name", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         if not callable(function):
             raise TypeError(f"Argument provided for function, {type(function)}, is not callable")
         fn_src = inspect.getsource(function)
-        super().set_script_multigpu(name, fn_src, first_gpu, num_gpus)
+        self._client.set_script_multigpu(name, fn_src, first_gpu, num_gpus)
 
     @exception_handler
     def set_script(self, name, script, device="CPU"):
         """Store a TorchScript at a key in the database
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
@@ -333,15 +350,15 @@
         :type device: str, optional
         :raises RedisReplyError: if script fails to set
         """
         typecheck(name, "name", str)
         typecheck(script, "script", str)
         typecheck(device, "device", str)
         device = self.__check_device(device)
-        super().set_script(name, device, script)
+        self._client.set_script(name, device, script)
 
     @exception_handler
     def set_script_multigpu(self, name, script, first_gpu, num_gpus):
         """Store a TorchScript at a key in the database
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
@@ -357,15 +374,15 @@
         :type num_gpus: int
         :raises RedisReplyError: if script fails to set
         """
         typecheck(name, "name", str)
         typecheck(script, "script", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
-        super().set_script_multigpu(name, script, first_gpu, num_gpus)
+        self._client.set_script_multigpu(name, script, first_gpu, num_gpus)
 
     @exception_handler
     def set_script_from_file(self, name, file, device="CPU"):
         """Same as Client.set_script, but from file
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
@@ -380,15 +397,15 @@
         :raises RedisReplyError: if script fails to set
         """
         typecheck(name, "name", str)
         typecheck(file, "file", str)
         typecheck(device, "device", str)
         device = self.__check_device(device)
         file_path = self.__check_file(file)
-        super().set_script_from_file(name, device, file_path)
+        self._client.set_script_from_file(name, device, file_path)
 
     @exception_handler
     def set_script_from_file_multigpu(self, name, file, first_gpu, num_gpus):
         """Same as Client.set_script_multigpu, but from file
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
@@ -405,15 +422,15 @@
         :raises RedisReplyError: if script fails to set
         """
         typecheck(name, "name", str)
         typecheck(file, "file", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         file_path = self.__check_file(file)
-        super().set_script_from_file_multigpu(name, file_path, first_gpu, num_gpus)
+        self._client.set_script_from_file_multigpu(name, file_path, first_gpu, num_gpus)
 
     @exception_handler
     def get_script(self, name):
         """Retrieve a Torchscript stored in the database
 
         The script key used to locate the script
         may be formed by applying a prefix to the supplied
@@ -423,15 +440,15 @@
         :param name: the name at which script is stored
         :type name: str
         :raises RedisReplyError: if script retrieval fails
         :return: TorchScript stored at name
         :rtype: str
         """
         typecheck(name, "name", str)
-        script = super().get_script(name)
+        script = self._client.get_script(name)
         return script
 
     @exception_handler
     def run_script(self, name, fn_name, inputs, outputs):
         """Execute TorchScript stored inside the database
 
         The script key used to locate the script to be run
@@ -452,15 +469,15 @@
         :raises RedisReplyError: if script execution fails
         """
         typecheck(name, "name", str)
         typecheck(fn_name, "fn_name", str)
         typecheck(inputs, "inputs", list)
         typecheck(outputs, "outputs", list)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().run_script(name, fn_name, inputs, outputs)
+        self._client.run_script(name, fn_name, inputs, outputs)
 
     @exception_handler
     def run_script_multigpu(
         self, name, fn_name, inputs, outputs, offset, first_gpu, num_gpus):
         """Execute TorchScript stored inside the database
 
         The script key used to locate the script to be run
@@ -491,15 +508,15 @@
         typecheck(fn_name, "fn_name", str)
         typecheck(inputs, "inputs", list)
         typecheck(outputs, "outputs", list)
         typecheck(offset, "offset", int)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().run_script_multigpu(
+        self._client.run_script_multigpu(
             name, fn_name, inputs, outputs, offset, first_gpu, num_gpus)
 
     @exception_handler
     def delete_script(self, name):
         """Remove a script from the database
 
         The script key used to locate the script to be run
@@ -508,15 +525,15 @@
         for more details
 
         :param name: the name the script is stored under
         :type name: str
         :raises RedisReplyError: if script deletion fails
         """
         typecheck(name, "name", str)
-        super().delete_script(name)
+        self._client.delete_script(name)
 
     @exception_handler
     def delete_script_multigpu(self, name, first_gpu, num_gpus):
         """Remove a script from the database
 
         The script key used to locate the script to be run
         may be formed by applying a prefix to the supplied
@@ -530,15 +547,15 @@
         :param num_gpus: the number of gpus for which the script was stored
         :type num_gpus: int
         :raises RedisReplyError: if script deletion fails
         """
         typecheck(name, "name", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
-        super().delete_script_multigpu(name, first_gpu, num_gpus)
+        self._client.delete_script_multigpu(name, first_gpu, num_gpus)
 
     @exception_handler
     def get_model(self, name):
         """Get a stored model
 
         The model key used to locate the model
         may be formed by applying a prefix to the supplied
@@ -548,15 +565,15 @@
         :param name: name of stored model
         :type name: str
         :raises RedisReplyError: if retrieval fails
         :return: model
         :rtype: bytes
         """
         typecheck(name, "name", str)
-        model = super().get_model(name)
+        model = self._client.get_model(name)
         return model
 
     @exception_handler
     def set_model(
         self,
         name,
         model,
@@ -604,15 +621,15 @@
         typecheck(device, "device", str)
         typecheck(batch_size, "batch_size", int)
         typecheck(min_batch_size, "min_batch_size", int)
         typecheck(tag, "tag", str)
         device = self.__check_device(device)
         backend = self.__check_backend(backend)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().set_model(
+        self._client.set_model(
             name,
             model,
             backend,
             device,
             batch_size,
             min_batch_size,
             tag,
@@ -671,15 +688,15 @@
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         typecheck(batch_size, "batch_size", int)
         typecheck(min_batch_size, "min_batch_size", int)
         typecheck(tag, "tag", str)
         backend = self.__check_backend(backend)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().set_model_multigpu(
+        self._client.set_model_multigpu(
             name,
             model,
             backend,
             first_gpu,
             num_gpus,
             batch_size,
             min_batch_size,
@@ -739,15 +756,15 @@
         typecheck(batch_size, "batch_size", int)
         typecheck(min_batch_size, "min_batch_size", int)
         typecheck(tag, "tag", str)
         device = self.__check_device(device)
         backend = self.__check_backend(backend)
         m_file = self.__check_file(model_file)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().set_model_from_file(
+        self._client.set_model_from_file(
             name,
             m_file,
             backend,
             device,
             batch_size,
             min_batch_size,
             tag,
@@ -808,15 +825,15 @@
         typecheck(num_gpus, "num_gpus", int)
         typecheck(batch_size, "batch_size", int)
         typecheck(min_batch_size, "min_batch_size", int)
         typecheck(tag, "tag", str)
         backend = self.__check_backend(backend)
         m_file = self.__check_file(model_file)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().set_model_from_file_multigpu(
+        self._client.set_model_from_file_multigpu(
             name,
             m_file,
             backend,
             first_gpu,
             num_gpus,
             batch_size,
             min_batch_size,
@@ -840,15 +857,15 @@
         :type inputs: list[str], optional
         :param outputs: names to store outputs under, defaults to None
         :type outputs: list[str], optional
         :raises RedisReplyError: if model execution fails
         """
         typecheck(name, "name", str)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().run_model(name, inputs, outputs)
+        self._client.run_model(name, inputs, outputs)
 
     @exception_handler
     def run_model_multigpu(
         self,
         name,
         offset,
         first_gpu,
@@ -878,15 +895,15 @@
         :raises RedisReplyError: if model execution fails
         """
         typecheck(name, "name", str)
         typecheck(offset, "offset", int)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        super().run_model_multigpu(name, inputs, outputs, offset, first_gpu, num_gpus)
+        self._client.run_model_multigpu(name, inputs, outputs, offset, first_gpu, num_gpus)
 
     @exception_handler
     def delete_model(self, name):
         """Remove a model from the database
 
         The model key used to locate the script to be run
         may be formed by applying a prefix to the supplied
@@ -894,15 +911,15 @@
         for more details
 
         :param name: the name the model is stored under
         :type name: str
         :raises RedisReplyError: if model deletion fails
         """
         typecheck(name, "name", str)
-        super().delete_model(name)
+        self._client.delete_model(name)
 
     @exception_handler
     def delete_model_multigpu(self, name, first_gpu, num_gpus):
         """Remove a model from the database that was stored for use with multiple GPUs
 
         The model key used to locate the script to be run
         may be formed by applying a prefix to the supplied
@@ -916,15 +933,15 @@
         :param num_gpus: the number of gpus for which the model was stored
         :type num_gpus: int
         :raises RedisReplyError: if model deletion fails
         """
         typecheck(name, "name", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
-        super().delete_model_multigpu(name, first_gpu, num_gpus)
+        self._client.delete_model_multigpu(name, first_gpu, num_gpus)
 
     @exception_handler
     def tensor_exists(self, name):
         """Check if a tensor exists in the database
 
         The tensor key used to check for existence
         may be formed by applying a prefix to the supplied
@@ -934,33 +951,33 @@
         :param name: The tensor name that will be checked in the database
         :type name: str
         :returns: Returns true if the tensor exists in the database
         :rtype: bool
         :raises RedisReplyError: if checking for tensor existence causes an error
         """
         typecheck(name, "name", str)
-        return super().tensor_exists(name)
+        return self._client.tensor_exists(name)
 
     @exception_handler
     def dataset_exists(self, name):
         """Check if a dataset exists in the database
 
         The dataset key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
-        and use_tensor_ensemble_prefix() for more details.
+        and use_dataset_ensemble_prefix() for more details.
 
         :param name: The dataset name that will be checked in the database
         :type name: str
         :returns: Returns true if the dataset exists in the database
         :rtype: bool
         :raises RedisReplyError: if `dataset_exists` fails (i.e. causes an error)
         """
         typecheck(name, "name", str)
-        return super().dataset_exists(name)
+        return self._client.dataset_exists(name)
 
     @exception_handler
     def model_exists(self, name):
         """Check if a model or script exists in the database
 
         The model or script key used to check for existence
         may be formed by applying a prefix to the supplied
@@ -970,28 +987,28 @@
         :param name: The model or script name that will be checked in the database
         :type name: str
         :returns: Returns true if the model exists in the database
         :rtype: bool
         :raises RedisReplyError: if `model_exists` fails (i.e. causes an error)
         """
         typecheck(name, "name", str)
-        return super().model_exists(name)
+        return self._client.model_exists(name)
 
     @exception_handler
     def key_exists(self, key):
         """Check if the key exists in the database
 
         :param key: The key that will be checked in the database
         :type key: str
         :returns: Returns true if the key exists in the database
         :rtype: bool
         :raises RedisReplyError: if `key_exists` fails
         """
         typecheck(key, "key", str)
-        return super().key_exists(key)
+        return self._client.key_exists(key)
 
     @exception_handler
     def poll_key(self, key, poll_frequency_ms, num_tries):
         """Check if the key exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
@@ -1006,15 +1023,15 @@
                   specified number of tries, otherwise false.
         :rtype: bool
         :raises RedisReplyError: if an error occurs while polling
         """
         typecheck(key, "key", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_key(key, poll_frequency_ms, num_tries)
+        return self._client.poll_key(key, poll_frequency_ms, num_tries)
 
     @exception_handler
     def poll_tensor(self, name, poll_frequency_ms, num_tries):
         """Check if a tensor exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
@@ -1033,26 +1050,26 @@
                   specified number of tries, otherwise false.
         :rtype: bool
         :raises RedisReplyError: if an error occurs while polling
         """
         typecheck(name, "name", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_tensor(name, poll_frequency_ms, num_tries)
+        return self._client.poll_tensor(name, poll_frequency_ms, num_tries)
 
     @exception_handler
     def poll_dataset(self, name, poll_frequency_ms, num_tries):
         """Check if a dataset exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
         The dataset key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
-        and use_tensor_ensemble_prefix() for more details.
+        and use_dataset_ensemble_prefix() for more details.
 
         :param name: The dataset name that will be checked in the database
         :type name: str
         :param poll_frequency_ms: The polling interval, in milliseconds
         :type poll_frequency_ms: int
         :param num_tries: The total number of retries for the check
         :type num_tries: int
@@ -1060,15 +1077,15 @@
                   specified number of tries, otherwise false.
         :rtype: bool
         :raises RedisReplyError: if an error occurs while polling
         """
         typecheck(name, "name", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_dataset(name, poll_frequency_ms, num_tries)
+        return self._client.poll_dataset(name, poll_frequency_ms, num_tries)
 
     @exception_handler
     def poll_model(self, name, poll_frequency_ms, num_tries):
         """Check if a model or script exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
@@ -1087,15 +1104,15 @@
                   specified number of tries, otherwise false.
         :rtype: bool
         :raises RedisReplyError: if an error occurs while polling
         """
         typecheck(name, "name", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_model(name, poll_frequency_ms, num_tries)
+        return self._client.poll_model(name, poll_frequency_ms, num_tries)
 
     @exception_handler
     def set_data_source(self, source_id):
         """Set the data source, a key prefix for future operations
 
         When running multiple applications, such as an ensemble
         computation, there is a risk that the same name is used
@@ -1116,15 +1133,15 @@
         :param source_id: The prefix for read operations; must have
                           previously been set via the SSKEYIN environment
                           variable
         :type source_id: str
         :raises RedisReplyError: if set data
         """
         typecheck(source_id, "source_id", str)
-        return super().set_data_source(source_id)
+        return self._client.set_data_source(source_id)
 
     @exception_handler
     def use_model_ensemble_prefix(self, use_prefix):
         """Control whether model and script keys are
            prefixed (e.g. in an ensemble) when forming database keys
 
         This function can be used to avoid key collisions in an ensemble
@@ -1139,15 +1156,15 @@
 
         :param use_prefix: If set to true, all future operations
                            on models and scripts will use a prefix, if
                            available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
-        return super().use_model_ensemble_prefix(use_prefix)
+        return self._client.use_model_ensemble_prefix(use_prefix)
 
     @exception_handler
     def use_list_ensemble_prefix(self, use_prefix):
         """Control whether aggregation lists are prefixed
            when forming database keys
 
         This function can be used to avoid key collisions in an
@@ -1156,50 +1173,71 @@
         aggregation list names.  Prefixes will only be used if
         they were previously set through the environment variables
         SSKEYOUT and SSKEYIN. Keys for aggregation lists created
         before this function is called will not be retroactively
         prefixed. By default, the client prefixes aggregation
         list keys with the first prefix specified with the SSKEYIN
         and SSKEYOUT environment variables.  Note that
-        use_tensor_ensemble_prefix() controls prefixing
+        use_dataset_ensemble_prefix() controls prefixing
         for the entities in the aggregation list, and
-        use_tensor_ensemble_prefix() should be given the
+        use_dataset_ensemble_prefix() should be given the
         same value that was used during the initial
         setting of the DataSet into the database.
 
         :param use_prefix: If set to true, all future operations
                            on aggregation lists will use a prefix, if
                            available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
-        return super().use_list_ensemble_prefix(use_prefix)
+        return self._client.use_list_ensemble_prefix(use_prefix)
 
     @exception_handler
     def use_tensor_ensemble_prefix(self, use_prefix):
-        """Control whether tensor and dataset keys are
-           prefixed (e.g. in an ensemble) when forming database keys
+        """Control whether tensor keys are prefixed (e.g. in an
+        ensemble) when forming database keys
 
         This function can be used to avoid key collisions in an ensemble
         by prepending the string value from the environment variable SSKEYIN
-        to tensor and dataset names.
+        to tensor names.
         Prefixes will only be used if they were previously set through
         environment variables SSKEYIN and SSKEYOUT.
         Keys for entities created before this function is called
         will not be retroactively prefixed.
-        By default, the client prefixes tensor and dataset
-        keys when a prefix is available.
+        By default, the client prefixes tensor keys when a prefix is
+        available.
 
-        :param use_prefix: If set to true, all future operations
-                           on tensors and datasets will use a prefix, if
-                           available.
+        :param use_prefix: If set to true, all future operations on tensors
+                           will use a prefix, if available.
+        :type use_prefix: bool
+        """
+        typecheck(use_prefix, "use_prefix", bool)
+        return self._client.use_tensor_ensemble_prefix(use_prefix)
+
+    @exception_handler
+    def use_dataset_ensemble_prefix(self, use_prefix):
+        """Control whether dataset keys are prefixed (e.g. in an ensemble)
+           when forming database keys
+
+        This function can be used to avoid key collisions in an ensemble
+        by prepending the string value from the environment variable SSKEYIN
+        to dataset names.
+        Prefixes will only be used if they were previously set through
+        environment variables SSKEYIN and SSKEYOUT.
+        Keys for entities created before this function is called
+        will not be retroactively prefixed.
+        By default, the client prefixes dataset keys when a prefix is
+        available.
+
+        :param use_prefix: If set to true, all future operations on datasets
+                           will use a prefix, if available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
-        return super().use_tensor_ensemble_prefix(use_prefix)
+        return self._client.use_dataset_ensemble_prefix(use_prefix)
 
     @exception_handler
     def get_db_node_info(self, addresses):
         """Returns information about given database nodes
 
         :param addresses: The addresses of the database nodes
         :type address: list[str]
@@ -1214,15 +1252,15 @@
                 to a specific address to avoid inconsistencies in
                 addresses retrieved with the CLUSTER SLOTS command.
                 Inconsistencies in node addresses across
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
-        return super().get_db_node_info(addresses)
+        return self._client.get_db_node_info(addresses)
 
     @exception_handler
     def get_db_cluster_info(self, addresses):
         """Returns cluster information from a specified db node.
         If the address does not correspond to a cluster node,
         an empty dictionary is returned.
 
@@ -1240,15 +1278,15 @@
                 to a specific address to avoid inconsistencies in
                 addresses retrieved with the CLUSTER SLOTS command.
                 Inconsistencies in node addresses across
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
-        return super().get_db_cluster_info(addresses)
+        return self._client.get_db_cluster_info(addresses)
 
     @exception_handler
     def get_ai_info(self, address, key, reset_stat=False):
         """Returns AI.INFO command reply information for the
         script or model key at the provided addresses.
 
         :param addresses: The addresses of the database nodes
@@ -1264,15 +1302,15 @@
         :rtype: list[dict]
         :raises RedisReplyError: if there is an error
                 in command execution or parsing the command reply.
         """
         typecheck(address, "address", list)
         typecheck(key, "key", str)
         typecheck(reset_stat, "reset_stat", bool)
-        return super().get_ai_info(address, key, reset_stat)
+        return self._client.get_ai_info(address, key, reset_stat)
 
     @exception_handler
     def flush_db(self, addresses):
         """Removes all keys from a specified db node.
 
         :param addresses: The addresses of the database nodes
         :type address: list[str]
@@ -1284,15 +1322,15 @@
                 to a specific address to avoid inconsistencies in
                 addresses retrieved with the CLUSTER SLOTS command.
                 Inconsistencies in node addresses across
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
-        super().flush_db(addresses)
+        self._client.flush_db(addresses)
 
     @exception_handler
     def config_get(self, expression, address):
         """Read the configuration parameters of a running server.
         If the address does not correspond to a cluster node,
         an empty dictionary is returned.
 
@@ -1315,15 +1353,15 @@
                 addresses retrieved with the CLUSTER SLOTS command.
                 Inconsistencies in node addresses across
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(expression, "expression", str)
         typecheck(address, "address", str)
-        return super().config_get(expression, address)
+        return self._client.config_get(expression, address)
 
     @exception_handler
     def config_set(self, config_param, value, address):
         """Reconfigure the server. It can change both trivial
         parameters or switch from one to another persistence option.
         All the configuration parameters set using this command are
         immediately loaded by Redis and will take effect starting with
@@ -1347,15 +1385,15 @@
                 Inconsistencies in node addresses across
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(config_param, "config_param", str)
         typecheck(value, "value", str)
         typecheck(address, "address", str)
-        super().config_set(config_param, value, address)
+        self._client.config_set(config_param, value, address)
 
     @exception_handler
     def save(self, addresses):
         """Performs a synchronous save of the database shard
         producing a point in time snapshot of all the data
         inside the Redis instance, in the form of an RBD file.
 
@@ -1369,15 +1407,15 @@
                 to a specific address to avoid inconsistencies in
                 addresses retrieved with the CLUSTER SLOTS command.
                 Inconsistencies in node addresses across
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
-        super().save(addresses)
+        self._client.save(addresses)
 
     @exception_handler
     def append_to_list(self, list_name, dataset):
         """Appends a dataset to the aggregation list
 
         When appending a dataset to an aggregation list,
         the list will automatically be created if it does not
@@ -1396,15 +1434,15 @@
         :raises TypeError: if argument is not a Dataset
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(list_name, "list_name", str)
         typecheck(dataset, "dataset", Dataset)
         pybind_dataset = dataset.get_data()
-        super().append_to_list(list_name, pybind_dataset)
+        self._client.append_to_list(list_name, pybind_dataset)
 
     @exception_handler
     def delete_list(self, list_name):
         """Delete an aggregation list
 
         The key used to locate the aggregation list to be
         deleted may be formed by applying a prefix to the
@@ -1413,185 +1451,185 @@
 
         :param list_name: The name of the aggregation list
         :type list_name: str
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(list_name, "list_name", str)
-        super().delete_list(list_name)
+        self._client.delete_list(list_name)
 
     @exception_handler
     def copy_list(self, src_name, dest_name):
         """Copy an aggregation list
 
         The source and destination aggregation list keys used to
         locate and store the aggregation list may be formed by
         applying prefixes to the supplied src_name and dest_name.
         See set_data_source() and use_list_ensemble_prefix()
         for more details.
 
-        :param  src_name The source list name
+        :param src_name: The source list name
         :type src_name: str
-        :param  dest_name The destination list name
+        :param dest_name: The destination list name
         :type dest_name: str
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
-        super().copy_list(src_name, dest_name)
+        self._client.copy_list(src_name, dest_name)
 
     @exception_handler
     def rename_list(self, src_name, dest_name):
         """Rename an aggregation list
 
         The old and new aggregation list key used to find and
         relocate the list may be formed by applying prefixes to
         the supplied old_name and new_name. See set_data_source()
         and use_list_ensemble_prefix() for more details.
 
-        :param  src_name The source list name
+        :param src_name: The source list name
         :type src_name: str
-        :param  dest_name The destination list name
+        :param dest_name: The destination list name
         :type dest_name: str
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
-        super().rename_list(src_name, dest_name)
+        self._client.rename_list(src_name, dest_name)
 
     @exception_handler
     def get_list_length(self, list_name):
         """Get the number of entries in the list
 
-        :param  list_name The list name
+        :param list_name: The list name
         :type list_name: str
         :return: The length of the list
         :rtype: int
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(list_name, "list_name", str)
-        return super().get_list_length(list_name)
+        return self._client.get_list_length(list_name)
 
     @exception_handler
     def poll_list_length(self, name, list_length, poll_frequency_ms, num_tries):
         """Poll list length until length is equal
         to the provided length.  If maximum number of
         attempts is exceeded, returns False
 
         The aggregation list key used to check for list length
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
         for more details.
 
-        :param  name The name of the list
+        :param name: The name of the list
         :type name: str
-        :param  list_length The desired length of the list
+        :param list_length: The desired length of the list
         :type list_length: int
-        :param  poll_frequency_ms The time delay between checks, in milliseconds
+        :param poll_frequency_ms: The time delay between checks, in milliseconds
         :type poll_frequency_ms: int
-        :param  num_tries The total number of times to check for the name
+        :param num_tries: The total number of times to check for the name
         :type num_tries: int
-        :return:  Returns true if the list is found with a length greater
-                  than or equal to the provided length, otherwise false
+        :return: Returns true if the list is found with a length greater
+                than or equal to the provided length, otherwise false
         :rtype: bool
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(name, "name", str)
         typecheck(list_length, "list_length", int)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_list_length(
+        return self._client.poll_list_length(
             name, list_length, poll_frequency_ms, num_tries)
 
     @exception_handler
     def poll_list_length_gte(self, name, list_length, poll_frequency_ms, num_tries):
         """Poll list length until length is greater than or equal
         to the user-provided length. If maximum number of
         attempts is exceeded, false is returned.
 
         The aggregation list key used to check for list length
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
         for more details.
 
-        :param  name The name of the list
+        :param name: The name of the list
         :type name: str
-        :param  list_length The desired minimum length of the list
+        :param list_length: The desired minimum length of the list
         :type list_length: int
-        :param  poll_frequency_ms The time delay between checks, in milliseconds
+        :param poll_frequency_ms: The time delay between checks, in milliseconds
         :type poll_frequency_ms: int
-        :param  num_tries The total number of times to check for the name
+        :param num_tries: The total number of times to check for the name
         :type num_tries: int
-        :return:  Returns true if the list is found with a length greater
-                  than or equal to the provided length, otherwise false
+        :return: Returns true if the list is found with a length greater
+                 than or equal to the provided length, otherwise false
         :rtype: bool
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(name, "name", str)
         typecheck(list_length, "list_length", int)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_list_length_gte(
+        return self._client.poll_list_length_gte(
             name, list_length, poll_frequency_ms, num_tries)
 
     @exception_handler
     def poll_list_length_lte(self, name, list_length, poll_frequency_ms, num_tries):
         """Poll list length until length is less than or equal
         to the user-provided length. If maximum number of
         attempts is exceeded, false is returned.
 
         The aggregation list key used to check for list length
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
         for more details.
 
-        :param  name The name of the list
+        :param name: The name of the list
         :type name: str
-        :param  list_length The desired maximum length of the list
+        :param list_length: The desired maximum length of the list
         :type list_length: int
-        :param  poll_frequency_ms The time delay between checks, in milliseconds
+        :param poll_frequency_ms: The time delay between checks, in milliseconds
         :type poll_frequency_ms: int
-        :param  num_tries The total number of times to check for the name
+        :param num_tries: The total number of times to check for the name
         :type num_tries: int
-        :return:  Returns true if the list is found with a length less
-                  than or equal to the provided length, otherwise false
+        :return: Returns true if the list is found with a length less
+                 than or equal to the provided length, otherwise false
         :rtype: bool
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(name, "name", str)
         typecheck(list_length, "list_length", int)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
-        return super().poll_list_length_lte(
+        return self._client.poll_list_length_lte(
             name, list_length, poll_frequency_ms, num_tries)
 
     @exception_handler
     def get_datasets_from_list(self, list_name):
         """Get datasets from an aggregation list
 
         The aggregation list key used to retrieve datasets
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
         for more details.  An empty or nonexistant
         aggregation list returns an empty vector.
 
-        :param  list_name The name of the list
+        :param list_name: The name of the list
         :type list_name: str
-        :return:  A list of DataSet objects.
+        :return: A list of DataSet objects.
         :rtype: list[DataSet]
         :raises RedisReplyError: if there is an error in command execution.
         """
         typecheck(list_name, "list_name", str)
-        return super().get_datasets_from_list(list_name)
+        return self._client.get_datasets_from_list(list_name)
 
     @exception_handler
     def get_dataset_list_range(self, list_name, start_index, end_index):
         """Get a range of datasets (by index) from an aggregation list
 
         The aggregation list key used to retrieve datasets
         may be formed by applying a prefix to the supplied
@@ -1599,35 +1637,35 @@
         for more details.  An empty or nonexistant aggregation
         list returns an empty vector.  If the provided
         end_index is beyond the end of the list, that index will
         be treated as the last index of the list.  If start_index
         and end_index are inconsistent (e.g. end_index is less
         than start_index), an empty list of datasets will be returned.
 
-        :param  list_name The name of the list
+        :param list_name: The name of the list
         :type list_name: str
-        :param  start_index The starting index of the range (inclusive,
-                starting at zero).  Negative values are
-                supported.  A negative value indicates offsets
-                starting at the end of the list. For example, -1 is
-                the last element of the list.
+        :param start_index: The starting index of the range (inclusive,
+               starting at zero).  Negative values are
+               supported.  A negative value indicates offsets
+               starting at the end of the list. For example, -1 is
+               the last element of the list.
         :type start_index: int
-        :param end_index The ending index of the range (inclusive,
+        :param end_index: The ending index of the range (inclusive,
                starting at zero).  Negative values are
                supported.  A negative value indicates offsets
                starting at the end of the list. For example, -1 is
                the last element of the list.
-        :return:  A list of DataSet objects.
+        :return: A list of DataSet objects.
         :rtype: list[DataSet]
         :raises RedisReplyError: if there is an error in command execution.
         """
         typecheck(list_name, "list_name", str)
         typecheck(start_index, "start_index", int)
         typecheck(end_index, "end_index", int)
-        return super().get_dataset_list_range(
+        return self._client.get_dataset_list_range(
             list_name, start_index, end_index)
 
     # ---- helpers --------------------------------------------------------
 
     @staticmethod
     def __check_tensor_args(inputs, outputs):
         inputs = init_default([], inputs, (list, str))
```

### Comparing `smartredis-0.3.1/src/python/module/smartredis/dataset.py` & `smartredis-0.4.0/src/python/module/smartredis/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -25,27 +25,42 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from numbers import Number
 
 import numpy as np
 
 from .smartredisPy import PyDataset
+from .srobject import SRObject
 from .util import Dtypes, exception_handler, typecheck
 
 from .error import *
 
-class Dataset:
+class Dataset(SRObject):
     def __init__(self, name):
         """Initialize a Dataset object
 
         :param name: name of dataset
         :type name: str
         """
+        super().__init__(PyDataset(name))
         typecheck(name, "name", str)
-        self._data = PyDataset(name)
+
+    def __str__(self):
+        """Create a string representation of the client
+
+        :return: A string representation of the client
+        :rtype: str
+        """
+        return self._data.to_string()
+
+    @property
+    def _data(self):
+        """Alias _srobject to _data
+        """
+        return self._srobject
 
     @staticmethod
     def from_pybind(dataset):
         """Initialize a Dataset object from
         a PyDataset object
 
         :param dataset: The pybind PyDataset object
@@ -74,15 +89,15 @@
     def set_data(self, dataset):
         """Set the PyDataset attribute
 
         :param dataset: The PyDataset object
         :type dataset: PyDataset
         """
         typecheck(dataset, "dataset", PyDataset)
-        self._data = dataset
+        self._srobject = dataset
 
     @exception_handler
     def add_tensor(self, name, data):
         """Add a named tensor to this dataset
 
         :param name: tensor name
         :type name: str
@@ -165,7 +180,62 @@
 
         :param name: The name used to reference the metadata
                         field in the DataSet
         :type name: str
         """
         typecheck(name, "name", str)
         return self._data.get_meta_strings(name)
+
+    @exception_handler
+    def get_metadata_field_names(self):
+        """Get the names of all metadata scalars and strings from the DataSet
+
+        :return: a list of metadata field names
+        :rtype: list[str]
+        """
+        return self._data.get_metadata_field_names()
+
+    @exception_handler
+    def get_metadata_field_type(self, name):
+        """Get the names of all metadata scalars and strings from the DataSet
+
+        :param name: The name used to reference the metadata
+                     field in the DataSet
+        :type name: str
+        :return: the numpy type for the metadata field
+        :rtype: type
+        """
+        typecheck(name, "name", str)
+        type_str = self._data.get_metadata_field_type(name)
+        return Dtypes.from_string(type_str)
+
+    @exception_handler
+    def get_tensor_type(self, name):
+        """Get the type of a tensor in the DataSet
+
+        :param name: The name used to reference the tensor in the DataSet
+        :type name: str
+        :return: the numpy type for the tensor
+        :rtype: type
+        """
+        typecheck(name, "name", str)
+        type_str = self._data.get_tensor_type(name)
+        return Dtypes.from_string(type_str)
+
+    @exception_handler
+    def get_tensor_names(self):
+        """Get the names of all tensors in the DataSet
+
+        :return: a list of tensor names
+        :rtype: list[str]
+        """
+        return self._data.get_tensor_names()
+
+    @exception_handler
+    def get_tensor_dims(self, name):
+        """Get the dimensions of a tensor in the DataSet
+
+        :return: a list of the tensor dimensions
+        :rtype: list[int]
+        """
+        typecheck(name, "name", str)
+        return self._data.get_tensor_dims(name)
```

### Comparing `smartredis-0.3.1/src/python/module/smartredis/error.py` & `smartredis-0.4.0/src/python/module/smartredis/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/src/python/module/smartredis/util.py` & `smartredis-0.4.0/src/python/module/smartredis/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -23,14 +23,17 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .error import *
 from functools import wraps
 from .smartredisPy import RedisReplyError as PybindRedisReplyError
+from .smartredisPy import c_get_last_error_location
+import numpy as np
+
 class Dtypes:
     @staticmethod
     def tensor_from_numpy(array):
         mapping = {
             "float64": "DOUBLE",
             "float32": "FLOAT",
             "uint8": "UINT8",
@@ -56,14 +59,32 @@
             "int64": "INT64",
         }
         dtype = str(array.dtype)
         if dtype in mapping:
             return mapping[dtype]
         raise TypeError(f"Incompatible metadata type provided {dtype}")
 
+    @staticmethod
+    def from_string(type_name):
+        mapping = {
+            "DOUBLE": np.double,
+            "FLOAT":  np.float64,
+            "UINT8":  np.uint8,
+            "UINT16": np.uint16,
+            "UINT32": np.uint32,
+            "UINT64": np.uint64,
+            "INT8":   np.int8,
+            "INT16":  np.int16,
+            "INT32":  np.int32,
+            "INT64":  np.int64,
+            "STRING": str,
+        }
+        if type_name in mapping:
+            return mapping[type_name]
+        raise TypeError(f"Unrecognized type name {type_name}")
 
 def init_default(default, init_value, expected_type=None):
     """Used for setting a mutable type to a default value.
 
     PEP standards forbid setting a default value to a mutable type
     Use this function to get around that.
     """
@@ -91,23 +112,28 @@
         except PybindRedisReplyError as cpp_error:
             # query args[0] (i.e. 'self') for the class name
             method_name = args[0].__class__.__name__ + "." + func.__name__
             # Get our exception from the global symbol table.
             # The smartredis.error hierarchy exactly
             # parallels the one built via pybind to enable this
             exception_name = cpp_error.__class__.__name__
-            raise globals()[exception_name](str(cpp_error), method_name) from None
+            error_loc = c_get_last_error_location()
+            if error_loc == "unavailable":
+                cpp_error_str = str(cpp_error)
+            else:
+                cpp_error_str = f"File {error_loc}, in SmartRedis library\n{str(cpp_error)}"
+            raise globals()[exception_name](cpp_error_str, method_name) from None
     return smartredis_api_wrapper
 
 def typecheck(arg, name, _type):
     """Validate that an argument is of a given type
 
     :param arg: the variable to be type tested
     :type arg: variable, expected to match _type
     :param name: the name of the variable
     :type name: str
     :param _type: the expected type for the variable
     :type _type: a Python type
     :raises TypeError exception if arg is not of type _type
     """
     if not isinstance(arg, _type):
-        raise TypeError(f"Argument {name} is of type {type(arg)}, not {_type}")
+        raise TypeError(f"Argument {name} is of type {type(arg)}, not {_type}")
```

### Comparing `smartredis-0.3.1/src/python/module/smartredis.egg-info/PKG-INFO` & `smartredis-0.4.0/src/python/module/smartredis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartredis
-Version: 0.3.1
+Version: 0.4.0
 Summary: RedisAI clients for SmartSim
 Home-page: https://github.com/CrayLabs/SmartRedis
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartRedis
 Project-URL: Documentation, https://www.craylabs.org
@@ -106,11 +106,12 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: xarray
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartredis Version: 0.3.1 Summary: RedisAI clients
+Metadata-Version: 2.1 Name: smartredis Version: 0.4.0 Summary: RedisAI clients
 for SmartSim Home-page: https://github.com/CrayLabs/SmartRedis Author:
 CrayLabs, a Hewlett Packard Enterprise OSS Organization Author-email:
 craylabs@hpe.com License: BSD 2-Clause License Project-URL: Source, https://
 github.com/CrayLabs/SmartRedis Project-URL: Documentation, https://
 www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
@@ -54,9 +54,9 @@
 Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins}, year=
 {2021}, eprint={2104.09355}, archivePrefix={arXiv}, primaryClass={cs.CE} } ```
 Keywords: redis,clients,hpc,ai,deep learning Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: BSD License Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
-Extra: doc
+<3.11,>=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
+Provides-Extra: doc Provides-Extra: xarray
```

### Comparing `smartredis-0.3.1/src/python/module/smartredis.egg-info/SOURCES.txt` & `smartredis-0.4.0/src/python/module/smartredis.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,129 +11,156 @@
 build-scripts/build-catch.sh
 build-scripts/build-keydb.sh
 build-scripts/build-lcov.sh
 build-scripts/build-redis.sh
 build-scripts/build-redisai-cpu.sh
 build-scripts/build-redisai-gpu.sh
 build-scripts/build_c_tests.sh
-build-scripts/build_cpp_cov.sh
 build-scripts/build_cpp_tests.sh
 build-scripts/build_cpp_unit_tests.sh
 build-scripts/build_deps.sh
 build-scripts/build_fortran_tests.sh
 build-scripts/build_lib.sh
 build-scripts/build_parallel_examples.sh
 build-scripts/build_serial_examples.sh
 build-scripts/build_test_deps.sh
+include/address.h
 include/addressallcommand.h
 include/addressanycommand.h
 include/addressatcommand.h
 include/c_client.h
 include/c_dataset.h
+include/c_logcontext.h
+include/c_logger.h
 include/client.h
 include/clusterinfocommand.h
 include/command.h
 include/command.tcc
 include/commandlist.h
 include/commandlist.tcc
 include/commandreply.h
 include/compoundcommand.h
 include/dataset.h
 include/dbinfocommand.h
 include/dbnode.h
 include/enum_fortran.inc
 include/gettensorcommand.h
 include/keyedcommand.h
+include/logcontext.h
+include/logger.h
 include/metadata.h
 include/metadatabuffer.h
 include/metadatafield.h
 include/multikeycommand.h
 include/nonkeyedcommand.h
 include/pipelinereply.h
 include/pyclient.h
 include/pydataset.h
+include/pylogcontext.h
+include/pysrobject.h
 include/redis.h
 include/rediscluster.h
 include/redisserver.h
 include/scalarfield.h
 include/scalarfield.tcc
 include/sharedmemorylist.h
 include/sharedmemorylist.tcc
 include/singlekeycommand.h
 include/sr_enums.h
 include/srassert.h
 include/srexception.h
+include/srobject.h
 include/stringfield.h
 include/tensor.h
 include/tensor.tcc
 include/tensorbase.h
 include/tensorpack.h
 include/threadpool.h
+include/utility.h
 src/c/c_client.cpp
 src/c/c_dataset.cpp
 src/c/c_error.cpp
+src/c/c_logcontext.cpp
+src/c/c_logger.cpp
+src/cpp/address.cpp
 src/cpp/addressallcommand.cpp
 src/cpp/addressanycommand.cpp
 src/cpp/addressatcommand.cpp
 src/cpp/client.cpp
 src/cpp/clusterinfocommand.cpp
 src/cpp/command.cpp
 src/cpp/commandlist.cpp
 src/cpp/commandreply.cpp
 src/cpp/compoundcommand.cpp
 src/cpp/dataset.cpp
 src/cpp/dbinfocommand.cpp
 src/cpp/dbnode.cpp
 src/cpp/gettensorcommand.cpp
 src/cpp/keyedcommand.cpp
+src/cpp/logger.cpp
 src/cpp/metadata.cpp
 src/cpp/metadatafield.cpp
 src/cpp/multikeycommand.cpp
 src/cpp/nonkeyedcommand.cpp
 src/cpp/pipelinereply.cpp
 src/cpp/redis.cpp
 src/cpp/rediscluster.cpp
 src/cpp/redisserver.cpp
 src/cpp/singlekeycommand.cpp
+src/cpp/srobject.cpp
 src/cpp/stringfield.cpp
 src/cpp/tensorbase.cpp
 src/cpp/tensorpack.cpp
 src/cpp/threadpool.cpp
+src/cpp/utility.cpp
 src/fortran/client.F90
 src/fortran/dataset.F90
+src/fortran/errors.F90
 src/fortran/fortran_c_interop.F90
+src/fortran/logcontext.F90
+src/fortran/logger.F90
 src/fortran/client/aggregation_interfaces.inc
 src/fortran/client/client_dataset_interfaces.inc
 src/fortran/client/client_interfaces.inc
 src/fortran/client/ensemble_interfaces.inc
 src/fortran/client/misc_tensor_interfaces.inc
 src/fortran/client/model_interfaces.inc
 src/fortran/client/put_tensor_interfaces.inc
 src/fortran/client/put_tensor_methods_common.inc
 src/fortran/client/script_interfaces.inc
 src/fortran/client/unpack_tensor_interfaces.inc
 src/fortran/client/unpack_tensor_methods_common.inc
 src/fortran/dataset/add_meta_scalar_common.inc
-src/fortran/dataset/add_tensor_interfaces.inc
 src/fortran/dataset/add_tensor_methods_common.inc
 src/fortran/dataset/dataset_interfaces.inc
 src/fortran/dataset/get_meta_scalars_common.inc
 src/fortran/dataset/metadata_interfaces.inc
+src/fortran/dataset/tensor_interfaces.inc
 src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
 src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
+src/fortran/errors/errors_interfaces.inc
+src/fortran/logcontext/logcontext_interfaces.inc
+src/fortran/logger/logger_interfaces.inc
 src/python/bindings/bind.cpp
 src/python/module/smartredis/__init__.py
 src/python/module/smartredis/client.py
 src/python/module/smartredis/dataset.py
+src/python/module/smartredis/dataset_utils.py
 src/python/module/smartredis/error.py
+src/python/module/smartredis/logcontext.py
+src/python/module/smartredis/logger.py
+src/python/module/smartredis/srobject.py
 src/python/module/smartredis/util.py
 src/python/module/smartredis.egg-info/PKG-INFO
 src/python/module/smartredis.egg-info/SOURCES.txt
 src/python/module/smartredis.egg-info/dependency_links.txt
 src/python/module/smartredis.egg-info/not-zip-safe
 src/python/module/smartredis.egg-info/requires.txt
 src/python/module/smartredis.egg-info/top_level.txt
 src/python/src/pyclient.cpp
 src/python/src/pydataset.cpp
+src/python/src/pylogcontext.cpp
+src/python/src/pysrobject.cpp
+utils/check_redis.sh
 utils/create_cluster/local_cluster.py
 utils/create_cluster/slurm_cluster.py
 utils/create_cluster/smartredisdb.conf
```

### Comparing `smartredis-0.3.1/utils/create_cluster/local_cluster.py` & `smartredis-0.4.0/utils/create_cluster/local_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/utils/create_cluster/slurm_cluster.py` & `smartredis-0.4.0/utils/create_cluster/slurm_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartredis-0.3.1/utils/create_cluster/smartredisdb.conf` & `smartredis-0.4.0/utils/create_cluster/smartredisdb.conf`

 * *Files identical despite different names*

