# Comparing `tmp/pdm-pep517-1.1.3.tar.gz` & `tmp/pdm-pep517-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-pep517-1.1.3.tar", last modified: Thu Mar 23 05:03:15 2023, max compression
+gzip compressed data, was "pdm-pep517-1.1.4.tar", last modified: Wed Apr 12 01:06:09 2023, max compression
```

## Comparing `pdm-pep517-1.1.3.tar` & `pdm-pep517-1.1.4.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0     1067 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/LICENSE
--rw-r--r--   0        0        0     6104 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/README.md
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/__init__.py
--rw-r--r--   0        0        0     1429 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/boolean/__init__.py
--rw-r--r--   0        0        0    51195 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/boolean/boolean.py
--rw-r--r--   0        0        0     1331 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/boolean.py.LICENSE.txt
--rw-r--r--   0        0        0      751 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/LICENSE
--rw-r--r--   0        0        0      694 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/__init__.py
--rw-r--r--   0        0        0    21290 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/errors.py
--rw-r--r--   0        0        0      856 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/platform.py
--rw-r--r--   0        0        0    18394 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/schema.py
--rw-r--r--   0        0        0     3913 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/utils.py
--rw-r--r--   0        0        0    65036 2023-03-23 05:03:13.184757 pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/validator.py
--rw-r--r--   0        0        0    62517 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/__init__.py
--rw-r--r--   0        0        0      880 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/_pyahocorasick.ABOUT
--rw-r--r--   0        0        0    20579 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/_pyahocorasick.py
--rw-r--r--   0        0        0    11413 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/apache-2.0.LICENSE
--rw-r--r--   0        0        0    18651 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/cc-by-4.0.LICENSE
--rw-r--r--   0        0        0    18651 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/data/cc-by-4.0.LICENSE
--rw-r--r--   0        0        0      215 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/data/license_key_index.json.ABOUT
--rw-r--r--   0        0        0   660008 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/data/scancode-licensedb-index.json
--rw-r--r--   0        0        0      197 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      501 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39084 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16314 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1072 2023-03-23 05:03:13.188757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      176 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0      104 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/_vendor/vendor.txt
--rw-r--r--   0        0        0     3565 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/api.py
--rw-r--r--   0        0        0    15529 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/base.py
--rw-r--r--   0        0        0     6388 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/editable.py
--rw-r--r--   0        0        0      510 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/exceptions.py
--rw-r--r--   0        0        0     1148 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/license.py
--rw-r--r--   0        0        0    14960 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/macosx_platform.py
--rw-r--r--   0        0        0    17260 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/metadata.py
--rw-r--r--   0        0        0        0 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/py.typed
--rw-r--r--   0        0        0     9737 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/scm.py
--rw-r--r--   0        0        0     3894 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/sdist.py
--rw-r--r--   0        0        0     6982 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/utils.py
--rw-r--r--   0        0        0     2680 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/validator.py
--rw-r--r--   0        0        0     2888 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/version.py
--rw-r--r--   0        0        0    12934 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pdm/pep517/wheel.py
--rw-r--r--   0        0        0     3036 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       72 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0      746 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/conftest.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0      197 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/build.py
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      582 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      201 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/build.py
--rw-r--r--   0        0        0      138 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      586 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      381 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      435 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      404 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      399 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-no-license/src/foo_module.py
-lrwxr-xr-x   0        0        0        0 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      310 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      600 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      557 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      557 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      576 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      515 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.192757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      466 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      259 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-purelib-with-build/build.py
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      580 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      415 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      397 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      502 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      408 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-using-scm/foo_module.py
--rw-r--r--   0        0        0      379 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0    14694 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/test_api.py
--rw-r--r--   0        0        0     4366 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/test_file_finder.py
--rw-r--r--   0        0        0     9638 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/test_metadata.py
--rw-r--r--   0        0        0      310 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/test_utils.py
--rw-r--r--   0        0        0     1883 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/test_validator.py
--rw-r--r--   0        0        0      732 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/test_wheel.py
--rw-r--r--   0        0        0      597 2023-03-23 05:03:13.196757 pdm-pep517-1.1.3/tests/testutils.py
--rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 pdm-pep517-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-12 01:06:09.289615 pdm-pep517-1.1.4/LICENSE
+-rw-r--r--   0        0        0     6104 2023-04-12 01:06:09.289615 pdm-pep517-1.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.289615 pdm-pep517-1.1.4/pdm/pep517/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 01:06:09.289615 pdm-pep517-1.1.4/pdm/pep517/_vendor/__init__.py
+-rw-r--r--   0        0        0     1429 2023-04-12 01:06:09.289615 pdm-pep517-1.1.4/pdm/pep517/_vendor/boolean/__init__.py
+-rw-r--r--   0        0        0    51195 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/boolean/boolean.py
+-rw-r--r--   0        0        0     1331 2023-04-12 01:06:09.289615 pdm-pep517-1.1.4/pdm/pep517/_vendor/boolean.py.LICENSE.txt
+-rw-r--r--   0        0        0      751 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/LICENSE
+-rw-r--r--   0        0        0      694 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/__init__.py
+-rw-r--r--   0        0        0    21290 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/errors.py
+-rw-r--r--   0        0        0      856 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/platform.py
+-rw-r--r--   0        0        0    18394 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/schema.py
+-rw-r--r--   0        0        0     3913 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/utils.py
+-rw-r--r--   0        0        0    65036 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/validator.py
+-rw-r--r--   0        0        0    62517 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/_pyahocorasick.ABOUT
+-rw-r--r--   0        0        0    20579 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/_pyahocorasick.py
+-rw-r--r--   0        0        0    11413 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/apache-2.0.LICENSE
+-rw-r--r--   0        0        0    18651 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/cc-by-4.0.LICENSE
+-rw-r--r--   0        0        0    18651 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/data/cc-by-4.0.LICENSE
+-rw-r--r--   0        0        0      215 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/data/license_key_index.json.ABOUT
+-rw-r--r--   0        0        0   660008 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/data/scancode-licensedb-index.json
+-rw-r--r--   0        0        0      197 2023-04-12 01:06:09.293615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      501 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39084 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16314 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1072 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      176 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0      104 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/_vendor/vendor.txt
+-rw-r--r--   0        0        0     3565 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/api.py
+-rw-r--r--   0        0        0    15529 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/base.py
+-rw-r--r--   0        0        0     6388 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/editable.py
+-rw-r--r--   0        0        0      510 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/license.py
+-rw-r--r--   0        0        0    14960 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/macosx_platform.py
+-rw-r--r--   0        0        0    17260 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/metadata.py
+-rw-r--r--   0        0        0        0 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/py.typed
+-rw-r--r--   0        0        0     9737 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/scm.py
+-rw-r--r--   0        0        0     3894 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/sdist.py
+-rw-r--r--   0        0        0     6982 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/utils.py
+-rw-r--r--   0        0        0     2680 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/validator.py
+-rw-r--r--   0        0        0     2888 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/version.py
+-rw-r--r--   0        0        0    12947 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pdm/pep517/wheel.py
+-rw-r--r--   0        0        0     3036 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/conftest.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0      197 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/build.py
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      582 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      201 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/build.py
+-rw-r--r--   0        0        0      138 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      586 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      381 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      435 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      404 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      399 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-no-license/src/foo_module.py
+lrwxr-xr-x   0        0        0        0 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      310 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      600 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      557 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      557 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-04-12 01:06:09.297615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      576 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      515 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      466 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      259 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-purelib-with-build/build.py
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      580 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      415 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      397 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      502 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      408 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       12 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-using-scm/foo_module.py
+-rw-r--r--   0        0        0      379 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0    14694 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/test_api.py
+-rw-r--r--   0        0        0     4366 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/test_file_finder.py
+-rw-r--r--   0        0        0     9638 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/test_metadata.py
+-rw-r--r--   0        0        0      310 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/test_utils.py
+-rw-r--r--   0        0        0     1883 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/test_validator.py
+-rw-r--r--   0        0        0      732 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/test_wheel.py
+-rw-r--r--   0        0        0      597 2023-04-12 01:06:09.301615 pdm-pep517-1.1.4/tests/testutils.py
+-rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 pdm-pep517-1.1.4/PKG-INFO
```

### Comparing `pdm-pep517-1.1.3/LICENSE` & `pdm-pep517-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/README.md` & `pdm-pep517-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/boolean/__init__.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/boolean/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/boolean/boolean.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/boolean/boolean.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/boolean.py.LICENSE.txt` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/boolean.py.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/LICENSE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/__init__.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/errors.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/errors.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/platform.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/platform.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/schema.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/schema.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/utils.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/cerberus/validator.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/cerberus/validator.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/__init__.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/_pyahocorasick.ABOUT` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/_pyahocorasick.ABOUT`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/_pyahocorasick.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/_pyahocorasick.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/apache-2.0.LICENSE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/cc-by-4.0.LICENSE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/data/cc-by-4.0.LICENSE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/data/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/license_expression/data/scancode-licensedb-index.json` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/license_expression/data/scancode-licensedb-index.json`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/LICENSE.APACHE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/LICENSE.BSD` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_elffile.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_manylinux.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_musllinux.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_parser.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_structures.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/_tokenizer.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/markers.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/requirements.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/specifiers.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/tags.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/utils.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/packaging/version.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/LICENSE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/_parser.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli/_re.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli_w/LICENSE` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/_vendor/tomli_w/_writer.py` & `pdm-pep517-1.1.4/pdm/pep517/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/api.py` & `pdm-pep517-1.1.4/pdm/pep517/api.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/base.py` & `pdm-pep517-1.1.4/pdm/pep517/base.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/editable.py` & `pdm-pep517-1.1.4/pdm/pep517/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/license.py` & `pdm-pep517-1.1.4/pdm/pep517/license.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/macosx_platform.py` & `pdm-pep517-1.1.4/pdm/pep517/macosx_platform.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/metadata.py` & `pdm-pep517-1.1.4/pdm/pep517/metadata.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/scm.py` & `pdm-pep517-1.1.4/pdm/pep517/scm.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/sdist.py` & `pdm-pep517-1.1.4/pdm/pep517/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/utils.py` & `pdm-pep517-1.1.4/pdm/pep517/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/validator.py` & `pdm-pep517-1.1.4/pdm/pep517/validator.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/version.py` & `pdm-pep517-1.1.4/pdm/pep517/version.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/pdm/pep517/wheel.py` & `pdm-pep517-1.1.4/pdm/pep517/wheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
 
     def _write_metadata_file(self, fp: TextIO) -> None:
         fp.write(self.format_pkginfo())
 
     def _write_wheel_file(self, fp: TextIO) -> None:
         fp.write(
             WHEEL_FILE_FORMAT.format(
-                is_purelib=self.meta.config.is_purelib, tag=self.tag
+                is_purelib=str(self.meta.config.is_purelib).lower(), tag=self.tag
             )
         )
 
     def _write_entry_points(self, fp: TextIO) -> None:
         entry_points = self.meta.entry_points
         for group_name in sorted(entry_points):
             fp.write(f"[{group_name}]\n")
```

