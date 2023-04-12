# Comparing `tmp/fast-matrix-market-1.5.0.tar.gz` & `tmp/fast-matrix-market-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-matrix-market-1.5.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "fast-matrix-market-1.5.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `fast-matrix-market-1.5.0.tar` & `fast-matrix-market-1.5.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/CMakeLists.txt
--rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/README.md
--rw-r--r--   0        0        0     6336 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/benchmark/bench_fmm.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/benchmark/requirements.txt
--rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/benchmark/run.sh
--rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/CMakeLists.txt
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/Blaze.cmake
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/Dragonbox.cmake
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/Eigen.cmake
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/GoogleBenchmark.cmake
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/GoogleTest.cmake
--rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/GraphBLAS.cmake
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/fast_float.cmake
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/from_chars_tests.cmake
--rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/cmake/to_chars_tests.cmake
--rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/README.md
--rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
--rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
--rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
--rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
--rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
--rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
--rw-r--r--   0        0        0   118134 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
--rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost
--rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/common.h
--rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
--rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
--rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c
--rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
--rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
--rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
--rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
--rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
--rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
--rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.c
--rw-r--r--   0        0        0    34192 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.h
--rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h
--rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h
--rw-r--r--   0        0        0     8362 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/s2d.c
--rw-r--r--   0        0        0     8591 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/s2f.c
--rw-r--r--   0        0        0    15697 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/3rdparty/BS_thread_pool_light.hpp
--rw-r--r--   0        0        0     3967 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
--rw-r--r--   0        0        0    15486 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
--rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
--rw-r--r--   0        0        0     7152 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
--rw-r--r--   0        0        0    57554 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
--rw-r--r--   0        0        0     4512 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp
--rw-r--r--   0        0        0     4077 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
--rw-r--r--   0        0        0     4111 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
--rw-r--r--   0        0        0     3147 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp
--rw-r--r--   0        0        0     5210 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
--rw-r--r--   0        0        0    21141 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
--rw-r--r--   0        0        0    14705 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp
--rw-r--r--   0        0        0     9849 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/header.hpp
--rw-r--r--   0        0        0     9271 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
--rw-r--r--   0        0        0    17948 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp
--rw-r--r--   0        0        0     5487 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
--rw-r--r--   0        0        0     4977 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/types.hpp
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp
--rw-r--r--   0        0        0     2497 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    16022 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/src/fast_matrix_market/__init__.py
--rw-r--r--   0        0        0    23643 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/src/fast_matrix_market/core.cpp
--rw-r--r--   0        0        0    19432 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/src/fast_matrix_market/pystreambuf.h
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/eye3.mtx
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/long_double/longcomplex_array.mtx
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/long_double/longcomplex_coordinate.mtx
--rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/long_double/longdouble_array.mtx
--rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/long_double/longdouble_coordinate.mtx
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_array_complex_general.mtx
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_array_integer_general.mtx
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_array_real_general.mtx
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_complex_general.mtx
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_complex_hermitian.mtx
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_integer_general.mtx
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_pattern_general.mtx
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_real_general.mtx
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_real_general.mtx.bz2
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_real_general.mtx.gz
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/matrix_coordinate_real_symmetric.mtx
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/misc/windows_newlines.mtx
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/scipy_crashes/vector_array_real_general.mtx
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
--rw-r--r--   0        0        0     1769 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/test_array.py
--rw-r--r--   0        0        0      428 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/test_basic.py
--rw-r--r--   0        0        0     3194 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/test_coo.py
--rw-r--r--   0        0        0     3477 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/test_header.py
--rw-r--r--   0        0        0    13095 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/tests/test_scipy.py
--rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/testsuite_scipy/test_scipy_suite.py
--rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1275 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/README.md
+-rw-r--r--   0        0        0     6336 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/benchmark/bench_fmm.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/benchmark/requirements.txt
+-rwxr-xr-x   0        0        0      742 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/benchmark/run.sh
+-rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/CMakeLists.txt
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/Blaze.cmake
+-rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/Dragonbox.cmake
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/Eigen.cmake
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/GoogleBenchmark.cmake
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/GoogleTest.cmake
+-rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/GraphBLAS.cmake
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/fast_float.cmake
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/from_chars_tests.cmake
+-rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/cmake/to_chars_tests.cmake
+-rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/README.md
+-rw-r--r--   0        0        0     3811 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt
+-rw-r--r--   0        0        0    12262 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/cmake/dragonboxConfig.cmake
+-rw-r--r--   0        0        0   144785 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h
+-rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h
+-rw-r--r--   0        0        0    25425 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/CMakeLists.txt
+-rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-MIT
+-rw-r--r--   0        0        0   118134 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h
+-rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Apache2
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Boost
+-rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/common.h
+-rw-r--r--   0        0        0    26321 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c
+-rw-r--r--   0        0        0   329074 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h
+-rw-r--r--   0        0        0    17721 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s.c
+-rw-r--r--   0        0        0    34501 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h
+-rw-r--r--   0        0        0    13015 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h
+-rw-r--r--   0        0        0     7434 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h
+-rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/digit_table.h
+-rw-r--r--   0        0        0    11279 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s.c
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h
+-rw-r--r--   0        0        0     4294 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h
+-rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.c
+-rw-r--r--   0        0        0    34192 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.h
+-rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu.h
+-rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h
+-rw-r--r--   0        0        0     8362 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2d.c
+-rw-r--r--   0        0        0     8591 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2f.c
+-rw-r--r--   0        0        0    15697 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/3rdparty/BS_thread_pool_light.hpp
+-rw-r--r--   0        0        0     3967 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp
+-rw-r--r--   0        0        0    15486 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp
+-rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp
+-rw-r--r--   0        0        0     7152 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp
+-rw-r--r--   0        0        0    57554 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp
+-rw-r--r--   0        0        0     4512 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/array.hpp
+-rw-r--r--   0        0        0     4077 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp
+-rw-r--r--   0        0        0     4111 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp
+-rw-r--r--   0        0        0     3147 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/chunking.hpp
+-rw-r--r--   0        0        0     5210 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp
+-rw-r--r--   0        0        0    21141 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/field_conv.hpp
+-rw-r--r--   0        0        0    14705 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/formatters.hpp
+-rw-r--r--   0        0        0    10063 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/header.hpp
+-rw-r--r--   0        0        0     9271 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp
+-rw-r--r--   0        0        0    18534 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body.hpp
+-rw-r--r--   0        0        0     5487 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp
+-rw-r--r--   0        0        0     4977 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/types.hpp
+-rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body.hpp
+-rw-r--r--   0        0        0     2497 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    16022 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/src/fast_matrix_market/__init__.py
+-rw-r--r--   0        0        0    23643 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/src/fast_matrix_market/core.cpp
+-rw-r--r--   0        0        0    19432 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/src/fast_matrix_market/pystreambuf.h
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/eye3.mtx
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longcomplex_array.mtx
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longcomplex_coordinate.mtx
+-rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longdouble_array.mtx
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/long_double/longdouble_coordinate.mtx
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_array_complex_general.mtx
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_array_integer_general.mtx
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_array_real_general.mtx
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_complex_general.mtx
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_complex_hermitian.mtx
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_integer_general.mtx
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_pattern_general.mtx
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_pattern_symmetric.mtx
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_general.mtx
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_general.mtx.bz2
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_general.mtx.gz
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_skew-symmetric.mtx
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/matrix_coordinate_real_symmetric.mtx
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/misc/windows_newlines.mtx
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/scipy_crashes/dim_over_32_bit.mtx
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/scipy_crashes/vector_array_real_general.mtx
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/matrices/scipy_crashes/vector_coordinate_real_general.mtx
+-rw-r--r--   0        0        0     1769 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_array.py
+-rw-r--r--   0        0        0      428 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_basic.py
+-rw-r--r--   0        0        0     3194 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_coo.py
+-rw-r--r--   0        0        0     3477 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_header.py
+-rw-r--r--   0        0        0    13095 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/tests/test_scipy.py
+-rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/testsuite_scipy/test_scipy_suite.py
+-rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 fast-matrix-market-1.5.1/PKG-INFO
```

### Comparing `fast-matrix-market-1.5.0/CMakeLists.txt` & `fast-matrix-market-1.5.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/LICENSE.txt` & `fast-matrix-market-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/README.md` & `fast-matrix-market-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/benchmark/bench_fmm.py` & `fast-matrix-market-1.5.1/benchmark/bench_fmm.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/benchmark/run.sh` & `fast-matrix-market-1.5.1/benchmark/run.sh`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/CMakeLists.txt` & `fast-matrix-market-1.5.1/fast_matrix_market/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/cmake/GraphBLAS.cmake` & `fast-matrix-market-1.5.1/fast_matrix_market/cmake/GraphBLAS.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/cmake/from_chars_tests.cmake` & `fast-matrix-market-1.5.1/fast_matrix_market/cmake/from_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/cmake/to_chars_tests.cmake` & `fast-matrix-market-1.5.1/fast_matrix_market/cmake/to_chars_tests.cmake`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/README.md` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/README.md`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Apache2-LLVM`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/include/dragonbox/dragonbox_to_chars.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/dragonbox/source/dragonbox_to_chars.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/CMakeLists.txt` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/LICENSE-MIT` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/fast_float/include/fast_float/fast_float.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/CMakeLists.txt` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/LICENSE-Apache2` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Apache2`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/LICENSE-Boost` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/LICENSE-Boost`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/common.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/common.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2fixed_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s.c` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/d2s_small_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/digit_table.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/digit_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/f2s.c` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_full_table.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/f2s_intrinsics.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.c` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/generic_128.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/generic_128.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/ryu.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_generic_128.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/ryu_parse.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/s2d.c` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2d.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/dependencies/ryu/ryu/s2f.c` & `fast-matrix-market-1.5.1/fast_matrix_market/dependencies/ryu/ryu/s2f.c`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/3rdparty/BS_thread_pool_light.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/3rdparty/BS_thread_pool_light.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Armadillo.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Blaze.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/CXSparse.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/Eigen.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/GraphBLAS.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/array.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/array.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/doublet.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/app/triplet.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/chunking.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/chunking.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/fast_matrix_market.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 namespace fast_matrix_market {
 
     // Version macros.
     // Keep in sync with python/pyproject.toml
 #define FAST_MATRIX_MARKET_VERSION_MAJOR 1
 #define FAST_MATRIX_MARKET_VERSION_MINOR 5
-#define FAST_MATRIX_MARKET_VERSION_PATCH 0
+#define FAST_MATRIX_MARKET_VERSION_PATCH 1
 
     constexpr std::string_view kSpace = " ";
     constexpr std::string_view kNewline = "\n";
 
     template<class T> struct is_complex : std::false_type {};
     template<class T> struct is_complex<std::complex<T>> : std::true_type {};
```

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/field_conv.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/field_conv.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/formatters.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/formatters.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/header.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/header.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -153,25 +153,28 @@
         int64_t lines_read = 0;
         std::string line;
 
         // read banner
         std::getline(instream, line);
         lines_read++;
 
