# Comparing `tmp/notter-0.1.0.tar.gz` & `tmp/notter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notter-0.1.0.tar", last modified: Mon Feb 20 08:29:41 2023, max compression
+gzip compressed data, was "notter-0.2.0.tar", last modified: Tue Apr 11 23:21:53 2023, max compression
```

## Comparing `notter-0.1.0.tar` & `notter-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-02-20 08:29:41.398767 notter-0.1.0/
--rw-r--r--   0 taylan     (501) staff       (20)     1843 2023-02-17 19:36:56.000000 notter-0.1.0/.gitignore
--rw-r--r--   0 taylan     (501) staff       (20)     1069 2022-02-20 15:04:38.000000 notter-0.1.0/LICENSE
--rw-r--r--   0 taylan     (501) staff       (20)      895 2023-02-17 19:38:24.000000 notter-0.1.0/Makefile
--rw-r--r--   0 taylan     (501) staff       (20)     1975 2023-02-20 08:29:41.398944 notter-0.1.0/PKG-INFO
--rw-r--r--   0 taylan     (501) staff       (20)       58 2023-02-09 14:36:24.000000 notter-0.1.0/README.md
--rw-r--r--   0 taylan     (501) staff       (20)     1697 2023-02-17 19:40:06.000000 notter-0.1.0/pyproject.toml
--rw-r--r--   0 taylan     (501) staff       (20)      926 2023-02-20 08:29:41.399529 notter-0.1.0/setup.cfg
--rw-r--r--   0 taylan     (501) staff       (20)      504 2023-02-17 18:49:22.000000 notter-0.1.0/setup.py
-drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-02-20 08:29:41.363469 notter-0.1.0/src/
-drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-02-20 08:29:41.393159 notter-0.1.0/src/notter/
--rw-r--r--   0 taylan     (501) staff       (20)        0 2022-02-20 16:37:42.000000 notter-0.1.0/src/notter/__init__.py
--rw-r--r--   0 taylan     (501) staff       (20)     5613 2023-02-17 19:55:14.000000 notter-0.1.0/src/notter/cli.py
--rw-r--r--   0 taylan     (501) staff       (20)      339 2023-02-03 18:00:03.000000 notter-0.1.0/src/notter/constants.py
--rw-r--r--   0 taylan     (501) staff       (20)      235 2023-02-02 13:55:14.000000 notter-0.1.0/src/notter/context.py
--rw-r--r--   0 taylan     (501) staff       (20)     2143 2023-02-17 16:39:17.000000 notter-0.1.0/src/notter/controller.py
--rw-r--r--   0 taylan     (501) staff       (20)      266 2023-02-03 18:00:12.000000 notter-0.1.0/src/notter/exceptions.py
--rw-r--r--   0 taylan     (501) staff       (20)     2010 2023-02-17 16:52:59.000000 notter-0.1.0/src/notter/explorer.py
--rw-r--r--   0 taylan     (501) staff       (20)     2145 2023-02-17 16:49:54.000000 notter-0.1.0/src/notter/index.py
--rw-r--r--   0 taylan     (501) staff       (20)      979 2023-02-17 18:47:56.000000 notter-0.1.0/src/notter/model.py
--rw-r--r--   0 taylan     (501) staff       (20)     2787 2023-02-17 16:46:19.000000 notter-0.1.0/src/notter/notter.py
--rw-r--r--   0 taylan     (501) staff       (20)     4235 2023-02-17 18:48:13.000000 notter-0.1.0/src/notter/repository.py
--rw-r--r--   0 taylan     (501) staff       (20)     1251 2023-02-17 16:45:32.000000 notter-0.1.0/src/notter/utils.py
-drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-02-20 08:29:41.396652 notter-0.1.0/src/notter.egg-info/
--rw-r--r--   0 taylan     (501) staff       (20)     1975 2023-02-20 08:29:41.000000 notter-0.1.0/src/notter.egg-info/PKG-INFO
--rw-r--r--   0 taylan     (501) staff       (20)      611 2023-02-20 08:29:41.000000 notter-0.1.0/src/notter.egg-info/SOURCES.txt
--rw-r--r--   0 taylan     (501) staff       (20)        1 2023-02-20 08:29:41.000000 notter-0.1.0/src/notter.egg-info/dependency_links.txt
--rw-r--r--   0 taylan     (501) staff       (20)       42 2023-02-20 08:29:41.000000 notter-0.1.0/src/notter.egg-info/entry_points.txt
--rw-r--r--   0 taylan     (501) staff       (20)       86 2023-02-20 08:29:41.000000 notter-0.1.0/src/notter.egg-info/requires.txt
--rw-r--r--   0 taylan     (501) staff       (20)        7 2023-02-20 08:29:41.000000 notter-0.1.0/src/notter.egg-info/top_level.txt
-drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-02-20 08:29:41.397318 notter-0.1.0/tests/
--rw-r--r--   0 taylan     (501) staff       (20)        0 2023-02-17 16:30:24.000000 notter-0.1.0/tests/__init__.py
-drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-02-20 08:29:41.398267 notter-0.1.0/tests/notter/
--rw-r--r--   0 taylan     (501) staff       (20)        0 2023-02-17 16:30:42.000000 notter-0.1.0/tests/notter/__init__.py
--rw-r--r--   0 taylan     (501) staff       (20)      461 2023-02-20 08:15:34.000000 notter-0.1.0/tests/notter/test_cli.py
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.510060 notter-0.2.0/
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.451220 notter-0.2.0/.github/
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.483040 notter-0.2.0/.github/workflows/
+-rw-r--r--   0 taylan     (501) staff       (20)      894 2023-04-11 22:26:00.000000 notter-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 taylan     (501) staff       (20)     1843 2023-02-17 19:36:56.000000 notter-0.2.0/.gitignore
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.485814 notter-0.2.0/.vscode/
+-rw-r--r--   0 taylan     (501) staff       (20)      644 2023-04-05 19:26:19.000000 notter-0.2.0/.vscode/launch.json
+-rw-r--r--   0 taylan     (501) staff       (20)     1069 2022-02-20 15:04:38.000000 notter-0.2.0/LICENSE
+-rw-r--r--   0 taylan     (501) staff       (20)      995 2023-04-11 22:26:29.000000 notter-0.2.0/Makefile
+-rw-r--r--   0 taylan     (501) staff       (20)     8371 2023-04-11 23:21:53.510246 notter-0.2.0/PKG-INFO
+-rw-r--r--   0 taylan     (501) staff       (20)     6403 2023-04-11 23:12:40.000000 notter-0.2.0/README.md
+-rw-r--r--   0 taylan     (501) staff       (20)       65 2023-02-20 09:31:16.000000 notter-0.2.0/install.py
+-rw-r--r--   0 taylan     (501) staff       (20)     1754 2023-04-11 23:21:14.000000 notter-0.2.0/pyproject.toml
+-rw-r--r--   0 taylan     (501) staff       (20)      966 2023-04-11 23:21:53.511315 notter-0.2.0/setup.cfg
+-rw-r--r--   0 taylan     (501) staff       (20)      519 2023-04-11 23:21:20.000000 notter-0.2.0/setup.py
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.452411 notter-0.2.0/src/
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.495884 notter-0.2.0/src/notter/
+-rw-r--r--   0 taylan     (501) staff       (20)        0 2022-02-20 16:37:42.000000 notter-0.2.0/src/notter/__init__.py
+-rw-r--r--   0 taylan     (501) staff       (20)     4761 2023-04-05 19:26:20.000000 notter-0.2.0/src/notter/cli.py
+-rw-r--r--   0 taylan     (501) staff       (20)      339 2023-02-03 18:00:03.000000 notter-0.2.0/src/notter/constants.py
+-rw-r--r--   0 taylan     (501) staff       (20)      235 2023-02-02 13:55:14.000000 notter-0.2.0/src/notter/context.py
+-rw-r--r--   0 taylan     (501) staff       (20)     2344 2023-04-05 19:26:20.000000 notter-0.2.0/src/notter/controller.py
+-rw-r--r--   0 taylan     (501) staff       (20)      266 2023-04-05 19:00:32.000000 notter-0.2.0/src/notter/exceptions.py
+-rw-r--r--   0 taylan     (501) staff       (20)     2010 2023-04-05 19:00:39.000000 notter-0.2.0/src/notter/explorer.py
+-rw-r--r--   0 taylan     (501) staff       (20)     2332 2023-04-05 19:26:20.000000 notter-0.2.0/src/notter/index.py
+-rw-r--r--   0 taylan     (501) staff       (20)      947 2023-02-22 16:04:34.000000 notter-0.2.0/src/notter/model.py
+-rw-r--r--   0 taylan     (501) staff       (20)     2776 2023-04-05 19:26:20.000000 notter-0.2.0/src/notter/notter.py
+-rw-r--r--   0 taylan     (501) staff       (20)     4397 2023-04-11 22:33:36.000000 notter-0.2.0/src/notter/repository.py
+-rw-r--r--   0 taylan     (501) staff       (20)     1477 2023-04-05 19:26:20.000000 notter-0.2.0/src/notter/utils.py
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.500725 notter-0.2.0/src/notter.egg-info/
+-rw-r--r--   0 taylan     (501) staff       (20)     8371 2023-04-11 23:21:53.000000 notter-0.2.0/src/notter.egg-info/PKG-INFO
+-rw-r--r--   0 taylan     (501) staff       (20)      834 2023-04-11 23:21:53.000000 notter-0.2.0/src/notter.egg-info/SOURCES.txt
+-rw-r--r--   0 taylan     (501) staff       (20)        1 2023-04-11 23:21:53.000000 notter-0.2.0/src/notter.egg-info/dependency_links.txt
+-rw-r--r--   0 taylan     (501) staff       (20)       42 2023-04-11 23:21:53.000000 notter-0.2.0/src/notter.egg-info/entry_points.txt
+-rw-r--r--   0 taylan     (501) staff       (20)       98 2023-04-11 23:21:53.000000 notter-0.2.0/src/notter.egg-info/requires.txt
+-rw-r--r--   0 taylan     (501) staff       (20)        7 2023-04-11 23:21:53.000000 notter-0.2.0/src/notter.egg-info/top_level.txt
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.502263 notter-0.2.0/tests/
+-rw-r--r--   0 taylan     (501) staff       (20)        0 2023-02-17 16:30:24.000000 notter-0.2.0/tests/__init__.py
+-rw-r--r--   0 taylan     (501) staff       (20)     1266 2023-04-05 19:26:20.000000 notter-0.2.0/tests/conftest.py
+drwxr-xr-x   0 taylan     (501) staff       (20)        0 2023-04-11 23:21:53.509700 notter-0.2.0/tests/notter/
+-rw-r--r--   0 taylan     (501) staff       (20)        0 2023-02-17 16:30:42.000000 notter-0.2.0/tests/notter/__init__.py
+-rw-r--r--   0 taylan     (501) staff       (20)      379 2023-04-05 19:26:20.000000 notter-0.2.0/tests/notter/test_cli.py
+-rw-r--r--   0 taylan     (501) staff       (20)     5446 2023-04-05 19:26:20.000000 notter-0.2.0/tests/notter/test_controller.py
+-rw-r--r--   0 taylan     (501) staff       (20)     5128 2023-04-05 19:26:20.000000 notter-0.2.0/tests/notter/test_index.py
+-rw-r--r--   0 taylan     (501) staff       (20)     4098 2023-04-05 19:26:20.000000 notter-0.2.0/tests/notter/test_notter.py
+-rw-r--r--   0 taylan     (501) staff       (20)     6704 2023-04-11 22:43:45.000000 notter-0.2.0/tests/notter/test_repository.py
+-rw-r--r--   0 taylan     (501) staff       (20)      686 2023-04-05 19:26:20.000000 notter-0.2.0/tests/notter/test_utils.py
```

### Comparing `notter-0.1.0/.gitignore` & `notter-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `notter-0.1.0/LICENSE` & `notter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notter-0.1.0/Makefile` & `notter-0.2.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 00000000: 5041 434b 4147 455f 4e41 4d45 3a3d 6e6f  PACKAGE_NAME:=no
 00000010: 7474 6572 0a50 4143 4b41 4745 5f4c 4f43  tter.PACKAGE_LOC
 00000020: 3a3d 7372 632f 2428 5041 434b 4147 455f  :=src/$(PACKAGE_
 00000030: 4e41 4d45 290a 5059 5448 4f4e 3a3d 7079  NAME).PYTHON:=py
-00000040: 7468 6f6e 332e 3130 0a56 454e 563a 3d2e  thon3.10.VENV:=.
-00000050: 2f76 656e 760a 5049 505f 5645 4e56 3a3d  /venv.PIP_VENV:=
-00000060: 2428 5645 4e56 292f 6269 6e2f 7069 700a  $(VENV)/bin/pip.
-00000070: 5245 504f 5254 5f44 4952 3d2e 2f72 6570  REPORT_DIR=./rep
-00000080: 6f72 7473 0a0a 2e50 484f 4e59 3a20 7665  orts...PHONY: ve
-00000090: 6e76 0a76 656e 763a 0a09 2428 5059 5448  nv.venv:..$(PYTH
-000000a0: 4f4e 2920 2d6d 2076 656e 7620 2428 5645  ON) -m venv $(VE
-000000b0: 4e56 290a 0924 2850 4950 5f56 454e 5629  NV)..$(PIP_VENV)
-000000c0: 2069 6e73 7461 6c6c 202d 6520 2e0a 0a2e   install -e ....
-000000d0: 5048 4f4e 593a 2076 656e 765f 6465 760a  PHONY: venv_dev.
-000000e0: 7665 6e76 5f64 6576 3a0a 0924 2850 5954  venv_dev:..$(PYT
-000000f0: 484f 4e29 202d 6d20 7665 6e76 2024 2856  HON) -m venv $(V
-00000100: 454e 5629 0a09 2428 5049 505f 5645 4e56  ENV)..$(PIP_VENV
-00000110: 2920 696e 7374 616c 6c20 2d65 2027 2e5b  ) install -e '.[
-00000120: 6465 765d 270a 0a2e 5048 4f4e 593a 2063  dev]'...PHONY: c
-00000130: 6c65 616e 0a63 6c65 616e 3a0a 0972 6d20  lean.clean:..rm 
-00000140: 2d72 6620 2428 5645 4e56 290a 0966 696e  -rf $(VENV)..fin
-00000150: 6420 2428 5041 434b 4147 455f 4c4f 4329  d $(PACKAGE_LOC)
-00000160: 202d 7479 7065 2064 202d 6e61 6d65 205f   -type d -name _
-00000170: 5f70 7963 6163 6865 5f5f 202d 6578 6563  _pycache__ -exec
-00000180: 2072 6d20 2d72 207b 7d20 5c2b 0a09 726d   rm -r {} \+..rm
-00000190: 202d 7266 202a 2e65 6767 2d69 6e66 6f20   -rf *.egg-info 
-000001a0: 6275 696c 6420 6469 7374 0a09 726d 202d  build dist..rm -
-000001b0: 7266 2027 2e6d 7970 795f 6361 6368 6527  rf '.mypy_cache'
-000001c0: 0a09 726d 202d 7266 2027 2e65 6767 7327  ..rm -rf '.eggs'
-000001d0: 0a0a 2e50 484f 4e59 3a20 666f 726d 6174  ...PHONY: format
-000001e0: 0a66 6f72 6d61 743a 2024 2856 454e 565f  .format: $(VENV_
-000001f0: 4445 5629 0a09 6973 6f72 7420 2428 5041  DEV)..isort $(PA
-00000200: 434b 4147 455f 4c4f 4329 0a09 626c 6163  CKAGE_LOC)..blac
-00000210: 6b20 2428 5041 434b 4147 455f 4c4f 4329  k $(PACKAGE_LOC)
-00000220: 0a0a 2e50 484f 4e59 3a20 6c69 6e74 0a6c  ...PHONY: lint.l
-00000230: 696e 743a 2066 6f72 6d61 740a 0962 6c61  int: format..bla
-00000240: 636b 202d 2d64 6966 6620 2d2d 6368 6563  ck --diff --chec
-00000250: 6b20 2428 5041 434b 4147 455f 4c4f 4329  k $(PACKAGE_LOC)
-00000260: 0a09 666c 616b 6538 2024 2850 4143 4b41  ..flake8 $(PACKA
-00000270: 4745 5f4c 4f43 290a 096d 7970 7920 2428  GE_LOC)..mypy $(
-00000280: 5041 434b 4147 455f 4c4f 4329 0a09 6973  PACKAGE_LOC)..is
-00000290: 6f72 7420 2d2d 6469 6666 202d 2d63 6865  ort --diff --che
-000002a0: 636b 2024 2850 4143 4b41 4745 5f4c 4f43  ck $(PACKAGE_LOC
-000002b0: 290a 0a2e 5048 4f4e 593a 2075 6e69 7474  )...PHONY: unitt
-000002c0: 6573 7473 0a75 6e69 7474 6573 7473 3a20  ests.unittests: 
-000002d0: 7665 6e76 5f64 6576 0a09 5059 5448 4f4e  venv_dev..PYTHON
-000002e0: 5041 5448 3d73 7263 2063 6f76 6572 6167  PATH=src coverag
-000002f0: 6520 7275 6e20 2d6d 2070 7974 6573 7420  e run -m pytest 
-00000300: 2d73 7620 7465 7374 7320 2d2d 6a75 6e69  -sv tests --juni
-00000310: 7478 6d6c 3d24 2852 4550 4f52 545f 4449  txml=$(REPORT_DI
-00000320: 5229 2f6a 756e 6974 2e78 6d6c 0a09 636f  R)/junit.xml..co
-00000330: 7665 7261 6765 2078 6d6c 202d 6920 2d6f  verage xml -i -o
-00000340: 2024 2852 4550 4f52 545f 4449 5229 2f63   $(REPORT_DIR)/c
-00000350: 6f76 6572 6167 652e 786d 6c0a 0a2e 5048  overage.xml...PH
-00000360: 4f4e 593a 2074 6573 740a 7465 7374 3a20  ONY: test.test: 
-00000370: 6c69 6e74 2075 6e69 7474 6573 7473 0a    lint unittests.
+00000040: 7468 6f6e 330a 5645 4e56 3a3d 2e2f 7665  thon3.VENV:=./ve
+00000050: 6e76 0a50 4950 5f56 454e 563a 3d24 2856  nv.PIP_VENV:=$(V
+00000060: 454e 5629 2f62 696e 2f70 6970 0a52 4550  ENV)/bin/pip.REP
+00000070: 4f52 545f 4449 523d 2e2f 7265 706f 7274  ORT_DIR=./report
+00000080: 730a 0a2e 5048 4f4e 593a 2076 656e 760a  s...PHONY: venv.
+00000090: 7665 6e76 3a0a 0924 2850 5954 484f 4e29  venv:..$(PYTHON)
+000000a0: 202d 6d20 7665 6e76 2024 2856 454e 5629   -m venv $(VENV)
+000000b0: 0a09 2428 5049 505f 5645 4e56 2920 696e  ..$(PIP_VENV) in
+000000c0: 7374 616c 6c20 2d65 202e 0a0a 2e50 484f  stall -e ....PHO
+000000d0: 4e59 3a20 7665 6e76 5f64 6576 0a76 656e  NY: venv_dev.ven
+000000e0: 765f 6465 763a 0a09 2428 5059 5448 4f4e  v_dev:..$(PYTHON
+000000f0: 2920 2d6d 2076 656e 7620 2428 5645 4e56  ) -m venv $(VENV
+00000100: 290a 0924 2850 4950 5f56 454e 5629 2069  )..$(PIP_VENV) i
+00000110: 6e73 7461 6c6c 202d 6520 272e 5b64 6576  nstall -e '.[dev
+00000120: 5d27 0a0a 2e50 484f 4e59 3a20 636c 6561  ]'...PHONY: clea
+00000130: 6e0a 636c 6561 6e3a 0a09 726d 202d 7266  n.clean:..rm -rf
+00000140: 2024 2856 454e 5629 0a09 6669 6e64 2024   $(VENV)..find $
+00000150: 2850 4143 4b41 4745 5f4c 4f43 2920 2d74  (PACKAGE_LOC) -t
+00000160: 7970 6520 6420 2d6e 616d 6520 5f5f 7079  ype d -name __py
+00000170: 6361 6368 655f 5f20 2d65 7865 6320 726d  cache__ -exec rm
+00000180: 202d 7220 7b7d 205c 2b0a 0972 6d20 2d72   -r {} \+..rm -r
+00000190: 6620 2a2e 6567 672d 696e 666f 2062 7569  f *.egg-info bui
+000001a0: 6c64 2064 6973 740a 0972 6d20 2d72 6620  ld dist..rm -rf 
+000001b0: 272e 6d79 7079 5f63 6163 6865 270a 0972  '.mypy_cache'..r
+000001c0: 6d20 2d72 6620 272e 6567 6773 270a 0a2e  m -rf '.eggs'...
+000001d0: 5048 4f4e 593a 2066 6f72 6d61 740a 666f  PHONY: format.fo
+000001e0: 726d 6174 3a20 2428 5645 4e56 5f44 4556  rmat: $(VENV_DEV
+000001f0: 290a 0969 736f 7274 2024 2850 4143 4b41  )..isort $(PACKA
+00000200: 4745 5f4c 4f43 290a 0962 6c61 636b 2024  GE_LOC)..black $
+00000210: 2850 4143 4b41 4745 5f4c 4f43 290a 0a2e  (PACKAGE_LOC)...
+00000220: 5048 4f4e 593a 206c 696e 740a 6c69 6e74  PHONY: lint.lint
+00000230: 3a20 666f 726d 6174 0a09 626c 6163 6b20  : format..black 
+00000240: 2d2d 6469 6666 202d 2d63 6865 636b 2024  --diff --check $
+00000250: 2850 4143 4b41 4745 5f4c 4f43 290a 0966  (PACKAGE_LOC)..f
+00000260: 6c61 6b65 3820 2428 5041 434b 4147 455f  lake8 $(PACKAGE_
+00000270: 4c4f 4329 0a09 6d79 7079 2024 2850 4143  LOC)..mypy $(PAC
+00000280: 4b41 4745 5f4c 4f43 290a 0969 736f 7274  KAGE_LOC)..isort
+00000290: 202d 2d64 6966 6620 2d2d 6368 6563 6b20   --diff --check 
+000002a0: 2428 5041 434b 4147 455f 4c4f 4329 0a0a  $(PACKAGE_LOC)..
+000002b0: 2e50 484f 4e59 3a20 756e 6974 7465 7374  .PHONY: unittest
+000002c0: 730a 756e 6974 7465 7374 733a 2076 656e  s.unittests: ven
+000002d0: 765f 6465 760a 0950 5954 484f 4e50 4154  v_dev..PYTHONPAT
+000002e0: 483d 7372 6320 636f 7665 7261 6765 2072  H=src coverage r
+000002f0: 756e 202d 6d20 7079 7465 7374 202d 7376  un -m pytest -sv
+00000300: 2074 6573 7473 202d 2d6a 756e 6974 786d   tests --junitxm
+00000310: 6c3d 2428 5245 504f 5254 5f44 4952 292f  l=$(REPORT_DIR)/
+00000320: 6a75 6e69 742e 786d 6c0a 0963 6f76 6572  junit.xml..cover
+00000330: 6167 6520 786d 6c20 2d69 202d 6f20 2428  age xml -i -o $(
+00000340: 5245 504f 5254 5f44 4952 292f 636f 7665  REPORT_DIR)/cove
+00000350: 7261 6765 2e78 6d6c 0a0a 2e50 484f 4e59  rage.xml...PHONY
+00000360: 3a20 7465 7374 0a74 6573 743a 206c 696e  : test.test: lin
+00000370: 7420 756e 6974 7465 7374 730a 0a2e 5048  t unittests...PH
+00000380: 4f4e 593a 2062 756e 646c 650a 6275 6e64  ONY: bundle.bund
+00000390: 6c65 3a20 2428 5645 4e56 290a 0970 7969  le: $(VENV)..pyi
+000003a0: 6e73 7461 6c6c 6572 2069 6e73 7461 6c6c  nstaller install
+000003b0: 2e70 7920 2d2d 6e61 6d65 206e 6f74 7465  .py --name notte
+000003c0: 7220 2d2d 6f6e 6566 696c 6520 2d2d 636f  r --onefile --co
+000003d0: 7079 2d6d 6574 6164 6174 6120 6e6f 7474  py-metadata nott
+000003e0: 6572 0a                                  er.
```