### Comparing `pdm-pep517-1.1.3/pyproject.toml` & `pdm-pep517-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = []
-version = "1.1.3"
+version = "1.1.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://pdm.fming.dev"
 repository = "https://github.com/pdm-project/pdm-pep517"
```

### Comparing `pdm-pep517-1.1.3/tests/conftest.py` & `pdm-pep517-1.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm-pep517-1.1.4/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/test_api.py` & `pdm-pep517-1.1.4/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
         with zipfile.ZipFile(tmp_path / wheel_name) as zf:
             wheel_metadata = email.message_from_bytes(
                 zf.read("demo_package-0.1.0.dist-info/WHEEL")
             )
             version = zf.read("my_package/version.foo").decode("utf-8").strip()
             assert version == "0.1.0"
-            assert wheel_metadata["Root-Is-Purelib"] == "True"
+            assert wheel_metadata["Root-Is-Purelib"] == "true"
 
 
 @pytest.mark.skipif(
     sys.platform.startswith("win"), reason="Check file mode on Unix only"
 )
 def test_build_wheel_preserve_permission(tmp_path: Path) -> None:
     with build_fixture_project("demo-package"):
```

### Comparing `pdm-pep517-1.1.3/tests/test_file_finder.py` & `pdm-pep517-1.1.4/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/test_metadata.py` & `pdm-pep517-1.1.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/test_validator.py` & `pdm-pep517-1.1.4/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/test_wheel.py` & `pdm-pep517-1.1.4/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/tests/testutils.py` & `pdm-pep517-1.1.4/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `pdm-pep517-1.1.3/PKG-INFO` & `pdm-pep517-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-pep517
-Version: 1.1.3
+Version: 1.1.4
 Summary: A PEP 517 backend for PDM that supports PEP 621 metadata
 License: MIT
 Keywords: packaging,PEP 517,build
 Author-email: Frost Ming <mianghong@gmail.com>
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