-        if (line.rfind(kMatrixMarketBanner, 0) != 0
-            && line.rfind(kMatrixMarketBanner2, 0) != 0) {
+        if (line.find("MatrixMarket", 0) == std::string::npos) {
             // not a matrix market file because the banner is missing
             throw invalid_mm("Not a Matrix Market file. Missing banner.", lines_read);
         }
 
         // parse banner
         {
             std::istringstream iss(line);
             std::string banner, f_object, f_format, f_field, f_symmetry;
             iss >> banner >> f_object >> f_format >> f_field >> f_symmetry;
+            if (banner != kMatrixMarketBanner && banner != kMatrixMarketBanner2) {
+                // not a matrix market file because the banner is wrong
+                throw invalid_mm("Not a Matrix Market file. Missing banner.", lines_read);
+            }
 
             header.object = parse_header_enum(f_object, object_map, lines_read);
             header.format = parse_header_enum(f_format, format_map, lines_read);
             header.field = parse_header_enum(f_field, field_map, lines_read);
             header.symmetry = parse_header_enum(f_symmetry, symmetry_map, lines_read);
         }
```

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/parse_handlers.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/read_body.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -129,15 +129,19 @@
                 if (header.symmetry != general && options.generalize_symmetry) {
                     if (col != row) {
                         switch (header.symmetry) {
                             case symmetric:
                                 handler.handle(col - 1, row - 1, value);
                                 break;
                             case skew_symmetric:
-                                handler.handle(col - 1, row - 1, negate(value));
+                                if constexpr (!std::is_unsigned_v<typename HANDLER::value_type>) {
+                                    handler.handle(col - 1, row - 1, negate(value));
+                                } else {
+                                    throw invalid_argument("Cannot load skew-symmetric matrix into unsigned value type.");
+                                }
                                 break;
                             case hermitian:
                                 handler.handle(col - 1, row - 1, complex_conjugate(value));
                                 break;
                             case general: break;
                         }
                     } else {
@@ -247,15 +251,19 @@
 
                 if (row != col && options.generalize_symmetry) {
                     switch (header.symmetry) {
                         case symmetric:
                             handler.handle(col, row, value);
                             break;
                         case skew_symmetric:
-                            handler.handle(col, row, negate(value));
+                            if constexpr (!std::is_unsigned_v<typename HANDLER::value_type>) {
+                                handler.handle(col, row, negate(value));
+                            } else {
+                                throw invalid_argument("Cannot load skew-symmetric matrix into unsigned value type.");
+                            }
                             break;
                         case hermitian:
                             handler.handle(col, row, complex_conjugate(value));
                             break;
                         case general:
                             break;
                     }
```

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/read_body_threads.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/types.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/types.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/write_body.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp` & `fast-matrix-market-1.5.1/fast_matrix_market/include/fast_matrix_market/write_body_threads.hpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/pyproject.toml` & `fast-matrix-market-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "fast_matrix_market"
-version = "1.5.0"
+version = "1.5.1"
 description="Fast and full-featured Matrix Market file I/O"
 readme = "README.md"
 authors = [
     { name = "Adam Lugowski"},
 ]
 requires-python = ">=3.7"
```

### Comparing `fast-matrix-market-1.5.0/src/fast_matrix_market/__init__.py` & `fast-matrix-market-1.5.1/src/fast_matrix_market/__init__.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/src/fast_matrix_market/core.cpp` & `fast-matrix-market-1.5.1/src/fast_matrix_market/core.cpp`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/src/fast_matrix_market/pystreambuf.h` & `fast-matrix-market-1.5.1/src/fast_matrix_market/pystreambuf.h`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/tests/test_array.py` & `fast-matrix-market-1.5.1/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/tests/test_coo.py` & `fast-matrix-market-1.5.1/tests/test_coo.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/tests/test_header.py` & `fast-matrix-market-1.5.1/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/tests/test_scipy.py` & `fast-matrix-market-1.5.1/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/testsuite_scipy/test_scipy_suite.py` & `fast-matrix-market-1.5.1/testsuite_scipy/test_scipy_suite.py`

 * *Files identical despite different names*

### Comparing `fast-matrix-market-1.5.0/PKG-INFO` & `fast-matrix-market-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-matrix-market
-Version: 1.5.0
+Version: 1.5.1
 Summary: Fast and full-featured Matrix Market file I/O
 Home-page: https://github.com/alugowski/fast_matrix_market
 Author: Adam Lugowski
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

