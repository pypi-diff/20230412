# Comparing `tmp/scargo-1.1.0.tar.gz` & `tmp/scargo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.1.0.tar", last modified: Thu Mar 23 18:41:20 2023, max compression
+gzip compressed data, was "scargo-1.2.0.tar", last modified: Wed Apr 12 09:37:03 2023, max compression
```

## Comparing `scargo-1.1.0.tar` & `scargo-1.2.0.tar`

### file list

```diff
@@ -1,95 +1,94 @@
--rw-r--r--   0        0        0     4508 2023-03-23 18:41:15.082148 scargo-1.1.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-03-23 18:41:15.082148 scargo-1.1.0/LICENSE
--rw-r--r--   0        0        0     2445 2023-03-23 18:41:15.082148 scargo-1.1.0/README.md
--rw-r--r--   0        0        0     2599 2023-03-23 18:41:15.206148 scargo-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/__init__.py
--rwxr-xr-x   0        0        0    19839 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     4914 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      914 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/clang_utils.py
--rw-r--r--   0        0        0    12793 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1628 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/build.py
--rw-r--r--   0        0        0    11381 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/check.py
--rw-r--r--   0        0        0     1103 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/clean.py
--rw-r--r--   0        0        0     3658 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/debug.py
--rw-r--r--   0        0        0     3526 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/doc.py
--rw-r--r--   0        0        0     3408 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/docker.py
--rw-r--r--   0        0        0     1170 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/fix.py
--rw-r--r--   0        0        0     3340 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/flash.py
--rw-r--r--   0        0        0     6756 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/gen.py
--rw-r--r--   0        0        0     3286 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/new.py
--rw-r--r--   0        0        0     3561 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/publish.py
--rw-r--r--   0        0        0     1656 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/run.py
--rw-r--r--   0        0        0     3027 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/test.py
--rw-r--r--   0        0        0     3653 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/commands/version.py
--rw-r--r--   0        0        0     6066 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/config.py
--rw-r--r--   0        0        0     2445 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/config_utils.py
--rw-r--r--   0        0        0     2196 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/docker_utils.py
--rw-r--r--   0        0        0      646 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/global_values.py
--rw-r--r--   0        0        0       86 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/__init__.py
--rw-r--r--   0        0        0     1891 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/base_gen.py
--rw-r--r--   0        0        0     1036 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cicd_gen.py
--rw-r--r--   0        0        0      858 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cmake_gen.py
--rw-r--r--   0        0        0     1693 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/conan/conanfiletest.j2
--rw-r--r--   0        0        0     1228 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/conan_gen.py
--rw-r--r--   0        0        0      150 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2415 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-03-23 18:41:15.206148 scargo-1.1.0/scargo/jinja/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/cpp/main.cpp.j2
--rw-r--r--   0        0        0     2336 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/cpp_gen.py
--rw-r--r--   0        0        0      159 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2290 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0     1251 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0      236 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2341 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/devcontainer.json.j2
--rw-r--r--   0        0        0      813 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker/stm32.cfg.j2
--rw-r--r--   0        0        0     2980 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/docker_gen.py
--rw-r--r--   0        0        0     1426 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/env_gen.py
--rwxr-xr-x   0        0        0     5474 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_gen.py
--rw-r--r--   0        0        0       39 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_templates/.clang-format
--rw-r--r--   0        0        0      475 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_templates/CMakeLists.txt
--rw-r--r--   0        0        0     1300 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_templates/class_interface.h.j2
--rw-r--r--   0        0        0     1058 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_templates/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_templates/class_mock.h.j2
--rw-r--r--   0        0        0       86 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_utils/__init__.py
--rw-r--r--   0        0        0     1663 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_utils/cmake_utils.py
--rw-r--r--   0        0        0     2396 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_utils/data_classes.py
--rw-r--r--   0        0        0      339 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/mock_utils/missing_mocks.json
--rw-r--r--   0        0        0     1008 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/readme_gen.py
--rw-r--r--   0        0        0     4832 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1580 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4290 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/README.md.j2
--rw-r--r--   0        0        0      294 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/esp32.cmake.j2
--rw-r--r--   0        0        0      510 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/project.cmake.j2
--rw-r--r--   0        0        0     2194 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/scargo.toml.j2
--rw-r--r--   0        0        0      802 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/stm32.cmake.j2
--rw-r--r--   0        0        0      213 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/templates/x86.cmake.j2
--rw-r--r--   0        0        0       91 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/test_templates/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/test_templates/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1036 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/test_templates/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/test_templates/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/test_templates/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/test_templates/static_mock/static_mock.h
--rw-r--r--   0        0        0     2239 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/tests_gen.py
--rw-r--r--   0        0        0     1680 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/toml_gen.py
--rw-r--r--   0        0        0     6877 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/ut_gen.py
--rw-r--r--   0        0        0       39 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/ut_templates/.clang-format
--rw-r--r--   0        0        0      575 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/ut_templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0      703 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/jinja/ut_templates/ut.cpp.j2
--rw-r--r--   0        0        0     2044 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/logger.py
--rw-r--r--   0        0        0     1331 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-03-23 18:41:15.210148 scargo-1.1.0/scargo/templates/LICENSE
--rw-r--r--   0        0        0      515 2023-03-23 18:41:15.210148 scargo-1.1.0/setup.cfg
--rw-r--r--   0        0        0     5176 1970-01-01 00:00:00.000000 scargo-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-04-12 09:36:58.133182 scargo-1.2.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-04-12 09:36:58.133182 scargo-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2527 2023-04-12 09:36:58.133182 scargo-1.2.0/README.md
+-rw-r--r--   0        0        0     2567 2023-04-12 09:36:58.257181 scargo-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-04-12 09:36:58.257181 scargo-1.2.0/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19839 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     4914 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      914 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12538 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1588 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/build.py
+-rw-r--r--   0        0        0    11335 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/check.py
+-rw-r--r--   0        0        0     1153 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4227 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3417 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3274 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3235 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6711 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/gen.py
+-rw-r--r--   0        0        0     3302 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/new.py
+-rw-r--r--   0        0        0     3352 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/run.py
+-rw-r--r--   0        0        0     3180 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/test.py
+-rw-r--r--   0        0        0     4361 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/version.py
+-rw-r--r--   0        0        0     6458 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/config.py
+-rw-r--r--   0        0        0     2403 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/config_utils.py
+-rw-r--r--   0        0        0     2185 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1669 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0      395 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0      569 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2520 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     5093 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0       86 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_utils/__init__.py
+-rw-r--r--   0        0        0     1663 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_utils/cmake_utils.py
+-rw-r--r--   0        0        0     2396 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_utils/data_classes.py
+-rw-r--r--   0        0        0      454 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4832 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1580 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     1693 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1464 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      150 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2415 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      886 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      159 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2290 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0     1251 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0      236 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2348 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      158 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1000 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      294 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1300 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0     1058 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      510 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2194 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      802 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      703 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      213 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1698 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      579 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     6757 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      640 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/logger.py
+-rw-r--r--   0        0        0     1144 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      515 2023-04-12 09:36:58.261181 scargo-1.2.0/setup.cfg
+-rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 scargo-1.2.0/PKG-INFO
```

### Comparing `scargo-1.1.0/CODE-OF-CONDUCT.md` & `scargo-1.2.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/LICENSE` & `scargo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/README.md` & `scargo-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # Working with scargo
 You can find all information on how to work with scargo on official documentation webpage: https://spyro-soft.github.io/scargo/index.html
 ![Scargo flow gif](https://raw.githubusercontent.com/Spyro-Soft/scargo/develop/docs/source/_static/scargo_flow_docker.gif)
 
 # Project dependencies
 ## Working with docker (recommended)
 - docker
-- docker-compose version 1.29.2
+- docker-compose
 - pip
 - python3
 
 ## Working natively (not recommended, a lot of env setup)
 Base:
 
 - python >= 3.8
@@ -56,7 +56,11 @@
 1) If you create a new project, run `docker-compose run scargo-dev` to run project development image depending on chosen architecture. All dependencies should be already there.
 Run scargo commands as you would do natively.
 
 2) If you create a project with --docker flag (`scargo new <my_proj> --docker ...`) or with any docker flag, by default each scargo command will be triggered in docker.
 
 ## Working natively
 1) Create a project with --no-docker flag (`scargo new <my_proj> --no-docker ...`).
+
+# Contributing
+
+See contributing guide on https://spyro-soft.github.io/scargo/contributing.html
```

### Comparing `scargo-1.1.0/pyproject.toml` & `scargo-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,18 @@
 dynamic = ["version"]
 keywords = ["scargo", "Package manager", "C++"]
 dependencies = [
     "clang==14.0",
     "cmake==3.25.2",
     "coloredlogs==15.0.1",
     "conan==1.59.0",
-    "docker-compose==1.29.2",
     "docker==6.0.1",
     "esptool==4.5.1",
     "jinja2==3.1.2",
-    "libclang==15.0.6.1",
+    "libclang==16.0.0",
     "lizard==1.17.10",
     "pydantic==1.10.6",
     "shellingham==1.5.0.post1",
     "toml==0.10.2",
     "tomlkit==0.11.6",
     "typer==0.7.0",
 ]