### Comparing `notter-0.1.0/pyproject.toml` & `notter-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notter"
-version = "0.1.0"
+version = "0.2.0"
 description = "A simple note taking tool for software projects."
 authors = [
     {name = "Taylan Dogan", email = "taylandogan.nl@gmail.com"},
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["notes", "todos", "tracking", "index"]
 
 # Requirements
 dependencies = ["click", "pygments"]
 
 [project.optional-dependencies]
 # TODO: Add minimum versions next to dev/test dependencies
-dev  = ["black", "flake8", "isort", "mypy", "coverage", "pytest"]
+dev  = ["black", "flake8", "isort", "mypy", "coverage", "pytest", "pyinstaller"]
 test = [ "coverage", "pytest"]
 
 [scripts]
 notter = "notter.cli:cli"
 
 [tool.black]
 line-length = 120
@@ -40,21 +40,24 @@
 multi_line_output = 3
 order_by_type = true
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 use_parentheses = true
 line_length = 120
 force_grid_wrap = 0
 
+[tool.coverage.paths]
+source = ["src"]
+
 [tool.coverage.run]
+branch = true
 source = ["src"]
 relative_files = true
-branch = true
 omit = [
   "reports/*",
-	"tests/*",
+	"*/tests/*",
   "src/notter/constants.py",
 ]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 testpaths = ["tests"]
 asyncio_mode = "auto"
```

### Comparing `notter-0.1.0/setup.cfg` & `notter-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = notter
-version = 0.1.0
+version = 0.2.0
 author = Taylan Dogan
 author_email = taylandogan.nl@gmail.com
 license = MIT
 summary = A simple note taking tool for software projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taylandogan/notter
 home_page = https://github.com/taylandogan/notter
 classifier = 
 	Intended Audience :: Developers
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
```

### Comparing `notter-0.1.0/src/notter/cli.py` & `notter-0.2.0/src/notter/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-import subprocess
+import sys
 from importlib.metadata import version as pkg_version
 from pathlib import Path
 from typing import Optional, Tuple
 
 import click
 from click import Context, pass_context
 
@@ -15,62 +15,40 @@
 from notter.model import NoteType
 from notter.notter import Notter
 
 SRC_PATH_VAR = "SRC_PATH"
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
-def fetch_git_config() -> Tuple[str, str]:
-    click.echo("Binding your Git user to Notter")
-    username_process = subprocess.run(["git", "config", "user.name"], capture_output=True)
-    email_process = subprocess.run(["git", "config", "user.email"], capture_output=True)
-
-    if username_process.returncode != 0 or email_process.returncode != 0:
-        click.secho(
-            "Could not fetch your Git username/email, please make sure that `git config` command works.",
-            fg="red",
-        )
-        quit()
-
-    username = username_process.stdout.decode("utf-8").strip("\n")
-    email = email_process.stdout.decode("utf-8").strip("\n")
-    if not username or not email:
-        click.secho("Git username/email not configured properly.", fg="red")
-        quit()
-
-    click.secho(f"Using Git username: {username}", fg="yellow")
-    return username, email
-
-
 @click.group(invoke_without_command=True)
-@click.option("--init", is_flag=True, help="Initialize Notter tool.")
+@click.option("--init", nargs=2, type=str, help="Initialize Notter tool with a username & email.")
 @click.option("--version", is_flag=True, help="Print Notter version.")
 @click.pass_context
-def cli(ctx: Context, init: bool, version: bool) -> None:
+def cli(ctx: Context, init: Tuple[str, str], version: bool) -> None:
     src_path = os.getenv(SRC_PATH_VAR)
     if not src_path:
         click.secho(
-            f"Could not find the source folder. Please export your source \
-                folder as the environment variable: `{SRC_PATH_VAR}`",
+            f"Could not find the source folder.\
+            Please export your source folder as the environment variable: `{SRC_PATH_VAR}`",
             fg="red",
         )
-        quit()
+        sys.exit(1)
 
     # Initialize Notter instance
     notter = Notter()
 
     if version:
         click.echo(f'{pkg_version("notter")}')
         return
 
     if not init:
         notter.load(src_path)
     else:
         # TODO: Do not initialize if the Notter instance is already there
-        username, email = fetch_git_config()
+        username, email = init
         click.secho(f"Initializing Notter with `{src_path}` as source folder.", fg="yellow")
         notter.configure(Path(src_path).resolve())
         notter.set_config(ncons.USERNAME, username)
         notter.set_config(ncons.EMAIL, email)
 
     controller = NoteController(notter)
     # Add a custom object to context so they are available for other commands
```

### Comparing `notter-0.1.0/src/notter/controller.py` & `notter-0.2.0/src/notter/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+import uuid
 from typing import List
 
 import notter.constants as ncons
 from notter.exceptions import NoteAlreadyExists
 from notter.explorer import LexicalExplorer
 from notter.model import Comment, Content, Note, NoteType, NoteWithContent
 from notter.notter import Notter
 from notter.repository import JsonFileRepository
+from notter.utils import convert_to_local_path
 
 
 class NoteController:
     def __init__(self, notter: Notter):
         self.notter = notter
         self.repository = JsonFileRepository(self.notter)
         self.explorer = LexicalExplorer(self.notter)
 
     def _create_note_with_content(self, filepath: str, line: int, text: str, type: NoteType) -> NoteWithContent:
+        src_folder = self.notter.get_config(ncons.SRC_PATH)
+        filepath = convert_to_local_path(filepath, src_folder)
         username = self.notter.get_config(ncons.USERNAME)
         email = self.notter.get_config(ncons.EMAIL)
         # TODO: Add input validation, max number of characters for each field
-        note = Note(username, email, filepath, line, type)
+        note = Note(str(uuid.uuid4()), username, email, filepath, line, type)
         content = Content(text)
         return NoteWithContent(note, content)
 
     def create(self, filepath: str, line: int, text: str, type: NoteType = NoteType.NOTE) -> None:
         note_with_content = self._create_note_with_content(filepath, line, text, type)
         self.repository.create(note_with_content)
```

### Comparing `notter-0.1.0/src/notter/explorer.py` & `notter-0.2.0/src/notter/explorer.py`

 * *Files identical despite different names*

### Comparing `notter-0.1.0/src/notter/index.py` & `notter-0.2.0/src/notter/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
-from typing import Dict, Optional, Set
+from dataclasses import asdict
+from typing import Any, Dict, Optional, Set
 
 from notter.exceptions import NoteAlreadyExists, NoteNotFound
 from notter.model import Note
 from notter.utils import CustomEncoder, persist_index_after
 
 Line = str
 FilePath = str
-NoteDict = Dict[FilePath, Dict[Line, Note]]
+NoteEntry = Dict[str, Any]
+NoteDict = Dict[FilePath, Dict[Line, NoteEntry]]
 
 
 class NoteIndex:
     def __init__(self, index_path: str) -> None:
         self.idx: NoteDict = {}
         self.idx_path = index_path
 
@@ -30,41 +32,46 @@
 
         note_entry = file_entry.get(line)
         if not note_entry:
             return False
 
         return True
 
-    def fetch(self, filepath: str, line: str) -> Optional[Note]:
+    def fetch(self, filepath: str, line: str) -> Note:
         note_exists = self.seek(filepath, line)
         if not note_exists:
             raise NoteNotFound
 
-        return self.idx[filepath][line]
+        note_dict = Note(**self.idx[filepath][line])
+        return note_dict
 
     def summarize(self) -> Set[str]:
         entry_set: Set[str] = set()
         for filepath, note_dict in self.idx.items():
             for line in note_dict.keys():
                 entry_set.add(f"{filepath}:{line}")
 
         return entry_set
 
     @persist_index_after
     def store(self, note: Note, update: bool = False) -> None:
-        note_exists = self.seek(note.filepath, str(note.line))
+        note_exists: bool = self.seek(note.filepath, str(note.line))
         if not update and note_exists:
             raise NoteAlreadyExists
 
         self.idx[note.filepath] = self.idx.get(note.filepath, {})
-        self.idx[note.filepath][str(note.line)] = note
+        self.idx[note.filepath][str(note.line)] = asdict(note)
 
     @persist_index_after
     def clean(self, filepath: str, line: str) -> Optional[Note]:
-        note = self.fetch(filepath, line)
+        try:
+            note: Note = self.fetch(filepath, line)
+        except NoteNotFound:
+            return None
+
         file_entry = self.idx[filepath]
         file_entry.pop(line)
 
         # Get rid of file entry if it has no keys inside
         if not file_entry:
             self.idx.pop(filepath)
```

### Comparing `notter-0.1.0/src/notter/model.py` & `notter-0.2.0/src/notter/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import uuid
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import Optional
 
 
 class NoteType(str, Enum):
     NOTE = "NOTE"
     TODO = "TODO"
 
 
 # TODO: Add input validation, max number of characters for each field
 @dataclass
 class Note:
+    id: str
     username: str
     email: str
     filepath: str
     line: int
     type: NoteType = NoteType.NOTE
-    id: str = str(uuid.uuid4())
     created_at: Optional[str] = datetime.now().isoformat()
     updated_at: Optional[str] = datetime.now().isoformat()
 
 
 @dataclass
 class Content:
     text: str
```

### Comparing `notter-0.1.0/src/notter/notter.py` & `notter-0.2.0/src/notter/notter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from pathlib import Path
 from shutil import rmtree
 from typing import Any, Dict
 
 import click
 
 import notter.constants as ncons
@@ -12,39 +13,38 @@
     def __init__(self) -> None:
         self.config: Dict[str, Any] = {}
         self.config[ncons.INITIALIZED_FLAG] = False
         self.config[ncons.IDX_INITIALIZED_FLAG] = False
 
     @persist_config_after
     def configure(self, src_folder: Path) -> None:
-        self.path = src_folder.parent / ".notter"
-        self.config[ncons.CONFIG_PATH] = str(self.path / ncons.CONFIG_FILENAME)
+        path = src_folder.parent / ".notter"
+        self.config[ncons.CONFIG_PATH] = str(path / ncons.CONFIG_FILENAME)
         self.config[ncons.SRC_PATH] = str(src_folder)
-        self.config[ncons.PATH] = str(self.path)
-        self.config[ncons.NOTES_PATH] = str(self.path / ncons.NOTES_DIRNAME)
+        self.config[ncons.PATH] = str(path)
+        self.config[ncons.NOTES_PATH] = str(path / ncons.NOTES_DIRNAME)
         self.init_notter_folders()
 
     def init_notter_folders(self) -> None:
         if self.get_config(ncons.INITIALIZED_FLAG):
-            click.secho(f"Notter folders found at location: {self.path}", fg="red")
+            click.secho(f"Notter folders found at location: {self.config[ncons.PATH]}", fg="red")
         else:
-            click.secho(f"Creating Notter folders at location: {self.path}", fg="yellow")
+            click.secho(f"Creating Notter folders at location: {self.config[ncons.PATH]}", fg="yellow")
             Path(self.get_config(ncons.PATH)).mkdir(parents=True, exist_ok=True)
             Path(self.get_config(ncons.NOTES_PATH)).mkdir(parents=True, exist_ok=True)
             self.set_config(ncons.INITIALIZED_FLAG, True)
 
     def load(self, src_folder: str) -> None:
         src_path = Path(src_folder).resolve()
-        parent_path = src_path.parent
-        notter_path = parent_path / ".notter"
+        notter_path = src_path.parent / ".notter"
         notter_config_file = str(notter_path / ncons.CONFIG_FILENAME)
         loaded_config = load_config(notter_config_file)
         if not loaded_config:
             click.secho("Could not load Notter configuration", fg="red")
-            quit()
+            sys.exit()
 
         self.config = loaded_config
 
     def destroy(self) -> None:
         if not self.get_config(ncons.INITIALIZED_FLAG):
             click.secho("No Notter instance is found, nothing to delete", fg="red")
         else:
```

### Comparing `notter-0.1.0/src/notter/repository.py` & `notter-0.2.0/src/notter/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import datetime
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 import notter.constants as ncons
 from notter.exceptions import NotterException
 from notter.index import NoteIndex
 from notter.model import Comment, Content, Note, NoteWithContent
 from notter.notter import Notter
+from notter.utils import convert_to_local_path
 
 
 class BaseRepository:
     def __init__(self, notter: Notter) -> None:
         raise NotImplementedError
 
     def create(self, note_with_content: NoteWithContent) -> None:
@@ -48,16 +49,16 @@
         # Update the index
         self.note_index.store(note_with_content.note)
         # Write note content to a file
         with open(self._get_note_content_path(note_with_content.note.id), "w") as note_file:
             note_file.write(note_with_content.content.text)
 
     def read(self, filepath: str, line: int) -> NoteWithContent:
-        entry = self.note_index.fetch(filepath, str(line))
-        note = Note(**entry.__dict__)
+        note: Note = self.note_index.fetch(filepath, str(line))
+
         with open(self._get_note_content_path(note.id), "r") as note_file:
             text = note_file.read()
 
         content = Content(text)
         return NoteWithContent(note, content)
 
     def update(self, filepath: str, line: int, note_with_content: NoteWithContent) -> None:
@@ -76,24 +77,27 @@
         # Write note content to a file
         with open(self._get_note_content_path(existing_note.note.id), "w") as note_file:
             note_file.write(existing_note.content.text)
 
     def delete(self, filepath: str, line: int) -> None:
         # TODO: Make these two operations atomic
         # Update the index
-        entry = self.note_index.clean(filepath, str(line))
-        note = Note(**entry)
+        note: Optional[Note] = self.note_index.clean(filepath, str(line))
+        if not note:
+            return
+
         note_path = self._get_note_content_path(note.id)
         # Remove note content
-        Path(note_path).unlink()
+        Path(note_path).unlink(missing_ok=True)
 
     def prune(self, comments: List[Comment]) -> List[str]:
         comments_set = set()
         for comment in comments:
-            comments_set.add(f"{comment.filepath}:{comment.line}")
+            filepath = convert_to_local_path(comment.filepath, self.notter.get_config(ncons.SRC_PATH))
+            comments_set.add(f"{filepath}:{comment.line}")
 
         entry_set = self.note_index.summarize()
         items_to_prune = list(entry_set.difference(comments_set))
         for item in items_to_prune:
             filepath, line = item.split(":")
             try:
                 self.delete(filepath, int(line))
```

### Comparing `notter-0.1.0/src/notter.egg-info/SOURCES.txt` & `notter-0.2.0/src/notter.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 .gitignore
 LICENSE
 Makefile
 README.md
+install.py
 pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/tests.yml
+.vscode/launch.json
 src/notter/__init__.py
 src/notter/cli.py
 src/notter/constants.py
 src/notter/context.py
 src/notter/controller.py
 src/notter/exceptions.py
 src/notter/explorer.py
@@ -20,9 +23,15 @@
 src/notter.egg-info/PKG-INFO
 src/notter.egg-info/SOURCES.txt
 src/notter.egg-info/dependency_links.txt
 src/notter.egg-info/entry_points.txt
 src/notter.egg-info/requires.txt
 src/notter.egg-info/top_level.txt
 tests/__init__.py
+tests/conftest.py
 tests/notter/__init__.py
-tests/notter/test_cli.py
+tests/notter/test_cli.py
+tests/notter/test_controller.py
+tests/notter/test_index.py
+tests/notter/test_notter.py
+tests/notter/test_repository.py
+tests/notter/test_utils.py
```