```

### Comparing `scargo-1.1.0/scargo/certs/certGen.sh` & `scargo-1.2.0/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/certs/generateAllCertificates.sh` & `scargo-1.2.0/scargo/certs/generateAllCertificates.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.2.0/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/certs/openssl_root_ca.cnf` & `scargo-1.2.0/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/clang_utils.py` & `scargo-1.2.0/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/cli.py` & `scargo-1.2.0/scargo/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 import os
 import sys
 from pathlib import Path
 from typing import List, Optional
 
-from typer import Argument, Context, Option, Typer
+from typer import Argument, Option, Typer
 
 from scargo.commands.build import scargo_build
 from scargo.commands.check import scargo_check
 from scargo.commands.clean import scargo_clean
 from scargo.commands.debug import scargo_debug
 from scargo.commands.doc import scargo_doc
 from scargo.commands.docker import (
@@ -26,15 +26,17 @@
 from scargo.commands.run import scargo_run
 from scargo.commands.test import scargo_test
 from scargo.commands.update import scargo_update
 from scargo.commands.version import scargo_version
 from scargo.config import ScargoTargets, Target
 from scargo.global_values import DESCRIPTION, SCARGO_DEFAULT_CONFIG_FILE
 from scargo.logger import get_logger
-from scargo.path_utils import get_config_file_path, get_project_root
+from scargo.path_utils import get_config_file_path
+
+logger = get_logger()
 
 ###############################################################################
 
 
 cli = Typer(context_settings={"help_option_names": ["-h", "--help"]}, help=DESCRIPTION)
 
 
@@ -144,49 +146,53 @@
 
 docker = Typer(help="Manage the docker environment for the project")
 
 
 @docker.command(
     "build", context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
-def docker_build(ctx: Context, base_dir: Optional[Path] = BASE_DIR_OPTION) -> None:
+def docker_build(
+    docker_opts: List[str] = Argument(None), base_dir: Optional[Path] = BASE_DIR_OPTION
+) -> None:
     """Build docker layers for this project depending on the target"""
     if base_dir:
         os.chdir(base_dir)
-    scargo_docker_build(ctx.args)
+    scargo_docker_build(docker_opts)
 
 
 @docker.command(
     "run", context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
 def docker_run(
-    ctx: Context,
     command: str = Option(
         "bash",
         "-c",
         "--command",
         metavar="COMMAND",
         help="Select command to be used with docker run.",
     ),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
+    docker_opts: List[str] = Argument(None),
 ) -> None:
     """Run project in docker environment"""
     if base_dir:
         os.chdir(base_dir)
-    scargo_docker_run(docker_opts=ctx.args, command=command)
+    scargo_docker_run(docker_opts=docker_opts, command=command)
 
 
 @docker.command(
     "exec", context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
-def docker_exec(ctx: Context, base_dir: Optional[Path] = BASE_DIR_OPTION) -> None:
+def docker_exec(
+    base_dir: Optional[Path] = BASE_DIR_OPTION, docker_opts: List[str] = Argument(None)
+) -> None:
     """Attach to existing docker environment"""
     if base_dir:
         os.chdir(base_dir)
-    scargo_docker_exec(ctx.args)
+    scargo_docker_exec(docker_opts)
 
 
 cli.add_typer(docker, name="docker")
 
 
 ###############################################################################
 
@@ -287,25 +293,23 @@
         False, "--bin", "-b", help="Generate single binary image."
     ),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Manage the auto file generator"""
     if base_dir:
         os.chdir(base_dir)
-    project_profile_path = get_project_root() / "build" / profile
     if (gen_ut is gen_mock is certs is None) and not (file_system or single_bin):
-        logger = get_logger()
         logger.warning(
             "Please add one of the following options to the command:"
             "\n--unit-test\n--mock\n--certs\n--fs\n--bin"
         )
         sys.exit(1)
 
     scargo_gen(
-        project_profile_path,
+        profile,
         gen_ut,
         gen_mock,
         certs,
         certs_mode,
         certs_input,
         certs_passwd,
         file_system,
@@ -347,15 +351,15 @@
         name,
         bin_name,
         lib_name,
         Target.get_target_by_id(target.value),
         create_docker,
         git,
     )
-    scargo_update(Path(SCARGO_DEFAULT_CONFIG_FILE))
+    scargo_update(Path(SCARGO_DEFAULT_CONFIG_FILE).absolute())
 
 
 ###############################################################################
 
 
 @cli.command()
 def publish(
@@ -388,16 +392,15 @@
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Build and run project"""
     if base_dir:
         os.chdir(base_dir)
     if not skip_build:
         scargo_build(profile)
-    project_profile_path = get_project_root() / "build" / profile
-    scargo_run(bin_path, project_profile_path, bin_params)
+    scargo_run(bin_path, profile, bin_params)
 
 
 ###############################################################################
 
 
 @cli.command()
 def test(
@@ -425,15 +428,14 @@
         help="Path to .toml configuration file.",
     ),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Read .toml config file and generate `CMakeLists.txt`."""
     if base_dir:
         os.chdir(base_dir)
-    logger = get_logger()
     if config_file_path is None:
         config_file_path = get_config_file_path(SCARGO_DEFAULT_CONFIG_FILE)
         if not config_file_path:
             logger.error("Config file not found.")
             sys.exit(1)
     scargo_update(config_file_path)
 
@@ -446,12 +448,8 @@
     """Get scargo version"""
     scargo_version()
 
 
 ###############################################################################
 
 if __name__ == "__main__":
-    try:
-        cli()
-    except Exception as e:  # pylint: disable=broad-exception-caught
-        print(f"\nA fatal error occurred: {e}")
-        sys.exit(2)
+    cli()
```

### Comparing `scargo-1.1.0/scargo/commands/build.py` & `scargo-1.2.0/scargo/commands/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from scargo.commands.publish import (
     conan_add_conancenter,
     conan_add_remote,
     conan_clean_remote,
 )
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 
 def scargo_build(profile: str) -> None:
     """
     Build project exec file.
 
     :param str profile: Profile
     :return: None
     """
-    prepare_config()
-    logger = get_logger()
+    config = prepare_config()
 
-    project_dir = get_project_root()
+    project_dir = config.project_root
     if not project_dir:
         logger.error("Current working directory is not part of scargo project.")
         sys.exit(1)
 
     if not Path(project_dir, "CMakeLists.txt").exists():
         logger.error("File `CMakeLists.txt` does not exist.")
         logger.info("Did you run `scargo update`?")
```

### Comparing `scargo-1.1.0/scargo/commands/check.py` & `scargo-1.2.0/scargo/commands/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pathlib import Path
 from typing import Iterable, List, NamedTuple, Sequence, Type
 
 from scargo.clang_utils import get_comment_lines
 from scargo.config import CheckConfig, Config, TodoCheckConfig
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
 
 logger = get_logger()
 
 
 def scargo_check(
     clang_format: bool,
     clang_tidy: bool,
@@ -43,15 +42,15 @@
     :param bool todo: check todo left in code
     :param bool verbose: set verbose
     :return: None
     """
     config = prepare_config()
 
     # Todo, remove chdir and change cwd for checks
-    os.chdir(get_project_root())
+    os.chdir(config.project_root)
 
     checkers: List[Type[CheckerFixer]] = []
     if clang_format:
         checkers.append(ClangFormatChecker)
     if clang_tidy:
         checkers.append(ClangTidyChecker)
     if copy_right:
```

### Comparing `scargo-1.1.0/scargo/commands/clean.py` & `scargo-1.2.0/scargo/commands/clean.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 # #
 
 """Clean project from unnecessary files"""
 import shutil
 from pathlib import Path
 from typing import Optional
 
+from scargo.config_utils import get_scargo_config_or_exit
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 
 def _case_insensitive_find_dir(source_dir: Path, dirname: str) -> Optional[Path]:
     if source_dir and source_dir.exists():
         for child in source_dir.iterdir():
             if child.name.lower() == dirname.lower():
                 return child.absolute()
     return None
 
 
 def scargo_clean() -> None:
     """Clean project dir from unnecessary files"""
-    logger = get_logger()
 
-    project_path = get_project_root()
+    config = get_scargo_config_or_exit()
+    project_path = config.project_root
     test_dir = _case_insensitive_find_dir(project_path, "test")
     source_directories = [project_path, test_dir]
 
     for source_dir in source_directories:
         if source_dir:
             build_dir = _case_insensitive_find_dir(source_dir, "build")
             if build_dir and build_dir.exists():
```

### Comparing `scargo-1.1.0/scargo/commands/debug.py` & `scargo-1.2.0/scargo/commands/debug.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,106 +2,121 @@
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 import subprocess
 import sys
 from pathlib import Path
 from time import sleep
-from typing import Optional
+from typing import List, Optional
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.docker_utils import run_scargo_again_in_docker
 from scargo.logger import get_logger
-from scargo.path_utils import find_program_path, get_project_root
+from scargo.path_utils import find_program_path
+
+logger = get_logger()
 
 
 class _ScargoDebug:
-    SUPPORTED_TARGETS = ["x86", "stm32"]
+    SUPPORTED_TARGETS = ["x86", "stm32", "esp32"]
 
     def __init__(self, config: Config, bin_path: Optional[Path]):
-        self._logger = get_logger()
         self._target = config.project.target
+        self._project_root = config.project_root
 
         if self._target.family not in self.SUPPORTED_TARGETS:
-            self._logger.error("Debugging currently not supported for %s", self._target)
-            self._logger.info(
+            logger.error("Debugging currently not supported for %s", self._target)
+            logger.info(
                 "Scargo currently supports debug for %s", self.SUPPORTED_TARGETS
             )
             sys.exit(1)
 
         bin_name = config.project.bin_name
         bin_path = bin_path or (self._get_bin_path(bin_name) if bin_name else None)
         if not bin_path:
-            self._logger.error("No bin_name in config")
+            logger.error("No bin_name in config")
             sys.exit(1)
         self._bin_path = bin_path
         if not self._bin_path.exists():
-            self._logger.error("Binary %s does not exist", self._bin_path)
-            self._logger.info("Did you run scargo build --profile Debug?")
+            logger.error("Binary %s does not exist", self._bin_path)
+            logger.info("Did you run scargo build --profile Debug?")
             sys.exit(1)
 
         if self._target.family == "stm32":
             stm32_config = config.get_stm32_config()
             self._chip = stm32_config.chip
             if not self._chip:
-                self._logger.error("Chip label not defined in toml.")
-                self._logger.info(
-                    "Define chip under stm32 section and run scargo update."
-                )
+                logger.error("Chip label not defined in toml.")
+                logger.info("Define chip under stm32 section and run scargo update.")
                 sys.exit(1)
 
     def run_debugger(self) -> None:
         if self._target.family == "x86":
             self._debug_x86()
         elif self._target.family == "stm32":
             self._debug_stm32()
+        elif self._target.family == "esp32":
+            self._debug_esp32()
 
     def _debug_x86(self) -> None:
         subprocess.run(["gdb", self._bin_path], check=False)
 
-    def _debug_stm32(self) -> None:
+    def _debug_embedded(self, openocd_args: List[str], gdb_bin: str) -> None:
         openocd_path = find_program_path("openocd")
         if not openocd_path:
-            self._logger.error("Could not find openocd.")
+            logger.error("Could not find openocd.")
             sys.exit(1)
+        openocd_call = [openocd_path] + openocd_args
 
-        chip_script = f"target/{self._chip[:7].lower()}x.cfg"
-        openocd = subprocess.Popen(  # pylint: disable=consider-using-with
-            [
-                openocd_path,
-                "-f",
-                "interface/stlink-v2-1.cfg",
-                "-f",
-                chip_script,
-                "-f",
-                ".devcontainer/stm32.cfg",
-            ]
-        )
+        openocd = subprocess.Popen(openocd_call)  # pylint: disable=consider-using-with
         # Wait for openocd to start
         sleep(1)
         try:
             subprocess.run(
                 [
-                    "gdb-multiarch",
+                    gdb_bin,
                     self._bin_path,
                     "--eval-command=target extended-remote localhost:3333",
                 ],
                 check=True,
             )
         finally:
             openocd.terminate()
 
+    def _debug_stm32(self) -> None:
+        chip_script = f"target/{self._chip[:7].lower()}x.cfg"
+        openocd_args = [
+            "-f",
+            "interface/stlink-v2-1.cfg",
+            "-f",
+            chip_script,
+            "-f",
+            ".devcontainer/stm32.cfg",
+        ]
+        self._debug_embedded(openocd_args, "gdb-multiarch")
+
+    def _debug_esp32(self) -> None:
+        openocd_args = [
+            "-f",
+            "interface/ftdi/esp32_devkitj_v1.cfg",
+            "-f",
+            "board/esp-wroom-32.cfg",
+        ]
+        self._debug_embedded(openocd_args, "xtensa-esp32-elf-gdb")
+
     def _get_bin_path(self, bin_name: str) -> Path:
-        project_path = get_project_root()
-        bin_path = Path(project_path, "build/Debug/bin", bin_name).absolute()
-        if self._target.family == "stm32" and bin_path.suffix != "elf":
+        if self._target.family == "esp32":
+            bin_path = Path(self._project_root, "build/Debug", bin_name).absolute()
+        else:
+            bin_path = Path(self._project_root, "build/Debug/bin", bin_name).absolute()
+        if self._target.family in ("stm32", "esp32") and bin_path.suffix != "elf":
             bin_path = bin_path.with_suffix(".elf")
         return bin_path
 
 
 def scargo_debug(bin_path: Optional[Path]) -> None:
     config = prepare_config(run_in_docker=False)
     if config.project.target.family != "x86":
-        run_scargo_again_in_docker(config.project)
+        run_scargo_again_in_docker(config.project, config.project_root)
     debug = _ScargoDebug(config, bin_path)
     debug.run_debugger()
```

### Comparing `scargo-1.1.0/scargo/commands/doc.py` & `scargo-1.2.0/scargo/commands/doc.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 from pathlib import Path
 
 import typer
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
-from scargo.path_utils import find_program_path, get_project_root
+from scargo.path_utils import find_program_path
+
+logger = get_logger()
 
 
 class _ScargoGenDoc:
     EXCLUDE_LIST = ["build"]
 
     def __init__(self, config: Config, doxygen_path: Path, doc_dir_path: Path):
-        self._logger = get_logger()
         self._config = config
         self._doxygen_path = doxygen_path
         self._doc_dir_path = doc_dir_path
 
     def create_default_doxyfile(self) -> None:
         """Create default doxyfile"""
         subprocess.check_call("doxygen -g", shell=True, cwd=self._doc_dir_path)
 
     def update_doxyfile(self) -> None:
         """Update Doxyfile configuration according specified values"""
         project_name = self._config.project.name
-        project_path = get_project_root()
+        project_path = self._config.project_root
         exclude = " ".join(
             f"{project_path}/{dir}"
             for dir in self.EXCLUDE_LIST + self._config.doc.exclude
         )
 
         doxy_values = {
             "PROJECT_NAME": f'"{project_name}"',
@@ -59,16 +60,14 @@
 
     def generate_doxygen(self) -> None:
         """Generate doxygen according to doxyfile"""
         subprocess.check_call("doxygen", shell=True, cwd=self._doc_dir_path)
 
 
 def _open_doc(doc_dir_path: Path) -> None:
-    logger = get_logger()
-
     html_file_path = doc_dir_path / "html/index.html"
     if html_file_path.exists():
         try:
             typer.launch(str(html_file_path))
         except subprocess.CalledProcessError:
             logger.error("Fail to open documentation")
     else:
@@ -80,23 +79,20 @@
 def scargo_doc(open_doc: bool) -> None:
     """
     Create documentation for project
 
     :param bool open_doc: if true open documentation instead creating it
     :return: None
     """
-    project_path = get_project_root()
-    doc_dir_path = project_path / "build/doc"
+    config = prepare_config()
+    doc_dir_path = config.project_root / "build/doc"
     if open_doc:
         _open_doc(doc_dir_path)
         sys.exit(0)
 
-    config = prepare_config()
-    logger = get_logger()
-
     doxygen_path = find_program_path("doxygen")
     if not doxygen_path:
         logger.error("Doxygen not installed or not in PATH environment variable")
         sys.exit(1)
 
     doc_dir_path.mkdir(parents=True, exist_ok=True)
```

### Comparing `scargo-1.1.0/scargo/commands/docker.py` & `scargo-1.2.0/scargo/commands/docker.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 import subprocess
 import sys
 from pathlib import Path
 from typing import List, Optional, Sequence
 
 import docker
 
-from scargo.config import ProjectConfig
 from scargo.config_utils import get_scargo_config_or_exit
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 
 def scargo_docker_build(docker_opts: Sequence[str]) -> None:
     """
     Build docker
 
     :param docker_opts: additional docker options
     :raises CalledProcessError: if docker build fail
     """
-    logger = get_logger()
     logger.debug("Build docker environment.")
 
-    docker_path = _get_docker_path()
+    config = get_scargo_config_or_exit()
+    docker_path = _get_docker_path(config.project_root)
 
     try:
         subprocess.run(
             ["docker-compose", "build", *docker_opts], cwd=docker_path, check=True
         )
         logger.info("Initialize docker environment.")
     except subprocess.CalledProcessError:
@@ -45,19 +45,19 @@
     """
     Run docker
 
     :param docker_opts: additional docker options
     :param command: command to run in the container
     :raises CalledProcessError: if docker did not start
     """
-    logger = get_logger()
     logger.debug("Run docker environment.")
 
-    docker_path = _get_docker_path()
-    project_config_name = _get_project_config().name
+    config = get_scargo_config_or_exit()
+    docker_path = _get_docker_path(config.project_root)
+    project_config_name = config.project.name
 
     cmd = [
         "docker-compose",
         "run",
         *docker_opts,
         f"{project_config_name}_dev",
     ]
@@ -75,18 +75,18 @@
 def scargo_docker_exec(docker_opts: List[str]) -> None:
     """
     Exec docker
 
     :param docker_opts: additional docker options
     :raises CalledProcessError: if docker did not start
     """
-    logger = get_logger()
     logger.debug("Exec docker environment.")
 
-    image = _get_project_config().docker_image_tag
+    config = get_scargo_config_or_exit()
+    image = config.project.docker_image_tag
 
     if not image:
         logger.error("docker-image-tag not defined in .toml under project section")
         sys.exit(1)
 
     client = docker.from_env()
     newest_container = client.containers.list(
@@ -94,28 +94,22 @@
     )
     if not newest_container:
         logger.error("No running containers using image `%s` to attach to!", image)
         logger.info("Use scargo docker run to run container.")
         sys.exit(1)
 
     bash_command = ["bash"]
-    cmd = ["docker", "exec"] + docker_opts + [newest_container[0].id] + bash_command
+    cmd = ["docker", "exec", "-it", *docker_opts, newest_container[0].id, *bash_command]
     try:
         subprocess.run(cmd, check=True)
         logger.info("Stop exec docker environment.")
     except subprocess.CalledProcessError:
         logger.error("Exec docker fail.")
         sys.exit(1)
 
 
-def _get_docker_path() -> Path:
-    project_path = get_project_root()
+def _get_docker_path(project_path: Path) -> Path:
     # do not rebuild dockers in the docker
     if Path(project_path, ".dockerenv").exists():
-        logger = get_logger()
         logger.error("Cannot used docker command inside the docker container.")
         sys.exit(1)
     return Path(project_path, ".devcontainer")
-
-
-def _get_project_config() -> ProjectConfig:
-    return get_scargo_config_or_exit().project
```

### Comparing `scargo-1.1.0/scargo/commands/fix.py` & `scargo-1.2.0/scargo/commands/fix.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from scargo.commands.check import (
     CheckerFixer,
     ClangFormatChecker,
     CopyrightChecker,
     PragmaChecker,
 )
 from scargo.config_utils import prepare_config
-from scargo.path_utils import get_project_root
 
 
 def scargo_fix(pragma: bool, copy_right: bool, clang_format: bool) -> None:
     """
     Fix format
 
     :param bool pragma: fix pragma format
@@ -34,11 +33,11 @@
     if clang_format:
         checkers.append(ClangFormatChecker)
 
     if not checkers:
         checkers = [PragmaChecker, CopyrightChecker, ClangFormatChecker]
 
     # Todo, remove chdir and change cwd for checks
-    os.chdir(get_project_root())
+    os.chdir(config.project_root)
 
     for checker_class in checkers:
         checker_class(config, fix_errors=True).check()
```

### Comparing `scargo-1.1.0/scargo/commands/flash.py` & `scargo-1.2.0/scargo/commands/flash.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import sys
 from pathlib import Path
 from typing import Optional
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 
 def scargo_flash(
     app: bool, fs: bool, flash_profile: str, port: Optional[str] = None
 ) -> None:
     config = prepare_config()
     target = config.project.target
-    logger = get_logger()
 
     if port and target.family != "esp32":
         logger.error("--port option is only supported for esp32 projects.")
         sys.exit(1)
     if target.family == "esp32":
         flash_esp32(config, app=app, fs=fs, flash_profile=flash_profile, port=port)
     elif target.family == "stm32":
@@ -34,15 +34,15 @@
 def flash_esp32(
     config: Config,
     app: bool,
     fs: bool,
     flash_profile: str = "Debug",
     port: Optional[str] = None,
 ) -> None:
-    project_path = get_project_root()
+    project_path = config.project_root
     out_dir = project_path / "build" / flash_profile
     target = config.project.target
     command = []
     try:
         if app:
             app_name = config.project.name
             app_path = out_dir / f"{app_name}.bin"
@@ -68,22 +68,19 @@
             subprocess.check_call(command, cwd=project_path)
         else:
             command = ["esptool.py", "--chip", target.id, "write_flash", "@flash_args"]
             if port:
                 command.append(f"--port={port}")
             subprocess.check_call(command, cwd=out_dir)
     except subprocess.CalledProcessError:
-        logger = get_logger()
         logger.error("%s fail", command)
 
 
 def flash_stm32(config: Config, flash_profile: str = "Debug") -> None:
-    logger = get_logger()
-
-    project_path = get_project_root()
+    project_path = config.project_root
     bin_name = config.project.bin_name
     if not bin_name:
         logger.error("No bin_name in config!")
         sys.exit(1)
     bin_name = bin_name.lower()
     bin_path = project_path / "build" / flash_profile / "bin" / f"{bin_name}.bin"
```

### Comparing `scargo-1.1.0/scargo/commands/gen.py` & `scargo-1.2.0/scargo/commands/gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,69 +9,71 @@
 import sys
 from pathlib import Path
 from shutil import copyfile
 from typing import Optional
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
-from scargo.global_values import SCARGO_PGK_PATH
-from scargo.jinja.mock_gen import generate_mocks
-from scargo.jinja.ut_gen import generate_ut
+from scargo.file_generators.mock_gen import generate_mocks
+from scargo.file_generators.ut_gen import generate_ut
+from scargo.global_values import SCARGO_PKG_PATH
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 OUT_FS_DIR = Path("build", "fs")
 
 
 def scargo_gen(
-    project_profile_path: Path,
+    profile: str,
     gen_ut: Optional[Path],
     gen_mock: Optional[Path],
     certs: Optional[str],
     certs_mode: Optional[str],
     certs_input: Optional[Path],
     certs_passwd: Optional[str],
     fs: bool,
     single_bin: bool,
 ) -> None:
     config = prepare_config()
-    logger = get_logger()
 
     if gen_ut:
         generate_ut(gen_ut, config)
 
     if gen_mock:
         if gen_mock.suffix not in (".h", ".hpp"):
             logger.error("Not a header file. Please chose .h or .hpp file.")
             sys.exit(1)
-        if generate_mocks(gen_mock):
+        if generate_mocks(gen_mock, config.project.target.source_dir, config):
             logger.info(f"Generated: {gen_mock}")
         else:
             logger.info(f"Skipping: {gen_mock}")
 
     if certs:
-        generate_certs(certs, certs_mode, certs_input, certs_passwd)
+        generate_certs(
+            certs, certs_mode, certs_input, certs_passwd, config.project_root
+        )
 
     if fs:
         generate_fs(config)
 
     if single_bin:
+        project_profile_path = config.project_root / "build" / profile
         gen_single_binary(project_profile_path, config)
 
 
 def generate_certs(
     device_name: str,
     mode_for_certs: Optional[str],
     certs_intermediate_dir: Optional[Path],
     certs_passwd: Optional[str],
+    project_path: Path,
 ) -> None:
-    project_path = get_project_root()
-
-    internal_certs_dir = Path(SCARGO_PGK_PATH, "certs")
-    projects_builds_path = get_project_root() / "build"
+    internal_certs_dir = Path(SCARGO_PKG_PATH, "certs")
+    projects_builds_path = project_path / "build"
     certs_out_dir = projects_builds_path / "certs"
     if not certs_intermediate_dir:
         certs_intermediate_dir = projects_builds_path / "certs"
     if not certs_passwd:
         certs_passwd = "1234"
 
     if mode_for_certs == "all":
@@ -100,15 +102,14 @@
 
     certs_out_azure_dir = certs_out_dir / "azure"
     certs_out_uc_dir = project_path / OUT_FS_DIR
 
     certs_out_uc_dir.mkdir(parents=True, exist_ok=True)
     certs_out_azure_dir.mkdir(parents=True, exist_ok=True)
 
-    logger = get_logger()
     try:
         copyfile(
             certs_out_dir / "certs" / "iot-device.cert.pem",
             certs_out_uc_dir / "device_cert.pem",
         )
         copyfile(
             certs_out_dir / "private" / "iot-device.key.pem",
@@ -127,39 +128,36 @@
 
 
 def generate_fs(config: Config) -> None:
     target = config.project.target
     if target.family == "esp32":
         gen_fs_esp32(config)
     else:
-        logger = get_logger()
         logger.warning("Gen --fs command not supported for this target yet.")
 
 
 def gen_single_binary(project_profile_path: Path, config: Config) -> None:
     target = config.project.target
     if target.family == "esp32":
         gen_single_binary_esp32(project_profile_path, config)
     else:
-        logger = get_logger()
         logger.warning("Gen --bin command not supported for this target yet.")
 
 
 def gen_fs_esp32(config: Config) -> None:
     command = []
-    logger = get_logger()
     partition_list = config.get_esp32_config().partitions
     fs_size = 0
     for i in partition_list:
         split_list = i.split(",")
         if "spiffs" in split_list[0]:
             fs_size = int(re.sub(",", "", split_list[4]), 16)
 
     try:
-        project_path = get_project_root()
+        project_path = config.project_root
         fs_in_dir = project_path / "main/fs"
         fs_out_dir = project_path / OUT_FS_DIR
         fs_out_bin = project_path / "build/spiffs.bin"
         fs_in_dir.mkdir(parents=True, exist_ok=True)
         fs_out_dir.mkdir(parents=True, exist_ok=True)
 
         shutil.copytree(fs_in_dir, fs_out_dir, dirs_exist_ok=True)
@@ -177,15 +175,14 @@
 
     except subprocess.CalledProcessError:
         logger.error("%s fail", command)
         sys.exit(1)
 
 
 def gen_single_binary_esp32(project_profile_path: Path, config: Config) -> None:
-    logger = get_logger()
     partition_list = config.get_esp32_config().partitions
     target = config.project.target
 
     flasher_args_path = project_profile_path / "flash_args"
     if not flasher_args_path.is_file():
         logger.warning("%s does not exists", flasher_args_path)
         sys.exit(1)
@@ -219,11 +216,11 @@
     command.extend(line_list)
 
     if spiffs_addr:
         command.extend([spiffs_addr, "build/spiffs.bin"])
 
     try:
         logger.info("Running: %s", " ".join(command))
-        subprocess.check_call(command, cwd=get_project_root())
+        subprocess.check_call(command, cwd=config.project_root)
     except subprocess.CalledProcessError:
         logger.error("Generation of single binary failed")
         sys.exit(1)
```

### Comparing `scargo-1.1.0/scargo/commands/new.py` & `scargo-1.2.0/scargo/commands/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 from scargo import __version__
 from scargo.config import Target
 from scargo.config_utils import get_scargo_config_or_exit
+from scargo.file_generators.cpp_gen import generate_cpp
+from scargo.file_generators.toml_gen import generate_toml
 from scargo.global_values import SCARGO_DEFAULT_CONFIG_FILE, SCARGO_DOCKER_ENV
-from scargo.jinja.cpp_gen import generate_cpp
-from scargo.jinja.toml_gen import generate_toml
 from scargo.logger import get_logger
 
+logger = get_logger()
+
 
 def scargo_new(
     name: str,
     bin_name: Optional[str],
     lib_name: Optional[str],
     target: Target,
     create_docker: bool,
@@ -35,16 +37,14 @@
     :param str lib_name: name of lib file
     :param Target target: architecture type
     :param bool create_docker: initialize docker environment
     :param bool git: initialize git repository
     :return: None
     :raises FileExistsError: if project with provided name exist
     """
-    logger = get_logger()
-
     if not re.match(r"[a-zA-Z][\w-]*$", name):
         logger.error(
             "Name must consist of letters, digits, dash and undescore only,"
             " and the first character must be a letter"
         )
         sys.exit(1)
```

### Comparing `scargo-1.1.0/scargo/commands/publish.py` & `scargo-1.2.0/scargo/commands/publish.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,37 +7,36 @@
 import os
 import subprocess
 import sys
 from pathlib import Path
 
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 
 def scargo_publish(repo: str) -> None:
     """
     Publish conan package
 
     :param str repo: repository name
     :return: None
     """
-    logger = get_logger()
     config = prepare_config()
-    project_path = get_project_root()
+    project_path = config.project_root
     project_config = config.project
     project_name = project_config.name
     version = project_config.version
 
     conan_clean_remote()
     conan_add_remote(project_path)
     conan_add_conancenter()
 
     # Export package
-    # TODO discuss where to put package
     try:
         subprocess.check_call(
             "conan export-pkg . -f",
             cwd=project_path,
             shell=True,
         )
     except subprocess.CalledProcessError:
@@ -65,15 +64,14 @@
 def conan_add_remote(project_path: Path) -> None:
     """
     Add conan remote repository
 
     :param Path project_path: path to project
     :return: None
     """
-    logger = get_logger()
     config = prepare_config()
     conan_repo = config.conan.repo
     for repo_name, repo_url in conan_repo.items():
         try:
             subprocess.check_call(
                 ["conan", "remote", "add", repo_name, repo_url],
                 cwd=project_path,
@@ -90,28 +88,26 @@
     :return: None
     """
     try:
         subprocess.check_call(
             "conan remote add conancenter https://center.conan.io", shell=True
         )
     except subprocess.CalledProcessError:
-        logger = get_logger()
         logger.error("Unable to add conancenter remote repository")
 
 
 def conan_clean_remote() -> None:
     """
     Clean all remote repositories
 
     :return: None
     """
     try:
         subprocess.check_call("conan remote clean", shell=True)
     except subprocess.CalledProcessError:
-        logger = get_logger()
         logger.error("Unable to clean remote repository list")
 
 
 def conan_add_user(remote: str) -> None:
     """
     Add conan user
 
@@ -127,9 +123,8 @@
 
     if env_conan_user not in conan_user:
         try:
             subprocess.check_call(
                 ["conan", "user", "-p", env_conan_passwd, "-r", remote, env_conan_user],
             )
         except subprocess.CalledProcessError:
-            logger = get_logger()
             logger.error("Unable to add user")
```

### Comparing `scargo-1.1.0/scargo/commands/run.py` & `scargo-1.2.0/scargo/commands/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,45 +7,45 @@
 import sys
 from pathlib import Path
 from typing import List, Optional
 
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
+logger = get_logger()
 
-def scargo_run(
-    bin_path: Optional[Path], project_profile_path: Path, params: List[str]
-) -> None:
+
+def scargo_run(bin_path: Optional[Path], profile: str, params: List[str]) -> None:
     """
     Run command from CLI
 
     :param str bin_path: path to bin file
-    :param Path project_profile_path: path to build file
+    :param Path profile: build profile name
     :param str params: params for bin file
     :return: None
     """
-    logger = get_logger()
-    logger.info('Running "%s" build', project_profile_path.name)
+    logger.info('Running "%s" build', profile)
 
-    target = prepare_config().project.target
-    if "x86" not in target.family:
+    config = prepare_config()
+    if "x86" not in config.project.target.family:
         logger.info(
             "Run project on x86 architecture is not implemented for %s yet.",
-            target.family,
+            config.project.target.family,
         )
         sys.exit(1)
 
     if bin_path:
         bin_file_name = bin_path.name
         bin_file_path = bin_path.parent
         try:
             subprocess.check_call([f"./{bin_file_name}"] + params, cwd=bin_file_path)
         except subprocess.CalledProcessError:
             logger.error("bin file not found")
     else:
+        project_profile_path = config.project_root / "build" / profile
         bin_dir = project_profile_path / "bin"
         if bin_dir.is_dir():
             first_bin = next(bin_dir.iterdir())
             # Run project
             try:
                 subprocess.check_call([f"./{first_bin.name}"] + params, cwd=bin_dir)
             except subprocess.CalledProcessError:
```

### Comparing `scargo-1.1.0/scargo/commands/test.py` & `scargo-1.2.0/scargo/commands/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 """Run test from project"""
 import subprocess
 import sys
 from pathlib import Path
+from typing import List, Union
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+
+logger = get_logger()
 
 
 def scargo_test(verbose: bool) -> None:
     """
     Run test
     :param bool verbose: if verbose
     """
-    logger = get_logger()
     config = prepare_config()
 
     test_dir_name = "tests"
-    project_dir = get_project_root()
+    project_dir = config.project_root
     tests_src_dir = project_dir / test_dir_name
     test_build_dir = project_dir / "build" / test_dir_name
 
     if not tests_src_dir.exists():
         logger.error("Directory `tests` does not exist.")
         sys.exit(1)
 
@@ -53,34 +54,42 @@
 
     # run ut
     run_ut(config, verbose, test_build_dir)
 
 
 def run_ut(config: Config, verbose: bool, cwd: Path) -> None:
     # Run tests.
-    cmd = ["ctest"]
+    cmd: List[Union[str, Path]] = ["ctest"]
 
     if verbose:
         cmd.append("--verbose")
     try:
         # Using `subprocess.run` because tests can fail,
         # and we do not want Python to throw exception.
         subprocess.run(cmd, cwd=cwd, check=False)
 
         # Run code coverage.
-        cmd = ["gcovr", "-r", "ut", ".", "--html", "ut-coverage.html"]
+        cmd = [
+            "gcovr",
+            "-r",
+            "ut",
+            ".",
+            "-f",
+            config.project_root.joinpath(config.project.target.source_dir),
+            "--html",
+            "ut-coverage.html",
+        ]
 
         gcov_executable = config.tests.gcov_executable
 
         if gcov_executable != "":
             cmd.extend(["--gcov-executable", gcov_executable])
 
         subprocess.check_call(cmd, cwd=cwd)
     except subprocess.CalledProcessError:
-        logger = get_logger()
         logger.error("Fail to run project tests")
         sys.exit(1)
 
 
 def run_it(config: Config, verbose: bool) -> None:
     # Run tests.
     cmd = ["ctest"]
```

### Comparing `scargo-1.1.0/scargo/config.py` & `scargo-1.2.0/scargo/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,39 +16,44 @@
 
 
 class Config(BaseModel):
     project: "ProjectConfig"
     profiles: Dict[str, "ProfileConfig"] = Field(..., alias="profile")
     check: "ChecksConfig"
     doc: "DocConfig" = Field(
-        default_factory=lambda: DocConfig()
-    )  # pylint: disable=unnecessary-lambda
+        default_factory=lambda: DocConfig()  # pylint: disable=unnecessary-lambda
+    )
     tests: "TestConfig"
     dependencies: "Dependencies"
     conan: "ConanConfig"
     stm32: Optional["Stm32Config"]
     esp32: Optional["Esp32Config"]
     scargo: "ScargoConfig" = Field(
-        default_factory=lambda: ScargoConfig()
-    )  # pylint: disable=unnecessary-lambda
+        default_factory=lambda: ScargoConfig()  # pylint: disable=unnecessary-lambda
+    )
+    docker_compose: "DockerComposeConfig" = Field(
+        default_factory=lambda: DockerComposeConfig(),  # pylint: disable=unnecessary-lambda
+        alias="docker-compose",
+    )
+    project_root: Path
 
     def get_stm32_config(self) -> "Stm32Config":
         if not self.stm32:
             raise ConfigError("No [stm32] section in config")
         return self.stm32
 
     def get_esp32_config(self) -> "Esp32Config":
         if not self.esp32:
             raise ConfigError("No [esp32] section in config")
         return self.esp32
 
     @root_validator
-    def validate_special_configs(
+    def validate_special_configs(  # pylint: disable=no-self-argument
         cls, values: Dict[str, Any]
-    ) -> Dict[str, Any]:  # pylint: disable=no-self-argument
+    ) -> Dict[str, Any]:
         target_id = values["project"].target_id
         if target_id == "stm32" and not values["stm32"]:
             raise ConfigError("No [stm32] section in config")
         if target_id == "esp32" and not values["esp32"]:
             raise ConfigError("No [esp32] section in config")
         return values
 
@@ -205,16 +210,22 @@
 class ScargoConfig(BaseModel):
     console_log_level: str = Field("INFO", alias="console-log-level")
     file_log_level: str = Field("WARNING", alias="file-log-level")
     update_exclude: List[str] = Field(alias="update-exclude", default_factory=list)
     version: Optional[str]
 
 
+class DockerComposeConfig(BaseModel):
+    ports: List[str] = Field(default_factory=list)
+
+
 Config.update_forward_refs()
 ProjectConfig.update_forward_refs()
 ChecksConfig.update_forward_refs()
 Stm32Config.update_forward_refs()
 Esp32Config.update_forward_refs()
 
 
 def parse_config(config_file_path: Path) -> Config:
-    return Config.parse_obj(toml.load(config_file_path))
+    config_obj = toml.load(config_file_path)
+    config_obj["project_root"] = config_file_path.parent.absolute()
+    return Config.parse_obj(config_obj)
```

### Comparing `scargo-1.1.0/scargo/config_utils.py` & `scargo-1.2.0/scargo/config_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from scargo import __version__
 from scargo.config import Config, ConfigError, parse_config
 from scargo.docker_utils import run_scargo_again_in_docker
 from scargo.global_values import SCARGO_LOCK_FILE
 from scargo.logger import get_logger
 from scargo.path_utils import get_config_file_path
 
+logger = get_logger()
+
 
 def get_scargo_config_or_exit(
     config_file_path: Optional[Path] = None,
 ) -> Config:
     """
     :param config_file_path
     :return: project configuration as dict
     """
-    logger = get_logger()
     if config_file_path is None:
         config_file_path = get_config_file_path(SCARGO_LOCK_FILE)
     if config_file_path is None or not config_file_path.exists():
         logger.error("File `%s` does not exist.", SCARGO_LOCK_FILE)
         logger.info("Did you run `scargo update`?")
         sys.exit(1)
 
@@ -39,41 +40,39 @@
     Prepare configuration file
 
     :return: project configuration
     """
     config = get_scargo_config_or_exit()
     check_scargo_version(config)
     if run_in_docker:
-        run_scargo_again_in_docker(config.project)
+        run_scargo_again_in_docker(config.project, config.project_root)
     return config
 
 
 def check_scargo_version(config: Config) -> None:
     """
     Check scargo version
 
     :param Config config: project configuration
     :return: None
     """
     version_lock = config.scargo.version
     if not version_lock:
         add_version_to_scargo_lock()
     elif __version__ != version_lock:
-        logger = get_logger()
         logger.warning("Warning: scargo package is different then in lock file")
         logger.info("Run scargo update")
 
 
 def add_version_to_scargo_lock() -> None:
     """
     :return: project configuration as dict
     """
     scargo_lock = get_config_file_path(SCARGO_LOCK_FILE)
     if not scargo_lock:
-        logger = get_logger()
         logger.error("ERROR: File `%s` does not exist.", SCARGO_LOCK_FILE)
         logger.info("Did you run `scargo update`?")
         sys.exit(1)
 
     with open(scargo_lock, encoding="utf-8") as scargo_lock_file:
         config = tomlkit.load(scargo_lock_file)
```

### Comparing `scargo-1.1.0/scargo/docker_utils.py` & `scargo-1.2.0/scargo/docker_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 
 import docker as dock
 from docker import DockerClient
 
 from scargo.config import ProjectConfig
 from scargo.global_values import SCARGO_DOCKER_ENV
 from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
 
+logger = get_logger()
 
-def run_scargo_again_in_docker(project_config: ProjectConfig) -> None:
+
+def run_scargo_again_in_docker(
+    project_config: ProjectConfig, project_path: Path
+) -> None:
     """
     Run command in docker
 
     :param dict project_config: project configuration
+    :param Path project_path: path to project root
     :return: None
     """
     build_env = project_config.build_env
     if build_env != SCARGO_DOCKER_ENV or Path("/.dockerenv").exists():
         return
-    project_path = get_project_root()
     relative_path = Path.cwd().absolute().relative_to(project_path)
     path_in_docker = Path("/workspace", relative_path)
 
     cmd_args = sys.argv[1:]
 
     entrypoint = ""
     if project_config.target.family == "esp32":
@@ -58,15 +61,14 @@
     command: List[str],
     client: DockerClient,
     docker_tag: str,
     entrypoint: str,
     project_path: Path,
     path_in_docker: Path,
 ) -> int:
-    logger = get_logger()
     logger.info(f"Running '{' '.join(command)}' command in docker.")
     container = client.containers.run(
         docker_tag,
         command,
         volumes=[f"{project_path}:/workspace/", "/dev/:/dev/"],
         entrypoint=entrypoint,
         privileged=True,
```

### Comparing `scargo-1.1.0/scargo/global_values.py` & `scargo-1.2.0/scargo/global_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 """Global values for scargo"""
 import pkgutil
 from pathlib import Path
 
 DESCRIPTION = "C/C++ package and software development life cycle manager based on RUST cargo idea."
 
-SCARGO_PGK_PATH = (
+SCARGO_PKG_PATH = (
     Path(pkgutil.get_loader("scargo").path).parent  # type: ignore[union-attr]
     if pkgutil.get_loader("scargo").path  # type: ignore[union-attr]
-    else Path(Path(__file__).absolute()).parent
+    else Path(__file__).absolute().parent
 )
 SCARGO_DEFAULT_BUILD_ENV = "docker"
 SCARGO_DOCKER_ENV = "docker"
 
 SCARGO_LOCK_FILE = "scargo.lock"
 SCARGO_DEFAULT_CONFIG_FILE = "scargo.toml"
 ENV_DEFAULT_NAME = ".env"
```

### Comparing `scargo-1.1.0/scargo/jinja/conan/conanfile.py.j2` & `scargo-1.2.0/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/conan/conanfiletest.j2` & `scargo-1.2.0/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/cpp/cmake-src-stm32.j2` & `scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/cpp/cmake-src-x86.j2` & `scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/cpp/main.cpp.j2` & `scargo-1.2.0/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/docker/Dockerfile-esp32.j2` & `scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/docker/Dockerfile-stm32.j2` & `scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/docker/Dockerfile.j2` & `scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 RUN apt -y install cppcheck bzr lib32z1 \
     clang clang-format clang-tidy valgrind \
     gcovr doxygen curl libcurl4-openssl-dev \
     libcmocka0 libcmocka-dev plantuml
 
 FROM cpp AS {{ project.target.family }}
-{% include 'Dockerfile-' + project.target.family + '.j2' %}
+{% include 'docker/Dockerfile-' + project.target.family + '.j2' %}
 
 WORKDIR /opt
 
 FROM {{ project.target.family }} AS custom_{{ project.name }}
 {{ custom_docker }}
 FROM custom_{{ project.name }} AS {{ project.name }}_dev
```

### Comparing `scargo-1.1.0/scargo/jinja/docker/docker-compose.yaml.j2` & `scargo-1.2.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files 22% similar despite different names*

```diff
@@ -10,23 +10,29 @@
   GID_NUMBER: ${GID_NUMBER}
   UID_NUMBER: ${UID_NUMBER}
   DOCKER_IMAGE_ROOT: ${DOCKER_IMAGE_ROOT}
   CONAN_LOGIN_USERNAME: ${CONAN_LOGIN_USERNAME}
   CONAN_PASSWORD: ${CONAN_PASSWORD}
 
 services:
-  {{ project.name }}_dev:
-    image: {{ project.docker_image_tag }}
+  {{ config.project.name }}_dev:
+    image: {{ config.project.docker_image_tag }}
     platform: linux/amd64
     build:
       context: .
       args:
         <<: *project_config
     privileged: true
     volumes:
       - ..:/workspace
       - /dev:/dev
     command: sleep infinity
-  {% if project.in_repo_conan_cache %}
+  {% if config.project.in_repo_conan_cache %}
     environment:
       - CONAN_USER_HOME=/workspace
   {% endif %}
+  {% if config.docker_compose.ports %}
+    ports:
+    {% for port_ranges in config.docker_compose.ports %}
+      - "{{ port_ranges }}"
+    {% endfor %}
+  {% endif %}
```

### Comparing `scargo-1.1.0/scargo/jinja/docker_gen.py` & `scargo-1.2.0/scargo/file_generators/docker_gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,96 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 import os
 import shutil
 from pathlib import Path
+from typing import Any, Dict
 
 from scargo import __version__
-from scargo.config import ProjectConfig
-from scargo.global_values import SCARGO_PGK_PATH
-from scargo.jinja.base_gen import BaseGen
-from scargo.logger import get_logger
-from scargo.path_utils import get_project_root
+from scargo.config import Config
+from scargo.file_generators.base_gen import create_file_from_template
+from scargo.global_values import SCARGO_PKG_PATH
 
 
-class _DockerComposeTemplate(BaseGen):
+class _DockerComposeTemplate:
     """
     This class is a container for docker compose yaml files creation with multilayer approach
     """
 
-    def __init__(self, project_config: ProjectConfig, docker_path: Path):
-        template_dir = Path(SCARGO_PGK_PATH, "jinja", "docker")
-        BaseGen.__init__(self, template_dir)
+    def __init__(self, config: Config, docker_path: Path):
         self.docker_path = docker_path
-        # List of files to generate (template_path, output_path)
-        self._gen_file_list = [
-            ("docker-compose.yaml.j2", docker_path / "docker-compose.yaml"),
-            ("Dockerfile.j2", docker_path / "Dockerfile"),
-            ("devcontainer.json.j2", docker_path / "devcontainer.json"),
-        ]
-        if project_config.target.family == "stm32":
-            self._gen_file_list.extend([("stm32.cfg.j2", docker_path / "stm32.cfg")])
-        self.project_config = project_config
+        self._config = config
 
     def generate_docker_env(self) -> None:
         """Generate dirs and files"""
-        custom_docker = ""
-        self.create_file_from_template(
-            "Dockerfile-custom.j2",
-            self.docker_path / "Dockerfile-custom",
+        self._create_file_from_template(
+            "docker/Dockerfile-custom.j2",
+            "Dockerfile-custom",
             template_params={},
             overwrite=False,
         )
+        self._create_file_from_template(
+            "docker/docker-compose.yaml.j2",
+            "docker-compose.yaml",
+            template_params={"config": self._config},
+        )
+        self._create_file_from_template(
+            "docker/devcontainer.json.j2",
+            "devcontainer.json",
+            template_params={"project": self._config.project},
+        )
+        if self._config.project.target.family == "stm32":
+            self._create_file_from_template(
+                "docker/stm32.cfg.j2",
+                "stm32.cfg",
+                template_params={},
+            )
 
-        project_root = get_project_root()
-        custom_docker_path = project_root / self.project_config.docker_file
-        if custom_docker_path.is_file():
-            custom_docker = custom_docker_path.read_text()
+        custom_docker = self._get_dockerfile_custom_content()
+        scargo_package_version = self._set_up_package_version()
 
-        logger = get_logger()
-        logger.debug(
-            "Custom docker file path: %s", custom_docker_path.relative_to(project_root)
+        self._create_file_from_template(
+            "docker/Dockerfile.j2",
+            "Dockerfile",
+            template_params={
+                "project": self._config.project,
+                "scargo_package_version": scargo_package_version,
+                "custom_docker": custom_docker,
+            },
         )
 
-        scargo_package_version = self._set_up_package_version()
+    def _create_file_from_template(
+        self,
+        template_path: str,
+        output_filename: str,
+        template_params: Dict[str, Any],
+        overwrite: bool = True,
+    ) -> None:
+        create_file_from_template(
+            template_path,
+            self.docker_path / output_filename,
+            template_params=template_params,
+            config=self._config,
+            overwrite=overwrite,
+        )
 
-        for template, output_path in self._gen_file_list:
-            self.create_file_from_template(
-                template,
-                output_path,
-                template_params={
-                    "project": self.project_config,
-                    "scargo_package_version": scargo_package_version,
-                    "custom_docker": custom_docker,
-                },
-            )
+    def _get_dockerfile_custom_content(self) -> str:
+        project_root = self._config.project_root
+        custom_docker_path = project_root / self._config.project.docker_file
+        if custom_docker_path.is_file():
+            return custom_docker_path.read_text()
+        return ""
 
     def _set_up_package_version(self) -> str:
         if whl_path_str := os.getenv("SCARGO_DOCKER_INSTALL_LOCAL"):
-            repo_root = Path(__file__).parent.parent.parent
+            repo_root = SCARGO_PKG_PATH.parent
             whl_path = repo_root / whl_path_str
-            shutil.copy(repo_root / whl_path, self.docker_path)
+            shutil.copy(whl_path, self.docker_path)
             return whl_path.name
         return f"scargo=={__version__}"
 
 
-def generate_docker_compose(docker_path: Path, project_config: ProjectConfig) -> None:
-    docker_compose_template = _DockerComposeTemplate(project_config, docker_path)
+def generate_docker_compose(docker_path: Path, config: Config) -> None:
+    docker_compose_template = _DockerComposeTemplate(config, docker_path)
     docker_compose_template.generate_docker_env()
```

### Comparing `scargo-1.1.0/scargo/jinja/mock_gen.py` & `scargo-1.2.0/scargo/file_generators/mock_gen.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,83 +3,72 @@
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 from pathlib import Path
 from typing import List, Optional
 
 from clang.cindex import Cursor, CursorKind, Index
-from jinja2 import Environment, FileSystemLoader
 
-from scargo.jinja.mock_utils.data_classes import (
+from scargo.config import Config
+from scargo.file_generators.base_gen import create_file_from_template
+from scargo.file_generators.mock_utils.data_classes import (
     ArgumentDescriptor,
     HeaderDescriptor,
     MockClassDescriptor,
     MockFunctionDescriptor,
     MockNamespaceDescriptor,
 )
 
-# define paths
-absolute_path = Path(__file__).parent.absolute()
-SRC_DIR = "src"
 MOCKS_DIR = "tests/mocks"
 
-jinja_env = Environment(
-    loader=FileSystemLoader(absolute_path / "mock_templates"),
-    trim_blocks=True,
-    lstrip_blocks=True,
-)
-
-# json where the mock paths are held, which lack of implementation has been accepted
-missing_mocks_json = absolute_path / "mock_utils" / "missing_mocks.json"
-
 
-def generate_mocks(src_header: Path) -> bool:
+def generate_mocks(src_header: Path, src_dir: str, config: Config) -> bool:
     """
     Generates mock header and implementations for specified source headers.
     Creates directories and CMake lists where required.
     :param src_header Path to source directory or header
+    :param src_dir source directory name (dependent on target)
+    :param config
     """
-    src_dir = src_header.parent.name
 
     dst_header = get_mock_path(src_header, src_dir)
 
     # Skip generation if destination header exists
     if dst_header.is_file():
         return False
 
-    dst_mock = dst_header.with_name(f"mock_{dst_header.name}")
-    dst_mock_source = dst_header.with_name(f"mock_{dst_header.stem}.cpp")
+    template_and_output_paths = [
+        ("mock/class_interface.h.j2", dst_header),
+        ("mock/class_mock.h.j2", dst_header.with_name(f"mock_{dst_header.name}")),
+        ("mock/class_mock.cpp.j2", dst_header.with_name(f"mock_{dst_header.stem}.cpp")),
+    ]
 
     # Read classes and functions from the source header
     header_data = parse_file(src_header)
 
-    # generate public interface header
-    gen_header(dst_header, "class_interface.h.j2", header_data)
-    # generate mock header
-    gen_header(dst_mock, "class_mock.h.j2", header_data)
-    # generate mock implementation
-    gen_header(dst_mock_source, "class_mock.cpp.j2", header_data)
+    for template_path, output_path in template_and_output_paths:
+        create_file_from_template(
+            template_path,
+            output_path,
+            template_params={"header": header_data},
+            config=config,
+        )
 
     return True
 
 
 def get_mock_path(path: Path, src_dir: str) -> Path:
     parts: List[str] = list(path.parts)
     for i, part in enumerate(parts):
         if part == src_dir:
             parts[i] = MOCKS_DIR
             break
     return Path(*parts)
 
 
-def gen_header(path: Path, template_name: str, header_data: HeaderDescriptor) -> None:
-    with path.open("w", encoding="utf-8") as out:
-        out.write(jinja_env.get_template(template_name).render(header=header_data))
-
-
 class ParamsExtractor:
     @staticmethod
     def extract_cxx_methods(cursor: Cursor) -> List[MockFunctionDescriptor]:
         descriptors = (
             ParamsExtractor._extract_method_params(descendant)
             for descendant in cursor.walk_preorder()
             if descendant.kind == CursorKind.CXX_METHOD
```

### Comparing `scargo-1.1.0/scargo/jinja/mock_templates/class_interface.h.j2` & `scargo-1.2.0/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/mock_templates/class_mock.cpp.j2` & `scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/mock_templates/class_mock.h.j2` & `scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/mock_utils/cmake_utils.py` & `scargo-1.2.0/scargo/file_generators/mock_utils/cmake_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/mock_utils/data_classes.py` & `scargo-1.2.0/scargo/file_generators/mock_utils/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/templates/.gitlab-ci.yml.j2` & `scargo-1.2.0/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/templates/CMakeLists.txt.j2` & `scargo-1.2.0/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/templates/README.md.j2` & `scargo-1.2.0/scargo/file_generators/templates/README.md.j2`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ## Working with docker (recommended)
 
 - python3
 - pip
 - scargo
 - docker
-- docker-compose version 1.29.2
+- docker-compose
 
 {% if project.target.family == "esp32" %}
 # ESP32 configure
 At the beginning of a project is strongly recommended to configure the project using `idf.py menuconfig`
 In the console please run `idf.py menuconfig` and configure at least the following options:
 - Bootloader config -> Bootloader Optimization Level ...  (O2 is recommended)
 - Serial Flasher Config -> Flash Size ... (e.g. for wroom is 4MB)
```

### Comparing `scargo-1.1.0/scargo/jinja/templates/scargo.toml.j2` & `scargo-1.2.0/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/templates/stm32.cmake.j2` & `scargo-1.2.0/scargo/file_generators/templates/stm32.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/test_templates/CMakeLists-test.txt.j2` & `scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 set(CMAKE_C_COMPILER   "{{ tests.cc }}")
 {% endif %} {# tests.cc #}
 
 {% if tests.cxx %}
 set(CMAKE_CXX_COMPILER "{{ tests.cxx }}")
 {% endif %} {# tests.cxx #}
 
+set(CMAKE_CXX_STANDARD {{ cxxstandard }})
+
 {% if tests.cflags %}
 set(CMAKE_C_FLAGS   "{{ tests.cflags }}")
 {% endif %} {# tests.cflags #}
 
 {% if tests.cxxflags %}
 set(CMAKE_CXX_FLAGS "{{ tests.cxxflags }}")
 {% endif %} {# tests.cxxflags #}
```

### Comparing `scargo-1.1.0/scargo/jinja/test_templates/static_mock/static_mock.h` & `scargo-1.2.0/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/ut_gen.py` & `scargo-1.2.0/scargo/file_generators/ut_gen.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 # #
 
 import re
 from pathlib import Path
 from typing import List, Sequence
 
 from scargo.config import Config
-from scargo.global_values import SCARGO_PGK_PATH
-from scargo.jinja.base_gen import BaseGen
-from scargo.jinja.mock_utils.cmake_utils import add_subdirs_to_cmake
-from scargo.path_utils import get_project_root
+from scargo.file_generators.base_gen import create_file_from_template
+from scargo.file_generators.mock_utils.cmake_utils import add_subdirs_to_cmake
 
 HEADER_EXTENSIONS = (".h", ".hpp")
 SRC_EXTENSIONS = (".c", ".cpp")
 
 
 class HeaderDescriptor:
     """
@@ -28,21 +26,18 @@
     ) -> None:
         self.name = name
         self.includes = includes
         self.classes = classes
         self.namespaces = namespaces
 
 
-class _UnitTestsGen(BaseGen):
+class _UnitTestsGen:
     def __init__(self, config: Config):
-        template_dir = Path(SCARGO_PGK_PATH, "jinja", "ut_templates")
-        BaseGen.__init__(self, template_dir)
-
         self._config = config
-        self._project_path = get_project_root()
+        self._project_path = config.project_root
         self._ut_dir = self._project_path / "tests/ut"
 
     def generate_tests(self, input_path: Path, overwrite: bool) -> None:
         """Generates unit test files and corresponding cmake file
 
         :param Path input_path: Path to src file or src directory
         :param bool overwrite: overwrite files if exist
@@ -67,19 +62,20 @@
         """Generates unit test source file
 
         :param Path input_file_path: Path to src file
         :param Path output_file_path: Path to unit test file
         :param bool overwrite: overwrite if exists
         """
         header_descriptor = self._parse_header_file(input_file_path)
-        self.create_file_from_template(
-            "ut.cpp.j2",
+        create_file_from_template(
+            "ut/ut.cpp.j2",
             output_file_path,
             overwrite=overwrite,
             template_params={"header": header_descriptor},
+            config=self._config,
         )
 
     def _generate_cmake(self, src_dir_path: Path, ut_dir_path: Path) -> None:
         """Generate CMakeLists for unit tests
 
         :param Path src_dir_path: Source directory for which tests are being generated
         :param Path ut_dir_path: Directory of generated unit tests
@@ -100,23 +96,24 @@
 
         src_files = [
             p.absolute().relative_to(self._project_path.absolute())
             for p in self._get_paths_with_ext(src_dir_path, SRC_EXTENSIONS)
             if p.name != main_cpp
         ]
 
-        self.create_file_from_template(
-            "CMakeLists.txt.j2",
+        create_file_from_template(
+            "ut/CMakeLists.txt.j2",
             ut_dir_path / "CMakeLists.txt",
             overwrite=True,
             template_params={
                 "src_files": src_files,
                 "utest_name": ut_name,
                 "ut_files": ut_files,
             },
+            config=self._config,
         )
 
     def _get_unit_test_path(self, input_src_path: Path) -> Path:
         """Return output path for unit test
 
         :param Path input_src_path: Source path
         :return Path: output path for unit test
```

### Comparing `scargo-1.1.0/scargo/jinja/ut_templates/CMakeLists.txt.j2` & `scargo-1.2.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/jinja/ut_templates/ut.cpp.j2` & `scargo-1.2.0/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/logger.py` & `scargo-1.2.0/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/path_utils.py` & `scargo-1.2.0/scargo/path_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,7 @@
 
 
 def get_project_root_or_none() -> Optional[Path]:
     config_path = get_config_file_path(SCARGO_LOCK_FILE) or get_config_file_path(
         SCARGO_DEFAULT_CONFIG_FILE
     )
     return config_path.parent if config_path else None
-
-
-def get_project_root() -> Path:
-    project_root = get_project_root_or_none()
-    if not project_root:
-        raise FileNotFoundError("Config file not found!")
-    return project_root
```

### Comparing `scargo-1.1.0/scargo/templates/.clang-format` & `scargo-1.2.0/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/templates/.clang-tidy` & `scargo-1.2.0/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/templates/.gitignore` & `scargo-1.2.0/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/scargo/templates/LICENSE` & `scargo-1.2.0/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/setup.cfg` & `scargo-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.1.0/PKG-INFO` & `scargo-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.1.0
+Version: 1.2.0
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,19 +18,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: clang==14.0
 Requires-Dist: cmake==3.25.2
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: conan==1.59.0
-Requires-Dist: docker-compose==1.29.2
 Requires-Dist: docker==6.0.1
 Requires-Dist: esptool==4.5.1
 Requires-Dist: jinja2==3.1.2
-Requires-Dist: libclang==15.0.6.1
+Requires-Dist: libclang==16.0.0
 Requires-Dist: lizard==1.17.10
 Requires-Dist: pydantic==1.10.6
 Requires-Dist: shellingham==1.5.0.post1
 Requires-Dist: toml==0.10.2
 Requires-Dist: tomlkit==0.11.6
 Requires-Dist: typer==0.7.0
 Requires-Dist: allure-pytest ; extra == "dev"
@@ -91,15 +90,15 @@
 # Working with scargo
 You can find all information on how to work with scargo on official documentation webpage: https://spyro-soft.github.io/scargo/index.html
 ![Scargo flow gif](https://raw.githubusercontent.com/Spyro-Soft/scargo/develop/docs/source/_static/scargo_flow_docker.gif)
 
 # Project dependencies
 ## Working with docker (recommended)
 - docker
-- docker-compose version 1.29.2
+- docker-compose
 - pip
 - python3
 
 ## Working natively (not recommended, a lot of env setup)
 Base:
 
 - python >= 3.8
@@ -123,7 +122,11 @@
 Run scargo commands as you would do natively.
 
 2) If you create a project with --docker flag (`scargo new <my_proj> --docker ...`) or with any docker flag, by default each scargo command will be triggered in docker.
 
 ## Working natively
 1) Create a project with --no-docker flag (`scargo new <my_proj> --no-docker ...`).
 
+# Contributing
+
+See contributing guide on https://spyro-soft.github.io/scargo/contributing.html
+
```

